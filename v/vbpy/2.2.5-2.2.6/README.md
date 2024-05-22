# Comparing `tmp/vbpy-2.2.5.tar.gz` & `tmp/vbpy-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.2.5.tar", last modified: Wed May 22 10:01:23 2024, max compression
+gzip compressed data, was "vbpy-2.2.6.tar", last modified: Wed May 22 10:03:36 2024, max compression
```

## Comparing `vbpy-2.2.5.tar` & `vbpy-2.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.020000 vbpy-2.2.5/
--rw-rw-rw-   0        0        0      122 2024-05-22 10:01:24.000000 vbpy-2.2.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 10:01:24.000000 vbpy-2.2.5/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 10:01:08.000000 vbpy-2.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.050000 vbpy-2.2.5/vbpy/
--rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.5/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.5/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.5/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.5/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    10324 2024-05-22 10:01:00.000000 vbpy-2.2.5/vbpy/load_open_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.5/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.090000 vbpy-2.2.5/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 10:03:35.940000 vbpy-2.2.6/
+-rw-rw-rw-   0        0        0      122 2024-05-22 10:03:38.000000 vbpy-2.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:03:38.000000 vbpy-2.2.6/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 10:03:18.000000 vbpy-2.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:03:36.050000 vbpy-2.2.6/vbpy/
+-rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.6/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.6/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.6/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.6/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    10324 2024-05-22 10:03:12.000000 vbpy-2.2.6/vbpy/load_open_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.6/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:03:36.090000 vbpy-2.2.6/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 10:03:36.000000 vbpy-2.2.6/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-22 10:03:36.000000 vbpy-2.2.6/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:03:36.000000 vbpy-2.2.6/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 10:03:36.000000 vbpy-2.2.6/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.2.5/setup.py` & `vbpy-2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.2.5',
+    version='2.2.6',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.2.5/vbpy/combine_data_file.py` & `vbpy-2.2.6/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.5/vbpy/load_channel_data_file.py` & `vbpy-2.2.6/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.5/vbpy/load_claim_auto_file.py` & `vbpy-2.2.6/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.5/vbpy/load_open_claim_auto_file.py` & `vbpy-2.2.6/vbpy/load_open_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.5/vbpy/load_revenue_auto_file.py` & `vbpy-2.2.6/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

