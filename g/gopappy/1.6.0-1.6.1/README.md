# Comparing `tmp/gopappy-1.6.0-py3-none-any.whl.zip` & `tmp/gopappy-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6234 bytes, number of entries: 10
+Zip file size: 6386 bytes, number of entries: 10
 -rwxr-xr-x  2.0 unx       21 b- defN 80-Jan-01 00:00 gopappy/__init__.py
--rwxr-xr-x  2.0 unx      966 b- defN 80-Jan-01 00:00 gopappy/api.py
+-rwxr-xr-x  2.0 unx     1160 b- defN 80-Jan-01 00:00 gopappy/api.py
 -rwxr-xr-x  2.0 unx     3350 b- defN 80-Jan-01 00:00 gopappy/auth.py
--rwxr-xr-x  2.0 unx     4444 b- defN 80-Jan-01 00:00 gopappy/cli.py
+-rwxr-xr-x  2.0 unx     4594 b- defN 80-Jan-01 00:00 gopappy/cli.py
 -rwxr-xr-x  2.0 unx      393 b- defN 80-Jan-01 00:00 gopappy/colorize.py
--rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1619 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 gopappy-1.6.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      751 b- defN 16-Jan-01 00:00 gopappy-1.6.0.dist-info/RECORD
-10 files, 12752 bytes uncompressed, 4966 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx     1077 b- defN 80-Jan-01 00:00 gopappy-1.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1709 b- defN 80-Jan-01 00:00 gopappy-1.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 gopappy-1.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       43 b- defN 80-Jan-01 00:00 gopappy-1.6.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      752 b- defN 16-Jan-01 00:00 gopappy-1.6.1.dist-info/RECORD
+10 files, 13187 bytes uncompressed, 5118 bytes compressed:  61.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: gopappy/cli.py
 Comment: 
 
 Filename: gopappy/colorize.py
 Comment: 
 
-Filename: gopappy-1.6.0.dist-info/LICENSE
+Filename: gopappy-1.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: gopappy-1.6.0.dist-info/METADATA
+Filename: gopappy-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: gopappy-1.6.0.dist-info/WHEEL
+Filename: gopappy-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: gopappy-1.6.0.dist-info/entry_points.txt
+Filename: gopappy-1.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: gopappy-1.6.0.dist-info/RECORD
+Filename: gopappy-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gopappy/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '1.6.0'
+__version__ = '1.6.1'
```

## gopappy/api.py

```diff
@@ -1,38 +1,38 @@
 #!/usr/bin/env python
 
 import requests
 from gopappy.auth import main as auth
 
 API_KEY, API_SECRET = auth()
 
-headers = {
-    'Authorization': 'sso-key {}:{}'.format(API_KEY,
-                                            API_SECRET
-    )
-}
+default_headers = {"Authorization": "sso-key {}:{}".format(API_KEY, API_SECRET)}
+
 
 class API:
-    api_url = 'https://api.godaddy.com/v1'
+    api_url = "https://api.godaddy.com/v1"
     _shared = None
 
     def __init__(self, key, secret):
         self.key = key
         self.secret = secret
+        self.default_headers = {"Authorization": f"sso-key {self.key}:{self.secret}"}
 
     @classmethod
     def shared(cls):
         if not cls._shared:
-            cls._shared = API(None, None)
+            cls._shared = API(API_KEY, API_SECRET)
         return cls._shared
 
     def get(self, path, **params):
-        url = '{}/{}'.format(self.api_url, path)
-        return requests.get(url, headers=headers, params=params)
+        url = f"{self.api_url}/{path}"
+        return requests.get(url, headers=self.default_headers, params=params)
 
     def patch(self, path, **kwargs):
-        url = '{}/{}'.format(self.api_url, path)
+        url = f"{self.api_url}/{path}"
+        headers = kwargs.pop('headers', {})  # Remove headers from kwargs
+        headers.update(self.default_headers)  # Merge with default headers
         return requests.patch(url, headers=headers, **kwargs)
 
     def delete(self, path):
-        url = '{}/{}'.format(self.api_url, path)
-        return requests.delete(url, headers=headers)
+        url = f"{self.api_url}/{path}"
+        return requests.delete(url, headers=self.default_headers)
```

## gopappy/cli.py

```diff
@@ -4,130 +4,143 @@
 import sys
 import os
 import typer
 from gopappy.api import API
 from gopappy.colorize import colorize
 from gopappy import __version__
 from typing import Optional
+from urllib.parse import urlencode
 
 app = typer.Typer()
 
 
 @app.command()
-def domain(
-    domain: str = typer.Argument(...,
-                                 help="Domain to be managed. e.g. mydomain.com"),
-    action: str = typer.Argument(...,
-                                 help="What to do with the domain"),
-    data: Optional[list[str]] = typer.Argument(None,
-                                               help="""add-record: [type, name, data]
-                                               delete-record: [type, name]"""),
-    only_type: Optional[str] = typer.Option(None,
-                                            "--type", "-t",
-                                            help="Filter by record type"),
+def records(
+    domain: str = typer.Argument(..., help="Domain to be managed. e.g. mydomain.com"),
+    only_type: Optional[str] = typer.Option(None, "--type", "-t", help="Filter by record type"),
 ):
     api = API.shared()
+    response = api.get(f"domains/{domain}/records")
+    records = response.json()
 
-    if action == "records":
-        response = api.get("domains/{}/records".format(domain))
-        data = response.json()
+    max_name_length = max(len(record["name"]) for record in records) if records else 0
+    name_width = max(max_name_length, len("Name"))
 
-        try:
-            for record in data:
-                if not only_type or record["type"].lower() == only_type.lower():
-                    print(f"{record['type']: <10}{record['name']: <20}{record['data']}")
-        except TypeError as e:
-            colorize("red", f"Domain:\t{domain}")
-            colorize("red", f"Error:\t{e}")
-
-    elif action == "add-record":
-        url = "domains/{}/records".format(domain)
-        params = [
-            {
-                "type": data[0].upper(),    # A / CNAME
-                "name": data[1],            # fulano., mangano.
-                "data": data[2],            # points to ip/domain
-            }
-        ]
-        response = api.patch(url, data=json.dumps(params))
+    print(f"Domain: {domain}")
+    try:
+        for record in records:
+            if not only_type or record["type"].lower() == only_type.lower():
+                print(f"{record['type']: <10}{record['name']: <{name_width}}{record['data']}")
+    except TypeError as e:
+        colorize("red", f"Domain:\t{domain}")
+        colorize("red", f"Error:\t{e}")
 
-        if response.status_code != 200:
+
+@app.command()
+def add_record(
+    domain: str = typer.Argument(..., help="Domain to be managed. e.g. mydomain.com"),
+    type_: str = typer.Option(..., "--type", "-t", help="Record type"),
+    name: str = typer.Option(..., "--name", "-n", help="Record name"),
+    data: str = typer.Option(..., "--data", "-d", help="Record data"),
+):
+    api = API.shared()
+    url = f"domains/{domain}/records"
+    record_data = [{"type": type_.upper(), "name": name, "data": data}]
+    response = api.patch(url, json=record_data)
+
+    print(f"Domain: {domain}")
+    print(f"Type: {type_}")
+    print(f"Name: {name}")
+    print(f"Data: {data}")
+
+    if response.status_code != 200:
+        try:
             info = response.json()
             print(info["code"], file=sys.stderr)
-            sys.exit(1)
+        except ValueError:
+            print(f"Failed to decode JSON response: {response.text}", file=sys.stderr)
+        sys.exit(1)
+    else:
+        print("Record added successfully.")
 
-    elif action == "delete-record":
-        if data and len(data) >= 2:
-            record_type, record_name = data[:2]
-            confirm = typer.confirm("Are you sure you want to delete this record?")
-            if confirm:
-                url = f"domains/{domain}/records/{record_type}/{record_name}"
-                response = api.delete(url)
-                if response.status_code != 200:
-                    try:
-                        info = response.json()
-                        print(info["code"], file=sys.stderr)
-                    except ValueError:
-                        print(f"Failed to decode JSON response: {response.text}", file=sys.stderr)
-                else:
-                    print("Record deleted successfully.")
-        else:
-            print("Insufficient data provided for deleting the record. Please provide [type, name].", file=sys.stderr)
 
-    elif action == "suggest":
-        url = "domains/suggest"
-        domains = data[0].split(",")
-        response = api.get(url, tlds=domains)
-
-    elif action == "available" or action == "check":
-        response = api.get("domains/available", domain=domain)
-        data = response.json()
-        if data["available"]:
-            print("available")
-        else:
-            print("not available")
+@app.command()
+def delete_record(
+    domain: str = typer.Argument(..., help="Domain to be managed. e.g. mydomain.com"),
+    type_: str = typer.Option(..., "--type", "-t", help="Record type"),
+    name: str = typer.Option(..., "--name", "-n", help="Record name"),
+):
+    api = API.shared()
 
-    else:
-        print("Unsupported action")
+    print(f"Domain: {domain}")
+    print(f"Type: {type_}")
+    print(f"Name: {name}")
+
+    confirm = typer.confirm("Are you sure you want to delete this record?")
+    if confirm:
+        url = f"domains/{domain}/records/{type_}/{name}"
+        response = api.delete(url)
+
+        # TODO: status code not being 200 w/successful deletion
+        # * ./cli.py delete-record $DOMAIN -t A -n subdomain
+        if response.status_code != 200:
+            try:
+                info = response.json()
+                print(info["code"], file=sys.stderr)
+            except ValueError:
+                print(f"Failed to decode JSON response: {response.text}", file=sys.stderr)
+            sys.exit(1)
+        else:
+            print("Record deleted successfully.")
 
 
 @app.command()
-def domains(
-    status: str = typer.Option("active",
-                               help="Filter by domain status")
-):
+def domains(status: str = typer.Option("active", help="Filter by domain status")):
     api = API.shared()
-    data = api.get('/domains')
-    status = status.upper() if status else ''
+    data = api.get("/domains")
+    status = status.upper() if status else ""
     for domain in data.json():
-        if status != '':
-            if domain['status'] == status:
+        if status != "":
+            if domain["status"] == status:
                 colorize("green", f"[DOMAIN] {domain['domain']}")
                 colorize("green", f"[STATUS] {domain['status']}")
             else:
                 colorize("green", f"[DOMAIN] {domain['domain']}")
                 colorize("red", f"[STATUS] {domain['status']}")
         else:
             colorize("white", f"[DOMAIN] {domain['domain']}")
             colorize("white", f"[STATUS] {domain['status']}")
 
 
+# TODO
+# ! {'code': 'ACCESS_DENIED', 'message': 'Authenticated user is not allowed access'}
+@app.command("check")
+def check_availability(domain: str = typer.Argument(..., help="Domain to check")):
+    api = API.shared()
+    params = urlencode({
+        "domain": domain,
+        "checkType": "FAST",
+        "forTransfer": "false"
+    })
+    url = f"domains/available?{params}"
+    data = [domain]
+    response = api.get(url, json=data)
+    print(response.json())
+
 
-def version_callback(value: bool):
+def _version_callback(value: bool):
     if value:
         print(__version__)
         raise typer.Exit()
 
 
 @app.callback()
 def version(
-    version: bool = typer.Option(None,
-                                 "--version", "-v",
-                                 callback=version_callback,
-                                 is_eager=True,
-                                 help="Print the version and exit")
+    version: bool = typer.Option(
+        None, "--version", "-v", callback=_version_callback, is_eager=True, help="Print the version and exit"
+    ),
 ):
     pass
 
 
 if __name__ == "__main__":
     app()
```

## Comparing `gopappy-1.6.0.dist-info/LICENSE` & `gopappy-1.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gopappy-1.6.0.dist-info/METADATA` & `gopappy-1.6.1.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gopappy
-Version: 1.6.0
+Version: 1.6.1
 Summary: GoDaddy v1 API implementation with secured auth token.
 License: MIT
 Author: Gamaliel Espinoza
 Author-email: gamaliel.espinoza@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -19,46 +19,61 @@
 Description-Content-Type: text/markdown
 
 # gopappy
 
 Inspo from [here](https://github.com/gamikun/gopapi).
 
 ## Installation
+
 ```bash
 python -m pip install gopappy
 ```
 
 ## Usage
 
 ### Adding a DNS record to a domain
+
 ```bash
 # A record
-gopappy domain yourdomain.com add-record A subdomain 127.0.0.1
+gopappy domain $DOMAIN add-record A subdomain 127.0.0.1
 # Where A can also be CNAME
 # 127.0.0.1 to be replaced with the actual IP
 
 # CNAME
-gopappy domain yourdomain.com add-record A subdomain 127.0.0.1
+gopappy add-record $DOMAIN -t A -n subdomain -d 127.0.0.1
 # Where A can also be CNAME
 # 127.0.0.1 to be replaced with the actual IP
+
+# TXT
+gopappy add-record $DOMAIN -t TXT -n subdomain -d "some text here"
+```
+
+### Deleting a DNS record from a domain
+
+```bash
+gopappy delete-record $DOMAIN -t A -n subdomain
 ```
+
 ### Listing records of a domain
+
 ```bash
-gopappy domain mydomain.com records
-# and if you need to filter by record type
-gopappy domain mydomain.com records -t cname
+# list all records
+gopappy records $DOMAIN
+
+# filter by record type
+gopappy records $DOMAIN -t cname
 ```
 
 ### Listing all domains in godaddy account
+
 ```bash
 gopappy domains
 # mydomain1.com
 # mydomain2.com
 ```
 
 ### Check whether a domain is available to purchase or not
+
 ```bash
-gopappy domain acme.com check
-# or with alias
-gopappy domain acme.com available
+gopappy check $DOMAIN 
 ```
```

## Comparing `gopappy-1.6.0.dist-info/RECORD` & `gopappy-1.6.1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-gopappy/__init__.py,sha256=aWnRnF5TUBHC_2RdGczq36VyxBiPAviva2RjtMVjCFg,21
-gopappy/api.py,sha256=c1FHv_HbCQkujVKzT3v4wFtlp1dtZ9y_yO5HBZc__F4,966
+gopappy/__init__.py,sha256=DH87PU9LcZeI_uvttoH-lyhGyb55UShgeFtsG2qIZgE,21
+gopappy/api.py,sha256=uTBiw_QuFpJ1zgpi43u2hoo6On1lT0IDF6NMSP8PiLQ,1160
 gopappy/auth.py,sha256=iHUD8wkCSZaN-9CB1cgYkA12RgdiDfZqT0WjKYgVEfM,3350
-gopappy/cli.py,sha256=V4QY6Buebwd-A5OVwDQ_IelM1W2jXIe0GPgEDhzURKk,4444
+gopappy/cli.py,sha256=SaA2oUiEaS4U_ebWDKA3W_ZNBXMXnyQzB88aTJALWl0,4594
 gopappy/colorize.py,sha256=QwGkEhGRzRprJjyONIMFo11fu3_a5t3mMg9y_PR6X88,393
-gopappy-1.6.0.dist-info/LICENSE,sha256=1hVkStSH9VsmTSzE-I_mGfPfx9W66QYQGJe_o_QmL44,1077
-gopappy-1.6.0.dist-info/METADATA,sha256=HqWAgzOQN_iwas9c8uea5dkSZVSm-38h6uU6vFMmDCM,1619
-gopappy-1.6.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-gopappy-1.6.0.dist-info/entry_points.txt,sha256=6KsM9dzJWMjjMpA72jNrBaaxz3O8aPsK4dDs4_PbirE,43
-gopappy-1.6.0.dist-info/RECORD,,
+gopappy-1.6.1.dist-info/LICENSE,sha256=1hVkStSH9VsmTSzE-I_mGfPfx9W66QYQGJe_o_QmL44,1077
+gopappy-1.6.1.dist-info/METADATA,sha256=7_eVIoWVMYq9m-OvKFI82iKhAQD66Xkqaq48y6SEDv0,1709
+gopappy-1.6.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+gopappy-1.6.1.dist-info/entry_points.txt,sha256=6KsM9dzJWMjjMpA72jNrBaaxz3O8aPsK4dDs4_PbirE,43
+gopappy-1.6.1.dist-info/RECORD,,
```

