# Comparing `tmp/mentabotix-0.1.4.8.tar.gz` & `tmp/mentabotix-0.1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.8.tar", last modified: Sun May 19 06:08:40 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.9.tar", last modified: Sun May 19 12:17:11 2024, max compression
```

## Comparing `mentabotix-0.1.4.8.tar` & `mentabotix-0.1.4.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/README.md
--rw-r--r--   0        0        0      680 2024-05-19 06:08:40.046571 mentabotix-0.1.4.8/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    70823 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    21088 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/find_tests.py
--rw-r--r--   0        0        0    15941 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_menta.py
--rw-r--r--   0        0        0     7747 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_moving_state.py
--rw-r--r--   0        0        0     5759 2024-05-19 06:08:05.442425 mentabotix-0.1.4.8/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-19 12:16:36.552828 mentabotix-0.1.4.9/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-19 12:16:36.552828 mentabotix-0.1.4.9/README.md
+-rw-r--r--   0        0        0      612 2024-05-19 12:17:11.425180 mentabotix-0.1.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1135 2024-05-19 12:16:36.552828 mentabotix-0.1.4.9/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    70823 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    21088 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0        0 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/find_tests.py
+-rw-r--r--   0        0        0    15941 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/test_menta.py
+-rw-r--r--   0        0        0     7747 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5759 2024-05-19 12:16:36.556828 mentabotix-0.1.4.9/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24151 1970-01-01 00:00:00.000000 mentabotix-0.1.4.9/PKG-INFO
```

### Comparing `mentabotix-0.1.4.8/LICENSE` & `mentabotix-0.1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/README.md` & `mentabotix-0.1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/pyproject.toml` & `mentabotix-0.1.4.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.8"
+version = "0.1.4.9"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
-    "pyapriltags>=3.3.0.3",
     "terminaltables>=3.1.10",
     "bdmc>=0.1.5.8",
-    "opencv-python-headless>=4.9.0.80",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.4.8/src/mentabotix/__init__.py` & `mentabotix-0.1.4.9/src/mentabotix/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .modules.botix import MovingState, MovingTransition, Botix
 from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
 from .modules.logger import set_log_level
 from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
 
 from .tools.composers import MovingChainComposer, straight_chain, snaking_chain, scanning_chain, random_lr_turn_branch
 from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
-from .vision.tagdetector import TagDetector
+
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
     "MovingTransition",
     "Botix",
@@ -17,16 +17,14 @@
     "Menta",
     "SequenceSampler",
     "IndexedSampler",
     "DirectSampler",
     "SamplerUsage",
     "SamplerType",
     "Sampler",
-    # vision
-    "TagDetector",
     # exceptions
     "BadSignatureError",
     "RequirementError",
     "SamplerTypeError",
     "TokenizeError",
     "StructuralError",
     # tools/composers
```

### Comparing `mentabotix-0.1.4.8/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.9/src/mentabotix/modules/botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.9/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.9/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.9/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.9/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/find_tests.py` & `mentabotix-0.1.4.9/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/test_botix.py` & `mentabotix-0.1.4.9/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/test_composer.py` & `mentabotix-0.1.4.9/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/test_menta.py` & `mentabotix-0.1.4.9/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/test_moving_state.py` & `mentabotix-0.1.4.9/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/tests/test_moving_transition.py` & `mentabotix-0.1.4.9/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.8/PKG-INFO` & `mentabotix-0.1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.8
+Version: 0.1.4.9
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
-Requires-Dist: pyapriltags>=3.3.0.3
 Requires-Dist: terminaltables>=3.1.10
 Requires-Dist: bdmc>=0.1.5.8
-Requires-Dist: opencv-python-headless>=4.9.0.80
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
```

