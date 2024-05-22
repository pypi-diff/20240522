# Comparing `tmp/pyxtream-0.7.0.tar.gz` & `tmp/pyxtream-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxtream-0.7.0.tar", last modified: Tue Dec 12 05:43:20 2023, max compression
+gzip compressed data, was "pyxtream-0.7.1.tar", last modified: Wed May 22 05:25:24 2024, max compression
```

## Comparing `pyxtream-0.7.0.tar` & `pyxtream-0.7.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2023-12-12 05:43:20.344805 pyxtream-0.7.0/
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)    35149 2021-06-05 03:13:35.000000 pyxtream-0.7.0/LICENSE
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     5588 2023-12-12 05:43:20.344805 pyxtream-0.7.0/PKG-INFO
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     4939 2023-12-12 05:34:53.000000 pyxtream-0.7.0/README.md
-drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2023-12-12 05:43:20.344805 pyxtream-0.7.0/pyxtream/
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)      229 2023-11-13 04:32:38.000000 pyxtream-0.7.0/pyxtream/__init__.py
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     1612 2023-11-09 22:19:39.000000 pyxtream-0.7.0/pyxtream/progress.py
--rwxrwxr-x   0 superolmo  (1000) superolmo  (1000)    42790 2023-11-16 05:19:03.000000 pyxtream-0.7.0/pyxtream/pyxtream.py
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     3031 2023-11-09 22:19:39.000000 pyxtream-0.7.0/pyxtream/rest_api.py
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     9776 2023-11-09 22:19:39.000000 pyxtream-0.7.0/pyxtream/schemaValidator.py
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       93 2023-11-15 04:08:15.000000 pyxtream-0.7.0/pyxtream/version.py
-drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2023-12-12 05:43:20.344805 pyxtream-0.7.0/pyxtream.egg-info/
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     5588 2023-12-12 05:43:20.000000 pyxtream-0.7.0/pyxtream.egg-info/PKG-INFO
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)      317 2023-12-12 05:43:20.000000 pyxtream-0.7.0/pyxtream.egg-info/SOURCES.txt
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)        1 2023-12-12 05:43:20.000000 pyxtream-0.7.0/pyxtream.egg-info/dependency_links.txt
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       25 2023-12-12 05:43:20.000000 pyxtream-0.7.0/pyxtream.egg-info/requires.txt
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)        9 2023-12-12 05:43:20.000000 pyxtream-0.7.0/pyxtream.egg-info/top_level.txt
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       38 2023-12-12 05:43:20.344805 pyxtream-0.7.0/setup.cfg
--rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     1085 2023-11-15 04:22:45.000000 pyxtream-0.7.0/setup.py
+drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2024-05-22 05:25:24.611740 pyxtream-0.7.1/
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)    35149 2021-06-05 03:13:35.000000 pyxtream-0.7.1/LICENSE
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     5797 2024-05-22 05:25:24.607740 pyxtream-0.7.1/PKG-INFO
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     5148 2024-05-22 05:06:11.000000 pyxtream-0.7.1/README.md
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)      691 2023-12-14 14:40:57.000000 pyxtream-0.7.1/pyproject.toml
+drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2024-05-22 05:25:24.607740 pyxtream-0.7.1/pyxtream/
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)      229 2023-12-13 04:45:55.000000 pyxtream-0.7.1/pyxtream/__init__.py
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     1612 2023-12-13 04:45:55.000000 pyxtream-0.7.1/pyxtream/progress.py
+-rwxrwxr-x   0 superolmo  (1000) superolmo  (1000)    42871 2024-05-22 04:54:37.000000 pyxtream-0.7.1/pyxtream/pyxtream.py
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     3031 2023-12-13 04:45:55.000000 pyxtream-0.7.1/pyxtream/rest_api.py
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     9776 2023-12-13 04:45:55.000000 pyxtream-0.7.1/pyxtream/schemaValidator.py
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       93 2024-05-22 04:54:37.000000 pyxtream-0.7.1/pyxtream/version.py
+drwxrwxr-x   0 superolmo  (1000) superolmo  (1000)        0 2024-05-22 05:25:24.607740 pyxtream-0.7.1/pyxtream.egg-info/
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     5797 2024-05-22 05:25:24.000000 pyxtream-0.7.1/pyxtream.egg-info/PKG-INFO
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)      332 2024-05-22 05:25:24.000000 pyxtream-0.7.1/pyxtream.egg-info/SOURCES.txt
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)        1 2024-05-22 05:25:24.000000 pyxtream-0.7.1/pyxtream.egg-info/dependency_links.txt
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       25 2024-05-22 05:25:24.000000 pyxtream-0.7.1/pyxtream.egg-info/requires.txt
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)        9 2024-05-22 05:25:24.000000 pyxtream-0.7.1/pyxtream.egg-info/top_level.txt
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)       38 2024-05-22 05:25:24.611740 pyxtream-0.7.1/setup.cfg
+-rw-rw-r--   0 superolmo  (1000) superolmo  (1000)     1135 2024-05-22 05:04:06.000000 pyxtream-0.7.1/setup.py
```

### Comparing `pyxtream-0.7.0/LICENSE` & `pyxtream-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxtream-0.7.0/PKG-INFO` & `pyxtream-0.7.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: pyxtream
-Version: 0.7.0
-Summary: xtream IPTV loader
-Home-page: https://github.com/superolmo/pyxtream
-Author: Claudio Olmi
-Author-email: superolmo2@gmail.com
-License: GPL3
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Description-Content-Type: text/markdown
-Provides-Extra: REST_API
-License-File: LICENSE
-
 # PyXtream - A Python Xtream Loader
 
 PyXtream loads the xtream IPTV content from a provider server. Groups, Channels, Series are all organized in dictionaries. Season and Episodes are retrieved as needed. It includes functions for searching streams and downloading.
 
 This library was originally designed to work with Hypnotix at https://github.com/linuxmint/hypnotix
 
 # Installing
@@ -128,19 +108,18 @@
 - Increment the MINOR version when you add functionality in a backwards-compatible manner.
 - Increment the PATCH version when you make backwards-compatible bug fixes.
 
 # Change Log
 
 | Date | Version | Description |
 | ----------- | -----| ----------- |
+| 2024-05-21 | 0.7.1 | - Fixed missing jsonschema package<br>- Fixed provider name in functional_test<br>- Improved print out of connection attempts<br>- Added method to read latest changes in functional_test
 | 2023-11-08 | 0.7.0 | - Added Schema Validator<br>- Added Channel Age<br>- Added list of movies added in the last 30 and 7 days<br>- Updated code based on PyLint<br>- Fixed Flask package to be optional [richard-de-vos](https://github.com/richard-de-vos)|
 | 2023-02-06 | 0.6.0 | - Added methods to change connection header, to turn off reload timer, and to enable/disable Flask debug mode<br>- Added a loop when attempting to connect to the provider <br>- Cleaned up some print lines|
 | 2021-08-19 | 0.5.0 | - Added method to gracefully handle connection errors<br>- Added setting to not load adult content<br>- Added sorting by stream name<br>- Changed the handling of special characters in streams<br>- Changed print formatting<br>- Changed index.html webpage to HTML5 and Bootstrap 5|
 | 2021-06-19 | 0.4.0 | - Updated to follow PEP8<br>- Updated Docstrings |
 | 2021-06-19 | 0.3.0 | - Added enhanced Home Page with Search Button and Player<br>- Added case insensitive search<br>- Improved handling of provider missing fields |
 | 2021-06-11 | 0.2.1 | - Fixed bug in the way it reload from cache |
 | 2021-06-08 | 0.2.0 | - Added searching<br>- Added video download<br>- Added REST Api<br>- Fixed cache-path issue |
 | 2021-06-05 | 0.1.2 | - Fixed Server Name |
 | 2021-06-04 | 0.1.1 | - Updated README.md |
 | 2021-06-04 | 0.1.0 | - Initial Release |
-
-
```

### Comparing `pyxtream-0.7.0/README.md` & `pyxtream-0.7.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: pyxtream
+Version: 0.7.1
+Summary: xtream IPTV loader
+Home-page: https://github.com/superolmo/pyxtream
+Author: Claudio Olmi
+Author-email: superolmo2@gmail.com
+License: GPL3
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: English
+Description-Content-Type: text/markdown
+Provides-Extra: REST_API
+License-File: LICENSE
+
 # PyXtream - A Python Xtream Loader
 
 PyXtream loads the xtream IPTV content from a provider server. Groups, Channels, Series are all organized in dictionaries. Season and Episodes are retrieved as needed. It includes functions for searching streams and downloading.
 
 This library was originally designed to work with Hypnotix at https://github.com/linuxmint/hypnotix
 
 # Installing
@@ -108,17 +128,20 @@
 - Increment the MINOR version when you add functionality in a backwards-compatible manner.
 - Increment the PATCH version when you make backwards-compatible bug fixes.
 
 # Change Log
 
 | Date | Version | Description |
 | ----------- | -----| ----------- |
+| 2024-05-21 | 0.7.1 | - Fixed missing jsonschema package<br>- Fixed provider name in functional_test<br>- Improved print out of connection attempts<br>- Added method to read latest changes in functional_test
 | 2023-11-08 | 0.7.0 | - Added Schema Validator<br>- Added Channel Age<br>- Added list of movies added in the last 30 and 7 days<br>- Updated code based on PyLint<br>- Fixed Flask package to be optional [richard-de-vos](https://github.com/richard-de-vos)|
 | 2023-02-06 | 0.6.0 | - Added methods to change connection header, to turn off reload timer, and to enable/disable Flask debug mode<br>- Added a loop when attempting to connect to the provider <br>- Cleaned up some print lines|
 | 2021-08-19 | 0.5.0 | - Added method to gracefully handle connection errors<br>- Added setting to not load adult content<br>- Added sorting by stream name<br>- Changed the handling of special characters in streams<br>- Changed print formatting<br>- Changed index.html webpage to HTML5 and Bootstrap 5|
 | 2021-06-19 | 0.4.0 | - Updated to follow PEP8<br>- Updated Docstrings |
 | 2021-06-19 | 0.3.0 | - Added enhanced Home Page with Search Button and Player<br>- Added case insensitive search<br>- Improved handling of provider missing fields |
 | 2021-06-11 | 0.2.1 | - Fixed bug in the way it reload from cache |
 | 2021-06-08 | 0.2.0 | - Added searching<br>- Added video download<br>- Added REST Api<br>- Fixed cache-path issue |
 | 2021-06-05 | 0.1.2 | - Fixed Server Name |
 | 2021-06-04 | 0.1.1 | - Updated README.md |
 | 2021-06-04 | 0.1.0 | - Initial Release |
+
+
```

### Comparing `pyxtream-0.7.0/pyxtream/progress.py` & `pyxtream-0.7.1/pyxtream/progress.py`

 * *Files identical despite different names*

### Comparing `pyxtream-0.7.0/pyxtream/pyxtream.py` & `pyxtream-0.7.1/pyxtream/pyxtream.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,22 +579,23 @@
             # Erase any previous data
             self.auth_data = {}
             # Loop through 30 seconds
             i = 0
             r = None
             # Prepare the authentication url
             url = f"{self.server}/player_api.php?username={self.username}&password={self.password}"
+            print(f"Attempting connection: ", end='')
             while i < 30:
                 try:
                     # Request authentication, wait 4 seconds maximum
                     r = requests.get(url, timeout=(4), headers=self.connection_headers)
                     i = 31
                 except requests.exceptions.ConnectionError:
                     time.sleep(1)
-                    print(i)
+                    print(f"{i} ", end='',flush=True)
                     i += 1
 
             if r is not None:
                 # If the answer is ok, process data and change state
                 if r.ok:
                     self.auth_data = r.json()
                     self.authorization = {
@@ -608,15 +609,15 @@
                     # If there is a secure server connection, construct the base url SSL for all requests
                     if "https_port" in self.auth_data["server_info"]:
                         self.base_url_ssl = f"https://{self.auth_data['server_info']['url']}:{self.auth_data['server_info']['https_port']}" \
                                             f"/player_api.php?username={self.username}&password={self.password}"
                 else:
                     print(f"Provider `{self.name}` could not be loaded. Reason: `{r.status_code} {r.reason}`")
             else:
-                print(f"{self.name}: Provider refused the connection")
+                print(f"\n{self.name}: Provider refused the connection")
 
     def _load_from_file(self, filename) -> dict:
         """Try to load the dictionary from file
 
         Args:
             filename ([type]): File name containing the data
```

### Comparing `pyxtream-0.7.0/pyxtream/rest_api.py` & `pyxtream-0.7.1/pyxtream/rest_api.py`

 * *Files identical despite different names*

### Comparing `pyxtream-0.7.0/pyxtream/schemaValidator.py` & `pyxtream-0.7.1/pyxtream/schemaValidator.py`

 * *Files identical despite different names*

### Comparing `pyxtream-0.7.0/pyxtream.egg-info/PKG-INFO` & `pyxtream-0.7.1/pyxtream.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxtream
-Version: 0.7.0
+Version: 0.7.1
 Summary: xtream IPTV loader
 Home-page: https://github.com/superolmo/pyxtream
 Author: Claudio Olmi
 Author-email: superolmo2@gmail.com
 License: GPL3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -128,14 +128,15 @@
 - Increment the MINOR version when you add functionality in a backwards-compatible manner.
 - Increment the PATCH version when you make backwards-compatible bug fixes.
 
 # Change Log
 
 | Date | Version | Description |
 | ----------- | -----| ----------- |
+| 2024-05-21 | 0.7.1 | - Fixed missing jsonschema package<br>- Fixed provider name in functional_test<br>- Improved print out of connection attempts<br>- Added method to read latest changes in functional_test
 | 2023-11-08 | 0.7.0 | - Added Schema Validator<br>- Added Channel Age<br>- Added list of movies added in the last 30 and 7 days<br>- Updated code based on PyLint<br>- Fixed Flask package to be optional [richard-de-vos](https://github.com/richard-de-vos)|
 | 2023-02-06 | 0.6.0 | - Added methods to change connection header, to turn off reload timer, and to enable/disable Flask debug mode<br>- Added a loop when attempting to connect to the provider <br>- Cleaned up some print lines|
 | 2021-08-19 | 0.5.0 | - Added method to gracefully handle connection errors<br>- Added setting to not load adult content<br>- Added sorting by stream name<br>- Changed the handling of special characters in streams<br>- Changed print formatting<br>- Changed index.html webpage to HTML5 and Bootstrap 5|
 | 2021-06-19 | 0.4.0 | - Updated to follow PEP8<br>- Updated Docstrings |
 | 2021-06-19 | 0.3.0 | - Added enhanced Home Page with Search Button and Player<br>- Added case insensitive search<br>- Improved handling of provider missing fields |
 | 2021-06-11 | 0.2.1 | - Fixed bug in the way it reload from cache |
 | 2021-06-08 | 0.2.0 | - Added searching<br>- Added video download<br>- Added REST Api<br>- Fixed cache-path issue |
```

### Comparing `pyxtream-0.7.0/setup.py` & `pyxtream-0.7.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,12 +26,15 @@
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3 :: Only",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Natural Language :: English"
     ],
+    install_require=[
+        'jsonschema'
+    ],
     extras_require={
         "REST_API":  ["Flask>=1.1.2",],
     }
  )
```

