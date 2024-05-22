# Comparing `tmp/giza_datasets-0.2.4.tar.gz` & `tmp/giza_datasets-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_datasets-0.2.4.tar", max compression
+gzip compressed data, was "giza_datasets-0.3.0.tar", max compression
```

## Comparing `giza_datasets-0.2.4.tar` & `giza_datasets-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/LICENSE
--rw-r--r--   0        0        0     3951 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/README.md
--rw-r--r--   0        0        0      136 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/__init__.py
--rw-r--r--   0        0        0     2853 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/cache_manager.py
--rw-r--r--   0        0        0   151370 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/constants.py
--rw-r--r--   0        0        0      635 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/defillama_constants.py
--rw-r--r--   0        0        0     3240 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/hub.py
--rw-r--r--   0        0        0     5982 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/loaders.py
--rw-r--r--   0        0        0     1441 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/giza_datasets/models.py
--rw-r--r--   0        0        0      554 2024-05-10 14:20:17.555941 giza_datasets-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3951 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/README.md
+-rw-r--r--   0        0        0      136 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/__init__.py
+-rw-r--r--   0        0        0     2854 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/cache_manager.py
+-rw-r--r--   0        0        0   151371 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/constants.py
+-rw-r--r--   0        0        0      635 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/defillama_constants.py
+-rw-r--r--   0        0        0     3240 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/hub.py
+-rw-r--r--   0        0        0     5984 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/loaders.py
+-rw-r--r--   0        0        0     1442 2024-05-22 13:55:03.524908 giza_datasets-0.3.0/giza/datasets/models.py
+-rw-r--r--   0        0        0      560 2024-05-22 13:55:03.528908 giza_datasets-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 giza_datasets-0.3.0/PKG-INFO
```

### Comparing `giza_datasets-0.2.4/LICENSE` & `giza_datasets-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.4/README.md` & `giza_datasets-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 1. Install the `giza-datasets` package if you haven't already:
    ```
    pip install giza-datasets
    ```
 2. Import the `DatasetsLoader` class and initialize it:
    ```python
-   from giza_datasets import DatasetsLoader
+   from giza.datasets import DatasetsLoader
    loader = DatasetsLoader()
    ```
 3. Optional: Depending on your device's configuration, it may be necessary to provide SSL certificates to verify the authenticity of HTTPS connections. You can ensure that all these certifications are correct by executing the following line of code:
    ```python
    import certifi
    import os
    os.environ['SSL_CERT_FILE'] = certifi.where()
@@ -52,15 +52,15 @@
 - `get(dataset_name)`: Returns a Dataset object with the given name.
 - `describe(dataset_name)`: Prints a table of details for the given dataset.
 
 To get started with the `DatasetsHub` class, follow the steps below:
 
 1. Import the `DatasetsHub` class and initialize it:
    ```python
-   from giza_datasets import DatasetsHub
+   from giza.datasets import DatasetsHub
    hub = DatasetsHub()
    ```
 2. Use the `show` method to print a table of all datasets in the hub:
    ```python
    hub.show()
    ```
 3. Use the `list` method to get a list of all datasets in the hub:
```

### Comparing `giza_datasets-0.2.4/giza_datasets/cache_manager.py` & `giza_datasets-0.3.0/giza/datasets/cache_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
+
 import polars as pl
 import pyarrow.dataset as ds
-import os
 
 
 class CacheManager:
     def __init__(self, cache_dir):
         """
         Initializes the CacheManager with a specified cache directory.
```

### Comparing `giza_datasets-0.2.4/giza_datasets/constants.py` & `giza_datasets-0.3.0/giza/datasets/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from giza_datasets.defillama_constants import DEFILLAMA_SUPPORTED_PROJECTS
-from giza_datasets.models import Dataset
+from giza.datasets.defillama_constants import DEFILLAMA_SUPPORTED_PROJECTS
+from giza.datasets.models import Dataset
 
 APPLICATION_TAGS = ["Liquid Staking", "Dexes", "Yield", "Lending", "Yield Aggregator"]
 
 DATASET_HUB = [
     Dataset(
         name="tvl-fee-per-protocol",
         path="gs://datasets-giza/TVL_fee_per_protocol",
@@ -2280,15 +2280,15 @@
         tags=["PancakeSwap", "Trade Volume", "daily", "DeFi", "DEX"],
         documentation="https://datasets.gizatech.xyz/hub/pancakeswap/daily-trade-volume",
     ),
     Dataset(
         name="curve-daily-volume-fees",
         path="gs://datasets-giza/Curve/curve_daily_volume_fees.parquet",
         description="Daily Curve trade volume and fees generated in USD, per pool",
-        tags=["Curve","Trade Volume","Fees" ,"daily", "DeFi", "DEX"],
+        tags=["Curve", "Trade Volume", "Fees", "daily", "DeFi", "DEX"],
         documentation="https://datasets.gizatech.xyz/hub/curve/daily-trade-volume-and-fees",
     ),
     Dataset(
         name="gora-competition-training",
         path="gs://datasets-giza/Rocifi/gora_competition_training.parquet",
         description="Training data for the Gora competition",
         tags=["Lending"],
@@ -2298,8 +2298,7 @@
         name="gora-competition-evaluation",
         path="gs://datasets-giza/Rocifi/gora_competition_evaluation.parquet",
         description="Evaluation Data for the Gora competition",
         tags=["Lending"],
         documentation="",
     ),
 ]
-
```

### Comparing `giza_datasets-0.2.4/giza_datasets/defillama_constants.py` & `giza_datasets-0.3.0/giza/datasets/defillama_constants.py`

 * *Files identical despite different names*

### Comparing `giza_datasets-0.2.4/giza_datasets/hub.py` & `giza_datasets-0.3.0/giza/datasets/hub.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rich.console import Console
 from rich.table import Table
 
-from giza_datasets.constants import DATASET_HUB
+from giza.datasets.constants import DATASET_HUB
 
 
 class DatasetsHub:
     """
     Class to manage datasets from the DATASET_HUB.
 
     Attributes:
```

### Comparing `giza_datasets-0.2.4/giza_datasets/loaders.py` & `giza_datasets-0.3.0/giza/datasets/loaders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+import os
+
 import gcsfs
 import polars as pl
-import os
-from giza_datasets.constants import DATASET_HUB
-from giza_datasets.cache_manager import CacheManager
+
+from giza.datasets.cache_manager import CacheManager
+from giza.datasets.constants import DATASET_HUB
 
 
 class DatasetsLoader:
     """
     DatasetsLoader is a class for loading datasets from Google Cloud Storage (GCS).
     It uses the GCSFileSystem for accessing files and Polars for handling data.
     """
@@ -14,15 +16,15 @@
     def __init__(self, use_cache=True, cache_dir=None):
         self.fs = gcsfs.GCSFileSystem(verify=False)
         self.dataset_hub = DATASET_HUB
         self.use_cache = use_cache
         self.cache_dir = (
             cache_dir
             if cache_dir is not None
-            else os.path.join(os.path.expanduser("~"), ".cache/giza_datasets")
+            else os.path.join(os.path.expanduser("~"), ".cache/giza.datasets")
         )
         self.cache_manager = CacheManager(self.cache_dir) if use_cache else None
 
     def _get_all_parquet_files(self, directory):
         """
         Recursively retrieves all the parquet file paths in the given directory.
```

### Comparing `giza_datasets-0.2.4/giza_datasets/models.py` & `giza_datasets-0.3.0/giza/datasets/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Optional
 
 from pydantic import BaseModel
 
-from giza_datasets.defillama_constants import DEFILLAMA_SUPPORTED_PROJECTS
+from giza.datasets.defillama_constants import DEFILLAMA_SUPPORTED_PROJECTS
 
-sector_tags = ["DeFi","Social"]
+sector_tags = ["DeFi", "Social"]
 application_tags = ["Liquid Staking", "DEX", "Yield", "Lending", "Yield Aggregator"]
 protocol_tags = DEFILLAMA_SUPPORTED_PROJECTS + [
     "Aave-v2",
     "Aave-v3",
     "Compound-v2",
     "Balancer-v1",
     "Balancer-v2",
```

### Comparing `giza_datasets-0.2.4/pyproject.toml` & `giza_datasets-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 [tool.poetry]
 name = "giza-datasets"
-version = "0.2.4"
+version = "0.3.0"
 description = ""
 authors = ["Fran Algaba <f.algaba@outlook.es>"]
 readme = "README.md"
 license = "MIT"
-include = ["datasets/*"]
-
+packages = [{include = "giza"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 polars = "^0"
 gcsfs = "^2023.12.2.post1"
 pydantic = "^2"
 rich = "^13"
```

### Comparing `giza_datasets-0.2.4/PKG-INFO` & `giza_datasets-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-datasets
-Version: 0.2.4
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: Fran Algaba
 Author-email: f.algaba@outlook.es
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -37,15 +37,15 @@
 
 1. Install the `giza-datasets` package if you haven't already:
    ```
    pip install giza-datasets
    ```
 2. Import the `DatasetsLoader` class and initialize it:
    ```python
-   from giza_datasets import DatasetsLoader
+   from giza.datasets import DatasetsLoader
    loader = DatasetsLoader()
    ```
 3. Optional: Depending on your device's configuration, it may be necessary to provide SSL certificates to verify the authenticity of HTTPS connections. You can ensure that all these certifications are correct by executing the following line of code:
    ```python
    import certifi
    import os
    os.environ['SSL_CERT_FILE'] = certifi.where()
@@ -71,15 +71,15 @@
 - `get(dataset_name)`: Returns a Dataset object with the given name.
 - `describe(dataset_name)`: Prints a table of details for the given dataset.
 
 To get started with the `DatasetsHub` class, follow the steps below:
 
 1. Import the `DatasetsHub` class and initialize it:
    ```python
-   from giza_datasets import DatasetsHub
+   from giza.datasets import DatasetsHub
    hub = DatasetsHub()
    ```
 2. Use the `show` method to print a table of all datasets in the hub:
    ```python
    hub.show()
    ```
 3. Use the `list` method to get a list of all datasets in the hub:
```

