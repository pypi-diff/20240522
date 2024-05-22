# Comparing `tmp/browsergym_miniwob-0.2.2.tar.gz` & `tmp/browsergym_miniwob-0.2.6.tar.gz`

## Comparing `browsergym_miniwob-0.2.2.tar` & `browsergym_miniwob-0.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/requirements.txt
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/src/browsergym/miniwob/__init__.py
--rw-r--r--   0        0        0    19080 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/src/browsergym/miniwob/all.py
--rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/src/browsergym/miniwob/base.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/tests/test_base.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/tests/test_click-menu-2.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/tests/test_click-scroll-list.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/tests/test_use-colorwheel-2.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/tests/utils.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/.gitignore
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/README.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/requirements.txt
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/src/browsergym/miniwob/__init__.py
+-rw-r--r--   0        0        0    19080 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/src/browsergym/miniwob/all.py
+-rw-r--r--   0        0        0     5694 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/src/browsergym/miniwob/base.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/tests/test_base.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/tests/test_click-menu-2.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/tests/test_click-scroll-list.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/tests/test_use-colorwheel-2.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/tests/utils.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/.gitignore
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 browsergym_miniwob-0.2.6/PKG-INFO
```

### Comparing `browsergym_miniwob-0.2.2/src/browsergym/miniwob/__init__.py` & `browsergym_miniwob-0.2.6/src/browsergym/miniwob/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-__version__ = "0.2.2"
-
 from browsergym.core.registration import register_task
 
 from . import all
 
 ALL_MINIWOB_TASKS = [
     all.AscendingNumbersTask,
     all.BisectAngleTask,
```

### Comparing `browsergym_miniwob-0.2.2/src/browsergym/miniwob/all.py` & `browsergym_miniwob-0.2.6/src/browsergym/miniwob/all.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/src/browsergym/miniwob/base.py` & `browsergym_miniwob-0.2.6/src/browsergym/miniwob/base.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/tests/test_base.py` & `browsergym_miniwob-0.2.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/tests/test_click-menu-2.py` & `browsergym_miniwob-0.2.6/tests/test_click-menu-2.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/tests/test_click-scroll-list.py` & `browsergym_miniwob-0.2.6/tests/test_click-scroll-list.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/tests/test_use-colorwheel-2.py` & `browsergym_miniwob-0.2.6/tests/test_use-colorwheel-2.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/tests/utils.py` & `browsergym_miniwob-0.2.6/tests/utils.py`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/README.md` & `browsergym_miniwob-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `browsergym_miniwob-0.2.2/pyproject.toml` & `browsergym_miniwob-0.2.6/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 ]
 dynamic = ["dependencies", "version"]
 
 [project.urls]
 homepage = "https://github.com/ServiceNow/BrowserGym"
 
 [tool.hatch.version]
-path = "src/browsergym/miniwob/__init__.py"
+path = "../core/src/browsergym/core/__init__.py"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/browsergym"]
```

### Comparing `browsergym_miniwob-0.2.2/PKG-INFO` & `browsergym_miniwob-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.3
 Name: browsergym-miniwob
-Version: 0.2.2
+Version: 0.2.6
 Summary: MiniWoB++ benchmark for BrowserGym
 Project-URL: homepage, https://github.com/ServiceNow/BrowserGym
 Author: Rim Assouel, Maxime Gasse, Tom Marty
 License: Apache-2.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >3.7
-Requires-Dist: browsergym-core==0.2.2
+Requires-Dist: browsergym-core==0.2.6
 Description-Content-Type: text/markdown
 
 # Miniwob benchmark for BrowserGym
 
 This package provides `browsergym.miniwob`, which is an unofficial port of the [MiniWoB++](https://miniwob.farama.org/) benchmark for BrowserGym.
 
 ## Setup
```

