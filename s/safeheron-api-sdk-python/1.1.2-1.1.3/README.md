# Comparing `tmp/safeheron_api_sdk_python-1.1.2.tar.gz` & `tmp/safeheron_api_sdk_python-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safeheron_api_sdk_python-1.1.2.tar", last modified: Tue May 21 13:27:53 2024, max compression
+gzip compressed data, was "safeheron_api_sdk_python-1.1.3.tar", last modified: Wed May 22 02:33:53 2024, max compression
```

## Comparing `safeheron_api_sdk_python-1.1.2.tar` & `safeheron_api_sdk_python-1.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.045145 safeheron_api_sdk_python-1.1.2/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.1.2/LICENSE
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-21 13:27:53.044021 safeheron_api_sdk_python-1.1.2/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     5327 2024-05-17 02:38:51.000000 safeheron_api_sdk_python-1.1.2/README.md
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.2/README.rst
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.026991 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.038353 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9934 2024-05-15 11:09:36.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/account_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2676 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/coin_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3484 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/mpc_sign_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    16938 2024-05-21 11:14:31.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/transaction_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11104 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/web3_api.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1192 2024-05-17 03:08:06.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/client.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.039952 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/cosigner/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3434 2024-05-21 13:25:49.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/cosigner/co_signer_converter.py
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)    10240 2024-05-21 13:22:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/tools.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.041166 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/webhook/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2102 2024-05-21 13:25:12.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/webhook/webhook_converter.py
-drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-21 13:27:53.042563 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-21 13:27:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-21 13:27:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-21 13:27:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       36 2024-05-21 13:27:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/requires.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-21 13:27:52.000000 safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-21 13:27:53.045402 safeheron_api_sdk_python-1.1.2/setup.cfg
--rw-r--r--   0 pengzhaofeng   (501) staff       (20)      929 2024-05-21 13:27:34.000000 safeheron_api_sdk_python-1.1.2/setup.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.466788 safeheron_api_sdk_python-1.1.3/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1071 2023-09-12 03:12:36.000000 safeheron_api_sdk_python-1.1.3/LICENSE
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-22 02:33:53.466189 safeheron_api_sdk_python-1.1.3/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     5327 2024-05-17 02:38:51.000000 safeheron_api_sdk_python-1.1.3/README.md
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       30 2024-05-08 10:08:15.000000 safeheron_api_sdk_python-1.1.3/README.rst
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.450830 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.461627 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     9934 2024-05-15 11:09:36.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/account_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2676 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/coin_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3484 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/mpc_sign_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    16938 2024-05-21 11:14:31.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/transaction_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    11104 2024-05-15 09:03:00.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/web3_api.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     1192 2024-05-17 03:08:06.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/client.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.462796 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/cosigner/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     3434 2024-05-21 13:25:49.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/cosigner/co_signer_converter.py
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)    10240 2024-05-21 13:22:52.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/tools.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.463894 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/webhook/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)     2102 2024-05-21 13:25:12.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/webhook/webhook_converter.py
+drwxr-xr-x   0 pengzhaofeng   (501) staff       (20)        0 2024-05-22 02:33:53.465149 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      486 2024-05-22 02:33:53.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      675 2024-05-22 02:33:53.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)        1 2024-05-22 02:33:53.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       36 2024-05-22 02:33:53.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       25 2024-05-22 02:33:53.000000 safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)       38 2024-05-22 02:33:53.466909 safeheron_api_sdk_python-1.1.3/setup.cfg
+-rw-r--r--   0 pengzhaofeng   (501) staff       (20)      929 2024-05-22 02:32:38.000000 safeheron_api_sdk_python-1.1.3/setup.py
```

### Comparing `safeheron_api_sdk_python-1.1.2/LICENSE` & `safeheron_api_sdk_python-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/README.md` & `safeheron_api_sdk_python-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/account_api.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/account_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/coin_api.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/coin_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/mpc_sign_api.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/mpc_sign_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/transaction_api.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/api/web3_api.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/api/web3_api.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/client.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/client.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/cosigner/co_signer_converter.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/cosigner/co_signer_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/tools.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/tools.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python/webhook/webhook_converter.py` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python/webhook/webhook_converter.py`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/safeheron_api_sdk_python.egg-info/SOURCES.txt` & `safeheron_api_sdk_python-1.1.3/safeheron_api_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safeheron_api_sdk_python-1.1.2/setup.py` & `safeheron_api_sdk_python-1.1.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 from setuptools import find_packages
 with open("README.rst", "r") as f:
     long_description = f.read()
 setup(name='safeheron_api_sdk_python',
-      version='1.1.2',
+      version='1.1.3',
       description='Python for Safeheron API',
       long_description=long_description,
       author='safeheron',
       author_email='support@safeheron.com',
       url='https://github.com/Safeheron/safeheron-api-sdk-python',
       install_requires=[
             'pyCryptodomex',
```

