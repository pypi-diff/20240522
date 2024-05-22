# Comparing `tmp/hmd_cli_docker-0.1.132-py3-none-any.whl.zip` & `tmp/hmd_cli_docker-0.1.133-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 9244 bytes, number of entries: 9
--rw-rw-rw-  2.0 unx        1 b- defN 24-Jan-02 14:20 hmd_cli_docker/__init__.py
--rw-rw-rw-  2.0 unx     1138 b- defN 24-Jan-02 14:20 hmd_cli_docker/config.py
--rw-rw-rw-  2.0 unx     7700 b- defN 24-Jan-02 14:20 hmd_cli_docker/controller.py
--rw-rw-rw-  2.0 unx    12939 b- defN 24-Jan-02 14:20 hmd_cli_docker/hmd_cli_docker.py
--rw-rw-rw-  2.0 unx     4434 b- defN 24-Jan-02 14:20 hmd_cli_docker/utils.py
--rw-rw-rw-  2.0 unx     1950 b- defN 24-Jan-02 14:20 hmd_cli_docker-0.1.132.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 24-Jan-02 14:20 hmd_cli_docker-0.1.132.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 24-Jan-02 14:20 hmd_cli_docker-0.1.132.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      750 b- defN 24-Jan-02 14:20 hmd_cli_docker-0.1.132.dist-info/RECORD
+-rw-rw-rw-  2.0 unx        1 b- defN 24-Jan-17 17:26 hmd_cli_docker/__init__.py
+-rw-rw-rw-  2.0 unx     1138 b- defN 24-Jan-17 17:26 hmd_cli_docker/config.py
+-rw-rw-rw-  2.0 unx     7700 b- defN 24-Jan-17 17:26 hmd_cli_docker/controller.py
+-rw-rw-rw-  2.0 unx    12939 b- defN 24-Jan-17 17:26 hmd_cli_docker/hmd_cli_docker.py
+-rw-rw-rw-  2.0 unx     4434 b- defN 24-Jan-17 17:26 hmd_cli_docker/utils.py
+-rw-rw-rw-  2.0 unx     1950 b- defN 24-Jan-17 17:27 hmd_cli_docker-0.1.133.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Jan-17 17:27 hmd_cli_docker-0.1.133.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 24-Jan-17 17:27 hmd_cli_docker-0.1.133.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      750 b- defN 24-Jan-17 17:27 hmd_cli_docker-0.1.133.dist-info/RECORD
 9 files, 29019 bytes uncompressed, 7944 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: hmd_cli_docker/hmd_cli_docker.py
 Comment: 
 
 Filename: hmd_cli_docker/utils.py
 Comment: 
 
-Filename: hmd_cli_docker-0.1.132.dist-info/METADATA
+Filename: hmd_cli_docker-0.1.133.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_docker-0.1.132.dist-info/WHEEL
+Filename: hmd_cli_docker-0.1.133.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_docker-0.1.132.dist-info/top_level.txt
+Filename: hmd_cli_docker-0.1.133.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_docker-0.1.132.dist-info/RECORD
+Filename: hmd_cli_docker-0.1.133.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `hmd_cli_docker-0.1.132.dist-info/METADATA` & `hmd_cli_docker-0.1.133.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-docker
-Version: 0.1.132
+Version: 0.1.133
 Summary: Implementation for docker cli command
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: attrs (==21.4.0)
@@ -18,15 +18,15 @@
 Requires-Dist: click (==8.0.4)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: docker (==5.0.3)
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: hmd-cli-app (~=1.1.600)
 Requires-Dist: hmd-cli-tools (~=1.1.230)
 Requires-Dist: hmd-lang-deployment (~=0.1.75)
-Requires-Dist: hmd-lib-containers (~=0.1.31)
+Requires-Dist: hmd-lib-containers (~=0.1.33)
 Requires-Dist: hmd-meta-types (~=0.2.87)
 Requires-Dist: hmd-schema-loader (~=0.2.35)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonschema (==4.4.0)
```

