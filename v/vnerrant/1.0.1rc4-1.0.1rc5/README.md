# Comparing `tmp/vnerrant-1.0.1rc4.tar.gz` & `tmp/vnerrant-1.0.1rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnerrant-1.0.1rc4.tar", last modified: Thu May 16 03:16:45 2024, max compression
+gzip compressed data, was "vnerrant-1.0.1rc5.tar", last modified: Wed May 22 08:27:43 2024, max compression
```

## Comparing `vnerrant-1.0.1rc4.tar` & `vnerrant-1.0.1rc5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.901372 vnerrant-1.0.1rc4/
--rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/MANIFEST.in
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-16 03:16:45.901085 vnerrant-1.0.1rc4/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-16 03:16:45.901422 vnerrant-1.0.1rc4/setup.cfg
--rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-16 03:14:49.000000 vnerrant-1.0.1rc4/setup.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.883010 vnerrant-1.0.1rc4/tests/
--rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/tests/test_vnerrant.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.884563 vnerrant-1.0.1rc4/vnerrant/
--rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-16 03:15:01.000000 vnerrant-1.0.1rc4/vnerrant/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12029 2024-05-16 03:12:28.000000 vnerrant-1.0.1rc4/vnerrant/annotator.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.886062 vnerrant-1.0.1rc4/vnerrant/cli/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/convert.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/evaluate.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.888423 vnerrant-1.0.1rc4/vnerrant/components/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/alignment.py
--rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/converter.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.890421 vnerrant-1.0.1rc4/vnerrant/components/en/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/constants.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/lancaster.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/merger.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.891052 vnerrant-1.0.1rc4/vnerrant/components/en/resources/
--rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/en-ptb_map
--rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/en_GB-large.txt
--rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/evaluater.py
--rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/merger.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/tokenizer.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.896251 vnerrant-1.0.1rc4/vnerrant/config/
--rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/config/errant_verbose.json
--rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/config/mapping_type_error.yaml
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/config.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/constants.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.896922 vnerrant-1.0.1rc4/vnerrant/metrics/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/criteria.py
--rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/stats.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.898380 vnerrant-1.0.1rc4/vnerrant/model/
--rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/vnerrant/model/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/vnerrant/model/edit.py
--rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/run_cli.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.900581 vnerrant-1.0.1rc4/vnerrant/utils/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7243 2024-05-16 03:11:45.000000 vnerrant-1.0.1rc4/vnerrant/utils/edit_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/helper.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/pretty_results.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/utils/string_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/utils.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.900793 vnerrant-1.0.1rc4/vnerrant.egg-info/
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/SOURCES.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/dependency_links.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/entry_points.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/requires.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/top_level.txt
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.207322 vnerrant-1.0.1rc5/
+-rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/MANIFEST.in
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 08:27:43.206956 vnerrant-1.0.1rc5/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-22 08:27:43.207395 vnerrant-1.0.1rc5/setup.cfg
+-rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-22 08:26:05.000000 vnerrant-1.0.1rc5/setup.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.189601 vnerrant-1.0.1rc5/tests/
+-rw-r--r--   0 manred1997   (501) staff       (20)     7372 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc5/tests/test_vnerrant.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.191044 vnerrant-1.0.1rc5/vnerrant/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-22 08:26:14.000000 vnerrant-1.0.1rc5/vnerrant/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    11994 2024-05-22 08:09:46.000000 vnerrant-1.0.1rc5/vnerrant/annotator.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.192656 vnerrant-1.0.1rc5/vnerrant/cli/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/convert.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/cli/evaluate.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.194941 vnerrant-1.0.1rc5/vnerrant/components/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/alignment.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/converter.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.197605 vnerrant-1.0.1rc5/vnerrant/components/en/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/constants.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/lancaster.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/en/merger.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.199205 vnerrant-1.0.1rc5/vnerrant/components/en/resources/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/en-ptb_map
+-rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/resources/en_GB-large.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/en/utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/evaluater.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/components/merger.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/components/tokenizer.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.202867 vnerrant-1.0.1rc5/vnerrant/config/
+-rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/config/errant_verbose.json
+-rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/config/mapping_type_error.yaml
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/config.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2047 2024-05-22 08:08:03.000000 vnerrant-1.0.1rc5/vnerrant/constants.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.203348 vnerrant-1.0.1rc5/vnerrant/metrics/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/criteria.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/metrics/stats.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.203980 vnerrant-1.0.1rc5/vnerrant/model/
+-rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc5/vnerrant/model/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc5/vnerrant/model/edit.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/run_cli.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.206358 vnerrant-1.0.1rc5/vnerrant/utils/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6539 2024-05-22 08:24:02.000000 vnerrant-1.0.1rc5/vnerrant/utils/edit_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/helper.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/pretty_results.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc5/vnerrant/utils/string_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc5/vnerrant/utils/utils.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-22 08:27:43.206578 vnerrant-1.0.1rc5/vnerrant.egg-info/
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/SOURCES.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/dependency_links.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/entry_points.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/requires.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-22 08:27:43.000000 vnerrant-1.0.1rc5/vnerrant.egg-info/top_level.txt
```

### Comparing `vnerrant-1.0.1rc4/PKG-INFO` & `vnerrant-1.0.1rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc4
+Version: 1.0.1rc5
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc4/README.md` & `vnerrant-1.0.1rc5/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/setup.py` & `vnerrant-1.0.1rc5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Readme text for long description
 with open(base_dir / "README.md") as f:
     readme = f.read()
 
 setup(
     name="vnerrant",
-    version="1.0.1rc4",
+    version="1.0.1rc5",
     license="MIT",
     description="The ERRor ANnotation Toolkit (ERRANT). \
         Automatically extract and classify edits in parallel sentences.",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=[
         "automatic annotation",
```

### Comparing `vnerrant-1.0.1rc4/tests/test_vnerrant.py` & `vnerrant-1.0.1rc5/tests/test_vnerrant.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 @pytest.mark.parametrize(
     'original, corrected',
     [
         ('I never thought about, people got so many pet.', 'I never thought about it before. People have so many pets.'),
         ("That I want to say, is very difficult to understand the conjuntion of the verb's in Spanish Languaje, just Imaging you the same but not in your native lenguaje.", "I want to say that it is very difficult to understand the conjugation of the verbs in Spanish, so just imagine the same but not in your native language."),
         ("Somehow, you can't always identify whether their bodies feel uncomfortable merely from their appearance, which leads to some misunderstanding between them.", "Somehow, not all of them can you identify whether their bodies feel uncomfortable merely from their appearance, which leads to Some misunderstanding between them?"),
+        ("We are so sorry we can give you a refund, but for the compensation, I think it a bit too much because you are sittimg here and we are also serving you. It’s salt free day, so it’s actually basically not our fault.", "We are so sorry. We can give you a refund, but for the compensation, I think it is a bit too much because you are sitting here and we are also serving you. It’s salt free day, so it’s actually basically not our fault."),
     ],
 )
 def test_normal_errant(original, corrected):
     check_edits(original, corrected)
 
 # Test the alignment of the original and corrected text (condition: the corrected text should be standardised)
 # Ignore the type of edit #TODO: add the type of edit
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `vnerrant-1.0.1rc4/vnerrant/__init__.py` & `vnerrant-1.0.1rc5/vnerrant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import spacy
 
 from vnerrant.annotator import Annotator
 from vnerrant.utils.utils import get_spacy_models_for_language
 
-__version__ = "v1.0.1rc4"
+__version__ = "v1.0.1rc5"
 
 
 def load(
     lang: str = "en",
     model_name: str = "en_core_web_sm",
     nlp: Any = None,
 ) -> Annotator:
```

### Comparing `vnerrant-1.0.1rc4/vnerrant/annotator.py` & `vnerrant-1.0.1rc5/vnerrant/annotator.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from spacy.tokens import Doc, Token
 
 from vnerrant.components.alignment import Alignment
 from vnerrant.components.classifier import BaseClassifer
 from vnerrant.components.explainer import BaseExplainer
 from vnerrant.components.merger import BaseMerger
-from vnerrant.constants import MERGING_ALL_EQUAL, MERGING_ALL_MERGE, MERGING_ALL_SPLIT, MERGING_RULES, TokenizeTypes
+from vnerrant.constants import MergeType, TokenizeTypes
 from vnerrant.model.edit import Edit, EditCollection
 from vnerrant.utils import edit_utils
 from vnerrant.utils.string_utils import StringTokenizer
 
 Token.set_extension("full_text", default=None, force=True)
 
 
@@ -114,44 +114,44 @@
         :param orig: An original text string
         :param cor: A corrected text string
         :param lev: A flag to use levenshtein alignment
         :return: An Alignment object
         """
         return Alignment(orig, cor, lev)
 
-    def merge(self, alignment: Alignment, merging: str = MERGING_RULES) -> list[Edit]:
+    def merge(self, alignment: Alignment, merging: str = MergeType.RULES) -> list[Edit]:
         """
         Merge an alignment into a list of edits.
         :param alignment: An Alignment object
         :param merging: A string merging strategy
         :return: A list of Edit objects
         """
         # rules: Rule-based merging
-        if merging == MERGING_RULES:
+        if merging == MergeType.RULES:
             edits = self.merger.get_all_rule_merge_edits(
                 alignment.orig,
                 alignment.cor,
                 alignment.align_seq,
             )
         # all-split: Don't merge anything
-        elif merging == MERGING_ALL_SPLIT:
+        elif merging == MergeType.ALL_SPLIT:
             edits = self.merger.get_all_split_edits(
                 alignment.orig,
                 alignment.cor,
                 alignment.align_seq,
             )
         # all-merge: Merge all adjacent non-match ops
-        elif merging == MERGING_ALL_MERGE:
+        elif merging == MergeType.ALL_MERGE:
             edits = self.merger.get_all_merge_edits(
                 alignment.orig,
                 alignment.cor,
                 alignment.align_seq,
             )
         # all-equal: Merge all edits of the same operation type
-        elif merging == MERGING_ALL_EQUAL:
+        elif merging == MergeType.ALL_EQUAL:
             edits = self.merger.get_all_equal_edits(
                 alignment.orig,
                 alignment.cor,
                 alignment.align_seq,
             )
         # Unknown
         else:
@@ -177,15 +177,15 @@
         return self.explainer.explain(edit)
 
     def annotate(
         self,
         orig: Doc,
         cor: Doc,
         lev: bool = False,
-        merging: str = "rules",
+        merging: str = MergeType.RULES,
     ) -> list[Edit]:
         """
         Annotate a pair of original and corrected spacy Doc objects.
         :param orig: An original spacy Doc object
         :param cor: A corrected spacy Doc object
         :param lev: A flag to use levenshtein alignment
         :param merging: A string merging strategy
@@ -199,15 +199,15 @@
         return edits
 
     def annotate_raw(
         self,
         orig: str,
         cor: str,
         lev: bool = False,
-        merging: str = "rules",
+        merging: str = MergeType.RULES,
         tokenize_type: str = TokenizeTypes.SPACY,
     ) -> list[Edit]:
         """
         Annotate a pair of original and corrected string objects.
         :param orig: An original text
         :param cor: A corrected text
         :param lev: A flag to use levenshtein alignment
@@ -286,15 +286,15 @@
                 continue
 
             space_edits.append(edit_utils.process_space_edit(edit))
 
         edit_utils.merge_edit_collection_with_space_edits(edit_collection, space_edits)
         edit_utils.update_operator(edit_collection.edits)
         if is_update_span:
-            edit_utils.upadte_span_edit(edit_collection.edits)
+            edit_utils.update_span_edit(edit_collection.edits)
 
     def import_edit(
         self,
         orig: Doc,
         cor: Doc,
         edit: list,
         min: bool = True,
```

### Comparing `vnerrant-1.0.1rc4/vnerrant/cli/convert.py` & `vnerrant-1.0.1rc5/vnerrant/cli/convert.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/cli/evaluate.py` & `vnerrant-1.0.1rc5/vnerrant/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/alignment.py` & `vnerrant-1.0.1rc5/vnerrant/components/alignment.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/converter.py` & `vnerrant-1.0.1rc5/vnerrant/components/converter.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/classifier.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/classifier.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/constants.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/explainer.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/explainer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/lancaster.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/merger.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/resources/README.md` & `vnerrant-1.0.1rc5/vnerrant/components/en/resources/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/resources/en_GB-large.txt` & `vnerrant-1.0.1rc5/vnerrant/components/en/resources/en_GB-large.txt`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/en/utils.py` & `vnerrant-1.0.1rc5/vnerrant/components/en/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/evaluater.py` & `vnerrant-1.0.1rc5/vnerrant/components/evaluater.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/merger.py` & `vnerrant-1.0.1rc5/vnerrant/components/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/components/tokenizer.py` & `vnerrant-1.0.1rc5/vnerrant/components/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/config/errant_verbose.json` & `vnerrant-1.0.1rc5/vnerrant/config/errant_verbose.json`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/config/mapping_type_error.yaml` & `vnerrant-1.0.1rc5/vnerrant/config/mapping_type_error.yaml`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/constants.py` & `vnerrant-1.0.1rc5/vnerrant/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,18 +2,24 @@
 
 from dataclasses import dataclass
 from pathlib import Path
 
 from vnerrant.utils.utils import load_yml_file
 
 # Replace magic strings with constants
-MERGING_RULES = "rules"
-MERGING_ALL_SPLIT = "all-split"
-MERGING_ALL_MERGE = "all-merge"
-MERGING_ALL_EQUAL = "all-equal"
+@dataclass
+class MergeType:
+    """
+    Merge types.
+    """
+
+    RULES: str = "rules"
+    ALL_SPLIT: str = "all-split"
+    ALL_MERGE: str = "all-merge"
+    ALL_EQUAL: str = "all-equal"
 
 KEY_SPELL = "SPELLING"
 
 base_dir = Path(__file__).resolve().parent
 # Load the data from the YAML file into the dataclass
 MAPPING_TYPE_ERROR = load_yml_file(base_dir / "config" / "mapping_type_error.yaml")
 EXPLANATION_PATH = base_dir / "config" / "errant_verbose.json"
```

### Comparing `vnerrant-1.0.1rc4/vnerrant/metrics/criteria.py` & `vnerrant-1.0.1rc5/vnerrant/metrics/criteria.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/model/edit.py` & `vnerrant-1.0.1rc5/vnerrant/model/edit.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/run_cli.py` & `vnerrant-1.0.1rc5/vnerrant/run_cli.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/utils/edit_utils.py` & `vnerrant-1.0.1rc5/vnerrant/utils/edit_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from itertools import groupby
 from typing import List
 
-from vnerrant.model import Edit, EditCollection
+from vnerrant.model import Edit, EditCollection, EditElement
 
 
 def get_match_edits(alignment):
     """
     Get the match edits from an alignment.
     Args:
         alignment (Alignment): An Alignment object
@@ -44,72 +44,55 @@
 
         if edit.corrected.start_token != 0:
             edit.corrected.start_char = len("".join(cor_tokens[: edit.corrected.start_token]))
         if edit.corrected.end_token != 0:
             edit.corrected.end_char = len("".join(cor_tokens[: edit.corrected.end_token]))
 
 
+def _merge_edit_elements(text: str, first: EditElement, second: EditElement, inplace: str = "first") -> None:
+    """
+    Merge two Edit Elements objects.
+
+    Args:
+        text (str): The text of the EditElement objects
+        first (EditElement): An EditElement object
+        second (EditElement): An EditElement object
+        inplace (str): The object to be updated. Default is "first".
+
+    Returns: None
+    """
+    if inplace not in ["first", "second"]:
+        raise ValueError("inplace should be either 'first' or 'second'.")
+
+    if inplace == "second":
+        first, second = second, first
+
+    first.start_token = min(first.start_token, second.start_token)
+    first.start_char = min(first.start_char, second.start_char)
+    first.end_token = max(first.end_token, second.end_token)
+    first.end_char = max(first.end_char, second.end_char)
+    first.text = text[first.start_char: first.end_char]
+
+
 def merge_edit_collection_with_space_edits(edit_collection: EditCollection, space_edits: List[Edit]):
     """
     Merge the space edits to the edit collection.
     Args:
         edit_collection (EditCollection): An EditCollection object
         space_edits (list[Edit]): A list of Edit objects
     """
     # Merge SPACE with PUNCTUATION
     remained_edits = []
     for space_edit in space_edits:
         for edit in edit_collection.edits:
             if space_edit.original.end_char == edit.original.start_char:
-                # new_edit, edit
-                # [5, 5, ''], [5, 6, ',']
-                if (
-                    space_edit.original.start_char == space_edit.original.end_char
-                    and space_edit.original.end_char == edit.original.start_char
-                ):
-                    edit.corrected.start_token = space_edit.corrected.start_token
-                    edit.corrected.start_char = space_edit.corrected.start_char
-                    edit.corrected.text = edit_collection.cor[edit.corrected.start_char : edit.corrected.end_char]
-                    break
-
-                if (
-                    space_edit.original.start_char == space_edit.original.end_char
-                    and space_edit.original.start_char == edit.original.end_char
-                ):
-                    edit.corrected.end_token = space_edit.corrected.end_token
-                    edit.corrected.end_char = space_edit.corrected.end_char
-                    edit.corrected.text = edit_collection.cor[edit.corrected.start_char : edit.corrected.end_char]
-                    break
-
-                # [14, 15, ' '], [15, 15, '']
-                if (
-                    edit.original.start_char == edit.original.end_char
-                    and space_edit.original.end_char == edit.original.start_char
-                ):
-                    edit.original.start_token = space_edit.original.start_token
-                    edit.original.start_char = space_edit.original.start_char
-                    edit.original.text = edit_collection.orig[edit.original.start_char : edit.original.end_char]
-
-                    edit.corrected.start_token = space_edit.corrected.start_token
-                    edit.corrected.start_char = space_edit.corrected.start_char
-                    edit.corrected.text = edit_collection.cor[edit.corrected.start_char : edit.corrected.end_char]
-                    break
-
-                if (
-                    edit.original.start_char == edit.original.end_char
-                    and space_edit.original.start_char == edit.original.end_char
-                ):
-                    edit.original.end_token = space_edit.original.end_token
-                    edit.original.end_char = space_edit.original.end_char
-                    edit.original.text = edit_collection.orig[edit.original.start_char : edit.original.end_char]
-
-                    edit.corrected.end_token = space_edit.corrected.end_token
-                    edit.corrected.end_char = space_edit.corrected.end_char
-                    edit.corrected.text = edit_collection.cor[edit.corrected.start_char : edit.corrected.end_char]
-                    break
+                _merge_edit_elements(edit_collection.orig, edit.original, space_edit.original)
+                _merge_edit_elements(edit_collection.cor, edit.corrected, space_edit.corrected)
+                break
+
         else:
             remained_edits.append(space_edit)
 
     edit_collection.edits.extend(remained_edits)
 
 
 def update_operator(edits: List[Edit]):
@@ -124,26 +107,46 @@
         if orig_text and cor_text:
             edit.edit_type = "R" + edit.edit_type[1:]
         elif not orig_text and cor_text:
             edit.edit_type = "M" + edit.edit_type[1:]
         else:
             edit.edit_type = "U" + edit.edit_type[1:]
 
-def upadte_span_edit(edits: List[Edit]): # noqa D103
+def update_span_edit(edits: List[Edit]):  # noqa D103
     """
     Update the replace operator of the edits.
     Args:
         edits (list[Edit]): A list of Edit objects to be updated.
     """
+    def trim_text_span(text: str, start: int, end: int) -> tuple:
+        # Increment the start index to skip leading whitespace
+        for t in text[:]:
+            if not t.isspace():
+                break
+            start += 1
+        # Decrement the end index to skip trailing whitespace
+        for t in text[::-1]:
+            if not t.isspace():
+                break
+            end -= 1
+        stripped_text = text.strip()
+        return stripped_text, start, end
+
     for edit in edits:
-        edit.original.text = edit.original.tokens.text
-        edit.original.end_char = edit.original.start_char + len(edit.original.text)
-        edit.corrected.text = edit.corrected.tokens.text
-        edit.corrected.end_char = edit.corrected.start_char + len(edit.corrected.text)
-            
+        if edit.edit_type[0] == "R":
+            stripped_orig_text, start_orig, end_orig = trim_text_span(edit.original.text, edit.original.start_char, edit.original.end_char)
+            stripped_corr_text, start_corr, end_corr = trim_text_span(edit.corrected.text, edit.corrected.start_char, edit.corrected.end_char)
+            edit.original.text = stripped_orig_text
+            edit.original.start_char = start_orig
+            edit.original.end_char = end_orig
+            edit.corrected.text = stripped_corr_text
+            edit.corrected.start_char = start_corr
+            edit.corrected.end_char = end_corr
+
+
 def process_space_edit(edit: Edit) -> Edit:
     """
     Process the space edit.
     Args:
         edit (Edit): An Edit object to be processed.
 
     Returns: An Edit object after processing.
```

### Comparing `vnerrant-1.0.1rc4/vnerrant/utils/helper.py` & `vnerrant-1.0.1rc5/vnerrant/utils/helper.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/utils/pretty_results.py` & `vnerrant-1.0.1rc5/vnerrant/utils/pretty_results.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/utils/string_utils.py` & `vnerrant-1.0.1rc5/vnerrant/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant/utils/utils.py` & `vnerrant-1.0.1rc5/vnerrant/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc4/vnerrant.egg-info/PKG-INFO` & `vnerrant-1.0.1rc5/vnerrant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc4
+Version: 1.0.1rc5
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc4/vnerrant.egg-info/SOURCES.txt` & `vnerrant-1.0.1rc5/vnerrant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

