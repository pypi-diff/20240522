# Comparing `tmp/zalando_cli_bundle-24.8.0.tar.gz` & `tmp/zalando_cli_bundle-24.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zalando_cli_bundle-24.8.0.tar", max compression
+gzip compressed data, was "zalando_cli_bundle-24.9.0.tar", max compression
```

## Comparing `zalando_cli_bundle-24.8.0.tar` & `zalando_cli_bundle-24.9.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1206 2024-04-17 07:20:54.000000 zalando_cli_bundle-24.8.0/pyproject.toml
--rw-r--r--   0        0        0       30 2024-04-17 07:20:54.000000 zalando_cli_bundle-24.8.0/zalando_cli_bundle/__main__.py
--rw-r--r--   0        0        0      581 2024-04-17 07:20:54.000000 zalando_cli_bundle-24.8.0/zalando_cli_bundle/cli.py
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 zalando_cli_bundle-24.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1206 2024-04-30 13:25:25.000000 zalando_cli_bundle-24.9.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2024-04-30 13:25:25.000000 zalando_cli_bundle-24.9.0/zalando_cli_bundle/__main__.py
+-rw-r--r--   0        0        0      581 2024-04-30 13:25:25.000000 zalando_cli_bundle-24.9.0/zalando_cli_bundle/cli.py
+-rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 zalando_cli_bundle-24.9.0/PKG-INFO
```

### Comparing `zalando_cli_bundle-24.8.0/pyproject.toml` & `zalando_cli_bundle-24.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zalando-cli-bundle"
-version = "24.8.0"
+version = "24.9.0"
 description = "CLI bundle for Zalando developers"
 authors = ["Henning Jacobs <henning@zalando.de>"]
 classifiers = [
     "Framework :: Pytest",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: System Administrators",
```

### Comparing `zalando_cli_bundle-24.8.0/zalando_cli_bundle/cli.py` & `zalando_cli_bundle-24.9.0/zalando_cli_bundle/cli.py`

 * *Files identical despite different names*

### Comparing `zalando_cli_bundle-24.8.0/PKG-INFO` & `zalando_cli_bundle-24.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zalando-cli-bundle
-Version: 24.8.0
+Version: 24.9.0
 Summary: CLI bundle for Zalando developers
 Home-page: https://github.bus.zalan.do/developer-productivity/zalando-cli-bundle
 Author: Henning Jacobs
 Author-email: henning@zalando.de
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: Framework :: Pytest
```

