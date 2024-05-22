# Comparing `tmp/w2rpy-0.1.8.tar.gz` & `tmp/w2rpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.8.tar", last modified: Mon May  6 19:49:40 2024, max compression
+gzip compressed data, was "w2rpy-0.1.9.tar", last modified: Mon May  6 19:57:17 2024, max compression
```

## Comparing `w2rpy-0.1.8.tar` & `w2rpy-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 19:49:40.610445 w2rpy-0.1.8/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      379 2024-05-06 19:49:40.610445 w2rpy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.8/README.md
--rw-rw-rw-   0        0        0       86 2024-05-06 19:49:40.611451 w2rpy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      640 2024-05-06 19:49:12.000000 w2rpy-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-06 19:49:40.609444 w2rpy-0.1.8/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      379 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 19:49:40.000000 w2rpy-0.1.8/w2rpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    28231 2024-05-06 19:48:33.000000 w2rpy-0.1.8/w2rpy.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:57:17.741409 w2rpy-0.1.9/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:57:17.741409 w2rpy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.9/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-06 19:57:17.742418 w2rpy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      640 2024-05-06 19:51:56.000000 w2rpy-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 19:57:17.740409 w2rpy-0.1.9/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      379 2024-05-06 19:57:17.000000 w2rpy-0.1.9/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2024-05-06 19:57:17.000000 w2rpy-0.1.9/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 19:57:17.000000 w2rpy-0.1.9/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 19:57:17.000000 w2rpy-0.1.9/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-06 19:57:17.000000 w2rpy-0.1.9/w2rpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    28295 2024-05-06 19:51:45.000000 w2rpy-0.1.9/w2rpy.py
```

### Comparing `w2rpy-0.1.8/LICENSE` & `w2rpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.8/setup.py` & `w2rpy-0.1.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from distutils.core import setup
 
 setup(
   name = 'w2rpy',    
   py_modules=['w2rpy'],
-  version = '0.1.8',     
+  version = '0.1.9',     
   license='MIT',        
   description = 'Water Resource Functions For Fluvial Systems',   
   author = 'Luke Russell',                   
   author_email = 'lrussell@wolfwaterresources.com',      
   install_requires=['pandas',
                     'numpy',
                     'shapely',
```

### Comparing `w2rpy-0.1.8/w2rpy.py` & `w2rpy-0.1.9/w2rpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,16 @@
     pour_point = lines.loc[lines.downstream.isnull(),'FID'].values[0]
     lines.loc[lines.FID==pour_point,'dist_to_pour_point'] = 0
     lines = get_dist_to_pour_point(pour_point,lines)
     
     lines.crs = terrain.crs
     
     if save:
+        del lines['upstream']
+        del lines['downstream']
         lines.to_file(save)
         print('Stream network extracted')
     else:
         print('Stream network extracted')
         return lines
     
 def catchment(terrain, pour_point, snap_threshold=None,save=None):
```

