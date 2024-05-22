# Comparing `tmp/Fr1997v011-1.6.1.tar.gz` & `tmp/Fr1997v011-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fr1997v011-1.6.1.tar", last modified: Wed May 22 06:16:53 2024, max compression
+gzip compressed data, was "Fr1997v011-1.6.3.tar", last modified: Wed May 22 06:34:41 2024, max compression
```

## Comparing `Fr1997v011-1.6.1.tar` & `Fr1997v011-1.6.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 06:16:53.308129 Fr1997v011-1.6.1/
-drwxrwxrwx   0        0        0        0 2024-05-22 06:16:53.298128 Fr1997v011-1.6.1/Fr1997v011.egg-info/
--rw-rw-rw-   0        0        0      182 2024-05-22 06:16:53.000000 Fr1997v011-1.6.1/Fr1997v011.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-22 06:16:53.000000 Fr1997v011-1.6.1/Fr1997v011.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 06:16:53.000000 Fr1997v011-1.6.1/Fr1997v011.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 06:16:53.000000 Fr1997v011-1.6.1/Fr1997v011.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2024-05-22 06:16:53.000000 Fr1997v011-1.6.1/Fr1997v011.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.1/LICENSE
--rw-rw-rw-   0        0        0      182 2024-05-22 06:16:53.307129 Fr1997v011-1.6.1/PKG-INFO
--rw-rw-rw-   0        0        0      773 2024-05-22 06:16:42.000000 Fr1997v011-1.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 06:16:53.299128 Fr1997v011-1.6.1/fr1997_mode/
--rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.1/fr1997_mode/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:16:53.302130 Fr1997v011-1.6.1/fr1997_mode/mode_func/
--rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.1/fr1997_mode/mode_func/__init__.py
--rw-rw-rw-   0        0        0   161601 2024-05-22 01:12:48.000000 Fr1997v011-1.6.1/fr1997_mode/mode_func/all_func.py
-drwxrwxrwx   0        0        0        0 2024-05-22 06:16:53.305129 Fr1997v011-1.6.1/fr1997_mode/mode_static/
--rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.1/fr1997_mode/mode_static/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-22 06:16:53.308129 Fr1997v011-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      322 2024-05-22 06:16:42.000000 Fr1997v011-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.795069 Fr1997v011-1.6.3/
+drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.790076 Fr1997v011-1.6.3/Fr1997v011.egg-info/
+-rw-rw-rw-   0        0        0      182 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/Fr1997v011.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-10-08 06:35:50.000000 Fr1997v011-1.6.3/LICENSE
+-rw-rw-rw-   0        0        0      182 2024-05-22 06:34:41.794176 Fr1997v011-1.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      773 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.791077 Fr1997v011-1.6.3/fr1997_mode/
+-rw-rw-rw-   0        0        0       56 2023-10-11 07:25:55.000000 Fr1997v011-1.6.3/fr1997_mode/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.792076 Fr1997v011-1.6.3/fr1997_mode/mode_func/
+-rw-rw-rw-   0        0        0       29 2024-04-25 01:03:20.000000 Fr1997v011-1.6.3/fr1997_mode/mode_func/__init__.py
+-rw-rw-rw-   0        0        0   161601 2024-05-22 01:12:48.000000 Fr1997v011-1.6.3/fr1997_mode/mode_func/all_func.py
+drwxrwxrwx   0        0        0        0 2024-05-22 06:34:41.793156 Fr1997v011-1.6.3/fr1997_mode/mode_static/
+-rw-rw-rw-   0        0        0        0 2023-10-13 07:18:36.000000 Fr1997v011-1.6.3/fr1997_mode/mode_static/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 06:34:41.795069 Fr1997v011-1.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      322 2024-05-22 06:34:41.000000 Fr1997v011-1.6.3/setup.py
```

### Comparing `Fr1997v011-1.6.1/LICENSE` & `Fr1997v011-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Fr1997v011-1.6.1/README.md` & `Fr1997v011-1.6.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ```sh
 python setup.py sdist
 ```
 
 ### （本地）安装包
 
 ```sh
-pip install dist/Fr1997v011-1.6.1.tar.gz
+pip install dist/Fr1997v011-1.6.3.tar.gz
 ```
 
 ### 下载包
 
 ```sh
 pip install Fr1997v011
 ```
```

### Comparing `Fr1997v011-1.6.1/fr1997_mode/mode_func/all_func.py` & `Fr1997v011-1.6.3/fr1997_mode/mode_func/all_func.py`

 * *Files identical despite different names*

