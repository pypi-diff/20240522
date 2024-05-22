# Comparing `tmp/uid2_client-2.3.0.tar.gz` & `tmp/uid2_client-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uid2_client-2.3.0.tar", last modified: Mon Apr 29 21:20:17 2024, max compression
+gzip compressed data, was "uid2_client-2.4.0.tar", last modified: Wed May 22 02:41:01 2024, max compression
```

## Comparing `uid2_client-2.3.0.tar` & `uid2_client-2.4.0.tar`

### file list

```diff
@@ -1,54 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.123012 uid2_client-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-29 21:19:55.000000 uid2_client-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 21:20:17.123012 uid2_client-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-29 21:19:55.000000 uid2_client-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-29 21:20:11.000000 uid2_client-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-29 21:20:17.123012 uid2_client-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 21:19:55.000000 uid2_client-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.115012 uid2_client-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_bidstream_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_key_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_publisher_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_refresh_keys_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_sharing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_sharing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-29 21:19:55.000000 uid2_client-2.3.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.119012 uid2_client-2.3.0/uid2_client/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/advertising_token_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/auto_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/bidstream_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/client_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/decryption_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption_data_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/encryption_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/euid_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/identity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/input_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/publisher_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/refresh_keys_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/refresh_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/request_response_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/sharing_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_generate_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_generate_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/token_refresh_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_base64_url_coder.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-29 21:19:55.000000 uid2_client-2.3.0/uid2_client/uid2_token_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:17.123012 uid2_client-2.3.0/uid2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 21:20:17.000000 uid2_client-2.3.0/uid2_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:16.000000 uid2_client-2.3.0/uid2_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:41:01.500651 uid2_client-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-22 02:40:40.000000 uid2_client-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-22 02:41:01.500651 uid2_client-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 02:40:40.000000 uid2_client-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 02:40:56.000000 uid2_client-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-22 02:41:01.500651 uid2_client-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 02:40:40.000000 uid2_client-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:41:01.492651 uid2_client-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17133 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_bidstream_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34500 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_identity_map_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_key_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_refresh_keys_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_sharing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19328 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_sharing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-05-22 02:40:40.000000 uid2_client-2.4.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:41:01.496651 uid2_client-2.4.0/uid2_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/advertising_token_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/auto_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/bidstream_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/client_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/decryption_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/encryption_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/encryption_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/euid_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_map_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_map_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_map_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/identity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/input_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/publisher_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/refresh_keys_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/request_response_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/sharing_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/token_generate_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/token_generate_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/token_refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/uid2_base64_url_coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/uid2_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-22 02:40:40.000000 uid2_client-2.4.0/uid2_client/uid2_token_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:41:01.500651 uid2_client-2.4.0/uid2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:41:01.000000 uid2_client-2.4.0/uid2_client.egg-info/zip-safe
```

### Comparing `uid2_client-2.3.0/LICENSE` & `uid2_client-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/pyproject.toml` & `uid2_client-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools == 68.2.2",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uid2_client"
-version = "2.3.0"
+version = "2.4.0"
 authors = [
     { name = "UID2 team", email = "unifiedid-admin@thetradedesk.com" }
 ]
 description = "UID2 SDK for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `uid2_client-2.3.0/setup.cfg` & `uid2_client-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_bidstream_client.py` & `uid2_client-2.4.0/tests/test_bidstream_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_client.py` & `uid2_client-2.4.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_encryption.py` & `uid2_client-2.4.0/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_key_parse.py` & `uid2_client-2.4.0/tests/test_key_parse.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_keys.py` & `uid2_client-2.4.0/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_normalization.py` & `uid2_client-2.4.0/tests/test_normalization.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_publisher_client.py` & `uid2_client-2.4.0/tests/test_publisher_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_refresh_keys_util.py` & `uid2_client-2.4.0/tests/test_refresh_keys_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_sharing.py` & `uid2_client-2.4.0/tests/test_sharing.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_sharing_client.py` & `uid2_client-2.4.0/tests/test_sharing_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/tests/test_utils.py` & `uid2_client-2.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/auto_refresh.py` & `uid2_client-2.4.0/uid2_client/auto_refresh.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/bidstream_client.py` & `uid2_client-2.4.0/uid2_client/bidstream_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/client.py` & `uid2_client-2.4.0/uid2_client/client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/decryption_status.py` & `uid2_client-2.4.0/uid2_client/decryption_status.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/encryption.py` & `uid2_client-2.4.0/uid2_client/encryption.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/encryption_data_response.py` & `uid2_client-2.4.0/uid2_client/encryption_data_response.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/identity_tokens.py` & `uid2_client-2.4.0/uid2_client/identity_tokens.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/input_util.py` & `uid2_client-2.4.0/uid2_client/input_util.py`

 * *Files 14% similar despite different names*

```diff
@@ -102,7 +102,20 @@
 
 def get_base64_encoded_hash(input):
     return byte_array_to_base64(get_sha256_bytes(input))
 
 
 def get_sha256_bytes(input):
     return hashlib.sha256(input.encode()).digest()
+
+
+def normalize_and_hash_email(email):
+    normalized_email = normalize_email_string(email)
+    if normalized_email is None:
+        raise ValueError("invalid email address: " + email)
+    return get_base64_encoded_hash(normalized_email)
+
+
+def normalize_and_hash_phone(phone):
+    if not is_phone_number_normalized(phone):
+        raise ValueError("phone number is not normalized: " + phone)
+    return get_base64_encoded_hash(phone)
```

### Comparing `uid2_client-2.3.0/uid2_client/keys.py` & `uid2_client-2.4.0/uid2_client/keys.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/publisher_client.py` & `uid2_client-2.4.0/uid2_client/publisher_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/refresh_keys_util.py` & `uid2_client-2.4.0/uid2_client/refresh_keys_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/request_response_util.py` & `uid2_client-2.4.0/uid2_client/request_response_util.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/sharing_client.py` & `uid2_client-2.4.0/uid2_client/sharing_client.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/token_generate_input.py` & `uid2_client-2.4.0/uid2_client/token_generate_input.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/token_generate_response.py` & `uid2_client-2.4.0/uid2_client/token_generate_response.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/token_refresh_response.py` & `uid2_client-2.4.0/uid2_client/token_refresh_response.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/uid2_base64_url_coder.py` & `uid2_client-2.4.0/uid2_client/uid2_base64_url_coder.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client/uid2_token_generator.py` & `uid2_client-2.4.0/uid2_client/uid2_token_generator.py`

 * *Files identical despite different names*

### Comparing `uid2_client-2.3.0/uid2_client.egg-info/SOURCES.txt` & `uid2_client-2.4.0/uid2_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 tests/test_bidstream_client.py
 tests/test_client.py
 tests/test_encryption.py
+tests/test_identity_map_client.py
 tests/test_key_parse.py
 tests/test_keys.py
 tests/test_normalization.py
 tests/test_publisher_client.py
 tests/test_refresh_keys_util.py
 tests/test_sharing.py
 tests/test_sharing_client.py
@@ -21,14 +22,17 @@
 uid2_client/client.py
 uid2_client/client_type.py
 uid2_client/decryption_status.py
 uid2_client/encryption.py
 uid2_client/encryption_data_response.py
 uid2_client/encryption_status.py
 uid2_client/euid_client_factory.py
+uid2_client/identity_map_client.py
+uid2_client/identity_map_input.py
+uid2_client/identity_map_response.py
 uid2_client/identity_scope.py
 uid2_client/identity_tokens.py
 uid2_client/identity_type.py
 uid2_client/input_util.py
 uid2_client/keys.py
 uid2_client/publisher_client.py
 uid2_client/refresh_keys_util.py
```

