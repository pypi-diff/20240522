# Comparing `tmp/sp_lib-1.0.0.tar.gz` & `tmp/sp_lib-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sp_lib-1.0.0.tar", last modified: Tue Apr  2 10:20:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

