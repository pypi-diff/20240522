# Comparing `tmp/wagtail_guide-2.1.0.tar.gz` & `tmp/wagtail_guide-2.2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_guide-2.1.0.tar", last modified: Mon Mar 11 08:59:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

