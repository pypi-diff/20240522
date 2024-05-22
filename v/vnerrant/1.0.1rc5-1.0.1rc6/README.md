# Comparing `tmp/vnerrant-1.0.1rc5.tar.gz` & `tmp/vnerrant-1.0.1rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnerrant-1.0.1rc5.tar", last modified: Wed May 22 08:27:43 2024, max compression
+gzip compressed data, was "vnerrant-1.0.1rc6.tar", last modified: Wed May 22 17:17:19 2024, max compression
```

## Comparing `vnerrant-1.0.1rc5.tar` & `vnerrant-1.0.1rc6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.207322 vnerrant-1.0.1rc5/
--rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/MANIFEST.in
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 08:27:43.206956 vnerrant-1.0.1rc5/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-22 08:27:43.207395 vnerrant-1.0.1rc5/setup.cfg
--rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-22 08:26:05.000000 vnerrant-1.0.1rc5/setup.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.189601 vnerrant-1.0.1rc5/tests/
--rw-r--r--   0 manred1997   (501) staff       (20)     7372 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc5/tests/test_vnerrant.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.191044 vnerrant-1.0.1rc5/vnerrant/
--rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-22 08:26:14.000000 vnerrant-1.0.1rc5/vnerrant/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    11994 2024-05-22 08:09:46.000000 vnerrant-1.0.1rc5/vnerrant/annotator.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.192656 vnerrant-1.0.1rc5/vnerrant/cli/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/convert.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/evaluate.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.194941 vnerrant-1.0.1rc5/vnerrant/components/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/alignment.py
--rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/converter.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.197605 vnerrant-1.0.1rc5/vnerrant/components/en/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/constants.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/lancaster.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/merger.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.199205 vnerrant-1.0.1rc5/vnerrant/components/en/resources/
--rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/en-ptb_map
--rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/en_GB-large.txt
--rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/evaluater.py
--rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/merger.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/tokenizer.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.202867 vnerrant-1.0.1rc5/vnerrant/config/
--rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/config/errant_verbose.json
--rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/config/mapping_type_error.yaml
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/config.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2047 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc5/vnerrant/constants.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.203348 vnerrant-1.0.1rc5/vnerrant/metrics/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/criteria.py
--rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/stats.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.203980 vnerrant-1.0.1rc5/vnerrant/model/
--rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc5/vnerrant/model/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc5/vnerrant/model/edit.py
--rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/run_cli.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.206358 vnerrant-1.0.1rc5/vnerrant/utils/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6539 2024-05-22 08:24:02.000000 vnerrant-1.0.1rc5/vnerrant/utils/edit_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/helper.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/pretty_results.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/utils/string_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/utils.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.206578 vnerrant-1.0.1rc5/vnerrant.egg-info/
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/SOURCES.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/dependency_links.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/entry_points.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/requires.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/top_level.txt
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.376209 vnerrant-1.0.1rc6/
+-rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/MANIFEST.in
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 17:17:19.375700 vnerrant-1.0.1rc6/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-22 17:17:19.376282 vnerrant-1.0.1rc6/setup.cfg
+-rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-22 17:16:06.000000 vnerrant-1.0.1rc6/setup.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.357478 vnerrant-1.0.1rc6/tests/
+-rw-r--r--   0 manred1997   (501) staff       (20)     7372 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc6/tests/test_vnerrant.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.358722 vnerrant-1.0.1rc6/vnerrant/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-22 17:16:09.000000 vnerrant-1.0.1rc6/vnerrant/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    11994 2024-05-22 17:14:08.000000 vnerrant-1.0.1rc6/vnerrant/annotator.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.360257 vnerrant-1.0.1rc6/vnerrant/cli/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/cli/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/cli/convert.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/cli/evaluate.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.361983 vnerrant-1.0.1rc6/vnerrant/components/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/alignment.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/converter.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.363530 vnerrant-1.0.1rc6/vnerrant/components/en/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/en/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/constants.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/en/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/lancaster.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/en/merger.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.364270 vnerrant-1.0.1rc6/vnerrant/components/en/resources/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/resources/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/resources/en-ptb_map
+-rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/resources/en_GB-large.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/en/utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/evaluater.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/components/merger.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/components/tokenizer.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.369720 vnerrant-1.0.1rc6/vnerrant/config/
+-rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/config/errant_verbose.json
+-rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/config/mapping_type_error.yaml
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/config.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2047 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc6/vnerrant/constants.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.370265 vnerrant-1.0.1rc6/vnerrant/metrics/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/metrics/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/metrics/criteria.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/metrics/stats.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.370646 vnerrant-1.0.1rc6/vnerrant/model/
+-rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc6/vnerrant/model/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc6/vnerrant/model/edit.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/run_cli.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.374711 vnerrant-1.0.1rc6/vnerrant/utils/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/utils/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6845 2024-05-22 17:13:40.000000 vnerrant-1.0.1rc6/vnerrant/utils/edit_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/utils/helper.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/utils/pretty_results.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc6/vnerrant/utils/string_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc6/vnerrant/utils/utils.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 17:17:19.375204 vnerrant-1.0.1rc6/vnerrant.egg-info/
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/SOURCES.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/dependency_links.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/entry_points.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/requires.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-22 17:17:19.000000 vnerrant-1.0.1rc6/vnerrant.egg-info/top_level.txt
```

### Comparing `vnerrant-1.0.1rc5/PKG-INFO` & `vnerrant-1.0.1rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc5
+Version: 1.0.1rc6
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc5/README.md` & `vnerrant-1.0.1rc6/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/setup.py` & `vnerrant-1.0.1rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Readme text for long description
 with open(base_dir / "README.md") as f:
     readme = f.read()
 
 setup(
     name="vnerrant",
-    version="1.0.1rc5",
+    version="1.0.1rc6",
     license="MIT",
     description="The ERRor ANnotation Toolkit (ERRANT). \
         Automatically extract and classify edits in parallel sentences.",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=[
         "automatic annotation",
```

### Comparing `vnerrant-1.0.1rc5/tests/test_vnerrant.py` & `vnerrant-1.0.1rc6/tests/test_vnerrant.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/__init__.py` & `vnerrant-1.0.1rc6/vnerrant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import spacy
 
 from vnerrant.annotator import Annotator
 from vnerrant.utils.utils import get_spacy_models_for_language
 
-__version__ = "v1.0.1rc5"
+__version__ = "v1.0.1rc6"
 
 
 def load(
     lang: str = "en",
     model_name: str = "en_core_web_sm",
     nlp: Any = None,
 ) -> Annotator:
```

### Comparing `vnerrant-1.0.1rc5/vnerrant/annotator.py` & `vnerrant-1.0.1rc6/vnerrant/annotator.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/cli/convert.py` & `vnerrant-1.0.1rc6/vnerrant/cli/convert.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/cli/evaluate.py` & `vnerrant-1.0.1rc6/vnerrant/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/alignment.py` & `vnerrant-1.0.1rc6/vnerrant/components/alignment.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/converter.py` & `vnerrant-1.0.1rc6/vnerrant/components/converter.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/classifier.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/classifier.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/constants.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/explainer.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/explainer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/lancaster.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/merger.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/resources/README.md` & `vnerrant-1.0.1rc6/vnerrant/components/en/resources/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/resources/en_GB-large.txt` & `vnerrant-1.0.1rc6/vnerrant/components/en/resources/en_GB-large.txt`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/en/utils.py` & `vnerrant-1.0.1rc6/vnerrant/components/en/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/evaluater.py` & `vnerrant-1.0.1rc6/vnerrant/components/evaluater.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/merger.py` & `vnerrant-1.0.1rc6/vnerrant/components/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/components/tokenizer.py` & `vnerrant-1.0.1rc6/vnerrant/components/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/config/errant_verbose.json` & `vnerrant-1.0.1rc6/vnerrant/config/errant_verbose.json`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/config/mapping_type_error.yaml` & `vnerrant-1.0.1rc6/vnerrant/config/mapping_type_error.yaml`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/constants.py` & `vnerrant-1.0.1rc6/vnerrant/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/metrics/criteria.py` & `vnerrant-1.0.1rc6/vnerrant/metrics/criteria.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/model/edit.py` & `vnerrant-1.0.1rc6/vnerrant/model/edit.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/run_cli.py` & `vnerrant-1.0.1rc6/vnerrant/run_cli.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/utils/edit_utils.py` & `vnerrant-1.0.1rc6/vnerrant/utils/edit_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -109,42 +109,48 @@
         elif not orig_text and cor_text:
             edit.edit_type = "M" + edit.edit_type[1:]
         else:
             edit.edit_type = "U" + edit.edit_type[1:]
 
 def update_span_edit(edits: List[Edit]):  # noqa D103
     """
-    Update the replace operator of the edits.
+    Update the replace operator of the edits by trimming matching leading
+    and trailing spaces in both original and corrected text of each edit.
+    
     Args:
-        edits (list[Edit]): A list of Edit objects to be updated.
+        edits (list): A list of Edit objects to be updated.
     """
-    def trim_text_span(text: str, start: int, end: int) -> tuple:
-        # Increment the start index to skip leading whitespace
-        for t in text[:]:
-            if not t.isspace():
-                break
-            start += 1
-        # Decrement the end index to skip trailing whitespace
-        for t in text[::-1]:
-            if not t.isspace():
-                break
-            end -= 1
-        stripped_text = text.strip()
-        return stripped_text, start, end
 
     for edit in edits:
         if edit.edit_type[0] == "R":
-            stripped_orig_text, start_orig, end_orig = trim_text_span(edit.original.text, edit.original.start_char, edit.original.end_char)
-            stripped_corr_text, start_corr, end_corr = trim_text_span(edit.corrected.text, edit.corrected.start_char, edit.corrected.end_char)
-            edit.original.text = stripped_orig_text
+            orig_text, start_orig, end_orig = edit.original.text, edit.original.start_char, edit.original.end_char
+            corr_text, start_corr, end_corr = edit.corrected.text, edit.corrected.start_char, edit.corrected.end_char
+            
+            # Remove trailing spaces if both original and corrected texts end with them
+            while orig_text.endswith(" ") and corr_text.endswith(" "):
+                orig_text = orig_text[:-1]
+                corr_text = corr_text[:-1]
+                end_orig -= 1
+                end_corr -= 1
+            
+            # Remove leading spaces if both original and corrected texts start with them
+            while orig_text.startswith(" ") and corr_text.startswith(" "):
+                orig_text = orig_text[1:]
+                corr_text = corr_text[1:]
+                start_orig += 1
+                start_corr += 1
+            
+            # Update the texts and character positions back to the Edit objects
+            edit.original.text = orig_text
+            edit.corrected.text = corr_text
             edit.original.start_char = start_orig
             edit.original.end_char = end_orig
-            edit.corrected.text = stripped_corr_text
             edit.corrected.start_char = start_corr
             edit.corrected.end_char = end_corr
+            
 
 
 def process_space_edit(edit: Edit) -> Edit:
     """
     Process the space edit.
     Args:
         edit (Edit): An Edit object to be processed.
```

### Comparing `vnerrant-1.0.1rc5/vnerrant/utils/helper.py` & `vnerrant-1.0.1rc6/vnerrant/utils/helper.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/utils/pretty_results.py` & `vnerrant-1.0.1rc6/vnerrant/utils/pretty_results.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/utils/string_utils.py` & `vnerrant-1.0.1rc6/vnerrant/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant/utils/utils.py` & `vnerrant-1.0.1rc6/vnerrant/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc5/vnerrant.egg-info/PKG-INFO` & `vnerrant-1.0.1rc6/vnerrant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc5
+Version: 1.0.1rc6
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc5/vnerrant.egg-info/SOURCES.txt` & `vnerrant-1.0.1rc6/vnerrant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

