# Comparing `tmp/cdsetool-0.2.8.tar.gz` & `tmp/cdsetool-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsetool-0.2.8.tar", last modified: Wed Mar 20 16:20:32 2024, max compression
+gzip compressed data, was "cdsetool-0.2.9.tar", last modified: Mon May 13 15:00:09 2024, max compression
```

## Comparing `cdsetool-0.2.8.tar` & `cdsetool-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:20:32.887336 cdsetool-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-03-20 16:20:28.000000 cdsetool-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-03-20 16:20:32.887336 cdsetool-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-03-20 16:20:28.000000 cdsetool-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-20 16:20:28.000000 cdsetool-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:20:32.887336 cdsetool-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:20:32.879336 cdsetool-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:20:32.883336 cdsetool-0.2.8/src/cdsetool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/download.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-03-20 16:20:28.000000 cdsetool-0.2.8/src/cdsetool/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:20:32.883336 cdsetool-0.2.8/src/cdsetool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 16:20:32.000000 cdsetool-0.2.8/src/cdsetool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:00:09.034577 cdsetool-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 15:00:01.000000 cdsetool-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-13 15:00:09.034577 cdsetool-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-05-13 15:00:01.000000 cdsetool-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-13 15:00:01.000000 cdsetool-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 15:00:09.038577 cdsetool-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:00:09.030577 cdsetool-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:00:09.034577 cdsetool-0.2.9/src/cdsetool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7206 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-13 15:00:01.000000 cdsetool-0.2.9/src/cdsetool/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 15:00:09.034577 cdsetool-0.2.9/src/cdsetool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-13 15:00:09.000000 cdsetool-0.2.9/src/cdsetool.egg-info/top_level.txt
```

### Comparing `cdsetool-0.2.8/LICENSE` & `cdsetool-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdsetool-0.2.8/PKG-INFO` & `cdsetool-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: cdsetool
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools & CLI for interacting with CDSE product APIs
 Author-email: Jacob Vejby <javej@sdfi.dk>
 Project-URL: Homepage, https://github.com/SDFIdk/CDSETool
 Project-URL: Bug Tracker, https://github.com/SDFIdk/CDSETool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer~=0.9.0
+Requires-Dist: typer<0.13,>=0.9
 Requires-Dist: rich<13.8,>=13.6
 Requires-Dist: requests<2.32.0,>=2.28.1
 Requires-Dist: pyjwt[crypto]~=2.8.0
 Requires-Dist: geopandas>=0.13.2
 Provides-Extra: test
-Requires-Dist: black==24.3.0; extra == "test"
+Requires-Dist: black==24.4.2; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: requests-mock==1.11.0; extra == "test"
-Requires-Dist: pytest-mock==3.12.0; extra == "test"
+Requires-Dist: pytest==8.2.0; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: requests-mock==1.12.1; extra == "test"
+Requires-Dist: pytest-mock==3.14.0; extra == "test"
 
 # CDSETool
 
 ## About CDSETool
 This script downloads copernicus data from the Copernicus Data Space Ecosystem
 
 ## Quick start
@@ -92,15 +92,15 @@
   * [LICENSE](#license)
 
 ## Installation
 
 Install `cdsetool` using pip:
 
 ```bash
-pip install cdsetool==0.2.8
+pip install cdsetool==0.2.9
 ```
 
 ## Usage
 
 ### Querying features
 
 Querying is always done in batches, returning `len(results) <= maxRecords` records each time.
```

### Comparing `cdsetool-0.2.8/README.md` & `cdsetool-0.2.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
   * [LICENSE](#license)
 
 ## Installation
 
 Install `cdsetool` using pip:
 
 ```bash
-pip install cdsetool==0.2.8
+pip install cdsetool==0.2.9
 ```
 
 ## Usage
 
 ### Querying features
 
 Querying is always done in batches, returning `len(results) <= maxRecords` records each time.
```

### Comparing `cdsetool-0.2.8/pyproject.toml` & `cdsetool-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cdsetool"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Jacob Vejby", email="javej@sdfi.dk" },
 ]
 description = "Tools & CLI for interacting with CDSE product APIs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 dependencies = [
-  "typer ~= 0.9.0",
+  "typer >= 0.9,< 0.13",
   "rich >= 13.6,< 13.8",
   "requests >= 2.28.1,< 2.32.0",
   "pyjwt[crypto] ~= 2.8.0",
   "geopandas >= 0.13.2",
 ]
 [project.optional-dependencies]
 test = [
-    "black==24.3.0",
+    "black==24.4.2",
     "pylint==3.1.0",
-    "pytest==8.1.1",
-    "pytest-cov==4.1.0",
-    "requests-mock==1.11.0",
-    "pytest-mock==3.12.0",
+    "pytest==8.2.0",
+    "pytest-cov==5.0.0",
+    "requests-mock==1.12.1",
+    "pytest-mock==3.14.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/SDFIdk/CDSETool"
 "Bug Tracker" = "https://github.com/SDFIdk/CDSETool/issues"
 
 [project.scripts]
```

### Comparing `cdsetool-0.2.8/src/cdsetool/_processing.py` & `cdsetool-0.2.9/src/cdsetool/_processing.py`

 * *Files identical despite different names*

### Comparing `cdsetool-0.2.8/src/cdsetool/cli.py` & `cdsetool-0.2.9/src/cdsetool/cli.py`

 * *Files identical despite different names*

### Comparing `cdsetool-0.2.8/src/cdsetool/credentials.py` & `cdsetool-0.2.9/src/cdsetool/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,20 +52,28 @@
 
 class TokenClientConnectionError(Exception):
     """
     Raised when token connection fails.
     """
 
 
+class TokenExpiredSignatureError(Exception):
+    """
+    Raised when token signature has expired.
+    """
+
+
 class Credentials:  # pylint: disable=too-few-public-methods disable=too-many-instance-attributes
     """
     A class for handling credentials for the Copernicus Identity
     and Access Management (IAM) system
     """
 
+    RETRY_CODES = frozenset([413, 429, 500, 502, 503])
+
     def __init__(
         self,
         username=None,
         password=None,
         openid_configuration_endpoint=None,
         proxies=None,
     ):
@@ -73,28 +81,28 @@
         self.__password = password
 
         self.__proxies = proxies
         self.__retries = Retry(
             total=5,
             backoff_factor=0.5,
             raise_on_status=False,
-            status_forcelist=Retry.RETRY_AFTER_STATUS_CODES,
+            status_forcelist=self.RETRY_CODES,
         )
         self.__openid_conf = None
         self.__jwks = None
         self.__openid_configuration_endpoint = (
             openid_configuration_endpoint
             or "https://identity.dataspace.copernicus.eu"
             + "/auth/realms/CDSE/.well-known/openid-configuration"
         )
 
         self.__access_token = None
         self.__refresh_token = None
-        self.__access_token_expires = datetime.now()
-        self.__refresh_token_expires = datetime.now()
+        self.__access_token_expires = datetime.now() - timedelta(hours=8)
+        self.__refresh_token_expires = self.__access_token_expires
 
         self.__lock = threading.Lock()
 
         if self.__username is None or self.__password is None:
             self.__read_credentials()
 
         self.__ensure_tokens()
@@ -124,15 +132,15 @@
         session = self.__make_session(
             authorization=False,
             max_retries=Retry(
                 total=2,
                 backoff_factor=0.5,
                 allowed_methods=None,
                 raise_on_status=False,
-                status_forcelist=Retry.RETRY_AFTER_STATUS_CODES,
+                status_forcelist=self.RETRY_CODES,
             ),
             proxies=self.__proxies,
         )
         now = datetime.now()
         response = session.post(self.__token_endpoint, data=data, timeout=120)
 
         if response.status_code == 401:
@@ -171,20 +179,23 @@
                         "client_id": "cdse-public",
                     }
                 self.__token_exchange(data)
             try:
                 key = self.__jwk_client.get_signing_key_from_jwt(self.__access_token)
             except jwt.PyJWKClientConnectionError as e:
                 raise TokenClientConnectionError from e
-            jwt.decode(
-                self.__access_token,
-                key=key.key,
-                algorithms=key._algorithms,  # pylint: disable=protected-access
-                options={"verify_aud": False},
-            )
+            try:
+                jwt.decode(
+                    self.__access_token,
+                    key=key.key,
+                    algorithms=self.__id_token_signing_algos,  # pylint: disable=protected-access
+                    options={"verify_aud": False},
+                )
+            except jwt.ExpiredSignatureError as e:
+                raise TokenExpiredSignatureError from e
 
     def __read_credentials(self):
         try:
             self.__username, _, self.__password = netrc.netrc().authenticators(
                 self.__token_endpoint
             )
         except Exception as exc:
@@ -208,14 +219,18 @@
         return self.__openid_configuration["token_endpoint"]
 
     @property
     def __jwks_uri(self):
         return self.__openid_configuration["jwks_uri"]
 
     @property
+    def __id_token_signing_algos(self):
+        return self.__openid_configuration["id_token_signing_alg_values_supported"]
+
+    @property
     def __jwk_client(self):
         if self.__jwks:
             return self.__jwks
 
         self.__jwks = jwt.PyJWKClient(self.__jwks_uri)
 
         return self.__jwks
```

### Comparing `cdsetool-0.2.8/src/cdsetool/download.py` & `cdsetool-0.2.9/src/cdsetool/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,16 +6,22 @@
 """
 
 import os
 import random
 import tempfile
 import time
 import shutil
+from requests.exceptions import ChunkedEncodingError
+from urllib3.exceptions import ProtocolError
 from cdsetool._processing import _concurrent_process
-from cdsetool.credentials import Credentials, TokenClientConnectionError
+from cdsetool.credentials import (
+    Credentials,
+    TokenClientConnectionError,
+    TokenExpiredSignatureError,
+)
 from cdsetool.logger import NoopLogger
 from cdsetool.monitor import NoopMonitor
 
 
 def download_feature(feature, path, options=None):
     """
     Download a single feature
@@ -35,44 +41,52 @@
     result_path = os.path.join(path, filename)
 
     if not options.get("overwrite_existing", False) and os.path.exists(result_path):
         log.debug(f"File {result_path} already exists, skipping..")
         return filename
 
     with _get_monitor(options).status() as status:
-        (fd, tmp) = tempfile.mkstemp()  # pylint: disable=invalid-name
         status.set_filename(filename)
         attempts = 0
-        while attempts < 5:
+        while attempts < 10:
+            attempts += 1
             # Always get a new session, credentials might have expired.
             try:
                 session = _get_credentials(options).get_session()
-            except TokenClientConnectionError as e:
+            except (TokenClientConnectionError, TokenExpiredSignatureError) as e:
                 log.warning(e)
                 continue
             url = _follow_redirect(url, session)
             with session.get(url, stream=True) as response:
                 if response.status_code != 200:
                     log.warning(f"Status code {response.status_code}, retrying..")
-                    attempts += 1
                     time.sleep(60 * (1 + (random.random() / 4)))
                     continue
 
                 status.set_filesize(int(response.headers["Content-Length"]))
 
-                with open(fd, "wb") as file:
-                    for chunk in response.iter_content(chunk_size=1024 * 1024 * 5):
-                        file.write(chunk)
-                        status.add_progress(len(chunk))
+                with tempfile.NamedTemporaryFile() as file:
+                    # Server might not send all bytes specified by the
+                    # Content-Length header before closing connection.
+                    # Log as a warning and try again.
+                    try:
+                        for chunk in response.iter_content(chunk_size=1024 * 1024 * 5):
+                            file.write(chunk)
+                            status.add_progress(len(chunk))
+                    except (
+                        ChunkedEncodingError,
+                        ConnectionResetError,
+                        ProtocolError,
+                    ) as e:
+                        log.warning(e)
+                        continue
+                    shutil.copy(file.name, result_path)
 
-                shutil.move(tmp, result_path)
                 return filename
     log.error(f"Failed to download {filename}")
-    os.close(fd)
-    os.remove(tmp)
     return None
 
 
 def download_features(features, path, options=None):
     """
     Generator function that downloads all features in a result set
```

### Comparing `cdsetool-0.2.8/src/cdsetool/monitor.py` & `cdsetool-0.2.9/src/cdsetool/monitor.py`

 * *Files identical despite different names*

### Comparing `cdsetool-0.2.8/src/cdsetool/query.py` & `cdsetool-0.2.9/src/cdsetool/query.py`

 * *Files identical despite different names*

### Comparing `cdsetool-0.2.8/src/cdsetool.egg-info/PKG-INFO` & `cdsetool-0.2.9/src/cdsetool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: cdsetool
-Version: 0.2.8
+Version: 0.2.9
 Summary: Tools & CLI for interacting with CDSE product APIs
 Author-email: Jacob Vejby <javej@sdfi.dk>
 Project-URL: Homepage, https://github.com/SDFIdk/CDSETool
 Project-URL: Bug Tracker, https://github.com/SDFIdk/CDSETool/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: typer~=0.9.0
+Requires-Dist: typer<0.13,>=0.9
 Requires-Dist: rich<13.8,>=13.6
 Requires-Dist: requests<2.32.0,>=2.28.1
 Requires-Dist: pyjwt[crypto]~=2.8.0
 Requires-Dist: geopandas>=0.13.2
 Provides-Extra: test
-Requires-Dist: black==24.3.0; extra == "test"
+Requires-Dist: black==24.4.2; extra == "test"
 Requires-Dist: pylint==3.1.0; extra == "test"
-Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: pytest-cov==4.1.0; extra == "test"
-Requires-Dist: requests-mock==1.11.0; extra == "test"
-Requires-Dist: pytest-mock==3.12.0; extra == "test"
+Requires-Dist: pytest==8.2.0; extra == "test"
+Requires-Dist: pytest-cov==5.0.0; extra == "test"
+Requires-Dist: requests-mock==1.12.1; extra == "test"
+Requires-Dist: pytest-mock==3.14.0; extra == "test"
 
 # CDSETool
 
 ## About CDSETool
 This script downloads copernicus data from the Copernicus Data Space Ecosystem
 
 ## Quick start
@@ -92,15 +92,15 @@
   * [LICENSE](#license)
 
 ## Installation
 
 Install `cdsetool` using pip:
 
 ```bash
-pip install cdsetool==0.2.8
+pip install cdsetool==0.2.9
 ```
 
 ## Usage
 
 ### Querying features
 
 Querying is always done in batches, returning `len(results) <= maxRecords` records each time.
```

