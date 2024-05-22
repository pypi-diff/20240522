# Comparing `tmp/airbyte_source_twilio-0.11.3.tar.gz` & `tmp/airbyte_source_twilio-0.11.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_twilio-0.11.3.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

