# Comparing `tmp/drift_jit_proxy-0.1.4.tar.gz` & `tmp/drift_jit_proxy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drift_jit_proxy-0.1.4.tar", max compression
+gzip compressed data, was "drift_jit_proxy-0.1.5.tar", max compression
```

## Comparing `drift_jit_proxy-0.1.4.tar` & `drift_jit_proxy-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1897 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/README.md
--rw-r--r--   0        0        0      466 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/sdk/jit_proxy/__init__.py
--rw-r--r--   0        0        0     6028 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/sdk/jit_proxy/jit_proxy_client.py
--rw-r--r--   0        0        0     7626 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/base_jitter.py
--rw-r--r--   0        0        0     4094 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/jitter_shotgun.py
--rw-r--r--   0        0        0    13267 2024-03-11 20:34:16.791415 drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/jitter_sniper.py
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 drift_jit_proxy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1897 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/README.md
+-rw-r--r--   0        0        0      466 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/sdk/jit_proxy/__init__.py
+-rw-r--r--   0        0        0     6028 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/sdk/jit_proxy/jit_proxy_client.py
+-rw-r--r--   0        0        0     7626 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/base_jitter.py
+-rw-r--r--   0        0        0     4094 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/jitter_shotgun.py
+-rw-r--r--   0        0        0    13267 2024-05-22 17:58:02.209975 drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/jitter_sniper.py
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 drift_jit_proxy-0.1.5/PKG-INFO
```

### Comparing `drift_jit_proxy-0.1.4/README.md` & `drift_jit_proxy-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `drift_jit_proxy-0.1.4/sdk/jit_proxy/jit_proxy_client.py` & `drift_jit_proxy-0.1.5/sdk/jit_proxy/jit_proxy_client.py`

 * *Files identical despite different names*

### Comparing `drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/base_jitter.py` & `drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/base_jitter.py`

 * *Files identical despite different names*

### Comparing `drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/jitter_shotgun.py` & `drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/jitter_shotgun.py`

 * *Files identical despite different names*

### Comparing `drift_jit_proxy-0.1.4/sdk/jit_proxy/jitter/jitter_sniper.py` & `drift_jit_proxy-0.1.5/sdk/jit_proxy/jitter/jitter_sniper.py`

 * *Files identical despite different names*

### Comparing `drift_jit_proxy-0.1.4/PKG-INFO` & `drift_jit_proxy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: drift-jit-proxy
-Version: 0.1.4
+Version: 0.1.5
 Summary: python sdk for drift protocol v2 jit proxy program
 Author: Frank
 Author-email: frank@lunoho.company
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anchorpy (>=0.17.1,<0.18.0)
-Requires-Dist: driftpy (>=0.7.38,<0.8.0)
+Requires-Dist: anchorpy (>=0.20.1,<0.21.0)
+Requires-Dist: driftpy (>=0.7.52,<0.8.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
-Requires-Dist: solana (>=0.30.1,<0.31.0)
+Requires-Dist: solana (>=0.34.0,<0.35.0)
 Description-Content-Type: text/markdown
 
 # Python JIT Proxy SDK
 
 ## QuickStart Guide
 
 1. Run `poetry install` in the `/python` directory
```

