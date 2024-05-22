# Comparing `tmp/ss_python-0.0.51.tar.gz` & `tmp/ss_python-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ss_python-0.0.51.tar", last modified: Fri May 17 16:19:32 2024, max compression
+gzip compressed data, was "ss_python-0.0.52.tar", last modified: Wed May 22 00:48:46 2024, max compression
```

## Comparing `ss_python-0.0.51.tar` & `ss_python-0.0.52.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2024-05-17 16:19:15.156701 ss_python-0.0.51/LICENSE
--rw-r--r--   0        0        0     6963 2024-05-17 16:19:15.156701 ss_python-0.0.51/README.md
--rw-r--r--   0        0        0     2602 2024-05-17 16:19:32.800795 ss_python-0.0.51/pyproject.toml
--rw-r--r--   0        0        0       28 2024-05-17 16:19:15.160701 ss_python-0.0.51/src/ss_python/__init__.py
--rw-r--r--   0        0        0      660 2024-05-17 16:19:15.160701 ss_python-0.0.51/src/ss_python/cli.py
--rw-r--r--   0        0        0        0 2024-05-17 16:19:15.160701 ss_python-0.0.51/src/ss_python/py.typed
--rw-r--r--   0        0        0     1055 2024-05-17 16:19:15.160701 ss_python-0.0.51/src/ss_python/settings.py
--rw-r--r--   0        0        0       25 2024-05-17 16:19:15.164701 ss_python-0.0.51/tests/__init__.py
--rw-r--r--   0        0        0      438 2024-05-17 16:19:15.164701 ss_python-0.0.51/tests/cli_test.py
--rw-r--r--   0        0        0      136 2024-05-17 16:19:15.164701 ss_python-0.0.51/tests/pkg_test.py
--rw-r--r--   0        0        0      338 2024-05-17 16:19:15.164701 ss_python-0.0.51/tests/settings_test.py
--rw-r--r--   0        0        0     7977 1970-01-01 00:00:00.000000 ss_python-0.0.51/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-22 00:48:30.265985 ss_python-0.0.52/LICENSE
+-rw-r--r--   0        0        0     7100 2024-05-22 00:48:30.265985 ss_python-0.0.52/README.md
+-rw-r--r--   0        0        0     2581 2024-05-22 00:48:46.637897 ss_python-0.0.52/pyproject.toml
+-rw-r--r--   0        0        0       28 2024-05-22 00:48:30.269985 ss_python-0.0.52/src/ss_python/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-22 00:48:30.269985 ss_python-0.0.52/src/ss_python/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 00:48:30.269985 ss_python-0.0.52/src/ss_python/py.typed
+-rw-r--r--   0        0        0     1055 2024-05-22 00:48:30.269985 ss_python-0.0.52/src/ss_python/settings.py
+-rw-r--r--   0        0        0       25 2024-05-22 00:48:30.273985 ss_python-0.0.52/tests/__init__.py
+-rw-r--r--   0        0        0      438 2024-05-22 00:48:30.273985 ss_python-0.0.52/tests/cli_test.py
+-rw-r--r--   0        0        0      136 2024-05-22 00:48:30.273985 ss_python-0.0.52/tests/pkg_test.py
+-rw-r--r--   0        0        0      338 2024-05-22 00:48:30.273985 ss_python-0.0.52/tests/settings_test.py
+-rw-r--r--   0        0        0     8114 1970-01-01 00:00:00.000000 ss_python-0.0.52/PKG-INFO
```

### Comparing `ss_python-0.0.51/LICENSE` & `ss_python-0.0.52/LICENSE`

 * *Files identical despite different names*

### Comparing `ss_python-0.0.51/README.md` & `ss_python-0.0.52/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [![CI](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml)
 [![CommitLint](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml)
 [![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
 [![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
 [![Renovate](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://serious-scaffold.github.io/ss-python/_static/badges/coverage.json)](https://serious-scaffold.github.io/ss-python/reports/coverage)
+[![Release](https://img.shields.io/github/v/release/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/releases)
 [![PyPI](https://img.shields.io/pypi/v/ss-python)](https://pypi.org/project/ss-python/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ss-python)](https://pypi.org/project/ss-python/)
 [![GitHub](https://img.shields.io/github/license/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/blob/main/LICENSE)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

### Comparing `ss_python-0.0.51/pyproject.toml` & `ss_python-0.0.52/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "full-development-lifecycle",
     "project-template",
     "serious-scaffold",
 ]
 name = "ss-python"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.0.51"
+version = "0.0.52"
 
 [project.license]
 text = "MIT"
 
 [project.scripts]
 ss-python-cli = "ss_python.cli:app"
 
@@ -75,15 +75,14 @@
 
 [tool.pdm.dev-dependencies]
 doc = [
     "Sphinx",
     "autodoc-pydantic",
     "coverage",
     "furo",
-    "git-changelog",
     "mypy[reports]",
     "myst-parser",
     "pytest",
     "sphinx-autobuild",
     "sphinx-click",
     "sphinx-design",
 ]
```

### Comparing `ss_python-0.0.51/src/ss_python/cli.py` & `ss_python-0.0.52/src/ss_python/cli.py`

 * *Files identical despite different names*

### Comparing `ss_python-0.0.51/src/ss_python/settings.py` & `ss_python-0.0.52/src/ss_python/settings.py`

 * *Files identical despite different names*

### Comparing `ss_python-0.0.51/PKG-INFO` & `ss_python-0.0.52/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ss-python
-Version: 0.0.51
+Version: 0.0.52
 Summary: An evolving Python project template that covers the full development lifecycle.
 Keywords: copier-template,full-development-lifecycle,project-template,serious-scaffold
 Author-Email: huxuan <i@huxuan.org>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,14 +27,15 @@
 
 [![CI](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/ci.yml)
 [![CommitLint](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/commitlint.yml)
 [![DevContainer](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/devcontainer.yml)
 [![Release](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/release.yml)
 [![Renovate](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml/badge.svg)](https://github.com/serious-scaffold/ss-python/actions/workflows/renovate.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://serious-scaffold.github.io/ss-python/_static/badges/coverage.json)](https://serious-scaffold.github.io/ss-python/reports/coverage)
+[![Release](https://img.shields.io/github/v/release/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/releases)
 [![PyPI](https://img.shields.io/pypi/v/ss-python)](https://pypi.org/project/ss-python/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ss-python)](https://pypi.org/project/ss-python/)
 [![GitHub](https://img.shields.io/github/license/serious-scaffold/ss-python)](https://github.com/serious-scaffold/ss-python/blob/main/LICENSE)
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](https://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

