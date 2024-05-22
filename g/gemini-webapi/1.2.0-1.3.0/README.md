# Comparing `tmp/gemini_webapi-1.2.0.tar.gz` & `tmp/gemini_webapi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemini_webapi-1.2.0.tar", last modified: Sun Apr 28 09:01:25 2024, max compression
+gzip compressed data, was "gemini_webapi-1.3.0.tar", last modified: Wed May 22 00:26:05 2024, max compression
```

## Comparing `gemini_webapi-1.2.0.tar` & `gemini_webapi-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.927631 gemini_webapi-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.github/workflows/github-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/assets/banner.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.927631 gemini_webapi-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/src/gemini_webapi/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20288 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.931631 gemini_webapi-1.2.0/src/gemini_webapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/types/modeloutput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/src/gemini_webapi/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/get_access_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/load_browser_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/rotate_1psidts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/src/gemini_webapi/utils/upload_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-28 09:01:25.000000 gemini_webapi-1.2.0/src/gemini_webapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 09:01:25.935631 gemini_webapi-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_client_features.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_rotate_cookies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-28 09:01:21.000000 gemini_webapi-1.2.0/tests/test_save_image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.488650 gemini_webapi-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.github/workflows/github-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)   149995 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/assets/banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.488650 gemini_webapi-1.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/src/gemini_webapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20341 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.492650 gemini_webapi-1.3.0/src/gemini_webapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/types/modeloutput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/src/gemini_webapi/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/get_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/load_browser_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/rotate_1psidts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/src/gemini_webapi/utils/upload_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    55181 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 00:26:05.000000 gemini_webapi-1.3.0/src/gemini_webapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 00:26:05.496650 gemini_webapi-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_client_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_rotate_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-22 00:26:00.000000 gemini_webapi-1.3.0/tests/test_save_image.py
```

### Comparing `gemini_webapi-1.2.0/.github/workflows/pypi-publish.yml` & `gemini_webapi-1.3.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/.gitignore` & `gemini_webapi-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/LICENSE` & `gemini_webapi-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/PKG-INFO` & `gemini_webapi-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.2.0
+Version: 1.3.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.2.0/README.md` & `gemini_webapi-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/assets/banner.png` & `gemini_webapi-1.3.0/assets/banner.png`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/assets/logo.svg` & `gemini_webapi-1.3.0/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/pyproject.toml` & `gemini_webapi-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/client.py` & `gemini_webapi-1.3.0/src/gemini_webapi/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,23 +345,24 @@
                     "Failed to generate contents. Invalid response data received. Client will try to re-initialize on next request."
                 )
 
             try:
                 candidates = []
                 for candidate in body[4]:
                     web_images = (
-                        candidate[4]
+                        candidate[12]
+                        and candidate[12][1]
                         and [
                             WebImage(
                                 url=image[0][0][0],
-                                title=image[2],
+                                title=image[7][0],
                                 alt=image[0][4],
                                 proxies=self.proxies,
                             )
-                            for image in candidate[4]
+                            for image in candidate[12][1]
                         ]
                         or []
                     )
                     generated_images = (
                         candidate[12]
                         and candidate[12][7]
                         and candidate[12][7][0]
```

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/constants.py` & `gemini_webapi-1.3.0/src/gemini_webapi/constants.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/exceptions.py` & `gemini_webapi-1.3.0/src/gemini_webapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/types/candidate.py` & `gemini_webapi-1.3.0/src/gemini_webapi/types/candidate.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/types/image.py` & `gemini_webapi-1.3.0/src/gemini_webapi/types/image.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/types/modeloutput.py` & `gemini_webapi-1.3.0/src/gemini_webapi/types/modeloutput.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/utils/get_access_token.py` & `gemini_webapi-1.3.0/src/gemini_webapi/utils/get_access_token.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/utils/load_browser_cookies.py` & `gemini_webapi-1.3.0/src/gemini_webapi/utils/load_browser_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/utils/logger.py` & `gemini_webapi-1.3.0/src/gemini_webapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/utils/rotate_1psidts.py` & `gemini_webapi-1.3.0/src/gemini_webapi/utils/rotate_1psidts.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi/utils/upload_file.py` & `gemini_webapi-1.3.0/src/gemini_webapi/utils/upload_file.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi.egg-info/PKG-INFO` & `gemini_webapi-1.3.0/src/gemini_webapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gemini-webapi
-Version: 1.2.0
+Version: 1.3.0
 Summary: ✨ An elegant async Python wrapper for Google Gemini web app
 Author: UZQueen
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `gemini_webapi-1.2.0/src/gemini_webapi.egg-info/SOURCES.txt` & `gemini_webapi-1.3.0/src/gemini_webapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/tests/test_client_features.py` & `gemini_webapi-1.3.0/tests/test_client_features.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/tests/test_rotate_cookies.py` & `gemini_webapi-1.3.0/tests/test_rotate_cookies.py`

 * *Files identical despite different names*

### Comparing `gemini_webapi-1.2.0/tests/test_save_image.py` & `gemini_webapi-1.3.0/tests/test_save_image.py`

 * *Files identical despite different names*

