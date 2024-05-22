# Comparing `tmp/dataloader_gyqk-0.0.0.tar.gz` & `tmp/dataloader_gyqk-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dataloader_gyqk-0.0.0.tar", last modified: Wed May 22 10:36:03 2024, max compression
+gzip compressed data, was "dist/dataloader_gyqk-0.0.1.tar", last modified: Wed May 22 10:43:20 2024, max compression
```

## Comparing `dataloader_gyqk-0.0.0.tar` & `dataloader_gyqk-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:36:03.931681 dataloader_gyqk-0.0.0/
--rw-r--r--   0 guoxun    (1001) guoxun    (1001)      313 2024-05-22 10:36:03.931681 dataloader_gyqk-0.0.0/PKG-INFO
-drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:36:03.931681 dataloader_gyqk-0.0.0/dataloader_gyqk/
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:29:05.000000 dataloader_gyqk-0.0.0/dataloader_gyqk/__init__.py
--rw-r--r--   0 guoxun    (1001) guoxun    (1001)    12960 2024-05-22 10:29:12.000000 dataloader_gyqk-0.0.0/dataloader_gyqk/client.py
-drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:36:03.931681 dataloader_gyqk-0.0.0/dataloader_gyqk.egg-info/
--rw-r--r--   0 guoxun    (1001) guoxun    (1001)      313 2024-05-22 10:36:03.000000 dataloader_gyqk-0.0.0/dataloader_gyqk.egg-info/PKG-INFO
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)      218 2024-05-22 10:36:03.000000 dataloader_gyqk-0.0.0/dataloader_gyqk.egg-info/SOURCES.txt
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)        1 2024-05-22 10:36:03.000000 dataloader_gyqk-0.0.0/dataloader_gyqk.egg-info/dependency_links.txt
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)       16 2024-05-22 10:36:03.000000 dataloader_gyqk-0.0.0/dataloader_gyqk.egg-info/top_level.txt
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)       38 2024-05-22 10:36:03.931681 dataloader_gyqk-0.0.0/setup.cfg
--rw-rw-r--   0 guoxun    (1001) guoxun    (1001)      437 2024-05-22 10:35:37.000000 dataloader_gyqk-0.0.0/setup.py
+drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:43:20.386233 dataloader_gyqk-0.0.1/
+-rw-r--r--   0 guoxun    (1001) guoxun    (1001)      313 2024-05-22 10:43:20.386233 dataloader_gyqk-0.0.1/PKG-INFO
+drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:43:20.382233 dataloader_gyqk-0.0.1/dataloader_gyqk/
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)       27 2024-05-22 10:41:59.000000 dataloader_gyqk-0.0.1/dataloader_gyqk/__init__.py
+-rw-r--r--   0 guoxun    (1001) guoxun    (1001)    12960 2024-05-22 10:42:33.000000 dataloader_gyqk-0.0.1/dataloader_gyqk/client.py
+drwxrwxr-x   0 guoxun    (1001) guoxun    (1001)        0 2024-05-22 10:43:20.382233 dataloader_gyqk-0.0.1/dataloader_gyqk.egg-info/
+-rw-r--r--   0 guoxun    (1001) guoxun    (1001)      313 2024-05-22 10:43:20.000000 dataloader_gyqk-0.0.1/dataloader_gyqk.egg-info/PKG-INFO
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)      218 2024-05-22 10:43:20.000000 dataloader_gyqk-0.0.1/dataloader_gyqk.egg-info/SOURCES.txt
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)        1 2024-05-22 10:43:20.000000 dataloader_gyqk-0.0.1/dataloader_gyqk.egg-info/dependency_links.txt
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)       16 2024-05-22 10:43:20.000000 dataloader_gyqk-0.0.1/dataloader_gyqk.egg-info/top_level.txt
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)       38 2024-05-22 10:43:20.386233 dataloader_gyqk-0.0.1/setup.cfg
+-rw-rw-r--   0 guoxun    (1001) guoxun    (1001)      437 2024-05-22 10:43:07.000000 dataloader_gyqk-0.0.1/setup.py
```

### Comparing `dataloader_gyqk-0.0.0/dataloader_gyqk/client.py` & `dataloader_gyqk-0.0.1/dataloader_gyqk/client.py`

 * *Files identical despite different names*

