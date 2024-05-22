# Comparing `tmp/hmd_cli_python-0.2.77-py3-none-any.whl.zip` & `tmp/hmd_cli_python-0.2.78-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6081 bytes, number of entries: 7
--rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-21 11:20 hmd_cli_python/__init__.py
--rw-rw-rw-  2.0 unx     3624 b- defN 23-Jul-21 11:20 hmd_cli_python/controller.py
--rw-rw-rw-  2.0 unx     9749 b- defN 23-Jul-21 11:20 hmd_cli_python/hmd_cli_python.py
--rw-rw-rw-  2.0 unx     2534 b- defN 23-Jul-21 11:21 hmd_cli_python-0.2.77.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Jul-21 11:21 hmd_cli_python-0.2.77.dist-info/WHEEL
--rw-rw-rw-  2.0 unx       15 b- defN 23-Jul-21 11:21 hmd_cli_python-0.2.77.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-21 11:21 hmd_cli_python-0.2.77.dist-info/RECORD
-7 files, 16598 bytes uncompressed, 5035 bytes compressed:  69.7%
+Zip file size: 5972 bytes, number of entries: 7
+-rw-rw-rw-  2.0 unx        0 b- defN 24-May-22 14:52 hmd_cli_python/__init__.py
+-rw-rw-rw-  2.0 unx     3675 b- defN 24-May-22 14:52 hmd_cli_python/controller.py
+-rw-rw-rw-  2.0 unx     9165 b- defN 24-May-22 14:52 hmd_cli_python/hmd_cli_python.py
+-rw-rw-rw-  2.0 unx     2499 b- defN 24-May-22 14:55 hmd_cli_python-0.2.78.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-May-22 14:55 hmd_cli_python-0.2.78.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       15 b- defN 24-May-22 14:55 hmd_cli_python-0.2.78.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 24-May-22 14:55 hmd_cli_python-0.2.78.dist-info/RECORD
+7 files, 16030 bytes uncompressed, 4926 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: hmd_cli_python/controller.py
 Comment: 
 
 Filename: hmd_cli_python/hmd_cli_python.py
 Comment: 
 
-Filename: hmd_cli_python-0.2.77.dist-info/METADATA
+Filename: hmd_cli_python-0.2.78.dist-info/METADATA
 Comment: 
 
-Filename: hmd_cli_python-0.2.77.dist-info/WHEEL
+Filename: hmd_cli_python-0.2.78.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_cli_python-0.2.77.dist-info/top_level.txt
+Filename: hmd_cli_python-0.2.78.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_cli_python-0.2.77.dist-info/RECORD
+Filename: hmd_cli_python-0.2.78.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_cli_python/controller.py

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from importlib.metadata import version
 
 from cement import Controller, ex
 
-from hmd_cli_tools.hmd_cli_tools import get_standard_parameters
+from hmd_cli_tools.hmd_cli_tools import get_standard_parameters, load_hmd_env
 
 
 VERSION_BANNER = """
 hmd docker version: {}
 """
 
 
@@ -39,14 +39,15 @@
         self.app.args.print_help()
 
     @ex(
         help="login into multiple registries and edit pip config",
         arguments=get_standard_parameters(["account"]),
     )
     def login(self):
+        load_hmd_env(override=False)
         from .hmd_cli_python import login as do_login
 
         registries = os.environ.get("PYTHON_REGISTRIES", "{}")
         default_username = os.environ.get("PIP_USERNAME")
         default_password = os.environ.get("PIP_PASSWORD")
         default_url = os.environ.get("PIP_EXTRA_INDEX_URL")
```

## hmd_cli_python/hmd_cli_python.py

```diff
@@ -1,10 +1,10 @@
 import os
 from pathlib import Path
-from base64 import b64decode
+import configparser
 import shutil
 from typing import Any, Dict, List
 from urllib.parse import urlparse, urlunparse
 
 from cement.utils import shell
 from setuptools import find_packages
 
@@ -158,63 +158,36 @@
                 )
 
             url_parts = url_parts._replace(
                 netloc=f"{username}:{password}@{url_parts.hostname}"
             )
             extra_index_urls.append(urlunparse(url_parts))
 
-    data = []
-    if os.path.exists(pip_conf_name):
-        with open(pip_conf_name, "r") as pc:
-            data = pc.readlines()
-
-    extra_urls = []
-    extra_urls_line = False
-    for line in data:
-        if line.startswith("extra-index-url"):
-            _, urls = line.split("=")
-            extra_urls_str = urls.strip()
-            extra_urls_line = True
-
-            if len(extra_urls_str) > 0:
-                extra_urls = extra_urls_str.split(",")
-
-            if len(extra_urls) > 0:
-                break
-            else:
-                continue
-
-        if extra_urls_line:
-            url = line.strip()
-
-            if len(url) == 0 or url.startswith("["):
-                break
-            extra_urls.append(url)
+    pip_config = configparser.ConfigParser()
+    pip_config.read(pip_conf_name)
+
+    extra_urls = pip_config["global"]["extra-index-url"]
+    if not isinstance(extra_urls, list):
+        extra_urls = extra_urls.split("\n")
 
     existing_urls = list(
-        filter(lambda u: urlparse(u).hostname not in registry_urls, extra_urls)
+        filter(lambda u: urlparse(u.strip()).hostname not in registry_urls, extra_urls)
+    )
+    pip_config["global"]["extra-index-url"] = "\n".join(
+        [*existing_urls, *extra_index_urls]
     )
-    extra_index_urls = [*existing_urls, *extra_index_urls]
-    extra_str = "\n    ".join(extra_index_urls)
-    pip_conf = f"""
-[global]
-extra-index-url = 
-    {extra_str}
-    
-"""
-
     with open(pip_conf_name, "w") as pc:
-        pc.write(pip_conf)
+        pip_config.write(pc)
 
     if len(twine_urls) > 0:
         if not os.path.exists(Path.home() / ".pypirc"):
             with open(Path.home() / ".pypirc", "w") as twine:
                 cfg = f"""
 [distutils]
-index-servers = 
+index-servers =
     neuronsphere
 
 [neuronsphere]
 repository = {twine_urls[0][0]}
 username = {twine_urls[0][1]}
 password = {twine_urls[0][2]}
                 """
```

## Comparing `hmd_cli_python-0.2.77.dist-info/METADATA` & `hmd_cli_python-0.2.78.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmd-cli-python
-Version: 0.2.77
+Version: 0.2.78
 Summary: Implementation for python cli command
 Home-page: UNKNOWN
 Author: Jim Majure
 Author-email: jim.majure@hmdlabs.io
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Dist: attrs (==21.4.0)
@@ -18,41 +18,40 @@
 Requires-Dist: cffi (==1.15.0)
 Requires-Dist: charset-normalizer (==2.0.12)
 Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: coverage[toml] (==6.3.2)
 Requires-Dist: cryptography (==39.0.1)
 Requires-Dist: docutils (==0.18.1)
 Requires-Dist: google-auth (==2.9.1)
-Requires-Dist: hmd-cli-app (~=1.1.597)
-Requires-Dist: hmd-cli-tools (~=1.1.229)
+Requires-Dist: hmd-cli-app (~=1.1.600)
+Requires-Dist: hmd-cli-tools (~=1.1.230)
 Requires-Dist: idna (==3.3)
 Requires-Dist: importlib-metadata (==4.11.2)
 Requires-Dist: iniconfig (==1.1.1)
 Requires-Dist: inquirerpy (==0.3.4)
 Requires-Dist: jeepney (==0.8.0)
 Requires-Dist: jinja2 (==3.0.3)
 Requires-Dist: jmespath (==0.10.0)
 Requires-Dist: keyring (==23.5.0)
 Requires-Dist: kubernetes (==24.2.0)
 Requires-Dist: markdown-it-py (==2.2.0)
 Requires-Dist: markupsafe (==2.1.0)
 Requires-Dist: mdurl (==0.1.2)
 Requires-Dist: oauthlib (==3.2.2)
-Requires-Dist: packaging (==21.3)
+Requires-Dist: packaging (==24.0)
 Requires-Dist: pfzy (==0.3.4)
 Requires-Dist: pkginfo (==1.8.2)
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: prompt-toolkit (==3.0.38)
 Requires-Dist: py (==1.11.0)
 Requires-Dist: pyasn1 (==0.4.8)
 Requires-Dist: pyasn1-modules (==0.2.8)
 Requires-Dist: pycparser (==2.21)
 Requires-Dist: pygments (==2.14.0)
 Requires-Dist: pyopenssl (==23.0.0)
-Requires-Dist: pyparsing (==3.0.7)
 Requires-Dist: pytest (==7.0.1)
 Requires-Dist: pytest-cov (==3.0.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-dotenv (==0.19.2)
 Requires-Dist: pyyaml (==6.0)
 Requires-Dist: readme-renderer (==37.3)
 Requires-Dist: requests (==2.28.2)
```

