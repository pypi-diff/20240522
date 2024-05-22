# Comparing `tmp/GeoEntropy-0.1.1.tar.gz` & `tmp/GeoEntropy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GeoEntropy-0.1.1.tar", last modified: Thu May 16 18:02:18 2024, max compression
+gzip compressed data, was "GeoEntropy-0.2.0.tar", last modified: Wed May 22 11:55:08 2024, max compression
```

## Comparing `GeoEntropy-0.1.1.tar` & `GeoEntropy-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-16 18:02:18.426191 GeoEntropy-0.1.1/
-drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-16 18:02:18.420910 GeoEntropy-0.1.1/GeoEntropy.egg-info/
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)    10991 2024-05-16 18:02:18.000000 GeoEntropy-0.1.1/GeoEntropy.egg-info/PKG-INFO
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      608 2024-05-16 18:02:18.000000 GeoEntropy-0.1.1/GeoEntropy.egg-info/SOURCES.txt
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)        1 2024-05-16 18:02:18.000000 GeoEntropy-0.1.1/GeoEntropy.egg-info/dependency_links.txt
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)       38 2024-05-16 18:02:18.000000 GeoEntropy-0.1.1/GeoEntropy.egg-info/requires.txt
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)       11 2024-05-16 18:02:18.000000 GeoEntropy-0.1.1/GeoEntropy.egg-info/top_level.txt
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     1085 2024-05-15 18:11:12.000000 GeoEntropy-0.1.1/LICENSE
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)    10991 2024-05-16 18:02:18.425825 GeoEntropy-0.1.1/PKG-INFO
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)    10382 2024-05-16 17:32:17.000000 GeoEntropy-0.1.1/README.md
-drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-16 18:02:18.423083 GeoEntropy-0.1.1/geoentropy/
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      550 2024-05-16 17:56:33.000000 GeoEntropy-0.1.1/geoentropy/__init__.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3367 2024-05-15 18:01:37.000000 GeoEntropy-0.1.1/geoentropy/batty.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3645 2024-05-16 17:32:17.000000 GeoEntropy-0.1.1/geoentropy/csv_to_matrix.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     4217 2024-05-15 17:53:00.000000 GeoEntropy-0.1.1/geoentropy/karlstrom.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3718 2024-05-15 17:43:47.000000 GeoEntropy-0.1.1/geoentropy/leibovici.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     2817 2024-05-16 17:32:17.000000 GeoEntropy-0.1.1/geoentropy/oneill.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     2149 2024-05-15 17:36:51.000000 GeoEntropy-0.1.1/geoentropy/shannon.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3021 2024-05-15 17:35:40.000000 GeoEntropy-0.1.1/geoentropy/shannon_z.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)     4276 2024-05-16 13:50:41.000000 GeoEntropy-0.1.1/geoentropy/spatial_partition.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)       38 2024-05-16 18:02:18.426233 GeoEntropy-0.1.1/setup.cfg
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      767 2024-05-16 17:56:33.000000 GeoEntropy-0.1.1/setup.py
-drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-16 18:02:18.425467 GeoEntropy-0.1.1/tests/
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      655 2024-05-16 17:24:12.000000 GeoEntropy-0.1.1/tests/test_batty.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      262 2024-05-16 17:32:17.000000 GeoEntropy-0.1.1/tests/test_csv_to_matrix.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      498 2024-05-16 17:24:52.000000 GeoEntropy-0.1.1/tests/test_karlstrom.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      507 2024-05-16 17:25:37.000000 GeoEntropy-0.1.1/tests/test_leibovici.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      456 2024-05-16 17:32:17.000000 GeoEntropy-0.1.1/tests/test_oneill.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      474 2024-05-16 17:26:51.000000 GeoEntropy-0.1.1/tests/test_shannon.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      470 2024-05-16 17:27:56.000000 GeoEntropy-0.1.1/tests/test_shannon_z.py
--rw-r--r--   0 maximiliankryschi   (501) staff       (20)      399 2024-05-16 17:24:12.000000 GeoEntropy-0.1.1/tests/test_spatial_partition.py
+drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-22 11:55:08.506327 GeoEntropy-0.2.0/
+drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-22 11:55:08.500213 GeoEntropy-0.2.0/GeoEntropy.egg-info/
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)    17858 2024-05-22 11:55:08.000000 GeoEntropy-0.2.0/GeoEntropy.egg-info/PKG-INFO
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      608 2024-05-22 11:55:08.000000 GeoEntropy-0.2.0/GeoEntropy.egg-info/SOURCES.txt
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)        1 2024-05-22 11:55:08.000000 GeoEntropy-0.2.0/GeoEntropy.egg-info/dependency_links.txt
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)       38 2024-05-22 11:55:08.000000 GeoEntropy-0.2.0/GeoEntropy.egg-info/requires.txt
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)       11 2024-05-22 11:55:08.000000 GeoEntropy-0.2.0/GeoEntropy.egg-info/top_level.txt
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     1085 2024-05-15 18:11:12.000000 GeoEntropy-0.2.0/LICENSE
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)    17858 2024-05-22 11:55:08.505704 GeoEntropy-0.2.0/PKG-INFO
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)    17249 2024-05-22 11:52:39.000000 GeoEntropy-0.2.0/README.md
+drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-22 11:55:08.502614 GeoEntropy-0.2.0/geoentropy/
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      550 2024-05-22 11:54:22.000000 GeoEntropy-0.2.0/geoentropy/__init__.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3388 2024-05-22 11:45:54.000000 GeoEntropy-0.2.0/geoentropy/batty.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     6954 2024-05-22 11:23:18.000000 GeoEntropy-0.2.0/geoentropy/csv_to_matrix.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     4217 2024-05-15 17:53:00.000000 GeoEntropy-0.2.0/geoentropy/karlstrom.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3718 2024-05-15 17:43:47.000000 GeoEntropy-0.2.0/geoentropy/leibovici.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     2817 2024-05-16 17:32:17.000000 GeoEntropy-0.2.0/geoentropy/oneill.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     2149 2024-05-15 17:36:51.000000 GeoEntropy-0.2.0/geoentropy/shannon.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     3021 2024-05-15 17:35:40.000000 GeoEntropy-0.2.0/geoentropy/shannon_z.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)     4276 2024-05-16 13:50:41.000000 GeoEntropy-0.2.0/geoentropy/spatial_partition.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)       38 2024-05-22 11:55:08.506388 GeoEntropy-0.2.0/setup.cfg
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      767 2024-05-22 11:53:55.000000 GeoEntropy-0.2.0/setup.py
+drwxr-xr-x   0 maximiliankryschi   (501) staff       (20)        0 2024-05-22 11:55:08.505250 GeoEntropy-0.2.0/tests/
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      655 2024-05-16 17:24:12.000000 GeoEntropy-0.2.0/tests/test_batty.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      414 2024-05-22 11:13:38.000000 GeoEntropy-0.2.0/tests/test_csv_to_matrix.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      498 2024-05-16 17:24:52.000000 GeoEntropy-0.2.0/tests/test_karlstrom.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      507 2024-05-16 17:25:37.000000 GeoEntropy-0.2.0/tests/test_leibovici.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      456 2024-05-16 17:32:17.000000 GeoEntropy-0.2.0/tests/test_oneill.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      474 2024-05-16 17:26:51.000000 GeoEntropy-0.2.0/tests/test_shannon.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      470 2024-05-16 17:27:56.000000 GeoEntropy-0.2.0/tests/test_shannon_z.py
+-rw-r--r--   0 maximiliankryschi   (501) staff       (20)      399 2024-05-16 17:24:12.000000 GeoEntropy-0.2.0/tests/test_spatial_partition.py
```

### Comparing `GeoEntropy-0.1.1/GeoEntropy.egg-info/SOURCES.txt` & `GeoEntropy-0.2.0/GeoEntropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/LICENSE` & `GeoEntropy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/__init__.py` & `GeoEntropy-0.2.0/geoentropy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 from .leibovici import leibovici
 from .oneill import oneill
 from .shannon import shannon
 from .shannon_z import shannon_z
 from .spatial_partition import spatial_partition
 
 print(
-    "GeoEntropy is in a very early version (0.1.1), no guarantee for correctness. Source code is available at https://github.com/maxkryschi/geoentropy")
+    "GeoEntropy is in a very early version (0.2.0), no guarantee for correctness. Source code is available at https://github.com/maxkryschi/geoentropy")
 
 __all__ = ['batty', 'csv_to_matrix', 'karlstrom', 'leibovici', 'oneill', 'shannon', 'shannon_z', 'spatial_partition']
```

### Comparing `GeoEntropy-0.1.1/geoentropy/batty.py` & `GeoEntropy-0.2.0/geoentropy/batty.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,16 @@
             batty_terms_rescaled = np.where(area_data['rel_freq'] > 0,
                                             area_data['rel_freq'] * np.log(resc_Tg / area_data['rel_freq']), 0)
             batty_entropy = np.sum(batty_terms_rescaled) - np.log(cc)
             print(
                 "Some sub-areas have size < 1, so they have been internally rescaled to avoid computational issues. The entropy in the output refers to the original area scale.")
     else:
         batty_entropy = np.sum(
-            np.where(area_data['rel_freq'] > 0, area_data['rel_freq'] * np.log(sub_area_sizes / area_data['rel_freq']), 0))
+            np.where(area_data['rel_freq'] > 0, area_data['rel_freq'] * np.log(sub_area_sizes / area_data['rel_freq']),
+                     0))
     return batty_entropy
 
 
 def _calculate_batty_entropy_range(sub_area_sizes):
     return [max(0, np.log(min(sub_area_sizes))), np.log(sum(sub_area_sizes))]
```

### Comparing `GeoEntropy-0.1.1/geoentropy/karlstrom.py` & `GeoEntropy-0.2.0/geoentropy/karlstrom.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/leibovici.py` & `GeoEntropy-0.2.0/geoentropy/leibovici.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/oneill.py` & `GeoEntropy-0.2.0/geoentropy/oneill.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/shannon.py` & `GeoEntropy-0.2.0/geoentropy/shannon.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/shannon_z.py` & `GeoEntropy-0.2.0/geoentropy/shannon_z.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/geoentropy/spatial_partition.py` & `GeoEntropy-0.2.0/geoentropy/spatial_partition.py`

 * *Files identical despite different names*

### Comparing `GeoEntropy-0.1.1/setup.py` & `GeoEntropy-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='GeoEntropy',
-    version='0.1.1',
+    version='0.2.0',
     packages=find_packages(),
     install_requires=['numpy', 'pandas', 'matplotlib', 'scipy', 'shapely'],
     include_package_data=True,
     description='A Python package for computing geometric/spatial entropy metrics for data in matrix format.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/maxkryschi/geoentropy',
```

### Comparing `GeoEntropy-0.1.1/tests/test_batty.py` & `GeoEntropy-0.2.0/tests/test_batty.py`

 * *Files identical despite different names*

