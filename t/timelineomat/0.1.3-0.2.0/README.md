# Comparing `tmp/timelineomat-0.1.3.tar.gz` & `tmp/timelineomat-0.2.0.tar.gz`

## Comparing `timelineomat-0.1.3.tar` & `timelineomat-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 timelineomat-0.1.3/timelineomat.py
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 timelineomat-0.1.3/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.1.3/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.1.3/LICENSE
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 timelineomat-0.1.3/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 timelineomat-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 timelineomat-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 timelineomat-0.2.0/timelineomat.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 timelineomat-0.2.0/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 timelineomat-0.2.0/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 timelineomat-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 timelineomat-0.2.0/PKG-INFO
```

### Comparing `timelineomat-0.1.3/timelineomat.py` & `timelineomat-0.2.0/timelineomat.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-__all__ = [
-    "streamline_event_times",
-    "streamline_event",
-    "TimelineOMat",
-    "SkipEvent",
-]
+__all__ = ["streamline_event_times", "streamline_event", "TimelineOMat", "SkipEvent", "NewTimesResult"]
 
 from collections.abc import Callable
 from datetime import datetime as dt
 from datetime import timezone as tz
 from itertools import chain
 from typing import Any, NamedTuple, Optional, Union
 
-ExtractionResult = Union[dt, float, int]
+ExtractionResult = Union[dt, float, int, str]
 CallableExtractor = Callable[[Any], ExtractionResult]
 Extractor = Union[str, CallableExtractor]
 CallableSetter = Callable[[Any, dt], None]
 Setter = Union[str, CallableSetter]
 
 
 class SkipEvent(BaseException):
     pass
 
 
 class NoCallAllowed(BaseException):
     pass
 
 
-class EventResult(NamedTuple):
+class NewTimesResult(NamedTuple):
     start: dt
     stop: dt
 
 
 def create_extractor(extractor: Extractor) -> CallableExtractor:
     if not isinstance(extractor, str):
         return extractor
@@ -68,98 +63,89 @@
             event[setter] = value
         else:
             setattr(event, setter, value)
 
     return _setter
 
 
-def handle_result(
-    result: ExtractionResult, fallback_timezone: Optional[tz] = None
-) -> Optional[dt]:
+def handle_result(result: ExtractionResult, fallback_timezone: Optional[tz] = None) -> Optional[dt]:
     if isinstance(result, dt):
         if fallback_timezone and not result.tzinfo:
             result = result.replace(tzinfo=fallback_timezone)
         return result
-    elif isinstance(result, (int, float)):  # type: ignore
+    elif isinstance(result, (int, float)):
         return dt.fromtimestamp(result, fallback_timezone)
+    elif isinstance(result, str):  # type: ignore
+        return handle_result(dt.fromisoformat(result), fallback_timezone=fallback_timezone)
     else:
         raise TypeError(f"not supported type: {type(result)}")
 
 
 def streamline_event_times(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[Callable[[Any], bool]] = None,
     fallback_timezone: Optional[tz] = None,
-) -> EventResult:
+) -> NewTimesResult:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
-    start = handle_result(
-        start_extractor(event), fallback_timezone=fallback_timezone
-    )
-    stop = handle_result(
-        stop_extractor(event), fallback_timezone=fallback_timezone
-    )
+    start = handle_result(start_extractor(event), fallback_timezone=fallback_timezone)
+    stop = handle_result(stop_extractor(event), fallback_timezone=fallback_timezone)
     if stop <= start:
         raise SkipEvent
     for ev in chain.from_iterable(timelines):
         if filter_fn and not filter_fn(ev):
             continue
         try:
-            ev_start = handle_result(
-                start_extractor(ev), fallback_timezone=fallback_timezone
-            )
-            ev_stop = handle_result(
-                stop_extractor(ev), fallback_timezone=fallback_timezone
-            )
+            ev_start = handle_result(start_extractor(ev), fallback_timezone=fallback_timezone)
+            ev_stop = handle_result(stop_extractor(ev), fallback_timezone=fallback_timezone)
         except SkipEvent:
             continue
         if ev_stop <= ev_start:
             continue
         if ev_start <= start and ev_stop >= stop:
             raise SkipEvent
         if ev_start <= start and ev_stop > start:
             start = ev_stop
         if ev_start < stop and ev_stop >= stop:
             stop = ev_start
         if stop <= start:
             raise SkipEvent
-    return EventResult(start=start, stop=stop)
+    return NewTimesResult(start=start, stop=stop)
 
 
 def streamline_event(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     start_setter: Optional[Setter] = None,
     stop_setter: Optional[Setter] = None,
     **kwargs,
-) -> None:
+) -> Any:
     if start_setter is not None:
         start_setter = create_setter(start_setter)
     else:
-        start_setter = create_setter(
-            start_extractor, disallow_call_instant=True
-        )
+        start_setter = create_setter(start_extractor, disallow_call_instant=True)
     if stop_setter is not None:
         stop_setter = create_setter(stop_setter)
     else:
         stop_setter = create_setter(stop_extractor, disallow_call_instant=True)
     result = streamline_event_times(
         event,
         chain.from_iterable(timelines),
         start_extractor=start_extractor,
         stop_extractor=stop_extractor,
         **kwargs,
     )
     start_setter(event, result.start)
     stop_setter(event, result.stop)
+    return event
 
 
 class TimelineOMat:
     def __init__(
         self,
         start_extractor: Extractor = "start",
         stop_extractor: Extractor = "stop",
@@ -171,36 +157,34 @@
         self.start_extractor = create_extractor(start_extractor)
         self.stop_extractor = create_extractor(stop_extractor)
         self.filter_fn = filter_fn
         self.fallback_timezone = fallback_timezone
         if start_setter is not None:
             self.start_setter = create_setter(start_setter)
         else:
-            self.start_setter = create_setter(
-                start_extractor, disallow_call=True
-            )
+            self.start_setter = create_setter(start_extractor, disallow_call=True)
         if stop_setter is not None:
             self.stop_setter = create_setter(stop_setter)
         else:
             self.stop_setter = create_setter(stop_extractor, disallow_call=True)
 
-    def streamline_event_times(
-        self,
-        event: Any,
-        *timelines,
-    ) -> EventResult:
+    def streamline_event_times(self, event: Any, *timelines, **kwargs) -> NewTimesResult:
         return streamline_event_times(
             event,
             chain.from_iterable(timelines),
-            start_extractor=self.start_extractor,
-            stop_extractor=self.stop_extractor,
-            filter_fn=self.filter_fn,
-            fallback_timezone=self.fallback_timezone,
+            start_extractor=kwargs.get("start_extractor", self.start_extractor),
+            stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
+            filter_fn=kwargs.get("filter_fn", self.filter_fn),
+            fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
         )
 
     def streamline_event(self, event: Any, *timelines, **kwargs) -> None:
-        result = self.streamline_event_times(
+        return streamline_event(
             event,
             chain.from_iterable(timelines),
+            start_extractor=kwargs.get("start_extractor", self.start_extractor),
+            stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
+            filter_fn=kwargs.get("filter_fn", self.filter_fn),
+            fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+            start_setter=kwargs.get("start_setter", self.start_setter),
+            stop_setter=kwargs.get("stop_setter", self.stop_setter),
         )
-        self.start_setter(event, result.start)
-        self.stop_setter(event, result.stop)
```

### Comparing `timelineomat-0.1.3/.gitignore` & `timelineomat-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.1.3/LICENSE` & `timelineomat-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.1.3/pyproject.toml` & `timelineomat-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [project]
 name = "timelineomat"
-version = "0.1.3"
+version = "0.2.0"
 description = ""
 authors = [{name = "Alexander Kaftan", email="devkral@web.de"}]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.ruff]
-line-length = 80
+line-length = 120
 target-version = "py39"
 
 [tool.ruff.lint]
 select = [
     # pycodestyle
     "E",
     # Pyflakes
```

