# Comparing `tmp/geo_bound-0.1.tar.gz` & `tmp/geo_bound-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo_bound-0.1.tar", last modified: Tue May 21 23:51:22 2024, max compression
+gzip compressed data, was "geo_bound-0.1.1.tar", last modified: Tue May 21 23:44:33 2024, max compression
```

## Comparing `geo_bound-0.1.tar` & `geo_bound-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 23:51:22.342346 geo_bound-0.1/
--rw-rw-rw-   0        0        0    35018 2024-05-21 15:01:44.000000 geo_bound-0.1/COPYING.txt
--rw-rw-rw-   0        0        0    35803 2024-05-21 15:01:44.000000 geo_bound-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       83 2024-05-21 23:01:01.000000 geo_bound-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6455 2024-05-21 23:51:22.342346 geo_bound-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5549 2024-05-21 15:01:44.000000 geo_bound-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 23:51:22.311101 geo_bound-0.1/geo_bound/
--rw-rw-rw-   0        0        0     3217 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/Area.py
--rw-rw-rw-   0        0        0     2654 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/Line.py
--rw-rw-rw-   0        0        0    15313 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/Map.py
--rw-rw-rw-   0        0        0       62 2024-05-21 23:43:15.000000 geo_bound-0.1/geo_bound/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:51:22.326723 geo_bound-0.1/geo_bound/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/utils/__init__.py
--rw-rw-rw-   0        0        0     4700 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/utils/geometry.py
--rw-rw-rw-   0        0        0     4819 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/utils/io.py
--rw-rw-rw-   0        0        0     2461 2024-05-21 15:01:44.000000 geo_bound-0.1/geo_bound/utils/treat_data.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:51:22.342346 geo_bound-0.1/geo_bound.egg-info/
--rw-rw-rw-   0        0        0     6455 2024-05-21 23:51:22.000000 geo_bound-0.1/geo_bound.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2024-05-21 23:51:22.000000 geo_bound-0.1/geo_bound.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 23:51:22.000000 geo_bound-0.1/geo_bound.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 23:51:22.000000 geo_bound-0.1/geo_bound.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-21 22:30:26.000000 geo_bound-0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 23:51:22.342346 geo_bound-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1954 2024-05-21 23:49:34.000000 geo_bound-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:44:33.898137 geo_bound-0.1.1/
+-rw-rw-rw-   0        0        0    35018 2024-05-21 15:01:44.000000 geo_bound-0.1.1/COPYING.txt
+-rw-rw-rw-   0        0        0    35803 2024-05-21 15:01:44.000000 geo_bound-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       83 2024-05-21 23:01:01.000000 geo_bound-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6457 2024-05-21 23:44:33.728001 geo_bound-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5549 2024-05-21 15:01:44.000000 geo_bound-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:44:33.478930 geo_bound-0.1.1/geo_bound/
+-rw-rw-rw-   0        0        0     3217 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/Area.py
+-rw-rw-rw-   0        0        0     2654 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/Line.py
+-rw-rw-rw-   0        0        0    15313 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/Map.py
+-rw-rw-rw-   0        0        0       62 2024-05-21 23:43:15.000000 geo_bound-0.1.1/geo_bound/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:44:33.717005 geo_bound-0.1.1/geo_bound/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/utils/__init__.py
+-rw-rw-rw-   0        0        0     4700 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/utils/geometry.py
+-rw-rw-rw-   0        0        0     4819 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/utils/io.py
+-rw-rw-rw-   0        0        0     2461 2024-05-21 15:01:44.000000 geo_bound-0.1.1/geo_bound/utils/treat_data.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:44:33.728001 geo_bound-0.1.1/geo_bound.egg-info/
+-rw-rw-rw-   0        0        0     6457 2024-05-21 23:44:33.000000 geo_bound-0.1.1/geo_bound.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2024-05-21 23:44:33.000000 geo_bound-0.1.1/geo_bound.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:44:33.000000 geo_bound-0.1.1/geo_bound.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 23:44:33.000000 geo_bound-0.1.1/geo_bound.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-21 22:30:26.000000 geo_bound-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:44:33.898137 geo_bound-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1956 2024-05-21 23:43:28.000000 geo_bound-0.1.1/setup.py
```

### Comparing `geo_bound-0.1/COPYING.txt` & `geo_bound-0.1.1/COPYING.txt`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/LICENSE.txt` & `geo_bound-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/PKG-INFO` & `geo_bound-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo_bound
-Version: 0.1
+Version: 0.1.1
 Summary: Location of coordinates in geospatial maps.
 Home-page: https://github.com/TDPessoa/geolocation-with-coordinates
 Author: TDPessoa
 Author-email: thiago.d.pessoa@gmail.com
 License: GPL-3.0 license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `geo_bound-0.1/README.md` & `geo_bound-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/Area.py` & `geo_bound-0.1.1/geo_bound/Area.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/Line.py` & `geo_bound-0.1.1/geo_bound/Line.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/Map.py` & `geo_bound-0.1.1/geo_bound/Map.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/utils/geometry.py` & `geo_bound-0.1.1/geo_bound/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/utils/io.py` & `geo_bound-0.1.1/geo_bound/utils/io.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound/utils/treat_data.py` & `geo_bound-0.1.1/geo_bound/utils/treat_data.py`

 * *Files identical despite different names*

### Comparing `geo_bound-0.1/geo_bound.egg-info/PKG-INFO` & `geo_bound-0.1.1/geo_bound.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo_bound
-Version: 0.1
+Version: 0.1.1
 Summary: Location of coordinates in geospatial maps.
 Home-page: https://github.com/TDPessoa/geolocation-with-coordinates
 Author: TDPessoa
 Author-email: thiago.d.pessoa@gmail.com
 License: GPL-3.0 license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `geo_bound-0.1/setup.py` & `geo_bound-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from setuptools import (
     setup, 
     find_packages
 )
 
 setup(
     name='geo_bound',
-    version='0.1',
+    version='0.1.1',
     description='Location of coordinates in geospatial maps.',
     long_description=pathlib.Path('README.md').read_text(),
     long_description_content_type='text/markdown',
     url='https://github.com/TDPessoa/geolocation-with-coordinates',
     license='GPL-3.0 license',
     author='TDPessoa',
     author_email='thiago.d.pessoa@gmail.com',
```

