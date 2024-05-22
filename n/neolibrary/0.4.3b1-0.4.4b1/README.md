# Comparing `tmp/neolibrary-0.4.3b1.tar.gz` & `tmp/neolibrary-0.4.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neolibrary-0.4.3b1.tar", max compression
+gzip compressed data, was "neolibrary-0.4.4b1.tar", max compression
```

## Comparing `neolibrary-0.4.3b1.tar` & `neolibrary-0.4.4b1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-05-06 12:58:22.221624 neolibrary-0.4.3b1/LICENSE
--rw-r--r--   0        0        0     3284 2024-05-06 12:58:22.221624 neolibrary-0.4.3b1/README.md
--rw-r--r--   0        0        0     1889 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/__init__.py
--rw-r--r--   0        0        0      696 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/decorators.py
--rw-r--r--   0        0        0        0 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/__init__.py
--rw-r--r--   0        0        0      770 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/config/config.py
--rw-r--r--   0        0        0     8365 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/monitoring/logger.py
--rw-r--r--   0        0        0      144 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/preproc.py
--rw-r--r--   0        0        0    26817 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/thumbnail_creator.py
--rw-r--r--   0        0        0     8628 2024-05-06 12:58:22.225625 neolibrary-0.4.3b1/src/neolibrary/utils.py
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 neolibrary-0.4.3b1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-08 11:19:06.171593 neolibrary-0.4.4b1/LICENSE
+-rw-r--r--   0        0        0     3284 2024-02-15 15:42:08.595159 neolibrary-0.4.4b1/README.md
+-rw-r--r--   0        0        0     1889 2024-05-22 12:57:37.804001 neolibrary-0.4.4b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-08 11:19:06.171593 neolibrary-0.4.4b1/src/neolibrary/__init__.py
+-rw-r--r--   0        0        0      696 2024-02-12 11:41:50.573522 neolibrary-0.4.4b1/src/neolibrary/decorators.py
+-rw-r--r--   0        0        0        0 2023-11-08 11:19:06.175593 neolibrary-0.4.4b1/src/neolibrary/monitoring/__init__.py
+-rw-r--r--   0        0        0      770 2024-02-12 11:41:50.573522 neolibrary-0.4.4b1/src/neolibrary/monitoring/config/config.py
+-rw-r--r--   0        0        0     8365 2024-02-12 11:51:19.368824 neolibrary-0.4.4b1/src/neolibrary/monitoring/logger.py
+-rw-r--r--   0        0        0      144 2024-02-12 11:51:19.368824 neolibrary-0.4.4b1/src/neolibrary/preproc.py
+-rw-r--r--   0        0        0    27021 2024-05-22 12:57:32.704069 neolibrary-0.4.4b1/src/neolibrary/thumbnail_creator.py
+-rw-r--r--   0        0        0     8628 2024-02-12 11:41:50.577522 neolibrary-0.4.4b1/src/neolibrary/utils.py
+-rw-r--r--   0        0        0     4100 1970-01-01 00:00:00.000000 neolibrary-0.4.4b1/PKG-INFO
```

### Comparing `neolibrary-0.4.3b1/LICENSE` & `neolibrary-0.4.4b1/LICENSE`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/README.md` & `neolibrary-0.4.4b1/README.md`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/pyproject.toml` & `neolibrary-0.4.4b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'neolibrary'
-version = "v0.4.3b1"
+version = "v0.4.4b1"
 description = 'The general utils library for neomedsys development'
 authors = ['Martin Soria Røvang <martinrovang@gmail.com>']
 license = 'Apache-2.0 license'
 readme = 'README.md'
 
 [tool.poetry.dependencies]
 python = '^3.9'
```

### Comparing `neolibrary-0.4.3b1/src/neolibrary/decorators.py` & `neolibrary-0.4.4b1/src/neolibrary/decorators.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/src/neolibrary/monitoring/config/config.py` & `neolibrary-0.4.4b1/src/neolibrary/monitoring/config/config.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/src/neolibrary/monitoring/logger.py` & `neolibrary-0.4.4b1/src/neolibrary/monitoring/logger.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/src/neolibrary/thumbnail_creator.py` & `neolibrary-0.4.4b1/src/neolibrary/thumbnail_creator.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,17 +674,21 @@
         np.ndarray
             The oriented image array.
 
         """
         self.manage_save_cache()
         log.info('Orienting volume to LPI')
         tempfilename = os.path.join(ROOT, 'temp', str(uuid.uuid4()) + '.nii.gz')
-        nifti = nib.Nifti1Image(image, affine)
-        nib.save(nifti, tempfilename)
-        simple_payload = sitk.ReadImage(tempfilename)
+        try:
+            nifti = nib.Nifti1Image(image, affine)
+            nib.save(nifti, tempfilename)
+            simple_payload = sitk.ReadImage(tempfilename)
+        except Exception as e:
+            log.warning(f'Error reading nifti file: {e}, setting affine to identity...')
+            simple_payload = sitk.GetImageFromArray(image)
         # RPI, LPI, RAI, LAI, RPS, LPS, RAS, LAS
         data_payload_re = sitk.DICOMOrient(simple_payload, 'LPI')
         spacings = list(data_payload_re.GetSpacing()[::-1])
         data_payload_re = sitk.GetArrayFromImage(data_payload_re)
         log.success('=> Volume oriented to LPI')
         return data_payload_re, spacings
```

### Comparing `neolibrary-0.4.3b1/src/neolibrary/utils.py` & `neolibrary-0.4.4b1/src/neolibrary/utils.py`

 * *Files identical despite different names*

### Comparing `neolibrary-0.4.3b1/PKG-INFO` & `neolibrary-0.4.4b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: neolibrary
-Version: 0.4.3b1
+Version: 0.4.4b1
 Summary: The general utils library for neomedsys development
 License: Apache-2.0 license
 Author: Martin Soria Røvang
 Author-email: martinrovang@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: arrow (>=1.2.3,<2.0.0)
 Requires-Dist: blosc (>=1.11.1,<2.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: scikit-image (>=0.22.0,<0.23.0)
 Requires-Dist: simpleitk (>=2.0.0,<3.0.0)
```

