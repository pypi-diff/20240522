# Comparing `tmp/teklia-line-image-extractor-0.2.9.tar.gz` & `tmp/teklia_line_image_extractor-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teklia-line-image-extractor-0.2.9.tar", last modified: Wed Mar 13 16:03:07 2024, max compression
+gzip compressed data, was "teklia_line_image_extractor-0.3.0.tar", last modified: Wed May 22 10:59:37 2024, max compression
```

## Comparing `teklia-line-image-extractor-0.2.9.tar` & `teklia_line_image_extractor-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:03:07.080017 teklia-line-image-extractor-0.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2387 2024-03-13 16:03:07.080017 teklia-line-image-extractor-0.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1500 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-13 16:02:57.000000 teklia-line-image-extractor-0.2.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:03:07.076017 teklia-line-image-extractor-0.2.9/line_image_extractor/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/line_image_extractor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4810 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/line_image_extractor/extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     7197 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/line_image_extractor/image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2796 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/line_image_extractor/main.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 16:03:07.080017 teklia-line-image-extractor-0.2.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1448 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:03:07.080017 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      572 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 16:03:07.000000 teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 16:03:07.076017 teklia-line-image-extractor-0.2.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6248 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/tests/test_extractor.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/tests/test_image_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-13 16:01:40.000000 teklia-line-image-extractor-0.2.9/tests/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 10:59:37.180854 teklia_line_image_extractor-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-22 10:59:37.180854 teklia_line_image_extractor-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1500 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-05-22 10:57:46.000000 teklia_line_image_extractor-0.3.0/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 10:59:37.176854 teklia_line_image_extractor-0.3.0/line_image_extractor/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/line_image_extractor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4810 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/line_image_extractor/extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     7197 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/line_image_extractor/image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2796 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/line_image_extractor/main.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 10:59:37.180854 teklia_line_image_extractor-0.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1448 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 10:59:37.180854 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      572 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       72 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 10:59:37.000000 teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 10:59:37.180854 teklia_line_image_extractor-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6248 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/tests/test_extractor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/tests/test_image_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2024-05-22 10:56:28.000000 teklia_line_image_extractor-0.3.0/tests/test_main.py
```

### Comparing `teklia-line-image-extractor-0.2.9/LICENSE` & `teklia_line_image_extractor-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/PKG-INFO` & `teklia_line_image_extractor-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.9
+Version: 0.3.0
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.teklia.com/atr/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python-headless==4.8.1.78
-Requires-Dist: Pillow==10.2.0
+Requires-Dist: Pillow==10.3.0
 
 # Line image extractor
 
 This is a tool and a library to be used for extracting line images. Built by [Teklia](https://teklia.com) and freely available as open-source under the MIT licence.
 
 It supports different extraction methods:
 * boundingRect - bounding rectangle of the line polygon
```

### Comparing `teklia-line-image-extractor-0.2.9/README.md` & `teklia_line_image_extractor-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/line_image_extractor/extractor.py` & `teklia_line_image_extractor-0.3.0/line_image_extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/line_image_extractor/image_utils.py` & `teklia_line_image_extractor-0.3.0/line_image_extractor/image_utils.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/line_image_extractor/main.py` & `teklia_line_image_extractor-0.3.0/line_image_extractor/main.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/setup.py` & `teklia_line_image_extractor-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/PKG-INFO` & `teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teklia-line-image-extractor
-Version: 0.2.9
+Version: 0.3.0
 Summary: A tool for extracting a text line image from the contour with different methods
 Home-page: https://gitlab.teklia.com/atr/line_image_extractor
 Author: Martin Maarand
 Author-email: maarand@teklia.com
 Keywords: line transformation image extraction
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: opencv-python-headless==4.8.1.78
-Requires-Dist: Pillow==10.2.0
+Requires-Dist: Pillow==10.3.0
 
 # Line image extractor
 
 This is a tool and a library to be used for extracting line images. Built by [Teklia](https://teklia.com) and freely available as open-source under the MIT licence.
 
 It supports different extraction methods:
 * boundingRect - bounding rectangle of the line polygon
```

### Comparing `teklia-line-image-extractor-0.2.9/teklia_line_image_extractor.egg-info/SOURCES.txt` & `teklia_line_image_extractor-0.3.0/teklia_line_image_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/tests/test_extractor.py` & `teklia_line_image_extractor-0.3.0/tests/test_extractor.py`

 * *Files identical despite different names*

### Comparing `teklia-line-image-extractor-0.2.9/tests/test_image_utils.py` & `teklia_line_image_extractor-0.3.0/tests/test_image_utils.py`

 * *Files identical despite different names*

