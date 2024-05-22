# Comparing `tmp/MARCIA-0.1.3.tar.gz` & `tmp/MARCIA-0.1.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/hadrien/Documents/MARCIA/dist/tmp5qngn9de/MARCIA-0.1.3.tar", last modified: Sun May  9 09:26:46 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

