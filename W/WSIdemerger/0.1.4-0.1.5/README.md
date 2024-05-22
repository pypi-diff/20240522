# Comparing `tmp/wsidemerger-0.1.4.tar.gz` & `tmp/WSIdemerger-0.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.4.tar", last modified: Tue May 21 12:22:50 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

