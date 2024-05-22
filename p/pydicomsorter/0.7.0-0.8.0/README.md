# Comparing `tmp/pydicomsorter-0.7.0.tar.gz` & `tmp/pydicomsorter-0.8.0.tar.gz`

## Comparing `pydicomsorter-0.7.0.tar` & `pydicomsorter-0.8.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/releaserc.toml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/ruff.toml
--rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/index.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/main.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort 2.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/README.md
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/ruff.toml
+-rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/index.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/cli.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/dicomsort.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/tests/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/README.md
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/PKG-INFO
```

### Comparing `pydicomsorter-0.7.0/pixi.lock` & `pydicomsorter-0.8.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -4104,17 +4104,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.7.0
+  version: 0.8.0
   path: .
-  sha256: 278573a875fae65ff58c04bf48067e51b64bc85484d47ff9ecf896b7e4289bd4
+  sha256: 5c89e7d04587084e955119712fe123292ece4cc93c8556c1e7f156f5a1fc3582
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.7.0/.github/workflows/main.yaml` & `pydicomsorter-0.8.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/config/mkdocs.yaml` & `pydicomsorter-0.8.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/config/releaserc.toml` & `pydicomsorter-0.8.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/config/ruff.toml` & `pydicomsorter-0.8.0/config/ruff.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 target-version = "py39"
 output-format = "full"
 line-length = 99
 fix = true
 
 # extend-exclude is used to exclude directories from the flake8 checks
-extend-exclude = ["docs/*", "tests/*", ".pixi/", "src/**/sandbox/*"]
+extend-exclude = ["docs/*", "tests/*", ".pixi/", "src/**/sandbox/*.py"]
 
 extend-include = []
 
 [lint]
 select = [
   "E",
   "F",
```

### Comparing `pydicomsorter-0.7.0/docs/CHANGELOG.md` & `pydicomsorter-0.8.0/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.8.0 (2024-05-22)
+
+### Feature
+
+* feat: add basic cli ([`40fb02b`](https://github.com/jjjermiah/PyDicomSorter/commit/40fb02bebf887223c7436ec3d3eb0319ca7c2397))
+
+### Fix
+
+* fix: lint and format ([`1e8269b`](https://github.com/jjjermiah/PyDicomSorter/commit/1e8269b69f6513adabb90841c5ce2823ddeeb6b9))
+
+
 ## v0.7.0 (2024-05-22)
 
 ### Feature
 
 * feat: add pixi lock durin gpre-commit ([`a987074`](https://github.com/jjjermiah/PyDicomSorter/commit/a98707490ebd7d5beca515e0ddd8ec56cf223d13))
 
 ### Fix
```

### Comparing `pydicomsorter-0.7.0/docs/about.md` & `pydicomsorter-0.8.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/src/pydicomsorter/options.py` & `pydicomsorter-0.8.0/src/pydicomsorter/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 ALL_TAGS: Final[list[str]] = [value[4] for _, value in DicomDictionary.items()]
 
 
 class DICOMSorterOptions(BaseModel):
     """A Pydantic model for the DICOMSorter options."""
 
-    target_pattern: str = "%PatientID/%StudyID-{SeriesID}"
+    target_pattern: str = '%PatientID/%StudyID-{SeriesID}'
     delete_source: bool = False
     symlink: bool = False
     keep_going: bool = False
     dry_run: bool = False
     verbose: bool = False
 
 
 # dataclass describing DICOMSorter options
 class DicomKeyHighlighter(RegexHighlighter):
     """Highlight DICOM keys."""
 
-    base_style = "example."
+    base_style = 'example.'
     # i.e in "%(PatientID)s" should highlight "PatientID"
     highlights: ClassVar[list[str]] = [
-        r"%\((?P<DicomTag>[a-zA-Z0-9_]+)\)s",
+        r'%\((?P<DicomTag>[a-zA-Z0-9_]+)\)s',
     ]
```

### Comparing `pydicomsorter-0.7.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.8.0/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.8.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort 2.py` & `pydicomsorter-0.8.0/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Dicomsort functionality."""
 
 import difflib
-from pathlib import Path
-from pydicomsorter.io import find_dicom_files
 from pydicomsorter.parser import PatternParser
-from pydicomsorter.tags4format import tag_exists, tag_for_keyword
+from pydicomsorter.tags4format import tag_exists, all_dicom_tags
 
-from pydicom._dicom_dict import DicomDictionary
 
 from rich.console import Console
 from rich.highlighter import RegexHighlighter
 from rich.theme import Theme
 from pydantic import BaseModel
 
 from rich.text import Text
 from rich.tree import Tree
 from rich import print
 
-all_dicom_tags: list[str] = [value[4] for key, value in DicomDictionary.items()]
-
 
 def print_dicom_path_tree(path: str, tree: Tree):  # pragma: no cover
     """Print a tree of the DICOM path."""
     if not path:
         return
     parts = path.split("/")
     if parts[0] in ["", ".", "/"]:
@@ -81,26 +76,25 @@
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
-            self.console.print(f"Invalid key:UID- {key}")
+            self.console.print(f"Invalid key:{key}")
             closest_match = difflib.get_close_matches(key, all_dicom_tags, 3, 0.4)
             if closest_match:
                 self.console.print("Closest matches:")
                 [
                     self.console.print(f"\t[bold cyan]{match}[/bold cyan]")
                     for match in closest_match
                 ]
@@ -112,22 +106,21 @@
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
+        targetPattern="/COLLECTION_ID/%PatientID/%StudyID/{Modalixty}-{SeriesInstanceUID}/%InstanceNumber.dcm",
     )
     sorter = DICOMSorter(options)
     sorter.validate_keys()
+    print(f"All DICOM tags: {sorter.keys}")
+    print(sorter)
```

### Comparing `pydicomsorter-0.7.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.8.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/tests/test_parser.py` & `pydicomsorter-0.8.0/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from pydicomsorter.parser import PatternParser, NoPlaceholdersError
 
 
 @pytest.fixture
 def parser():
     return PatternParser()
-  
+
 @pytest.mark.parametrize(
     "target_pattern, expected_fmt, expected_keys",
     [
         ("%PatientID/%StudyID-{SeriesID}", "%(PatientID)s/%(StudyID)s-%(SeriesID)s", ["PatientID", "StudyID", "SeriesID"]),
         ("{PatientID}/%StudyID-{SeriesID}", "%(PatientID)s/%(StudyID)s-%(SeriesID)s", ["PatientID", "StudyID", "SeriesID"]),
         ("{PatientID}/%StudyID-{SeriesID}", "%(PatientID)s/%(StudyID)s-%(SeriesID)s", ["PatientID", "StudyID", "SeriesID"]),
         ("/%PatientID/%StudyID-{SeriesID}", "/%(PatientID)s/%(StudyID)s-%(SeriesID)s", ["PatientID", "StudyID", "SeriesID"]),
@@ -28,14 +28,14 @@
 def test_parse_none_pattern(parser):
     with pytest.raises(ValueError):
         parser.parse(None)  # type: ignore
 
 def test_NoPlaceholdersError():
     with pytest.raises(NoPlaceholdersError):
         raise NoPlaceholdersError()
-      
+
 def test_NoPlaceholdersError_works(parser):
     with pytest.raises(NoPlaceholdersError):
         parser.parse("No placeholders here!")
 
 if __name__ == "__main__":
-    pytest.main()
+    pytest.main()
```

### Comparing `pydicomsorter-0.7.0/.gitignore` & `pydicomsorter-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.7.0/LICENSE` & `pydicomsorter-0.8.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2024 
+Copyright (c) 2024
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pydicomsorter-0.7.0/README.md` & `pydicomsorter-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 # pydicomsorter
 
-=============================
-
 [![codecov](https://codecov.io/gh/jjjermiah/PyDicomSorter/graph/badge.svg?token=tCcajRIGz9)](https://codecov.io/gh/jjjermiah/PyDicomSorter)
 [![CI-CD](https://github.com/jjjermiah/PyDicomSorter/actions/workflows/main.yaml/badge.svg)](https://github.com/jjjermiah/PyDicomSorter/actions/workflows/main.yaml)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Built with Material for MkDocs](https://img.shields.io/badge/mkdocs--material-gray?logo=materialformkdocs)](https://github.com/squidfunk/mkdocs-material)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
@@ -18,20 +16,20 @@
 
 ``` bash
 
 dicomsort [options] sourceDir destinationDir/<TARGET_PATTERN>
 
 options:
 
-- [-d, --deleteSource] 
+- [-d, --deleteSource]
 - [-k, --keepGoing]
 - [-s, --symlink]
 - [-n, --dryRun]
 - [-v, --verbose]
 
 ```
 
 <!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
 
 [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
 
-[![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io)
+<!-- [![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io) -->
```

### Comparing `pydicomsorter-0.7.0/pyproject.toml` & `pydicomsorter-0.8.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.7.0"
+version = "0.8.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -19,15 +19,15 @@
 homepage = "https://github.com/jjjermiah/pydicomsorter"
 repository = "https://github.com/jjjermiah/pydicomsorter"
 documentation = "https://jjjermiah.github.io/pydicomsorter/"
 changelog = "https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md"
 issues = "https://github.com/jjjermiah/pydicomsorter/issues"
 
 [project.scripts]
-myscript = "pydicomsorter.main:main"
+dicomsort = "pydicomsorter.cli:main"
 
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 #--------------------------------------------------------------------------------------------------#
@@ -67,14 +67,18 @@
 outputs = ["coverage-report/coverage.xml"]
 
 [tool.pixi.feature.test.tasks.coverage]
 cmd = "coverage report --rcfile=config/coverage.toml"
 inputs = ["coverage-report/coverage.xml", "config/coverage.toml"]
 depends-on = ["test"]
 
+[tool.pixi.feature.test.tasks.validate]
+cmd = "pre-commit run --all-files"
+inputs = ["src/*", "tests/*", "config/*"]
+
 ############################################## STYLE ###############################################
 # See config/ruff.toml for the configuration
 [tool.pixi.feature.style.dependencies]
 ruff = ">=0.4.4"
 pre-commit = ">=3.7.1,<3.8"
 
 [tool.pixi.feature.style.tasks.lint]
```

### Comparing `pydicomsorter-0.7.0/PKG-INFO` & `pydicomsorter-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
@@ -17,16 +17,14 @@
 Requires-Dist: pydicom
 Requires-Dist: rich
 Requires-Dist: rich-click
 Description-Content-Type: text/markdown
 
 # pydicomsorter
 
-=============================
-
 [![codecov](https://codecov.io/gh/jjjermiah/PyDicomSorter/graph/badge.svg?token=tCcajRIGz9)](https://codecov.io/gh/jjjermiah/PyDicomSorter)
 [![CI-CD](https://github.com/jjjermiah/PyDicomSorter/actions/workflows/main.yaml/badge.svg)](https://github.com/jjjermiah/PyDicomSorter/actions/workflows/main.yaml)
 
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Built with Material for MkDocs](https://img.shields.io/badge/mkdocs--material-gray?logo=materialformkdocs)](https://github.com/squidfunk/mkdocs-material)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
@@ -39,20 +37,20 @@
 
 ``` bash
 
 dicomsort [options] sourceDir destinationDir/<TARGET_PATTERN>
 
 options:
 
-- [-d, --deleteSource] 
+- [-d, --deleteSource]
 - [-k, --keepGoing]
 - [-s, --symlink]
 - [-n, --dryRun]
 - [-v, --verbose]
 
 ```
 
 <!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
 
 [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
 
-[![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io)
+<!-- [![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io) -->
```

