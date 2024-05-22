# Comparing `tmp/pytech_zp-0.1.0.tar.gz` & `tmp/pytech_zp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytech_zp-0.1.0.tar", last modified: Tue May 21 12:39:11 2024, max compression
+gzip compressed data, was "pytech_zp-0.1.1.tar", last modified: Tue May 21 15:07:03 2024, max compression
```

## Comparing `pytech_zp-0.1.0.tar` & `pytech_zp-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.247542 pytech_zp-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-05-13 10:56:51.000000 pytech_zp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       33 2024-05-13 11:16:04.000000 pytech_zp-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1914 2024-05-21 12:39:11.245541 pytech_zp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-05-13 10:55:50.000000 pytech_zp-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.231541 pytech_zp-0.1.0/getpricedata/
--rw-rw-rw-   0        0        0       41 2024-05-21 11:43:07.000000 pytech_zp-0.1.0/getpricedata/__init__.py
--rw-rw-rw-   0        0        0     1398 2024-05-17 08:27:09.000000 pytech_zp-0.1.0/getpricedata/getETFprice.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.234540 pytech_zp-0.1.0/pytech/
--rw-rw-rw-   0        0        0       36 2024-05-14 02:16:03.000000 pytech_zp-0.1.0/pytech/__init__.py
--rw-rw-rw-   0        0        0   413696 2024-05-21 11:32:00.000000 pytech_zp-0.1.0/pytech/pytech.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2024-05-21 12:39:11.243540 pytech_zp-0.1.0/pytech_zp.egg-info/
--rw-rw-rw-   0        0        0     1914 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-21 12:39:11.000000 pytech_zp-0.1.0/pytech_zp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 12:39:11.247542 pytech_zp-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      664 2024-05-21 12:38:15.000000 pytech_zp-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:07:03.169697 pytech_zp-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 10:56:51.000000 pytech_zp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2024-05-13 11:16:04.000000 pytech_zp-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     9882 2024-05-21 15:07:03.167695 pytech_zp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8300 2024-05-21 14:48:18.000000 pytech_zp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:07:03.154695 pytech_zp-0.1.1/getpricedata/
+-rw-rw-rw-   0        0        0       41 2024-05-21 11:43:07.000000 pytech_zp-0.1.1/getpricedata/__init__.py
+-rw-rw-rw-   0        0        0     1398 2024-05-17 08:27:09.000000 pytech_zp-0.1.1/getpricedata/getETFprice.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:07:03.156695 pytech_zp-0.1.1/pytech/
+-rw-rw-rw-   0        0        0       36 2024-05-14 02:16:03.000000 pytech_zp-0.1.1/pytech/__init__.py
+-rw-rw-rw-   0        0        0   413696 2024-05-21 15:04:20.000000 pytech_zp-0.1.1/pytech/pytech.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2024-05-21 15:07:03.166697 pytech_zp-0.1.1/pytech_zp.egg-info/
+-rw-rw-rw-   0        0        0     9882 2024-05-21 15:07:03.000000 pytech_zp-0.1.1/pytech_zp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2024-05-21 15:07:03.000000 pytech_zp-0.1.1/pytech_zp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:07:03.000000 pytech_zp-0.1.1/pytech_zp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 15:07:03.000000 pytech_zp-0.1.1/pytech_zp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-21 15:07:03.000000 pytech_zp-0.1.1/pytech_zp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:07:03.169697 pytech_zp-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      682 2024-05-21 15:00:04.000000 pytech_zp-0.1.1/setup.py
```

### Comparing `pytech_zp-0.1.0/LICENSE` & `pytech_zp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytech_zp-0.1.0/getpricedata/getETFprice.py` & `pytech_zp-0.1.1/getpricedata/getETFprice.py`

 * *Files identical despite different names*

### Comparing `pytech_zp-0.1.0/setup.py` & `pytech_zp-0.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
   
 setup(  
     name='pytech-zp',  
-    version='0.1.0',  
+    version='0.1.1',  
     author='Peng Zhao',
     author_email='zhaokehan86@163.com',
     description='Python function package of technical indicators and patterns implemented by C++',
     packages=find_packages(),
     include_package_data=True,
     package_data={'pytech': ['*.pyd']},
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     license=open('LICENSE').read(),
     install_requires=[
         'numpy',
         'pandas',
         'pyodbc'],
     # 其他必要信息，如 author, description, license 等
```

