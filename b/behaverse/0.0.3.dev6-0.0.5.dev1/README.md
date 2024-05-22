# Comparing `tmp/behaverse-0.0.3.dev6.tar.gz` & `tmp/behaverse-0.0.5.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "behaverse-0.0.3.dev6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "behaverse-0.0.5.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `behaverse-0.0.3.dev6.tar` & `behaverse-0.0.5.dev1.tar`

### file list

```diff
@@ -1,26 +1,33 @@
--rw-r--r--   0        0        0     1759 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/.github/workflows/docs-publish.yml
--rw-r--r--   0        0        0     1243 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      100 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/.gitignore
--rw-r--r--   0        0        0      158 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/.pypirc
--rw-r--r--   0        0        0      375 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/.vscode/settings.json
--rw-r--r--   0        0        0     1071 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/LICENSE
--rw-r--r--   0        0        0      890 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/README.md
--rw-r--r--   0        0        0       54 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/.gitignore
--rw-r--r--   0        0        0       22 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0        0        0      126 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0        0        0     6853 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0        0        0     1392 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/_quarto.yml
--rw-r--r--   0        0        0     1147 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/getting_started.qmd
--rw-r--r--   0        0        0      176 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/docs/index.qmd
--rw-r--r--   0        0        0      209 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/environment.yml
--rw-r--r--   0        0        0     1615 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/pyproject.toml
--rw-r--r--   0        0        0      487 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/__init__.py
--rw-r--r--   0        0        0       27 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/conftest.py
--rw-r--r--   0        0        0     6773 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/dataset.py
--rw-r--r--   0        0        0      238 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/dataset_description.py
--rw-r--r--   0        0        0     1369 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/dataset_test.py
--rw-r--r--   0        0        0     2487 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/functional.py
--rw-r--r--   0        0        0       28 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/functions_test.py
--rw-r--r--   0        0        0     3722 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/utils.py
--rw-r--r--   0        0        0      178 2024-05-07 05:11:19.435291 behaverse-0.0.3.dev6/src/behaverse/utils_test.py
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 behaverse-0.0.3.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1759 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/.github/workflows/docs-publish.yml
+-rw-r--r--   0        0        0     1243 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0      160 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/.gitignore
+-rw-r--r--   0        0        0      158 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/.pypirc
+-rw-r--r--   0        0        0      375 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/.vscode/settings.json
+-rw-r--r--   0        0        0     1071 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/LICENSE
+-rw-r--r--   0        0        0      890 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/README.md
+-rw-r--r--   0        0        0       54 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/.gitignore
+-rw-r--r--   0        0        0       22 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0        0        0      126 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0        0        0     6853 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0        0        0     1392 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/_quarto.yml
+-rw-r--r--   0        0        0     1147 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/getting_started.qmd
+-rw-r--r--   0        0        0      176 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/docs/index.qmd
+-rw-r--r--   0        0        0      209 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/environment.yml
+-rw-r--r--   0        0        0     1724 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/examples/1 Getting Started with Behaverse Data.ipynb
+-rw-r--r--   0        0        0     1788 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0      494 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/src/behaverse/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-22 19:42:36.275062 behaverse-0.0.5.dev1/src/behaverse/additional_storage/huggingface.py
+-rw-r--r--   0        0        0      276 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/additional_storage/osf.py
+-rw-r--r--   0        0        0      278 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/additional_storage/ulhpc.py
+-rw-r--r--   0        0        0      279 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/additional_storage/zenodo.py
+-rw-r--r--   0        0        0       27 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/conftest.py
+-rw-r--r--   0        0        0     7188 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/dataset.py
+-rw-r--r--   0        0        0      238 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/dataset_description.py
+-rw-r--r--   0        0        0     1694 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/dataset_test.py
+-rw-r--r--   0        0        0     1612 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/dvc_storage.py
+-rw-r--r--   0        0        0      535 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/dvc_storage_test.py
+-rw-r--r--   0        0        0     2487 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/functional.py
+-rw-r--r--   0        0        0       28 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/functions_test.py
+-rw-r--r--   0        0        0     2565 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/http_storage.py
+-rw-r--r--   0        0        0     1898 2024-05-22 19:42:36.279062 behaverse-0.0.5.dev1/src/behaverse/utils.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 behaverse-0.0.5.dev1/PKG-INFO
```

### Comparing `behaverse-0.0.3.dev6/.github/workflows/docs-publish.yml` & `behaverse-0.0.5.dev1/.github/workflows/docs-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/.github/workflows/pypi-publish.yml` & `behaverse-0.0.5.dev1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/LICENSE` & `behaverse-0.0.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/README.md` & `behaverse-0.0.5.dev1/README.md`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/docs/_extensions/machow/interlinks/interlinks.lua` & `behaverse-0.0.5.dev1/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/docs/_quarto.yml` & `behaverse-0.0.5.dev1/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/docs/getting_started.qmd` & `behaverse-0.0.5.dev1/docs/getting_started.qmd`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/pyproject.toml` & `behaverse-0.0.5.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,41 @@
 ]
 maintainers = [
     {name = "Morteza Ansarinia", email = "ansarinia@me.com"},
     {name = "Hoorieh Afkari", email = "hoorieh.afkari@uni.lu"},
     {name = "Pedro Cardoso-Leite", email = "pedro.cardosoleite@uni.lu"},
 ]
 readme = "README.md"
+license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 1 - Planning",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.10"
 dynamic = ["version", "description"]
 
+dependencies = [
+    "pandas",
+    "tqdm",
+    "requests"
+]
+
+[project.optional-dependencies]
+dvc = ["dvc>3","dvc-ssh"]
+test = [
+    "pytest"
+]
+
 [project.urls]
 Homepage = "https://behaverse.org"
 Documentation = "https://behaverse.github.io"
 Repository = "https://github.com/behaverse/behaverse"
 
 [tools.flit.module]
 name = "behaverse"
```

### Comparing `behaverse-0.0.3.dev6/src/behaverse/dataset.py` & `behaverse-0.0.5.dev1/src/behaverse/dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Dataset class."""
 
 import re
 from pathlib import Path
 import pandas as pd
 from tqdm.auto import tqdm
 from typing import Any
-from .utils import download_dataset
 from .dataset_description import DatasetDescription
 import logging
 logger = logging.getLogger(__name__)
 
 
 class Dataset():
     """Dataset provides methods to load and describe datasets.
@@ -34,15 +33,15 @@
     def __init__(self, name: str, **kwargs) -> None:
         """Initialize the Dataset class."""
         if not kwargs.get('allow_instantiation', False):
             raise NotImplementedError('You cannot instantiate this class. Use the class methods instead.')
 
         self.name = name
 
-        self.db_path = Path.home() / '.behaverse' / 'datasets' / name
+        self.db_path = Path.home() / '.behaverse' / 'datasets' / self.name
 
         if not self.db_path.exists():
             raise FileNotFoundError(f'Dataset not found: {self.db_path}')
 
         # TODO add dataset-level attributes
         # TODO move time-consuming operations to methods and/or lazy load
         self.description = DatasetDescription()
@@ -149,27 +148,35 @@
         # TODO SECTION option table
         self.option = ...
         # !SECTION option table
 
         return self
 
     @classmethod
-    def open(cls, name: str, download: bool = True) -> 'Dataset':
+    def open(cls, name: str, download: bool = True, storage='http') -> 'Dataset':
         """Open the dataset with the given name, and optionally download it if it does not exist.
 
         Args:
             name: Name of the dataset to open.
             download: whether to download the dataset if it does not exist.
+            storage: storage backend to use (`http` or `dvc`). Defaults to 'http'.
 
         """
         path = Path.home() / '.behaverse' / 'datasets' / name
 
+        match storage:
+            case 'dvc':
+                from .dvc_storage import download_dataset
+            case _:
+                from .http_storage import download_dataset
+
         if not path.exists():
             if not download:
-                raise FileNotFoundError(f'Dataset not found: {path}')
+                raise FileNotFoundError(f'Dataset not found: {path}. '
+                                        'Use `download=True` to download it.')
             download_dataset(name)
 
         return cls(name, allow_instantiation=True)
 
     def describe(self) -> DatasetDescription:
         """Provides metadata and information card for the dataset."""
         return self.description
@@ -188,13 +195,14 @@
 
         Returns:
             bool: True if the dataset is valid, False otherwise.
 
         """
         try:
             path = Path.home() / '.behaverse' / 'datasets' / self.name
-            assert path.exists, f'Path not found: {path.as_posix()}'
+            assert path.exists(), f'Path not found: {path.as_posix()}'
+            assert path.is_dir(), f'Path is not a directory: {path.as_posix()}'
             # TODO add more rules here
             return True
         except AssertionError as e:
             logger.error(e)
             return False
```

### Comparing `behaverse-0.0.3.dev6/src/behaverse/dataset_test.py` & `behaverse-0.0.5.dev1/src/behaverse/dataset_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """Test the dataset module."""
 
 from pathlib import Path
 
 
+def test_list_datasets():
+    """List available datasets."""
+    from .http_storage import list_datasets
+    datasets = list_datasets()
+    print(datasets)
+
+
 def test_download_dataset():
     """Download a behaverse dataset from a public OneDrive link."""
+    # NOTE this commented section is ALT to get one of the available datasets
     # datasets = list_datasets()
-    # url = datasets.query('name == "P500-L1m"')['url'].item()
+    # url = datasets.query('name == "P500_9subjects/L1m"')['url'].item()
     # print(url)
 
-    from .utils import download_dataset
+    from .http_storage import download_dataset
 
-    output = download_dataset('P500-L1m')
+    output = download_dataset('P500_9subjects/L1m')
 
     assert output.exists()
     assert output.is_dir()
     assert len(list(output.iterdir())) > 0
-    assert output == Path.home() / '.behaverse' / 'datasets' / 'P500-L1m'
+    assert output == (Path.home() / '.behaverse' / 'datasets' / 'P500_9subjects' / 'L1m')
 
 
-def test_load_all_dataset():
-    """Load a behaverse dataset."""
+def test_load_full_dataset():
+    """Load all records of a dataset."""
     from .dataset import Dataset
 
-    dataset = Dataset.open('P500-L1m').load()
+    dataset = Dataset.open('P500_9subjects/L1m').load()
 
-    assert dataset.name == 'P500-L1m'
+    assert dataset.name == 'P500_9subjects/L1m'
     assert len(dataset.subjects) > 0
     assert len(dataset.study_flow) > 0
     assert len(dataset.response) > 0
 
 
 def test_load_selected_dataset():
-    """Load a behaverse dataset partially."""
+    """Partially load a behaverse dataset."""
     from .dataset import Dataset
 
     subject_ids = ['001', '002']
 
-    dataset = Dataset.open('P500-L1m').select(subject_id=subject_ids).load()
+    dataset = Dataset.open('P500_9subjects/L1m').select(subject_id=subject_ids).load()
 
-    assert dataset.name == 'P500-L1m'
+    assert dataset.name == 'P500_9subjects/L1m'
     assert len(dataset.subjects) == len(subject_ids)
     assert len(dataset.study_flow.subject_id.unique()) == len(subject_ids)
 
     # FIXME subject_index in response table must be renamed to subject_id
     assert len(dataset.response.subject_index.unique()) == len(subject_ids)
```

### Comparing `behaverse-0.0.3.dev6/src/behaverse/functional.py` & `behaverse-0.0.5.dev1/src/behaverse/functional.py`

 * *Files identical despite different names*

### Comparing `behaverse-0.0.3.dev6/PKG-INFO` & `behaverse-0.0.5.dev1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: behaverse
-Version: 0.0.3.dev6
+Version: 0.0.5.dev1
 Summary: Behaverse Python Package.
 Author-email: xCIT Development Team <contact@xcit.org>
 Maintainer-email: Morteza Ansarinia <ansarinia@me.com>, Hoorieh Afkari <hoorieh.afkari@uni.lu>, Pedro Cardoso-Leite <pedro.cardosoleite@uni.lu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
+Requires-Dist: pandas
+Requires-Dist: tqdm
+Requires-Dist: requests
+Requires-Dist: dvc>3 ; extra == "dvc"
+Requires-Dist: dvc-ssh ; extra == "dvc"
+Requires-Dist: pytest ; extra == "test"
 Project-URL: Documentation, https://behaverse.github.io
 Project-URL: Homepage, https://behaverse.org
 Project-URL: Repository, https://github.com/behaverse/behaverse
+Provides-Extra: dvc
+Provides-Extra: test
 
 # Behaverse Python Package
 
 This package is a Python implementation of the Behaverse API. It allows you to interact with the Behaverse datasets in Python.
 
 ## Installation
```

