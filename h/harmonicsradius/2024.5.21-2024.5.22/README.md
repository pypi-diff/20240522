# Comparing `tmp/harmonicsradius-2024.5.21.tar.gz` & `tmp/harmonicsradius-2024.5.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonicsradius-2024.5.21.tar", last modified: Tue May 21 21:20:40 2024, max compression
+gzip compressed data, was "harmonicsradius-2024.5.22.tar", last modified: Wed May 22 19:22:56 2024, max compression
```

## Comparing `harmonicsradius-2024.5.21.tar` & `harmonicsradius-2024.5.22.tar`

### file list

```diff
@@ -1,27 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:20:40.424500 harmonicsradius-2024.5.21/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    43810 2024-05-21 21:20:40.424500 harmonicsradius-2024.5.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:20:40.420500 harmonicsradius-2024.5.21/harmonicsradius/
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/hri95.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/image.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:20:40.424500 harmonicsradius-2024.5.21/harmonicsradius/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/harmonics_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/interface_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/mean_squared_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/peak_signal_to_noise_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/metrics/structural_similarity_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/sr_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/harmonicsradius/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:20:40.424500 harmonicsradius-2024.5.21/harmonicsradius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43810 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 21:20:40.000000 harmonicsradius-2024.5.21/harmonicsradius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-21 21:20:36.000000 harmonicsradius-2024.5.21/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:20:40.424500 harmonicsradius-2024.5.21/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:22:56.002150 harmonicsradius-2024.5.22/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43828 2024-05-22 19:22:56.002150 harmonicsradius-2024.5.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:22:55.998150 harmonicsradius-2024.5.22/harmonicsradius/
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/hri95.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/image.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:22:55.998150 harmonicsradius-2024.5.22/harmonicsradius/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/harmonics_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/interface_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/peak_signal_to_noise_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/metrics/structural_similarity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/sr_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/harmonicsradius/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:22:56.002150 harmonicsradius-2024.5.22/harmonicsradius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43828 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 19:22:55.000000 harmonicsradius-2024.5.22/harmonicsradius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:22:56.002150 harmonicsradius-2024.5.22/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:22:56.002150 harmonicsradius-2024.5.22/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_metric_mean_squared_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_metrics_harmonics_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_metrics_interface_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_metrics_peak_signal_to_noise_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_metrics_structural_similarity_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_sr_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-22 19:22:51.000000 harmonicsradius-2024.5.22/tests/test_utils.py
```

### Comparing `harmonicsradius-2024.5.21/LICENSE` & `harmonicsradius-2024.5.22/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/PKG-INFO` & `harmonicsradius-2024.5.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmonicsradius
-Version: 2024.5.21
+Version: 2024.5.22
 Summary: Harmonics' Radius Index (HRI95) is a full-reference image quality index based harmonic structures of the images for the comparison super-resolution models.
 Author-email: Gökhan Koçmarlı <gokhan.kocmarli@gmail.com>
 Maintainer-email: Gökhan Koçmarlı <gokhan.kocmarli@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,23 +675,23 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/electricalgorithm/harmonics-radius-index
-Project-URL: Repository, https://github.com/electricalgorithm/harmonics-radius-index.git
-Project-URL: Issues, https://github.com/electricalgorithm/harmonics-radius-index/issues
+Project-URL: Homepage, https://github.com/electricalgorithm/universal-hri95
+Project-URL: Repository, https://github.com/electricalgorithm/universal-hri95.git
+Project-URL: Issues, https://github.com/electricalgorithm/universal-hri95/issues
 Keywords: super-resolution,frequency-analysis,image-quality-metrics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `harmonicsradius-2024.5.21/README.md` & `harmonicsradius-2024.5.22/README.md`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/hri95.py` & `harmonicsradius-2024.5.22/harmonicsradius/hri95.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/image.py` & `harmonicsradius-2024.5.22/harmonicsradius/image.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/metrics/harmonics_radius.py` & `harmonicsradius-2024.5.22/harmonicsradius/metrics/harmonics_radius.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/metrics/interface_metric.py` & `harmonicsradius-2024.5.22/harmonicsradius/metrics/interface_metric.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/metrics/mean_squared_error.py` & `harmonicsradius-2024.5.22/harmonicsradius/metrics/mean_squared_error.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/metrics/peak_signal_to_noise_ratio.py` & `harmonicsradius-2024.5.22/harmonicsradius/metrics/peak_signal_to_noise_ratio.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/metrics/structural_similarity_index.py` & `harmonicsradius-2024.5.22/harmonicsradius/metrics/structural_similarity_index.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/preprocessors.py` & `harmonicsradius-2024.5.22/harmonicsradius/preprocessors.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/sr_analyzer.py` & `harmonicsradius-2024.5.22/harmonicsradius/sr_analyzer.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius/utils.py` & `harmonicsradius-2024.5.22/harmonicsradius/utils.py`

 * *Files identical despite different names*

### Comparing `harmonicsradius-2024.5.21/harmonicsradius.egg-info/PKG-INFO` & `harmonicsradius-2024.5.22/harmonicsradius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harmonicsradius
-Version: 2024.5.21
+Version: 2024.5.22
 Summary: Harmonics' Radius Index (HRI95) is a full-reference image quality index based harmonic structures of the images for the comparison super-resolution models.
 Author-email: Gökhan Koçmarlı <gokhan.kocmarli@gmail.com>
 Maintainer-email: Gökhan Koçmarlı <gokhan.kocmarli@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -675,23 +675,23 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
-Project-URL: Homepage, https://github.com/electricalgorithm/harmonics-radius-index
-Project-URL: Repository, https://github.com/electricalgorithm/harmonics-radius-index.git
-Project-URL: Issues, https://github.com/electricalgorithm/harmonics-radius-index/issues
+Project-URL: Homepage, https://github.com/electricalgorithm/universal-hri95
+Project-URL: Repository, https://github.com/electricalgorithm/universal-hri95.git
+Project-URL: Issues, https://github.com/electricalgorithm/universal-hri95/issues
 Keywords: super-resolution,frequency-analysis,image-quality-metrics
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Other Audience
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: opencv-python
```

### Comparing `harmonicsradius-2024.5.21/pyproject.toml` & `harmonicsradius-2024.5.22/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "harmonicsradius"
 description = "Harmonics' Radius Index (HRI95) is a full-reference image quality index based harmonic structures of the images for the comparison super-resolution models."
 keywords = ["super-resolution", "frequency-analysis", "image-quality-metrics"]
-version = "2024.5.21"
+version = "2024.5.22"
 readme = { file = "README.md", content-type = "text/markdown" }
 license = { file = "LICENSE" }
 
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Other Audience",
     "Topic :: Scientific/Engineering :: Image Processing",
-    "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = ["numpy", "opencv-python", "scikit-image"]
 
 
@@ -32,17 +32,17 @@
 [tool.setuptools.packages.find]
 include = ["harmonicsradius*"]
 
 [project.scripts]
 hri95 = "harmonicsradius.hri95:main"
 
 [project.urls]
-Homepage = "https://github.com/electricalgorithm/harmonics-radius-index"
-Repository = "https://github.com/electricalgorithm/harmonics-radius-index.git"
-Issues = "https://github.com/electricalgorithm/harmonics-radius-index/issues"
+Homepage = "https://github.com/electricalgorithm/universal-hri95"
+Repository = "https://github.com/electricalgorithm/universal-hri95.git"
+Issues = "https://github.com/electricalgorithm/universal-hri95/issues"
 
 
 [tool.flake8]
 exclude = [".git", "__pycache__", "*venv", "build", "dist", "venv*", "examples"]
 max-line-length = 100
 count = true
```

