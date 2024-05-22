# Comparing `tmp/hoffmanstmpy-1.0.1.tar.gz` & `tmp/hoffmanstmpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hoffmanstmpy-1.0.1.tar", last modified: Mon Jun 12 20:08:27 2023, max compression
+gzip compressed data, was "hoffmanstmpy-1.0.2.tar", last modified: Wed May 22 00:49:38 2024, max compression
```

## Comparing `hoffmanstmpy-1.0.1.tar` & `hoffmanstmpy-1.0.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.063629 hoffmanstmpy-1.0.1/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1065 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/LICENSE.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       71 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/MANIFEST.in
--rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-06-12 20:08:27.063908 hoffmanstmpy-1.0.1/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1283 2023-05-25 15:46:08.000000 hoffmanstmpy-1.0.1/README.md
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.027938 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/
--rw-r--r--   0 richardyuliu   (501) staff       (20)      621 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/PKG-INFO
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1139 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/SOURCES.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/dependency_links.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       50 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/requires.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2023-06-12 20:08:26.000000 hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/top_level.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)       79 2023-06-12 20:08:27.064796 hoffmanstmpy-1.0.1/setup.cfg
--rw-r--r--   0 richardyuliu   (501) staff       (20)      922 2023-06-12 20:07:31.000000 hoffmanstmpy-1.0.1/setup.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.034884 hoffmanstmpy-1.0.1/stmpy/
--rw-r--r--   0 richardyuliu   (501) staff       (20)      670 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/__init__.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.037292 hoffmanstmpy-1.0.1/stmpy/color/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     7611 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/colormap.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.053202 hoffmanstmpy-1.0.1/stmpy/color/maps/
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8055 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/ALS-og.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)    19200 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/ALS.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1944 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Autumn.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2251 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue1.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2045 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1955 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Blue3.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1905 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect0.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1733 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect1.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1494 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1734 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Defect4.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1073 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Gray.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1536 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/GrayInverse.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)    25600 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/PuGn.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)    25585 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/Red_Blue.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1511 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/SailingMod2.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)      694 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/YH.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2996 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/maps/mhblue.mat
--rw-r--r--   0 richardyuliu   (501) staff       (20)     2410 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/color/palette.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1544 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.1/stmpy/cv.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    83396 2023-05-25 19:46:50.000000 hoffmanstmpy-1.0.1/stmpy/driftcorr.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.056792 hoffmanstmpy-1.0.1/stmpy/hp/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8939 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/kondo_holes.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    20378 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/hp/tight_binding.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    19176 2023-05-25 20:07:07.000000 hoffmanstmpy-1.0.1/stmpy/image.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    39913 2023-05-18 21:06:25.000000 hoffmanstmpy-1.0.1/stmpy/io.py
-drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2023-06-12 20:08:27.062853 hoffmanstmpy-1.0.1/stmpy/mapviewer/
--rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/__init__.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    32564 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/gui_components.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)      886 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/helptext.txt
--rw-r--r--   0 richardyuliu   (501) staff       (20)     3393 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/misc.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     8131 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/mapviewer/view3ds.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     7015 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/matio.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)     1226 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/read_STMView.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)    26985 2023-05-04 01:55:03.000000 hoffmanstmpy-1.0.1/stmpy/read_all.py
--rw-r--r--   0 richardyuliu   (501) staff       (20)   104850 2023-05-25 19:30:41.000000 hoffmanstmpy-1.0.1/stmpy/tools.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.058063 hoffmanstmpy-1.0.2/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1073 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.2/LICENSE
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1065 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.2/LICENSE.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       71 2023-05-04 01:55:02.000000 hoffmanstmpy-1.0.2/MANIFEST.in
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      755 2024-05-22 00:49:38.057729 hoffmanstmpy-1.0.2/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1283 2023-05-25 15:46:08.000000 hoffmanstmpy-1.0.2/README.md
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.056254 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      755 2024-05-22 00:49:37.000000 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/PKG-INFO
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1147 2024-05-22 00:49:37.000000 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/SOURCES.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2024-05-22 00:49:37.000000 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/dependency_links.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       50 2024-05-22 00:49:37.000000 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/requires.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        6 2024-05-22 00:49:37.000000 hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/top_level.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)       79 2024-05-22 00:49:38.059070 hoffmanstmpy-1.0.2/setup.cfg
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      922 2024-05-22 00:36:54.000000 hoffmanstmpy-1.0.2/setup.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.021219 hoffmanstmpy-1.0.2/stmpy/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      670 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/__init__.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.026064 hoffmanstmpy-1.0.2/stmpy/color/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     7611 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/colormap.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.045007 hoffmanstmpy-1.0.2/stmpy/color/maps/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8055 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/ALS-og.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    19200 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/ALS.txt
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1944 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Autumn.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     2251 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Blue1.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     2045 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Blue2.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1955 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Blue3.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1905 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Defect0.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1733 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Defect1.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1494 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Defect2.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1734 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Defect4.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1073 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Gray.mat
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1536 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/GrayInverse.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    25600 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/PuGn.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    25585 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/Red_Blue.txt
+-rwxr-xr-x   0 richardyuliu   (501) staff       (20)     1511 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/SailingMod2.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      694 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/YH.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2996 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/maps/mhblue.mat
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     2410 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/color/palette.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1544 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/cv.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    83370 2023-08-02 21:31:17.000000 hoffmanstmpy-1.0.2/stmpy/driftcorr.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.048581 hoffmanstmpy-1.0.2/stmpy/hp/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/hp/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8939 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/hp/kondo_holes.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    20378 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/hp/tight_binding.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    19330 2024-05-22 00:38:58.000000 hoffmanstmpy-1.0.2/stmpy/image.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    39756 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/io.py
+drwxr-xr-x   0 richardyuliu   (501) staff       (20)        0 2024-05-22 00:49:38.055030 hoffmanstmpy-1.0.2/stmpy/mapviewer/
+-rw-r--r--   0 richardyuliu   (501) staff       (20)        1 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/mapviewer/__init__.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    32564 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/mapviewer/gui_components.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)      886 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/mapviewer/helptext.txt
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     3393 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/mapviewer/misc.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     8131 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/mapviewer/view3ds.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     7015 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/matio.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)     1226 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/read_STMView.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)    26985 2023-10-03 08:40:56.000000 hoffmanstmpy-1.0.2/stmpy/read_all.py
+-rw-r--r--   0 richardyuliu   (501) staff       (20)   104850 2023-05-25 19:30:41.000000 hoffmanstmpy-1.0.2/stmpy/tools.py
```

### Comparing `hoffmanstmpy-1.0.1/LICENSE.txt` & `hoffmanstmpy-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/PKG-INFO` & `hoffmanstmpy-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: hoffmanstmpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scanning tunneling microscopy data analysis suite
 Home-page: https://github.com/hoffmanlabcoding/stmpy
+Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
 Author: Harris Pirie
 Author-email: hoffmanlabcoding@gmail.com
 License: MIT
-Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
-Description: UNKNOWN
 Keywords: STM,Python,Data Analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: opencv-python
+Requires-Dist: scikit-image
```

### Comparing `hoffmanstmpy-1.0.1/README.md` & `hoffmanstmpy-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/PKG-INFO` & `hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: hoffmanstmpy
-Version: 1.0.1
+Version: 1.0.2
 Summary: Scanning tunneling microscopy data analysis suite
 Home-page: https://github.com/hoffmanlabcoding/stmpy
+Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
 Author: Harris Pirie
 Author-email: hoffmanlabcoding@gmail.com
 License: MIT
-Download-URL: https://github.com/hoffmanlabcoding/stmpy.git
-Description: UNKNOWN
 Keywords: STM,Python,Data Analysis
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: matplotlib
+Requires-Dist: opencv-python
+Requires-Dist: scikit-image
```

### Comparing `hoffmanstmpy-1.0.1/hoffmanstmpy.egg-info/SOURCES.txt` & `hoffmanstmpy-1.0.2/hoffmanstmpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 hoffmanstmpy.egg-info/PKG-INFO
 hoffmanstmpy.egg-info/SOURCES.txt
```

### Comparing `hoffmanstmpy-1.0.1/setup.py` & `hoffmanstmpy-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'hoffmanstmpy',
-  version = '1.0.1',
+  version = '1.0.2',
   packages = find_packages(),
   package_data = {
     "":["*.txt", "*.mat"]
     },
   include_package_data=True,
   license='MIT',
   description = 'Scanning tunneling microscopy data analysis suite',
```

### Comparing `hoffmanstmpy-1.0.1/stmpy/__init__.py` & `hoffmanstmpy-1.0.2/stmpy/__init__.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/colormap.py` & `hoffmanstmpy-1.0.2/stmpy/color/colormap.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/ALS-og.txt` & `hoffmanstmpy-1.0.2/stmpy/color/maps/ALS-og.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/ALS.txt` & `hoffmanstmpy-1.0.2/stmpy/color/maps/ALS.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Autumn.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Autumn.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue1.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Blue1.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue2.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Blue2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Blue3.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Blue3.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect0.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Defect0.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect1.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Defect1.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect2.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Defect2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Defect4.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Defect4.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Gray.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Gray.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/GrayInverse.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/GrayInverse.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/PuGn.txt` & `hoffmanstmpy-1.0.2/stmpy/color/maps/PuGn.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/Red_Blue.txt` & `hoffmanstmpy-1.0.2/stmpy/color/maps/Red_Blue.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/SailingMod2.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/SailingMod2.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/YH.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/YH.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/maps/mhblue.mat` & `hoffmanstmpy-1.0.2/stmpy/color/maps/mhblue.mat`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/color/palette.py` & `hoffmanstmpy-1.0.2/stmpy/color/palette.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/cv.py` & `hoffmanstmpy-1.0.2/stmpy/cv.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/driftcorr.py` & `hoffmanstmpy-1.0.2/stmpy/driftcorr.py`

 * *Files 0% similar despite different names*

```diff
@@ -2010,18 +2010,18 @@
         extents = [-qscale, qscale, -qscale, qscale, ]
         
     # Use the default color maps if cmap is not set
     if cmap == None:
         cmap = stmpy.cm.blue2 if rspace else stmpy.cm.gray_r
         
     if rspace == True:
-        plt.imshow(A, clim=[c-thres*s, c+thres*s], cmap=cmap, **kwargs)
+        plt.imshow(A, clim=clims, cmap=cmap, **kwargs)
         plt.gca().set_aspect(1)
     else:
-        plt.imshow(A, extent=extents, clim=[0, c+thres*s], cmap=cmap, **kwargs)
+        plt.imshow(A, extent=extents, clim=clims, cmap=cmap, **kwargs)
     plt.gca().axes.get_xaxis().set_visible(False)
     plt.gca().axes.get_yaxis().set_visible(False)
     plt.gca().set_frame_on(False)
     
     if imgName != None:
         if extension == 'png':
             plt.savefig("{}.{}".format(imgName, extension), dpi=dpi, bbox_inches='tight', pad_inches=0)
```

### Comparing `hoffmanstmpy-1.0.1/stmpy/hp/kondo_holes.py` & `hoffmanstmpy-1.0.2/stmpy/hp/kondo_holes.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/hp/tight_binding.py` & `hoffmanstmpy-1.0.2/stmpy/hp/tight_binding.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/image.py` & `hoffmanstmpy-1.0.2/stmpy/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     y_high = np.absolute(level_high - pdf)
     c_low = y[np.argmin(y_low)]
     c_high = y[np.argmin(y_high)]
     for image in images:
         image.set_clim(c_low, c_high)
 
 
-def write_animation(data, fileName, saturation=2, clims=(0,1), cmap=None,
+def write_animation(data, fileName, saturation=2, clims=(0,1), cmap=None, scale=None,
                     label=None, label_caption='meV', speed=8, zoom=1, **kwargs):
     ''' Create a movie from a 3D data set and save it to the path specified. Intended
     for visualising DOS maps and QPI data. Iterates through the first index in
     the data set to create an animation.
 
     Notes:
         Make sure you include file extension (eg '.mov') in the file path.
@@ -130,14 +130,16 @@
         else:
             if len(np.shape(clims)) > 1:
                 plt.clim(clims[i])
             else:
                 plt.clim(clims)
         if label is not None:
             tx.set_text('{:2.1f} {:}'.format(label[i], label_caption))
+        if scale is not None:
+            add_scale_bar(length=scale['length'], imgsize=scale['imgsize'], imgpixels=scale['imgpixels'],ax=im)
         return [im]
     fig.tight_layout()
     ani = FuncAnimation(fig, animate, init_func=init, frames=data.shape[0])
     if fileName.endswith('.mov'):
         ani.save(fileName, codec='prores', dpi=200, fps=speed)
     elif fileName.endswith('.mp4'):
         ani.save(fileName, dpi=200, bitrate=1e5, fps=speed)
```

### Comparing `hoffmanstmpy-1.0.1/stmpy/io.py` & `hoffmanstmpy-1.0.2/stmpy/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,14 @@
         2018-11-07  - HP : Add byte support to SPY files.
         2018-11-13  - HP : Add nice_units to .dat files
         2019-01-09  - BB : Generalize file extension extraction
         2019-02-28  - HP : Loads multisweep .dat files even if missing header.
         2020-07-12  - WT : Added support for sm4 file from rhk system.
         2022-06-22  - HP : Added support for Cornell files: .2FL .1FL .TFR .1FR
         2022-02-15  - HP : Added support for STM1 Cornell .FFL files
-        2023-05-18  - RL : Loads sxm scan files even if missing header.
 
     '''
     try:
         filename, extension = os.path.splitext(filePath)
         extension = extension.replace(".","")
     except IndexError:
         raise IOError('Please include file extension in path.')
@@ -632,18 +631,15 @@
             tagname = line[1:-1]
         else:
             if 'Z-CONTROLLER' == tagname:
                 keys = line.split('\t')
                 values = fileObj.readline().strip().decode('utf-8').split('\t')
                 self.header['z-controller'] = dict(zip(keys, values))
             elif tagname in ('BIAS', 'REC_TEMP', 'ACQ_TIME', 'SCAN_ANGLE'):
-                try:
-                    self.header[tagname.lower()] = float(line)
-                except ValueError:
-                    pass
+                self.header[tagname.lower()] = float(line)
             elif tagname in ('SCAN_PIXELS', 'SCAN_TIME', 'SCAN_RANGE', 'SCAN_OFFSET'):
                 self.header[tagname.lower()] = [ float(i) for i in re.split('\s+', line) ]
             elif 'DATA_INFO' == tagname:
                 if 1 == self.header['version']:
                     keys = re.split('\s\s+',line)
                 else:
                     keys = line.split('\t')
```

### Comparing `hoffmanstmpy-1.0.1/stmpy/mapviewer/gui_components.py` & `hoffmanstmpy-1.0.2/stmpy/mapviewer/gui_components.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/mapviewer/helptext.txt` & `hoffmanstmpy-1.0.2/stmpy/mapviewer/helptext.txt`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/mapviewer/misc.py` & `hoffmanstmpy-1.0.2/stmpy/mapviewer/misc.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/mapviewer/view3ds.py` & `hoffmanstmpy-1.0.2/stmpy/mapviewer/view3ds.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/matio.py` & `hoffmanstmpy-1.0.2/stmpy/matio.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/read_STMView.py` & `hoffmanstmpy-1.0.2/stmpy/read_STMView.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/read_all.py` & `hoffmanstmpy-1.0.2/stmpy/read_all.py`

 * *Files identical despite different names*

### Comparing `hoffmanstmpy-1.0.1/stmpy/tools.py` & `hoffmanstmpy-1.0.2/stmpy/tools.py`

 * *Files identical despite different names*

