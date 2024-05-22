# Comparing `tmp/f5_sphinx_theme-2.6.0.tar.gz` & `tmp/f5_sphinx_theme-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-a381fsp4/f5_sphinx_theme-2.6.0.tar", last modified: Mon May  6 18:23:23 2024, max compression
+gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-__jpqoa3/f5_sphinx_theme-2.6.1.tar", last modified: Wed May 22 20:41:14 2024, max compression
```

## Comparing `f5_sphinx_theme-2.6.0.tar` & `f5_sphinx_theme-2.6.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/extralinks.html
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/CoveoFullSearch.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap-theme.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/f5-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   122826 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/f5.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaBold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaThin.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/
--rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/bootstrap.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/bootstrap.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/clouddocs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/feedback.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/jquery.appear.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/printThis.js
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 18:23:03.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 18:23:23.000000 f5_sphinx_theme-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-06 18:22:56.000000 f5_sphinx_theme-2.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/extralinks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/CoveoFullSearch.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap-theme.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/f5-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   122826 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/f5.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaBold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaThin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/bootstrap.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/bootstrap.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/clouddocs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/feedback.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/jquery.appear.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/printThis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:40:53.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 20:41:14.000000 f5_sphinx_theme-2.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-22 20:40:50.000000 f5_sphinx_theme-2.6.1/setup.py
```

### Comparing `f5_sphinx_theme-2.6.0/LICENSE` & `f5_sphinx_theme-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/PKG-INFO` & `f5_sphinx_theme-2.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5_sphinx_theme
-Version: 2.6.0
+Version: 2.6.1
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.6.0/README.rst` & `f5_sphinx_theme-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/__init__.py` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from os import path
 
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 
 
 def get_html_theme_path():
     """Return the html theme path for this template library.
 
     :returns: List of directories to find template files in
     """
```

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/globaltoc.html` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/globaltoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/head.html` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/head.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/layout.html` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/localtoc.html` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/localtoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/searchbox.html` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/CoveoFullSearch.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/CoveoFullSearch.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap-theme.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/bootstrap.min.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/custom.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/f5-theme.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/f5-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/css/f5.css` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/css/f5.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaBold.woff` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaBold.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaBold.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaMedium.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaThin.woff` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaThin.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/ProximaThin.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/bootstrap.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/bootstrap.min.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/clouddocs.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/clouddocs.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/feedback.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/feedback.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/jquery.appear.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/jquery.appear.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme/static/js/printThis.js` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme/static/js/printThis.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/PKG-INFO` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5-sphinx-theme
-Version: 2.6.0
+Version: 2.6.1
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.6.0/f5_sphinx_theme.egg-info/SOURCES.txt` & `f5_sphinx_theme-2.6.1/f5_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.6.0/setup.py` & `f5_sphinx_theme-2.6.1/setup.py`

 * *Files identical despite different names*

