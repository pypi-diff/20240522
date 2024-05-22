# Comparing `tmp/go_console-0.0.2.tar.gz` & `tmp/go_console-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.0.2.tar", max compression
+gzip compressed data, was "go_console-0.0.3.tar", max compression
```

## Comparing `go_console-0.0.2.tar` & `go_console-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       23 2024-05-22 08:31:06.776023 go_console-0.0.2/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.2/go_console/api.go
--rw-r--r--   0        0        0     2840 2024-05-22 08:30:48.093742 go_console-0.0.2/go_console/gen.py
--rw-r--r--   0        0        0      300 2024-05-22 08:31:11.533292 go_console-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-22 08:32:11.914803 go_console-0.0.3/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.3/go_console/api.go
+-rw-r--r--   0        0        0     2840 2024-05-22 08:30:48.093742 go_console-0.0.3/go_console/gen.py
+-rw-r--r--   0        0        0      300 2024-05-22 08:32:18.002720 go_console-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.3/PKG-INFO
```

### Comparing `go_console-0.0.2/go_console/api.go` & `go_console-0.0.3/go_console/api.go`

 * *Files identical despite different names*

### Comparing `go_console-0.0.2/go_console/gen.py` & `go_console-0.0.3/go_console/gen.py`

 * *Files identical despite different names*

