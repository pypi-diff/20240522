# Comparing `tmp/pydicomsorter-0.5.2.tar.gz` & `tmp/pydicomsorter-0.6.0.tar.gz`

## Comparing `pydicomsorter-0.5.2.tar` & `pydicomsorter-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/pixi.lock
--rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/releaserc.toml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/config/ruff.toml
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/docs/index.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/README.md
--rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/ruff.toml
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/index.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/README.md
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/PKG-INFO
```

### Comparing `pydicomsorter-0.5.2/pixi.lock` & `pydicomsorter-0.6.0/pixi.lock`

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
-  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
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
-  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
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
-  version: 0.5.2
+  version: 0.6.0
   path: .
-  sha256: 895c029e497081ad4d891d861a033458e33dcdeab47704f7f8dbceb5bcb1a1d7
+  sha256: 9ff8d3dbbb2245af03f10dca84f34a29408e118c706dedabca888d2767ae2cb4
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.5.2/.github/workflows/main.yaml` & `pydicomsorter-0.6.0/.github/workflows/main.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -15,32 +15,28 @@
   Unit-Tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 15 # Consider increasing timeout
     env:
       PIXI_ENV: "dev"
     strategy:
       matrix:
-        os: [ubuntu-latest]
-        # os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
-        # python-version: ["3.12", "3.11", "3.10"]
+        os: [ubuntu-latest, macos-latest, macos-14, windows-latest]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Install Pixi
         uses: prefix-dev/setup-pixi@v0.7.0
         with:
           environments: ${{ env.PIXI_ENV }}
           pixi-version: v0.22.0
           cache: false
-          # cache-key: pixi-ENV_${{ env.PIXI_ENV }}-
 
       - name: Run pytest
         run: |
-          pixi run which python
           pixi run test
 
       - name: Upload coverage report artifact to be used by Codecov
         # only upload if matrix.os is ubuntu-latest and matrix.python-version is 3.12
         if: matrix.os == 'ubuntu-latest'
         uses: actions/upload-artifact@v2
         with:
```

### Comparing `pydicomsorter-0.5.2/config/mkdocs.yaml` & `pydicomsorter-0.6.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/config/releaserc.toml` & `pydicomsorter-0.6.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/config/ruff.toml` & `pydicomsorter-0.6.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/docs/CHANGELOG.md` & `pydicomsorter-0.6.0/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # CHANGELOG
 
 
 
+## v0.6.0 (2024-05-22)
+
+### Chore
+
+* chore: Update pydantic-core to version 2.18.2 ([`3934df3`](https://github.com/jjjermiah/PyDicomSorter/commit/3934df3bbef2fefde3c704b01f1d73cf8418464e))
+
+### Ci
+
+* ci: test on multiple platforms ([`da7f026`](https://github.com/jjjermiah/PyDicomSorter/commit/da7f0265c92c2970839208a14a483dd62b6964ee))
+
+### Feature
+
+* feat: add precommit ([`74adc48`](https://github.com/jjjermiah/PyDicomSorter/commit/74adc483ce2df8bd06ff3fc34f9fccfa584c80d7))
+
+* feat: add precommit ([`2e4ad2c`](https://github.com/jjjermiah/PyDicomSorter/commit/2e4ad2cead4ae1b806d38a8e3b7dc90e1245ad49))
+
+* feat: add precommit ([`58eee66`](https://github.com/jjjermiah/PyDicomSorter/commit/58eee66e1c67fcc111a01dd6b9d57330d5c634c1))
+
+
 ## v0.5.2 (2024-05-21)
 
 ### Fix
 
 * fix: add linting options ([`122cca1`](https://github.com/jjjermiah/PyDicomSorter/commit/122cca187f10d95aceb439be4ff3305e6f187d85))
```

### Comparing `pydicomsorter-0.5.2/docs/about.md` & `pydicomsorter-0.6.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/src/pydicomsorter/parser.py` & `pydicomsorter-0.6.0/src/pydicomsorter/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module contains functions for parsing DICOM keys from a target pattern."""
 
 import re
 from typing import List, Match, Pattern, Tuple
 
-
 # A custom exception to throw when a pattern is valid but there arent any % or {} in it
 class NoPlaceholdersError(Exception):
     """Custom exception to throw when a pattern is valid but there arent any % or {} in it."""
 
     def __init__(self, message: str = 'No placeholders found in the target pattern.') -> None:
         """Initialize the NoPlaceholdersError.
```

### Comparing `pydicomsorter-0.5.2/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.6.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.6.0/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,20 +81,19 @@
         )
 
         # make all keys in the string within
         replacements = dict(
             zip(self.keys, ["{{{0}}}".format(key) for key in self.keys])
         )
         self.new_format = self.format % replacements
-        tree = Tree(
+        self.tree = Tree(
             ":file_folder: BASE_DIR",
             guide_style="bold bright_blue",
         )
-        print_dicom_path_tree(self.new_format, tree)
-        print(tree)
+        print_dicom_path_tree(self.new_format, self.tree)
 
     def validate_keys(self) -> None:
         """Validate the keys."""
         invalid_keys: list[str] = self.invalid_keys()
         for key in invalid_keys:
             self.console.print(f"Invalid key:UID- {key}")
             closest_match = difflib.get_close_matches(key, all_dicom_tags, 3, 0.4)
@@ -112,22 +111,21 @@
         self.console.print(f"Format: {self.format}")
         self.console.print(f"Keys: {self.keys}")
 
     def invalid_keys(self) -> list[str]:
         """Validate the keys."""
         return [key for key in self.keys if not tag_exists(keyword=key)]
 
-    def __rich__(self) -> Text:
+    def __rich__(self) -> Tree:
         """Rich output."""
-        return Text.assemble(
-            f"Target Pattern: {self.options.targetPattern}\n",
-            f"Format: {self.format}\n",
-            f"Keys: {self.keys}\n",
-        )
+        # return the tree as a rich object
+        return self.tree
 
 
 if "__main__" == __name__:
     options = DICOMSorterOptions(
-        targetPattern="/COLLECTION_ID/%PatientID/%StudyID/{SeriesInstanceUID}",
+        targetPattern="/COLLECTION_ID/%PatientID/%StudyID/{Modality}-{SeriesInstanceUID}/%InstanceNumber.dcm",
     )
     sorter = DICOMSorter(options)
     sorter.validate_keys()
+    print(f"All DICOM tags: {sorter.keys}")
+    print(sorter)
```

### Comparing `pydicomsorter-0.5.2/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.6.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/tests/test_parser.py` & `pydicomsorter-0.6.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/.gitignore` & `pydicomsorter-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/LICENSE` & `pydicomsorter-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/README.md` & `pydicomsorter-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.2/pyproject.toml` & `pydicomsorter-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.5.2"
+version = "0.6.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -21,14 +21,15 @@
 documentation = "https://jjjermiah.github.io/pydicomsorter/"
 changelog = "https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md"
 issues = "https://github.com/jjjermiah/pydicomsorter/issues"
 
 [project.scripts]
 myscript = "pydicomsorter.main:main"
 
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 #--------------------------------------------------------------------------------------------------#
 ############################################## PIXI ################################################
 #__________________________________________________________________________________________________#
```

### Comparing `pydicomsorter-0.5.2/PKG-INFO` & `pydicomsorter-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

