# Comparing `tmp/dataverse_sdk-1.2.1.tar.gz` & `tmp/dataverse_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_sdk-1.2.1.tar", last modified: Tue May 21 02:04:17 2024, max compression
+gzip compressed data, was "dataverse_sdk-1.3.0.tar", last modified: Wed May 22 09:09:49 2024, max compression
```

## Comparing `dataverse_sdk-1.2.1.tar` & `dataverse_sdk-1.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.135285 dataverse_sdk-1.2.1/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14020 2024-05-21 02:04:17.135000 dataverse_sdk-1.2.1/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    13697 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.132289 dataverse_sdk-1.2.1/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.133172 dataverse_sdk-1.2.1/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    11172 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    37533 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse_sdk-1.2.1/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      740 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.133466 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      141 2024-05-20 09:34:51.000000 dataverse_sdk-1.2.1/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134145 dataverse_sdk-1.2.1/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1216 2024-05-21 02:03:44.000000 dataverse_sdk-1.2.1/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134477 dataverse_sdk-1.2.1/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse_sdk-1.2.1/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-21 02:04:17.134775 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14020 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       37 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-05-21 02:04:17.000000 dataverse_sdk-1.2.1/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-21 02:04:17.135329 dataverse_sdk-1.2.1/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      636 2024-05-21 02:03:44.000000 dataverse_sdk-1.2.1/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.616184 dataverse_sdk-1.3.0/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-22 09:09:49.615946 dataverse_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14273 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.612956 dataverse_sdk-1.3.0/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.613904 dataverse_sdk-1.3.0/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    11552 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    37893 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.0/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      776 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.614192 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      141 2024-05-20 09:34:51.000000 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615064 dataverse_sdk-1.3.0/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1216 2024-05-21 02:03:44.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615413 dataverse_sdk-1.3.0/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615733 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       37 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-22 09:09:49.616223 dataverse_sdk-1.3.0/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      636 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/setup.py
```

### Comparing `dataverse_sdk-1.2.1/PKG-INFO` & `dataverse_sdk-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: dataverse-sdk
-Version: 1.2.1
-Summary: Dataverse SDK For Python
-Home-page: 
-Author: LinkerVision
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10, <4
-Description-Content-Type: text/markdown
-Requires-Dist: pydantic==1.*
-Requires-Dist: requests
-Requires-Dist: httpx>=0.23.0
-
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in computer vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
   - Get Dataset by dataset-id
@@ -28,62 +15,79 @@
 
 ### Install the package
 
 ```
 pip install dataverse-sdk
 ```
 
-**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.9+](https://www.python.org/downloads/) to use this package.
+**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.10+](https://www.python.org/downloads/) to use this package.
 
 ### Create the client
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", service_id="xxxx-xxxx-xx-xxx", alias="default", force = False
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
+    host=DataverseHost.PRODUCTION, email="account-2", password="***", service_id="xxxx-xxxx-xx-xxx", alias="client2", force = False
+)
+assert client2 is get_connection()
+
+client3 = DataverseClient(
+    host=DataverseHost.PRODUCTION, email="XXX", password="", service_id="xxxx-xxxx-xx-xxx", access_token="xxx"
 )
 assert client2 is get_connection()
 ```
 
 * Input arguments:
 
 | Argument name      | Type/Options   | Default   | Description   |
 | :---                 |     :---    |     :---  |          :--- |
 | host        | str  | 	＊--    | the host url of the dataverse site    |
 | email  | str | ＊--  |  the email account of your dataverse workspace |
 | password  | str | ＊--  |  the password of your dataverse workspace  |
+| service_id  | str | ＊--   |  The service id of the dataverse you want to connect |
 | alias | str | 'default' |  the connection alias of your dataverse client |
 | force  | bool | False  |  whether force to replace the connection if the given alias exists |
+| access_token  | str | None   | instead of password to do authentication |
 
 
 ## Key concepts
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [Get User](#get-user)
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 * [List Models](#list-models)
 * [Get and Download Model](#get-model)
 
+### Get User
+
+The `get_user` method is to list the current user info.
+You can get the detail info, such as role, permission and user detail.
+
+```python
+user = client.get_user()
+```
+
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 * Example Usage:
 ```Python
 projects = client.list_projects(current_user = True,
                                 exclude_sensor_type=SensorType.LIDAR,
```

### Comparing `dataverse_sdk-1.2.1/README.md` & `dataverse_sdk-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: dataverse-sdk
+Version: 1.3.0
+Summary: Dataverse SDK For Python
+Home-page: 
+Author: LinkerVision
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10, <4
+Description-Content-Type: text/markdown
+Requires-Dist: pydantic==1.*
+Requires-Dist: requests
+Requires-Dist: httpx>=0.23.0
+
 # Dataverse SDK For Python
 Dataverse is a MLOPs platform for assisting in data selection, data visualization and model training in computer vision.
 Use Dataverse-SDK for Python to help you to interact with the Dataverse platform by Python. Currently, the library supports:
   - Create Project with your input ontology and sensors
   - Get Project by project-id
   - Create Dataset from your AWS/Azure storage or local
   - Get Dataset by dataset-id
@@ -15,62 +28,79 @@
 
 ### Install the package
 
 ```
 pip install dataverse-sdk
 ```
 
-**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.9+](https://www.python.org/downloads/) to use this package.
+**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.10+](https://www.python.org/downloads/) to use this package.
 
 ### Create the client
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", service_id="xxxx-xxxx-xx-xxx", alias="default", force = False
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
+    host=DataverseHost.PRODUCTION, email="account-2", password="***", service_id="xxxx-xxxx-xx-xxx", alias="client2", force = False
+)
+assert client2 is get_connection()
+
+client3 = DataverseClient(
+    host=DataverseHost.PRODUCTION, email="XXX", password="", service_id="xxxx-xxxx-xx-xxx", access_token="xxx"
 )
 assert client2 is get_connection()
 ```
 
 * Input arguments:
 
 | Argument name      | Type/Options   | Default   | Description   |
 | :---                 |     :---    |     :---  |          :--- |
 | host        | str  | 	＊--    | the host url of the dataverse site    |
 | email  | str | ＊--  |  the email account of your dataverse workspace |
 | password  | str | ＊--  |  the password of your dataverse workspace  |
+| service_id  | str | ＊--   |  The service id of the dataverse you want to connect |
 | alias | str | 'default' |  the connection alias of your dataverse client |
 | force  | bool | False  |  whether force to replace the connection if the given alias exists |
+| access_token  | str | None   | instead of password to do authentication |
 
 
 ## Key concepts
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [Get User](#get-user)
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 * [List Models](#list-models)
 * [Get and Download Model](#get-model)
 
+### Get User
+
+The `get_user` method is to list the current user info.
+You can get the detail info, such as role, permission and user detail.
+
+```python
+user = client.get_user()
+```
+
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 * Example Usage:
 ```Python
 projects = client.list_projects(current_user = True,
                                 exclude_sensor_type=SensorType.LIDAR,
```

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/__init__.py` & `dataverse_sdk-1.3.0/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/apis/backend.py` & `dataverse_sdk-1.3.0/dataverse_sdk/apis/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
     def __init__(
         self,
         host: str,
         email: str,
         password: str,
         service_id: str,
+        access_token: str = "",
     ):
         # TODO: Support api versioning
         self.host = host
         self.headers = {
             "Content-Type": "application/json",
             "X-Request-Service-Id": service_id,
         }
-        self.access_token = None
+        self.access_token = access_token
         self.email = email
         self.password = password
         self.login(email=email, password=password)
 
     def send_request(
         self,
         url: str,
@@ -100,32 +101,44 @@
             raise Exception(
                 f"[{parent_func}] request failed (kwargs: {kwargs})"
                 f", status code: {resp.status_code}, response detail: {resp.__dict__}"
             )
         return resp
 
     def login(self, email: str, password: str):
+        if email and password:
+            resp = self.send_request(
+                url=f"{self.host}/auth/users/jwt/",
+                method="post",
+                headers={"Content-Type": "application/json"},
+                data={"email": email, "password": password},
+            )
+            json_data = resp.json()
+            self.set_auth(access_token=json_data["access_token"])
+            return
+
+        if self.access_token:
+            self.set_auth(access_token=self.access_token)
+            return
+
         if email is None:
             raise ValueError("Can't login with null email.")
         if password is None:
             raise ValueError("Can't login with null password.")
 
-        resp = self.send_request(
-            url=f"{self.host}/auth/users/jwt/",
-            method="post",
-            headers={"Content-Type": "application/json"},
-            data={"email": email, "password": password},
-        )
-        json_data = resp.json()
-        self.set_auth(access_token=json_data["access_token"])
-
     def set_auth(self, access_token: str) -> None:
-        self.access_token = access_token
         self.headers["Authorization"] = f"Bearer {access_token}"
 
+    def get_user(self) -> dict:
+        return self.send_request(
+            url=f"{self.host}/auth/users/me/",
+            method="get",
+            headers=self.headers,
+        ).json()
+
     def create_project(
         self,
         name: str,
         ontology_data: dict,
         sensor_data: list[dict],
         project_tag_data: Optional[dict] = None,
         description: Optional[str] = None,
```

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/client.py` & `dataverse_sdk-1.3.0/dataverse_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 from collections import deque
 from typing import Optional
 
 from httpx import AsyncClient, AsyncHTTPTransport, Response, Timeout
 from pydantic import ValidationError
 
 from .apis.backend import BackendAPI
-from .connections import (
-    add_connection,
-    get_connection,
-)
+from .connections import add_connection, get_connection
 from .constants import DataverseHost
 from .exceptions.client import BadRequest, ClientConnectionError
 from .schemas.api import (
     AttributeAPISchema,
     DatasetAPISchema,
     OntologyAPISchema,
     ProjectAPISchema,
@@ -53,50 +50,60 @@
         self,
         host: DataverseHost,
         email: str,
         password: str,
         service_id: str,
         alias: str = "default",
         force: bool = False,
+        access_token: str = "",
     ) -> None:
         """
         Instantiate a Dataverse client.
 
         Parameters
         ----------
         host : DataverseHost
         email : str
         password : str
+        service_id : str
         alias: str
         force: bool, whether replace the connection if alias exists, default is False
+        access_token: str, optional, will try to use access_token to do authentication
 
         Raises
         ------
         ValueError
         """
         if host not in DataverseHost:
             raise ValueError("Invalid dataverse host, is the host available?")
         self.host = host
         self._api_client = None
         self.alias = alias
-        self._init_api_client(email=email, password=password, service_id=service_id)
+        self._init_api_client(
+            email=email,
+            password=password,
+            service_id=service_id,
+            access_token=access_token,
+        )
         add_connection(alias=alias, conn=self, force=force)
 
     def _init_api_client(
         self,
         email: str,
         password: str,
         service_id: str,
+        access_token: str = "",
     ) -> None:
         try:
             self._api_client = BackendAPI(
                 host=self.host,
                 email=email,
                 password=password,
                 service_id=service_id,
+                access_token=access_token,
             )
         except Exception as e:
             raise ClientConnectionError(f"Failed to initialize the api client: {e}")
 
     @staticmethod
     def _get_api_client(
         client: Optional["DataverseClient"] = None, client_alias: Optional[str] = None
@@ -115,14 +122,17 @@
     @staticmethod
     def get_client(alias: str = "default") -> "DataverseClient":
         try:
             return get_connection(alias)
         except KeyError:
             raise
 
+    def get_user(self):
+        return self._api_client.get_user()
+
     def create_project(
         self,
         name: str,
         ontology: Ontology,
         sensors: list[Sensor],
         project_tag: Optional[ProjectTag] = None,
         description: Optional[str] = None,
```

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/connections.py` & `dataverse_sdk-1.3.0/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/constants.py` & `dataverse_sdk-1.3.0/dataverse_sdk/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,14 @@
     def __contains__(cls, item):
         if cls._value_set is None:
             cls._value_set: set[Any] = {v.value for v in cls.__members__.values()}
         return item in cls._value_set
 
 
 class DataverseHost(str, Enum, metaclass=BaseEnumMeta):
-    DEV = "https://dev.dataverse.linkervision.ai"
-    DEV2 = "https://dev2.dataverse.linkervision.ai"
-    DEV3 = "https://dev3.dataverse.linkervision.ai"
-    STAGING = "https://staging.dataverse.linkervision.ai"
+    DEV = "https://dev.dataverse.linkervision.ai/curation"
+    DEV2 = "https://dev2.dataverse.linkervision.ai/curation"
+    DEV3 = "https://dev3.dataverse.linkervision.ai/curation"
+    STAGING = "https://staging.dataverse.linkervision.ai/curation"
     DEMO = "https://demo.dataverse.linkervision.ai"
     PRODUCTION = "https://dataverse.linkervision.ai"
     LOCAL = "http://localhost:8000"
```

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/schemas/api.py` & `dataverse_sdk-1.3.0/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/schemas/client.py` & `dataverse_sdk-1.3.0/dataverse_sdk/schemas/client.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/schemas/common.py` & `dataverse_sdk-1.3.0/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk/utils/utils.py` & `dataverse_sdk-1.3.0/dataverse_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk.egg-info/PKG-INFO` & `dataverse_sdk-1.3.0/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 1.2.1
+Version: 1.3.0
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
@@ -28,62 +28,79 @@
 
 ### Install the package
 
 ```
 pip install dataverse-sdk
 ```
 
-**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.9+](https://www.python.org/downloads/) to use this package.
+**Prerequisites**: You must have an Dataverse Platform Account and [Python 3.10+](https://www.python.org/downloads/) to use this package.
 
 ### Create the client
 
 Interaction with the Dataverse site starts with an instance of the `DataverseClient` class. You need site url, an email-account and its password to instantiate the client object.
 
 ```Python
 from dataverse_sdk import *
 from dataverse_sdk.connections import get_connection
 client = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="XXX", password="***", alias="default", force = False, service_id="xxxx-xxxx-xx-xxx"
+    host=DataverseHost.PRODUCTION, email="XXX", password="***", service_id="xxxx-xxxx-xx-xxx", alias="default", force = False
 )
 assert client is get_connection()
 
 # Should provide different alias if you are trying to connect to different workspaces
 client2 = DataverseClient(
-    host=DataverseHost.PRODUCTION, email="account-2", password="***", alias="client2", force = False,
+    host=DataverseHost.PRODUCTION, email="account-2", password="***", service_id="xxxx-xxxx-xx-xxx", alias="client2", force = False
+)
+assert client2 is get_connection()
+
+client3 = DataverseClient(
+    host=DataverseHost.PRODUCTION, email="XXX", password="", service_id="xxxx-xxxx-xx-xxx", access_token="xxx"
 )
 assert client2 is get_connection()
 ```
 
 * Input arguments:
 
 | Argument name      | Type/Options   | Default   | Description   |
 | :---                 |     :---    |     :---  |          :--- |
 | host        | str  | 	＊--    | the host url of the dataverse site    |
 | email  | str | ＊--  |  the email account of your dataverse workspace |
 | password  | str | ＊--  |  the password of your dataverse workspace  |
+| service_id  | str | ＊--   |  The service id of the dataverse you want to connect |
 | alias | str | 'default' |  the connection alias of your dataverse client |
 | force  | bool | False  |  whether force to replace the connection if the given alias exists |
+| access_token  | str | None   | instead of password to do authentication |
 
 
 ## Key concepts
 
 Once you've initialized a DataverseClient, you can interact with Dataverse from the initialized object.
 
 ## Examples
 
 The following sections provide examples for the most common DataVerse tasksm including:
 
+* [Get User](#get-user)
 * [List Projects](#list-projects)
 * [Create Project](#create-project)
 * [Get Project](#get-project)
 * [Create Dataset](#create-dataset)
 * [Get Dataset](#get-dataset)
 * [List Models](#list-models)
 * [Get and Download Model](#get-model)
 
+### Get User
+
+The `get_user` method is to list the current user info.
+You can get the detail info, such as role, permission and user detail.
+
+```python
+user = client.get_user()
+```
+
 ### List Projects
 The `list_projects` method will list all projects of the given sites.
 
 * Example Usage:
 ```Python
 projects = client.list_projects(current_user = True,
                                 exclude_sensor_type=SensorType.LIDAR,
```

### Comparing `dataverse_sdk-1.2.1/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse_sdk-1.3.0/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.2.1/setup.py` & `dataverse_sdk-1.3.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "1.2.1"
+PACKAGE_VERSION = "1.3.0"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

