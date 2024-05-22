# Comparing `tmp/bflower-1.0.0a32.tar.gz` & `tmp/bflower-1.0.0a33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bflower-1.0.0a32.tar", max compression
+gzip compressed data, was "bflower-1.0.0a33.tar", max compression
```

## Comparing `bflower-1.0.0a32.tar` & `bflower-1.0.0a33.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-05-22 11:18:04.718349 bflower-1.0.0a32/LICENSE
--rw-r--r--   0        0        0     6998 2024-05-22 11:18:04.718349 bflower-1.0.0a32/README.md
--rw-r--r--   0        0        0     4301 2024-05-22 11:18:30.578350 bflower-1.0.0a32/pyproject.toml
--rw-r--r--   0        0        0       63 2024-05-22 11:18:05.230348 bflower-1.0.0a32/src/backend/bflower/version/__init__.py
--rw-r--r--   0        0        0      326 2024-05-22 11:18:05.230348 bflower-1.0.0a32/src/backend/bflower/version/version.py
--rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 bflower-1.0.0a32/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-22 13:57:43.691837 bflower-1.0.0a33/LICENSE
+-rw-r--r--   0        0        0     6998 2024-05-22 13:57:43.691837 bflower-1.0.0a33/README.md
+-rw-r--r--   0        0        0     4301 2024-05-22 13:58:08.743715 bflower-1.0.0a33/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-22 13:57:44.203835 bflower-1.0.0a33/src/backend/bflower/version/__init__.py
+-rw-r--r--   0        0        0      326 2024-05-22 13:57:44.203835 bflower-1.0.0a33/src/backend/bflower/version/version.py
+-rw-r--r--   0        0        0    10627 1970-01-01 00:00:00.000000 bflower-1.0.0a33/PKG-INFO
```

### Comparing `bflower-1.0.0a32/LICENSE` & `bflower-1.0.0a33/LICENSE`

 * *Files identical despite different names*

### Comparing `bflower-1.0.0a32/README.md` & `bflower-1.0.0a33/README.md`

 * *Files identical despite different names*

### Comparing `bflower-1.0.0a32/pyproject.toml` & `bflower-1.0.0a33/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bflower"
-version = "1.0.0a32"
+version = "1.0.0a33"
 description = "A Python package with a built-in web application"
 authors = ["Langflow <contact@langflow.org>"]
 maintainers = [
     "Carlos Coelho <carlos@langflow.org>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@langflow.org>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
```

### Comparing `bflower-1.0.0a32/PKG-INFO` & `bflower-1.0.0a33/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bflower
-Version: 1.0.0a32
+Version: 1.0.0a33
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/BNationsDEV/BFlower
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Langflow
 Author-email: contact@langflow.org
 Maintainer: Carlos Coelho
```

