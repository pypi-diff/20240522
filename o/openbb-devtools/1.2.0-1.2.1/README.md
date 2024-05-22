# Comparing `tmp/openbb_devtools-1.2.0.tar.gz` & `tmp/openbb_devtools-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_devtools-1.2.0.tar", max compression
+gzip compressed data, was "openbb_devtools-1.2.1.tar", max compression
```

## Comparing `openbb_devtools-1.2.0.tar` & `openbb_devtools-1.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      604 2024-02-29 11:03:36.732430 openbb_devtools-1.2.0/README.md
--rw-r--r--   0        0        0       39 2024-02-29 11:03:36.732586 openbb_devtools-1.2.0/openbb_devtools/__init__.py
--rw-r--r--   0        0        0      737 2024-05-15 16:04:25.865417 openbb_devtools-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1809 1970-01-01 00:00:00.000000 openbb_devtools-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      604 2024-05-14 16:56:41.557863 openbb_devtools-1.2.1/README.md
+-rw-r--r--   0        0        0       39 2024-05-14 16:56:41.557863 openbb_devtools-1.2.1/openbb_devtools/__init__.py
+-rw-r--r--   0        0        0      819 2024-05-22 13:55:18.911437 openbb_devtools-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 openbb_devtools-1.2.1/PKG-INFO
```

### Comparing `openbb_devtools-1.2.0/README.md` & `openbb_devtools-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_devtools-1.2.0/pyproject.toml` & `openbb_devtools-1.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 [tool.poetry]
 name = "openbb-devtools"
-version = "1.2.0"
+version = "1.2.1"
 description = "Tools for OpenBB Platform Developers"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_devtools" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"               # scipy forces <4.0 explicitly
-ruff = "^0.1.6"
+ruff = "^0.4.4"
 pylint = "^3.0.2"
 mypy = "^1.6.1"
 pydocstyle = "^6.3.0"
-black = "^24.1.0"
+black = "^24.4.2"
 bandit = "^1.7.5"
 codespell = "^2.2.5"
 pre-commit = "^3.5.0"
 tox = "^4.11.3"
 pytest = "^7.4.3"
+pytest-subtests = "^0.11.0"
+pytest-recorder = "^0.2.4"
+pytest-asyncio = "^0.23.2"
 pytest-cov = "^4.1.0"
 ipykernel = "^6.26.0"
 types-python-dateutil = "^2.8.19.14"
 types-toml = "^0.10.8.7"
 poetry = "^1.7.0"
```

### Comparing `openbb_devtools-1.2.0/PKG-INFO` & `openbb_devtools-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: openbb-devtools
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tools for OpenBB Platform Developers
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bandit (>=1.7.5,<2.0.0)
-Requires-Dist: black (>=24.1.0,<25.0.0)
+Requires-Dist: black (>=24.4.2,<25.0.0)
 Requires-Dist: codespell (>=2.2.5,<3.0.0)
 Requires-Dist: ipykernel (>=6.26.0,<7.0.0)
 Requires-Dist: mypy (>=1.6.1,<2.0.0)
 Requires-Dist: poetry (>=1.7.0,<2.0.0)
 Requires-Dist: pre-commit (>=3.5.0,<4.0.0)
 Requires-Dist: pydocstyle (>=6.3.0,<7.0.0)
 Requires-Dist: pylint (>=3.0.2,<4.0.0)
 Requires-Dist: pytest (>=7.4.3,<8.0.0)
+Requires-Dist: pytest-asyncio (>=0.23.2,<0.24.0)
 Requires-Dist: pytest-cov (>=4.1.0,<5.0.0)
-Requires-Dist: ruff (>=0.1.6,<0.2.0)
+Requires-Dist: pytest-recorder (>=0.2.4,<0.3.0)
+Requires-Dist: pytest-subtests (>=0.11.0,<0.12.0)
+Requires-Dist: ruff (>=0.4.4,<0.5.0)
 Requires-Dist: tox (>=4.11.3,<5.0.0)
 Requires-Dist: types-python-dateutil (>=2.8.19.14,<3.0.0.0)
 Requires-Dist: types-toml (>=0.10.8.7,<0.11.0.0)
 Description-Content-Type: text/markdown
 
 # The OpenBB DevTools Extension
```

