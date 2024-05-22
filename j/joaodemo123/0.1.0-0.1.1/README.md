# Comparing `tmp/joaodemo123-0.1.0.tar.gz` & `tmp/joaodemo123-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joaodemo123-0.1.0.tar", max compression
+gzip compressed data, was "joaodemo123-0.1.1.tar", max compression
```

## Comparing `joaodemo123-0.1.0.tar` & `joaodemo123-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2024-05-21 22:12:44.302317 joaodemo123-0.1.0/README.md
--rw-r--r--   0        0        0      312 2024-05-22 14:03:30.389479 joaodemo123-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2024-05-21 22:13:32.941075 joaodemo123-0.1.0/src/demo123/__init__.py
--rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 joaodemo123-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-21 22:12:44.302317 joaodemo123-0.1.1/README.md
+-rw-r--r--   0        0        0      525 2024-05-22 14:08:54.566476 joaodemo123-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-05-21 22:13:32.941075 joaodemo123-0.1.1/src/demo123/__init__.py
+-rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 joaodemo123-0.1.1/PKG-INFO
```

