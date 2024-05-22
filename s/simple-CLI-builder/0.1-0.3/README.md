# Comparing `tmp/simple_CLI_builder-0.1.tar.gz` & `tmp/simple_CLI_builder-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_CLI_builder-0.1.tar", last modified: Wed May 22 01:44:21 2024, max compression
+gzip compressed data, was "simple_CLI_builder-0.3.tar", last modified: Wed May 22 01:55:31 2024, max compression
```

## Comparing `simple_CLI_builder-0.1.tar` & `simple_CLI_builder-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:44:21.461068 simple_CLI_builder-0.1/
--rw-rw-rw-   0        0        0     1086 2024-05-22 00:30:28.000000 simple_CLI_builder-0.1/LICENSE
--rw-rw-rw-   0        0        0       86 2024-05-22 01:44:21.460070 simple_CLI_builder-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3322 2024-05-22 01:23:30.000000 simple_CLI_builder-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 01:44:21.461068 simple_CLI_builder-0.1/setup.cfg
--rw-rw-rw-   0        0        0      165 2024-05-22 01:44:19.000000 simple_CLI_builder-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:44:21.446542 simple_CLI_builder-0.1/simple_CLI_builder/
--rw-rw-rw-   0        0        0       21 2024-05-22 00:42:16.000000 simple_CLI_builder-0.1/simple_CLI_builder/__init__.py
--rw-rw-rw-   0        0        0     4307 2024-05-22 00:50:37.000000 simple_CLI_builder-0.1/simple_CLI_builder/main.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:44:21.458060 simple_CLI_builder-0.1/simple_CLI_builder.egg-info/
--rw-rw-rw-   0        0        0       86 2024-05-22 01:44:21.000000 simple_CLI_builder-0.1/simple_CLI_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-05-22 01:44:21.000000 simple_CLI_builder-0.1/simple_CLI_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:44:21.000000 simple_CLI_builder-0.1/simple_CLI_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 01:44:21.000000 simple_CLI_builder-0.1/simple_CLI_builder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:31.779611 simple_CLI_builder-0.3/
+-rw-rw-rw-   0        0        0     1086 2024-05-22 00:30:28.000000 simple_CLI_builder-0.3/LICENSE
+-rw-rw-rw-   0        0        0     3451 2024-05-22 01:55:31.778447 simple_CLI_builder-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3322 2024-05-22 01:23:30.000000 simple_CLI_builder-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:55:31.779611 simple_CLI_builder-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-05-22 01:55:09.000000 simple_CLI_builder-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:31.769763 simple_CLI_builder-0.3/simple_CLI_builder/
+-rw-rw-rw-   0        0        0       21 2024-05-22 00:42:16.000000 simple_CLI_builder-0.3/simple_CLI_builder/__init__.py
+-rw-rw-rw-   0        0        0     4307 2024-05-22 00:50:37.000000 simple_CLI_builder-0.3/simple_CLI_builder/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:55:31.777441 simple_CLI_builder-0.3/simple_CLI_builder.egg-info/
+-rw-rw-rw-   0        0        0     3451 2024-05-22 01:55:31.000000 simple_CLI_builder-0.3/simple_CLI_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-05-22 01:55:31.000000 simple_CLI_builder-0.3/simple_CLI_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:55:31.000000 simple_CLI_builder-0.3/simple_CLI_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 01:55:31.000000 simple_CLI_builder-0.3/simple_CLI_builder.egg-info/top_level.txt
```

### Comparing `simple_CLI_builder-0.1/LICENSE` & `simple_CLI_builder-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_CLI_builder-0.1/README.md` & `simple_CLI_builder-0.3/README.md`

 * *Files identical despite different names*

### Comparing `simple_CLI_builder-0.1/simple_CLI_builder/main.py` & `simple_CLI_builder-0.3/simple_CLI_builder/main.py`

 * *Files identical despite different names*

