# Comparing `tmp/amf_fast_inference-0.0.1.tar.gz` & `tmp/amf_fast_inference-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amf_fast_inference-0.0.1.tar", last modified: Thu Apr  4 09:35:23 2024, max compression
+gzip compressed data, was "amf_fast_inference-0.0.2.tar", last modified: Wed May 22 20:47:29 2024, max compression
```

## Comparing `amf_fast_inference-0.0.1.tar` & `amf_fast_inference-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:35:23.939762 amf_fast_inference-0.0.1/
--rw-r--r--   0 debelagemechu   (501) staff       (20)      728 2024-04-04 09:35:23.939545 amf_fast_inference-0.0.1/PKG-INFO
--rw-r--r--   0 debelagemechu   (501) staff       (20)      679 2024-04-04 09:30:32.000000 amf_fast_inference-0.0.1/pyproject.toml
--rw-r--r--   0 debelagemechu   (501) staff       (20)       38 2024-04-04 09:35:23.939829 amf_fast_inference-0.0.1/setup.cfg
-drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:35:23.938126 amf_fast_inference-0.0.1/src/
--rw-r--r--   0 debelagemechu   (501) staff       (20)        2 2024-04-04 09:32:53.000000 amf_fast_inference-0.0.1/src/__init__.py
-drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:35:23.938381 amf_fast_inference-0.0.1/src/amf_fast_inference/
--rw-r--r--   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:32:13.000000 amf_fast_inference-0.0.1/src/amf_fast_inference/__init__.py
--rw-r--r--   0 debelagemechu   (501) staff       (20)      850 2024-04-04 09:34:16.000000 amf_fast_inference-0.0.1/src/amf_fast_inference/model.py
-drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:35:23.939292 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/
--rw-r--r--   0 debelagemechu   (501) staff       (20)      728 2024-04-04 09:35:23.000000 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/PKG-INFO
--rw-r--r--   0 debelagemechu   (501) staff       (20)      326 2024-04-04 09:35:23.000000 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/SOURCES.txt
--rw-r--r--   0 debelagemechu   (501) staff       (20)        1 2024-04-04 09:35:23.000000 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/dependency_links.txt
--rw-r--r--   0 debelagemechu   (501) staff       (20)       78 2024-04-04 09:35:23.000000 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/requires.txt
--rw-r--r--   0 debelagemechu   (501) staff       (20)       28 2024-04-04 09:35:23.000000 amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/top_level.txt
+drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-05-22 20:47:29.129046 amf_fast_inference-0.0.2/
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      834 2024-05-22 20:47:29.128861 amf_fast_inference-0.0.2/PKG-INFO
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      775 2024-05-22 20:47:25.000000 amf_fast_inference-0.0.2/pyproject.toml
+-rw-r--r--   0 debelagemechu   (501) staff       (20)       38 2024-05-22 20:47:29.129087 amf_fast_inference-0.0.2/setup.cfg
+drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-05-22 20:47:29.127633 amf_fast_inference-0.0.2/src/
+-rw-r--r--   0 debelagemechu   (501) staff       (20)        2 2024-04-04 09:32:53.000000 amf_fast_inference-0.0.2/src/__init__.py
+drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-05-22 20:47:29.127850 amf_fast_inference-0.0.2/src/amf_fast_inference/
+-rw-r--r--   0 debelagemechu   (501) staff       (20)        0 2024-04-04 09:32:13.000000 amf_fast_inference-0.0.2/src/amf_fast_inference/__init__.py
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      850 2024-04-04 09:34:16.000000 amf_fast_inference-0.0.2/src/amf_fast_inference/model.py
+drwxr-xr-x   0 debelagemechu   (501) staff       (20)        0 2024-05-22 20:47:29.128636 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      834 2024-05-22 20:47:29.000000 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/PKG-INFO
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      326 2024-05-22 20:47:29.000000 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 debelagemechu   (501) staff       (20)        1 2024-05-22 20:47:29.000000 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 debelagemechu   (501) staff       (20)      169 2024-05-22 20:47:29.000000 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/requires.txt
+-rw-r--r--   0 debelagemechu   (501) staff       (20)       28 2024-05-22 20:47:29.000000 amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/top_level.txt
```

### Comparing `amf_fast_inference-0.0.1/PKG-INFO` & `amf_fast_inference-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: amf_fast_inference
-Version: 0.0.1
+Version: 0.0.2
 Summary: uses pruning and quatisation to make inference speed faster
 Author-email: Debela Gemechu <dabookoo@gmail.com>
 Project-URL: Homepage, https://github.com/debelatesfaye/amf_fast_inference
 Project-URL: Issues, https://github.com/debelatesfaye/amf_fast_inference/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: optimum
-Requires-Dist: optimum-intel
-Requires-Dist: openvino
-Requires-Dist: onnx
-Requires-Dist: onnxruntime
+Requires-Dist: optimum==1.18.0
+Requires-Dist: optimum-intel==1.17.0.dev0+447ef50
+Requires-Dist: openvino==2024.0.0
+Requires-Dist: onnx==1.16.0
+Requires-Dist: onnxruntime==1.17.1
 Requires-Dist: onnxruntime-tools==1.7.0
-Requires-Dist: nncf
+Requires-Dist: nncf==2.9.0
+Requires-Dist: openvino-telemetry==2023.2.1
```

### Comparing `amf_fast_inference-0.0.1/src/amf_fast_inference/model.py` & `amf_fast_inference-0.0.2/src/amf_fast_inference/model.py`

 * *Files identical despite different names*

### Comparing `amf_fast_inference-0.0.1/src/amf_fast_inference.egg-info/PKG-INFO` & `amf_fast_inference-0.0.2/src/amf_fast_inference.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: amf_fast_inference
-Version: 0.0.1
+Version: 0.0.2
 Summary: uses pruning and quatisation to make inference speed faster
 Author-email: Debela Gemechu <dabookoo@gmail.com>
 Project-URL: Homepage, https://github.com/debelatesfaye/amf_fast_inference
 Project-URL: Issues, https://github.com/debelatesfaye/amf_fast_inference/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: optimum
-Requires-Dist: optimum-intel
-Requires-Dist: openvino
-Requires-Dist: onnx
-Requires-Dist: onnxruntime
+Requires-Dist: optimum==1.18.0
+Requires-Dist: optimum-intel==1.17.0.dev0+447ef50
+Requires-Dist: openvino==2024.0.0
+Requires-Dist: onnx==1.16.0
+Requires-Dist: onnxruntime==1.17.1
 Requires-Dist: onnxruntime-tools==1.7.0
-Requires-Dist: nncf
+Requires-Dist: nncf==2.9.0
+Requires-Dist: openvino-telemetry==2023.2.1
```

