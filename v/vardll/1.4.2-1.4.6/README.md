# Comparing `tmp/vardll-1.4.2.tar.gz` & `tmp/vardll-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vardll-1.4.2.tar", last modified: Wed May 15 20:42:33 2024, max compression
+gzip compressed data, was "vardll-1.4.6.tar", last modified: Wed May 22 20:46:56 2024, max compression
```

## Comparing `vardll-1.4.2.tar` & `vardll-1.4.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 20:42:33.159302 vardll-1.4.2/
--rw-rw-rw-   0        0        0      280 2024-05-15 20:42:33.156304 vardll-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 vardll-1.4.2/license
--rw-rw-rw-   0        0        0       42 2024-05-15 20:42:33.160303 vardll-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0      507 2024-05-15 20:36:05.000000 vardll-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 20:42:33.153760 vardll-1.4.2/vardll.egg-info/
--rw-rw-rw-   0        0        0      280 2024-05-15 20:42:32.000000 vardll-1.4.2/vardll.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-05-15 20:42:32.000000 vardll-1.4.2/vardll.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:42:32.000000 vardll-1.4.2/vardll.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-15 20:42:32.000000 vardll-1.4.2/vardll.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 20:42:32.000000 vardll-1.4.2/vardll.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:46:56.245805 vardll-1.4.6/
+-rw-rw-rw-   0        0        0      280 2024-05-22 20:46:56.242224 vardll-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1103 2024-05-15 20:32:47.000000 vardll-1.4.6/license
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:46:56.246772 vardll-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      507 2024-05-22 20:46:42.000000 vardll-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:46:56.239635 vardll-1.4.6/vardll.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:46:55.000000 vardll-1.4.6/vardll.egg-info/top_level.txt
```

### Comparing `vardll-1.4.2/license` & `vardll-1.4.6/license`

 * *Files identical despite different names*

