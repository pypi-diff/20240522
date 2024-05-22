# Comparing `tmp/input4mips_validation-0.3.1.tar.gz` & `tmp/input4mips_validation-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "input4mips_validation-0.3.1.tar", max compression
+gzip compressed data, was "input4mips_validation-0.3.2.tar", max compression
```

## Comparing `input4mips_validation-0.3.1.tar` & `input4mips_validation-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1685 2024-04-23 11:14:44.237952 input4mips_validation-0.3.1/LICENCE
--rw-r--r--   0        0        0     3810 2024-04-23 11:14:44.237952 input4mips_validation-0.3.1/README.md
--rw-r--r--   0        0        0     5606 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      171 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/__init__.py
--rw-r--r--   0        0        0     3795 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/attrs_helpers.py
--rw-r--r--   0        0        0     1164 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/cli/__init__.py
--rw-r--r--   0        0        0     1031 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/cli/cli_logging.py
--rw-r--r--   0        0        0       39 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/constants.py
--rw-r--r--   0        0        0      613 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/file_id.py
--rw-r--r--   0        0        0     3688 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
--rw-r--r--   0        0        0     4384 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
--rw-r--r--   0        0        0     6986 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
--rw-r--r--   0        0        0      740 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
--rw-r--r--   0        0        0     2257 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
--rw-r--r--   0        0        0      779 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/email.py
--rw-r--r--   0        0        0      634 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
--rw-r--r--   0        0        0    10284 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/dataset.py
--rw-r--r--   0        0        0      674 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/exceptions.py
--rw-r--r--   0        0        0     3553 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/metadata.py
--rw-r--r--   0        0        0        0 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/py.typed
--rw-r--r--   0        0        0     1429 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/testing.py
--rw-r--r--   0        0        0     5886 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/time.py
--rw-r--r--   0        0        0     1691 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/validation/__init__.py
--rw-r--r--   0        0        0     4207 2024-04-23 11:14:44.241952 input4mips_validation-0.3.1/src/input4mips_validation/xarray_helpers.py
--rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 input4mips_validation-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1685 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/LICENCE
+-rw-r--r--   0        0        0     3810 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/README.md
+-rw-r--r--   0        0        0     5606 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      171 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/__init__.py
+-rw-r--r--   0        0        0     3795 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/attrs_helpers.py
+-rw-r--r--   0        0        0     1164 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/cli/__init__.py
+-rw-r--r--   0        0        0     1031 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/cli/cli_logging.py
+-rw-r--r--   0        0        0       39 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/__init__.py
+-rw-r--r--   0        0        0     2029 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/constants.py
+-rw-r--r--   0        0        0      613 2024-05-22 13:06:51.978783 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/file_id.py
+-rw-r--r--   0        0        0     3688 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/inference/__init__.py
+-rw-r--r--   0        0        0     4384 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/__init__.py
+-rw-r--r--   0        0        0     6986 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py
+-rw-r--r--   0        0        0      740 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py
+-rw-r--r--   0        0        0     2257 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py
+-rw-r--r--   0        0        0      779 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/email.py
+-rw-r--r--   0        0        0      634 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/uuid.py
+-rw-r--r--   0        0        0    10284 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/dataset.py
+-rw-r--r--   0        0        0      674 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/exceptions.py
+-rw-r--r--   0        0        0     3553 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/metadata.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/py.typed
+-rw-r--r--   0        0        0     1429 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/testing.py
+-rw-r--r--   0        0        0     5886 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/time.py
+-rw-r--r--   0        0        0     1691 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/validation/__init__.py
+-rw-r--r--   0        0        0     4207 2024-05-22 13:06:51.982782 input4mips_validation-0.3.2/src/input4mips_validation/xarray_helpers.py
+-rw-r--r--   0        0        0     4942 1970-01-01 00:00:00.000000 input4mips_validation-0.3.2/PKG-INFO
```

### Comparing `input4mips_validation-0.3.1/LICENCE` & `input4mips_validation-0.3.2/LICENCE`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/README.md` & `input4mips_validation-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/pyproject.toml` & `input4mips_validation-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "input4mips-validation"
-version = "0.3.1"
+version = "0.3.2"
 description = "Validation of input4MIPs data (checking file formats, metadata etc.)."
 authors = ["Zebedee Nicholls <zebedee.nicholls@climate-resource.com>"]
 readme = "README.md"
 packages = [{include = "input4mips_validation", from = "src"}]
 license = "BSD-3-Clause"
 include = ["LICENCE"]  # poetry uses US English so assumes it will be spelt LICENSE
```

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/attrs_helpers.py` & `input4mips_validation-0.3.2/src/input4mips_validation/attrs_helpers.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/cli/__init__.py` & `input4mips_validation-0.3.2/src/input4mips_validation/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/cli/cli_logging.py` & `input4mips_validation-0.3.2/src/input4mips_validation/cli/cli_logging.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/constants.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,26 +11,30 @@
     "tos": "SSTsAndSeaIce",
     "siconc": "SSTsAndSeaIce",
     "sftof": "SSTsAndSeaIce",
     "areacello": "SSTsAndSeaIce",
     "mole_fraction_of_carbon_dioxide_in_air": "GHGConcentrations",
     "mole_fraction_of_methane_in_air": "GHGConcentrations",
     "mole_fraction_of_nitrous_oxide_in_air": "GHGConcentrations",
+    "mole_fraction_of_sulfur_hexafluoride_in_air": "GHGConcentrations",
+    "mole_fraction_of_cfc11_in_air": "GHGConcentrations",
 }
 
 # TODO: remove this hard-coding based on some logic/map held elsewhere,
 # e.g. CVs website, that defines this map
 VARIABLE_REALM_MAP = {
     "tos": "ocean",
     "siconc": "seaIce",
     "sftof": "ocean",
     "areacello": "ocean",
     "mole_fraction_of_carbon_dioxide_in_air": "atmos",
     "mole_fraction_of_methane_in_air": "atmos",
     "mole_fraction_of_nitrous_oxide_in_air": "atmos",
+    "mole_fraction_of_sulfur_hexafluoride_in_air": "atmos",
+    "mole_fraction_of_cfc11_in_air": "atmos",
 }
 
 CREATION_DATE_REGEX: re.Pattern[str] = re.compile(
     r"^[0-9]{4}-[0-9]{2}-[0-9]{2}T[0-9]{2}:[0-9]{2}:[0-9]{2}Z$"
 )
 """
 Regular expression that checks the creation date is formatted correctly
```

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/file_id.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/file_id.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/inference/__init__.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/__init__.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/comparison_with_cvs.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/creation_date.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/ds_metadata_consistency.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/email.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/email.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/controlled_vocabularies/validators/uuid.py` & `input4mips_validation-0.3.2/src/input4mips_validation/controlled_vocabularies/validators/uuid.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/dataset.py` & `input4mips_validation-0.3.2/src/input4mips_validation/dataset.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/exceptions.py` & `input4mips_validation-0.3.2/src/input4mips_validation/exceptions.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/metadata.py` & `input4mips_validation-0.3.2/src/input4mips_validation/metadata.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/testing.py` & `input4mips_validation-0.3.2/src/input4mips_validation/testing.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/time.py` & `input4mips_validation-0.3.2/src/input4mips_validation/time.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/validation/__init__.py` & `input4mips_validation-0.3.2/src/input4mips_validation/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/src/input4mips_validation/xarray_helpers.py` & `input4mips_validation-0.3.2/src/input4mips_validation/xarray_helpers.py`

 * *Files identical despite different names*

### Comparing `input4mips_validation-0.3.1/PKG-INFO` & `input4mips_validation-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: input4mips-validation
-Version: 0.3.1
+Version: 0.3.2
 Summary: Validation of input4MIPs data (checking file formats, metadata etc.).
 License: BSD-3-Clause
 Author: Zebedee Nicholls
 Author-email: zebedee.nicholls@climate-resource.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

