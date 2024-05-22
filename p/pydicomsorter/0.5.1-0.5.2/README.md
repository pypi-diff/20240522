# Comparing `tmp/pydicomsorter-0.5.1.tar.gz` & `tmp/pydicomsorter-0.5.2.tar.gz`

## Comparing `pydicomsorter-0.5.1.tar` & `pydicomsorter-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/pixi.lock
--rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/releaserc.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/ruff.toml
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/index.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/README.md
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/pixi.lock
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/releaserc.toml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/ruff.toml
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/index.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/README.md
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/PKG-INFO
```

### Comparing `pydicomsorter-0.5.1/pixi.lock` & `pydicomsorter-0.5.2/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3974,40 +3974,40 @@
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282275
   timestamp: 1713905769522
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
+  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
-  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
+  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
+  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.2
   build: py312h2615798_0
@@ -4104,17 +4104,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.5.1
+  version: 0.5.2
   path: .
-  sha256: 0c0adf531580037c43b03bb82b4f051852893b937dd0927fa0eea7d020b32b33
+  sha256: 895c029e497081ad4d891d861a033458e33dcdeab47704f7f8dbceb5bcb1a1d7
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.5.1/.github/workflows/main.yaml` & `pydicomsorter-0.5.2/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/config/mkdocs.yaml` & `pydicomsorter-0.5.2/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/config/releaserc.toml` & `pydicomsorter-0.5.2/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/config/ruff.toml` & `pydicomsorter-0.5.2/config/ruff.toml`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 "tests/*" = ["S101"]
 
 [lint.mccabe]
 max-complexity = 10
 
 [lint.isort]
 known-first-party = ["pydicomsorter"]
+force-wrap-aliases = true
+combine-as-imports = true
+lines-after-imports = 1
+relative-imports-order = "closest-to-furthest"
 
 [lint.pydocstyle]
 convention = "google"
 
 [format]
 quote-style = "single"
 docstring-code-format = true
```

### Comparing `pydicomsorter-0.5.1/docs/CHANGELOG.md` & `pydicomsorter-0.5.2/docs/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v0.5.2 (2024-05-21)
+
+### Fix
+
+* fix: add linting options ([`122cca1`](https://github.com/jjjermiah/PyDicomSorter/commit/122cca187f10d95aceb439be4ff3305e6f187d85))
+
+
 ## v0.5.1 (2024-05-21)
 
 ### Chore
 
 * chore: Update pre-commit configuration to include src/.*\.py$ files ([`74082dc`](https://github.com/jjjermiah/PyDicomSorter/commit/74082dc9bcdbed0813da6f14f056a29dbbd0421b))
 
 * chore: Update dependencies and add DICOMSorter class ([`640f409`](https://github.com/jjjermiah/PyDicomSorter/commit/640f409859c60bc3bd5294b09a660a8057360198))
```

### Comparing `pydicomsorter-0.5.1/docs/about.md` & `pydicomsorter-0.5.2/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/src/pydicomsorter/parser.py` & `pydicomsorter-0.5.2/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.5.2/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.5.2/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.5.2/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/tests/test_parser.py` & `pydicomsorter-0.5.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/.gitignore` & `pydicomsorter-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/LICENSE` & `pydicomsorter-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/README.md` & `pydicomsorter-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.1/pyproject.toml` & `pydicomsorter-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.5.1"
+version = "0.5.2"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.5.1/PKG-INFO` & `pydicomsorter-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.5.1
+Version: 0.5.2
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

