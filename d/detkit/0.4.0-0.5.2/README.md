# Comparing `tmp/detkit-0.4.0.tar.gz` & `tmp/detkit-0.5.2-pp39-pypy39_pp73-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detkit-0.4.0.tar", last modified: Mon Apr 22 10:22:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

