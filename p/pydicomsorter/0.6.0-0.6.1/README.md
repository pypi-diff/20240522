# Comparing `tmp/pydicomsorter-0.6.0.tar.gz` & `tmp/pydicomsorter-0.6.1.tar.gz`

## Comparing `pydicomsorter-0.6.0.tar` & `pydicomsorter-0.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/releaserc.toml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/config/ruff.toml
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/docs/index.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/main.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/README.md
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/releaserc.toml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/ruff.toml
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/index.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/README.md
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/PKG-INFO
```

### Comparing `pydicomsorter-0.6.0/.pre-commit-config.yaml` & `pydicomsorter-0.6.1/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: local
     hooks:
       - id: pixi-install
         name: Run pixi install
-        entry: bash -c 'pixi install & pixi install -e dev & pixi install -e publish'
+        entry: bash -c 'pixi install && pixi install -e dev && pixi install -e publish'
         language: system
         files: ^src/.*\.py$|^pyproject\.toml$|^pixi\.lock$
       - id: pixi-run-tests
         name: Run pixi tests
         entry: bash -c 'pixi run test'
         language: system
         files: ^src/.*\.py$|^pyproject\.toml$
```

### Comparing `pydicomsorter-0.6.0/pixi.lock` & `pydicomsorter-0.6.1/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3990,24 +3990,24 @@
   sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
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
+  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
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
-  version: 0.6.0
+  version: 0.6.1
   path: .
-  sha256: 9ff8d3dbbb2245af03f10dca84f34a29408e118c706dedabca888d2767ae2cb4
+  sha256: c24df5e40b7201804870cc0343a4a76596da92c8532c671c68fa5c2eb867b703
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.6.0/.github/workflows/main.yaml` & `pydicomsorter-0.6.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/config/mkdocs.yaml` & `pydicomsorter-0.6.1/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/config/releaserc.toml` & `pydicomsorter-0.6.1/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/config/ruff.toml` & `pydicomsorter-0.6.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/docs/CHANGELOG.md` & `pydicomsorter-0.6.1/docs/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v0.6.1 (2024-05-22)
+
+### Fix
+
+* fix: lock ([`3bb9612`](https://github.com/jjjermiah/PyDicomSorter/commit/3bb96126c40d70b82bbffcbd5b3d1a9f12d0c533))
+
+* fix: lock ([`9603cac`](https://github.com/jjjermiah/PyDicomSorter/commit/9603cac4749df2bb5a6809961556adb879e8c3a7))
+
+* fix: lock ([`503ad7a`](https://github.com/jjjermiah/PyDicomSorter/commit/503ad7ac8e66eb748c61eaef56a2c8e7d83634db))
+
+* fix: some formatting ([`59d3f28`](https://github.com/jjjermiah/PyDicomSorter/commit/59d3f2882f95dc3dad21e42abff71f31db20a0cc))
+
+
 ## v0.6.0 (2024-05-22)
 
 ### Chore
 
 * chore: Update pydantic-core to version 2.18.2 ([`3934df3`](https://github.com/jjjermiah/PyDicomSorter/commit/3934df3bbef2fefde3c704b01f1d73cf8418464e))
 
 ### Ci
```

### Comparing `pydicomsorter-0.6.0/docs/about.md` & `pydicomsorter-0.6.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.6.1/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.6.1/src/pydicomsorter/tags4format.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,37 +30,33 @@
 
 
 all_dicom_tags: list[str] = [
     item for key, value in DicomDictionary.items() for item in (value[2], value[4])
 ]
 
 
-def build_tree(
-    tree: ttk.Treeview, ds: pydicom.Dataset, parent: str | None = None
-) -> None:
+def build_tree(tree: ttk.Treeview, ds: pydicom.Dataset, parent: str | None = None) -> None:
     """Build out the tree.
 
     Parameters
     ----------
     tree : ttk.Treeview
         The treeview object.
     ds : pydicom.dataset.Dataset
         The dataset object to add to the `tree`.
     parent : str | None
         The item ID of the parent item in the tree (if any), default ``None``.
     """
     # For each DataElement in the current Dataset
     for idx, elem in enumerate(ds):
-        tree_item = tree.insert("", tk.END, text=str(elem))
+        tree_item = tree.insert('', tk.END, text=str(elem))
         if parent:
             tree.move(tree_item, parent, idx)
 
-        if elem.VR == "SQ":
+        if elem.VR == 'SQ':
             # DataElement is a sequence, containing 0 or more Datasets
             for seq_idx, seq_item in enumerate(elem.value):
-                tree_seq_item = tree.insert(
-                    "", tk.END, text=f"{elem.name} Item {seq_idx + 1}"
-                )
+                tree_seq_item = tree.insert('', tk.END, text=f'{elem.name} Item {seq_idx + 1}')
                 tree.move(tree_seq_item, tree_item, seq_idx)
 
                 # Recurse into the sequence item(s)
                 build_tree(tree, seq_item, tree_seq_item)
```

### Comparing `pydicomsorter-0.6.0/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.6.1/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         )
         print_dicom_path_tree(self.new_format, self.tree)
 
     def validate_keys(self) -> None:
         """Validate the keys."""
         invalid_keys: list[str] = self.invalid_keys()
         for key in invalid_keys:
-            self.console.print(f"Invalid key:UID- {key}")
+            self.console.print(f"Invalid key:{key}")
             closest_match = difflib.get_close_matches(key, all_dicom_tags, 3, 0.4)
             if closest_match:
                 self.console.print("Closest matches:")
                 [
                     self.console.print(f"\t[bold cyan]{match}[/bold cyan]")
                     for match in closest_match
                 ]
@@ -119,13 +119,13 @@
         """Rich output."""
         # return the tree as a rich object
         return self.tree
 
 
 if "__main__" == __name__:
     options = DICOMSorterOptions(
-        targetPattern="/COLLECTION_ID/%PatientID/%StudyID/{Modality}-{SeriesInstanceUID}/%InstanceNumber.dcm",
+        targetPattern="/COLLECTION_ID/%PatientID/%StudyID/{Modalixty}-{SeriesInstanceUID}/%InstanceNumber.dcm",
     )
     sorter = DICOMSorter(options)
     sorter.validate_keys()
     print(f"All DICOM tags: {sorter.keys}")
     print(sorter)
```

### Comparing `pydicomsorter-0.6.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.6.1/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/tests/test_parser.py` & `pydicomsorter-0.6.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/.gitignore` & `pydicomsorter-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/LICENSE` & `pydicomsorter-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/README.md` & `pydicomsorter-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.0/pyproject.toml` & `pydicomsorter-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.6.0"
+version = "0.6.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.6.0/PKG-INFO` & `pydicomsorter-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

