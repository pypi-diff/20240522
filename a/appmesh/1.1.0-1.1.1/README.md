# Comparing `tmp/appmesh-1.1.0-py3-none-any.whl.zip` & `tmp/appmesh-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16377 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-21 14:05 appmesh/__init__.py
--rw-r--r--  2.0 unx    59572 b- defN 24-May-21 14:05 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10786 b- defN 24-May-21 14:05 appmesh-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 14:05 appmesh-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-21 14:05 appmesh-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-21 14:05 appmesh-1.1.0.dist-info/RECORD
-6 files, 70924 bytes uncompressed, 15555 bytes compressed:  78.1%
+Zip file size: 16391 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-21 22:45 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59624 b- defN 24-May-21 22:45 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10786 b- defN 24-May-21 22:45 appmesh-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-21 22:45 appmesh-1.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-21 22:45 appmesh-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-21 22:45 appmesh-1.1.1.dist-info/RECORD
+6 files, 70976 bytes uncompressed, 15569 bytes compressed:  78.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.1.0.dist-info/METADATA
+Filename: appmesh-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.1.0.dist-info/WHEEL
+Filename: appmesh-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.1.0.dist-info/top_level.txt
+Filename: appmesh-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.1.0.dist-info/RECORD
+Filename: appmesh-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## appmesh/appmesh_client.py

```diff
@@ -1296,15 +1296,16 @@
     def __del__(self) -> None:
         """De-construction"""
         self.__close_socket()
 
     def __connect_socket(self) -> None:
         """Establish tcp connection"""
         context = ssl.create_default_context(ssl.Purpose.SERVER_AUTH)
-        context.minimum_version = ssl.TLSVersion.TLSv1_2
+        if hasattr(context, "minimum_version"):
+            context.minimum_version = ssl.TLSVersion.TLSv1_2
         context.verify_mode = ssl.CERT_NONE if self.ssl_verify is False else ssl.CERT_REQUIRED
         if isinstance(self.ssl_verify, str):
             # Load server-side certificate authority (CA) certificates
             context.check_hostname = True
             context.load_verify_locations(self.ssl_verify)
         if self.ssl_client_cert is not None:
             # Load client-side certificate and private key
```

## Comparing `appmesh-1.1.0.dist-info/METADATA` & `appmesh-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.1.0
+Version: 1.1.1
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.1.0 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.1.1 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
```

