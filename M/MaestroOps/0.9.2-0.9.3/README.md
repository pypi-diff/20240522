# Comparing `tmp/maestroops-0.9.2.tar.gz` & `tmp/maestroops-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestroops-0.9.2.tar", last modified: Mon May 13 14:53:05 2024, max compression
+gzip compressed data, was "maestroops-0.9.3.tar", last modified: Wed May 22 13:18:48 2024, max compression
```

## Comparing `maestroops-0.9.2.tar` & `maestroops-0.9.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.661196 maestroops-0.9.2/
--rw-r--r--   0 mperttula   (502) staff       (20)     1081 2024-02-27 16:30:05.000000 maestroops-0.9.2/LICENSE
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.659440 maestroops-0.9.2/MaestroOps.egg-info/
--rw-r--r--   0 mperttula   (502) staff       (20)      282 2024-05-13 14:53:05.000000 maestroops-0.9.2/MaestroOps.egg-info/PKG-INFO
--rw-r--r--   0 mperttula   (502) staff       (20)      648 2024-05-13 14:53:05.000000 maestroops-0.9.2/MaestroOps.egg-info/SOURCES.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-13 14:53:05.000000 maestroops-0.9.2/MaestroOps.egg-info/dependency_links.txt
--rw-r--r--   0 mperttula   (502) staff       (20)       14 2024-05-13 14:53:05.000000 maestroops-0.9.2/MaestroOps.egg-info/requires.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        8 2024-05-13 14:53:05.000000 maestroops-0.9.2/MaestroOps.egg-info/top_level.txt
--rw-r--r--   0 mperttula   (502) staff       (20)      282 2024-05-13 14:53:05.660393 maestroops-0.9.2/PKG-INFO
--rw-r--r--   0 mperttula   (502) staff       (20)      115 2024-02-27 16:30:05.000000 maestroops-0.9.2/README.md
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.614540 maestroops-0.9.2/maestro/
--rw-r--r--   0 mperttula   (502) staff       (20)       46 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/__init__.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.626829 maestroops-0.9.2/maestro/aws/
--rw-r--r--   0 mperttula   (502) staff       (20)       84 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)    30006 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/cf_stack.py
--rw-r--r--   0 mperttula   (502) staff       (20)    20046 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/dynamodb.py
--rw-r--r--   0 mperttula   (502) staff       (20)     9237 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/parameter_store.py
--rw-r--r--   0 mperttula   (502) staff       (20)    11716 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/r53.py
--rw-r--r--   0 mperttula   (502) staff       (20)    13344 2024-04-23 19:13:16.000000 maestroops-0.9.2/maestro/aws/s3.py
--rw-r--r--   0 mperttula   (502) staff       (20)    10701 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/aws/ssm_documents.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.632660 maestroops-0.9.2/maestro/core/
--rw-r--r--   0 mperttula   (502) staff       (20)       39 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/core/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     1487 2024-02-27 16:30:09.000000 maestroops-0.9.2/maestro/core/execute.py
--rw-r--r--   0 mperttula   (502) staff       (20)     2554 2024-02-27 16:30:09.000000 maestroops-0.9.2/maestro/core/ioc.py
--rw-r--r--   0 mperttula   (502) staff       (20)     4583 2024-02-27 16:30:09.000000 maestroops-0.9.2/maestro/core/module.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.651585 maestroops-0.9.2/maestro/jenkins/
--rw-r--r--   0 mperttula   (502) staff       (20)       19 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/jenkins/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     6683 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/jenkins/jobs.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 14:53:05.658009 maestroops-0.9.2/maestro/tools/
--rw-r--r--   0 mperttula   (502) staff       (20)       37 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/tools/__init__.py
--rw-r--r--   0 mperttula   (502) staff       (20)     1713 2024-04-23 19:13:16.000000 maestroops-0.9.2/maestro/tools/file.py
--rw-r--r--   0 mperttula   (502) staff       (20)      742 2024-02-27 16:30:05.000000 maestroops-0.9.2/maestro/tools/os_tools.py
--rw-r--r--   0 mperttula   (502) staff       (20)     3425 2024-02-27 16:30:09.000000 maestroops-0.9.2/maestro/tools/path.py
--rw-r--r--   0 mperttula   (502) staff       (20)      423 2024-02-27 16:30:09.000000 maestroops-0.9.2/maestro/tools/string.py
--rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-13 14:53:05.661345 maestroops-0.9.2/setup.cfg
--rw-r--r--   0 mperttula   (502) staff       (20)      421 2024-05-13 14:51:19.000000 maestroops-0.9.2/setup.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.232541 maestroops-0.9.3/
+-rw-r--r--   0 mperttula   (502) staff       (20)     1081 2024-02-27 16:30:05.000000 maestroops-0.9.3/LICENSE
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.230982 maestroops-0.9.3/MaestroOps.egg-info/
+-rw-r--r--   0 mperttula   (502) staff       (20)      282 2024-05-22 13:18:48.000000 maestroops-0.9.3/MaestroOps.egg-info/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      648 2024-05-22 13:18:48.000000 maestroops-0.9.3/MaestroOps.egg-info/SOURCES.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-22 13:18:48.000000 maestroops-0.9.3/MaestroOps.egg-info/dependency_links.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       14 2024-05-22 13:18:48.000000 maestroops-0.9.3/MaestroOps.egg-info/requires.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        8 2024-05-22 13:18:48.000000 maestroops-0.9.3/MaestroOps.egg-info/top_level.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)      282 2024-05-22 13:18:48.231719 maestroops-0.9.3/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      115 2024-02-27 16:30:05.000000 maestroops-0.9.3/README.md
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.211242 maestroops-0.9.3/maestro/
+-rw-r--r--   0 mperttula   (502) staff       (20)       46 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/__init__.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.219461 maestroops-0.9.3/maestro/aws/
+-rw-r--r--   0 mperttula   (502) staff       (20)       84 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    30006 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/cf_stack.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    20046 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/dynamodb.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     9237 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/parameter_store.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    11716 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/r53.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    13218 2024-05-22 13:04:47.000000 maestroops-0.9.3/maestro/aws/s3.py
+-rw-r--r--   0 mperttula   (502) staff       (20)    10701 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/aws/ssm_documents.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.223281 maestroops-0.9.3/maestro/core/
+-rw-r--r--   0 mperttula   (502) staff       (20)       39 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/core/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1487 2024-02-27 16:30:09.000000 maestroops-0.9.3/maestro/core/execute.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     2554 2024-02-27 16:30:09.000000 maestroops-0.9.3/maestro/core/ioc.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     4583 2024-02-27 16:30:09.000000 maestroops-0.9.3/maestro/core/module.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.225176 maestroops-0.9.3/maestro/jenkins/
+-rw-r--r--   0 mperttula   (502) staff       (20)       19 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/jenkins/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     6683 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/jenkins/jobs.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-22 13:18:48.230075 maestroops-0.9.3/maestro/tools/
+-rw-r--r--   0 mperttula   (502) staff       (20)       37 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/tools/__init__.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1713 2024-04-23 19:13:16.000000 maestroops-0.9.3/maestro/tools/file.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      742 2024-02-27 16:30:05.000000 maestroops-0.9.3/maestro/tools/os_tools.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     3425 2024-02-27 16:30:09.000000 maestroops-0.9.3/maestro/tools/path.py
+-rw-r--r--   0 mperttula   (502) staff       (20)      423 2024-02-27 16:30:09.000000 maestroops-0.9.3/maestro/tools/string.py
+-rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-22 13:18:48.232714 maestroops-0.9.3/setup.cfg
+-rw-r--r--   0 mperttula   (502) staff       (20)      421 2024-05-22 13:14:35.000000 maestroops-0.9.3/setup.py
```

### Comparing `maestroops-0.9.2/LICENSE` & `maestroops-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/MaestroOps.egg-info/SOURCES.txt` & `maestroops-0.9.3/MaestroOps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/aws/cf_stack.py` & `maestroops-0.9.3/maestro/aws/cf_stack.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/aws/dynamodb.py` & `maestroops-0.9.3/maestro/aws/dynamodb.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/aws/parameter_store.py` & `maestroops-0.9.3/maestro/aws/parameter_store.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/aws/r53.py` & `maestroops-0.9.3/maestro/aws/r53.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/aws/s3.py` & `maestroops-0.9.3/maestro/aws/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,29 +50,28 @@
         # Iterate over objects, and append only ones that match lower case and don't end with '/'
         for obj in remote_bucket.objects.all():
             if obj.key.lower().startswith(prefix.lower()) and not obj.key.endswith("/"):
                 if sha256:
                     try:
                         objsum = s3client.head_object(Bucket=bucket, Key=obj.key, ChecksumMode='ENABLED')['ResponseMetadata']['HTTPHeaders']["x-amz-checksum-sha256"]
                     except Exception:
-                        raise ChecksumFailure(f"Unable head object for checksum. Please verify sha256 exists on object {bucket}/{obj.key}")
+                        print(f"Cannot read checksum. Please verify sha256 exists on object {bucket}/{obj.key}")
                         objsum = "unknown"
                 else:
                     objsum = s3client.get_object(Bucket=bucket, Key=obj.key)["ETag"][1:-1]
                 files.append((obj, objsum))
     else:  # If we're case sensitive, just use the filter
         files = remote_bucket.objects.filter(Prefix=prefix)
         sum_files = list()
         for f in files:
             if sha256:
                 try:
                     objsum = s3client.head_object(Bucket=bucket, Key=f.key, ChecksumMode='ENABLED')['ResponseMetadata']['HTTPHeaders']["x-amz-checksum-sha256"]
                 except Exception:
-                    raise ChecksumFailure(
-                        f"Unable head object for checksum. Please verify sha256 exists on object {bucket}/{obj.key}")
+                    print(f"Cannot read checksum. Please verify sha256 exists on object {bucket}/{f.key}")
                     objsum = "unknown"
             else:
                 objsum = s3client.get_object_attributes(Bucket=bucket, Key=f.key, ObjectAttributes=['ETag'])[1:-1]
             sum_files.append((f, objsum))
         files = sum_files
 
     return files
@@ -154,18 +153,14 @@
         else:
             raise e
 
 
 class DownloadError(Exception):
     pass
 
-class ChecksumFailure(Exception):
-    pass
-
-
 # MODULES #
 
 BUCKET_KEYS = ["b", "bucket"]
 CASE_INSENSITIVE_KEYS = ["i", "case-insensitive"]
 DESTINATION_KEYS = ["d", "destination"]
 PATH_KEYS = ["p", "prefix"]
 REGION_KEYS = ["r", "region"]
```

### Comparing `maestroops-0.9.2/maestro/aws/ssm_documents.py` & `maestroops-0.9.3/maestro/aws/ssm_documents.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/core/execute.py` & `maestroops-0.9.3/maestro/core/execute.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/core/ioc.py` & `maestroops-0.9.3/maestro/core/ioc.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/core/module.py` & `maestroops-0.9.3/maestro/core/module.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/jenkins/jobs.py` & `maestroops-0.9.3/maestro/jenkins/jobs.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/tools/file.py` & `maestroops-0.9.3/maestro/tools/file.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/tools/os_tools.py` & `maestroops-0.9.3/maestro/tools/os_tools.py`

 * *Files identical despite different names*

### Comparing `maestroops-0.9.2/maestro/tools/path.py` & `maestroops-0.9.3/maestro/tools/path.py`

 * *Files identical despite different names*

