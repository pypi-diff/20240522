# Comparing `tmp/ugrc-palletjack-4.3.1.tar.gz` & `tmp/ugrc-palletjack-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugrc-palletjack-4.3.1.tar", last modified: Mon Apr  1 22:56:40 2024, max compression
+gzip compressed data, was "ugrc-palletjack-4.4.0.tar", last modified: Wed May 22 17:51:16 2024, max compression
```

## Comparing `ugrc-palletjack-4.3.1.tar` & `ugrc-palletjack-4.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.126240 ugrc-palletjack-4.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.126240 ugrc-palletjack-4.3.1/src/palletjack/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    45152 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    38332 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/load.py
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-01 22:56:37.000000 ugrc-palletjack-4.3.1/src/palletjack/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 22:56:40.130240 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 22:56:40.000000 ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:51:16.732033 ugrc-palletjack-4.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-22 17:51:16.728033 ugrc-palletjack-4.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:51:16.732033 ugrc-palletjack-4.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:51:16.728033 ugrc-palletjack-4.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:51:16.728033 ugrc-palletjack-4.4.0/src/palletjack/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46281 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38332 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40269 2024-05-22 17:51:10.000000 ugrc-palletjack-4.4.0/src/palletjack/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 17:51:11.000000 ugrc-palletjack-4.4.0/src/palletjack/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:51:16.728033 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6737 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:51:16.000000 ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/zip-safe
```

### Comparing `ugrc-palletjack-4.3.1/LICENSE` & `ugrc-palletjack-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/PKG-INFO` & `ugrc-palletjack-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugrc-palletjack
-Version: 4.3.1
+Version: 4.4.0
 Summary: Updating AGOL feature services with data from external tables.
 Home-page: https://github.com/agrc/palletjack
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
 Keywords: gis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ugrc-palletjack-4.3.1/README.md` & `ugrc-palletjack-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/setup.py` & `ugrc-palletjack-4.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             "pdoc3==0.10.*",
             "pytest-cov>=3,<6",
             "pytest-instafail~=0.4",
             "pytest-mock>=3.10,<3.15",
             "pytest-ruff==0.*",
             "pytest-watch~=4.2",
             "pytest>=6,<9",
-            "black>=23.3,<24.4",
+            "black>=23.3,<24.5",
             "requests-mock==1.*",
             "ruff==0.0.*",
         ]
     },
     setup_requires=[
         "pytest-runner",
     ],
```

### Comparing `ugrc-palletjack-4.3.1/src/palletjack/__init__.py` & `ugrc-palletjack-4.4.0/src/palletjack/__init__.py`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/src/palletjack/extract.py` & `ugrc-palletjack-4.4.0/src/palletjack/extract.py`

 * *Files 2% similar despite different names*

```diff
@@ -907,16 +907,16 @@
 
     sandbox = False
 
     access_token_template = Template("https://$org.my.salesforce.com/services/oauth2/token")
     access_token_url = ""
     access_token = {}
 
-    query_template = Template("https://$org.my.salesforce.com/services/data/v58.0/query")
-    query_url = ""
+    org_template = Template("https://$org.my.salesforce.com")
+    org_url = ""
 
     client_secret = None
     client_id = None
     username = None
     password = None
 
     token_lease_in_days = 30
@@ -943,15 +943,15 @@
 
         if sandbox:
             self.username = credentials.username
             self.password = credentials.password
             org = org + ".sandbox"
 
         self.access_token_url = self.access_token_template.substitute(org=org)
-        self.query_url = self.query_template.substitute(org=org)
+        self.org_url = self.org_template.substitute(org=org)
 
         self.sandbox = sandbox
 
         self._class_logger = logging.getLogger(__name__).getChild(self.__class__.__name__)
 
     def _is_token_valid(self, token: dict[str, str]) -> bool:
         """Checks if the token is valid by looking at the issued_at field.
@@ -982,20 +982,21 @@
 
     def _get_token(self) -> dict[str, str]:
         """Gets a new Salesforce access token if the current one is expired."""
         if self._is_token_valid(self.access_token):
             return self.access_token
 
         form_data = {
-            "grant_type": "password",
+            "grant_type": "client_credentials",
             "client_id": self.client_id,
             "client_secret": self.client_secret,
         }
 
         if self.sandbox:
+            form_data["grant_type"] = "password"
             form_data["username"] = self.username
             form_data["password"] = self.password
 
         response = requests.post(
             self.access_token_url,
             data=form_data,
             headers={"Content-Type": "application/x-www-form-urlencoded"},
@@ -1006,40 +1007,64 @@
 
         response.raise_for_status()
 
         self.access_token = response.json()
 
         return self.access_token
 
-    def get_records(self, query) -> pd.DataFrame:
+    def get_records(self, query_endpoint, query_string) -> pd.DataFrame:
         """Queries the Salesforce API and returns the results as a dataframe.
 
         Args:
-            query (str): A SOQL query string.
+            query_endpoint (str): The REST endpoint to use for the query. Usually "/services/data/vXX.X/query".
+            query_string (str): A SOQL query string.
 
         Raises:
             ValueError: If the query fails.
 
         Returns:
             pd.Dataframe: A dataframe of the results.
         """
+
+        response_data = self._query_records(query_endpoint, {"q": query_string})
+
+        df = pd.DataFrame(response_data["records"])
+
+        while response_data["done"] is False:
+            response_data = self._query_records(response_data["nextRecordsUrl"])
+            df = pd.concat([df, pd.DataFrame(response_data["records"])])
+
+        return df.reset_index(drop=True)  #: the concatted index is just a repeat of 0:2000
+
+    def _query_records(self, query_endpoint, query_params=None) -> dict:
+        """Queries the Salesforce API and returns the results as a dictionary.
+
+        Args:
+            query_endpoint (str): The REST endpoint to use for the query, either 'query' or the nextRecordsUrl.
+            query_params (dict): A dictionary of params holding the SOQL query. Defaults to None for paged queries.
+
+        Raises:
+            ValueError: If the query fails.
+
+        Returns:
+            dict: A dictionary of the results.
+        """
         token = self._get_token()
 
-        response = requests.get(
-            self.query_url,
-            params={"q": query},
+        response = utils.retry(
+            requests.get,
+            f"{self.org_url}/{query_endpoint}",
+            params=query_params,
             headers={
                 "Authorization": f"Bearer {token['access_token']}",
             },
             timeout=self.soql_query_timeout_in_seconds,
         )
 
         try:
             response.raise_for_status()
         except requests.exceptions.HTTPError as error:
             self._class_logger.error("Error getting records from Salesforce %s", error)
 
             raise ValueError(f"Error getting records from Salesforce {response.json()}") from error
 
-        data = response.json()
-
-        return pd.DataFrame(data["records"])
+        return response.json()
```

### Comparing `ugrc-palletjack-4.3.1/src/palletjack/load.py` & `ugrc-palletjack-4.4.0/src/palletjack/load.py`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/src/palletjack/transform.py` & `ugrc-palletjack-4.4.0/src/palletjack/transform.py`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/src/palletjack/utils.py` & `ugrc-palletjack-4.4.0/src/palletjack/utils.py`

 * *Files identical despite different names*

### Comparing `ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/PKG-INFO` & `ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugrc-palletjack
-Version: 4.3.1
+Version: 4.4.0
 Summary: Updating AGOL feature services with data from external tables.
 Home-page: https://github.com/agrc/palletjack
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 Project-URL: Issue Tracker, https://github.com/agrc/palletjack/issues
 Keywords: gis
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ugrc-palletjack-4.3.1/src/ugrc_palletjack.egg-info/SOURCES.txt` & `ugrc-palletjack-4.4.0/src/ugrc_palletjack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

