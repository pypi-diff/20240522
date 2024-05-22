# Comparing `tmp/fred_pandas-0.0.2.tar.gz` & `tmp/fred_pandas-0.0.3.tar.gz`

## Comparing `fred_pandas-0.0.2.tar` & `fred_pandas-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/src/fred_pandas/__init__.py
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/src/fred_pandas/fred_pandas.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/LICENSE
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/README.md
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fred_pandas-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/src/fred_pandas/__init__.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/src/fred_pandas/fred_pandas.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/LICENSE
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/README.md
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 fred_pandas-0.0.3/PKG-INFO
```

### Comparing `fred_pandas-0.0.2/src/fred_pandas/fred_pandas.py` & `fred_pandas-0.0.3/src/fred_pandas/fred_pandas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import requests
 import pandas as pd
+import pathlib
 
 # ----------------------------------------------------------------------
 def download_series_after(series, observation_start=None):
 
     url = 'https://api.stlouisfed.org/fred/series/observations'
 
     if observation_start is None:
@@ -54,17 +55,19 @@
 
         df = download_series_after(series, observation_start)
 
         df.to_pickle(path)
 
         return df
 # ----------------------------------------------------------------------
-def load_records(series, observation_start=None, update=False):
+def load_records(series, observation_start=None, update=False, pkl_path='pkl'):
 
-    path = f'{series}.pkl'
+    # path = f'{series}.pkl'
+
+    path = os.path.join(pkl_path, f'{series}.pkl')
 
     if os.path.isfile(path):
 
         print(f'Found {path}. Importing.')
 
         df = pd.read_pickle(path)
 
@@ -87,11 +90,24 @@
 
     else:
 
         print(f'Using observation_start={observation_start}.')
 
         df = download_series_after(series, observation_start)
 
+        # Ensure path to pkl file exists
+
+        pathlib.Path(os.path.dirname(path)).mkdir(parents=True, exist_ok=True)
+
         df.to_pickle(path)
 
         return df
+
 # ----------------------------------------------------------------------
+
+# get series name from command line
+
+if __name__ == '__main__':
+    import sys
+    series = sys.argv[1]
+    df = load_records(series=series, update=True)
+    print(df)
```

### Comparing `fred_pandas-0.0.2/LICENSE` & `fred_pandas-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fred_pandas-0.0.2/pyproject.toml` & `fred_pandas-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fred_pandas"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Eduardo Cavazos", email="wayo.cavazos@gmail.com" },
 ]
 description = "Library for downloading FRED series data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fred_pandas-0.0.2/PKG-INFO` & `fred_pandas-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fred_pandas
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for downloading FRED series data
 Project-URL: Homepage, https://github.com/dharmatech/fred_pandas.py
 Project-URL: Issues, https://github.com/dharmatech/fred_pandas.py/issues
 Author-email: Eduardo Cavazos <wayo.cavazos@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

