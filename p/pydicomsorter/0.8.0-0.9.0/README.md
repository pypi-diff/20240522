# Comparing `tmp/pydicomsorter-0.8.0.tar.gz` & `tmp/pydicomsorter-0.9.0.tar.gz`

## Comparing `pydicomsorter-0.8.0.tar` & `pydicomsorter-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/releaserc.toml
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/config/ruff.toml
--rw-r--r--   0        0        0     6450 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/docs/index.md
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/cli.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/dicomsort.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/tests/test_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/LICENSE
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/README.md
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pydicomsorter-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/config/ruff.toml
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/cli.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/dicomsort.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     3847 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/tests/test_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/README.md
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2562 2020-02-02 00:00:00.000000 pydicomsorter-0.9.0/PKG-INFO
```

### Comparing `pydicomsorter-0.8.0/.pre-commit-config.yaml` & `pydicomsorter-0.9.0/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
       - id: pretty-format-json
   - repo: local
     hooks:
       - id: pixi-install
         name: Run pixi install
         entry: bash -c 'pixi install --all && git add pixi.lock'
         language: system
-        files: ^src/.*\.py$|^pyproject\.toml$|^pixi\.lock$
+        files: ^src/pydicomsorter/.*\.py$|^pyproject\.toml$|^pixi\.lock$
       # - id: pixi-run-tests
       #   name: Run pixi tests
       #   entry: bash -c 'pixi run test'
       #   language: system
       #   files: ^src/.*\.py$|^pyproject\.toml$
       - id: pixi-run-lint
         name: Run pixi lint
```

### Comparing `pydicomsorter-0.8.0/pixi.lock` & `pydicomsorter-0.9.0/pixi.lock`

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
+  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
-  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
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
-  version: 0.8.0
+  version: 0.9.0
   path: .
-  sha256: 5c89e7d04587084e955119712fe123292ece4cc93c8556c1e7f156f5a1fc3582
+  sha256: dd3f41cc50e1ee2292b9acd5c46633dde72ffc007b02dd98da0918d011ad4926
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
```

### Comparing `pydicomsorter-0.8.0/.github/workflows/main.yaml` & `pydicomsorter-0.9.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/config/mkdocs.yaml` & `pydicomsorter-0.9.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/config/releaserc.toml` & `pydicomsorter-0.9.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/config/ruff.toml` & `pydicomsorter-0.9.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/docs/CHANGELOG.md` & `pydicomsorter-0.9.0/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 # CHANGELOG
 
 
 
+## v0.9.0 (2024-05-22)
+
+### Feature
+
+* feat: functioning cli ([`69e5d57`](https://github.com/jjjermiah/PyDicomSorter/commit/69e5d57da188b1161197a040d04477ebb278eeba))
+
+### Fix
+
+* fix: lock ([`ffe0bac`](https://github.com/jjjermiah/PyDicomSorter/commit/ffe0bacd6090a683b20b3b271f9149784b7f5bda))
+
+
 ## v0.8.0 (2024-05-22)
 
 ### Feature
 
 * feat: add basic cli ([`40fb02b`](https://github.com/jjjermiah/PyDicomSorter/commit/40fb02bebf887223c7436ec3d3eb0319ca7c2397))
 
 ### Fix
```

### Comparing `pydicomsorter-0.8.0/docs/about.md` & `pydicomsorter-0.9.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/cli.py` & `pydicomsorter-0.9.0/src/pydicomsorter/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 """Main module of the package."""
 
 import pathlib
 
 import rich_click as click
+from rich import print
 
 from pydicomsorter.dicomsort import DICOMSorter
+from pydicomsorter.io import find_dicom_files
 
 click.rich_click.OPTION_GROUPS = {
-    'dicomsort': [
+    "dicomsort": [
         {
-            'name': 'Advanced options',
-            'options': ['--delete_source', '--keep_going', '--symlink', '--dry_run'],
+            "name": "Advanced options",
+            "options": ["--delete_source", "--keep_going", "--symlink", "--dry_run"],
         },
         {
-            'name': 'Basic options',
-            'options': ['--verbose', '--debug', '--help'],
+            "name": "Basic options",
+            "options": ["--verbose", "--debug", "--help"],
         },
     ]
 }
 
 
-@click.command(context_settings={'help_option_names': ['-h', '--help']})
+@click.command(context_settings={"help_option_names": ["-h", "--help"]})
 @click.argument(
-    'sourcedir',
+    "sourcedir",
     type=click.Path(
         exists=True,
         path_type=pathlib.Path,
         resolve_path=True,
         file_okay=False,
     ),
 )
 @click.argument(
-    'destination_dir',
+    "destination_dir",
     type=str,
 )
 @click.option(
-    '-d',
-    '--delete_source',
+    "-d",
+    "--delete_source",
     is_flag=True,
-    help='Delete the source files after sorting.',
+    help="Delete the source files after sorting.",
 )
 @click.option(
-    '-k',
-    '--keep_going',
+    "-k",
+    "--keep_going",
     is_flag=True,
-    help='Keep going when an error occurs.',
+    help="Keep going when an error occurs.",
 )
 @click.option(
-    '-s',
-    '--symlink',
+    "-s",
+    "--symlink",
     is_flag=True,
-    help='Create symbolic links instead of moving files.',
+    help="Create symbolic links instead of moving files.",
 )
 @click.option(
-    '-n',
-    '--dry_run',
+    "-n",
+    "--dry_run",
     is_flag=True,
-    help='Do not move or copy files, just print what would be done.',
+    help="Do not move or copy files, just print what would be done.",
 )
 @click.option(
-    '--verbose',
+    "--verbose",
     is_flag=True,
-    help='Print verbose output.',
+    help="Print verbose output.",
 )
 @click.option(
-    '--debug',
+    "--debug",
     is_flag=True,
-    help='Print debug output.',
+    help="Print debug output.",
 )
 def main(
     sourcedir: pathlib.Path,
     destination_dir: str,
     delete_source: bool,
     keep_going: bool,
     symlink: bool,
@@ -78,8 +80,44 @@
     verbose: bool,
     debug: bool,
 ) -> None:
     """Main function of the package.
 
     pixi run dicomsort data data/test/%PatientID/%StudyInstanceUID-%Modality/%InstanceNumber.dcm
     """
-    DICOMSorter(destination_dir=destination_dir).validate_keys()
+    import asyncio
+
+    asyncio.run(
+        _main(
+            sourcedir,
+            destination_dir,
+            delete_source,
+            keep_going,
+            symlink,
+            dry_run,
+            verbose,
+            debug,
+        )
+    )
+
+
+async def _main(
+    sourcedir: pathlib.Path,
+    destination_dir: str,
+    delete_source: bool,
+    keep_going: bool,
+    symlink: bool,
+    dry_run: bool,
+    verbose: bool,
+    debug: bool,
+) -> None:
+    """Main function of the package.
+
+    pixi run dicomsort data data/test/%PatientID/%StudyInstanceUID-%Modality/%InstanceNumber.dcm
+    """
+    # run find_dicom_files asynchronously
+    files = await find_dicom_files(sourcedir)
+    print(f"Found {len(files)} DICOM files.")
+    # other code here
+    sorter = DICOMSorter(destination_dir=destination_dir).validate_keys()
+
+    print(f"Keys to use: {sorter.keys}")
```

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/dicomsort.py` & `pydicomsorter-0.9.0/src/pydicomsorter/dicomsort.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,25 +15,27 @@
     """Dicomsort class."""
 
     def __init__(self, destination_dir: str) -> None:
         """Initialize the DICOMSorter."""
         self.format, self.keys = PatternParser().parse(destination_dir)
         self.console = Console()
 
-    def validate_keys(self) -> None:
+    def validate_keys(self) -> "DICOMSorter":
         """Validate the keys."""
         invalid_keys: list[str] = self.invalid_keys()
         for key in invalid_keys:
-            self.console.print(f'Invalid key:{key}')
+            self.console.print(f"Invalid key:{key}")
             closest_match = difflib.get_close_matches(key, all_dicom_tags, 3, 0.4)
             if closest_match:
-                self.console.print('Closest matches:')
+                self.console.print("Closest matches:")
                 [
-                    self.console.print(f'\t[bold cyan]{match}[/bold cyan]')
+                    self.console.print(f"\t[bold cyan]{match}[/bold cyan]")
                     for match in closest_match
                 ]
             else:
-                self.console.print('No close match found.')
+                self.console.print("No close match found.")
+
+        return self
 
     def invalid_keys(self) -> list[str]:
         """Validate the keys."""
         return [key for key in self.keys if not tag_exists(keyword=key)]
```

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/io.py` & `pydicomsorter-0.9.0/src/pydicomsorter/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """I/O utilities."""
 
 from pathlib import Path
 
 from pydicom import dcmread
 from pydicom.errors import InvalidDicomError
 
-def find_dicom_files(source_dir: Path) -> list[Path]:
+async def find_dicom_files(source_dir: Path) -> list[Path]:
     """Find all DICOM files in the source directory."""
-    return [file.resolve() for file in source_dir.glob('**/*.dcm') if file.is_file()]
+    return [file.resolve() for file in source_dir.glob("**/*.dcm") if file.is_file()]
 
 
 def read_all(file: Path, tags: list[str]) -> dict[str, str]:
     """Read all tags from the DICOM file."""
     try:
         dicom = dcmread(file, stop_before_pixels=True)
     except TypeError as te:
-        raise TypeError(f'Type error reading DICOM file: {file}') from te
+        raise TypeError(f"Type error reading DICOM file: {file}") from te
     except InvalidDicomError as ide:
-        raise InvalidDicomError(f'Invalid DICOM file: {file}') from ide
+        raise InvalidDicomError(f"Invalid DICOM file: {file}") from ide
     except ValueError as ve:
-        raise ValueError(f'Value error reading DICOM file: {file}') from ve
-    return {tag: str(dicom.get(tag, '')) for tag in tags}
+        raise ValueError(f"Value error reading DICOM file: {file}") from ve
+    return {tag: str(dicom.get(tag, "")) for tag in tags}
 
 
 def read_tags(file: Path, tags: list[str]) -> dict[str, str]:
     """Read the specified tags from the DICOM file."""
     try:
         dicom = dcmread(file, specific_tags=tags, stop_before_pixels=True)
     except TypeError as te:
-        raise TypeError(f'Type error reading DICOM file: {file}') from te
+        raise TypeError(f"Type error reading DICOM file: {file}") from te
     except InvalidDicomError as ide:
-        raise InvalidDicomError(f'Invalid DICOM file: {file}') from ide
+        raise InvalidDicomError(f"Invalid DICOM file: {file}") from ide
     except ValueError as ve:
-        raise ValueError(f'Value error reading DICOM file: {file}') from ve
-    return {tag: str(dicom.get(tag, '')) for tag in tags}
+        raise ValueError(f"Value error reading DICOM file: {file}") from ve
+    return {tag: str(dicom.get(tag, "")) for tag in tags}
```

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/options.py` & `pydicomsorter-0.9.0/src/pydicomsorter/options.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.9.0/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.9.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.9.0/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.9.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/tests/test_parser.py` & `pydicomsorter-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/.gitignore` & `pydicomsorter-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/LICENSE` & `pydicomsorter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/README.md` & `pydicomsorter-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.8.0/pyproject.toml` & `pydicomsorter-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.8.0"
+version = "0.9.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.8.0/PKG-INFO` & `pydicomsorter-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.8.0
+Version: 0.9.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

