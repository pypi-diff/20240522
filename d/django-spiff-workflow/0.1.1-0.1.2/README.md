# Comparing `tmp/django-spiff-workflow-0.1.1.tar.gz` & `tmp/django_spiff_workflow-0.1.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-spiff-workflow-0.1.1.tar", last modified: Mon May 13 03:59:18 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

