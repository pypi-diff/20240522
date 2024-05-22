# Comparing `tmp/ewah_bool_utils-1.2.0b1.tar.gz` & `tmp/ewah_bool_utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ewah_bool_utils-1.2.0b1.tar", last modified: Tue Mar 12 12:46:02 2024, max compression
+gzip compressed data, was "ewah_bool_utils-1.2.1.tar", last modified: Wed May 22 20:11:05 2024, max compression
```

## Comparing `ewah_bool_utils-1.2.0b1.tar` & `ewah_bool_utils-1.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.865620 ewah_bool_utils-1.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-12 12:46:02.865620 ewah_bool_utils-1.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.861620 ewah_bool_utils-1.2.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4968 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.861620 ewah_bool_utils-1.2.0b1/ewah_bool_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/_testing.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.861620 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/README
--rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/boolarray.h
--rw-r--r--   0 runner    (1001) docker     (127)    58615 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewah-inl.h
--rw-r--r--   0 runner    (1001) docker     (127)    21434 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewah.h
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewahutil.h
--rw-r--r--   0 runner    (1001) docker     (127)    16263 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/runninglengthword.h
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_array.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_wrap.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    74091 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_wrap.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/morton_utils.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/morton_utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.865620 ewah_bool_utils-1.2.0b1/ewah_bool_utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils/tests/test_ewah_bool_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 12:46:02.865620 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-03-12 12:46:02.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-12 12:46:02.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 12:46:02.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-12 12:46:02.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-12 12:46:02.000000 ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 12:46:02.865620 ewah_bool_utils-1.2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/setupext.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-12 12:45:51.000000 ewah_bool_utils-1.2.0b1/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.097511 ewah_bool_utils-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 20:11:05.097511 ewah_bool_utils-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.093511 ewah_bool_utils-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4966 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.093511 ewah_bool_utils-1.2.1/ewah_bool_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/_testing.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.093511 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/README
+-rw-r--r--   0 runner    (1001) docker     (127)    13538 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/boolarray.h
+-rw-r--r--   0 runner    (1001) docker     (127)    58615 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewah-inl.h
+-rw-r--r--   0 runner    (1001) docker     (127)    21434 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewah.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewahutil.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16263 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/runninglengthword.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_array.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_wrap.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    74091 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_wrap.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/morton_utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/morton_utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.097511 ewah_bool_utils-1.2.1/ewah_bool_utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/ewah_bool_utils/tests/test_ewah_bool_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:11:05.097511 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-22 20:11:05.000000 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-22 20:11:05.000000 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:11:05.000000 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:11:05.000000 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 20:11:05.000000 ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:11:05.097511 ewah_bool_utils-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/setupext.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 20:10:54.000000 ewah_bool_utils-1.2.1/test_requirements.txt
```

### Comparing `ewah_bool_utils-1.2.0b1/CONTRIBUTING.rst` & `ewah_bool_utils-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/HISTORY.rst` & `ewah_bool_utils-1.2.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/LICENSE` & `ewah_bool_utils-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/MANIFEST.in` & `ewah_bool_utils-1.2.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/PKG-INFO` & `ewah_bool_utils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewah_bool_utils
-Version: 1.2.0b1
+Version: 1.2.1
 Summary: EWAH Bool Array utils for yt
 Author: Matthew Turk, Meagan Lang, Navaneeth Suresh
 License: BSD
 Project-URL: Homepage, https://github.com/yt-project/ewah_bool_utils
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ewah_bool_utils-1.2.0b1/README.rst` & `ewah_bool_utils-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/docs/Makefile` & `ewah_bool_utils-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/docs/conf.py` & `ewah_bool_utils-1.2.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = "1.2"
 # The full version, including alpha/beta/rc tags.
-release = "1.2.0b1"
+release = "1.2.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `ewah_bool_utils-1.2.0b1/docs/installation.rst` & `ewah_bool_utils-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/docs/make.bat` & `ewah_bool_utils-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/docs/usage.rst` & `ewah_bool_utils-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/_testing.pyx` & `ewah_bool_utils-1.2.1/ewah_bool_utils/_testing.pyx`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/LICENSE` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/boolarray.h` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/boolarray.h`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewah-inl.h` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewah-inl.h`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewah.h` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewah.h`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/ewahutil.h` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/ewahutil.h`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/cpp/runninglengthword.h` & `ewah_bool_utils-1.2.1/ewah_bool_utils/cpp/runninglengthword.h`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_array.pxd` & `ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_array.pxd`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_wrap.pxd` & `ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_wrap.pxd`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/ewah_bool_wrap.pyx` & `ewah_bool_utils-1.2.1/ewah_bool_utils/ewah_bool_wrap.pyx`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/morton_utils.pxd` & `ewah_bool_utils-1.2.1/ewah_bool_utils/morton_utils.pxd`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/morton_utils.pyx` & `ewah_bool_utils-1.2.1/ewah_bool_utils/morton_utils.pyx`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils/tests/test_ewah_bool_utils.py` & `ewah_bool_utils-1.2.1/ewah_bool_utils/tests/test_ewah_bool_utils.py`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/PKG-INFO` & `ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewah_bool_utils
-Version: 1.2.0b1
+Version: 1.2.1
 Summary: EWAH Bool Array utils for yt
 Author: Matthew Turk, Meagan Lang, Navaneeth Suresh
 License: BSD
 Project-URL: Homepage, https://github.com/yt-project/ewah_bool_utils
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ewah_bool_utils-1.2.0b1/ewah_bool_utils.egg-info/SOURCES.txt` & `ewah_bool_utils-1.2.1/ewah_bool_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/pyproject.toml` & `ewah_bool_utils-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = [
     "setuptools>=61.2",
     "Cython>=3.0",
-    "numpy>=2.0.0b1",
+    "numpy>=2.0.0rc1",
 ]
 
 [project]
 name = "ewah_bool_utils"
-version = "1.2.0b1"
+version = "1.2.1"
 description = "EWAH Bool Array utils for yt"
 authors = [
   { name = "Matthew Turk" },
   { name = "Meagan Lang" },
   { name = "Navaneeth Suresh" },
 ]
 requires-python =">=3.9"
```

### Comparing `ewah_bool_utils-1.2.0b1/setup.py` & `ewah_bool_utils-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `ewah_bool_utils-1.2.0b1/setupext.py` & `ewah_bool_utils-1.2.1/setupext.py`

 * *Files identical despite different names*

