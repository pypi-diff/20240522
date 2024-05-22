# Comparing `tmp/vbpy-2.0.8.tar.gz` & `tmp/vbpy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.0.8.tar", last modified: Tue May 21 07:54:37 2024, max compression
+gzip compressed data, was "vbpy-2.0.9.tar", last modified: Tue May 21 08:25:57 2024, max compression
```

## Comparing `vbpy-2.0.8.tar` & `vbpy-2.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.680000 vbpy-2.0.8/
--rw-rw-rw-   0        0        0      122 2024-05-21 07:54:38.000000 vbpy-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-21 07:54:38.000000 vbpy-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-21 07:53:58.000000 vbpy-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.710000 vbpy-2.0.8/vbpy/
--rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.8/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.8/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0    17970 2024-05-21 07:53:50.000000 vbpy-2.0.8/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.8/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-21 07:54:37.750000 vbpy-2.0.8/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 07:54:38.000000 vbpy-2.0.8/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.500000 vbpy-2.0.9/
+-rw-rw-rw-   0        0        0      122 2024-05-21 08:25:58.000000 vbpy-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-21 08:25:58.000000 vbpy-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-21 08:25:28.000000 vbpy-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.540000 vbpy-2.0.9/vbpy/
+-rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.9/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.9/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.0.9/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.9/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.580000 vbpy-2.0.9/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.0.8/setup.py` & `vbpy-2.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.0.8',
+    version='2.0.9',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.0.8/vbpy/combine_data_file.py` & `vbpy-2.0.9/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.0.8/vbpy/load_claim_auto_file.py` & `vbpy-2.0.9/vbpy/load_claim_auto_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,19 @@
                     for col in removed_cols:
                         if col in df.columns:
                             df.drop(columns=col, inplace=True)
                         else:
                             print(f"   Column {col} not found in DataFrame.")                       
 
 
+                    """ ADD COLUMN FOR DATA YEAR"""
+                    print("--------------------------------------------------------------------------\nAdding Column NAM_DATA:")
+                    df['NAM_DATA'] = year
+
+
                     """ FILTER FOR LHNV"""
                     if lhnv:
                         print("--------------------------------------------------------------------------\nFiltering for LHNV:")    
                         rows_b4 = df.shape[0]    
                         df = df[df['MA_LHNV'] == lhnv]
                         print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
```

### Comparing `vbpy-2.0.8/vbpy/load_revenue_auto_file.py` & `vbpy-2.0.9/vbpy/load_revenue_auto_file.py`

 * *Files identical despite different names*

