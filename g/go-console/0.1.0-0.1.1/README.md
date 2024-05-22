# Comparing `tmp/go_console-0.1.0.tar.gz` & `tmp/go_console-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "go_console-0.1.0.tar", max compression
+gzip compressed data, was "go_console-0.1.1.tar", max compression
```

## Comparing `go_console-0.1.0.tar` & `go_console-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3024 2024-05-22 08:46:22.591483 go_console-0.1.0/go_console/__main__.py
--rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.1.0/go_console/api.go
--rw-r--r--   0        0        0      300 2024-05-22 08:46:33.592856 go_console-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3015 2024-05-22 08:50:12.393830 go_console-0.1.1/go_console/__main__.py
+-rw-r--r--   0        0        0     2937 2024-05-22 08:22:21.654556 go_console-0.1.1/go_console/api.go
+-rw-r--r--   0        0        0      305 2024-05-22 08:50:26.456871 go_console-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      350 1970-01-01 00:00:00.000000 go_console-0.1.1/PKG-INFO
```

### Comparing `go_console-0.1.0/go_console/__main__.py` & `go_console-0.1.1/go_console/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,10 +87,7 @@
     print('!!!------------------------------------!!!')
     print(f'请在main包使用\nimport "{package_name}/extract"')
     print("console := extract.New()")
     print("""
 console.Init(map[string]any{
     "key": value... // 需要引入的遍历
 })""")
-
-
-main()
```

### Comparing `go_console-0.1.0/go_console/api.go` & `go_console-0.1.1/go_console/api.go`

 * *Files identical despite different names*

