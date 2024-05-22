# Comparing `tmp/direnumerate-4.0a1.tar.gz` & `tmp/direnumerate-4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-4.0a1.tar", last modified: Wed May 22 03:09:39 2024, max compression
+gzip compressed data, was "direnumerate-4.0a2.tar", last modified: Wed May 22 15:10:30 2024, max compression
```

## Comparing `direnumerate-4.0a1.tar` & `direnumerate-4.0a2.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.405815 direnumerate-4.0a1/
--rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-22 01:51:31.000000 direnumerate-4.0a1/LICENSE
--rw-r--r--   0 juan      (1000) juan      (1000)     3707 2024-05-22 03:09:39.401815 direnumerate-4.0a1/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)     2282 2024-05-22 01:52:16.000000 direnumerate-4.0a1/README.md
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.393814 direnumerate-4.0a1/direnumerate/
--rw-rw-r--   0 juan      (1000) juan      (1000)      553 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/__init__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    16553 2024-05-22 03:07:23.000000 direnumerate-4.0a1/direnumerate/__main__.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/banner.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     3401 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/cli.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/colors.py
--rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/createlist.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/exceptions.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      170 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/getinfo.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/help.py
--rw-rw-r--   0 juan      (1000) juan      (1000)     2966 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/ipcalculator.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       78 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-22 03:08:07.000000 direnumerate-4.0a1/direnumerate/version.py
--rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/warning.py
-drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.401815 direnumerate-4.0a1/direnumerate.egg-info/
--rw-r--r--   0 juan      (1000) juan      (1000)     3707 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 juan      (1000) juan      (1000)      577 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-22 03:08:00.000000 direnumerate-4.0a1/pyproject.toml
--rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-22 03:09:39.405815 direnumerate-4.0a1/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.477868 direnumerate-4.0a2/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-22 13:02:07.000000 direnumerate-4.0a2/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3707 2024-05-22 15:10:30.473868 direnumerate-4.0a2/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2282 2024-05-22 13:03:37.000000 direnumerate-4.0a2/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.469868 direnumerate-4.0a2/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     7822 2024-05-22 15:08:55.000000 direnumerate-4.0a2/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-22 15:09:05.000000 direnumerate-4.0a2/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3401 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/exceptions.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/help.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2013 2024-05-22 15:09:00.000000 direnumerate-4.0a2/direnumerate/port_scan.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       73 2024-05-22 13:04:21.000000 direnumerate-4.0a2/direnumerate/version.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-22 13:02:07.000000 direnumerate-4.0a2/direnumerate/warning.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-22 15:10:30.473868 direnumerate-4.0a2/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3707 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      515 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-22 15:10:30.000000 direnumerate-4.0a2/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1567 2024-05-22 15:09:12.000000 direnumerate-4.0a2/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-22 15:10:30.477868 direnumerate-4.0a2/setup.cfg
```

### Comparing `direnumerate-4.0a1/LICENSE` & `direnumerate-4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/PKG-INFO` & `direnumerate-4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a1
+Version: 4.0a2
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a2 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a1/README.md` & `direnumerate-4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/direnumerate/__init__.py` & `direnumerate-4.0a2/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/direnumerate/cli.py` & `direnumerate-4.0a2/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/direnumerate/createlist.py` & `direnumerate-4.0a2/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/direnumerate/help.py` & `direnumerate-4.0a2/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-4.0a1/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0a2/direnumerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 4.0a1
+Version: 4.0a2
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 4.0a1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a2 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-4.0a1/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0a2/direnumerate.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 direnumerate/__init__.py
 direnumerate/__main__.py
 direnumerate/banner.py
 direnumerate/cli.py
 direnumerate/colors.py
 direnumerate/createlist.py
 direnumerate/exceptions.py
-direnumerate/getinfo.py
 direnumerate/help.py
-direnumerate/ipcalculator.py
-direnumerate/list_urls_accounts.py
+direnumerate/port_scan.py
 direnumerate/version.py
 direnumerate/warning.py
 direnumerate.egg-info/PKG-INFO
 direnumerate.egg-info/SOURCES.txt
 direnumerate.egg-info/dependency_links.txt
 direnumerate.egg-info/entry_points.txt
 direnumerate.egg-info/requires.txt
```

### Comparing `direnumerate-4.0a1/pyproject.toml` & `direnumerate-4.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "4.0a1"
+version = "4.0a2"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

