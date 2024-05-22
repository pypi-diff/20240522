# Comparing `tmp/TlseHypDataSet-0.0.3.tar.gz` & `tmp/TlseHypDataSet-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/rothor/Documents/ONERA/code/3A/TlseHypDataSet/dist/.tmp-l1wi4arv/TlseHypDataSet-0.0.3.tar", last modified: Sat Nov 25 15:26:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

