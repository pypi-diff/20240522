# Comparing `tmp/openclimatedata-0.8.tar.gz` & `tmp/openclimatedata-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openclimatedata-0.8.tar", last modified: Thu Jan 18 13:26:03 2024, max compression
+gzip compressed data, was "openclimatedata-0.9.tar", last modified: Wed Jan 24 20:30:01 2024, max compression
```

## Comparing `openclimatedata-0.8.tar` & `openclimatedata-0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:03.803407 openclimatedata-0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-18 13:25:55.000000 openclimatedata-0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-18 13:26:03.803407 openclimatedata-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-18 13:25:55.000000 openclimatedata-0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-18 13:25:55.000000 openclimatedata-0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 13:26:03.803407 openclimatedata-0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:03.799407 openclimatedata-0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:03.799407 openclimatedata-0.8/src/openclimatedata/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-18 13:25:55.000000 openclimatedata-0.8/src/openclimatedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-01-18 13:25:55.000000 openclimatedata-0.8/src/openclimatedata/_gcb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-01-18 13:25:55.000000 openclimatedata-0.8/src/openclimatedata/_gcb_fossil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-18 13:25:55.000000 openclimatedata-0.8/src/openclimatedata/_gcb_national.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-01-18 13:25:55.000000 openclimatedata-0.8/src/openclimatedata/_primap_hist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:03.803407 openclimatedata-0.8/src/openclimatedata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-18 13:26:03.000000 openclimatedata-0.8/src/openclimatedata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-18 13:26:03.000000 openclimatedata-0.8/src/openclimatedata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 13:26:03.000000 openclimatedata-0.8/src/openclimatedata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 13:26:03.000000 openclimatedata-0.8/src/openclimatedata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-18 13:26:03.000000 openclimatedata-0.8/src/openclimatedata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 13:26:03.803407 openclimatedata-0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-18 13:25:55.000000 openclimatedata-0.8/tests/test_gcb_fossil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-18 13:25:55.000000 openclimatedata-0.8/tests/test_primaphist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:30:01.868310 openclimatedata-0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-01-24 20:29:53.000000 openclimatedata-0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-24 20:30:01.868310 openclimatedata-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-24 20:29:53.000000 openclimatedata-0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-24 20:29:53.000000 openclimatedata-0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-24 20:30:01.868310 openclimatedata-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:30:01.864310 openclimatedata-0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:30:01.864310 openclimatedata-0.9/src/openclimatedata/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-24 20:29:53.000000 openclimatedata-0.9/src/openclimatedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-01-24 20:29:53.000000 openclimatedata-0.9/src/openclimatedata/_gcb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-01-24 20:29:53.000000 openclimatedata-0.9/src/openclimatedata/_gcb_fossil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-01-24 20:29:53.000000 openclimatedata-0.9/src/openclimatedata/_gcb_national.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-01-24 20:29:53.000000 openclimatedata-0.9/src/openclimatedata/_primap_hist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:30:01.864310 openclimatedata-0.9/src/openclimatedata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-01-24 20:30:01.000000 openclimatedata-0.9/src/openclimatedata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-01-24 20:30:01.000000 openclimatedata-0.9/src/openclimatedata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-24 20:30:01.000000 openclimatedata-0.9/src/openclimatedata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-24 20:30:01.000000 openclimatedata-0.9/src/openclimatedata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-24 20:30:01.000000 openclimatedata-0.9/src/openclimatedata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-24 20:30:01.864310 openclimatedata-0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-01-24 20:29:53.000000 openclimatedata-0.9/tests/test_gcb_fossil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-24 20:29:53.000000 openclimatedata-0.9/tests/test_primaphist.py
```

### Comparing `openclimatedata-0.8/LICENSE` & `openclimatedata-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openclimatedata-0.8/PKG-INFO` & `openclimatedata-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclimatedata
-Version: 0.8
+Version: 0.9
 Summary: Library to help download and locally cache climate data
 Author: Robert Gieseke
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/openclimatedata/openclimatedata
 Project-URL: Changelog, https://github.com/openclimatedata/openclimatedata/releases
 Project-URL: Issues, https://github.com/openclimatedata/openclimatedata/issues
 Project-URL: CI, https://github.com/openclimatedat/openclimatedata/actions
```

### Comparing `openclimatedata-0.8/pyproject.toml` & `openclimatedata-0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "openclimatedata"
-version = "0.8"
+version = "0.9"
 description = "Library to help download and locally cache climate data"
 readme = "README.md"
 authors = [{name = "Robert Gieseke"}]
 license = {text = "BSD-2-Clause"}
 requires-python = ">=3.8"
 dependencies = [
     "openpyxl", "pandas", "pooch", "tqdm"
```

### Comparing `openclimatedata-0.8/src/openclimatedata/_gcb.py` & `openclimatedata-0.9/src/openclimatedata/_gcb.py`

 * *Files identical despite different names*

### Comparing `openclimatedata-0.8/src/openclimatedata/_gcb_fossil.py` & `openclimatedata-0.9/src/openclimatedata/_gcb_fossil.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,24 +39,30 @@
     def to_long_dataframe(self):
         """
         Turn GCB Fossil data into a long dataframe and add source metadata
         as a column. `ISO 3166-1 alpha-3` is renamed to `Code`.
         """
         df = self.to_dataframe()
 
+        if "UN M49" in df.columns:
+            df = df.drop("UN M49", axis=1)
+
         file_path_sources = pooch.retrieve(
             path=pooch.os_cache("openclimatedata"),
             fname=self.filename_sources,
             url=self.url_sources,
             known_hash=self.hash_sources,
         )
         df_sources = pd.read_csv(file_path_sources, encoding="latin-1")
 
+        if "UN M49" in df_sources.columns:
+            df_sources = df_sources.drop("UN M49", axis=1)
+
         # Saint Kitts and Nevis and St. Kitts-Nevis-Anguilla both use KNA.
-        # It's replaced with NaN and treated as below to be differentiable.
+        # The code is replaced with NaN and treated as below to be differentiable.
         if len(df[df["ISO 3166-1 alpha-3"] == "KNA"].Country.unique()) > 1:
             df["ISO 3166-1 alpha-3"] = df["ISO 3166-1 alpha-3"].replace("KNA", np.nan)
             df_sources["ISO 3166-1 alpha-3"] = df_sources["ISO 3166-1 alpha-3"].replace(
                 "KNA", np.nan
             )
 
         # A few islands and Kuwaiti oil fires have no code, reusing country.
@@ -91,14 +97,27 @@
         df = self.to_long_dataframe()
         df.columns = df.columns.map(lambda x: x.lower())
 
         return df
 
 
 GCB_Fossil_Emissions = {
+    "2023v43": _GCB_Fossil(
+        name="The Global Carbon Project's fossil CO2 emissions dataset",
+        doi="10.5281/zenodo.10562476",
+        published="2024-01-24",
+        filename="GCB2023v43_MtCO2_flat.csv",
+        url="https://zenodo.org/records/10562476/files/GCB2023v43_MtCO2_flat.csv",
+        hash="md5:e8cc0ffc5b6a4dbc2c1ae2453dcfb859",
+        filename_sources="GCB2023v43_sources_flat.csv",
+        url_sources="https://zenodo.org/records/10562476/files/GCB2023v43_sources_flat.csv",
+        hash_sources="md5:1e88fa3eb7322628b7c4bf1f5a278d97",
+        citation="""Andrew, R. M., & Peters, G. P. (2024). The Global Carbon Project's fossil CO2 emissions dataset (2023v43) [Data set]. Zenodo. https://doi.org/10.5281/zenodo.10562476""",
+        license="CC BY 4.0",
+    ),
     "2023v36": _GCB_Fossil(
         name="The Global Carbon Project's fossil CO2 emissions dataset",
         doi="10.5281/zenodo.10177738",
         published="2023-11-21",
         filename="GCB2023v36_MtCO2_flat.csv",
         url="https://zenodo.org/records/10177738/files/GCB2023v36_MtCO2_flat.csv",
         hash="md5:5bb46f04063157eff3dcdca66c19c553",
```

### Comparing `openclimatedata-0.8/src/openclimatedata/_gcb_national.py` & `openclimatedata-0.9/src/openclimatedata/_gcb_national.py`

 * *Files identical despite different names*

### Comparing `openclimatedata-0.8/src/openclimatedata/_primap_hist.py` & `openclimatedata-0.9/src/openclimatedata/_primap_hist.py`

 * *Files identical despite different names*

### Comparing `openclimatedata-0.8/src/openclimatedata.egg-info/PKG-INFO` & `openclimatedata-0.9/src/openclimatedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openclimatedata
-Version: 0.8
+Version: 0.9
 Summary: Library to help download and locally cache climate data
 Author: Robert Gieseke
 License: BSD-2-Clause
 Project-URL: Homepage, https://github.com/openclimatedata/openclimatedata
 Project-URL: Changelog, https://github.com/openclimatedata/openclimatedata/releases
 Project-URL: Issues, https://github.com/openclimatedata/openclimatedata/issues
 Project-URL: CI, https://github.com/openclimatedat/openclimatedata/actions
```

### Comparing `openclimatedata-0.8/tests/test_gcb_fossil.py` & `openclimatedata-0.9/tests/test_gcb_fossil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 import os
 import pytest
 from pytest import approx
 
 from openclimatedata import GCB_Fossil_Emissions
 
 GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
@@ -57,14 +58,27 @@
         == leeward_islands[leeward_islands.Year == 1950].Total.values[0]
     )
 
     assert sum(df_long.Code.isnull()) == 0
 
 
 @pytest.mark.skipif(GITHUB_ACTIONS, reason="Test requires downloading.")
+def test_gcb_fossil_2023v43():
+    df = GCB_Fossil_Emissions["2023v43"].to_dataframe()
+    # This version has Cement with zero and Total as `nan`.
+    assert math.isnan(df.iloc[0]["Total"])
+    assert df.iloc[-1]["Per Capita"] == approx(4.658365)
+
+    ocdf = GCB_Fossil_Emissions["2023v43"].to_ocd()
+    # First and last value should be the same after re-shaping.
+    assert math.isnan(ocdf.iloc[0]["value"]) and ocdf.iloc[0]["category"] == "Total"
+    assert ocdf.iloc[-1]["value"] == df.iloc[-1]["Per Capita"]
+
+
+@pytest.mark.skipif(GITHUB_ACTIONS, reason="Test requires downloading.")
 def test_unique_code_name_combinations():
     # Saint Kitts and Nevis is included twice in GCB Fossil with code 'KNA'.
     # The second time the name is 'St-Kitts-Nevis-Anguilla'.
     # This should be handled in the long DataFrame which drops the country.
     for version in versions:
         df = GCB_Fossil_Emissions[version].to_dataframe()
         dfl = GCB_Fossil_Emissions[version].to_long_dataframe()
```

### Comparing `openclimatedata-0.8/tests/test_primaphist.py` & `openclimatedata-0.9/tests/test_primaphist.py`

 * *Files identical despite different names*

