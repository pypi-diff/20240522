# Comparing `tmp/ms2lipid-0.1.2.tar.gz` & `tmp/ms2lipid-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms2lipid-0.1.2.tar", max compression
+gzip compressed data, was "ms2lipid-0.1.3.tar", max compression
```

## Comparing `ms2lipid-0.1.2.tar` & `ms2lipid-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      598 2024-05-21 13:02:21.127197 ms2lipid-0.1.2/README.md
--rw-r--r--   0        0        0       29 2024-05-21 14:30:40.183120 ms2lipid-0.1.2/ms2lipid/__init__.py
--rw-r--r--   0        0        0    14684 2024-05-21 09:47:51.276164 ms2lipid-0.1.2/ms2lipid/ms2slipid_func.py
--rw-r--r--   0        0        0      844 2024-05-21 14:38:33.887963 ms2lipid-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 ms2lipid-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      598 2024-05-21 13:02:21.127197 ms2lipid-0.1.3/README.md
+-rw-r--r--   0        0        0       23 2024-05-22 02:12:01.935591 ms2lipid-0.1.3/ms2lipid/__init__.py
+-rw-r--r--   0        0        0    14678 2024-05-22 01:49:57.970792 ms2lipid-0.1.3/ms2lipid/ms2lipid.py
+-rw-r--r--   0        0        0      844 2024-05-22 00:48:30.018557 ms2lipid-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1472 1970-01-01 00:00:00.000000 ms2lipid-0.1.3/PKG-INFO
```

### Comparing `ms2lipid-0.1.2/README.md` & `ms2lipid-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ms2lipid-0.1.2/ms2lipid/ms2slipid_func.py` & `ms2lipid-0.1.3/ms2lipid/ms2lipid.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,10 +361,8 @@
     else:
         if exppath == None: #show df 
             return df_test_predclass_eval
         else:  #save df
             df_test_predclass_eval.to_csv(exppath, index=False)
             return df_test_predclass_eval
         
-__all__ = ['predclass', 'prediction_summary']
-
-
+__all__ = ['predclass', 'prediction_summary']
```

### Comparing `ms2lipid-0.1.2/PKG-INFO` & `ms2lipid-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms2lipid
-Version: 0.1.2
+Version: 0.1.3
 Summary: ms2lipid is a Python library for predicted lipid class by using ms2 spectrum.
 Home-page: https://github.com/systemsomicslab/ms2lipid
 License: MIT
 Author: NamiSakamoto
 Author-email: 123930464+NamiSakamoto@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

