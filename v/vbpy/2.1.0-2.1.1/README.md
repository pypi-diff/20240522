# Comparing `tmp/vbpy-2.1.0.tar.gz` & `tmp/vbpy-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.1.0.tar", last modified: Wed May 22 08:09:56 2024, max compression
+gzip compressed data, was "vbpy-2.1.1.tar", last modified: Wed May 22 08:13:49 2024, max compression
```

## Comparing `vbpy-2.1.0.tar` & `vbpy-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.210000 vbpy-2.1.0/
--rw-rw-rw-   0        0        0      122 2024-05-22 08:09:58.000000 vbpy-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 08:09:58.000000 vbpy-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 08:09:32.000000 vbpy-2.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.240000 vbpy-2.1.0/vbpy/
--rw-rw-rw-   0        0        0      204 2024-05-22 08:09:12.000000 vbpy-2.1.0/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.1.0/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1034 2024-05-22 08:07:54.000000 vbpy-2.1.0/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.1.0/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.1.0/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.280000 vbpy-2.1.0/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-05-22 08:09:58.000000 vbpy-2.1.0/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:13:49.520000 vbpy-2.1.1/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:13:50.000000 vbpy-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:13:50.000000 vbpy-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 08:13:22.000000 vbpy-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:13:49.550000 vbpy-2.1.1/vbpy/
+-rw-rw-rw-   0        0        0      204 2024-05-22 08:09:12.000000 vbpy-2.1.1/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.1.1/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0      986 2024-05-22 08:12:40.000000 vbpy-2.1.1/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.1.1/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.1.1/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:13:49.580000 vbpy-2.1.1/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:13:50.000000 vbpy-2.1.1/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-22 08:13:50.000000 vbpy-2.1.1/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:13:50.000000 vbpy-2.1.1/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 08:13:50.000000 vbpy-2.1.1/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.1.0/setup.py` & `vbpy-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.1.0',
+    version='2.1.1',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.1.0/vbpy/combine_data_file.py` & `vbpy-2.1.1/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.1.0/vbpy/load_channel_data_file.py` & `vbpy-2.1.1/vbpy/load_channel_data_file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 
 def load_channel_data():
-    df_channel = pd.read_excel('0. misc/.DANH SÁCH MÃ ĐẠI LÝ.xlsx')
-    df_channel.drop(df_channel.columns[-2:], axis=1, inplace=True)
-    df_channel.rename(columns = {
+    df = pd.read_excel('0. misc/.DANH SÁCH MÃ ĐẠI LÝ.xlsx')
+    df.drop(df.columns[-2:], axis=1, inplace=True)
+    df.rename(columns = {
         'Mã Đại lý': 'MA_DL',
         'Tên Đại lý': 'TEN_DL',
         'Nguồn khai thác': 'NGUON_KT',
         'Phân loại Đại lý': 'LOAI_DL',
         'Thông tin đại lý': 'THONG_TIN_DL'
     }, inplace = True)
 
@@ -23,10 +23,10 @@
         df[col] = df[col].apply(replace_blanks)
         replaced = (col_copy != df[col]).sum()
         if replaced > 0:
             print(f"   Converted {replaced} values in {col}")
     
     del col_copy
 
-    df_channel.dropna(subset = 'MA_DL', inplace = True)
+    df.dropna(subset = 'MA_DL', inplace = True)
     
-    return df_channel
+    return df
```

### Comparing `vbpy-2.1.0/vbpy/load_claim_auto_file.py` & `vbpy-2.1.1/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.1.0/vbpy/load_revenue_auto_file.py` & `vbpy-2.1.1/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

