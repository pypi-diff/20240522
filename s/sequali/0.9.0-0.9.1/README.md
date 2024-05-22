# Comparing `tmp/sequali-0.9.0.tar.gz` & `tmp/sequali-0.9.1-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequali-0.9.0.tar", last modified: Tue May 21 11:38:35 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

