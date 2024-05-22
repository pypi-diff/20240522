# Comparing `tmp/go_console-0.0.6.tar.gz` & `tmp/go_console-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.0.6.tar", max compression
+gzip compressed data, was "go_console-0.1.0.tar", max compression
```

## Comparing `go_console-0.0.6.tar` & `go_console-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2904 2024-05-22 08:40:01.576182 go_console-0.0.6/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.6/go_console/api.go
--rw-r--r--   0        0        0      300 2024-05-22 08:40:22.869044 go_console-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3024 2024-05-22 08:46:22.591483 go_console-0.1.0/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.1.0/go_console/api.go
+-rw-r--r--   0        0        0      300 2024-05-22 08:46:33.592856 go_console-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.1.0/PKG-INFO
```

### Comparing `go_console-0.0.6/go_console/__main__.py` & `go_console-0.1.0/go_console/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from concurrent.futures import ThreadPoolExecutor
 from shutil import which
 import re
 import importlib.resources
 
 
 def main():
-    print(123)
-
     root = os.getcwd()
 
     if pathlib.Path(root).joinpath('go.mod').exists():
         with open(pathlib.Path(root).joinpath('go.mod')) as f:
             for line in f:
                 m = re.search(r'^module\s+(\S+)', line)
                 if m:
@@ -47,15 +45,15 @@
     def extract_files(pack):
         os.chdir(extract_dir)
         time.sleep(1)
         res = subprocess.run(f'yaegi extract {package_name + pack[len(root):]}', shell=True, stdout=subprocess.PIPE, )
         print(pack[len(root):] + ' done')
         return res.stdout.decode().strip()
 
-    # list_directories(root)
+    list_directories(root)
 
     with ThreadPoolExecutor(max_workers=10) as executor:
         futures = [executor.submit(extract_files, pack) for pack in dirs]
 
         for f in futures:
             f.result()
 
@@ -83,11 +81,16 @@
             for k, v in tips.items():
                 if k in info:
                     print(v)
                     break
             else:
                 print('未知错误')
     print('!!!------------------------------------!!!')
-    print(f'请在main包引入\n_ "{package_name}/extract"')
+    print(f'请在main包使用\nimport "{package_name}/extract"')
+    print("console := extract.New()")
+    print("""
+console.Init(map[string]any{
+    "key": value... // 需要引入的遍历
+})""")
 
 
 main()
```

### Comparing `go_console-0.0.6/go_console/api.go` & `go_console-0.1.0/go_console/api.go`

 * *Files identical despite different names*

