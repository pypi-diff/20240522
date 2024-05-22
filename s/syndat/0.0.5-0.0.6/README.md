# Comparing `tmp/syndat-0.0.5.tar.gz` & `tmp/syndat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndat-0.0.5.tar", last modified: Fri May 10 12:59:36 2024, max compression
+gzip compressed data, was "syndat-0.0.6.tar", last modified: Tue May 21 13:54:21 2024, max compression
```

## Comparing `syndat-0.0.5.tar` & `syndat-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-10 12:59:32.000000 syndat-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:59:36.206779 syndat-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-10 12:59:32.000000 syndat-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 12:59:36.206779 syndat-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-10 12:59:34.000000 syndat-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/syndat/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/quality.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-10 12:59:32.000000 syndat-0.0.5/syndat/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/syndat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 12:59:36.000000 syndat-0.0.5/syndat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 12:59:36.206779 syndat-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_auc.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-10 12:59:32.000000 syndat-0.0.5/tests/test_jsd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 13:54:17.000000 syndat-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 13:54:21.503998 syndat-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-21 13:54:17.000000 syndat-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:54:21.503998 syndat-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-21 13:54:19.000000 syndat-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/syndat/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-21 13:54:17.000000 syndat-0.0.6/syndat/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/syndat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 13:54:21.000000 syndat-0.0.6/syndat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:54:21.503998 syndat-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_auc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-21 13:54:17.000000 syndat-0.0.6/tests/test_jsd.py
```

### Comparing `syndat-0.0.5/LICENSE` & `syndat-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `syndat-0.0.5/setup.py` & `syndat-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='syndat',
-    version='v0.0.5',
+    version='v0.0.6',
     packages=['syndat'],
     url='https://github.com/SCAI-BIO/syndat',
     license='CC BY-NC-ND 4.0.',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `syndat-0.0.5/syndat/quality.py` & `syndat-0.0.6/syndat/quality.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,10 +109,13 @@
     """
     corr_real = real.corr()
     corr_synthetic = synthetic.corr()
     norm_diff = np.linalg.norm(corr_real - corr_synthetic)
     norm_real = np.linalg.norm(corr_real)
     norm_quotient = norm_diff / norm_real
     if score:
+        # will not happen in a realistic scenario, only if (nearly) all correlations are opposing
+        if norm_quotient > 1:
+            return 0
         return (1 - max(norm_quotient, 0)) * 100
     else:
         return norm_quotient
```

### Comparing `syndat-0.0.5/syndat/visualization.py` & `syndat-0.0.6/syndat/visualization.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.5/tests/test_auc.py` & `syndat-0.0.6/tests/test_auc.py`

 * *Files identical despite different names*

### Comparing `syndat-0.0.5/tests/test_correlation.py` & `syndat-0.0.6/tests/test_correlation.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,20 +13,34 @@
             'B': [5, 4, 3, 2, 1]
         })
         synthetic_data = pd.DataFrame({
             'A': [1, 2, 3, 4, 5],
             'B': [5, 4, 3, 2, 1]
         })
         result = correlation(real_data, synthetic_data)
-        self.assertEqual(result, 100, "Correlation score should be 100 for identical datasets")
+        self.assertEqual(100, result, "Correlation score should be 100 for identical datasets")
+
+    def test_correlation_zero(self):
+        # positive correlation
+        real_data = pd.DataFrame({
+            'A': [-1, 1, -2, 2, -3],
+            'B': [-2, 2, -4, 4, -6]
+        })
+        # negative correlation
+        synthetic_data = pd.DataFrame({
+            'A': [1, -1, 2, -2, 3],
+            'B': [-1, 1, -2, 2, -3]
+        })
+        result = correlation(real_data, synthetic_data)
+        self.assertEqual(0, result)
 
     def test_correlation_normalized(self):
         real_data = pd.DataFrame({
             'A': [1, 2, 3, 4, 5],
             'B': [5, 4, 3, 2, 1]
         })
         synthetic_data = pd.DataFrame({
             'A': [1, 2, 3, 4, 5],
             'B': [5, 4, 3, 2, 1]
         })
         result = correlation(real_data, synthetic_data, score=False)
-        self.assertEqual(result, 0, "Normalized correlation score should be 0 for identical datasets")
+        self.assertEqual(0, result, "Normalized correlation score should be 0 for identical datasets")
```

### Comparing `syndat-0.0.5/tests/test_jsd.py` & `syndat-0.0.6/tests/test_jsd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from unittest import TestCase
 
 import pandas as pd
 
 import syndat
 
+
 class Test(TestCase):
 
     def test_jsd_zero_int64(self):
         synthetic = pd.DataFrame({
             'feature1': [1, 2, 3, 4, 5],
             'feature2': [10, 11, 12, 13, 14]
         })
@@ -54,21 +55,20 @@
         real = pd.DataFrame({
             'feature1': [1, 2, 1, 2, 3],
             'feature2': [0.1, 0.2, 0.3, 0.4, 0.5]
         })
         jsd = syndat.quality.jsd(real, synthetic)
         self.assertEqual(jsd, 100)
 
-    def test_jsd_different_coltypes(self):
+    def test_jsd_different_col_types(self):
         synthetic = pd.DataFrame({
             'feature1': [1, 2, 1, 2, 3],
             'feature2': [1.1, 2.1, 3.1, 4.1, 5.1]
         })
         # Create real data
         real = pd.DataFrame({
             'feature1': [1.2, 2.1, 1.1, 2.1, 3.1],
             'feature2': [1, 2, 3, 4, 5]
         })
         jsd = syndat.quality.jsd(real, synthetic, score=False)
         print(jsd)
         print(jsd)
-
```

