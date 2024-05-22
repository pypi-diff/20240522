# Comparing `tmp/fnschool-20240520.81248.848.tar.gz` & `tmp/fnschool-20240523.80109.809-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240520.81248.848.tar", last modified: Mon May 20 04:48:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

