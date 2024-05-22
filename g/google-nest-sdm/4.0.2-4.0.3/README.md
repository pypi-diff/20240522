# Comparing `tmp/google_nest_sdm-4.0.2.tar.gz` & `tmp/google_nest_sdm-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_nest_sdm-4.0.2.tar", last modified: Tue May 21 05:58:04 2024, max compression
+gzip compressed data, was "google_nest_sdm-4.0.3.tar", last modified: Wed May 22 14:20:19 2024, max compression
```

## Comparing `google_nest_sdm-4.0.2.tar` & `google_nest_sdm-4.0.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:04.984125 google_nest_sdm-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-21 05:58:04.984125 google_nest_sdm-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:04.980125 google_nest_sdm-4.0.2/google_nest_sdm/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/google_nest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22919 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/google_nest_sdm/transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:04.984125 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 05:58:04.000000 google_nest_sdm-4.0.2/google_nest_sdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-21 05:58:04.988125 google_nest_sdm-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:04.984125 google_nest_sdm-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_camera_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    23950 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_device_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_device_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_doorbell_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_event_media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_google_nest_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_google_nest_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_thermostat_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-21 05:58:00.000000 google_nest_sdm-4.0.2/tests/test_transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:19.634416 google_nest_sdm-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-22 14:20:19.634416 google_nest_sdm-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:19.630416 google_nest_sdm-4.0.3/google_nest_sdm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12499 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28495 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12166 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/google_nest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22919 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/google_nest_sdm/transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:19.630416 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 14:20:19.000000 google_nest_sdm-4.0.3/google_nest_sdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-22 14:20:19.634416 google_nest_sdm-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:20:19.630416 google_nest_sdm-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15798 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_camera_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26647 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_device_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_device_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_doorbell_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19502 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67768 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_event_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10670 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_google_nest_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28764 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_google_nest_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_thermostat_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-22 14:20:15.000000 google_nest_sdm-4.0.3/tests/test_transcoder.py
```

### Comparing `google_nest_sdm-4.0.2/LICENSE` & `google_nest_sdm-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/PKG-INFO` & `google_nest_sdm-4.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 4.0.2
+Version: 4.0.3
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-4.0.2/README.md` & `google_nest_sdm-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/__init__.py` & `google_nest_sdm-4.0.3/google_nest_sdm/__init__.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/auth.py` & `google_nest_sdm-4.0.3/google_nest_sdm/auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/camera_traits.py` & `google_nest_sdm-4.0.3/google_nest_sdm/camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/device.py` & `google_nest_sdm-4.0.3/google_nest_sdm/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A device from the Smart Device Management API."""
 
 from __future__ import annotations
 
 import datetime
 import logging
 from typing import Any, Awaitable, Callable
-from dataclasses import dataclass, field, fields
+from dataclasses import dataclass, field, fields, asdict
 
 from mashumaro import field_options, DataClassDictMixin
 from mashumaro.config import BaseConfig
 from mashumaro.types import SerializationStrategy
 
 from . import camera_traits, device_traits, doorbell_traits, thermostat_traits
 from .auth import AbstractAuth
@@ -302,15 +302,15 @@
                 _LOGGER.debug("Discarding stale update (%s)", event_message.timestamp)
                 continue
 
             # Only merge updates into existing models, updating the existing
             # fields present in the update trait
             if not (existing := getattr(self, trait_field.name)):
                 continue
-            for k, v in new.to_dict().items():
+            for k, v in asdict(new).items():
                 if v is not None:
                     setattr(existing, k, v)
             self._trait_event_ts[trait_field.name] = event_message.timestamp
 
     @property
     def event_media_manager(self) -> EventMediaManager:
         return self._event_media_manager
```

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/device_manager.py` & `google_nest_sdm-4.0.3/google_nest_sdm/device_manager.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/device_traits.py` & `google_nest_sdm-4.0.3/google_nest_sdm/device_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/diagnostics.py` & `google_nest_sdm-4.0.3/google_nest_sdm/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,16 +83,16 @@
 def get_diagnostics() -> dict[str, Any]:
     """Produce diagnostics information for the library."""
     return {k: v.as_dict() for (k, v) in MAP.items() if v.as_dict()}
 
 
 REDACT_KEYS = {
     "name",
-    "customName",
-    "displayName",
+    "custom_name",
+    "display_name",
     "parent",
     "assignee",
     "subject",
     "object",
     "userId",
     "resourceGroup",
     "eventId",
```

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/doorbell_traits.py` & `google_nest_sdm-4.0.3/google_nest_sdm/doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/event.py` & `google_nest_sdm-4.0.3/google_nest_sdm/event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/event_media.py` & `google_nest_sdm-4.0.3/google_nest_sdm/event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/exceptions.py` & `google_nest_sdm-4.0.3/google_nest_sdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/google_nest.py` & `google_nest_sdm-4.0.3/google_nest_sdm/google_nest.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/google_nest_api.py` & `google_nest_sdm-4.0.3/google_nest_sdm/google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/google_nest_subscriber.py` & `google_nest_sdm-4.0.3/google_nest_sdm/google_nest_subscriber.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/model.py` & `google_nest_sdm-4.0.3/google_nest_sdm/model.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/registry.py` & `google_nest_sdm-4.0.3/google_nest_sdm/registry.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/structure.py` & `google_nest_sdm-4.0.3/google_nest_sdm/structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/thermostat_traits.py` & `google_nest_sdm-4.0.3/google_nest_sdm/thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/traits.py` & `google_nest_sdm-4.0.3/google_nest_sdm/traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm/transcoder.py` & `google_nest_sdm-4.0.3/google_nest_sdm/transcoder.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm.egg-info/PKG-INFO` & `google_nest_sdm-4.0.3/google_nest_sdm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google_nest_sdm
-Version: 4.0.2
+Version: 4.0.3
 Summary: Library for the Google Nest SDM API
 Home-page: https://github.com/allenporter/python-google_nest_sdm
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
```

### Comparing `google_nest_sdm-4.0.2/google_nest_sdm.egg-info/SOURCES.txt` & `google_nest_sdm-4.0.3/google_nest_sdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/pyproject.toml` & `google_nest_sdm-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/setup.cfg` & `google_nest_sdm-4.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = google_nest_sdm
-version = 4.0.2
+version = 4.0.3
 description = Library for the Google Nest SDM API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/python-google_nest_sdm
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
```

### Comparing `google_nest_sdm-4.0.2/tests/test_auth.py` & `google_nest_sdm-4.0.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_camera_traits.py` & `google_nest_sdm-4.0.3/tests/test_camera_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_device.py` & `google_nest_sdm-4.0.3/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_device_manager.py` & `google_nest_sdm-4.0.3/tests/test_device_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -696,7 +696,84 @@
                     },
                 },
                 "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
             }
         )
     )
     assert callback.invoked
+
+
+async def test_update_with_new_trait(
+    fake_device: Callable[[Dict[str, Any]], Device],
+    fake_event_message: Callable[[Dict[str, Any]], EventMessage],
+) -> None:
+    mgr = DeviceManager()
+    mgr.add_device(
+        fake_device(
+            {
+                "name": "my/device/name1",
+                "type": "sdm.devices.types.SomeDeviceType",
+                "traits": {
+                    "sdm.devices.traits.ThermostatHvac": {"status": "OFF"},
+                    "sdm.devices.traits.ThermostatMode": {
+                        "availableModes": ["HEAT", "COOL", "HEATCOOL", "OFF"],
+                        "mode": "OFF",
+                    },
+                },
+            }
+        )
+    )
+    assert 1 == len(mgr.devices)
+    device = mgr.devices["my/device/name1"]
+    assert device.thermostat_hvac
+    assert device.thermostat_hvac.status == "OFF"
+    assert device.thermostat_mode
+    assert device.thermostat_mode.mode == "OFF"
+
+    # Heat is enabled
+    await mgr.async_handle_event(
+        fake_event_message(
+            {
+                "eventId": "0120ecc7-3b57-4eb4-9941-91609f189fb4",
+                "timestamp": "2019-01-01T00:00:01Z",
+                "resourceUpdate": {
+                    "name": "my/device/name1",
+                    "traits": {
+                        "sdm.devices.traits.ThermostatMode": {
+                            "availableModes": ["HEAT", "COOL", "HEATCOOL", "OFF"],
+                            "mode": "HEAT",
+                        },
+                    },
+                },
+                "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+            }
+        )
+    )
+    device = mgr.devices["my/device/name1"]
+    assert device.thermostat_hvac
+    assert device.thermostat_hvac.status == "OFF"
+    assert device.thermostat_mode
+    assert device.thermostat_mode.mode == "HEAT"
+
+    # Heating has started.
+    await mgr.async_handle_event(
+        fake_event_message(
+            {
+                "eventId": "0120ecc7-3b57-4eb4-9941-91609f189fb4",
+                "timestamp": "2019-01-01T00:00:01Z",
+                "resourceUpdate": {
+                    "name": "my/device/name1",
+                    "traits": {
+                        "sdm.devices.traits.ThermostatHvac": {
+                            "status": "HEATING",
+                        },
+                    },
+                },
+                "userId": "AVPHwEuBfnPOnTqzVFT4IONX2Qqhu9EJ4ubO-bNnQ-yi",
+            }
+        )
+    )
+    device = mgr.devices["my/device/name1"]
+    assert device.thermostat_hvac
+    assert device.thermostat_hvac.status == "HEATING"
+    assert device.thermostat_mode
+    assert device.thermostat_mode.mode == "HEAT"
```

### Comparing `google_nest_sdm-4.0.2/tests/test_device_traits.py` & `google_nest_sdm-4.0.3/tests/test_device_traits.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import datetime
 from typing import Any, Callable, Dict
 
 import pytest
 
 from google_nest_sdm.device import Device
 
+from .conftest import assert_diagnostics
+
 
 def test_info_traits(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
     device = fake_device(
         {
             "name": "my/device/name",
             "traits": {
                 "sdm.devices.traits.Info": {
@@ -21,14 +23,31 @@
     )
     assert "my/device/name" == device.name
     assert "sdm.devices.traits.Info" in device.traits
     trait = device.traits["sdm.devices.traits.Info"]
     assert "Device Name" == trait.custom_name
 
 
+    assert_diagnostics(
+        device.get_diagnostics(),
+        {
+            "data": {
+                "name": "**REDACTED**",
+                "parentRelations": [],
+                "traits": {
+                    "sdm.devices.traits.Info": {
+                        "custom_name": "**REDACTED**",
+                    }
+                },
+            },
+        },
+    )
+
+
+
 def test_connectivity_traits(fake_device: Callable[[Dict[str, Any]], Device]) -> None:
     device = fake_device(
         {
             "name": "my/device/name",
             "traits": {
                 "sdm.devices.traits.Connectivity": {
                     "status": "OFFLINE",
```

### Comparing `google_nest_sdm-4.0.2/tests/test_doorbell_traits.py` & `google_nest_sdm-4.0.3/tests/test_doorbell_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_event.py` & `google_nest_sdm-4.0.3/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_event_media.py` & `google_nest_sdm-4.0.3/tests/test_event_media.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_google_nest_api.py` & `google_nest_sdm-4.0.3/tests/test_google_nest_api.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_google_nest_subscriber.py` & `google_nest_sdm-4.0.3/tests/test_google_nest_subscriber.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_structure.py` & `google_nest_sdm-4.0.3/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_thermostat_traits.py` & `google_nest_sdm-4.0.3/tests/test_thermostat_traits.py`

 * *Files identical despite different names*

### Comparing `google_nest_sdm-4.0.2/tests/test_transcoder.py` & `google_nest_sdm-4.0.3/tests/test_transcoder.py`

 * *Files identical despite different names*

