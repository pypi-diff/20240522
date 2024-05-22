# Comparing `tmp/rasal-0.0.0.tar.gz` & `tmp/rasal-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasal-0.0.0.tar", last modified: Wed Jan 10 05:35:31 2024, max compression
+gzip compressed data, was "rasal-0.1.0.tar", last modified: Wed May 22 03:48:47 2024, max compression
```

## Comparing `rasal-0.0.0.tar` & `rasal-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,55 @@
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.077070 rasal-0.0.0/
--rw-rw-r--   0 orange    (1000) orange    (1000)       66 2024-01-08 05:21:47.000000 rasal-0.0.0/AUTHORS.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       86 2024-01-08 05:21:47.000000 rasal-0.0.0/CHANGELOG.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)     2309 2024-01-08 05:21:47.000000 rasal-0.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)     1102 2024-01-08 05:21:47.000000 rasal-0.0.0/LICENSE
--rw-rw-r--   0 orange    (1000) orange    (1000)      427 2024-01-08 05:21:47.000000 rasal-0.0.0/MANIFEST.in
--rw-r--r--   0 orange    (1000) orange    (1000)     1988 2024-01-10 05:35:31.073070 rasal-0.0.0/PKG-INFO
--rw-rw-r--   0 orange    (1000) orange    (1000)     2341 2024-01-10 05:28:53.000000 rasal-0.0.0/README.rst
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/ci/
--rwxrwxr-x   0 orange    (1000) orange    (1000)     2867 2024-01-08 05:21:47.000000 rasal-0.0.0/ci/bootstrap.py
--rw-rw-r--   0 orange    (1000) orange    (1000)       72 2024-01-08 05:21:47.000000 rasal-0.0.0/ci/requirements.txt
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.069070 rasal-0.0.0/ci/templates/
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.069070 rasal-0.0.0/ci/templates/.github/
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/ci/templates/.github/workflows/
--rw-rw-r--   0 orange    (1000) orange    (1000)     1965 2024-01-08 05:21:47.000000 rasal-0.0.0/ci/templates/.github/workflows/github-actions.yml
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/docs/
--rw-rw-r--   0 orange    (1000) orange    (1000)       28 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/authors.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       30 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/changelog.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)     1088 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/conf.py
--rw-rw-r--   0 orange    (1000) orange    (1000)       33 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/contributing.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)      244 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/index.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       85 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/installation.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       27 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/readme.rst
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/docs/reference/
--rw-rw-r--   0 orange    (1000) orange    (1000)       57 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/reference/index.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       90 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/reference/rasal.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)       17 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/requirements.txt
--rw-rw-r--   0 orange    (1000) orange    (1000)      109 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/spelling_wordlist.txt
--rw-rw-r--   0 orange    (1000) orange    (1000)       62 2024-01-08 05:21:47.000000 rasal-0.0.0/docs/usage.rst
--rw-rw-r--   0 orange    (1000) orange    (1000)     1193 2024-01-10 05:34:02.000000 rasal-0.0.0/pyproject.toml
--rw-rw-r--   0 orange    (1000) orange    (1000)      770 2024-01-08 05:21:47.000000 rasal-0.0.0/pytest.ini
--rw-rw-r--   0 orange    (1000) orange    (1000)       38 2024-01-10 05:35:31.077070 rasal-0.0.0/setup.cfg
--rwxrwxr-x   0 orange    (1000) orange    (1000)     2661 2024-01-10 05:34:02.000000 rasal-0.0.0/setup.py
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.069070 rasal-0.0.0/src/
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/src/rasal/
--rw-rw-r--   0 orange    (1000) orange    (1000)       22 2024-01-08 05:21:47.000000 rasal-0.0.0/src/rasal/__init__.py
--rw-rw-r--   0 orange    (1000) orange    (1000)      357 2024-01-08 05:21:47.000000 rasal-0.0.0/src/rasal/__main__.py
--rw-rw-r--   0 orange    (1000) orange    (1000)      910 2024-01-08 05:21:47.000000 rasal-0.0.0/src/rasal/cli.py
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/src/rasal.egg-info/
--rw-r--r--   0 orange    (1000) orange    (1000)     1988 2024-01-10 05:35:31.000000 rasal-0.0.0/src/rasal.egg-info/PKG-INFO
--rw-rw-r--   0 orange    (1000) orange    (1000)      721 2024-01-10 05:35:31.000000 rasal-0.0.0/src/rasal.egg-info/SOURCES.txt
--rw-rw-r--   0 orange    (1000) orange    (1000)        1 2024-01-10 05:35:31.000000 rasal-0.0.0/src/rasal.egg-info/dependency_links.txt
--rw-rw-r--   0 orange    (1000) orange    (1000)       41 2024-01-10 05:35:31.000000 rasal-0.0.0/src/rasal.egg-info/entry_points.txt
--rw-rw-r--   0 orange    (1000) orange    (1000)        1 2024-01-10 05:20:58.000000 rasal-0.0.0/src/rasal.egg-info/not-zip-safe
--rw-rw-r--   0 orange    (1000) orange    (1000)        6 2024-01-10 05:35:31.000000 rasal-0.0.0/src/rasal.egg-info/top_level.txt
-drwxrwxr-x   0 orange    (1000) orange    (1000)        0 2024-01-10 05:35:31.073070 rasal-0.0.0/tests/
--rw-rw-r--   0 orange    (1000) orange    (1000)       60 2024-01-08 05:21:47.000000 rasal-0.0.0/tests/test_rasal.py
--rw-rw-r--   0 orange    (1000) orange    (1000)     1670 2024-01-08 05:21:47.000000 rasal-0.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.696619 rasal-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.684619 rasal-0.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.688619 rasal-0.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-05-22 03:48:39.000000 rasal-0.1.0/.github/workflows/github-actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 03:48:39.000000 rasal-0.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 03:48:39.000000 rasal-0.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-22 03:48:39.000000 rasal-0.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-22 03:48:39.000000 rasal-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-22 03:48:39.000000 rasal-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-22 03:48:39.000000 rasal-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-22 03:48:47.696619 rasal-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-22 03:48:39.000000 rasal-0.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.688619 rasal-0.1.0/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2867 2024-05-22 03:48:39.000000 rasal-0.1.0/ci/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-22 03:48:39.000000 rasal-0.1.0/ci/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.684619 rasal-0.1.0/ci/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.684619 rasal-0.1.0/ci/templates/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.688619 rasal-0.1.0/ci/templates/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-22 03:48:39.000000 rasal-0.1.0/ci/templates/.github/workflows/github-actions.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.692619 rasal-0.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.692619 rasal-0.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/reference/rasal.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 03:48:39.000000 rasal-0.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-22 03:48:39.000000 rasal-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-22 03:48:39.000000 rasal-0.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:48:47.696619 rasal-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-22 03:48:39.000000 rasal-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.688619 rasal-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.692619 rasal-0.1.0/src/rasal/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/_lens.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5461 2024-05-22 03:48:39.000000 rasal-0.1.0/src/rasal/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.696619 rasal-0.1.0/src/rasal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 03:48:47.000000 rasal-0.1.0/src/rasal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:48:47.692619 rasal-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-22 03:48:39.000000 rasal-0.1.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-22 03:48:39.000000 rasal-0.1.0/tox.ini
```

### Comparing `rasal-0.0.0/CONTRIBUTING.rst` & `rasal-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rasal-0.0.0/LICENSE` & `rasal-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rasal-0.0.0/PKG-INFO` & `rasal-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: rasal
-Version: 0.0.0
+Version: 0.1.0
 Summary: Resolution and Sensors and Lens.
 Home-page: https://github.com/AidanJohnston/rasal
 Author: Aidan Johnston
 Author-email: contact@aidanjohnston.ca
 License: MIT
-Project-URL: Documentation, https://rasal.readthedocs.io/
+Project-URL: Documentation, https://rasal.readthedocs.io/en/latest
 Project-URL: Changelog, https://rasal.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/AidanJohnston/rasal/issues
+Keywords: resolution,sensorlens
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -22,24 +23,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: test
 
-========
-Overview
-========
-
+=====
+RASAL
+=====
 
 
 Resolution and Sensors and Lens.
 
-* Free software: MIT license
+
 
 Installation
 ============
 
 ::
 
     pip install rasal
@@ -59,32 +60,25 @@
 Development
 ===========
 
 To run all the tests run::
 
     tox
 
-Note, to combine the coverage data from all the tox environments run:
-
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
-
-    - - Windows
-      - ::
-
-            set PYTEST_ADDOPTS=--cov-append
-            tox
+License
+=======
 
-    - - Other
-      - ::
-
-            PYTEST_ADDOPTS=--cov-append tox
+Rasal is under the MIT license. See the LICENSE file for more information.
 
 
 Changelog
 =========
 
+0.1.0 (2024-05-21)
+------------------
+
+* Initial dataclasses for sensor and resolution.
+
 0.0.0 (2024-01-08)
 ------------------
 
 * First release on PyPI.
```

### Comparing `rasal-0.0.0/ci/bootstrap.py` & `rasal-0.1.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `rasal-0.0.0/ci/templates/.github/workflows/github-actions.yml` & `rasal-0.1.0/ci/templates/.github/workflows/github-actions.yml`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             os: '{{ os }}-latest'
 {% endfor %}
 {% endfor %}
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
+        submodules: recursive
     - uses: actions/setup-python@v5
       with:
         python-version: {{ '${{ matrix.python }}' }}
         architecture: {{ '${{ matrix.python_arch }}' }}
     - name: install dependencies
       run: |
         python -mpip install --progress-bar=off -r ci/requirements.txt
```

### Comparing `rasal-0.0.0/docs/conf.py` & `rasal-0.1.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import furo
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.extlinks",
@@ -22,23 +21,19 @@
 pygments_style = "trac"
 templates_path = ["."]
 extlinks = {
     "issue": ("https://github.com/AidanJohnston/rasal/issues/%s", "#"),
     "pr": ("https://github.com/AidanJohnston/rasal/pull/%s", "PR #"),
 }
 html_theme = "furo"
-html_theme_path = [furo.get_html_theme_path()]
 html_theme_options = {
     "githuburl": "https://github.com/AidanJohnston/rasal/",
 }
 
 html_use_smartypants = True
 html_last_updated_fmt = "%b %d, %Y"
 html_split_index = False
-html_sidebars = {
-    "**": ["searchbox.html", "globaltoc.html", "sourcelink.html"],
-}
 html_short_title = f"{project}-{version}"
 
 napoleon_use_ivar = True
 napoleon_use_rtype = False
 napoleon_use_param = False
```

### Comparing `rasal-0.0.0/pytest.ini` & `rasal-0.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `rasal-0.0.0/setup.py` & `rasal-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 #!/usr/bin/env python
 import re
 from pathlib import Path
 
-from setuptools import find_packages
-from setuptools import setup
+from setuptools import find_packages, setup
 
 
 def read(*names, **kwargs):
-    with Path(__file__).parent.joinpath(*names).open(encoding=kwargs.get("encoding", "utf8")) as fh:
+    with Path(__file__).parent.joinpath(*names).open(
+        encoding=kwargs.get("encoding", "utf8")
+    ) as fh:
         return fh.read()
 
 
+__name__ = "rasal"
+__version__ = "0.1.0"
+
+
 setup(
-    name="rasal",
-    version="0.0.0",
+    name=__name__,
+    version=__version__,
+    package_dir={'': 'src'},
+    packages=find_packages(where='src'),
     license="MIT",
     description="Resolution and Sensors and Lens.",
     long_description="{}\n{}".format(
-        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub("", read("README.rst")),
+        re.compile("^.. start-badges.*^.. end-badges", re.M | re.S).sub(
+            "", read("README.rst")
+        ),
         re.sub(":[a-z]+:`~?(.*?)`", r"``\1``", read("CHANGELOG.rst")),
     ),
     author="Aidan Johnston",
     author_email="contact@aidanjohnston.ca",
     url="https://github.com/AidanJohnston/rasal",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    py_modules=[path.stem for path in Path("src").glob("*.py")],
     include_package_data=True,
     zip_safe=False,
     classifiers=[
         # complete classifier list: http://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -39,36 +45,26 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
-        # uncomment if you test on these interpreters:
-        # "Programming Language :: Python :: Implementation :: IronPython",
-        # "Programming Language :: Python :: Implementation :: Jython",
-        # "Programming Language :: Python :: Implementation :: Stackless",
         "Topic :: Utilities",
     ],
     project_urls={
-        "Documentation": "https://rasal.readthedocs.io/",
+        "Documentation": "https://rasal.readthedocs.io/en/latest",
         "Changelog": "https://rasal.readthedocs.io/en/latest/changelog.html",
         "Issue Tracker": "https://github.com/AidanJohnston/rasal/issues",
     },
     keywords=[
-        # eg: "keyword1", "keyword2", "keyword3",
+        "resolution", "sensor" "lens",
     ],
     python_requires=">=3.8",
     install_requires=[
         # eg: "aspectlib==1.1.1", "six>=1.7",
     ],
     extras_require={
-        # eg:
-        #   "rst": ["docutils>=0.11"],
-        #   ":python_version=="2.6"": ["argparse"],
-    },
-    entry_points={
-        "console_scripts": [
-            "rasal = rasal.cli:main",
+        "test": [
         ]
     },
 )
```

### Comparing `rasal-0.0.0/src/rasal.egg-info/PKG-INFO` & `rasal-0.1.0/src/rasal.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: rasal
-Version: 0.0.0
+Version: 0.1.0
 Summary: Resolution and Sensors and Lens.
 Home-page: https://github.com/AidanJohnston/rasal
 Author: Aidan Johnston
 Author-email: contact@aidanjohnston.ca
 License: MIT
-Project-URL: Documentation, https://rasal.readthedocs.io/
+Project-URL: Documentation, https://rasal.readthedocs.io/en/latest
 Project-URL: Changelog, https://rasal.readthedocs.io/en/latest/changelog.html
 Project-URL: Issue Tracker, https://github.com/AidanJohnston/rasal/issues
+Keywords: resolution,sensorlens
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -22,24 +23,24 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE
 License-File: AUTHORS.rst
+Provides-Extra: test
 
-========
-Overview
-========
-
+=====
+RASAL
+=====
 
 
 Resolution and Sensors and Lens.
 
-* Free software: MIT license
+
 
 Installation
 ============
 
 ::
 
     pip install rasal
@@ -59,32 +60,25 @@
 Development
 ===========
 
 To run all the tests run::
 
     tox
 
-Note, to combine the coverage data from all the tox environments run:
-
-.. list-table::
-    :widths: 10 90
-    :stub-columns: 1
-
-    - - Windows
-      - ::
-
-            set PYTEST_ADDOPTS=--cov-append
-            tox
+License
+=======
 
-    - - Other
-      - ::
-
-            PYTEST_ADDOPTS=--cov-append tox
+Rasal is under the MIT license. See the LICENSE file for more information.
 
 
 Changelog
 =========
 
+0.1.0 (2024-05-21)
+------------------
+
+* Initial dataclasses for sensor and resolution.
+
 0.0.0 (2024-01-08)
 ------------------
 
 * First release on PyPI.
```

### Comparing `rasal-0.0.0/src/rasal.egg-info/SOURCES.txt` & `rasal-0.1.0/src/rasal.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+.readthedocs.yaml
 AUTHORS.rst
 CHANGELOG.rst
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 pytest.ini
 setup.py
 tox.ini
+.github/workflows/github-actions.yml
 ci/bootstrap.py
 ci/requirements.txt
 ci/templates/.github/workflows/github-actions.yml
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
@@ -20,16 +22,19 @@
 docs/readme.rst
 docs/requirements.txt
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/index.rst
 docs/reference/rasal.rst
 src/rasal/__init__.py
-src/rasal/__main__.py
-src/rasal/cli.py
+src/rasal/_lens.py
+src/rasal/_resolution.py
+src/rasal/_sensor.py
+src/rasal/_version.py
+src/rasal/units.py
 src/rasal.egg-info/PKG-INFO
 src/rasal.egg-info/SOURCES.txt
 src/rasal.egg-info/dependency_links.txt
-src/rasal.egg-info/entry_points.txt
 src/rasal.egg-info/not-zip-safe
+src/rasal.egg-info/requires.txt
 src/rasal.egg-info/top_level.txt
-tests/test_rasal.py
+tests/test_import.py
```

### Comparing `rasal-0.0.0/tox.ini` & `rasal-0.1.0/tox.ini`

 * *Files 8% similar despite different names*

```diff
@@ -30,37 +30,33 @@
     py312: {env:TOXPYTHON:python3.12}
     {bootstrap,clean,check,report,docs,codecov}: {env:TOXPYTHON:python3}
 setenv =
     PYTHONPATH={toxinidir}/tests
     PYTHONUNBUFFERED=yes
 passenv =
     *
-usedevelop = false
 deps =
     pytest
     pytest-cov
 commands =
     {posargs:pytest --cov --cov-report=term-missing --cov-report=xml -vv tests}
 
 [testenv:check]
 deps =
     docutils
     check-manifest
-    pre-commit
     readme-renderer
     pygments
     isort
-skip_install = true
+    pybind11
 commands =
     python setup.py check --strict --metadata --restructuredtext
     check-manifest .
-    pre-commit run --all-files --show-diff-on-failure
 
 [testenv:docs]
-usedevelop = true
 deps =
     -r{toxinidir}/docs/requirements.txt
 commands =
     sphinx-build {posargs:-E} -b html docs dist/docs
     sphinx-build -b linkcheck docs dist/docs
 
 [testenv:report]
```

