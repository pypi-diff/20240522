# Comparing `tmp/vbpy-2.2.4.tar.gz` & `tmp/vbpy-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.2.4.tar", last modified: Wed May 22 09:58:30 2024, max compression
+gzip compressed data, was "vbpy-2.2.5.tar", last modified: Wed May 22 10:01:23 2024, max compression
```

## Comparing `vbpy-2.2.4.tar` & `vbpy-2.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:58:29.990000 vbpy-2.2.4/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:58:32.000000 vbpy-2.2.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 09:58:32.000000 vbpy-2.2.4/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-22 09:58:22.000000 vbpy-2.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:58:30.030000 vbpy-2.2.4/vbpy/
--rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.4/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.4/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.4/vbpy/load_channel_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.4/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    10327 2024-05-22 09:58:00.000000 vbpy-2.2.4/vbpy/load_open_claim_auto_file.py
--rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.4/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:58:30.070000 vbpy-2.2.4/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 09:58:30.000000 vbpy-2.2.4/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.020000 vbpy-2.2.5/
+-rw-rw-rw-   0        0        0      122 2024-05-22 10:01:24.000000 vbpy-2.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:01:24.000000 vbpy-2.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 10:01:08.000000 vbpy-2.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.050000 vbpy-2.2.5/vbpy/
+-rw-rw-rw-   0        0        0      265 2024-05-22 09:16:04.000000 vbpy-2.2.5/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.2.5/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1006 2024-05-22 08:23:28.000000 vbpy-2.2.5/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.2.5/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    10324 2024-05-22 10:01:00.000000 vbpy-2.2.5/vbpy/load_open_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.2.5/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:01:23.090000 vbpy-2.2.5/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 10:01:24.000000 vbpy-2.2.5/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.2.4/setup.py` & `vbpy-2.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.2.4',
+    version='2.2.5',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.2.4/vbpy/combine_data_file.py` & `vbpy-2.2.5/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.4/vbpy/load_channel_data_file.py` & `vbpy-2.2.5/vbpy/load_channel_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.4/vbpy/load_claim_auto_file.py` & `vbpy-2.2.5/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.2.4/vbpy/load_open_claim_auto_file.py` & `vbpy-2.2.5/vbpy/load_open_claim_auto_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
                     # Set the determined headers as column names
                     df.columns = headers
                     df = df.drop([0, 1])
                     df.reset_index(drop = True, inplace=True)
                     print(f'   Rows = {df.shape[0]}')
                     # print(f'Columns = {df.shape[1]}')
-                    print(df)
+                    
             
                     """ RENAME COLUMNS"""
                     print("--------------------------------------------------------------------------\nRenaming Columns:")
                     df_clm_dict = {
                         'Số hồ sơ': 'SO_HSBT', 
                         'Ngày mở HSBT': 'NGAY_MO_HSBT',
                         'Ngày thông báo': 'NGAY_THONG_BAO',
@@ -163,18 +163,18 @@
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
                         
                         
                     
                     """ SAVE DF TO GLOBAL VARIABLE"""
                     print("--------------------------------------------------------------------------\nSaving DF:")
                     # Assign DataFrame to a global variable dynamically using the year
-                    df_name = f'df_clm_{year}'
+                    df_name = f'df_clm_{quarter}'
                     globals()[df_name] = df
                     global_df_names.append(df_name)
-                    print(f"Summary of CY{year}:\n   -NUM CLAIMS = {df.shape[0]:,.0f}\n   -TOTAL CLAIMS = {df['STBT'].sum():,.0f}")
+                    print(f"Summary of CY{quarter}:\n   -NUM CLAIMS = {df.shape[0]:,.0f}\n   -TOTAL CLAIMS = {df['STBT'].sum():,.0f}")
                     print('--------------------------------------------------------------------------\nxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx')
                     
                 except Exception as e:
                     print(f"Failed to process {file}: {e}")
             else:
                 print(f"No year found in the file name {file}")
```

### Comparing `vbpy-2.2.4/vbpy/load_revenue_auto_file.py` & `vbpy-2.2.5/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

