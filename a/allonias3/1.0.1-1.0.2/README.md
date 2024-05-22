# Comparing `tmp/allonias3-1.0.1.tar.gz` & `tmp/allonias3-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allonias3-1.0.1.tar", max compression
+gzip compressed data, was "allonias3-1.0.2.tar", max compression
```

## Comparing `allonias3-1.0.1.tar` & `allonias3-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3202 2024-05-15 09:15:12.944654 allonias3-1.0.1/README.md
--rw-r--r--   0        0        0      830 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/__init__.py
--rw-r--r--   0        0        0    42274 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/base_path.py
--rw-r--r--   0        0        0        0 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/boto/__init__.py
--rw-r--r--   0        0        0    20703 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/boto/boto_path.py
--rw-r--r--   0        0        0     2265 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/configs.py
--rw-r--r--   0        0        0        0 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/encoder_decoder/__init__.py
--rw-r--r--   0        0        0    23840 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/encoder_decoder/advanced.py
--rw-r--r--   0        0        0     5282 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/encoder_decoder/basic.py
--rw-r--r--   0        0        0        0 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/__init__.py
--rw-r--r--   0        0        0     1167 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/class_property.py
--rw-r--r--   0        0        0      882 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/enums.py
--rw-r--r--   0        0        0     1412 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/getattr_safe_property.py
--rw-r--r--   0        0        0     8797 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/responses.py
--rw-r--r--   0        0        0     4460 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/helpers/utils.py
--rw-r--r--   0        0        0        0 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/minio/__init__.py
--rw-r--r--   0        0        0     2532 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/minio/helpers.py
--rw-r--r--   0        0        0    21626 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/minio/minio_path.py
--rw-r--r--   0        0        0     2938 2024-05-15 09:15:12.944654 allonias3-1.0.1/allonias3/s3_path.py
--rw-r--r--   0        0        0     4371 2024-05-15 09:16:38.056723 allonias3-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 allonias3-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3202 2024-05-22 14:07:19.499562 allonias3-1.0.2/README.md
+-rw-r--r--   0        0        0      830 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/__init__.py
+-rw-r--r--   0        0        0    42274 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/base_path.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/boto/__init__.py
+-rw-r--r--   0        0        0    20956 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/boto/boto_path.py
+-rw-r--r--   0        0        0     2265 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/configs.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/encoder_decoder/__init__.py
+-rw-r--r--   0        0        0    23840 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/encoder_decoder/advanced.py
+-rw-r--r--   0        0        0     5282 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/encoder_decoder/basic.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/helpers/__init__.py
+-rw-r--r--   0        0        0     1167 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/helpers/class_property.py
+-rw-r--r--   0        0        0      882 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/helpers/enums.py
+-rw-r--r--   0        0        0     1412 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/helpers/getattr_safe_property.py
+-rw-r--r--   0        0        0     8797 2024-05-22 14:07:19.499562 allonias3-1.0.2/allonias3/helpers/responses.py
+-rw-r--r--   0        0        0     4460 2024-05-22 14:07:19.503562 allonias3-1.0.2/allonias3/helpers/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:07:19.503562 allonias3-1.0.2/allonias3/minio/__init__.py
+-rw-r--r--   0        0        0     2532 2024-05-22 14:07:19.503562 allonias3-1.0.2/allonias3/minio/helpers.py
+-rw-r--r--   0        0        0    21927 2024-05-22 14:07:19.503562 allonias3-1.0.2/allonias3/minio/minio_path.py
+-rw-r--r--   0        0        0     2938 2024-05-22 14:07:19.503562 allonias3-1.0.2/allonias3/s3_path.py
+-rw-r--r--   0        0        0     4371 2024-05-22 14:09:02.655672 allonias3-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4767 1970-01-01 00:00:00.000000 allonias3-1.0.2/PKG-INFO
```

### Comparing `allonias3-1.0.1/README.md` & `allonias3-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/__init__.py` & `allonias3-1.0.2/allonias3/__init__.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/base_path.py` & `allonias3-1.0.2/allonias3/base_path.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/boto/boto_path.py` & `allonias3-1.0.2/allonias3/boto/boto_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,19 +79,24 @@
                 raise NotADirectoryError(
                     f"Bucket {bucket} does not exist."
                 ) from error
             cls._KEY = key
 
     def _check_existing_type(self):
         try:
-            existing_type = (
-                self.client.head_object(Bucket=self.bucket, Key=str(self))
-                .get("Metadata", {})
-                .get("type", "unknown")
-            )
+            metadata = self.client.head_object(
+                Bucket=self.bucket, Key=str(self)
+            ).get("Metadata", {})
+            existing_type = metadata.get("x-amz-meta-type")
+            if not existing_type:
+                existing_type = metadata.get("type")
+            if not existing_type:
+                existing_type = metadata.get("object_type")
+            if not existing_type:
+                existing_type = "unknown"
             if existing_type != self.object_type:
                 raise TypeError(
                     f"{self.str_persistent} {self} already exists with type "
                     f"'{existing_type}'."
                 )
         except botocore.exceptions.ClientError as error:
             if (
```

### Comparing `allonias3-1.0.1/allonias3/configs.py` & `allonias3-1.0.2/allonias3/configs.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/encoder_decoder/advanced.py` & `allonias3-1.0.2/allonias3/encoder_decoder/advanced.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/encoder_decoder/basic.py` & `allonias3-1.0.2/allonias3/encoder_decoder/basic.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/helpers/class_property.py` & `allonias3-1.0.2/allonias3/helpers/class_property.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/helpers/enums.py` & `allonias3-1.0.2/allonias3/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/helpers/getattr_safe_property.py` & `allonias3-1.0.2/allonias3/helpers/getattr_safe_property.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/helpers/responses.py` & `allonias3-1.0.2/allonias3/helpers/responses.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/helpers/utils.py` & `allonias3-1.0.2/allonias3/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/minio/helpers.py` & `allonias3-1.0.2/allonias3/minio/helpers.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/allonias3/minio/minio_path.py` & `allonias3-1.0.2/allonias3/minio/minio_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,22 @@
         return (
             self.client.get_bucket_versioning(bucket_name=self.bucket).status
             == "Enabled"
         )
 
     def _check_existing_type(self):
         try:
-            if (existing_type := self.metadata.get("type")) != self.object_type:
+            existing_type = self.metadata.get("x-amz-meta-type")
+            if not existing_type:
+                existing_type = self.metadata.get("type")
+            if not existing_type:
+                existing_type = self.metadata.get("object_type")
+            if not existing_type:
+                existing_type = "unknown"
+            if existing_type != self.object_type:
                 raise TypeError(
                     f"{self.str_persistent} {self} already exists with type "
                     f"'{existing_type}'."
                 )
         except S3Error as error:
             if error.code == "NoSuchKey":
                 # File does not exist, so no type conflict
```

### Comparing `allonias3-1.0.1/allonias3/s3_path.py` & `allonias3-1.0.2/allonias3/s3_path.py`

 * *Files identical despite different names*

### Comparing `allonias3-1.0.1/pyproject.toml` & `allonias3-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "allonias3"
-version = "1.0.1"
+version = "1.0.2"
 description = "Class to interact with S3 in a similar fashion as pathlib.Path"
 authors = ["ALLONIA"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 alloniaconfigs = "^1.1.0"
 python = "^3.9"
```

### Comparing `allonias3-1.0.1/PKG-INFO` & `allonias3-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allonias3
-Version: 1.0.1
+Version: 1.0.2
 Summary: Class to interact with S3 in a similar fashion as pathlib.Path
 Author: ALLONIA
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

