# Comparing `tmp/timelineomat-0.1.0.tar.gz` & `tmp/timelineomat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timelineomat-0.1.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `timelineomat-0.1.0.tar` & `timelineomat-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-05-22 09:54:50.881221 timelineomat-0.1.0/LICENSE
--rw-r--r--   0        0        0      208 2024-05-22 09:53:00.781420 timelineomat-0.1.0/README.md
--rw-r--r--   0        0        0      275 2024-05-22 08:50:24.305367 timelineomat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5869 2024-05-22 09:48:54.699437 timelineomat-0.1.0/timelineomat.py
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 timelineomat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 timelineomat-0.1.1/timelineomat.py
+-rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 timelineomat-0.1.1/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.1.1/LICENSE
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 timelineomat-0.1.1/README.md
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 timelineomat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 timelineomat-0.1.1/PKG-INFO
```

### Comparing `timelineomat-0.1.0/LICENSE` & `timelineomat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.1.0/timelineomat.py` & `timelineomat-0.1.1/timelineomat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,13 @@
-__all__ = ["streamline_event_times", "streamline_event", "TimelineOMat", "SkipEvent"]
+__all__ = [
+    "streamline_event_times",
+    "streamline_event",
+    "TimelineOMat",
+    "SkipEvent",
+]
 
 from itertools import chain
 from typing import Any, Union, Optional
 from collections.abc import Callable
 from datetime import datetime as dt, timezone as tz
 from collections import namedtuple
 
@@ -82,28 +87,34 @@
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[Callable[[Any], bool]] = None,
     fallback_timezone: Optional[tz] = None,
 ) -> EventResult:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
-    start = handle_result(start_extractor(event), fallback_timezone=fallback_timezone)
-    stop = handle_result(stop_extractor(event), fallback_timezone=fallback_timezone)
+    start = handle_result(
+        start_extractor(event), fallback_timezone=fallback_timezone
+    )
+    stop = handle_result(
+        stop_extractor(event), fallback_timezone=fallback_timezone
+    )
     for ev in chain(timelines):
         if filter_fn and not filter_fn(ev):
             continue
         try:
             ev_start = handle_result(
                 start_extractor(ev), fallback_timezone=fallback_timezone
             )
             ev_stop = handle_result(
                 stop_extractor(ev), fallback_timezone=fallback_timezone
             )
         except SkipEvent:
             continue
+        if ev_stop <= ev_start:
+            continue
         if ev_start < start and ev_stop > start:
             if ev_stop > stop:
                 raise SkipEvent()
             start = ev_stop
         if ev_start < stop and ev_stop > stop:
             stop = ev_start
         if stop <= start:
@@ -119,15 +130,17 @@
     start_setter: Optional[Setter] = None,
     stop_setter: Optional[Setter] = None,
     **kwargs,
 ) -> None:
     if start_setter is not None:
         start_setter = create_setter(start_setter)
     else:
-        start_setter = create_setter(start_extractor, disallow_call_instant=True)
+        start_setter = create_setter(
+            start_extractor, disallow_call_instant=True
+        )
     if stop_setter is not None:
         stop_setter = create_setter(stop_setter)
     else:
         stop_setter = create_setter(stop_extractor, disallow_call_instant=True)
     result = streamline_event_times(
         event,
         chain(timelines),
@@ -152,15 +165,17 @@
         self.start_extractor = create_extractor(start_extractor)
         self.stop_extractor = create_extractor(stop_extractor)
         self.filter_fn = filter_fn
         self.fallback_timezone = fallback_timezone
         if start_setter is not None:
             self.start_setter = create_setter(start_setter)
         else:
-            self.start_setter = create_setter(start_extractor, disallow_call=True)
+            self.start_setter = create_setter(
+                start_extractor, disallow_call=True
+            )
         if stop_setter is not None:
             self.stop_setter = create_setter(stop_setter)
         else:
             self.stop_setter = create_setter(stop_extractor, disallow_call=True)
 
     def streamline_event_times(
         self,
```

