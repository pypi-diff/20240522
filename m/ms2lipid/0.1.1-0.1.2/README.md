# Comparing `tmp/ms2lipid-0.1.1.tar.gz` & `tmp/ms2lipid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2lipid-0.1.1.tar", max compression
+gzip compressed data, was "ms2lipid-0.1.2.tar", max compression
```

## Comparing `ms2lipid-0.1.1.tar` & `ms2lipid-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      598 2024-05-21 13:02:21.127197 ms2lipid-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-21 08:14:36.587584 ms2lipid-0.1.1/ms2lipid/__init__.py
--rw-r--r--   0        0        0    14684 2024-05-21 09:47:51.276164 ms2lipid-0.1.1/ms2lipid/ms2slipid_func.py
--rw-r--r--   0        0        0      844 2024-05-21 10:28:48.813274 ms2lipid-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 ms2lipid-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      598 2024-05-21 13:02:21.127197 ms2lipid-0.1.2/README.md
+-rw-r--r--   0        0        0       29 2024-05-21 14:30:40.183120 ms2lipid-0.1.2/ms2lipid/__init__.py
+-rw-r--r--   0        0        0    14684 2024-05-21 09:47:51.276164 ms2lipid-0.1.2/ms2lipid/ms2slipid_func.py
+-rw-r--r--   0        0        0      844 2024-05-21 14:38:33.887963 ms2lipid-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 ms2lipid-0.1.2/PKG-INFO
```

### Comparing `ms2lipid-0.1.1/README.md` & `ms2lipid-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ms2lipid-0.1.1/ms2lipid/ms2slipid_func.py` & `ms2lipid-0.1.2/ms2lipid/ms2slipid_func.py`

 * *Files identical despite different names*

### Comparing `ms2lipid-0.1.1/pyproject.toml` & `ms2lipid-0.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms2lipid"
-version = "0.1.1"
+version = "0.1.2"
 description = "ms2lipid is a Python library for predicted lipid class by using ms2 spectrum."
 license = 'MIT'
 authors = ["NamiSakamoto <123930464+NamiSakamoto@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/systemsomicslab/ms2lipid"
 
 [tool.poetry.dependencies]
```

### Comparing `ms2lipid-0.1.1/PKG-INFO` & `ms2lipid-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2lipid
-Version: 0.1.1
+Version: 0.1.2
 Summary: ms2lipid is a Python library for predicted lipid class by using ms2 spectrum.
 Home-page: https://github.com/systemsomicslab/ms2lipid
 License: MIT
 Author: NamiSakamoto
 Author-email: 123930464+NamiSakamoto@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

