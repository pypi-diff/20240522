# Comparing `tmp/openbb_seeking_alpha-1.2.0.tar.gz` & `tmp/openbb_seeking_alpha-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_seeking_alpha-1.2.0.tar", max compression
+gzip compressed data, was "openbb_seeking_alpha-1.2.1.tar", max compression
```

## Comparing `openbb_seeking_alpha-1.2.0.tar` & `openbb_seeking_alpha-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      326 2024-05-15 14:24:46.652204 openbb_seeking_alpha-1.2.0/README.md
--rw-r--r--   0        0        0      539 2024-05-14 15:30:05.618862 openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/__init__.py
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.969719 openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/models/__init__.py
--rw-r--r--   0        0        0     3791 2024-02-29 11:03:36.969804 openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/models/upcoming_release_days.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.969831 openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/py.typed
--rw-r--r--   0        0        0       27 2024-02-29 11:03:36.969907 openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/utils/__init__.py
--rw-r--r--   0        0        0      519 2024-05-15 16:05:49.729833 openbb_seeking_alpha-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 openbb_seeking_alpha-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      326 2024-05-22 11:48:40.547330 openbb_seeking_alpha-1.2.1/README.md
+-rw-r--r--   0        0        0      539 2024-05-15 09:21:56.097885 openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-14 16:56:42.109866 openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/models/__init__.py
+-rw-r--r--   0        0        0     3791 2024-05-14 16:56:42.109866 openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/models/upcoming_release_days.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:42.109866 openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/py.typed
+-rw-r--r--   0        0        0       27 2024-05-14 16:56:42.109866 openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/utils/__init__.py
+-rw-r--r--   0        0        0      519 2024-05-22 13:56:52.283747 openbb_seeking_alpha-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 openbb_seeking_alpha-1.2.1/PKG-INFO
```

### Comparing `openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/__init__.py` & `openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_seeking_alpha-1.2.0/openbb_seeking_alpha/models/upcoming_release_days.py` & `openbb_seeking_alpha-1.2.1/openbb_seeking_alpha/models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_seeking_alpha-1.2.0/pyproject.toml` & `openbb_seeking_alpha-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-seeking-alpha"
-version = "1.2.0"
+version = "1.2.1"
 description = "Seeking Alpha extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_seeking_alpha" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 seeking_alpha = "openbb_seeking_alpha:seeking_alpha_provider"
```

### Comparing `openbb_seeking_alpha-1.2.0/PKG-INFO` & `openbb_seeking_alpha-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-seeking-alpha
-Version: 1.2.0
+Version: 1.2.1
 Summary: Seeking Alpha extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Seeking Alpha Provider
 
 This extension integrates the [Seeking Alpha](https://seekingalpha.com) data provider into the OpenBB Platform.
 
 ## Installation
```

