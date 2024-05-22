# Comparing `tmp/sdkfabric_starwars-0.1.1.tar.gz` & `tmp/sdkfabric_starwars-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_starwars-0.1.1.tar", last modified: Mon May 20 15:28:37 2024, max compression
+gzip compressed data, was "sdkfabric_starwars-0.1.2.tar", last modified: Wed May 22 18:46:59 2024, max compression
```

## Comparing `sdkfabric_starwars-0.1.1.tar` & `sdkfabric_starwars-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.130717 sdkfabric_starwars-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/film_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/people_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/planet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/specie_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/starship_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 15:28:27.000000 sdkfabric_starwars-0.1.1/src/sdk/vehicle_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:28:37.138717 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 15:28:37.000000 sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:46:59.594452 sdkfabric_starwars-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 18:46:59.594452 sdkfabric_starwars-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-22 18:46:56.000000 sdkfabric_starwars-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:46:59.594452 sdkfabric_starwars-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:46:59.586452 sdkfabric_starwars-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:46:59.590452 sdkfabric_starwars-0.1.2/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/film.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/film_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/film_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/people.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/people_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/people_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/planet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/planet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/planet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/specie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/specie_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/specie_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/starship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/starship_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/starship_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/vehicle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-22 18:46:55.000000 sdkfabric_starwars-0.1.2/src/sdk/vehicle_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:46:59.594452 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 18:46:59.000000 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 18:46:59.000000 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:46:59.000000 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 18:46:59.000000 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 18:46:59.000000 sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/top_level.txt
```

### Comparing `sdkfabric_starwars-0.1.1/LICENSE` & `sdkfabric_starwars-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.1/PKG-INFO` & `sdkfabric_starwars-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.1
+Version: 0.1.2
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.1/README.md` & `sdkfabric_starwars-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.1/pyproject.toml` & `sdkfabric_starwars-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-starwars"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Starwars Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/client.py` & `sdkfabric_starwars-0.1.2/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/collection.py` & `sdkfabric_starwars-0.1.2/src/sdk/collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/film.py` & `sdkfabric_starwars-0.1.2/src/sdk/film.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Film resource is a single film.
+# A Film is a single film.
 class Film(BaseModel):
     title: Optional[str] = Field(default=None, alias="title")
     episode_id: Optional[int] = Field(default=None, alias="episode_id")
     opening_crawl: Optional[str] = Field(default=None, alias="opening_crawl")
     director: Optional[str] = Field(default=None, alias="director")
     producer: Optional[str] = Field(default=None, alias="producer")
     release_date: Optional[datetime.date] = Field(default=None, alias="release_date")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/film_tag.py` & `sdkfabric_starwars-0.1.2/src/sdk/people_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-FilmTag automatically generated by SDKgen please do not edit this file manually
+PeopleTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .film import Film
-from .film_collection import FilmCollection
+from .people import People
+from .people_collection import PeopleCollection
 
-class FilmTag(sdkgen.TagAbstract):
+class PeopleTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> FilmCollection:
+    def get_all(self, search: str) -> PeopleCollection:
         """
-        Get all the film resources
+        Get all the people
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/films", path_params)
+            url = self.parser.url("/people", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return FilmCollection.model_validate_json(json_data=response.content)
+                return PeopleCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> Film:
+    def get(self, id: str) -> People:
         """
-        Get a specific film resource
+        Get a specific people
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/films/:id", path_params)
+            url = self.parser.url("/people/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Film.model_validate_json(json_data=response.content)
+                return People.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/people.py` & `sdkfabric_starwars-0.1.2/src/sdk/people.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A People resource is an individual person or character within the Star Wars universe.
+# A People is an individual person or character within the Star Wars universe.
 class People(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     birth_year: Optional[str] = Field(default=None, alias="birth_year")
     eye_color: Optional[str] = Field(default=None, alias="eye_color")
     gender: Optional[str] = Field(default=None, alias="gender")
     hair_color: Optional[str] = Field(default=None, alias="hair_color")
     height: Optional[str] = Field(default=None, alias="height")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/people_tag.py` & `sdkfabric_starwars-0.1.2/src/sdk/vehicle_tag.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-PeopleTag automatically generated by SDKgen please do not edit this file manually
+VehicleTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .people import People
-from .people_collection import PeopleCollection
+from .vehicle import Vehicle
+from .vehicle_collection import VehicleCollection
 
-class PeopleTag(sdkgen.TagAbstract):
+class VehicleTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> PeopleCollection:
+    def get_all(self, search: str) -> VehicleCollection:
         """
-        Get all the people resources
+        Get all the vehicles
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/people", path_params)
+            url = self.parser.url("/vehicles", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return PeopleCollection.model_validate_json(json_data=response.content)
+                return VehicleCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> People:
+    def get(self, id: str) -> Vehicle:
         """
-        Get a specific people resource
+        Get a specific vehicle
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/people/:id", path_params)
+            url = self.parser.url("/vehicles/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return People.model_validate_json(json_data=response.content)
+                return Vehicle.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/planet.py` & `sdkfabric_starwars-0.1.2/src/sdk/planet.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Planet resource is a large mass, planet or planetoid in the Star Wars Universe, at the time of 0 ABY.
+# A Planet is a large mass, planet or planetoid in the Star Wars Universe, at the time of 0 ABY.
 class Planet(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     diameter: Optional[str] = Field(default=None, alias="diameter")
     rotation_period: Optional[str] = Field(default=None, alias="rotation_period")
     orbital_period: Optional[str] = Field(default=None, alias="orbital_period")
     gravity: Optional[str] = Field(default=None, alias="gravity")
     population: Optional[str] = Field(default=None, alias="population")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/planet_tag.py` & `sdkfabric_starwars-0.1.2/src/sdk/specie_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-PlanetTag automatically generated by SDKgen please do not edit this file manually
+SpecieTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .planet import Planet
-from .planet_collection import PlanetCollection
+from .specie import Specie
+from .specie_collection import SpecieCollection
 
-class PlanetTag(sdkgen.TagAbstract):
+class SpecieTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> PlanetCollection:
+    def get_all(self, search: str) -> SpecieCollection:
         """
-        Get all the planets resources
+        Get all the species
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/planets", path_params)
+            url = self.parser.url("/species", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return PlanetCollection.model_validate_json(json_data=response.content)
+                return SpecieCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> Planet:
+    def get(self, id: str) -> Specie:
         """
-        Get a specific planets resource
+        Get a specific specie
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/planets/:id", path_params)
+            url = self.parser.url("/species/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Planet.model_validate_json(json_data=response.content)
+                return Specie.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/root.py` & `sdkfabric_starwars-0.1.2/src/sdk/root.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/specie.py` & `sdkfabric_starwars-0.1.2/src/sdk/specie.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Species resource is a type of person or character within the Star Wars Universe.
+# A Species is a type of person or character within the Star Wars Universe.
 class Specie(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     classification: Optional[str] = Field(default=None, alias="classification")
     designation: Optional[str] = Field(default=None, alias="designation")
     average_height: Optional[str] = Field(default=None, alias="average_height")
     average_lifespan: Optional[str] = Field(default=None, alias="average_lifespan")
     eye_colors: Optional[str] = Field(default=None, alias="eye_colors")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/specie_tag.py` & `sdkfabric_starwars-0.1.2/src/sdk/planet_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-SpecieTag automatically generated by SDKgen please do not edit this file manually
+PlanetTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .specie import Specie
-from .specie_collection import SpecieCollection
+from .planet import Planet
+from .planet_collection import PlanetCollection
 
-class SpecieTag(sdkgen.TagAbstract):
+class PlanetTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> SpecieCollection:
+    def get_all(self, search: str) -> PlanetCollection:
         """
-        Get all the species resources
+        Get all the planets
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/species", path_params)
+            url = self.parser.url("/planets", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return SpecieCollection.model_validate_json(json_data=response.content)
+                return PlanetCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> Specie:
+    def get(self, id: str) -> Planet:
         """
-        Get a specific species resource
+        Get a specific planet
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/species/:id", path_params)
+            url = self.parser.url("/planets/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Specie.model_validate_json(json_data=response.content)
+                return Planet.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/starship.py` & `sdkfabric_starwars-0.1.2/src/sdk/vehicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 """
-starship automatically generated by SDKgen please do not edit this file manually
+vehicle automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Starship resource is a single transport craft that has hyperdrive capability.
-class Starship(BaseModel):
+# A Vehicle is a single transport craft that does not have hyperdrive capability.
+class Vehicle(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     model: Optional[str] = Field(default=None, alias="model")
-    starship_class: Optional[str] = Field(default=None, alias="starship_class")
+    vehicle_class: Optional[str] = Field(default=None, alias="vehicle_class")
     manufacturer: Optional[str] = Field(default=None, alias="manufacturer")
-    cost_in_credits: Optional[str] = Field(default=None, alias="cost_in_credits")
     length: Optional[str] = Field(default=None, alias="length")
+    cost_in_credits: Optional[str] = Field(default=None, alias="cost_in_credits")
     crew: Optional[str] = Field(default=None, alias="crew")
     passengers: Optional[str] = Field(default=None, alias="passengers")
     max_atmosphering_speed: Optional[str] = Field(default=None, alias="max_atmosphering_speed")
-    hyperdrive_rating: Optional[str] = Field(default=None, alias="hyperdrive_rating")
-    mglt: Optional[str] = Field(default=None, alias="MGLT")
     cargo_capacity: Optional[str] = Field(default=None, alias="cargo_capacity")
     consumables: Optional[str] = Field(default=None, alias="consumables")
     films: Optional[List[str]] = Field(default=None, alias="films")
     pilots: Optional[List[str]] = Field(default=None, alias="pilots")
     url: Optional[str] = Field(default=None, alias="url")
     created: Optional[datetime.datetime] = Field(default=None, alias="created")
     edited: Optional[datetime.datetime] = Field(default=None, alias="edited")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/starship_tag.py` & `sdkfabric_starwars-0.1.2/src/sdk/starship_tag.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class StarshipTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
     def get_all(self, search: str) -> StarshipCollection:
         """
-        Get all the starship resources
+        Get all the starships
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
@@ -40,15 +40,15 @@
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
     def get(self, id: str) -> Starship:
         """
-        Get a specific starship resource
+        Get a specific starship
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdk/vehicle.py` & `sdkfabric_starwars-0.1.2/src/sdk/starship.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
-vehicle automatically generated by SDKgen please do not edit this file manually
+starship automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
-# A Vehicle resource is a single transport craft that does not have hyperdrive capability.
-class Vehicle(BaseModel):
+# A Starship is a single transport craft that has hyperdrive capability.
+class Starship(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     model: Optional[str] = Field(default=None, alias="model")
-    vehicle_class: Optional[str] = Field(default=None, alias="vehicle_class")
+    starship_class: Optional[str] = Field(default=None, alias="starship_class")
     manufacturer: Optional[str] = Field(default=None, alias="manufacturer")
-    length: Optional[str] = Field(default=None, alias="length")
     cost_in_credits: Optional[str] = Field(default=None, alias="cost_in_credits")
+    length: Optional[str] = Field(default=None, alias="length")
     crew: Optional[str] = Field(default=None, alias="crew")
     passengers: Optional[str] = Field(default=None, alias="passengers")
     max_atmosphering_speed: Optional[str] = Field(default=None, alias="max_atmosphering_speed")
+    hyperdrive_rating: Optional[str] = Field(default=None, alias="hyperdrive_rating")
+    mglt: Optional[str] = Field(default=None, alias="MGLT")
     cargo_capacity: Optional[str] = Field(default=None, alias="cargo_capacity")
     consumables: Optional[str] = Field(default=None, alias="consumables")
     films: Optional[List[str]] = Field(default=None, alias="films")
     pilots: Optional[List[str]] = Field(default=None, alias="pilots")
     url: Optional[str] = Field(default=None, alias="url")
     created: Optional[datetime.datetime] = Field(default=None, alias="created")
     edited: Optional[datetime.datetime] = Field(default=None, alias="edited")
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/PKG-INFO` & `sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.1
+Version: 0.1.2
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.1/src/sdkfabric_starwars.egg-info/SOURCES.txt` & `sdkfabric_starwars-0.1.2/src/sdkfabric_starwars.egg-info/SOURCES.txt`

 * *Files identical despite different names*

