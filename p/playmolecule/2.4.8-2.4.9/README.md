# Comparing `tmp/playmolecule-2.4.8.tar.gz` & `tmp/playmolecule-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-2.4.8.tar", last modified: Mon Nov 27 12:01:20 2023, max compression
+gzip compressed data, was "playmolecule-2.4.9.tar", last modified: Tue Nov 28 14:48:34 2023, max compression
```

## Comparing `playmolecule-2.4.8.tar` & `playmolecule-2.4.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.239232 playmolecule-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-27 12:00:47.000000 playmolecule-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-27 12:00:47.000000 playmolecule-2.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-27 12:01:20.239232 playmolecule-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-27 12:00:47.000000 playmolecule-2.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.239232 playmolecule-2.4.8/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/_appfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/_pmws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14053 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-27 12:01:20.239232 playmolecule-2.4.8/playmolecule/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.235232 playmolecule-2.4.8/playmolecule/apps/
--rw-r--r--   0 runner    (1001) docker     (127)    28746 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/logging.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.235232 playmolecule-2.4.8/playmolecule/share/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/share/apptainer_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/share/func.py.jinja
--rwxr-xr-x   0 runner    (1001) docker     (127)  2305112 2023-11-27 12:00:47.000000 playmolecule-2.4.8/playmolecule/share/pm-licenses
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.239232 playmolecule-2.4.8/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-27 12:01:20.000000 playmolecule-2.4.8/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-11-27 12:01:20.000000 playmolecule-2.4.8/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 12:01:20.000000 playmolecule-2.4.8/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 12:01:19.000000 playmolecule-2.4.8/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-27 12:01:20.000000 playmolecule-2.4.8/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-27 12:01:20.000000 playmolecule-2.4.8/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-11-27 12:00:47.000000 playmolecule-2.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 12:01:20.239232 playmolecule-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-27 12:00:47.000000 playmolecule-2.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 12:01:20.239232 playmolecule-2.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2023-11-27 12:00:47.000000 playmolecule-2.4.8/tests/test_playmolecule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.673039 playmolecule-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-11-28 14:48:04.000000 playmolecule-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-11-28 14:48:04.000000 playmolecule-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-28 14:48:34.673039 playmolecule-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-28 14:48:04.000000 playmolecule-2.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.673039 playmolecule-2.4.9/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/_appfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/_pmws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14053 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-28 14:48:34.673039 playmolecule-2.4.9/playmolecule/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.669039 playmolecule-2.4.9/playmolecule/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)    28876 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/logging.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.669039 playmolecule-2.4.9/playmolecule/share/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/share/apptainer_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/share/func.py.jinja
+-rwxr-xr-x   0 runner    (1001) docker     (127)  2305112 2023-11-28 14:48:04.000000 playmolecule-2.4.9/playmolecule/share/pm-licenses
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.673039 playmolecule-2.4.9/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-28 14:48:34.000000 playmolecule-2.4.9/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2023-11-28 14:48:04.000000 playmolecule-2.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 14:48:34.673039 playmolecule-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-28 14:48:04.000000 playmolecule-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 14:48:34.673039 playmolecule-2.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5811 2023-11-28 14:48:04.000000 playmolecule-2.4.9/tests/test_playmolecule.py
```

### Comparing `playmolecule-2.4.8/LICENSE` & `playmolecule-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/PKG-INFO` & `playmolecule-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 2.4.8
+Version: 2.4.9
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-2.4.8/playmolecule/__init__.py` & `playmolecule-2.4.9/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/_appfiles.py` & `playmolecule-2.4.9/playmolecule/_appfiles.py`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/_pmws.py` & `playmolecule-2.4.9/playmolecule/_pmws.py`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/_tests.py` & `playmolecule-2.4.9/playmolecule/_tests.py`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/_update.py` & `playmolecule-2.4.9/playmolecule/_update.py`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/apps/__init__.py` & `playmolecule-2.4.9/playmolecule/apps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -549,18 +549,21 @@
                 outname = os.path.join(inputdir, os.path.basename(val))
                 i = 0
                 while os.path.exists(outname):
                     parts = os.path.splitext(os.path.basename(val))
                     outname = os.path.join(inputdir, f"{parts[0]}_{i}{parts[1]}")
                     i += 1
 
-                if os.path.isdir(val):
-                    shutil.copytree(val, outname)
+                if "PM_SYMLINK" in os.environ:
+                    os.symlink(val, outname)
                 else:
-                    shutil.copy(val, outname)
+                    if os.path.isdir(val):
+                        shutil.copytree(val, outname)
+                    else:
+                        shutil.copy(val, outname)
                 newvals.append(os.path.relpath(outname, write_dir))
 
             if len(newvals) == 0:
                 arguments[name] = None
             elif len(newvals) == 1:
                 arguments[name] = newvals[0]
                 if not isinstance(vals[0], _File):
```

### Comparing `playmolecule-2.4.8/playmolecule/share/apptainer_run.sh` & `playmolecule-2.4.9/playmolecule/share/apptainer_run.sh`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/share/func.py.jinja` & `playmolecule-2.4.9/playmolecule/share/func.py.jinja`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule/share/pm-licenses` & `playmolecule-2.4.9/playmolecule/share/pm-licenses`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/playmolecule.egg-info/PKG-INFO` & `playmolecule-2.4.9/playmolecule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 2.4.8
+Version: 2.4.9
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-2.4.8/playmolecule.egg-info/SOURCES.txt` & `playmolecule-2.4.9/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/pyproject.toml` & `playmolecule-2.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-2.4.8/tests/test_playmolecule.py` & `playmolecule-2.4.9/tests/test_playmolecule.py`

 * *Files identical despite different names*

