# Comparing `tmp/openbb_crypto-1.2.0.tar.gz` & `tmp/openbb_crypto-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_crypto-1.2.0.tar", max compression
+gzip compressed data, was "openbb_crypto-1.2.1.tar", max compression
```

## Comparing `openbb_crypto-1.2.0.tar` & `openbb_crypto-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      330 2024-05-15 14:22:42.887110 openbb_crypto-1.2.0/README.md
--rw-r--r--   0        0        0       31 2024-04-23 10:22:39.593321 openbb_crypto-1.2.0/openbb_crypto/__init__.py
--rw-r--r--   0        0        0     1053 2024-04-23 10:22:39.593531 openbb_crypto-1.2.0/openbb_crypto/crypto_router.py
--rw-r--r--   0        0        0       34 2024-04-23 10:22:39.593695 openbb_crypto-1.2.0/openbb_crypto/price/__init__.py
--rw-r--r--   0        0        0     1758 2024-04-08 12:02:16.520402 openbb_crypto-1.2.0/openbb_crypto/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.730131 openbb_crypto-1.2.0/openbb_crypto/py.typed
--rw-r--r--   0        0        0      478 2024-05-15 16:03:51.324281 openbb_crypto-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 openbb_crypto-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2024-05-22 11:48:40.399330 openbb_crypto-1.2.1/README.md
+-rw-r--r--   0        0        0       31 2024-05-14 16:56:41.553863 openbb_crypto-1.2.1/openbb_crypto/__init__.py
+-rw-r--r--   0        0        0     1053 2024-05-14 16:56:41.553863 openbb_crypto-1.2.1/openbb_crypto/crypto_router.py
+-rw-r--r--   0        0        0       34 2024-05-14 16:56:41.553863 openbb_crypto-1.2.1/openbb_crypto/price/__init__.py
+-rw-r--r--   0        0        0     1758 2024-05-14 16:56:41.553863 openbb_crypto-1.2.1/openbb_crypto/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.553863 openbb_crypto-1.2.1/openbb_crypto/py.typed
+-rw-r--r--   0        0        0      478 2024-05-22 13:55:15.631426 openbb_crypto-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 openbb_crypto-1.2.1/PKG-INFO
```

### Comparing `openbb_crypto-1.2.0/openbb_crypto/crypto_router.py` & `openbb_crypto-1.2.1/openbb_crypto/crypto_router.py`

 * *Files identical despite different names*

### Comparing `openbb_crypto-1.2.0/openbb_crypto/price/price_router.py` & `openbb_crypto-1.2.1/openbb_crypto/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_crypto-1.2.0/PKG-INFO` & `openbb_crypto-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-crypto
-Version: 1.2.0
+Version: 1.2.1
 Summary: Crypto extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Crypto data extension for OpenBB Platform
 
 This extension provides a set of commands for crypto data retrieval.
 
 ## Installation
```

