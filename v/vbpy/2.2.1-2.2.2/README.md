# Comparing `tmp/vbpy-2.2.1.tar.gz` & `tmp/vbpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.2.1.tar", last modified: Wed May 22 09:47:01 2024, max compression
+gzip compressed data, was "vbpy-2.2.2.tar", last modified: Wed May 22 09:51:10 2024, max compression
```

## Comparing `vbpy-2.2.1.tar` & `vbpy-2.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.210000 vbpy-2.2.1/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:47:02.000000 vbpy-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 09:47:02.000000 vbpy-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 09:46:58.000000 vbpy-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.240000 vbpy-2.2.1/vbpy/
--rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.1/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.1/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.1/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.1/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    16408 2024-05-22 09:46:12.000000 vbpy-2.2.1/vbpy/load_open_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.1/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:47:01.280000 vbpy-2.2.1/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 09:47:02.000000 vbpy-2.2.1/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:51:10.100000 vbpy-2.2.2/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:51:12.000000 vbpy-2.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:51:12.000000 vbpy-2.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 09:51:06.000000 vbpy-2.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:51:10.140000 vbpy-2.2.2/vbpy/
+-rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.2/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.2/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.2/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.2/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    16425 2024-05-22 09:50:24.000000 vbpy-2.2.2/vbpy/load_open_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.2/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:51:10.180000 vbpy-2.2.2/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 09:51:10.000000 vbpy-2.2.2/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-22 09:51:12.000000 vbpy-2.2.2/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:51:10.000000 vbpy-2.2.2/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 09:51:10.000000 vbpy-2.2.2/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.2.1/setup.py` & `vbpy-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.2.1',
+    version='2.2.2',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.2.1/vbpy/combine_data_file.py` & `vbpy-2.2.2/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.1/vbpy/load_channel_data_file.py` & `vbpy-2.2.2/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.1/vbpy/load_claim_auto_file.py` & `vbpy-2.2.2/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.1/vbpy/load_open_claim_auto_file.py` & `vbpy-2.2.2/vbpy/load_open_claim_auto_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
                     # Set the determined headers as column names
                     df.columns = headers
                     df = df.drop([0])
                     df.reset_index(drop = True, inplace=True)
                     print(f'   Rows = {df.shape[0]}')
                     # print(f'Columns = {df.shape[1]}')
-            
+                    print(df)
             
                     """ RENAME COLUMNS"""
                     print("--------------------------------------------------------------------------\nRenaming Columns:")
                     df_clm_dict = {
                         'Số hồ sơ': 'SO_HSBT', 
                         'Ngày mở HSBT': 'NGAY_MO_HSBT',
                         'Ngày thông báo': 'NGAY_THONG_BAO',
```

### Comparing `vbpy-2.2.1/vbpy/load_revenue_auto_file.py` & `vbpy-2.2.2/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

