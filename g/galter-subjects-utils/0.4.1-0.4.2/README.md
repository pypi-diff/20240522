# Comparing `tmp/galter-subjects-utils-0.4.1.tar.gz` & `tmp/galter_subjects_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galter-subjects-utils-0.4.1.tar", last modified: Mon Apr  8 20:29:29 2024, max compression
+gzip compressed data, was "galter_subjects_utils-0.4.2.tar", last modified: Wed May 22 20:35:28 2024, max compression
```

## Comparing `galter-subjects-utils-0.4.1.tar` & `galter_subjects_utils-0.4.2.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.598306 galter-subjects-utils-0.4.1/galter_subjects_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.598306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/deltor.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/types_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/galter_subjects_utils/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-08 20:29:29.000000 galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 20:29:29.606305 galter-subjects-utils-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.594306 galter-subjects-utils-0.4.1/tests/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/contrib/lcsh/
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/contrib/mesh/
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/contrib/mesh/test_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:29.602306 galter-subjects-utils-0.4.1/tests/downloads/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/downloads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_deltor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_keeptrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-04-08 20:29:23.000000 galter-subjects-utils-0.4.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.700563 galter_subjects_utils-0.4.2/galter_subjects_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.700563 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.700563 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/types_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11543 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/galter_subjects_utils/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 20:35:28.000000 galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.696563 galter_subjects_utils-0.4.2/tests/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/tests/contrib/lcsh/
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/contrib/lcsh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/contrib/lcsh/test_downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/tests/contrib/mesh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/contrib/mesh/test_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/contrib/mesh/test_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/contrib/mesh/test_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:28.704563 galter_subjects_utils-0.4.2/tests/downloads/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/downloads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7605 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/test_deltor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/test_keeptrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/test_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-22 20:35:24.000000 galter_subjects_utils-0.4.2/tests/test_writer.py
```

### Comparing `galter-subjects-utils-0.4.1/LICENSE` & `galter_subjects_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/MANIFEST.in` & `galter_subjects_utils-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/PKG-INFO` & `galter_subjects_utils-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `galter-subjects-utils-0.4.1/README.md` & `galter_subjects_utils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/adapter.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/cli.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/cli.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/adapter.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/cli.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/cli.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/converter.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/downloader.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/lcsh/scheme.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/lcsh/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/adapter.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/adapter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/cli.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             MeSHReader(qualifiers_fp).read(),
             by="QA"
         )
     else:
         qualifiers_mapping = {}
 
     converted = MeSHRDMConverter(topics, qualifiers_mapping).convert()
-    dst = converted_to_subjects(converted)
+    dst = converted_to_subjects(converted, mesh.prefix)
 
     # Replacements
     replace_fp = downloads_dir / f"replace{year}.txt"
     replacements = generate_replacements(
         MeSHReplaceReader(replace_fp).read()
     )
```

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/converter.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/downloader.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/reader.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/contrib/mesh/scheme.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/contrib/mesh/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/deltor.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/deltor.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/downloader.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/keeptrace.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/reader.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/scheme.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/scheme.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/updater.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils/writer.py` & `galter_subjects_utils-0.4.2/galter_subjects_utils/writer.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/PKG-INFO` & `galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galter-subjects-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Subject terms tooling for InvenioRDM
 Author-email: Northwestern University <DL_FSM_GDS@e.northwestern.edu>
 License: MIT License
         
         Copyright (C) 2021-2023 Northwestern University.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
```

### Comparing `galter-subjects-utils-0.4.1/galter_subjects_utils.egg-info/SOURCES.txt` & `galter_subjects_utils-0.4.2/galter_subjects_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/pyproject.toml` & `galter_subjects_utils-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 keywords = ["invenio", "inveniordm", "subjects"]
 license = {file = "LICENSE"}
 name = "galter-subjects-utils"
 readme = "README.md"
 requires-python = ">=3.8"
 scripts = {galter-subjects-utils = "galter_subjects_utils.cli:main"}
 urls = {Repository = "https://github.com/galterlibrary/galter-subjects-utils"}
-version = "0.4.1"
+version = "0.4.2"
 
 [project.optional-dependencies]
 dev = [
     "check-manifest>=0.49",
     "invenio-search[opensearch2]>=2.1.0,<3.0.0",  # Needs to be specified separately as it's up to instance
     "invoke>=2.2,<3.0",
     "pytest-invenio>=2.1.1,<3.0.0",
```

### Comparing `galter-subjects-utils-0.4.1/tests/conftest.py` & `galter_subjects_utils-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_converter.py` & `galter_subjects_utils-0.4.2/tests/contrib/lcsh/test_converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/contrib/lcsh/test_downloader.py` & `galter_subjects_utils-0.4.2/tests/contrib/lcsh/test_downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_converter.py` & `galter_subjects_utils-0.4.2/tests/contrib/mesh/test_converter.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_downloader.py` & `galter_subjects_utils-0.4.2/tests/contrib/mesh/test_downloader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/contrib/mesh/test_reader.py` & `galter_subjects_utils-0.4.2/tests/contrib/mesh/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/test_deltor.py` & `galter_subjects_utils-0.4.2/tests/test_deltor.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/test_keeptrace.py` & `galter_subjects_utils-0.4.2/tests/test_keeptrace.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/test_reader.py` & `galter_subjects_utils-0.4.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/test_updater.py` & `galter_subjects_utils-0.4.2/tests/test_updater.py`

 * *Files identical despite different names*

### Comparing `galter-subjects-utils-0.4.1/tests/test_writer.py` & `galter_subjects_utils-0.4.2/tests/test_writer.py`

 * *Files identical despite different names*

