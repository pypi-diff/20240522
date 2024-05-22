# Comparing `tmp/vbpy-2.1.2.tar.gz` & `tmp/vbpy-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.1.2.tar", last modified: Wed May 22 08:18:59 2024, max compression
+gzip compressed data, was "vbpy-2.1.3.tar", last modified: Wed May 22 08:23:50 2024, max compression
```

## Comparing `vbpy-2.1.2.tar` & `vbpy-2.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 08:18:59.010000 vbpy-2.1.2/
--rw-rw-rw-   0        0        0      122 2024-05-22 08:19:00.000000 vbpy-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 08:19:00.000000 vbpy-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 08:18:54.000000 vbpy-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:18:59.050000 vbpy-2.1.2/vbpy/
--rw-rw-rw-   0        0        0      204 2024-05-22 08:09:12.000000 vbpy-2.1.2/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.1.2/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:17:56.000000 vbpy-2.1.2/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.1.2/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.1.2/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:18:59.080000 vbpy-2.1.2/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 08:19:00.000000 vbpy-2.1.2/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-22 08:19:00.000000 vbpy-2.1.2/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 08:19:00.000000 vbpy-2.1.2/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 08:19:00.000000 vbpy-2.1.2/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:50.750000 vbpy-2.1.3/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:23:52.000000 vbpy-2.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:23:52.000000 vbpy-2.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 08:23:34.000000 vbpy-2.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:50.790000 vbpy-2.1.3/vbpy/
+-rw-rw-rw-   0        0        0      204 2024-05-22 08:09:12.000000 vbpy-2.1.3/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.1.3/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.1.3/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.1.3/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.1.3/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:50.830000 vbpy-2.1.3/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:23:52.000000 vbpy-2.1.3/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-22 08:23:52.000000 vbpy-2.1.3/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:23:52.000000 vbpy-2.1.3/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 08:23:52.000000 vbpy-2.1.3/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.1.2/setup.py` & `vbpy-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.1.2',
+    version='2.1.3',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.1.2/vbpy/combine_data_file.py` & `vbpy-2.1.3/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.1.2/vbpy/load_channel_data_file.py` & `vbpy-2.1.3/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.1.2/vbpy/load_claim_auto_file.py` & `vbpy-2.1.3/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.1.2/vbpy/load_revenue_auto_file.py` & `vbpy-2.1.3/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

