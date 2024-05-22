# Comparing `tmp/flytekitplugins_identity_aware_proxy-1.12.1b1.tar.gz` & `tmp/flytekitplugins_identity_aware_proxy-1.12.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_identity_aware_proxy-1.12.1b1.tar", last modified: Thu May 16 22:53:14 2024, max compression
+gzip compressed data, was "flytekitplugins_identity_aware_proxy-1.12.1b2.tar", last modified: Wed May 22 13:27:12 2024, max compression
```

## Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1.tar` & `flytekitplugins_identity_aware_proxy-1.12.1b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:14.427207 flytekitplugins_identity_aware_proxy-1.12.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-16 22:53:14.427207 flytekitplugins_identity_aware_proxy-1.12.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-05-16 22:52:45.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:14.423207 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:14.423207 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins/identity_aware_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 22:52:45.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins/identity_aware_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-16 22:52:45.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins/identity_aware_proxy/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:14.427207 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:14.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:14.427207 flytekitplugins_identity_aware_proxy-1.12.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 22:53:09.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:14.427207 flytekitplugins_identity_aware_proxy-1.12.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-16 22:52:45.000000 flytekitplugins_identity_aware_proxy-1.12.1b1/tests/test_flytekitplugins_iap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.622363 flytekitplugins_identity_aware_proxy-1.12.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-22 13:27:12.622363 flytekitplugins_identity_aware_proxy-1.12.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20805 2024-05-22 13:26:34.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.618363 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.618363 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins/identity_aware_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:26:34.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins/identity_aware_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-05-22 13:26:34.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins/identity_aware_proxy/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.622363 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:12.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:12.622363 flytekitplugins_identity_aware_proxy-1.12.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-22 13:27:07.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:12.618363 flytekitplugins_identity_aware_proxy-1.12.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-22 13:26:34.000000 flytekitplugins_identity_aware_proxy-1.12.1b2/tests/test_flytekitplugins_iap.py
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/README.md` & `flytekitplugins_identity_aware_proxy-1.12.1b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins/identity_aware_proxy/cli.py` & `flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins/identity_aware_proxy/cli.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO` & `flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-identity_aware_proxy
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: External command plugin to generate ID tokens for GCP Identity Aware Proxy
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-identity-aware-proxy
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt` & `flytekitplugins_identity_aware_proxy-1.12.1b2/flytekitplugins_identity_aware_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/setup.py` & `flytekitplugins_identity_aware_proxy-1.12.1b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "google-auth",
     "flytekit>=1.10",
     # https://github.com/grpc/grpc/issues/33935
     # https://github.com/grpc/grpc/issues/35323
     "grpcio>=1.62.0",
 ]
 
-__version__ = "1.12.1b1"
+__version__ = "1.12.1b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="External command plugin to generate ID tokens for GCP Identity Aware Proxy",
```

### Comparing `flytekitplugins_identity_aware_proxy-1.12.1b1/tests/test_flytekitplugins_iap.py` & `flytekitplugins_identity_aware_proxy-1.12.1b2/tests/test_flytekitplugins_iap.py`

 * *Files identical despite different names*

