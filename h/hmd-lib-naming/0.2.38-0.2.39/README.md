# Comparing `tmp/hmd_lib_naming-0.2.38-py3-none-any.whl.zip` & `tmp/hmd_lib_naming-0.2.39-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5704 bytes, number of entries: 10
--rw-rw-rw-  2.0 unx        0 b- defN 24-Jan-02 19:31 hmd_lib_naming/__init__.py
--rw-rw-rw-  2.0 unx     2948 b- defN 24-Jan-02 19:31 hmd_lib_naming/hmd_lib_naming.py
--rw-rw-rw-  2.0 unx     4733 b- defN 24-Jan-02 19:31 hmd_lib_naming/service_manager.py
--rw-rw-rw-  2.0 unx      535 b- defN 24-Jan-02 19:31 hmd_lib_naming/schemas/hmd_lang_naming/service.hms
--rw-rw-rw-  2.0 unx      246 b- defN 24-Jan-02 19:31 hmd_lib_naming/schemas/hmd_lang_naming/service_consists_of_repo_instance_deployment.hms
--rw-rw-rw-  2.0 unx      214 b- defN 24-Jan-02 19:31 hmd_lib_naming/schemas/hmd_lang_naming/service_is_in_environment.hms
--rw-rw-rw-  2.0 unx     2448 b- defN 24-Jan-02 19:32 hmd_lib_naming-0.2.38.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 24-Jan-02 19:32 hmd_lib_naming-0.2.38.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 24-Jan-02 19:32 hmd_lib_naming-0.2.38.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      962 b- defN 24-Jan-02 19:32 hmd_lib_naming-0.2.38.dist-info/RECORD
-10 files, 12193 bytes uncompressed, 4010 bytes compressed:  67.1%
+Zip file size: 5737 bytes, number of entries: 10
+-rw-rw-rw-  2.0 unx        0 b- defN 24-Apr-02 15:17 hmd_lib_naming/__init__.py
+-rw-rw-rw-  2.0 unx     2948 b- defN 24-Apr-02 15:17 hmd_lib_naming/hmd_lib_naming.py
+-rw-rw-rw-  2.0 unx     5058 b- defN 24-Apr-02 15:17 hmd_lib_naming/service_manager.py
+-rw-rw-rw-  2.0 unx      535 b- defN 24-Apr-02 15:17 hmd_lib_naming/schemas/hmd_lang_naming/service.hms
+-rw-rw-rw-  2.0 unx      246 b- defN 24-Apr-02 15:17 hmd_lib_naming/schemas/hmd_lang_naming/service_consists_of_repo_instance_deployment.hms
+-rw-rw-rw-  2.0 unx      214 b- defN 24-Apr-02 15:17 hmd_lib_naming/schemas/hmd_lang_naming/service_is_in_environment.hms
+-rw-rw-rw-  2.0 unx     2448 b- defN 24-Apr-02 15:18 hmd_lib_naming-0.2.39.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Apr-02 15:18 hmd_lib_naming-0.2.39.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 24-Apr-02 15:18 hmd_lib_naming-0.2.39.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      962 b- defN 24-Apr-02 15:18 hmd_lib_naming-0.2.39.dist-info/RECORD
+10 files, 12518 bytes uncompressed, 4043 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: hmd_lib_naming/schemas/hmd_lang_naming/service_consists_of_repo_instance_deployment.hms
 Comment: 
 
 Filename: hmd_lib_naming/schemas/hmd_lang_naming/service_is_in_environment.hms
 Comment: 
 
-Filename: hmd_lib_naming-0.2.38.dist-info/METADATA
+Filename: hmd_lib_naming-0.2.39.dist-info/METADATA
 Comment: 
 
-Filename: hmd_lib_naming-0.2.38.dist-info/WHEEL
+Filename: hmd_lib_naming-0.2.39.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_lib_naming-0.2.38.dist-info/top_level.txt
+Filename: hmd_lib_naming-0.2.39.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_lib_naming-0.2.38.dist-info/RECORD
+Filename: hmd_lib_naming-0.2.39.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_lib_naming/service_manager.py

```diff
@@ -95,14 +95,24 @@
                 expired_auth_token_callback=self.expired_auth_token_callback,
             )
 
     def get_loaders(self) -> Dict[str, DefaultLoader]:
         return self.loaders
 
     def _get_naming_service_client(self):
+        if self.environment == "local":
+            naming_url = "http://hmd_gateway:8080/ms-naming/"
+            auth_token = self.auth_token
+
+            return RestClient(
+                naming_url,
+                hmd_lib_naming.hmd_lib_naming.get_default_loader(),
+                auth_token=auth_token,
+            )
+
         if self.environment != self.naming_environment:
             naming_url = f"https://{self.naming_instance_name}-{self.naming_did}-{self.naming_region}.{os.environ['HMD_CUSTOMER_CODE']}-{self.naming_environment}-neuronsphere.io"
             auth_token = self.auth_token
 
             return RestClient(
                 naming_url,
                 hmd_lib_naming.hmd_lib_naming.get_default_loader(),
```

## Comparing `hmd_lib_naming-0.2.38.dist-info/METADATA` & `hmd_lib_naming-0.2.39.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-lib-naming
-Version: 0.2.38
+Version: 0.2.39
 Summary: Naming service library client
 Author: Alex Burgoon
 Author-email: alex.burgoon@hmdlabs.io
 License: Apache 2.0
 Requires-Dist: acachecontrol (==0.3.5)
 Requires-Dist: aenum (==2.2.6)
 Requires-Dist: aiohttp (==3.8.1)
@@ -27,16 +27,16 @@
 Requires-Dist: google-auth (==2.9.1)
 Requires-Dist: greenlet (==1.1.2)
 Requires-Dist: gremlinpython (==3.5.2)
 Requires-Dist: hmd-cli-tools (~=1.1.230)
 Requires-Dist: hmd-entity-storage (~=0.1.228)
 Requires-Dist: hmd-graphql-client (~=0.1.108)
 Requires-Dist: hmd-lang-naming (~=0.1.10)
-Requires-Dist: hmd-lib-auth (~=0.1.77)
-Requires-Dist: hmd-meta-types (~=0.2.87)
+Requires-Dist: hmd-lib-auth (~=0.1.81)
+Requires-Dist: hmd-meta-types (~=0.2.90)
 Requires-Dist: hmd-schema-loader (~=0.2.34)
 Requires-Dist: idna (==3.3)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: isodate (==0.6.1)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: jsonschema (==4.4.0)
 Requires-Dist: kubernetes (==24.2.0)
```

## Comparing `hmd_lib_naming-0.2.38.dist-info/RECORD` & `hmd_lib_naming-0.2.39.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 hmd_lib_naming/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hmd_lib_naming/hmd_lib_naming.py,sha256=gyNJtcnDJvtjc6VYjXvxC6lqiPjdAA3SbOdn6sOt3tU,2948
-hmd_lib_naming/service_manager.py,sha256=-Zz2vYN_kbNuN8k36JGtTyi8A-dkkGCBvTgmZcrkA30,4733
+hmd_lib_naming/service_manager.py,sha256=7Ic4BVcm2baK-DNyahm3pLTewMt7EF2MhiYZC0zODMg,5058
 hmd_lib_naming/schemas/hmd_lang_naming/service.hms,sha256=PNPWxgT0WPRmshIaW-nAp28C57wXr-KMrcLzJY9lWKQ,535
 hmd_lib_naming/schemas/hmd_lang_naming/service_consists_of_repo_instance_deployment.hms,sha256=SA71NGeNCGWfUW1hNmALM5o4f3htTbADOgLMsy64DUc,246
 hmd_lib_naming/schemas/hmd_lang_naming/service_is_in_environment.hms,sha256=vWqC4XRiOcjWWAF866kXrXT3o6IyXLAMdbGNJeovvHw,214
-hmd_lib_naming-0.2.38.dist-info/METADATA,sha256=CQ_ErwZeRvYteWbXvuLHH-OOyKy0qIJpDO_GdBizk6o,2448
-hmd_lib_naming-0.2.38.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
-hmd_lib_naming-0.2.38.dist-info/top_level.txt,sha256=fG1Q0BJvhWyylIHLLHOeN4x-sqlgryetRdij2ZhLCS0,15
-hmd_lib_naming-0.2.38.dist-info/RECORD,,
+hmd_lib_naming-0.2.39.dist-info/METADATA,sha256=mWoEywna3lfc9nKgVtyWlUciqA84x7zxmk1gTX4uTTg,2448
+hmd_lib_naming-0.2.39.dist-info/WHEEL,sha256=Ni9JGQXk2T4q02tFVwTZ-iAb8m9R1cjnSLMaE4VH1rg,92
+hmd_lib_naming-0.2.39.dist-info/top_level.txt,sha256=fG1Q0BJvhWyylIHLLHOeN4x-sqlgryetRdij2ZhLCS0,15
+hmd_lib_naming-0.2.39.dist-info/RECORD,,
```

