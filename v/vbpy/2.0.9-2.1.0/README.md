# Comparing `tmp/vbpy-2.0.9.tar.gz` & `tmp/vbpy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-2.0.9.tar", last modified: Tue May 21 08:25:57 2024, max compression
+gzip compressed data, was "vbpy-2.1.0.tar", last modified: Wed May 22 08:09:56 2024, max compression
```

## Comparing `vbpy-2.0.9.tar` & `vbpy-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.500000 vbpy-2.0.9/
--rw-rw-rw-   0        0        0      122 2024-05-21 08:25:58.000000 vbpy-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-21 08:25:58.000000 vbpy-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0      536 2024-05-21 08:25:28.000000 vbpy-2.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.540000 vbpy-2.0.9/vbpy/
--rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.9/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.9/vbpy/combine_data_file.py
--rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.0.9/vbpy/load_claim_auto_file.py
--rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.9/vbpy/load_revenue_auto_file.py
-drwxrwxrwx   0        0        0        0 2024-05-21 08:25:57.580000 vbpy-2.0.9/vbpy.egg-info/
--rw-rw-rw-   0        0        0      122 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 08:25:58.000000 vbpy-2.0.9/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.210000 vbpy-2.1.0/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:09:58.000000 vbpy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:09:58.000000 vbpy-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-22 08:09:32.000000 vbpy-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.240000 vbpy-2.1.0/vbpy/
+-rw-rw-rw-   0        0        0      204 2024-05-22 08:09:12.000000 vbpy-2.1.0/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.1.0/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0     1034 2024-05-22 08:07:54.000000 vbpy-2.1.0/vbpy/load_channel_data_file.py
+-rw-rw-rw-   0        0        0    18200 2024-05-21 08:25:22.000000 vbpy-2.1.0/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14873 2024-05-22 07:54:10.000000 vbpy-2.1.0/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:09:56.280000 vbpy-2.1.0/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-05-22 08:09:58.000000 vbpy-2.1.0/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 08:09:56.000000 vbpy-2.1.0/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-2.0.9/setup.py` & `vbpy-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='2.0.9',
+    version='2.1.0',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-2.0.9/vbpy/combine_data_file.py` & `vbpy-2.1.0/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.0.9/vbpy/load_claim_auto_file.py` & `vbpy-2.1.0/vbpy/load_claim_auto_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-2.0.9/vbpy/load_revenue_auto_file.py` & `vbpy-2.1.0/vbpy/load_revenue_auto_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,14 +204,32 @@
                     df.loc[~df['SO_BIEN_XE'].str.match(pattern, na = False), 'SO_BIEN_XE'] = pd.NA
                     
                     print(f'   Changed: {sum(df['SO_BIEN_XE'] == _copy)} values')
                     print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
                     del _copy
                     
                     
+                    """ REPLACE BLANKS WITH NAs """
+                    print("--------------------------------------------------------------------------\nReplacing Blanks:")
+                    def replace_blanks(x):
+                        if isinstance(x, str) and x.strip() == '':
+                            return np.nan
+                        else:
+                            return x
+                        
+                    for col in df.columns:
+                        col_copy = df[col].copy()
+                        df[col] = df[col].apply(replace_blanks)
+                        replaced = (col_copy != df[col]).sum()
+                        if replaced > 0:
+                            print(f"   Converted {replaced} values in {col}")
+                    
+                    del col_copy
+                    
+                    
                     """ PRINT EFF_YEAR COUNTS IN EACH DF"""
                     print("--------------------------------------------------------------------------\nEff Year Count:")
                     df['NAM_HL'] = df['NGAY_HL'].dt.year 
                     print(f"Effective Year Count in CY{year}: {df['NAM_HL'].value_counts()}")
                     
                     
                     """ SAVE DF TO GLOBAL VARIABLE"""
```

