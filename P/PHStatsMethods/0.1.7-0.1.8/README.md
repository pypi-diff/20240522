# Comparing `tmp/phstatsmethods-0.1.7.tar.gz` & `tmp/phstatsmethods-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phstatsmethods-0.1.7.tar", last modified: Fri May 17 19:26:16 2024, max compression
+gzip compressed data, was "phstatsmethods-0.1.8.tar", last modified: Wed May 22 10:16:49 2024, max compression
```

## Comparing `phstatsmethods-0.1.7.tar` & `phstatsmethods-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:26:16.554658 phstatsmethods-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:26:16.554658 phstatsmethods-0.1.7/PHStatsMethods/
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/DSR.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/ISRate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/ISRatio.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/confidence_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/funnels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/means.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/proportions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/quantiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/utils_funnel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/PHStatsMethods/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 19:26:16.554658 phstatsmethods-0.1.7/PHStatsMethods.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:26:16.000000 phstatsmethods-0.1.7/PHStatsMethods.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-17 19:26:16.000000 phstatsmethods-0.1.7/PHStatsMethods.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 19:26:16.000000 phstatsmethods-0.1.7/PHStatsMethods.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-17 19:26:16.000000 phstatsmethods-0.1.7/PHStatsMethods.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-17 19:26:16.000000 phstatsmethods-0.1.7/PHStatsMethods.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-17 19:26:16.554658 phstatsmethods-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 19:26:16.554658 phstatsmethods-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-17 19:26:12.000000 phstatsmethods-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    35170 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.737615 phstatsmethods-0.1.8/PHStatsMethods/
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/DSR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/ISRate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/ISRatio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9951 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/confidence_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/funnels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/means.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/proportions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/quantiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/utils_funnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/PHStatsMethods/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/PHStatsMethods.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:16:49.000000 phstatsmethods-0.1.8/PHStatsMethods.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:16:49.741615 phstatsmethods-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 10:16:46.000000 phstatsmethods-0.1.8/setup.py
```

### Comparing `phstatsmethods-0.1.7/LICENSE.md` & `phstatsmethods-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/DSR.py` & `phstatsmethods-0.1.8/PHStatsMethods/DSR.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/ISRate.py` & `phstatsmethods-0.1.8/PHStatsMethods/ISRate.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/ISRatio.py` & `phstatsmethods-0.1.8/PHStatsMethods/ISRatio.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/confidence_intervals.py` & `phstatsmethods-0.1.8/PHStatsMethods/confidence_intervals.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/funnels.py` & `phstatsmethods-0.1.8/PHStatsMethods/funnels.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/means.py` & `phstatsmethods-0.1.8/PHStatsMethods/means.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/proportions.py` & `phstatsmethods-0.1.8/PHStatsMethods/proportions.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/quantiles.py` & `phstatsmethods-0.1.8/PHStatsMethods/quantiles.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/rates.py` & `phstatsmethods-0.1.8/PHStatsMethods/rates.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/utils.py` & `phstatsmethods-0.1.8/PHStatsMethods/utils.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/utils_funnel.py` & `phstatsmethods-0.1.8/PHStatsMethods/utils_funnel.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods/validation.py` & `phstatsmethods-0.1.8/PHStatsMethods/validation.py`

 * *Files identical despite different names*

### Comparing `phstatsmethods-0.1.7/PHStatsMethods.egg-info/SOURCES.txt` & `phstatsmethods-0.1.8/PHStatsMethods.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE.md
+README.md
 setup.py
 PHStatsMethods/DSR.py
 PHStatsMethods/ISRate.py
 PHStatsMethods/ISRatio.py
 PHStatsMethods/__init__.py
 PHStatsMethods/confidence_intervals.py
 PHStatsMethods/funnels.py
```

### Comparing `phstatsmethods-0.1.7/setup.py` & `phstatsmethods-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import setup
 
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
 setup(
     name='PHStatsMethods',
-    version='0.1.7',
+    version='0.1.8',
     packages=['PHStatsMethods'],
     url='https://github.com/DataS-DHSC/PHStatsMethods',
-    license='GPL3',
+    license='GPL-3.0',
     author='Department of Health and Social Care',
     author_email='annabel.westermann@dhsc.gov.uk, hadley.nanayakkara@dhsc.gov.uk, cameron.stewart@dhsc.gov.uk, jack.burden@dhsc.gov.uk, thilaksan.vikneswaran@dhsc.gov.uk, paul.fryers@dhsc.gov.uk, karandeep.kaur@dhsc.gov.uk, phds@phe.gov.uk',
     description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
-    long_description='This is a python package to calculate statistics in public health, including indicators for Fingertips.',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     install_requires=['numpy >= 1.24.0',
                       'pandas >= 2.0.0',
                       'pytest >= 8.0.0',
                       'scipy >= 1.8.0',
                       'openpyxl >= 3.1.0'],
 )
```

