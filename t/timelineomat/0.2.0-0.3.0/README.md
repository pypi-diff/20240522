# Comparing `tmp/timelineomat-0.2.0.tar.gz` & `tmp/timelineomat-0.3.0.tar.gz`

## Comparing `timelineomat-0.2.0.tar` & `timelineomat-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 timelineomat-0.2.0/timelineomat.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 timelineomat-0.2.0/tests/test_basics.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.2.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.2.0/LICENSE
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 timelineomat-0.2.0/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 timelineomat-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 timelineomat-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     8093 2020-02-02 00:00:00.000000 timelineomat-0.3.0/timelineomat.py
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 timelineomat-0.3.0/tests/test_basics.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 timelineomat-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 timelineomat-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 timelineomat-0.3.0/README.md
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 timelineomat-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 timelineomat-0.3.0/PKG-INFO
```

### Comparing `timelineomat-0.2.0/timelineomat.py` & `timelineomat-0.3.0/timelineomat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__all__ = ["streamline_event_times", "streamline_event", "TimelineOMat", "SkipEvent", "NewTimesResult"]
+__all__ = ["streamline_event_times", "streamline_event", "TimelineOMat", "SkipEvent", "TimeRangeTuple"]
 
 from collections.abc import Callable
 from datetime import datetime as dt
 from datetime import timezone as tz
 from itertools import chain
 from typing import Any, NamedTuple, Optional, Union
 
@@ -17,19 +17,23 @@
     pass
 
 
 class NoCallAllowed(BaseException):
     pass
 
 
-class NewTimesResult(NamedTuple):
+class TimeRangeTuple(NamedTuple):
     start: dt
     stop: dt
 
 
+# old name
+NewTimesResult = TimeRangeTuple
+
+
 def create_extractor(extractor: Extractor) -> CallableExtractor:
     if not isinstance(extractor, str):
         return extractor
 
     def _extractor(event: Any) -> ExtractionResult:
         try:
             if isinstance(event, dict):
@@ -83,15 +87,16 @@
 def streamline_event_times(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
     filter_fn: Optional[Callable[[Any], bool]] = None,
     fallback_timezone: Optional[tz] = None,
-) -> NewTimesResult:
+    **kwargs,
+) -> TimeRangeTuple:
     start_extractor = create_extractor(start_extractor)
     stop_extractor = create_extractor(stop_extractor)
     start = handle_result(start_extractor(event), fallback_timezone=fallback_timezone)
     stop = handle_result(stop_extractor(event), fallback_timezone=fallback_timezone)
     if stop <= start:
         raise SkipEvent
     for ev in chain.from_iterable(timelines):
@@ -108,15 +113,15 @@
             raise SkipEvent
         if ev_start <= start and ev_stop > start:
             start = ev_stop
         if ev_start < stop and ev_stop >= stop:
             stop = ev_start
         if stop <= start:
             raise SkipEvent
-    return NewTimesResult(start=start, stop=stop)
+    return TimeRangeTuple(start=start, stop=stop)
 
 
 def streamline_event(
     event: Any,
     *timelines,
     start_extractor: Extractor = "start",
     stop_extractor: Extractor = "stop",
@@ -140,14 +145,39 @@
         **kwargs,
     )
     start_setter(event, result.start)
     stop_setter(event, result.stop)
     return event
 
 
+def transform_events_to_times(
+    *timelines,
+    start_extractor: Extractor = "start",
+    stop_extractor: Extractor = "stop",
+    filter_fn: Optional[Callable[[Any], bool]] = None,
+    fallback_timezone: Optional[tz] = None,
+    **kwargs,
+) -> list[TimeRangeTuple]:
+    start_extractor = create_extractor(start_extractor)
+    stop_extractor = create_extractor(stop_extractor)
+    transformed = []
+    for ev in chain.from_iterable(timelines):
+        if filter_fn and not filter_fn(ev):
+            continue
+        try:
+            ev_start = handle_result(start_extractor(ev), fallback_timezone=fallback_timezone)
+            ev_stop = handle_result(stop_extractor(ev), fallback_timezone=fallback_timezone)
+        except SkipEvent:
+            continue
+        if ev_stop <= ev_start:
+            continue
+        transformed.append(TimeRangeTuple(start=ev_start, stop=ev_stop))
+    return transformed
+
+
 class TimelineOMat:
     def __init__(
         self,
         start_extractor: Extractor = "start",
         stop_extractor: Extractor = "stop",
         filter_fn: Optional[Callable[[Any], bool]] = None,
         fallback_timezone: Optional[tz] = None,
@@ -163,15 +193,15 @@
         else:
             self.start_setter = create_setter(start_extractor, disallow_call=True)
         if stop_setter is not None:
             self.stop_setter = create_setter(stop_setter)
         else:
             self.stop_setter = create_setter(stop_extractor, disallow_call=True)
 
-    def streamline_event_times(self, event: Any, *timelines, **kwargs) -> NewTimesResult:
+    def streamline_event_times(self, event: Any, *timelines, **kwargs) -> TimeRangeTuple:
         return streamline_event_times(
             event,
             chain.from_iterable(timelines),
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
@@ -184,7 +214,16 @@
             start_extractor=kwargs.get("start_extractor", self.start_extractor),
             stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
             filter_fn=kwargs.get("filter_fn", self.filter_fn),
             fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
             start_setter=kwargs.get("start_setter", self.start_setter),
             stop_setter=kwargs.get("stop_setter", self.stop_setter),
         )
+
+    def transform_events_to_times(self, *timelines, **kwargs) -> list[TimeRangeTuple]:
+        return transform_events_to_times(
+            chain.from_iterable(timelines),
+            start_extractor=kwargs.get("start_extractor", self.start_extractor),
+            stop_extractor=kwargs.get("stop_extractor", self.stop_extractor),
+            filter_fn=kwargs.get("filter_fn", self.filter_fn),
+            fallback_timezone=kwargs.get("fallback_timezone", self.fallback_timezone),
+        )
```

### Comparing `timelineomat-0.2.0/tests/test_basics.py` & `timelineomat-0.3.0/tests/test_basics.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,26 +191,26 @@
         timelineomat.streamline_event_times(Event1(start=dt(2024, 1, 2), stop=dt(2024, 2, 1)), events)
 
 
 def test_result():
     timeline = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
     new_event = Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
     # one time methods
-    assert timelineomat.streamline_event_times(new_event, timeline) == timelineomat.NewTimesResult(
+    assert timelineomat.streamline_event_times(new_event, timeline) == timelineomat.TimeRangeTuple(
         start=dt(2024, 1, 3), stop=dt(2024, 1, 4)
     )
 
 
 def test_result_fallback_utc():
     timeline = [Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event1(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
     new_event = Event1(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
     # one time methods
     assert timelineomat.streamline_event_times(
         new_event, timeline, fallback_timezone=timezone.utc
-    ) == timelineomat.NewTimesResult(
+    ) == timelineomat.TimeRangeTuple(
         start=dt(2024, 1, 3, tzinfo=timezone.utc), stop=dt(2024, 1, 4, tzinfo=timezone.utc)
     )
 
 
 def one_time_overwrite_end(ev):
     if isinstance(ev, dict):
         return ev["end"]
@@ -228,7 +228,13 @@
     assert timeline[-1].stop == dt(2024, 1, 4)
     assert timeline[-1].start == dt(2024, 1, 3)
     timeline.append(
         Event1(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict())
     )
     assert timeline[-1].stop == dt(2024, 1, 5)
     assert timeline[-1].start == dt(2024, 1, 4)
+    assert tm.transform_events_to_times(timeline) == [
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 2), stop=dt(2024, 1, 3)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4)),
+        timelineomat.TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5)),
+    ]
```

### Comparing `timelineomat-0.2.0/.gitignore` & `timelineomat-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timelineomat-0.2.0/LICENSE` & `timelineomat-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timelineomat-0.2.0/README.md` & `timelineomat-0.3.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,38 +8,52 @@
 ## Installation
 ``` sh
 pip install timelineomat
 ```
 
 ## Usage
 
-see Code
+There are 3 different functions which also exist as methods of the TimelineOMat class
+
+- streamline_event_times: checks how to short the given event to fit into the timelines
+- streamline_event: uses streamline_event_times plus setters to update the event and returns event
+- transform_events_to_times: transforms timelines to TimeRangeTuple for e.g. databases
+
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
-from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, NewTimesResult
+from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
 timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # one time methods
 # get intermediate result of new times
-streamline_event_times(new_event, timeline) == NewTimesResult(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
+streamline_event_times(new_event, timeline) == TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
 # update the event
 timeline.append(streamline_event(new_event, timeline))
 
 tm = TimelineOMat()
 # use method instead
-tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == NewTimesResult(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
+tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
+
+# now integrate in django or whatever
+from django.db.models import Q
+
+q = Q()
+# this is not optimized
+for timetuple in tm.transform_events_to_times(timeline):
+    # timetuple is actually a 2 element tuple
+    q |= Q(timepoint__range=timetuple)
 
 ```
 
 
 ## Tricks to integrate in different datastructures
 
 TimelineOMat supports out of the box all kind of dicts as well as objects. It determinates
@@ -86,28 +100,28 @@
     stop: dt
 
 
 timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
 new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 new_event2 = dict(start=dt(2024, 1, 1), end=dt(2024, 1, 5))
 
+tm = TimelineOMat()
 ```
 
 it is possible to extract the data with
 
 ``` python
 
 
 def one_time_overwrite_end(ev):
     if isinstance(ev, dict):
         return ev["end"]
     else:
         return ev.stop
 
-tm = TimelineOMat()
 timeline.append(tm.streamline_event(new_event1, timeline))
 #
 
 timeline.append(Event(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict()))
 ```
 
 
@@ -141,7 +155,19 @@
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # here we generate the setters and extractors only onetime
 tm = TimelineOMat()
 tm.streamline_event_times(new_event, ordered_timeline[-1:])
 #
 
 ```
+
+
+## How to integrate in db systems
+
+DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
+
+An example is in Usage
+
+
+## Changes
+
+0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

### Comparing `timelineomat-0.2.0/PKG-INFO` & `timelineomat-0.3.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 Metadata-Version: 2.3
 Name: timelineomat
-Version: 0.2.0
+Version: 0.3.0
+Summary: Squeeze events into timelines and other timeline manipulations
 Author-email: Alexander Kaftan <devkral@web.de>
 License-Expression: MIT
 License-File: LICENSE
+Keywords: database,event,time,timelines
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # TimelineOMat
 
 This project allows to streamline events in timelines.
 Streamlining is here to fill to adjust the event start and stop times so it fits into the gaps of the timeline and to emit an Exception if this is not possible.
@@ -17,38 +30,52 @@
 ## Installation
 ``` sh
 pip install timelineomat
 ```
 
 ## Usage
 
-see Code
+There are 3 different functions which also exist as methods of the TimelineOMat class
+
+- streamline_event_times: checks how to short the given event to fit into the timelines
+- streamline_event: uses streamline_event_times plus setters to update the event and returns event
+- transform_events_to_times: transforms timelines to TimeRangeTuple for e.g. databases
+
 
 ``` python
 from dataclasses import dataclass
 from datetime import datetime as dt
-from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, NewTimesResult
+from timelineomat import TimelineOMat, streamline_event_times, stream_line_event, TimeRangeTuple
 
 
 @dataclass
 class Event:
     start: dt
     stop: dt
 
 timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # one time methods
 # get intermediate result of new times
-streamline_event_times(new_event, timeline) == NewTimesResult(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
+streamline_event_times(new_event, timeline) == TimeRangeTuple(start=dt(2024, 1, 3), stop=dt(2024, 1, 4))
 # update the event
 timeline.append(streamline_event(new_event, timeline))
 
 tm = TimelineOMat()
 # use method instead
-tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == NewTimesResult(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
+tm.streamline_event_times(Event(start=dt(2024, 1, 1), stop=dt(2024, 1, )), timeline) == TimeRangeTuple(start=dt(2024, 1, 4), stop=dt(2024, 1, 5))
+
+# now integrate in django or whatever
+from django.db.models import Q
+
+q = Q()
+# this is not optimized
+for timetuple in tm.transform_events_to_times(timeline):
+    # timetuple is actually a 2 element tuple
+    q |= Q(timepoint__range=timetuple)
 
 ```
 
 
 ## Tricks to integrate in different datastructures
 
 TimelineOMat supports out of the box all kind of dicts as well as objects. It determinates
@@ -95,28 +122,28 @@
     stop: dt
 
 
 timeline = [Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 2)), Event(start=dt(2024, 1, 2), stop=dt(2024, 1, 3))]
 new_event1 = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 new_event2 = dict(start=dt(2024, 1, 1), end=dt(2024, 1, 5))
 
+tm = TimelineOMat()
 ```
 
 it is possible to extract the data with
 
 ``` python
 
 
 def one_time_overwrite_end(ev):
     if isinstance(ev, dict):
         return ev["end"]
     else:
         return ev.stop
 
-tm = TimelineOMat()
 timeline.append(tm.streamline_event(new_event1, timeline))
 #
 
 timeline.append(Event(**tm.streamline_event_times(new_event2, timeline, stop_extractor=one_time_overwrite_end)._asdict()))
 ```
 
 
@@ -150,7 +177,19 @@
 new_event = Event(start=dt(2024, 1, 1), stop=dt(2024, 1, 4))
 # here we generate the setters and extractors only onetime
 tm = TimelineOMat()
 tm.streamline_event_times(new_event, ordered_timeline[-1:])
 #
 
 ```
+
+
+## How to integrate in db systems
+
+DB Systems like django support range queries, which receives two element tuples. TimelineOMat can convert the timelines into such tuples (TimeRangeTuple doubles as tuple)
+
+An example is in Usage
+
+
+## Changes
+
+0.3.0 rename NewTimesResult to TimeRangeTuple (the old name is still available)
```

