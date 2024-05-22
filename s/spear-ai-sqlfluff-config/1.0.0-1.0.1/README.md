# Comparing `tmp/spear_ai_sqlfluff_config-1.0.0.tar.gz` & `tmp/spear_ai_sqlfluff_config-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear_ai_sqlfluff_config-1.0.0.tar", max compression
+gzip compressed data, was "spear_ai_sqlfluff_config-1.0.1.tar", max compression
```

## Comparing `spear_ai_sqlfluff_config-1.0.0.tar` & `spear_ai_sqlfluff_config-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      416 2024-05-21 09:30:50.856954 spear_ai_sqlfluff_config-1.0.0/README.md
--rw-r--r--   0        0        0      490 2024-05-21 09:30:50.856954 spear_ai_sqlfluff_config-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      916 2024-05-21 09:30:50.856954 spear_ai_sqlfluff_config-1.0.0/spear_ai_sqlfluff_config/.sqlfluff
--rw-r--r--   0        0        0       32 2024-05-21 09:30:50.856954 spear_ai_sqlfluff_config-1.0.0/spear_ai_sqlfluff_config/__init__.py
--rw-r--r--   0        0        0     1015 1970-01-01 00:00:00.000000 spear_ai_sqlfluff_config-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      416 2024-05-22 17:57:54.151813 spear_ai_sqlfluff_config-1.0.1/README.md
+-rw-r--r--   0        0        0      494 2024-05-22 17:57:54.151813 spear_ai_sqlfluff_config-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      916 2024-05-22 17:57:54.151813 spear_ai_sqlfluff_config-1.0.1/spear_ai_sqlfluff_config/.sqlfluff
+-rw-r--r--   0        0        0       32 2024-05-22 17:57:54.151813 spear_ai_sqlfluff_config-1.0.1/spear_ai_sqlfluff_config/__init__.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 spear_ai_sqlfluff_config-1.0.1/PKG-INFO
```

### Comparing `spear_ai_sqlfluff_config-1.0.0/spear_ai_sqlfluff_config/.sqlfluff` & `spear_ai_sqlfluff_config-1.0.1/spear_ai_sqlfluff_config/.sqlfluff`

 * *Files identical despite different names*

### Comparing `spear_ai_sqlfluff_config-1.0.0/PKG-INFO` & `spear_ai_sqlfluff_config-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: spear-ai-sqlfluff-config
-Version: 1.0.0
-Summary: Spear AI Ruff config
+Version: 1.0.1
+Summary: Spear AI SQLFluff config
 Home-page: https://github.com/spear-ai/citizen
 Keywords: ai,config,SQLFluff,spear
 Author: Spear AI
 Author-email: org@spear.ai
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

