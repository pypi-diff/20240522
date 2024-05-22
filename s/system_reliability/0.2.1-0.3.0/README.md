# Comparing `tmp/system_reliability-0.2.1.tar.gz` & `tmp/system_reliability-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_reliability-0.2.1.tar", max compression
+gzip compressed data, was "system_reliability-0.3.0.tar", max compression
```

## Comparing `system_reliability-0.2.1.tar` & `system_reliability-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.2.1/README.md
--rw-r--r--   0        0        0      273 2024-05-22 05:27:37.583075 system_reliability-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3763 2024-05-22 05:27:22.575025 system_reliability-0.2.1/system_reliability/components/block.py
--rw-r--r--   0        0        0      410 2024-05-22 04:59:53.429535 system_reliability-0.2.1/system_reliability/components/component.py
--rw-r--r--   0        0        0     1187 2024-05-22 05:04:26.214077 system_reliability-0.2.1/system_reliability/components/element.py
--rw-r--r--   0        0        0      556 2024-05-22 05:16:50.736446 system_reliability-0.2.1/system_reliability/date.py
--rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.2.1/system_reliability/enums.py
--rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.2.1/system_reliability/exceptions.py
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.3.0/README.md
+-rw-r--r--   0        0        0      273 2024-05-22 05:30:32.263639 system_reliability-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3763 2024-05-22 05:27:22.575025 system_reliability-0.3.0/system_reliability/components/block.py
+-rw-r--r--   0        0        0      410 2024-05-22 04:59:53.429535 system_reliability-0.3.0/system_reliability/components/component.py
+-rw-r--r--   0        0        0     1187 2024-05-22 05:04:26.214077 system_reliability-0.3.0/system_reliability/components/element.py
+-rw-r--r--   0        0        0      556 2024-05-22 05:16:50.736446 system_reliability-0.3.0/system_reliability/date.py
+-rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.3.0/system_reliability/enums.py
+-rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.3.0/system_reliability/exceptions.py
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.3.0/PKG-INFO
```

### Comparing `system_reliability-0.2.1/system_reliability/components/block.py` & `system_reliability-0.3.0/system_reliability/components/block.py`

 * *Files identical despite different names*

### Comparing `system_reliability-0.2.1/system_reliability/components/element.py` & `system_reliability-0.3.0/system_reliability/components/element.py`

 * *Files identical despite different names*

### Comparing `system_reliability-0.2.1/system_reliability/date.py` & `system_reliability-0.3.0/system_reliability/date.py`

 * *Files identical despite different names*

