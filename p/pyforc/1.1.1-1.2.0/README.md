# Comparing `tmp/PyFORC-1.1.1.tar.gz` & `tmp/pyforc-1.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFORC-1.1.1.tar", last modified: Wed Feb 23 00:48:58 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

