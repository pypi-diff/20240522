# Comparing `tmp/spacetower_fds_sdk-1.0.3.tar.gz` & `tmp/spacetower_fds_sdk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetower_fds_sdk-1.0.3.tar", max compression
+gzip compressed data, was "spacetower_fds_sdk-1.0.4.tar", max compression
```

## Comparing `spacetower_fds_sdk-1.0.3.tar` & `spacetower_fds_sdk-1.0.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      147 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/README.md
--rw-r--r--   0        0        0       46 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/__init__.py
--rw-r--r--   0        0        0    32653 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/client.py
--rw-r--r--   0        0        0      525 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/config.py
--rw-r--r--   0        0        0      474 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/constants.py
--rw-r--r--   0        0        0      121 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/__init__.py
--rw-r--r--   0        0        0     8204 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/_model.py
--rw-r--r--   0        0        0     2448 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/_use_case.py
--rw-r--r--   0        0        0     8962 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/actions.py
--rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/__init__.py
--rw-r--r--   0        0        0     5265 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/configuration.py
--rw-r--r--   0        0        0     5079 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/requests.py
--rw-r--r--   0        0        0    18902 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/result.py
--rw-r--r--   0        0        0     3942 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/use_case.py
--rw-r--r--   0        0        0     2921 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/ground_station.py
--rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/__init__.py
--rw-r--r--   0        0        0     6069 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/result.py
--rw-r--r--   0        0        0     5505 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/strategy.py
--rw-r--r--   0        0        0     3705 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/use_case.py
--rw-r--r--   0        0        0     9777 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/nmea_processor.py
--rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/__init__.py
--rw-r--r--   0        0        0    13945 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/ephemeris.py
--rw-r--r--   0        0        0     3886 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/events.py
--rw-r--r--   0        0        0    23764 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/requests.py
--rw-r--r--   0        0        0    17095 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/result.py
--rw-r--r--   0        0        0    13074 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/use_case.py
--rw-r--r--   0        0        0    15539 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbital_state.py
--rw-r--r--   0        0        0    10771 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbits.py
--rw-r--r--   0        0        0    12996 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/quaternion.py
--rw-r--r--   0        0        0    14728 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/roadmaps.py
--rw-r--r--   0        0        0    25353 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/spacecraft.py
--rw-r--r--   0        0        0    20842 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/telemetry.py
--rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/__init__.py
--rw-r--r--   0        0        0      868 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/result.py
--rw-r--r--   0        0        0     1399 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/use_case.py
--rw-r--r--   0        0        0     8294 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/two_line_element.py
--rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/__init__.py
--rw-r--r--   0        0        0     2214 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/dates.py
--rw-r--r--   0        0        0     1993 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/dict.py
--rw-r--r--   0        0        0      440 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/enum.py
--rw-r--r--   0        0        0     2756 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/frames.py
--rw-r--r--   0        0        0     1803 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/geometry.py
--rw-r--r--   0        0        0      492 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/log.py
--rw-r--r--   0        0        0     1077 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/math.py
--rw-r--r--   0        0        0    13916 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/orbital_mechanics.py
--rw-r--r--   0        0        0      921 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 spacetower_fds_sdk-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      147 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/README.md
+-rw-r--r--   0        0        0       46 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/__init__.py
+-rw-r--r--   0        0        0    32653 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/client.py
+-rw-r--r--   0        0        0      525 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/config.py
+-rw-r--r--   0        0        0      474 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/constants.py
+-rw-r--r--   0        0        0     6266 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/__init__.py
+-rw-r--r--   0        0        0     8122 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/_model.py
+-rw-r--r--   0        0        0     2448 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/_use_case.py
+-rw-r--r--   0        0        0     8962 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/actions.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/determination/__init__.py
+-rw-r--r--   0        0        0     5265 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/determination/configuration.py
+-rw-r--r--   0        0        0     5079 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/determination/requests.py
+-rw-r--r--   0        0        0    18902 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/determination/result.py
+-rw-r--r--   0        0        0     3942 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/determination/use_case.py
+-rw-r--r--   0        0        0     2921 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/ground_station.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/maneuvers/__init__.py
+-rw-r--r--   0        0        0     6069 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/maneuvers/result.py
+-rw-r--r--   0        0        0     5505 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/maneuvers/strategy.py
+-rw-r--r--   0        0        0     3705 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/maneuvers/use_case.py
+-rw-r--r--   0        0        0     9777 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/nmea_processor.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/__init__.py
+-rw-r--r--   0        0        0    13945 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/ephemeris.py
+-rw-r--r--   0        0        0     3886 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/events.py
+-rw-r--r--   0        0        0    23764 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/requests.py
+-rw-r--r--   0        0        0    17095 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/result.py
+-rw-r--r--   0        0        0    13074 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/use_case.py
+-rw-r--r--   0        0        0    15539 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbital_state.py
+-rw-r--r--   0        0        0    10771 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/orbits.py
+-rw-r--r--   0        0        0    12996 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/quaternion.py
+-rw-r--r--   0        0        0    14728 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/roadmaps.py
+-rw-r--r--   0        0        0    25353 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/spacecraft.py
+-rw-r--r--   0        0        0    20842 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/telemetry.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/tle_extrapolation/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/tle_extrapolation/result.py
+-rw-r--r--   0        0        0     1399 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/tle_extrapolation/use_case.py
+-rw-r--r--   0        0        0     8294 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/models/two_line_element.py
+-rw-r--r--   0        0        0        0 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/__init__.py
+-rw-r--r--   0        0        0     2214 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/dates.py
+-rw-r--r--   0        0        0     1997 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/dict.py
+-rw-r--r--   0        0        0      440 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/enum.py
+-rw-r--r--   0        0        0     2756 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/frames.py
+-rw-r--r--   0        0        0     1803 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/geometry.py
+-rw-r--r--   0        0        0      492 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/log.py
+-rw-r--r--   0        0        0     1077 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/math.py
+-rw-r--r--   0        0        0    13916 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/fds/utils/orbital_mechanics.py
+-rw-r--r--   0        0        0      823 2024-05-21 21:37:42.367176 spacetower_fds_sdk-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 spacetower_fds_sdk-1.0.4/PKG-INFO
```

### Comparing `spacetower_fds_sdk-1.0.3/fds/client.py` & `spacetower_fds_sdk-1.0.4/fds/client.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/config.py` & `spacetower_fds_sdk-1.0.4/fds/config.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/_model.py` & `spacetower_fds_sdk-1.0.4/fds/models/_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import yaml
 from loguru import logger
 from typing_extensions import Self
 
 from fds.client import FdsClient
-from fds.models import BLUEPRINT_FILEPATH
+from fds.models import DEFAULT_CONFIG
 from fds.utils.dates import get_datetime
 from fds.utils.dict import compare_two_dicts
 from fds.utils.enum import EnumFromInput
 from fds.utils.log import log_and_raise
 
 
 class ModelSource(EnumFromInput):
@@ -195,17 +195,15 @@
         obj._model_source = ModelSource.CONFIG
         return obj
 
     @staticmethod
     def _get_config_dict_from_file(config_filepath: str | Path) -> dict:
         with open(config_filepath, 'r') as f:
             config = yaml.safe_load(f)
-        with open(BLUEPRINT_FILEPATH, 'r') as f:
-            blueprint = yaml.safe_load(f)
 
-        if config.get('version') != blueprint.get('version'):
+        if config.get('version') != DEFAULT_CONFIG.get('version'):
             msg = (f"Configuration file version ({config.get('version')}) "
-                   f"does not correspond to the blueprint version ({blueprint.get('version')}).")
+                   f"does not correspond to the default version ({DEFAULT_CONFIG.get('version')}).")
             log_and_raise(ValueError, msg)
 
-        compare_two_dicts(config, blueprint)
+        compare_two_dicts(config, DEFAULT_CONFIG)
         return config
```

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/_use_case.py` & `spacetower_fds_sdk-1.0.4/fds/models/_use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/actions.py` & `spacetower_fds_sdk-1.0.4/fds/models/actions.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/determination/configuration.py` & `spacetower_fds_sdk-1.0.4/fds/models/determination/configuration.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/determination/requests.py` & `spacetower_fds_sdk-1.0.4/fds/models/determination/requests.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/determination/result.py` & `spacetower_fds_sdk-1.0.4/fds/models/determination/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/determination/use_case.py` & `spacetower_fds_sdk-1.0.4/fds/models/determination/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/ground_station.py` & `spacetower_fds_sdk-1.0.4/fds/models/ground_station.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/result.py` & `spacetower_fds_sdk-1.0.4/fds/models/maneuvers/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/strategy.py` & `spacetower_fds_sdk-1.0.4/fds/models/maneuvers/strategy.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/use_case.py` & `spacetower_fds_sdk-1.0.4/fds/models/maneuvers/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/nmea_processor.py` & `spacetower_fds_sdk-1.0.4/fds/models/nmea_processor.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/ephemeris.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/ephemeris.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/events.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/events.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/requests.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/requests.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/result.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/use_case.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbit_extrapolation/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbital_state.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbital_state.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/orbits.py` & `spacetower_fds_sdk-1.0.4/fds/models/orbits.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/quaternion.py` & `spacetower_fds_sdk-1.0.4/fds/models/quaternion.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/roadmaps.py` & `spacetower_fds_sdk-1.0.4/fds/models/roadmaps.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/spacecraft.py` & `spacetower_fds_sdk-1.0.4/fds/models/spacecraft.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/telemetry.py` & `spacetower_fds_sdk-1.0.4/fds/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/result.py` & `spacetower_fds_sdk-1.0.4/fds/models/tle_extrapolation/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/use_case.py` & `spacetower_fds_sdk-1.0.4/fds/models/tle_extrapolation/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/models/two_line_element.py` & `spacetower_fds_sdk-1.0.4/fds/models/two_line_element.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/dates.py` & `spacetower_fds_sdk-1.0.4/fds/utils/dates.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/dict.py` & `spacetower_fds_sdk-1.0.4/fds/utils/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     each key corresponds to a dictionary, and keys of this dictionary must be the same as the blueprint one.
     """
     _check_if_dict(blueprint, "blueprint")
     _check_if_dict(test_dict, "test_dict")
 
     for key in test_dict.keys():
         if key not in blueprint.keys():
-            msg = f"Dictionary key {key} is not in blueprint keys {blueprint.keys()}"
+            msg = f"Dictionary key {key} is not in default config key {blueprint.keys()}"
             log_and_raise(ValueError, msg)
         if isinstance(blueprint[key], dict):
             _check_if_dict(test_dict[key], f"test_dict[{key}]")
             _check_if_same_keys(key, blueprint, test_dict)
 
 
 def _check_if_same_keys(key: str, blueprint: dict, test_dict: dict):
```

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/frames.py` & `spacetower_fds_sdk-1.0.4/fds/utils/frames.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/geometry.py` & `spacetower_fds_sdk-1.0.4/fds/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/math.py` & `spacetower_fds_sdk-1.0.4/fds/utils/math.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/fds/utils/orbital_mechanics.py` & `spacetower_fds_sdk-1.0.4/fds/utils/orbital_mechanics.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.3/PKG-INFO` & `spacetower_fds_sdk-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetower-fds-sdk
-Version: 1.0.3
+Version: 1.0.4
 Summary: SDK for spacetower Flight Dynamics System API
 License: Proprietary
 Keywords: FDS,API,Exotrail,Flight Dynamics
 Author: Exotrail
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

