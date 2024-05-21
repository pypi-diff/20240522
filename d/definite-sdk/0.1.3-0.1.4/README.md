# Comparing `tmp/definite_sdk-0.1.3.tar.gz` & `tmp/definite_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "definite_sdk-0.1.3.tar", max compression
+gzip compressed data, was "definite_sdk-0.1.4.tar", max compression
```

## Comparing `definite_sdk-0.1.3.tar` & `definite_sdk-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1064 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/LICENSE
--rw-r--r--   0        0        0      136 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/README.md
--rw-r--r--   0        0        0      721 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/definite_sdk/client.py
--rw-r--r--   0        0        0     5034 2024-05-16 23:16:41.775288 definite_sdk-0.1.3/definite_sdk/store.py
--rw-r--r--   0        0        0      503 2024-05-16 23:16:41.779288 definite_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 definite_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/LICENSE
+-rw-r--r--   0        0        0      136 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0     1354 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/definite_sdk/client.py
+-rw-r--r--   0        0        0     1647 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/definite_sdk/integration.py
+-rw-r--r--   0        0        0     2506 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/definite_sdk/secret.py
+-rw-r--r--   0        0        0     5034 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/definite_sdk/store.py
+-rw-r--r--   0        0        0      503 2024-05-21 22:06:46.987776 definite_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 definite_sdk-0.1.4/PKG-INFO
```

### Comparing `definite_sdk-0.1.3/LICENSE` & `definite_sdk-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `definite_sdk-0.1.3/definite_sdk/client.py` & `definite_sdk-0.1.4/definite_sdk/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from definite_sdk.integration import DefiniteIntegrationStore
+from definite_sdk.secret import DefiniteSecretStore
 from definite_sdk.store import DefiniteKVStore
 
 API_URL = "https://api.definite.app"
 
 
 class DefiniteClient:
     """Client for interacting with the Definite API."""
@@ -17,7 +19,23 @@
     def get_kv_store(self, name: str) -> DefiniteKVStore:
         """Initializes a key-value store with the provided name.
 
         See DefiniteKVStore for more how to interact with the store.
         """
 
         return DefiniteKVStore(name, self.api_key, self.api_url)
+
+    def get_secret_store(self) -> DefiniteSecretStore:
+        """Initializes the secret store.
+
+        See DefiniteSecretStore for more how to interact with the store.
+        """
+
+        return DefiniteSecretStore(self.api_key, self.api_url)
+
+    def get_integration_store(self) -> DefiniteIntegrationStore:
+        """Initializes the integration store.
+
+        See DefiniteIntegrationStore for more how to interact with the store.
+        """
+
+        return DefiniteIntegrationStore(self.api_key, self.api_url)
```

### Comparing `definite_sdk-0.1.3/definite_sdk/store.py` & `definite_sdk-0.1.4/definite_sdk/store.py`

 * *Files identical despite different names*

### Comparing `definite_sdk-0.1.3/PKG-INFO` & `definite_sdk-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: definite-sdk
-Version: 0.1.3
+Version: 0.1.4
 Summary: Definite SDK for Python
 License: MIT
 Author: Definite
 Author-email: hello@definite.app
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

