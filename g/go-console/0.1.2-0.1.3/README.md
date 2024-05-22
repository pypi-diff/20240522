# Comparing `tmp/go_console-0.1.2.tar.gz` & `tmp/go_console-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.1.2.tar", max compression
+gzip compressed data, was "go_console-0.1.3.tar", max compression
```

## Comparing `go_console-0.1.2.tar` & `go_console-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3015 2024-05-22 08:50:12.393830 go_console-0.1.2/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.1.2/go_console/api.go
--rw-r--r--   0        0        0      304 2024-05-22 08:54:33.342712 go_console-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 go_console-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3032 2024-05-22 08:59:34.385950 go_console-0.1.3/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.1.3/go_console/api.go
+-rw-r--r--   0        0        0      304 2024-05-22 08:59:42.595840 go_console-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 go_console-0.1.3/PKG-INFO
```

### Comparing `go_console-0.1.2/go_console/__main__.py` & `go_console-0.1.3/go_console/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     if not extract_dir.exists():
         extract_dir.mkdir()
     else:
         print("目录extract已经存在")
 
     if which('yaegi') is None:
         print('未安装yaegi\ngo install github.com/traefik/yaegi/cmd/yaegi@latest')
+        exit(-1)
 
     def list_directories(path):
         for entry in os.scandir(path):
             if entry.is_dir():
                 if any(x.endswith('.go') for x in os.listdir(entry.path)):
                     dirs.append(entry.path)
                 list_directories(entry.path)
```

### Comparing `go_console-0.1.2/go_console/api.go` & `go_console-0.1.3/go_console/api.go`

 * *Files identical despite different names*

