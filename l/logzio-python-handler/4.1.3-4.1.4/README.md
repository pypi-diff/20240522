# Comparing `tmp/logzio_python_handler-4.1.3.tar.gz` & `tmp/logzio_python_handler-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logzio_python_handler-4.1.3.tar", last modified: Sun May 12 07:32:22 2024, max compression
+gzip compressed data, was "logzio_python_handler-4.1.4.tar", last modified: Wed May 22 17:05:30 2024, max compression
```

## Comparing `logzio_python_handler-4.1.3.tar` & `logzio_python_handler-4.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.701995 logzio_python_handler-4.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.github/dependabot.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.701995 logzio_python_handler-4.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.github/workflows/auto-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/.whitesource
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/logzio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/flusher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/logzio/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-12 07:32:22.000000 logzio_python_handler-4.1.3/logzio_python_handler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-12 07:32:22.709996 logzio_python_handler-4.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:22.705995 logzio_python_handler-4.1.3/tests/mockLogzioListener/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/logsList.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/mockLogzioListener/persistentFlags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_add_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_logzioHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tests/test_logzioSender.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-12 07:32:07.000000 logzio_python_handler-4.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.354139 logzio_python_handler-4.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.346139 logzio_python_handler-4.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/.github/dependabot.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.346139 logzio_python_handler-4.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/.github/workflows/auto-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/.whitesource
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 17:05:30.354139 logzio_python_handler-4.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.350139 logzio_python_handler-4.1.4/logzio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/flusher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/logzio/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.350139 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-22 17:05:30.000000 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-22 17:05:30.000000 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:05:30.000000 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 17:05:30.000000 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 17:05:30.000000 logzio_python_handler-4.1.4/logzio_python_handler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 17:05:30.354139 logzio_python_handler-4.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.350139 logzio_python_handler-4.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:30.350139 logzio_python_handler-4.1.4/tests/mockLogzioListener/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/mockLogzioListener/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/mockLogzioListener/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/mockLogzioListener/logsList.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/mockLogzioListener/persistentFlags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/test_add_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/test_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/test_logzioHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tests/test_logzioSender.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-22 17:05:14.000000 logzio_python_handler-4.1.4/tox.ini
```

### Comparing `logzio_python_handler-4.1.3/.github/dependabot.yaml` & `logzio_python_handler-4.1.4/.github/dependabot.yaml`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/.github/workflows/auto-release.yml` & `logzio_python_handler-4.1.4/.github/workflows/auto-release.yml`

 * *Files 3% similar despite different names*

```diff
@@ -5,36 +5,36 @@
     types: [published]
 
 jobs:
   ci-tests:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
-        uses: actions/checkout@v2
+        uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python
-        uses: actions/setup-python@v3.0.0
+        uses: actions/setup-python@v5.1.0
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
       - name: Run tox
         run: python -m tox
 
   build-and-release:
     needs: ci-tests
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v3.0.0
+      - uses: actions/setup-python@v5.1.0
         with:
           python-version: '3.x'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements.txt
       - name: "Build and uploads to PyPI"
```

### Comparing `logzio_python_handler-4.1.3/.gitignore` & `logzio_python_handler-4.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/LICENSE` & `logzio_python_handler-4.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/PKG-INFO` & `logzio_python_handler-4.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: logzio-python-handler
-Version: 4.1.3
+Version: 4.1.4
 Summary: Logging handler to send logs to your Logz.io account with bulk SSL
 Home-page: https://github.com/logzio/logzio-python-handler/
 Author: roiravhon
 Maintainer: tamir-michaeli
 License: Apache License 2
 Keywords: logging handler logz.io bulk https
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 Requires-Dist: requests>=2.27.0
 Requires-Dist: protobuf>=3.20.2
 Provides-Extra: opentelemetry-logging
-Requires-Dist: opentelemetry-instrumentation-logging==0.39b0; extra == "opentelemetry-logging"
+Requires-Dist: opentelemetry-instrumentation-logging==0.45b0; extra == "opentelemetry-logging"
```

### Comparing `logzio_python_handler-4.1.3/README.md` & `logzio_python_handler-4.1.4/README.md`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/logzio/flusher.py` & `logzio_python_handler-4.1.4/logzio/flusher.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/logzio/handler.py` & `logzio_python_handler-4.1.4/logzio/handler.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/logzio/sender.py` & `logzio_python_handler-4.1.4/logzio/sender.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/logzio_python_handler.egg-info/PKG-INFO` & `logzio_python_handler-4.1.4/logzio_python_handler.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: logzio-python-handler
-Version: 4.1.3
+Version: 4.1.4
 Summary: Logging handler to send logs to your Logz.io account with bulk SSL
 Home-page: https://github.com/logzio/logzio-python-handler/
 Author: roiravhon
 Maintainer: tamir-michaeli
 License: Apache License 2
 Keywords: logging handler logz.io bulk https
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
 Requires-Dist: requests>=2.27.0
 Requires-Dist: protobuf>=3.20.2
 Provides-Extra: opentelemetry-logging
-Requires-Dist: opentelemetry-instrumentation-logging==0.39b0; extra == "opentelemetry-logging"
+Requires-Dist: opentelemetry-instrumentation-logging==0.45b0; extra == "opentelemetry-logging"
```

### Comparing `logzio_python_handler-4.1.3/logzio_python_handler.egg-info/SOURCES.txt` & `logzio_python_handler-4.1.4/logzio_python_handler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/setup.py` & `logzio_python_handler-4.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     license="Apache License 2",
     packages=find_packages(),
     install_requires=[
         "requests>=2.27.0",
         "protobuf>=3.20.2"
     ],
     extras_require={
-        "opentelemetry-logging": ["opentelemetry-instrumentation-logging==0.39b0"]
+        "opentelemetry-logging": ["opentelemetry-instrumentation-logging==0.45b0"]
     },
     test_requires=[
         "future"
     ],
     setup_requires=['setuptools_scm'],
     include_package_data=True,
     classifiers=[
```

### Comparing `logzio_python_handler-4.1.3/tests/mockLogzioListener/listener.py` & `logzio_python_handler-4.1.4/tests/mockLogzioListener/listener.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/tests/test_add_context.py` & `logzio_python_handler-4.1.4/tests/test_add_context.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/tests/test_extra_fields.py` & `logzio_python_handler-4.1.4/tests/test_extra_fields.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/tests/test_logzioHandler.py` & `logzio_python_handler-4.1.4/tests/test_logzioHandler.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/tests/test_logzioSender.py` & `logzio_python_handler-4.1.4/tests/test_logzioSender.py`

 * *Files identical despite different names*

### Comparing `logzio_python_handler-4.1.3/tox.ini` & `logzio_python_handler-4.1.4/tox.ini`

 * *Files identical despite different names*

