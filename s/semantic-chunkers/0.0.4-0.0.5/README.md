# Comparing `tmp/semantic_chunkers-0.0.4.tar.gz` & `tmp/semantic_chunkers-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_chunkers-0.0.4.tar", max compression
+gzip compressed data, was "semantic_chunkers-0.0.5.tar", max compression
```

## Comparing `semantic_chunkers-0.0.4.tar` & `semantic_chunkers-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1067 2024-05-15 17:40:17.975943 semantic_chunkers-0.0.4/LICENSE
--rw-r--r--   0        0        0     1397 2024-05-15 17:40:17.975943 semantic_chunkers-0.0.4/README.md
--rw-r--r--   0        0        0     1015 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      358 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/__init__.py
--rw-r--r--   0        0        0      375 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/__init__.py
--rw-r--r--   0        0        0     1521 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/base.py
--rw-r--r--   0        0        0     2734 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/consecutive.py
--rw-r--r--   0        0        0     3582 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/cumulative.py
--rw-r--r--   0        0        0    18475 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/chunkers/statistical.py
--rw-r--r--   0        0        0      353 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/schema.py
--rw-r--r--   0        0        0        0 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/splitters/__init__.py
--rw-r--r--   0        0        0     2003 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/splitters/sentence.py
--rw-r--r--   0        0        0        0 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/__init__.py
--rw-r--r--   0        0        0     1008 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/logger.py
--rw-r--r--   0        0        0      192 2024-05-15 17:40:18.031942 semantic_chunkers-0.0.4/semantic_chunkers/utils/text.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-22 07:54:59.900323 semantic_chunkers-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1397 2024-05-22 07:54:59.900323 semantic_chunkers-0.0.5/README.md
+-rw-r--r--   0        0        0     1066 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/__init__.py
+-rw-r--r--   0        0        0      375 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/__init__.py
+-rw-r--r--   0        0        0     1521 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/base.py
+-rw-r--r--   0        0        0     2734 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/consecutive.py
+-rw-r--r--   0        0        0     3582 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/cumulative.py
+-rw-r--r--   0        0        0    18475 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/chunkers/statistical.py
+-rw-r--r--   0        0        0      353 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/splitters/__init__.py
+-rw-r--r--   0        0        0     2003 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/splitters/sentence.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/__init__.py
+-rw-r--r--   0        0        0     1008 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/logger.py
+-rw-r--r--   0        0        0      192 2024-05-22 07:54:59.960323 semantic_chunkers-0.0.5/semantic_chunkers/utils/text.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 semantic_chunkers-0.0.5/PKG-INFO
```

### Comparing `semantic_chunkers-0.0.4/LICENSE` & `semantic_chunkers-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/README.md` & `semantic_chunkers-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/pyproject.toml` & `semantic_chunkers-0.0.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "semantic-chunkers"
-version = "0.0.4"
+version = "0.0.5"
 description = "Super advanced chunking methods for AI"
 authors = ["Aurelio AI <hello@aurelio.ai>"]
 readme = "README.md"
 packages = [{include = "semantic_chunkers"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pydantic = "^2.5.3"
 numpy = "^1.25.2"
 colorlog = "^6.8.0"
 colorama = "^0.4.6"
 regex = "^2023.12.25"
-tiktoken = "^0.6.0"
+tiktoken = ">=0.7.0,<1.0.0"
 matplotlib = { version = "^3.8.3", optional = true}
 requests-mock = "^1.12.1"
 semantic-router = ">=0.0.20,<0.1.0"
 
 [tool.poetry.extras]
 stats = ["matplotlib"]
 
@@ -27,15 +27,15 @@
 pytest = "^7.4.3"
 pytest-mock = "^3.12.0"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.5.0"
 mypy = "^1.7.1"
 types-pyyaml = "^6.0.12.12"
 types-requests = "^2.31.0"
-black = "^23.12.1"
+black = {extras = ["jupyter"], version = ">=23.12.1,<24.5.0"}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff.per-file-ignores]
 "*.ipynb" = ["ALL"]
```

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/base.py` & `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/base.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/consecutive.py` & `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/consecutive.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/cumulative.py` & `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/cumulative.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/chunkers/statistical.py` & `semantic_chunkers-0.0.5/semantic_chunkers/chunkers/statistical.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/splitters/sentence.py` & `semantic_chunkers-0.0.5/semantic_chunkers/splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/semantic_chunkers/utils/logger.py` & `semantic_chunkers-0.0.5/semantic_chunkers/utils/logger.py`

 * *Files identical despite different names*

### Comparing `semantic_chunkers-0.0.4/PKG-INFO` & `semantic_chunkers-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-chunkers
-Version: 0.0.4
+Version: 0.0.5
 Summary: Super advanced chunking methods for AI
 Author: Aurelio AI
 Author-email: hello@aurelio.ai
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,15 +14,15 @@
 Requires-Dist: colorlog (>=6.8.0,<7.0.0)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0) ; extra == "stats"
 Requires-Dist: numpy (>=1.25.2,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: regex (>=2023.12.25,<2024.0.0)
 Requires-Dist: requests-mock (>=1.12.1,<2.0.0)
 Requires-Dist: semantic-router (>=0.0.20,<0.1.0)
-Requires-Dist: tiktoken (>=0.6.0,<0.7.0)
+Requires-Dist: tiktoken (>=0.7.0,<1.0.0)
 Description-Content-Type: text/markdown
 
 [![Aurelio AI](https://pbs.twimg.com/profile_banners/1671498317455581184/1696285195/1500x500)](https://aurelio.ai)
 
 # Semantic Chunkers
 
 <p>
```

