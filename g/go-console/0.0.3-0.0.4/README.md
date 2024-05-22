# Comparing `tmp/go_console-0.0.3.tar.gz` & `tmp/go_console-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.0.3.tar", max compression
+gzip compressed data, was "go_console-0.0.4.tar", max compression
```

## Comparing `go_console-0.0.3.tar` & `go_console-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       39 2024-05-22 08:32:11.914803 go_console-0.0.3/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.3/go_console/api.go
--rw-r--r--   0        0        0     2840 2024-05-22 08:30:48.093742 go_console-0.0.3/go_console/gen.py
--rw-r--r--   0        0        0      300 2024-05-22 08:32:18.002720 go_console-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2842 2024-05-22 08:34:32.928161 go_console-0.0.4/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.0.4/go_console/api.go
+-rw-r--r--   0        0        0      300 2024-05-22 08:34:37.059901 go_console-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.0.4/PKG-INFO
```

### Comparing `go_console-0.0.3/go_console/api.go` & `go_console-0.0.4/go_console/api.go`

 * *Files identical despite different names*

### Comparing `go_console-0.0.3/go_console/gen.py` & `go_console-0.0.4/go_console/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def extract_files(pack):
         os.chdir(extract_dir)
         time.sleep(1)
         res = subprocess.run(f'yaegi extract {package_name + pack[len(root):]}', shell=True, stdout=subprocess.PIPE, )
         print(pack[len(root):] + ' done')
         return res.stdout.decode().strip()
 
-    list_directories(root)
+    # list_directories(root)
 
     with ThreadPoolExecutor(max_workers=10) as executor:
         futures = [executor.submit(extract_files, pack) for pack in dirs]
 
         for f in futures:
             f.result()
```

