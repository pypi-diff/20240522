# Comparing `tmp/pychzzk-0.1.0.tar.gz` & `tmp/pychzzk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychzzk-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pychzzk-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pychzzk-0.1.0.tar` & `pychzzk-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      862 2024-05-22 10:34:16.917613 pychzzk-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3873 2024-05-22 10:34:16.917613 pychzzk-0.1.0/.gitignore
--rw-r--r--   0        0        0     1065 2024-05-22 10:34:16.917613 pychzzk-0.1.0/LICENSE
--rw-r--r--   0        0        0       50 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/__init__.py
--rw-r--r--   0        0        0      953 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/_http.py
--rw-r--r--   0        0        0     2225 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/api.py
--rw-r--r--   0        0        0       52 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/enums/__init__.py
--rw-r--r--   0        0        0      303 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/enums/fields.py
--rw-r--r--   0        0        0      140 2024-05-22 10:34:16.917613 pychzzk-0.1.0/PyCHZZK/utils.py
--rw-r--r--   0        0        0      721 2024-05-22 10:34:16.917613 pychzzk-0.1.0/README.md
--rw-r--r--   0        0        0      514 2024-05-22 10:34:16.917613 pychzzk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       13 2024-05-22 10:34:16.917613 pychzzk-0.1.0/requirements.txt
--rw-r--r--   0        0        0       48 2024-05-22 10:34:16.917613 pychzzk-0.1.0/requirements_dev.txt
--rw-r--r--   0        0        0        0 2024-05-22 10:34:16.917613 pychzzk-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      448 2024-05-22 10:34:16.917613 pychzzk-0.1.0/tests/test_api.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 pychzzk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      862 2024-05-22 10:43:07.588089 pychzzk-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     3873 2024-05-22 10:43:07.588089 pychzzk-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1065 2024-05-22 10:43:07.588089 pychzzk-0.1.1/LICENSE
+-rw-r--r--   0        0        0       50 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/__init__.py
+-rw-r--r--   0        0        0      953 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/_http.py
+-rw-r--r--   0        0        0     2225 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/api.py
+-rw-r--r--   0        0        0       52 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/enums/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/enums/fields.py
+-rw-r--r--   0        0        0      140 2024-05-22 10:43:07.588089 pychzzk-0.1.1/PyCHZZK/utils.py
+-rw-r--r--   0        0        0      721 2024-05-22 10:43:07.588089 pychzzk-0.1.1/README.md
+-rw-r--r--   0        0        0      507 2024-05-22 10:43:07.588089 pychzzk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       13 2024-05-22 10:43:07.588089 pychzzk-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       48 2024-05-22 10:43:07.588089 pychzzk-0.1.1/requirements_dev.txt
+-rw-r--r--   0        0        0        0 2024-05-22 10:43:07.588089 pychzzk-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-22 10:43:07.588089 pychzzk-0.1.1/tests/test_api.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 pychzzk-0.1.1/PKG-INFO
```

### Comparing `pychzzk-0.1.0/.github/workflows/python-publish.yml` & `pychzzk-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/.gitignore` & `pychzzk-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/LICENSE` & `pychzzk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/PyCHZZK/_http.py` & `pychzzk-0.1.1/PyCHZZK/_http.py`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/PyCHZZK/api.py` & `pychzzk-0.1.1/PyCHZZK/api.py`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/README.md` & `pychzzk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pychzzk-0.1.0/PKG-INFO` & `pychzzk-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: PyCHZZK
-Version: 0.1.0
+Version: 0.1.1
 Summary: NAVER CHZZK Python SDK
 Author-email: Netchive <opensource@netchive.com>
 Maintainer-email: Euiseo Cha <zeroday0619_dev@outlook.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: httpx==0.27.0
-Project-URL: Source, https://github.com/zeroday0619/anamSDK.git
+Project-URL: Source, https://github.com/Netchive/PyCHZZK
 
 # PyCHZZK
 NAVER CHZZK Python SDK
 
 
 ## Usage
 ```
```

