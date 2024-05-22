# Comparing `tmp/transcoders_slim-0.2.0.tar.gz` & `tmp/transcoders_slim-0.2.1.tar.gz`

## Comparing `transcoders_slim-0.2.0.tar` & `transcoders_slim-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0   161756 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/pdm.lock
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.github/workflows/tests.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/docs/setup.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/test_init.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/tests/test_load_pretrained.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/__init__.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/load_pretrained.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/transcoder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/__init__.py
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/config.py
--rw-r--r--   0        0        0    28830 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/transcoders_slim/sae_training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/.gitignore
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/README.md
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 transcoders_slim-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0   161756 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/pdm.lock
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/.github/workflows/tests.yaml
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/docs/setup.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/tests/test_init.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/tests/test_load_pretrained.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/__init__.py
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/load_pretrained.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/transcoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/sae_training/__init__.py
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/sae_training/config.py
+-rw-r--r--   0        0        0    28830 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/transcoders_slim/sae_training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/README.md
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 transcoders_slim-0.2.1/PKG-INFO
```

### Comparing `transcoders_slim-0.2.0/CHANGELOG.md` & `transcoders_slim-0.2.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.2.1 (2024-05-17)
+
+### Fix
+
+* fix: relax tlens, einops versions ([`ab3da53`](https://github.com/dtch1997/transcoders-slim/commit/ab3da538519127a47e0bdad91e87808ff3ade756))
+
+
 ## v0.2.0 (2024-05-12)
 
 ### Feature
 
 * feat: bump version ([`1c5da65`](https://github.com/dtch1997/transcoders-slim/commit/1c5da65a8d542b313c2f360b6f09262a35db3479))
```

### Comparing `transcoders_slim-0.2.0/pdm.lock` & `transcoders_slim-0.2.1/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is @generated by PDM.
 # It is not intended for manual editing.
 
 [metadata]
 groups = ["default", "test"]
 strategy = ["cross_platform", "inherit_metadata"]
 lock_version = "4.4.1"
-content_hash = "sha256:58e4698f3647a8f1ad33ab4f7f7e5edb0e2d98e779cc9f9dc8f7f73c3ec15771"
+content_hash = "sha256:65a9381eef49bb9788eeb53463d5e6032d40460bd097c6963cba252dcabbe611"
 
 [[package]]
 name = "accelerate"
 version = "0.30.1"
 requires_python = ">=3.8.0"
 summary = "Accelerate"
 groups = ["default"]
```

### Comparing `transcoders_slim-0.2.0/.github/workflows/release.yaml` & `transcoders_slim-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/.github/workflows/tests.yaml` & `transcoders_slim-0.2.1/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/tests/test_load_pretrained.py` & `transcoders_slim-0.2.1/tests/test_load_pretrained.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/transcoders_slim/load_pretrained.py` & `transcoders_slim-0.2.1/transcoders_slim/load_pretrained.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/transcoders_slim/sae_training/config.py` & `transcoders_slim-0.2.1/transcoders_slim/sae_training/config.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/transcoders_slim/sae_training/sparse_autoencoder.py` & `transcoders_slim-0.2.1/transcoders_slim/sae_training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/.gitignore` & `transcoders_slim-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/README.md` & `transcoders_slim-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `transcoders_slim-0.2.0/pyproject.toml` & `transcoders_slim-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "transcoders-slim"
-version = "0.2.0"
+version = "0.2.1"
 description = "A template for python projects in PDM"
 authors = [
     { name = "Daniel Tan", email = "dtch1997@users.noreply.github.com" },
     { name = "Daniel CH Tan", email = "dtch1997@users.noreply.github.com" },
 ]
 dependencies = [
     "huggingface-hub>=0.23.0",
     "torch>=2.3.0",
     "transformer-lens>=1.14.0",
-    "einops>=0.7.0",
+    "einops>=0.6.0",
     "jaxtyping>=0.2.28",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = { text = "MIT" }
 
 [project.optional-dependencies]
```

### Comparing `transcoders_slim-0.2.0/PKG-INFO` & `transcoders_slim-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: transcoders-slim
-Version: 0.2.0
+Version: 0.2.1
 Summary: A template for python projects in PDM
 Author-email: Daniel Tan <dtch1997@users.noreply.github.com>, Daniel CH Tan <dtch1997@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.10
-Requires-Dist: einops>=0.7.0
+Requires-Dist: einops>=0.6.0
 Requires-Dist: huggingface-hub>=0.23.0
 Requires-Dist: jaxtyping>=0.2.28
 Requires-Dist: torch>=2.3.0
 Requires-Dist: transformer-lens>=1.14.0
 Provides-Extra: test
 Requires-Dist: pre-commit>=3.7.0; extra == 'test'
 Requires-Dist: pyright>=1.1.361; extra == 'test'
```

