# Comparing `tmp/mrd_python-2.0.0rc1.tar.gz` & `tmp/mrd_python-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrd_python-2.0.0rc1.tar", last modified: Wed May 22 16:59:17 2024, max compression
+gzip compressed data, was "mrd_python-2.0.0rc2.tar", last modified: Wed May 22 18:12:30 2024, max compression
```

## Comparing `mrd_python-2.0.0rc1.tar` & `mrd_python-2.0.0rc2.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 16:59:17.009572 mrd_python-2.0.0rc1/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1099 2024-05-22 02:23:27.000000 mrd_python-2.0.0rc1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1954 2024-05-22 16:59:17.009572 mrd_python-2.0.0rc1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 16:59:16.999571 mrd_python-2.0.0rc1/mrd/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2275 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc1/mrd/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    46614 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/_binary.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3390 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc1/mrd/_dtypes.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    39791 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/_ndjson.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    53801 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/binary.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)   169451 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/ndjson.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    23566 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/protocols.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 16:59:17.009572 mrd_python-2.0.0rc1/mrd/tools/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1372 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/tools/export_png_images.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5866 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/tools/phantom.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6220 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/tools/simulation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8396 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/tools/stream_recon.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1337 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/tools/transform.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    93782 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc1/mrd/types.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9563 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc1/mrd/yardl_types.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 16:59:17.009572 mrd_python-2.0.0rc1/mrd_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1954 2024-05-22 16:59:16.000000 mrd_python-2.0.0rc1/mrd_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      473 2024-05-22 16:59:16.000000 mrd_python-2.0.0rc1/mrd_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-22 16:59:16.000000 mrd_python-2.0.0rc1/mrd_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2024-05-22 16:59:16.000000 mrd_python-2.0.0rc1/mrd_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        4 2024-05-22 16:59:16.000000 mrd_python-2.0.0rc1/mrd_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2024-05-22 16:59:06.000000 mrd_python-2.0.0rc1/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-22 16:59:17.009572 mrd_python-2.0.0rc1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      157 2024-05-21 17:46:22.000000 mrd_python-2.0.0rc1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2024-05-22 18:06:12.000000 mrd_python-2.0.0rc2/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.353811 mrd_python-2.0.0rc2/mrd/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2275 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    46614 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/_binary.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3390 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/_dtypes.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    39791 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/_ndjson.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    53801 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/binary.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   169451 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/ndjson.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    23566 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/protocols.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.353811 mrd_python-2.0.0rc2/mrd/tools/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1372 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/export_png_images.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5866 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/phantom.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6220 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/simulation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8396 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/stream_recon.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1337 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/tools/transform.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    93782 2024-05-16 21:05:08.000000 mrd_python-2.0.0rc2/mrd/types.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     9563 2024-04-22 16:37:24.000000 mrd_python-2.0.0rc2/mrd/yardl_types.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/mrd_python.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      828 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      465 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        4 2024-05-22 18:12:30.000000 mrd_python-2.0.0rc2/mrd_python.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      849 2024-05-22 18:07:54.000000 mrd_python-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2024-05-22 18:12:30.363811 mrd_python-2.0.0rc2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      157 2024-05-21 17:46:22.000000 mrd_python-2.0.0rc2/setup.py
```

### Comparing `mrd_python-2.0.0rc1/mrd/__init__.py` & `mrd_python-2.0.0rc2/mrd/__init__.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/_binary.py` & `mrd_python-2.0.0rc2/mrd/_binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/_dtypes.py` & `mrd_python-2.0.0rc2/mrd/_dtypes.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/_ndjson.py` & `mrd_python-2.0.0rc2/mrd/_ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/binary.py` & `mrd_python-2.0.0rc2/mrd/binary.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/ndjson.py` & `mrd_python-2.0.0rc2/mrd/ndjson.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/protocols.py` & `mrd_python-2.0.0rc2/mrd/protocols.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/tools/export_png_images.py` & `mrd_python-2.0.0rc2/mrd/tools/export_png_images.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/tools/phantom.py` & `mrd_python-2.0.0rc2/mrd/tools/phantom.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/tools/simulation.py` & `mrd_python-2.0.0rc2/mrd/tools/simulation.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/tools/stream_recon.py` & `mrd_python-2.0.0rc2/mrd/tools/stream_recon.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/tools/transform.py` & `mrd_python-2.0.0rc2/mrd/tools/transform.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/types.py` & `mrd_python-2.0.0rc2/mrd/types.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/mrd/yardl_types.py` & `mrd_python-2.0.0rc2/mrd/yardl_types.py`

 * *Files identical despite different names*

### Comparing `mrd_python-2.0.0rc1/pyproject.toml` & `mrd_python-2.0.0rc2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 packages = ["mrd", "mrd.tools"]
 
 [project]
 name = "mrd-python"
 dynamic = ["version"]
 dependencies = ["numpy>=1.22.0", "pillow>=9.2.0"]
 requires-python = ">=3.9"
-description = "Libraries and tools for working with data in the ISMRM Raw Data (ISMRMRD or MRD)."
+description = "Library and tools for working with data in the ISMRM Raw Data (MRD) format."
 readme = "README.md"
-license = {file = "LICENSE" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Medical Science Apps."
 ]
 keywords = []
 
 [project.urls]
-Homepage = "https://github.com/ismrmrd/mrd"
-Documentation = "https://github.com/ismrmrd/mrd"
+Homepage = "https://ismrmrd.github.io/mrd"
+Documentation = "https://ismrmrd.github.io/mrd"
 Repository = "https://github.com/ismrmrd/mrd"
```

