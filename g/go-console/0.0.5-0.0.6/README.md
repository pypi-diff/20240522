# Comparing `tmp/go_console-0.0.5.tar.gz` & `tmp/go_console-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.0.5.tar", max compression
+gzip compressed data, was "go_console-0.0.6.tar", max compression
```

## Comparing `go_console-0.0.5.tar` & `go_console-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2867 2024-05-22 08:36:59.876869 go_console-0.0.5/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.5/go_console/api.go
--rw-r--r--   0        0        0      300 2024-05-22 08:37:13.660764 go_console-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2904 2024-05-22 08:40:01.576182 go_console-0.0.6/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.6/go_console/api.go
+-rw-r--r--   0        0        0      300 2024-05-22 08:40:22.869044 go_console-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.6/PKG-INFO
```

### Comparing `go_console-0.0.5/go_console/__main__.py` & `go_console-0.0.6/go_console/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pathlib
 import subprocess
 import time
 from concurrent.futures import ThreadPoolExecutor
 from shutil import which
 import re
+import importlib.resources
 
 
 def main():
     print(123)
 
     root = os.getcwd()
 
@@ -55,16 +56,15 @@
     with ThreadPoolExecutor(max_workers=10) as executor:
         futures = [executor.submit(extract_files, pack) for pack in dirs]
 
         for f in futures:
             f.result()
 
     with open(extract_dir.joinpath('api.go'), 'w') as f:
-        with open('./api.go') as rf:
-            f.write(rf.read())
+        f.write(importlib.resources.open_text('go_console', 'api.go').read())
     print('生成完成')
     for file in os.listdir(extract_dir):
         res = subprocess.run(
             f'go vet {extract_dir.joinpath(file)}',
             shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE
         ).stderr.decode().strip()
         for line in res.splitlines():
```

### Comparing `go_console-0.0.5/go_console/api.go` & `go_console-0.0.6/go_console/api.go`

 * *Files identical despite different names*

