# Comparing `tmp/timelineomat-0.1.1.tar.gz` & `tmp/timelineomat-0.1.3.tar.gz`

## Comparing `timelineomat-0.1.1.tar` & `timelineomat-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 timelineomat-0.1.1/timelineomat.py
--rw-r--r--   0        0        0     5966 2020-02-02 00:00:00.000000 timelineomat-0.1.1/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.1.1/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.1.1/LICENSE
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 timelineomat-0.1.1/README.md
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 timelineomat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 timelineomat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 timelineomat-0.1.3/timelineomat.py
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 timelineomat-0.1.3/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.1.3/LICENSE
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 timelineomat-0.1.3/README.md
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 timelineomat-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 timelineomat-0.1.3/PKG-INFO
```

### Comparing `timelineomat-0.1.1/timelineomat.py` & `timelineomat-0.1.3/timelineomat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 __all__ = [
     "streamline_event_times",
     "streamline_event",
     "TimelineOMat",
     "SkipEvent",
 ]
 
-from itertools import chain
-from typing import Any, Union, Optional
 from collections.abc import Callable
-from datetime import datetime as dt, timezone as tz
-from collections import namedtuple
+from datetime import datetime as dt
+from datetime import timezone as tz
+from itertools import chain
+from typing import Any, NamedTuple, Optional, Union
 
 ExtractionResult = Union[dt, float, int]
 CallableExtractor = Callable[[Any], ExtractionResult]
 Extractor = Union[str, CallableExtractor]
 CallableSetter = Callable[[Any, dt], None]
 Setter = Union[str, CallableSetter]
 
 
-class SkipEvent(Exception):
+class SkipEvent(BaseException):
     pass
 
 
-class NoCallAllowed(Exception):
+class NoCallAllowed(BaseException):
     pass
 
 
-EventResult = namedtuple("EventResult", ("start", "stop"))
+class EventResult(NamedTuple):
+    start: dt
+    stop: dt
 
 
 def create_extractor(extractor: Extractor) -> CallableExtractor:
     if not isinstance(extractor, str):
         return extractor
 
     def _extractor(event: Any) -> ExtractionResult:
         try:
             if isinstance(event, dict):
                 return event[extractor]
-            else:
-                return getattr(event, extractor)
+            return getattr(event, extractor)
         except (KeyError, AttributeError):
-            raise SkipEvent()
+            raise SkipEvent from None
 
     return _extractor
 
 
 def create_setter(
-    setter: Setter, disallow_call=False, disallow_call_instant=False
+    setter: Setter,
+    *,
+    disallow_call: bool = False,
+    disallow_call_instant: bool = False,
 ) -> CallableSetter:
     if not isinstance(setter, str):
         if disallow_call_instant:
-            raise NoCallAllowed()
+            raise NoCallAllowed
         if disallow_call:
 
-            def _setter(event: Any, value: dt) -> ExtractionResult:
-                raise NoCallAllowed()
+            def _setter(event: Any, value: dt) -> ExtractionResult:  # noqa: RET505
+                raise NoCallAllowed
 
             return _setter
         return setter
 
     def _setter(event: Any, value: dt) -> None:
         if isinstance(event, dict):
             event[setter] = value
         else:
-            return setattr(event, setter, value)
+            setattr(event, setter, value)
 
     return _setter
 
 
 def handle_result(
     result: ExtractionResult, fallback_timezone: Optional[tz] = None
 ) -> Optional[dt]:
     if isinstance(result, dt):
         if fallback_timezone and not result.tzinfo:
             result = result.replace(tzinfo=fallback_timezone)
         return result
-    elif isinstance(result, (int, float)):
+    elif isinstance(result, (int, float)):  # type: ignore
         return dt.fromtimestamp(result, fallback_timezone)
     else:
-        raise ValueError("not supported type: %s" % type(result))
+        raise TypeError(f"not supported type: {type(result)}")
 
 
 def streamline_event_times(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
@@ -93,36 +97,38 @@
     stop_extractor = create_extractor(stop_extractor)
     start = handle_result(
         start_extractor(event), fallback_timezone=fallback_timezone
     )
     stop = handle_result(
         stop_extractor(event), fallback_timezone=fallback_timezone
     )
-    for ev in chain(timelines):
+    if stop <= start:
+        raise SkipEvent
+    for ev in chain.from_iterable(timelines):
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
         if ev_stop <= ev_start:
             continue
-        if ev_start < start and ev_stop > start:
-            if ev_stop > stop:
-                raise SkipEvent()
+        if ev_start <= start and ev_stop >= stop:
+            raise SkipEvent
+        if ev_start <= start and ev_stop > start:
             start = ev_stop
-        if ev_start < stop and ev_stop > stop:
+        if ev_start < stop and ev_stop >= stop:
             stop = ev_start
         if stop <= start:
-            raise SkipEvent()
+            raise SkipEvent
     return EventResult(start=start, stop=stop)
 
 
 def streamline_event(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
@@ -139,15 +145,15 @@
         )
     if stop_setter is not None:
         stop_setter = create_setter(stop_setter)
     else:
         stop_setter = create_setter(stop_extractor, disallow_call_instant=True)
     result = streamline_event_times(
         event,
-        chain(timelines),
+        chain.from_iterable(timelines),
         start_extractor=start_extractor,
         stop_extractor=stop_extractor,
         **kwargs,
     )
     start_setter(event, result.start)
     stop_setter(event, result.stop)
 
@@ -180,21 +186,21 @@
     def streamline_event_times(
         self,
         event: Any,
         *timelines,
     ) -> EventResult:
         return streamline_event_times(
             event,
-            chain(timelines),
+            chain.from_iterable(timelines),
             start_extractor=self.start_extractor,
             stop_extractor=self.stop_extractor,
             filter_fn=self.filter_fn,
             fallback_timezone=self.fallback_timezone,
         )
 
     def streamline_event(self, event: Any, *timelines, **kwargs) -> None:
         result = self.streamline_event_times(
             event,
-            chain(timelines),
+            chain.from_iterable(timelines),
         )
         self.start_setter(event, result.start)
         self.stop_setter(event, result.stop)
```

### Comparing `timelineomat-0.1.1/tests/test_basics.py` & `timelineomat-0.1.3/tests/test_basics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,189 +1,200 @@
-from unittest import TestCase
+import contextlib
 from dataclasses import dataclass
 from datetime import datetime as dt
-import timelineomat
+from datetime import timedelta as td
+
+import pytest
 from faker import Faker
 
+import timelineomat
+
 
 @dataclass
 class Event1:
     start: dt
     stop: dt
 
 
 @dataclass
 class Event2:
     begin: dt
     end: dt
 
 
-class BasicTests(TestCase):
-    def _generate_event_series(self, _type, _variant):
-        faker = Faker()
-        ts_start = faker.past_datetime(
-            "-200d",
-        )
-        ts_stop = faker.past_datetime(
-            "-200d",
-        )
-        events = []
-        for i in range(2000):
-            while ts_stop < ts_start:
-                ts_stop += faker.time_delta("+2d")
-            if _variant == 1:
-                events.append(_type(start=ts_start, stop=ts_stop))
-            else:
-                events.append(_type(begin=ts_start, end=ts_stop))
-            ts_start += faker.time_delta("+2d")
-        return events
-
-    def test_event1_direct(self):
-        events = self._generate_event_series(Event1, 1)
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    timelineomat.streamline_event(ev, events_finished)
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event.stop, ev.start)
-            last_event = ev
-
-    def test_event2_direct(self):
-        events = self._generate_event_series(Event2, 2)
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    timelineomat.streamline_event(
-                        ev,
-                        events_finished,
-                        start_extractor="begin",
-                        stop_extractor="end",
-                    )
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event.end, ev.begin)
-            last_event = ev
-
-    def test_dict1_direct(self):
-        events = self._generate_event_series(dict, 1)
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    timelineomat.streamline_event(
-                        ev,
-                        events_finished,
-                    )
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event["start"], ev["stop"])
-            last_event = ev
-
-    def test_dict2_direct(self):
-        events = self._generate_event_series(dict, 2)
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    timelineomat.streamline_event(
-                        ev,
-                        events_finished,
-                        start_extractor="begin",
-                        stop_extractor="end",
-                    )
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event["end"], ev["begin"])
-            last_event = ev
-
-    def test_event1_timelineomat(self):
-        events = self._generate_event_series(Event1, 1)
-        events_finished = []
-        tm = timelineomat.TimelineOMat()
-        for ev in events:
-            try:
-                events_finished.append(tm.streamline_event(ev, events_finished))
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event.stop, ev.start)
-            last_event = ev
-
-    def test_event2_timelineomat(self):
-        events = self._generate_event_series(Event2, 2)
-        events_finished = []
-        tm = timelineomat.TimelineOMat(
-            start_extractor="begin", stop_extractor="end"
+def _generate_event_series(_type, _variant):
+    faker = Faker()
+    ts_start = faker.past_datetime(
+        "-200d",
+    )
+    ts_stop = faker.past_datetime(
+        "-200d",
+    )
+    events = []
+    for _i in range(1000):
+        while ts_stop < ts_start:
+            ts_stop += td(hours=faker.random_int(1, 48))
+        if _variant == 1:
+            events.append(_type(start=ts_start, stop=ts_stop))
+        else:
+            events.append(_type(begin=ts_start, end=ts_stop))
+        ts_start += td(hours=faker.random_int(1, 48))
+    return events
+
+
+def test_event1_direct():
+    events = _generate_event_series(Event1, 1)
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                timelineomat.streamline_event(ev, events_finished)
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event.stop <= ev.start
+        last_event = ev
+
+
+def test_event2_direct():
+    events = _generate_event_series(Event2, 2)
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                timelineomat.streamline_event(
+                    ev,
+                    events_finished,
+                    start_extractor="begin",
+                    stop_extractor="end",
+                )
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event.end <= ev.begin
+        last_event = ev
+
+
+def test_dict1_direct():
+    events = _generate_event_series(dict, 1)
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                timelineomat.streamline_event(
+                    ev,
+                    events_finished,
+                )
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event["start"] <= ev["stop"]
+        last_event = ev
+
+
+def test_dict2_direct():
+    events = _generate_event_series(dict, 2)
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                timelineomat.streamline_event(
+                    ev,
+                    events_finished,
+                    start_extractor="begin",
+                    stop_extractor="end",
+                )
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event["end"] <= ev["begin"]
+        last_event = ev
+
+
+def test_event1_timelineomat():
+    events = _generate_event_series(Event1, 1)
+    events_finished = []
+    tm = timelineomat.TimelineOMat()
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(tm.streamline_event(ev, events_finished))
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event.stop <= ev.start
+        last_event = ev
+
+
+def test_event2_timelineomat():
+    events = _generate_event_series(Event2, 2)
+    events_finished = []
+    tm = timelineomat.TimelineOMat(
+        start_extractor="begin", stop_extractor="end"
+    )
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(tm.streamline_event(ev, events_finished))
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event.end <= ev.begin
+        last_event = ev
+
+
+def test_dict1_timelineomat():
+    events = _generate_event_series(dict, 1)
+    tm = timelineomat.TimelineOMat()
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                tm.streamline_event(
+                    ev,
+                    events_finished,
+                )
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event["start"] <= ev["stop"]
+        last_event = ev
+
+
+def test_dict2_timelineomat():
+    events = _generate_event_series(dict, 2)
+    tm = timelineomat.TimelineOMat(
+        start_extractor="begin", stop_extractor="end"
+    )
+    events_finished = []
+    for ev in events:
+        with contextlib.suppress(timelineomat.SkipEvent):
+            events_finished.append(
+                tm.streamline_event(
+                    ev,
+                    events_finished,
+                )
+            )
+    last_event = None
+    for ev in events_finished:
+        if last_event:
+            assert last_event["end"] <= ev["begin"]
+        last_event = ev
+
+
+def test_invalid():
+    events = []
+    with pytest.raises(timelineomat.SkipEvent):
+        timelineomat.streamline_event_times(
+            Event1(start=dt(2024, 3, 2), stop=dt(2024, 2, 1)), events
         )
-        for ev in events:
-            try:
-                events_finished.append(tm.streamline_event(ev, events_finished))
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event.end, ev.begin)
-            last_event = ev
-
-    def test_dict1_direct(self):
-        events = self._generate_event_series(dict, 1)
-        tm = timelineomat.TimelineOMat()
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    tm.streamline_event(
-                        ev,
-                        events_finished,
-                    )
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event["start"], ev["stop"])
-            last_event = ev
-
-    def test_dict2_direct(self):
-        events = self._generate_event_series(dict, 2)
-        tm = timelineomat.TimelineOMat(
-            start_extractor="begin", stop_extractor="end"
+
+
+def test_within():
+    events = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 3, 1))]
+    with pytest.raises(timelineomat.SkipEvent):
+        timelineomat.streamline_event_times(
+            Event1(start=dt(2024, 1, 2), stop=dt(2024, 2, 1)), events
         )
-        events_finished = []
-        for ev in events:
-            try:
-                events_finished.append(
-                    tm.streamline_event(
-                        ev,
-                        events_finished,
-                    )
-                )
-            except timelineomat.SkipEvent:
-                print(ev)
-        last_event = None
-        for ev in events_finished:
-            if last_event:
-                self.assertLessEqual(last_event["end"], ev["begin"])
-            last_event = ev
```

### Comparing `timelineomat-0.1.1/.gitignore` & `timelineomat-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.1.1/LICENSE` & `timelineomat-0.1.3/LICENSE`

 * *Files identical despite different names*

