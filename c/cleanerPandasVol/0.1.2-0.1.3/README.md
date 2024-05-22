# Comparing `tmp/cleanerpandasvol-0.1.2.tar.gz` & `tmp/cleanerpandasvol-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanerpandasvol-0.1.2.tar", last modified: Tue May 21 12:58:46 2024, max compression
+gzip compressed data, was "cleanerpandasvol-0.1.3.tar", last modified: Tue May 21 13:11:57 2024, max compression
```

## Comparing `cleanerpandasvol-0.1.2.tar` & `cleanerpandasvol-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:58:46.350097 cleanerpandasvol-0.1.2/
--rw-rw-rw-   0        0        0     1082 2024-05-21 11:41:29.000000 cleanerpandasvol-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      578 2024-05-21 12:58:46.349098 cleanerpandasvol-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 12:58:46.269918 cleanerpandasvol-0.1.2/cleanerPandasVol/
--rw-rw-rw-   0        0        0      571 2024-05-21 09:59:58.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/__init__.py
--rw-rw-rw-   0        0        0      694 2024-05-21 08:54:01.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/categorical_encoder.py
--rw-rw-rw-   0        0        0      433 2024-05-21 08:54:44.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/data_type_converter.py
--rw-rw-rw-   0        0        0      486 2024-05-21 08:55:12.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/date_time_handler.py
--rw-rw-rw-   0        0        0      433 2024-05-21 08:56:02.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/feature_engineer.py
--rw-rw-rw-   0        0        0      847 2024-05-21 08:56:30.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/missing_value_handler.py
--rw-rw-rw-   0        0        0     1364 2024-05-21 08:56:56.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/outlier_handler.py
--rw-rw-rw-   0        0        0      419 2024-05-21 08:57:27.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/scaler.py
--rw-rw-rw-   0        0        0     1128 2024-05-21 08:57:55.000000 cleanerpandasvol-0.1.2/cleanerPandasVol/text_cleaner.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:58:46.347114 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/
--rw-rw-rw-   0        0        0      578 2024-05-21 12:58:46.000000 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      554 2024-05-21 12:58:46.000000 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:58:46.000000 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-21 12:58:46.000000 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-21 12:58:46.000000 cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 12:58:46.351093 cleanerpandasvol-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      715 2024-05-21 11:44:50.000000 cleanerpandasvol-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:58:46.342731 cleanerpandasvol-0.1.2/test/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:03:34.000000 cleanerpandasvol-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:11:57.569959 cleanerpandasvol-0.1.3/
+-rw-rw-rw-   0        0        0     1082 2024-05-21 11:41:29.000000 cleanerpandasvol-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      595 2024-05-21 13:11:57.569959 cleanerpandasvol-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 13:11:57.521894 cleanerpandasvol-0.1.3/cleanerPandasVol/
+-rw-rw-rw-   0        0        0      571 2024-05-21 09:59:58.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/__init__.py
+-rw-rw-rw-   0        0        0      694 2024-05-21 08:54:01.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/categorical_encoder.py
+-rw-rw-rw-   0        0        0      433 2024-05-21 08:54:44.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/data_type_converter.py
+-rw-rw-rw-   0        0        0      486 2024-05-21 08:55:12.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/date_time_handler.py
+-rw-rw-rw-   0        0        0      433 2024-05-21 08:56:02.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/feature_engineer.py
+-rw-rw-rw-   0        0        0      847 2024-05-21 08:56:30.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/missing_value_handler.py
+-rw-rw-rw-   0        0        0     1364 2024-05-21 08:56:56.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/outlier_handler.py
+-rw-rw-rw-   0        0        0      419 2024-05-21 08:57:27.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/scaler.py
+-rw-rw-rw-   0        0        0     1128 2024-05-21 08:57:55.000000 cleanerpandasvol-0.1.3/cleanerPandasVol/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:11:57.569959 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/
+-rw-rw-rw-   0        0        0      595 2024-05-21 13:11:57.000000 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2024-05-21 13:11:57.000000 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:11:57.000000 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-21 13:11:57.000000 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-21 13:11:57.000000 cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:11:57.575609 cleanerpandasvol-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      716 2024-05-21 13:11:40.000000 cleanerpandasvol-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:11:57.569330 cleanerpandasvol-0.1.3/test/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:03:34.000000 cleanerpandasvol-0.1.3/test/__init__.py
```

### Comparing `cleanerpandasvol-0.1.2/LICENSE` & `cleanerpandasvol-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/PKG-INFO` & `cleanerpandasvol-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cleanerPandasVol
-Version: 0.1.2
+Version: 0.1.3
 Summary: A comprehensive Python library for data preprocessing and cleaning
 Home-page: https://github.com/MuratKeskin0/Python_Data_Project_Vol
 Author: Murat Keskin & Ahmet Bagbakan & Cagla Ilhani
 Author-email: eng.murat.keskin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: pandas
-Requires-Dist: numpyscikit-learn
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
 Requires-Dist: nltk
```

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol/__init__.py` & `cleanerpandasvol-0.1.3/cleanerPandasVol/__init__.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol/categorical_encoder.py` & `cleanerpandasvol-0.1.3/cleanerPandasVol/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol/missing_value_handler.py` & `cleanerpandasvol-0.1.3/cleanerPandasVol/missing_value_handler.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol/outlier_handler.py` & `cleanerpandasvol-0.1.3/cleanerPandasVol/outlier_handler.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol/text_cleaner.py` & `cleanerpandasvol-0.1.3/cleanerPandasVol/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/PKG-INFO` & `cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cleanerPandasVol
-Version: 0.1.2
+Version: 0.1.3
 Summary: A comprehensive Python library for data preprocessing and cleaning
 Home-page: https://github.com/MuratKeskin0/Python_Data_Project_Vol
 Author: Murat Keskin & Ahmet Bagbakan & Cagla Ilhani
 Author-email: eng.murat.keskin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: pandas
-Requires-Dist: numpyscikit-learn
+Requires-Dist: numpy
+Requires-Dist: scikit-learn
 Requires-Dist: nltk
```

### Comparing `cleanerpandasvol-0.1.2/cleanerPandasVol.egg-info/SOURCES.txt` & `cleanerpandasvol-0.1.3/cleanerPandasVol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanerpandasvol-0.1.2/setup.py` & `cleanerpandasvol-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cleanerPandasVol',
-    version='0.1.2',
+    version='0.1.3',
     author='Murat Keskin & Ahmet Bagbakan & Cagla Ilhani',
     author_email='eng.murat.keskin@gmail.com',
     description='A comprehensive Python library for data preprocessing and cleaning',
     url='https://github.com/MuratKeskin0/Python_Data_Project_Vol',
     packages=find_packages(),
     install_requires=[
         'pandas',
-        'numpy'
+        'numpy',
         'scikit-learn',
         'nltk',
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

