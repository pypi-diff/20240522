# Comparing `tmp/flytekitplugins_async_fsspec-1.12.1b1.tar.gz` & `tmp/flytekitplugins_async_fsspec-1.12.1b2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_async_fsspec-1.12.1b1.tar", last modified: Thu May 16 22:53:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

