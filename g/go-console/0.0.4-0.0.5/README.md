# Comparing `tmp/go_console-0.0.4.tar.gz` & `tmp/go_console-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.0.4.tar", max compression
+gzip compressed data, was "go_console-0.0.5.tar", max compression
```

## Comparing `go_console-0.0.4.tar` & `go_console-0.0.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2842 2024-05-22 08:34:32.928161 go_console-0.0.4/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.4/go_console/api.go
--rw-r--r--   0        0        0      300 2024-05-22 08:34:37.059901 go_console-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2867 2024-05-22 08:36:59.876869 go_console-0.0.5/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.5/go_console/api.go
+-rw-r--r--   0        0        0      300 2024-05-22 08:37:13.660764 go_console-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.5/PKG-INFO
```

### Comparing `go_console-0.0.4/go_console/__main__.py` & `go_console-0.0.5/go_console/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import time
 from concurrent.futures import ThreadPoolExecutor
 from shutil import which
 import re
 
 
 def main():
+    print(123)
+
     root = os.getcwd()
 
     if pathlib.Path(root).joinpath('go.mod').exists():
         with open(pathlib.Path(root).joinpath('go.mod')) as f:
             for line in f:
                 m = re.search(r'^module\s+(\S+)', line)
                 if m:
@@ -82,7 +84,10 @@
                 if k in info:
                     print(v)
                     break
             else:
                 print('未知错误')
     print('!!!------------------------------------!!!')
     print(f'请在main包引入\n_ "{package_name}/extract"')
+
+
+main()
```

### Comparing `go_console-0.0.4/go_console/api.go` & `go_console-0.0.5/go_console/api.go`

 * *Files identical despite different names*

