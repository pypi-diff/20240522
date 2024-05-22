# Comparing `tmp/sleap_io-0.1.1.tar.gz` & `tmp/sleap_io-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleap_io-0.1.1.tar", last modified: Tue May 21 00:40:09 2024, max compression
+gzip compressed data, was "sleap_io-0.1.2.tar", last modified: Wed May 22 16:00:19 2024, max compression
```

## Comparing `sleap_io-0.1.1.tar` & `sleap_io-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-21 00:39:11.000000 sleap_io-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-21 00:40:09.551547 sleap_io-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-21 00:39:11.000000 sleap_io-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-21 00:39:11.000000 sleap_io-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:40:09.551547 sleap_io-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.547547 sleap_io-0.1.1/sleap_io/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io/io/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19988 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/jabs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/labelstudio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/nwb.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/slp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    27804 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/io/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io/model/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/labeled_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/labels.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/model/video.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-21 00:39:11.000000 sleap_io-0.1.1/sleap_io/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:40:09.551547 sleap_io-0.1.1/sleap_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 00:40:09.000000 sleap_io-0.1.1/sleap_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:00:19.747461 sleap_io-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-22 15:59:15.000000 sleap_io-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-22 16:00:19.743461 sleap_io-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-05-22 15:59:15.000000 sleap_io-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-22 15:59:15.000000 sleap_io-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:00:19.747461 sleap_io-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:00:19.739461 sleap_io-0.1.2/sleap_io/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:00:19.743461 sleap_io-0.1.2/sleap_io/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19988 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/jabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/labelstudio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17568 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/nwb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25613 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/slp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27804 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/io/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:00:19.743461 sleap_io-0.1.2/sleap_io/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14216 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/labeled_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/labels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/skeleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8019 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/model/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 15:59:15.000000 sleap_io-0.1.2/sleap_io/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:00:19.743461 sleap_io-0.1.2/sleap_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-22 16:00:19.000000 sleap_io-0.1.2/sleap_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 16:00:19.000000 sleap_io-0.1.2/sleap_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:00:19.000000 sleap_io-0.1.2/sleap_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 16:00:19.000000 sleap_io-0.1.2/sleap_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 16:00:19.000000 sleap_io-0.1.2/sleap_io.egg-info/top_level.txt
```

### Comparing `sleap_io-0.1.1/LICENSE` & `sleap_io-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/PKG-INFO` & `sleap_io-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleap-io
-Version: 0.1.1
+Version: 0.1.2
 Summary: Standalone utilities for working with pose data from SLEAP and other tools.
 Author-email: Liezl Maree <lmaree@salk.edu>, David Samy <davidasamy@gmail.com>, Talmo Pereira <talmo@salk.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://sleap.ai
 Project-URL: Repository, https://github.com/talmolab/sleap-io
 Keywords: sleap,pose tracking,pose estimation,behavior
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sleap_io-0.1.1/README.md` & `sleap_io-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/pyproject.toml` & `sleap_io-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/__init__.py` & `sleap_io-0.1.2/sleap_io/__init__.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/jabs.py` & `sleap_io-0.1.2/sleap_io/io/jabs.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/labelstudio.py` & `sleap_io-0.1.2/sleap_io/io/labelstudio.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/main.py` & `sleap_io-0.1.2/sleap_io/io/main.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/nwb.py` & `sleap_io-0.1.2/sleap_io/io/nwb.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/slp.py` & `sleap_io-0.1.2/sleap_io/io/slp.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,17 +193,19 @@
     Args:
         labels_path: A string path to the SLEAP labels file.
         videos: A list of `Video` objects.
 
     Returns:
         A list of `SuggestionFrame` objects.
     """
-    suggestions = [
-        json.loads(x) for x in read_hdf5_dataset(labels_path, "suggestions_json")
-    ]
+    try:
+        suggestions = read_hdf5_dataset(labels_path, "suggestions_json")
+    except KeyError:
+        return []
+    suggestions = [json.loads(x) for x in suggestions]
     suggestions_objects = []
     for suggestion in suggestions:
         suggestions_objects.append(
             SuggestionFrame(
                 video=videos[int(suggestion["video"])],
                 frame_idx=suggestion["frame_idx"],
             )
```

### Comparing `sleap_io-0.1.1/sleap_io/io/utils.py` & `sleap_io-0.1.2/sleap_io/io/utils.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/io/video.py` & `sleap_io-0.1.2/sleap_io/io/video.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/model/instance.py` & `sleap_io-0.1.2/sleap_io/model/instance.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/model/labeled_frame.py` & `sleap_io-0.1.2/sleap_io/model/labeled_frame.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/model/labels.py` & `sleap_io-0.1.2/sleap_io/model/labels.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/model/skeleton.py` & `sleap_io-0.1.2/sleap_io/model/skeleton.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io/model/video.py` & `sleap_io-0.1.2/sleap_io/model/video.py`

 * *Files identical despite different names*

### Comparing `sleap_io-0.1.1/sleap_io.egg-info/PKG-INFO` & `sleap_io-0.1.2/sleap_io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleap-io
-Version: 0.1.1
+Version: 0.1.2
 Summary: Standalone utilities for working with pose data from SLEAP and other tools.
 Author-email: Liezl Maree <lmaree@salk.edu>, David Samy <davidasamy@gmail.com>, Talmo Pereira <talmo@salk.edu>
 License: BSD-3-Clause
 Project-URL: Homepage, https://sleap.ai
 Project-URL: Repository, https://github.com/talmolab/sleap-io
 Keywords: sleap,pose tracking,pose estimation,behavior
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sleap_io-0.1.1/sleap_io.egg-info/SOURCES.txt` & `sleap_io-0.1.2/sleap_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

