# Comparing `tmp/tdewolff-minify-2.20.8.tar.gz` & `tmp/tdewolff-minify-2.20.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdewolff-minify-2.20.8.tar", last modified: Wed Nov 29 21:29:26 2023, max compression
+gzip compressed data, was "tdewolff-minify-2.20.9.tar", last modified: Sat Dec  2 18:32:03 2023, max compression
```

## Comparing `tdewolff-minify-2.20.8.tar` & `tdewolff-minify-2.20.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 21:29:26.995541 tdewolff-minify-2.20.8/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-29 21:29:26.991541 tdewolff-minify-2.20.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/build_minify.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-29 21:29:19.000000 tdewolff-minify-2.20.8/go.mod
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-11-29 21:29:19.000000 tdewolff-minify-2.20.8/go.sum
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/minify.go
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-29 21:29:26.995541 tdewolff-minify-2.20.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 21:29:26.991541 tdewolff-minify-2.20.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 21:29:26.991541 tdewolff-minify-2.20.8/src/minify/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-11-29 21:29:02.000000 tdewolff-minify-2.20.8/src/minify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 21:29:26.991541 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-29 21:29:26.000000 tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 18:32:03.793303 tdewolff-minify-2.20.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-12-02 18:32:03.793303 tdewolff-minify-2.20.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/build_minify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-02 18:31:53.000000 tdewolff-minify-2.20.9/go.mod
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-12-02 18:31:53.000000 tdewolff-minify-2.20.9/go.sum
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/minify.go
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-02 18:32:03.793303 tdewolff-minify-2.20.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 18:32:03.789303 tdewolff-minify-2.20.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 18:32:03.793303 tdewolff-minify-2.20.9/src/minify/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2023-12-02 18:31:37.000000 tdewolff-minify-2.20.9/src/minify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-02 18:32:03.793303 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-02 18:32:03.000000 tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/top_level.txt
```

### Comparing `tdewolff-minify-2.20.8/PKG-INFO` & `tdewolff-minify-2.20.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.20.8
+Version: 2.20.9
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tdewolff-minify-2.20.8/README.md` & `tdewolff-minify-2.20.9/README.md`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.20.8/go.sum` & `tdewolff-minify-2.20.9/go.sum`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 github.com/tdewolff/minify/v2 v2.12.1/go.mod h1:p5pwbvNs1ghbFED/ZW1towGsnnWwzvM8iz8l0eURi9g=
 github.com/tdewolff/minify/v2 v2.12.2 h1:AKIoVwJj/HgBm+d/fPqpEZ31EtCM5FJfJNGagdR9Ecg=
 github.com/tdewolff/minify/v2 v2.12.2/go.mod h1:p5pwbvNs1ghbFED/ZW1towGsnnWwzvM8iz8l0eURi9g=
 github.com/tdewolff/minify/v2 v2.12.9 h1:dvn5MtmuQ/DFMwqf5j8QhEVpPX6fi3WGImhv8RUB4zA=
 github.com/tdewolff/minify/v2 v2.12.9/go.mod h1:qOqdlDfL+7v0/fyymB+OP497nIxJYSvX4MQWA8OoiXU=
 github.com/tdewolff/minify/v2 v2.20.3 h1:8x2BICr21IoNFda5EUyNsoNcEZHL/W0ap+sfUJiGdmg=
 github.com/tdewolff/minify/v2 v2.20.3/go.mod h1:AMF0J/eNujZLDbfMZvWweg5TSG/KuK+/UGKc+k1N8/w=
-github.com/tdewolff/minify/v2 v2.20.8 h1:OqDc95F0OK239T7P5g5oL5XthQtOtKbhbhM9GKc2W9g=
-github.com/tdewolff/minify/v2 v2.20.8/go.mod h1:hZnNtFqXVQ5QIAR05tdgvS7h6E80jyRwHSGVmM4jbzQ=
+github.com/tdewolff/minify/v2 v2.20.9 h1:0RGsL+jBpm77obkuNCjNZ2eiN81CZzTnjeVmTqxCmYk=
+github.com/tdewolff/minify/v2 v2.20.9/go.mod h1:hZnNtFqXVQ5QIAR05tdgvS7h6E80jyRwHSGVmM4jbzQ=
 github.com/tdewolff/parse/v2 v2.6.3 h1:O5rshbkaRmpRtD7k2lG65bEJpcfUMNg5Cx2uRKWVsI8=
 github.com/tdewolff/parse/v2 v2.6.3/go.mod h1:woz0cgbLwFdtbjJu8PIKxhW05KplTFQkOdX78o+Jgrs=
 github.com/tdewolff/parse/v2 v2.6.8 h1:mhNZXYCx//xG7Yq2e/kVLNZw4YfYmeHbhx+Zc0OvFMA=
 github.com/tdewolff/parse/v2 v2.6.8/go.mod h1:XHDhaU6IBgsryfdnpzUXBlT6leW/l25yrFBTEb4eIyM=
 github.com/tdewolff/parse/v2 v2.7.2 h1:9NdxF0nk/+lPI0YADDonSlpiY15hGcVUhXRj9hnK8sM=
 github.com/tdewolff/parse/v2 v2.7.2/go.mod h1:9p2qMIHpjRSTr1qnFxQr+igogyTUTlwvf9awHSm84h8=
 github.com/tdewolff/parse/v2 v2.7.6 h1:PGZH2b/itDSye9RatReRn4GBhsT+KFEMtAMjHRuY1h8=
```

### Comparing `tdewolff-minify-2.20.8/minify.go` & `tdewolff-minify-2.20.9/minify.go`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.20.8/setup.py` & `tdewolff-minify-2.20.9/setup.py`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.20.8/src/minify/__init__.py` & `tdewolff-minify-2.20.9/src/minify/__init__.py`

 * *Files identical despite different names*

### Comparing `tdewolff-minify-2.20.8/src/tdewolff_minify.egg-info/PKG-INFO` & `tdewolff-minify-2.20.9/src/tdewolff_minify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdewolff-minify
-Version: 2.20.8
+Version: 2.20.9
 Summary: Go minifiers for web formats
 Home-page: https://github.com/tdewolff/minify
 Author: Taco de Wolff
 Author-email: tacodewolff@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

