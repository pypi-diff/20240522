# Comparing `tmp/gopappy-1.5.1-py3-none-any.whl.zip` & `tmp/gopappy-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5994 bytes, number of entries: 10
+Zip file size: 6234 bytes, number of entries: 10
 -rwxr-xr-x  2.0 unx       21 b- defN 80-Jan-01 00:00 gopappy/__init__.py
--rwxr-xr-x  2.0 unx     1079 b- defN 80-Jan-01 00:00 gopappy/api.py
+-rwxr-xr-x  2.0 unx      966 b- defN 80-Jan-01 00:00 gopappy/api.py
 -rwxr-xr-x  2.0 unx     3350 b- defN 80-Jan-01 00:00 gopappy/auth.py
--rwxr-xr-x  2.0 unx     3421 b- defN 80-Jan-01 00:00 gopappy/cli.py
+-rwxr-xr-x  2.0 unx     4444 b- defN 80-Jan-01 00:00 gopappy/cli.py
 -rwxr-xr-x  2.0 unx      393 b- defN 80-Jan-01 00:00 gopappy/colorize.py
--rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 gopappy-1.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1619 b- defN 80-Jan-01 00:00 gopappy-1.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gopappy-1.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 gopappy-1.5.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      752 b- defN 16-Jan-01 00:00 gopappy-1.5.1.dist-info/RECORD
-10 files, 11843 bytes uncompressed, 4726 bytes compressed:  60.1%
+-rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1619 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      751 b- defN 16-Jan-01 00:00 gopappy-1.6.0.dist-info/RECORD
+10 files, 12752 bytes uncompressed, 4966 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: gopappy/cli.py
 Comment: 
 
 Filename: gopappy/colorize.py
 Comment: 
 
-Filename: gopappy-1.5.1.dist-info/LICENSE
+Filename: gopappy-1.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: gopappy-1.5.1.dist-info/METADATA
+Filename: gopappy-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: gopappy-1.5.1.dist-info/WHEEL
+Filename: gopappy-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: gopappy-1.5.1.dist-info/entry_points.txt
+Filename: gopappy-1.6.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: gopappy-1.5.1.dist-info/RECORD
+Filename: gopappy-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gopappy/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.5.1'
+__version__ = '1.6.0'
```

## gopappy/api.py

```diff
@@ -1,14 +1,19 @@
 #!/usr/bin/env python
 
 import requests
 from gopappy.auth import main as auth
 
 API_KEY, API_SECRET = auth()
 
+headers = {
+    'Authorization': 'sso-key {}:{}'.format(API_KEY,
+                                            API_SECRET
+    )
+}
 
 class API:
     api_url = 'https://api.godaddy.com/v1'
     _shared = None
 
     def __init__(self, key, secret):
         self.key = key
@@ -17,23 +22,17 @@
     @classmethod
     def shared(cls):
         if not cls._shared:
             cls._shared = API(None, None)
         return cls._shared
 
     def get(self, path, **params):
-        headers = {
-            'Authorization': 'sso-key {}:{}'.format(API_KEY,
-                                                    API_SECRET
-            )
-        }
         url = '{}/{}'.format(self.api_url, path)
         return requests.get(url, headers=headers, params=params)
 
     def patch(self, path, **kwargs):
-        headers = {
-            "Authorization": "sso-key {}:{}".format(API_KEY,
-                                                    API_SECRET),
-            "Content-Type": "application/json",
-        }
         url = '{}/{}'.format(self.api_url, path)
         return requests.patch(url, headers=headers, **kwargs)
+
+    def delete(self, path):
+        url = '{}/{}'.format(self.api_url, path)
+        return requests.delete(url, headers=headers)
```

## gopappy/cli.py

```diff
@@ -15,15 +15,16 @@
 @app.command()
 def domain(
     domain: str = typer.Argument(...,
                                  help="Domain to be managed. e.g. mydomain.com"),
     action: str = typer.Argument(...,
                                  help="What to do with the domain"),
     data: Optional[list[str]] = typer.Argument(None,
-                                               help="Additional data"),
+                                               help="""add-record: [type, name, data]
+                                               delete-record: [type, name]"""),
     only_type: Optional[str] = typer.Option(None,
                                             "--type", "-t",
                                             help="Filter by record type"),
 ):
     api = API.shared()
 
     if action == "records":
@@ -50,27 +51,48 @@
         response = api.patch(url, data=json.dumps(params))
 
         if response.status_code != 200:
             info = response.json()
             print(info["code"], file=sys.stderr)
             sys.exit(1)
 
+    elif action == "delete-record":
+        if data and len(data) >= 2:
+            record_type, record_name = data[:2]
+            confirm = typer.confirm("Are you sure you want to delete this record?")
+            if confirm:
+                url = f"domains/{domain}/records/{record_type}/{record_name}"
+                response = api.delete(url)
+                if response.status_code != 200:
+                    try:
+                        info = response.json()
+                        print(info["code"], file=sys.stderr)
+                    except ValueError:
+                        print(f"Failed to decode JSON response: {response.text}", file=sys.stderr)
+                else:
+                    print("Record deleted successfully.")
+        else:
+            print("Insufficient data provided for deleting the record. Please provide [type, name].", file=sys.stderr)
+
     elif action == "suggest":
         url = "domains/suggest"
         domains = data[0].split(",")
         response = api.get(url, tlds=domains)
 
     elif action == "available" or action == "check":
         response = api.get("domains/available", domain=domain)
         data = response.json()
         if data["available"]:
             print("available")
         else:
             print("not available")
 
+    else:
+        print("Unsupported action")
+
 
 @app.command()
 def domains(
     status: str = typer.Option("active",
                                help="Filter by domain status")
 ):
     api = API.shared()
```

## Comparing `gopappy-1.5.1.dist-info/LICENSE` & `gopappy-1.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gopappy-1.5.1.dist-info/METADATA` & `gopappy-1.6.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopappy
-Version: 1.5.1
+Version: 1.6.0
 Summary: GoDaddy v1 API implementation with secured auth token.
 License: MIT
 Author: Gamaliel Espinoza
 Author-email: gamaliel.espinoza@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gopappy-1.5.1.dist-info/RECORD` & `gopappy-1.6.0.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-gopappy/__init__.py,sha256=oU1lLCdhmPP8CUfgzMFfhCPjCfk4eDfd8WSwOfXNBOk,21
-gopappy/api.py,sha256=soCP3oItPMvWN5PJJQBN5FgoWqKFtS-tR4Q0aEevxvc,1079
+gopappy/__init__.py,sha256=aWnRnF5TUBHC_2RdGczq36VyxBiPAviva2RjtMVjCFg,21
+gopappy/api.py,sha256=c1FHv_HbCQkujVKzT3v4wFtlp1dtZ9y_yO5HBZc__F4,966
 gopappy/auth.py,sha256=iHUD8wkCSZaN-9CB1cgYkA12RgdiDfZqT0WjKYgVEfM,3350
-gopappy/cli.py,sha256=3-9qXDQTrtyrNMZZsQb6XitUvzvV2xsEK9A5keEbi1U,3421
+gopappy/cli.py,sha256=V4QY6Buebwd-A5OVwDQ_IelM1W2jXIe0GPgEDhzURKk,4444
 gopappy/colorize.py,sha256=QwGkEhGRzRprJjyONIMFo11fu3_a5t3mMg9y_PR6X88,393
-gopappy-1.5.1.dist-info/LICENSE,sha256=1hVkStSH9VsmTSzE-I_mGfPfx9W66QYQGJe_o_QmL44,1077
-gopappy-1.5.1.dist-info/METADATA,sha256=R6345fW8Fckw9k7U9f_gxe79KQ08_IDSqZNIY-Lee1M,1619
-gopappy-1.5.1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-gopappy-1.5.1.dist-info/entry_points.txt,sha256=6KsM9dzJWMjjMpA72jNrBaaxz3O8aPsK4dDs4_PbirE,43
-gopappy-1.5.1.dist-info/RECORD,,
+gopappy-1.6.0.dist-info/LICENSE,sha256=1hVkStSH9VsmTSzE-I_mGfPfx9W66QYQGJe_o_QmL44,1077
+gopappy-1.6.0.dist-info/METADATA,sha256=HqWAgzOQN_iwas9c8uea5dkSZVSm-38h6uU6vFMmDCM,1619
+gopappy-1.6.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+gopappy-1.6.0.dist-info/entry_points.txt,sha256=6KsM9dzJWMjjMpA72jNrBaaxz3O8aPsK4dDs4_PbirE,43
+gopappy-1.6.0.dist-info/RECORD,,
```

