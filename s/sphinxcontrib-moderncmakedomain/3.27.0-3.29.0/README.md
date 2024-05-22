# Comparing `tmp/sphinxcontrib_moderncmakedomain-3.27.0.tar.gz` & `tmp/sphinxcontrib_moderncmakedomain-3.29.0.tar.gz`

## Comparing `sphinxcontrib_moderncmakedomain-3.27.0.tar` & `sphinxcontrib_moderncmakedomain-3.29.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/noxfile.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/.github/dependabot.yml
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/sphinxcontrib/moderncmakedomain/__init__.py
--rw-r--r--   0        0        0    27448 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/sphinxcontrib/moderncmakedomain/cmake.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/sphinxcontrib/moderncmakedomain/colors.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/conftest.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/test_basic.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/test_version.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/conf.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/external.rst
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/index.rst
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/local.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/more.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/padding.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/tests/roots/test-root/parallel.rst
--rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/.gitignore
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/LICENSE
--rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/README.md
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/pyproject.toml
--rw-r--r--   0        0        0     6302 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.27.0/PKG-INFO
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/noxfile.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.github/release.yml
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/sphinxcontrib/moderncmakedomain/__init__.py
+-rw-r--r--   0        0        0    27448 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/sphinxcontrib/moderncmakedomain/cmake.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/sphinxcontrib/moderncmakedomain/colors.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/conftest.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/test_basic.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/test_version.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/conf.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/external.rst
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/index.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/local.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/more.rst
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/padding.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/tests/roots/test-root/parallel.rst
+-rw-r--r--   0        0        0     3103 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/.gitignore
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/LICENSE
+-rw-r--r--   0        0        0     5129 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/README.md
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/pyproject.toml
+-rw-r--r--   0        0        0     6390 2020-02-02 00:00:00.000000 sphinxcontrib_moderncmakedomain-3.29.0/PKG-INFO
```

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/noxfile.py` & `sphinxcontrib_moderncmakedomain-3.29.0/noxfile.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-import nox
-import urllib.request
 import re
+import urllib.request
 from pathlib import Path
 
+import nox
+
+nox.needs_version = ">=2024.3.2"
 nox.options.sessions = ["lint", "tests"]
+nox.options.default_venv_backend = "uv|virtualenv"
 
-ALL_PYTHONS = ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
 
 @nox.session
 def lint(session: nox.Session) -> None:
     """
     Run the linter.
     """
     session.install("pre-commit")
@@ -51,15 +53,14 @@
 
     init_file = Path("sphinxcontrib/moderncmakedomain/__init__.py")
     txt = init_file.read_text(encoding="utf_8")
     txt_new = re.sub(r'__version__ = ".*"', f'__version__ = "{version}"', txt)
     init_file.write_text(txt_new, encoding="utf_8")
 
 
-@nox.session(python=ALL_PYTHONS)
+@nox.session
 def tests(session):
     """
     Run the unit and regular tests.
     """
-    # Setuptools is required due to sphinx installing sphinxcontrib extensions that use pkg_resources (fixed upstream but not released yet)
-    session.install(".", "pytest", "setuptools")
+    session.install(".[test]", silent=False)
     session.run("pytest", *session.posargs)
```

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/.github/workflows/cd.yml` & `sphinxcontrib_moderncmakedomain-3.29.0/.github/workflows/cd.yml`

 * *Files 3% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     - published
 
 
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Build SDist and wheel
       run: pipx run build
 
-    - uses: actions/upload-artifact@v3
+    - uses: actions/upload-artifact@v4
       with:
         path: dist/*
 
     - name: Check metadata
       run: pipx run twine check dist/*
 
 
@@ -31,13 +31,13 @@
     environment:
       name: pypi
       url: https://pypi.org/p/sphinxcontrib-moderncmakedomain
     permissions:
       id-token: write
 
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
         name: artifact
         path: dist
 
     - uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/sphinxcontrib/moderncmakedomain/cmake.py` & `sphinxcontrib_moderncmakedomain-3.29.0/sphinxcontrib/moderncmakedomain/cmake.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/sphinxcontrib/moderncmakedomain/colors.py` & `sphinxcontrib_moderncmakedomain-3.29.0/sphinxcontrib/moderncmakedomain/colors.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/tests/test_basic.py` & `sphinxcontrib_moderncmakedomain-3.29.0/tests/test_basic.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 
+
 @pytest.mark.parametrize("parallel", [0, 1, 2])
 @pytest.mark.sphinx(
     "html",
     freshenv=True,
     confoverrides={"html_baseurl": "https://example.org/docs/", "language": "en"},
 )
 def test_simple_html(app, status, warning, parallel):
@@ -15,13 +16,13 @@
 
     with open(str(local_pth), encoding="utf-8") as f:
         local = f.read()
 
     with open(str(external_pth), encoding="utf-8") as f:
         external = f.read()
 
-    print(local)
     assert 'href="#variable:MYVAR"' in local
     assert 'id="variable:MYVAR"' in local
 
-
-
+    assert 'id="index-0-command:find_program"' in external
+    assert "find_program()" in external
+    assert 'class="xref cmake cmake-command docutils literal notranslate"' in external
```

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/.gitignore` & `sphinxcontrib_moderncmakedomain-3.29.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/LICENSE` & `sphinxcontrib_moderncmakedomain-3.29.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/README.md` & `sphinxcontrib_moderncmakedomain-3.29.0/README.md`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_moderncmakedomain-3.27.0/PKG-INFO` & `sphinxcontrib_moderncmakedomain-3.29.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: sphinxcontrib-moderncmakedomain
-Version: 3.27.0
+Version: 3.29.0
 Summary: Sphinx Domain for Modern CMake
 Project-URL: Homepage, https://github.com/scikit-build/moderncmakedomain
 Author: Kitware
 License-File: LICENSE
 Keywords: cmake,documentation,kitware,sphinx,sphinxcontrib
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
+Classifier: Framework :: Sphinx :: Domain
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Documentation
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Requires-Dist: sphinx>=2
 Provides-Extra: test
+Requires-Dist: defusedxml; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Sphinx Domain for Modern CMake
 
 This is taken directly from the Kitware git repository's Utilities directory.
 The original [sphinxcontrib-cmakedomain][] has not been touched in quite some and
```

