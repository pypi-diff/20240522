# Comparing `tmp/astrapy-1.1.0.tar.gz` & `tmp/astrapy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrapy-1.1.0.tar", max compression
+gzip compressed data, was "astrapy-1.2.0.tar", max compression
```

## Comparing `astrapy-1.1.0.tar` & `astrapy-1.2.0.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0    11357 2023-10-19 21:10:53.110159 astrapy-1.1.0/LICENSE.md
--rw-r--r--   0        0        0    11564 2024-04-17 21:17:22.390941 astrapy-1.1.0/README.md
--rw-r--r--   0        0        0     2653 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/__init__.py
--rw-r--r--   0        0        0    82432 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/admin.py
--rw-r--r--   0        0        0      727 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/api/__init__.py
--rw-r--r--   0        0        0    17415 2024-04-16 08:29:58.955559 astrapy-1.1.0/astrapy/client.py
--rw-r--r--   0        0        0   214387 2024-04-27 10:55:31.525851 astrapy-1.1.0/astrapy/collection.py
--rw-r--r--   0        0        0     3004 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/constants.py
--rw-r--r--   0        0        0      569 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/__init__.py
--rw-r--r--   0        0        0     6136 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/api.py
--rw-r--r--   0        0        0     1692 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/core_types.py
--rw-r--r--   0        0        0   126840 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/db.py
--rw-r--r--   0        0        0     1009 2024-04-16 08:29:58.959558 astrapy-1.1.0/astrapy/core/defaults.py
--rw-r--r--   0        0        0      907 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/ids.py
--rw-r--r--   0        0        0    46165 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/ops.py
--rw-r--r--   0        0        0    13214 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/core/utils.py
--rw-r--r--   0        0        0    35775 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/cursors.py
--rw-r--r--   0        0        0    61320 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/database.py
--rw-r--r--   0        0        0      888 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/db/__init__.py
--rw-r--r--   0        0        0    28390 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/exceptions.py
--rw-r--r--   0        0        0      874 2024-04-16 08:29:58.963558 astrapy-1.1.0/astrapy/ids.py
--rw-r--r--   0        0        0    14210 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/info.py
--rw-r--r--   0        0        0    29870 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/operations.py
--rw-r--r--   0        0        0      717 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/ops/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 09:22:49.497793 astrapy-1.1.0/astrapy/py.typed
--rw-r--r--   0        0        0     6111 2024-04-16 08:29:58.967558 astrapy-1.1.0/astrapy/results.py
--rw-r--r--   0        0        0     2110 2024-04-27 10:55:31.525851 astrapy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12748 1970-01-01 00:00:00.000000 astrapy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-20 10:38:03.741711 astrapy-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0    11564 2024-05-03 14:48:57.304928 astrapy-1.2.0/README.md
+-rw-r--r--   0        0        0     2761 2024-05-22 09:39:50.067767 astrapy-1.2.0/astrapy/__init__.py
+-rw-r--r--   0        0        0   103813 2024-05-22 09:39:50.067767 astrapy-1.2.0/astrapy/admin.py
+-rw-r--r--   0        0        0      727 2024-04-11 09:17:31.515972 astrapy-1.2.0/astrapy/api/__init__.py
+-rw-r--r--   0        0        0     8620 2024-05-22 09:39:50.067767 astrapy-1.2.0/astrapy/api_commander.py
+-rw-r--r--   0        0        0     3265 2024-05-22 09:39:50.071767 astrapy-1.2.0/astrapy/api_options.py
+-rw-r--r--   0        0        0    20888 2024-05-22 09:39:50.071767 astrapy-1.2.0/astrapy/client.py
+-rw-r--r--   0        0        0   234094 2024-05-22 09:39:50.075767 astrapy-1.2.0/astrapy/collection.py
+-rw-r--r--   0        0        0     3137 2024-05-22 09:39:50.075767 astrapy-1.2.0/astrapy/constants.py
+-rw-r--r--   0        0        0      569 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/core/__init__.py
+-rw-r--r--   0        0        0     6484 2024-05-22 09:39:50.075767 astrapy-1.2.0/astrapy/core/api.py
+-rw-r--r--   0        0        0     1692 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/core/core_types.py
+-rw-r--r--   0        0        0   128508 2024-05-22 09:39:50.075767 astrapy-1.2.0/astrapy/core/db.py
+-rw-r--r--   0        0        0     1066 2024-05-22 09:39:50.075767 astrapy-1.2.0/astrapy/core/defaults.py
+-rw-r--r--   0        0        0      907 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/core/ids.py
+-rw-r--r--   0        0        0    46305 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/core/ops.py
+-rw-r--r--   0        0        0    13710 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/core/utils.py
+-rw-r--r--   0        0        0    35865 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/cursors.py
+-rw-r--r--   0        0        0    71303 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/database.py
+-rw-r--r--   0        0        0      888 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/db/__init__.py
+-rw-r--r--   0        0        0    28390 2024-05-09 13:24:53.849932 astrapy-1.2.0/astrapy/exceptions.py
+-rw-r--r--   0        0        0      874 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/ids.py
+-rw-r--r--   0        0        0    14723 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/info.py
+-rw-r--r--   0        0        0    29260 2024-05-22 09:39:50.079767 astrapy-1.2.0/astrapy/operations.py
+-rw-r--r--   0        0        0      717 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/ops/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-06 09:49:25.678169 astrapy-1.2.0/astrapy/py.typed
+-rw-r--r--   0        0        0     6111 2024-04-11 09:17:31.519972 astrapy-1.2.0/astrapy/results.py
+-rw-r--r--   0        0        0     2110 2024-05-22 09:39:50.083767 astrapy-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12748 1970-01-01 00:00:00.000000 astrapy-1.2.0/PKG-INFO
```

### Comparing `astrapy-1.1.0/LICENSE.md` & `astrapy-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/README.md` & `astrapy-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/__init__.py` & `astrapy-1.2.0/astrapy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 from astrapy.collection import (  # noqa: E402
     AsyncCollection,
     Collection,
 )
 from astrapy.admin import (  # noqa: E402
     AstraDBAdmin,
     AstraDBDatabaseAdmin,
+    DataAPIDatabaseAdmin,
 )
 from astrapy.client import (  # noqa: E402
     DataAPIClient,
 )
 
 import astrapy.ids  # noqa: E402
 import astrapy.constants  # noqa: E402
@@ -73,18 +74,21 @@
     "AstraDBAdmin",
     "AstraDBDatabaseAdmin",
     "AsyncCollection",
     "AsyncDatabase",
     "Collection",
     "Database",
     "DataAPIClient",
+    "DataAPIDatabaseAdmin",
     "__version__",
 ]
 
 
 __pdoc__ = {
     "api": False,
+    "api_commander": False,
+    "api_options": False,
     "core": False,
     "db": False,
     "ops": False,
     "ids": False,
 }
```

### Comparing `astrapy-1.1.0/astrapy/admin.py` & `astrapy-1.2.0/astrapy/admin.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,19 +21,23 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional, TYPE_CHECKING
 from dataclasses import dataclass
 
 import httpx
 
 from astrapy.core.ops import AstraDBOps
+from astrapy.core.defaults import DEFAULT_AUTH_HEADER
+from astrapy.api_commander import APICommander
 from astrapy.cursors import CommandCursor
+from astrapy.constants import Environment
 from astrapy.info import AdminDatabaseInfo, DatabaseInfo
 from astrapy.exceptions import (
     DevOpsAPIException,
     MultiCallTimeoutManager,
+    DataAPIFaultyResponseException,
     base_timeout_info,
     to_dataapi_timeout_exception,
     ops_recast_method_sync,
     ops_recast_method_async,
 )
 
 
@@ -51,54 +55,53 @@
 STATUS_ACTIVE = "ACTIVE"
 STATUS_PENDING = "PENDING"
 STATUS_INITIALIZING = "INITIALIZING"
 STATUS_ERROR = "ERROR"
 STATUS_TERMINATING = "TERMINATING"
 
 
-class Environment:
-    """
-    Admitted values for `environment` property, such as the one denoting databases.
-    """
-
-    def __init__(self) -> None:
-        raise NotImplementedError
-
-    PROD = "prod"
-    DEV = "dev"
-    TEST = "test"
-
-
 database_id_matcher = re.compile(
     "^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
 )
 
 api_endpoint_parser = re.compile(
     r"https://"
     r"([0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12})"
     r"-"
     r"([a-z0-9\-]+)"
     r".apps.astra[\-]{0,1}"
     r"(dev|test)?"
     r".datastax.com"
 )
 
+generic_api_url_matcher = re.compile(r"^https?:\/\/[a-zA-Z0-9.]+(\:[0-9]{1,6}){0,1}$")
+
 
 DEV_OPS_URL_MAP = {
     Environment.PROD: "https://api.astra.datastax.com",
     Environment.DEV: "https://api.dev.cloud.datastax.com",
     Environment.TEST: "https://api.test.cloud.datastax.com",
 }
 
 API_ENDPOINT_TEMPLATE_MAP = {
     Environment.PROD: "https://{database_id}-{region}.apps.astra.datastax.com",
     Environment.DEV: "https://{database_id}-{region}.apps.astra-dev.datastax.com",
     Environment.TEST: "https://{database_id}-{region}.apps.astra-test.datastax.com",
 }
 
+API_PATH_ENV_MAP = {
+    Environment.DSE: "",
+    Environment.OTHER: "",
+}
+
+API_VERSION_ENV_MAP = {
+    Environment.DSE: "v1",
+    Environment.OTHER: "v1",
+}
+
 
 @dataclass
 class ParsedAPIEndpoint:
     """
     The results of successfully parsing an Astra DB API endpoint, for internal
     by database metadata-related functions.
 
@@ -133,21 +136,45 @@
             region=d_re,
             environment=d_en_x if d_en_x else "prod",
         )
     else:
         return None
 
 
+def parse_generic_api_url(api_endpoint: str) -> Optional[str]:
+    """
+    Validate a generic API Endpoint string,
+    such as `http://10.1.1.1:123` or `https://my.domain`.
+
+    Args:
+        api_endpoint: a string supposedly expressing a valid API Endpoint
+        (not necessarily an Astra DB one).
+
+    Returns:
+        a normalized (stripped) version of the endpoint if valid. If invalid,
+        return None.
+    """
+    if api_endpoint and api_endpoint[-1] == "/":
+        _api_endpoint = api_endpoint[:-1]
+    else:
+        _api_endpoint = api_endpoint
+    match = generic_api_url_matcher.match(_api_endpoint)
+    if match:
+        return match[0].rstrip("/")
+    else:
+        return None
+
+
 def build_api_endpoint(environment: str, database_id: str, region: str) -> str:
     """
     Build the API Endpoint full strings from database parameters.
 
     Args:
-        environment: a label, whose value is one of Environment.PROD,
-            Environment.DEV or Environment.TEST.
+        environment: a label, whose value can be Environment.PROD
+            or another of Environment.* for which this operation makes sense.
         database_id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
         region: a region ID, such as "us-west1".
 
     Returns:
         the endpoint string, such as "https://01234567-...-eu-west1.apps.datastax.com"
     """
 
@@ -385,15 +412,15 @@
         environment: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
         dev_ops_url: Optional[str] = None,
         dev_ops_api_version: Optional[str] = None,
     ) -> None:
         self.token = token
-        self.environment = environment or Environment.PROD
+        self.environment = (environment or Environment.PROD).lower()
         if dev_ops_url is None:
             self.dev_ops_url = DEV_OPS_URL_MAP[self.environment]
         else:
             self.dev_ops_url = dev_ops_url
         self._caller_name = caller_name
         self._caller_version = caller_version
         self._dev_ops_url = dev_ops_url
@@ -1165,14 +1192,15 @@
         )
         return Database(
             api_endpoint=_api_endpoint,
             token=_token,
             namespace=_namespace,
             caller_name=self._caller_name,
             caller_version=self._caller_version,
+            environment=self.environment,
             api_path=api_path,
             api_version=api_version,
         )
 
     def get_async_database(
         self,
         id: str,
@@ -1204,14 +1232,16 @@
 class DatabaseAdmin(ABC):
     """
     An abstract class defining the interface for a database admin object.
     This supports generic namespace crud, as well as spawning databases,
     without committing to a specific database architecture (e.g. Astra DB).
     """
 
+    environment: str
+
     @abstractmethod
     def list_namespaces(self, *pargs: Any, **kwargs: Any) -> List[str]:
         """Get a list of namespaces for the database."""
         ...
 
     @abstractmethod
     def create_namespace(self, name: str, *pargs: Any, **kwargs: Any) -> Dict[str, Any]:
@@ -1265,15 +1295,15 @@
         """Get an AsyncDatabase object from this database admin."""
         ...
 
 
 class AstraDBDatabaseAdmin(DatabaseAdmin):
     """
     An "admin" object, able to perform administrative tasks at the namespaces level
-    (i.e. within a certani database), such as creating/listing/dropping namespaces.
+    (i.e. within a certain database), such as creating/listing/dropping namespaces.
 
     This is one layer below the AstraDBAdmin concept, in that it is tied to
     a single database and enables admin work within it. As such, it is generally
     created by a method call on an AstraDBAdmin.
 
     Args:
         id: e. g. "01234567-89ab-cdef-0123-456789abcdef".
@@ -1314,15 +1344,15 @@
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
         dev_ops_url: Optional[str] = None,
         dev_ops_api_version: Optional[str] = None,
     ) -> None:
         self.id = id
         self.token = token
-        self.environment = environment or Environment.PROD
+        self.environment = (environment or Environment.PROD).lower()
         self._astra_db_admin = AstraDBAdmin(
             token=self.token,
             environment=self.environment,
             caller_name=caller_name,
             caller_version=caller_version,
             dev_ops_url=dev_ops_url,
             dev_ops_api_version=dev_ops_api_version,
@@ -2124,7 +2154,536 @@
             token=token,
             namespace=namespace,
             region=region,
             api_path=api_path,
             api_version=api_version,
             max_time_ms=max_time_ms,
         ).to_async()
+
+
+class DataAPIDatabaseAdmin(DatabaseAdmin):
+    """
+    An "admin" object for non-Astra Data API environments, to perform administrative
+    tasks at the namespaces level such as creating/listing/dropping namespaces.
+
+    Conforming to the architecture of non-Astra deployments of the Data API,
+    this object works within the one existing database. It is within that database
+    that the namespace CRUD operations (and possibly other admin operations)
+    are performed. Since non-Astra environment lack the concept of an overall
+    admin (such as the all-databases AstraDBAdmin class), a `DataAPIDatabaseAdmin`
+    is generally created by invoking the `get_database_admin` method of the
+    corresponding `Database` object (which in turn is spawned by a DataAPIClient).
+
+    Args:
+        api_endpoint: the full URI to access the Data API,
+            e.g. "http://localhost:8181".
+        token: an access token with enough permission to perform admin tasks.
+        environment: a label, whose value is one of Environment.OTHER (default)
+            or other non-Astra environment values in the `Environment` enum.
+        api_path: path to append to the API Endpoint. In typical usage, this
+            should be left to its default of "".
+        api_version: version specifier to append to the API path. In typical
+            usage, this should be left to its default of "v1".
+        caller_name: name of the application, or framework, on behalf of which
+            the admin API calls are performed. This ends up in the request user-agent.
+        caller_version: version of the caller.
+
+    Example:
+        >>> from astrapy import DataAPIClient
+        >>> from astrapy.constants import Environment
+        >>>
+        >>> token = "Cassandra:..."
+        >>> endpoint = "http://localhost:8181"
+        >>>
+        >>> client = DataAPIClient(
+        >>>     token="Cassandra:Y2Fzc2FuZHJh:Y2Fzc2FuZHJh",
+        >>>     environment=Environment.OTHER,
+        >>> )
+        >>> database = client.get_database_by_api_endpoint(endpoint)
+        >>> admin_for_my_db = database.get_database_admin()
+        >>>
+        >>> admin_for_my_db.list_namespaces()
+        ['namespace1', 'namespace2']
+    """
+
+    def __init__(
+        self,
+        api_endpoint: str,
+        *,
+        token: str,
+        environment: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> None:
+        self.environment = (environment or Environment.OTHER).lower()
+        self.token = token
+        self.api_endpoint = api_endpoint
+        #
+        self.caller_name = caller_name
+        self.caller_version = caller_version
+        #
+        self._api_path = api_path if api_path is not None else ""
+        self._api_version = api_version if api_version is not None else ""
+        #
+        self._commander_headers = {
+            DEFAULT_AUTH_HEADER: token,
+        }
+        self._api_commander = APICommander(
+            api_endpoint=self.api_endpoint,
+            path="/".join(comp for comp in [self._api_path, self._api_version] if comp),
+            headers=self._commander_headers,
+            callers=[(self.caller_name, self.caller_version)],
+        )
+
+    def __repr__(self) -> str:
+        env_desc = f', environment="{self.environment}"'
+        return (
+            f'{self.__class__.__name__}(endpoint="{self.api_endpoint}", '
+            f'"{self.token[:12]}..."{env_desc})'
+        )
+
+    def __eq__(self, other: Any) -> bool:
+        if isinstance(other, DataAPIDatabaseAdmin):
+            return all(
+                [
+                    self.environment == other.environment,
+                    self._api_commander == other._api_commander,
+                ]
+            )
+        else:
+            return False
+
+    def _copy(
+        self,
+        api_endpoint: Optional[str] = None,
+        token: Optional[str] = None,
+        environment: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> DataAPIDatabaseAdmin:
+        return DataAPIDatabaseAdmin(
+            api_endpoint=api_endpoint or self.api_endpoint,
+            token=token or self.token,
+            environment=environment or self.environment,
+            api_path=api_path or self._api_path,
+            api_version=api_version or self._api_version,
+            caller_name=caller_name or self.caller_name,
+            caller_version=caller_version or self.caller_version,
+        )
+
+    def with_options(
+        self,
+        *,
+        api_endpoint: Optional[str] = None,
+        token: Optional[str] = None,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> DataAPIDatabaseAdmin:
+        """
+        Create a clone of this DataAPIDatabaseAdmin with some changed attributes.
+
+        Args:
+            api_endpoint: the full URI to access the Data API,
+                e.g. "http://localhost:8181".
+            token: an access token with enough permission to perform admin tasks.
+            caller_name: name of the application, or framework, on behalf of which
+                the admin API calls are performed. This ends up in the request user-agent.
+            caller_version: version of the caller.
+
+        Returns:
+            a new DataAPIDatabaseAdmin instance.
+
+        Example:
+            >>> admin_for_my_other_db = admin_for_my_db.with_options(
+            ...     api_endpoint="http://10.1.1.5:8181",
+            ... )
+        """
+
+        return self._copy(
+            api_endpoint=api_endpoint,
+            token=token,
+            caller_name=caller_name,
+            caller_version=caller_version,
+        )
+
+    def set_caller(
+        self,
+        caller_name: Optional[str] = None,
+        caller_version: Optional[str] = None,
+    ) -> None:
+        """
+        Set a new identity for the application/framework on behalf of which
+        the DevOps API calls will be performed (the "caller").
+
+        New objects spawned from this client afterwards will inherit the new settings.
+
+        Args:
+            caller_name: name of the application, or framework, on behalf of which
+                the DevOps API calls are performed. This ends up in the request user-agent.
+            caller_version: version of the caller.
+
+        Example:
+            >>> admin_for_my_db.set_caller(
+            ...     caller_name="the_caller",
+            ...     caller_version="0.1.0",
+            ... )
+        """
+
+        logger.info(f"setting caller to {caller_name}/{caller_version}")
+        self.caller_name = caller_name
+        self.caller_version = caller_version
+        self._api_commander = APICommander(
+            api_endpoint=self.api_endpoint,
+            path="/".join(comp for comp in [self._api_path, self._api_version] if comp),
+            headers=self._commander_headers,
+            callers=[(self.caller_name, self.caller_version)],
+        )
+
+    def list_namespaces(self, *, max_time_ms: Optional[int] = None) -> List[str]:
+        """
+        Query the API for a list of the namespaces in the database.
+
+        Args:
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
+
+        Returns:
+            A list of the namespaces, each a string, in no particular order.
+
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'staging_namespace']
+        """
+        logger.info("getting list of namespaces")
+        fn_response = self._api_commander.request(
+            payload={"findNamespaces": {}},
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if "namespaces" not in fn_response.get("status", {}):
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from findNamespaces API command.",
+                raw_response=fn_response,
+            )
+        else:
+            logger.info("finished getting list of namespaces")
+            return fn_response["status"]["namespaces"]  # type: ignore[no-any-return]
+
+    def create_namespace(
+        self,
+        name: str,
+        *,
+        replication_options: Optional[Dict[str, Any]] = None,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Create a namespace in the database, returning {'ok': 1} if successful.
+
+        Args:
+            name: the namespace name. If supplying a namespace that exists
+                already, the method call proceeds as usual, no errors are
+                raised, and the whole invocation is a no-op.
+            replication_options: this dictionary can specify the options about
+                replication of the namespace (across database nodes). If provided,
+                it must have a structure similar to:
+                `{"class": "SimpleStrategy", "replication_factor": 1}`.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace']
+            >>> admin_for_my_db.create_namespace("that_other_one")
+            {'ok': 1}
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+        """
+        options = {
+            k: v
+            for k, v in {
+                "replication": replication_options,
+            }.items()
+            if v
+        }
+        payload = {
+            "createNamespace": {
+                **{"name": name},
+                **({"options": options} if options else {}),
+            }
+        }
+        logger.info("creating namespace")
+        cn_response = self._api_commander.request(
+            payload=payload,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if (cn_response.get("status") or {}).get("ok") != 1:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from createNamespace API command.",
+                raw_response=cn_response,
+            )
+        else:
+            logger.info("finished creating namespace")
+            return cn_response["status"]  # type: ignore[no-any-return]
+
+    def drop_namespace(
+        self,
+        name: str,
+        *,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Drop (delete) a namespace from the database.
+
+        Args:
+            name: the namespace to delete. If it does not exist in this database,
+                an error is raised.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+            >>> admin_for_my_db.drop_namespace("that_other_one")
+            {'ok': 1}
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace']
+        """
+        logger.info("dropping namespace")
+        dn_response = self._api_commander.request(
+            payload={"dropNamespace": {"name": name}},
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if (dn_response.get("status") or {}).get("ok") != 1:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from dropNamespace API command.",
+                raw_response=dn_response,
+            )
+        else:
+            logger.info("finished dropping namespace")
+            return dn_response["status"]  # type: ignore[no-any-return]
+
+    async def async_list_namespaces(
+        self, *, max_time_ms: Optional[int] = None
+    ) -> List[str]:
+        """
+        Query the API for a list of the namespaces in the database.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            max_time_ms: a timeout, in milliseconds, for the DevOps API request.
+
+        Returns:
+            A list of the namespaces, each a string, in no particular order.
+
+        Example:
+            >>> asyncio.run(admin_for_my_db.async_list_namespaces())
+            ['default_keyspace', 'staging_namespace']
+        """
+        logger.info("getting list of namespaces, async")
+        fn_response = await self._api_commander.async_request(
+            payload={"findNamespaces": {}},
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if "namespaces" not in fn_response.get("status", {}):
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from findNamespaces API command.",
+                raw_response=fn_response,
+            )
+        else:
+            logger.info("finished getting list of namespaces, async")
+            return fn_response["status"]["namespaces"]  # type: ignore[no-any-return]
+
+    async def async_create_namespace(
+        self,
+        name: str,
+        *,
+        replication_options: Optional[Dict[str, Any]] = None,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Create a namespace in the database, returning {'ok': 1} if successful.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            name: the namespace name. If supplying a namespace that exists
+                already, the method call proceeds as usual, no errors are
+                raised, and the whole invocation is a no-op.
+            replication_options: this dictionary can specify the options about
+                replication of the namespace (across database nodes). If provided,
+                it must have a structure similar to:
+                `{"class": "SimpleStrategy", "replication_factor": 1}`.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the creation request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace']
+            >>> asyncio.run(admin_for_my_db.async_create_namespace(
+            ...     "that_other_one"
+            ... ))
+            {'ok': 1}
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace', 'that_other_one']
+        """
+        options = {
+            k: v
+            for k, v in {
+                "replication": replication_options,
+            }.items()
+            if v
+        }
+        payload = {
+            "createNamespace": {
+                **{"name": name},
+                **({"options": options} if options else {}),
+            }
+        }
+        logger.info("creating namespace, async")
+        cn_response = await self._api_commander.async_request(
+            payload=payload,
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if (cn_response.get("status") or {}).get("ok") != 1:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from createNamespace API command.",
+                raw_response=cn_response,
+            )
+        else:
+            logger.info("finished creating namespace, async")
+            return cn_response["status"]  # type: ignore[no-any-return]
+
+    async def async_drop_namespace(
+        self,
+        name: str,
+        *,
+        max_time_ms: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """
+        Drop (delete) a namespace from the database.
+        Async version of the method, for use in an asyncio context.
+
+        Args:
+            name: the namespace to delete. If it does not exist in this database,
+                an error is raised.
+            max_time_ms: a timeout, in milliseconds, for the whole requested
+                operation to complete.
+                Note that a timeout is no guarantee that the deletion request
+                has not reached the API server.
+
+        Returns:
+            A dictionary of the form {"ok": 1} in case of success.
+            Otherwise, an exception is raised.
+
+        Example:
+            >>> admin_for_my_db.list_namespaces()
+            ['that_other_one', 'default_keyspace']
+            >>> asyncio.run(admin_for_my_db.async_drop_namespace(
+            ...     "that_other_one"
+            ... ))
+            {'ok': 1}
+            >>> admin_for_my_db.list_namespaces()
+            ['default_keyspace']
+        """
+        logger.info("dropping namespace")
+        dn_response = await self._api_commander.async_request(
+            payload={"dropNamespace": {"name": name}},
+            timeout_info=base_timeout_info(max_time_ms),
+        )
+        if (dn_response.get("status") or {}).get("ok") != 1:
+            raise DataAPIFaultyResponseException(
+                text="Faulty response from dropNamespace API command.",
+                raw_response=dn_response,
+            )
+        else:
+            logger.info("finished dropping namespace")
+            return dn_response["status"]  # type: ignore[no-any-return]
+
+    def get_database(
+        self,
+        *,
+        token: Optional[str] = None,
+        namespace: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+    ) -> Database:
+        """
+        Create a Database instance out of this class for working with the data in it.
+
+        Args:
+            token: if supplied, is passed to the Database instead of
+                the one set for this object. Useful if one wants to work in
+                a least-privilege manner, limiting the permissions for non-admin work.
+            namespace: an optional namespace to set in the resulting Database.
+                If not provided, the default namespace is used.
+            api_path: path to append to the API Endpoint. In typical usage, this
+                should be left to its default of "".
+            api_version: version specifier to append to the API path. In typical
+                usage, this should be left to its default of "v1".
+
+        Returns:
+            A Database object, ready to be used for working with data and collections.
+
+        Example:
+            >>> my_db = admin_for_my_db.get_database()
+            >>> my_db.list_collection_names()
+            ['movies', 'another_collection']
+
+        Note:
+            creating an instance of Database does not trigger actual creation
+            of the database itself, which should exist beforehand.
+        """
+
+        # lazy importing here to avoid circular dependency
+        from astrapy import Database
+
+        return Database(
+            api_endpoint=self.api_endpoint,
+            token=token or self.token,
+            namespace=namespace,
+            caller_name=self.caller_name,
+            caller_version=self.caller_version,
+            environment=self.environment,
+            api_path=api_path,
+            api_version=api_version,
+        )
+
+    def get_async_database(
+        self,
+        *,
+        token: Optional[str] = None,
+        namespace: Optional[str] = None,
+        api_path: Optional[str] = None,
+        api_version: Optional[str] = None,
+    ) -> AsyncDatabase:
+        """
+        Create an AsyncDatabase instance for the database, to be used
+        when doing data-level work (such as creating/managing collections).
+
+        This method has identical behavior and signature as the sync
+        counterpart `get_database`: please see that one for more details.
+        """
+        return self.get_database(
+            token=token,
+            namespace=namespace,
+            api_path=api_path,
+            api_version=api_version,
+        ).to_async()
```

### Comparing `astrapy-1.1.0/astrapy/api/__init__.py` & `astrapy-1.2.0/astrapy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/client.py` & `astrapy-1.2.0/astrapy/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 from __future__ import annotations
 
 import logging
 import re
 from typing import Any, Dict, Optional, TYPE_CHECKING
 
 from astrapy.admin import (
-    Environment,
     api_endpoint_parser,
     build_api_endpoint,
     database_id_matcher,
     fetch_raw_database_info_from_id_token,
     parse_api_endpoint,
+    parse_generic_api_url,
 )
+from astrapy.constants import Environment
 
 
 if TYPE_CHECKING:
     from astrapy import AsyncDatabase, Database
     from astrapy.admin import AstraDBAdmin
 
 
@@ -44,17 +45,17 @@
     The client is created by passing a suitable Access Token. Starting from the
     client:
         - databases (Database and AsyncDatabase) are created for working with data
         - AstraDBAdmin objects can be created for admin-level work
 
     Args:
         token: an Access Token to the database. Example: `"AstraCS:xyz..."`.
-        environment: a string representing the target Astra environment.
+        environment: a string representing the target Data API environment.
             It can be left unspecified for the default value of `Environment.PROD`;
-            other values are `Environment.DEV` and `Environment.TEST`.
+            other values include `Environment.OTHER`, `Environment.DSE`.
         caller_name: name of the application, or framework, on behalf of which
             the Data API and DevOps API calls are performed. This ends up in
             the request user-agent.
         caller_version: version of the caller.
 
     Example:
         >>> from astrapy import DataAPIClient
@@ -76,15 +77,19 @@
         token: str,
         *,
         environment: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> None:
         self.token = token
-        self.environment = environment or Environment.PROD
+        self.environment = (environment or Environment.PROD).lower()
+
+        if self.environment not in Environment.values:
+            raise ValueError(f"Unsupported `environment` value: '{self.environment}'.")
+
         self._caller_name = caller_name
         self._caller_version = caller_version
 
     def __repr__(self) -> str:
         env_desc: str
         if self.environment == Environment.PROD:
             env_desc = ""
@@ -102,23 +107,26 @@
                     self._caller_version == other._caller_version,
                 ]
             )
         else:
             return False
 
     def __getitem__(self, database_id_or_api_endpoint: str) -> Database:
-        if re.match(database_id_matcher, database_id_or_api_endpoint):
-            return self.get_database(database_id_or_api_endpoint)
-        elif re.match(api_endpoint_parser, database_id_or_api_endpoint):
-            return self.get_database_by_api_endpoint(database_id_or_api_endpoint)
+        if self.environment in Environment.astra_db_values:
+            if re.match(database_id_matcher, database_id_or_api_endpoint):
+                return self.get_database(database_id_or_api_endpoint)
+            elif re.match(api_endpoint_parser, database_id_or_api_endpoint):
+                return self.get_database_by_api_endpoint(database_id_or_api_endpoint)
+            else:
+                raise ValueError(
+                    "The provided input does not look like either a database ID "
+                    f"or an API endpoint ('{database_id_or_api_endpoint}')."
+                )
         else:
-            raise ValueError(
-                "The provided input does not look like either a database ID "
-                f"or an API endpoint ('{database_id_or_api_endpoint}')."
-            )
+            return self.get_database_by_api_endpoint(database_id_or_api_endpoint)
 
     def _copy(
         self,
         *,
         token: Optional[str] = None,
         environment: Optional[str] = None,
         caller_name: Optional[str] = None,
@@ -199,84 +207,121 @@
         api_version: Optional[str] = None,
         max_time_ms: Optional[int] = None,
     ) -> Database:
         """
         Get a Database object from this client, for doing data-related work.
 
         Args:
-            id: the target database ID. The database must exist for the resulting
-                object to be effectively used; in other words, this invocation
+            id: the target database ID or the corresponding API Endpoint.
+                The database must exist already for the resulting object
+                to be effectively used; in other words, this invocation
                 does not create the database, just the object instance.
                 Actual admin work can be achieved by using the AstraDBAdmin object.
             token: if supplied, is passed to the Database instead of the client token.
             namespace: if provided, is passed to the Database
                 (it is left to the default otherwise).
             region: the region to use for connecting to the database. The
                 database must be located in that region.
-                Note that if this parameter is not passed, an additional
-                DevOps API request is made to determine the default region
-                and use it subsequently.
+                The region cannot be specified when he API endoint is used as `id`.
+                Note that if this parameter is not passed, and cannot be inferred
+                from the API endpoint, an additional DevOps API request is made
+                to determine the default region and use it subsequently.
             api_path: path to append to the API Endpoint. In typical usage, this
                 should be left to its default of "/api/json".
             api_version: version specifier to append to the API path. In typical
                 usage, this should be left to its default of "v1".
             max_time_ms: a timeout, in milliseconds, for the DevOps API
                 HTTP request should it be necessary (see the `region` argument).
 
         Returns:
             a Database object with which to work on Data API collections.
 
         Example:
             >>> my_db0 = my_client.get_database("01234567-...")
-            >>> my_db1 = my_client.get_database("01234567-...", token="AstraCS:...")
-            >>> my_db2 = my_client.get_database("01234567-...", region="us-west1")
+            >>> my_db1 = my_client.get_database(
+            ...     "https://01234567-...us-west1.apps.astra.datastax.com",
+            ... )
+            >>> my_db2 = my_client.get_database("01234567-...", token="AstraCS:...")
+            >>> my_db3 = my_client.get_database("01234567-...", region="us-west1")
             >>> my_coll = my_db0.create_collection("movies", dimension=512)
             >>> my_coll.insert_one({"title": "The Title"}, vector=...)
 
         Note:
             This method does not perform any admin-level operation through
             the DevOps API. For actual creation of a database, see the
             `create_database` method of class AstraDBAdmin.
         """
 
         # lazy importing here to avoid circular dependency
         from astrapy import Database
 
-        # need to inspect for values?
-        this_db_info: Optional[Dict[str, Any]] = None
-        # handle overrides. Only region is needed (namespace can stay empty)
-        if region:
-            _region = region
-        else:
-            if this_db_info is None:
-                logger.info(f"fetching raw database info for {id}")
-                this_db_info = fetch_raw_database_info_from_id_token(
-                    id=id,
-                    token=self.token,
-                    environment=self.environment,
-                    max_time_ms=max_time_ms,
+        if self.environment in Environment.astra_db_values:
+            # handle the "endpoint passed as id" case first:
+            if re.match(api_endpoint_parser, id):
+                if region is not None:
+                    raise ValueError(
+                        "Parameter `region` not supported when supplying an API endpoint."
+                    )
+                # in this case max_time_ms is ignored (no calls take place)
+                return self.get_database_by_api_endpoint(
+                    api_endpoint=id,
+                    token=token,
+                    namespace=namespace,
+                    api_path=api_path,
+                    api_version=api_version,
                 )
-                logger.info(f"finished fetching raw database info for {id}")
-            _region = this_db_info["info"]["region"]
+            else:
+                # need to inspect for values?
+                this_db_info: Optional[Dict[str, Any]] = None
+                # handle overrides. Only region is needed (namespace can stay empty)
+                if region:
+                    _region = region
+                else:
+                    if this_db_info is None:
+                        logger.info(f"fetching raw database info for {id}")
+                        this_db_info = fetch_raw_database_info_from_id_token(
+                            id=id,
+                            token=self.token,
+                            environment=self.environment,
+                            max_time_ms=max_time_ms,
+                        )
+                        logger.info(f"finished fetching raw database info for {id}")
+                    _region = this_db_info["info"]["region"]
 
-        _token = token or self.token
-        _api_endpoint = build_api_endpoint(
-            environment=self.environment,
-            database_id=id,
-            region=_region,
-        )
-        return Database(
-            api_endpoint=_api_endpoint,
-            token=_token,
-            namespace=namespace,
-            caller_name=self._caller_name,
-            caller_version=self._caller_version,
-            api_path=api_path,
-            api_version=api_version,
-        )
+                _token = token or self.token
+                _api_endpoint = build_api_endpoint(
+                    environment=self.environment,
+                    database_id=id,
+                    region=_region,
+                )
+                return Database(
+                    api_endpoint=_api_endpoint,
+                    token=_token,
+                    namespace=namespace,
+                    caller_name=self._caller_name,
+                    caller_version=self._caller_version,
+                    environment=self.environment,
+                    api_path=api_path,
+                    api_version=api_version,
+                )
+        else:
+            # this is an alias for get_database_by_api_endpoint
+            # max_time_ms ignored
+            # we treat id as the endpoint (!)
+            if region is not None:
+                raise ValueError(
+                    "Parameter `region` not supported outside of Astra DB."
+                )
+            return self.get_database_by_api_endpoint(
+                api_endpoint=id,
+                token=token,
+                namespace=namespace,
+                api_path=api_path,
+                api_version=api_version,
+            )
 
     def get_async_database(
         self,
         id: str,
         *,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
@@ -347,35 +392,57 @@
             the DevOps API. For actual creation of a database, see the
             `create_database` method of class AstraDBAdmin.
         """
 
         # lazy importing here to avoid circular dependency
         from astrapy import Database
 
-        parsed_api_endpoint = parse_api_endpoint(api_endpoint)
-        if parsed_api_endpoint is not None:
-            if parsed_api_endpoint.environment != self.environment:
+        if self.environment in Environment.astra_db_values:
+            parsed_api_endpoint = parse_api_endpoint(api_endpoint)
+            if parsed_api_endpoint is not None:
+                if parsed_api_endpoint.environment != self.environment:
+                    raise ValueError(
+                        "Environment mismatch between client and provided "
+                        "API endpoint. You can try adding "
+                        f'`environment="{parsed_api_endpoint.environment}"` '
+                        "to the DataAPIClient creation statement."
+                    )
+                _token = token or self.token
+                return Database(
+                    api_endpoint=api_endpoint,
+                    token=_token,
+                    namespace=namespace,
+                    caller_name=self._caller_name,
+                    caller_version=self._caller_version,
+                    environment=self.environment,
+                    api_path=api_path,
+                    api_version=api_version,
+                )
+            else:
                 raise ValueError(
-                    "Environment mismatch between client and provided "
-                    "API endpoint. You can try adding "
-                    f'`environment="{parsed_api_endpoint.environment}"` '
-                    "to the DataAPIClient creation statement."
+                    f"Cannot parse the provided API endpoint ({api_endpoint})."
                 )
-            _token = token or self.token
-            return Database(
-                api_endpoint=api_endpoint,
-                token=_token,
-                namespace=namespace,
-                caller_name=self._caller_name,
-                caller_version=self._caller_version,
-                api_path=api_path,
-                api_version=api_version,
-            )
         else:
-            raise ValueError("Cannot parse the provided API endpoint.")
+            parsed_generic_api_endpoint = parse_generic_api_url(api_endpoint)
+            if parsed_generic_api_endpoint:
+                _token = token or self.token
+                return Database(
+                    api_endpoint=parsed_generic_api_endpoint,
+                    token=_token,
+                    namespace=namespace,
+                    caller_name=self._caller_name,
+                    caller_version=self._caller_version,
+                    environment=self.environment,
+                    api_path=api_path,
+                    api_version=api_version,
+                )
+            else:
+                raise ValueError(
+                    f"Cannot parse the provided API endpoint ({api_endpoint})."
+                )
 
     def get_async_database_by_api_endpoint(
         self,
         api_endpoint: str,
         *,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
@@ -437,14 +504,17 @@
             >>> my_db_admin.list_namespaces()
             ['default_keyspace', 'that_other_one']
         """
 
         # lazy importing here to avoid circular dependency
         from astrapy.admin import AstraDBAdmin
 
+        if self.environment not in Environment.astra_db_values:
+            raise ValueError("Method not supported outside of Astra DB.")
+
         return AstraDBAdmin(
             token=token or self.token,
             environment=self.environment,
             caller_name=self._caller_name,
             caller_version=self._caller_version,
             dev_ops_url=dev_ops_url,
             dev_ops_api_version=dev_ops_api_version,
```

### Comparing `astrapy-1.1.0/astrapy/collection.py` & `astrapy-1.2.0/astrapy/collection.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, TYPE_CHECKING
 
 from astrapy.core.db import (
     AstraDBCollection,
     AsyncAstraDBCollection,
 )
-from astrapy.core.defaults import MAX_INSERT_NUM_DOCUMENTS
+from astrapy.core.defaults import (
+    MAX_INSERT_NUM_DOCUMENTS,
+    DEFAULT_VECTORIZE_SECRET_HEADER,
+)
+from astrapy.api_options import CollectionAPIOptions
 from astrapy.exceptions import (
     BulkWriteException,
     CollectionNotFoundException,
     CumulativeOperationException,
     DataAPIFaultyResponseException,
     DataAPIResponseException,
     DeleteManyException,
@@ -214,14 +218,16 @@
     Args:
         database: a Database object, instantiated earlier. This represents
             the database the collection belongs to.
         name: the collection name. This parameter should match an existing
             collection on the database.
         namespace: this is the namespace to which the collection belongs.
             If not specified, the database's working namespace is used.
+        api_options: An instance of `astrapy.api_options.CollectionAPIOptions`
+            providing the general settings for interacting with the Data API.
         caller_name: name of the application, or framework, on behalf of which
             the Data API calls are performed. This ends up in the request user-agent.
         caller_version: version of the caller.
 
     Examples:
         >>> from astrapy import DataAPIClient, Collection
         >>> my_client = astrapy.DataAPIClient("AstraCS:...")
@@ -246,38 +252,56 @@
 
     def __init__(
         self,
         database: Database,
         name: str,
         *,
         namespace: Optional[str] = None,
+        api_options: Optional[CollectionAPIOptions] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> None:
+        if api_options is None:
+            self.api_options = CollectionAPIOptions()
+        else:
+            self.api_options = api_options
+        additional_headers = {
+            k: v
+            for k, v in {
+                DEFAULT_VECTORIZE_SECRET_HEADER: self.api_options.embedding_api_key,
+            }.items()
+            if v is not None
+        }
         self._astra_db_collection: AstraDBCollection = AstraDBCollection(
             collection_name=name,
             astra_db=database._astra_db,
             namespace=namespace,
             caller_name=caller_name,
             caller_version=caller_version,
+            additional_headers=additional_headers,
         )
         # this comes after the above, lets AstraDBCollection resolve namespace
         self._database = database._copy(
             namespace=self._astra_db_collection.astra_db.namespace
         )
 
     def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(name="{self.name}", '
             f'namespace="{self.namespace}", database={self.database})'
         )
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Collection):
-            return self._astra_db_collection == other._astra_db_collection
+            return all(
+                [
+                    self._astra_db_collection == other._astra_db_collection,
+                    self.api_options == other.api_options,
+                ]
+            )
         else:
             return False
 
     def __call__(self, *pargs: Any, **kwargs: Any) -> None:
         raise TypeError(
             f"'{self.__class__.__name__}' object is not callable. If you "
             f"meant to call the '{self.name}' method on a "
@@ -287,65 +311,89 @@
 
     def _copy(
         self,
         *,
         database: Optional[Database] = None,
         name: Optional[str] = None,
         namespace: Optional[str] = None,
+        api_options: Optional[CollectionAPIOptions] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> Collection:
         return Collection(
             database=database or self.database._copy(),
             name=name or self.name,
             namespace=namespace or self.namespace,
+            api_options=self.api_options.with_override(api_options),
             caller_name=caller_name or self._astra_db_collection.caller_name,
             caller_version=caller_version or self._astra_db_collection.caller_version,
         )
 
     def with_options(
         self,
         *,
         name: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> Collection:
         """
         Create a clone of this collection with some changed attributes.
 
         Args:
             name: the name of the collection. This parameter is useful to
                 quickly spawn Collection instances each pointing to a different
                 collection existing in the same namespace.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
 
         Returns:
             a new Collection instance.
 
         Example:
             >>> my_other_coll = my_coll.with_options(
             ...     name="the_other_coll",
             ...     caller_name="caller_identity",
             ... )
         """
 
+        _api_options = CollectionAPIOptions(
+            embedding_api_key=embedding_api_key,
+            max_time_ms=collection_max_time_ms,
+        )
+
         return self._copy(
             name=name,
+            api_options=_api_options,
             caller_name=caller_name,
             caller_version=caller_version,
         )
 
     def to_async(
         self,
         *,
         database: Optional[AsyncDatabase] = None,
         name: Optional[str] = None,
         namespace: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> AsyncCollection:
         """
         Create an AsyncCollection from this one. Save for the arguments
         explicitly provided as overrides, everything else is kept identical
         to this collection in the copy (the database is converted into
@@ -354,30 +402,48 @@
         Args:
             database: an AsyncDatabase object, instantiated earlier.
                 This represents the database the new collection belongs to.
             name: the collection name. This parameter should match an existing
                 collection on the database.
             namespace: this is the namespace to which the collection belongs.
                 If not specified, the database's working namespace is used.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
 
         Returns:
             the new copy, an AsyncCollection instance.
 
         Example:
             >>> asyncio.run(my_coll.to_async().count_documents({},upper_bound=100))
             77
         """
 
+        _api_options = CollectionAPIOptions(
+            embedding_api_key=embedding_api_key,
+            max_time_ms=collection_max_time_ms,
+        )
+
         return AsyncCollection(
             database=database or self.database.to_async(),
             name=name or self.name,
             namespace=namespace or self.namespace,
+            api_options=self.api_options.with_override(_api_options),
             caller_name=caller_name or self._astra_db_collection.caller_name,
             caller_version=caller_version or self._astra_db_collection.caller_version,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
@@ -408,28 +474,30 @@
 
         The method issues a request to the Data API each time is invoked,
         without caching mechanisms: this ensures up-to-date information
         for usages such as real-time collection validation by the application.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a CollectionOptions instance describing the collection.
             (See also the database `list_collections` method.)
 
         Example:
             >>> my_coll.options()
             CollectionOptions(vector=CollectionVectorOptions(dimension=3, metric='cosine'))
         """
 
         logger.info(f"getting collections in search of '{self.name}'")
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         self_descriptors = [
             coll_desc
-            for coll_desc in self.database.list_collections(max_time_ms=max_time_ms)
+            for coll_desc in self.database.list_collections(max_time_ms=_max_time_ms)
             if coll_desc.name == self.name
         ]
         logger.info(f"finished getting collections in search of '{self.name}'")
         if self_descriptors:
             return self_descriptors[0].options  # type: ignore[no-any-return]
         else:
             raise CollectionNotFoundException(
@@ -531,23 +599,23 @@
 
         Args:
             document: the dictionary expressing the document to insert.
                 The `_id` field of the document can be left out, in which
                 case it will be created automatically.
             vector: a vector (a list of numbers appropriate for the collection)
                 for the document. Passing this parameter is equivalent to
-                providing the vector in the "$vector" field of the document itself,
+                providing a `$vector` field within the document itself,
                 however the two are mutually exclusive.
             vectorize: a string to be made into a vector, if such a service
                 is configured for the collection. Passing this parameter is
                 equivalent to providing a `$vectorize` field in the document itself,
                 however the two are mutually exclusive.
                 Moreover, this parameter cannot coexist with `vector`.
-                NOTE: This feature is under current development.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an InsertOneResult object.
 
         Examples:
             >>> my_coll.count_documents({}, upper_bound=10)
             0
@@ -571,18 +639,19 @@
         Note:
             If an `_id` is explicitly provided, which corresponds to a document
             that exists already in the collection, an error is raised and
             the insertion fails.
         """
 
         _document = _collate_vector_to_document(document, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"inserting one document in '{self.name}'")
         io_response = self._astra_db_collection.insert_one(
             _document,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished inserting one document in '{self.name}'")
         if "insertedIds" in io_response.get("status", {}):
             if io_response["status"]["insertedIds"]:
                 inserted_id = io_response["status"]["insertedIds"][0]
                 return InsertOneResult(
                     raw_results=[io_response],
@@ -602,15 +671,15 @@
     @recast_method_sync
     def insert_many(
         self,
         documents: Iterable[DocumentType],
         *,
         vectors: Optional[Iterable[Optional[VectorType]]] = None,
         vectorize: Optional[Iterable[Optional[str]]] = None,
-        ordered: bool = True,
+        ordered: bool = False,
         chunk_size: Optional[int] = None,
         concurrency: Optional[int] = None,
         max_time_ms: Optional[int] = None,
     ) -> InsertManyResult:
         """
         Insert a list of documents into the collection.
         This is not an atomic operation.
@@ -628,45 +697,52 @@
                 Passing vectors this way is indeed equivalent to the "$vector" field
                 of the documents, however the two are mutually exclusive.
             vectorize: an optional list of strings to be made into as many vectors
                 (one per document), if such a service is configured for the collection.
                 Passing this parameter is equivalent to providing a `$vectorize`
                 field in the documents themselves, however the two are mutually exclusive.
                 For any given document, this parameter cannot coexist with the
-                corresponding `vector` entry.
-                NOTE: This feature is under current development.
-            ordered: if True (default), the insertions are processed sequentially.
-                If False, they can occur in arbitrary order and possibly concurrently.
+                corresponding entry in `vectors`.
+            ordered: if False (default), the insertions can occur in arbitrary order
+                and possibly concurrently. If True, they are processed sequentially.
+                If there are no specific reasons against it, unordered insertions are to
+                be preferred as they complete much faster.
             chunk_size: how many documents to include in a single API request.
                 Exceeding the server maximum allowed value results in an error.
                 Leave it unspecified (recommended) to use the system default.
             concurrency: maximum number of concurrent requests to the API at
                 a given time. It cannot be more than one for ordered insertions.
             max_time_ms: a timeout, in milliseconds, for the operation.
+                If not passed, the collection-level setting is used instead:
+                If many documents are being inserted, this method corresponds
+                to several HTTP requests: in such cases one may want to specify
+                a more tolerant timeout here.
 
         Returns:
             an InsertManyResult object.
 
         Examples:
             >>> my_coll.count_documents({}, upper_bound=10)
             0
-            >>> my_coll.insert_many([{"a": 10}, {"a": 5}, {"b": [True, False, False]}])
+            >>> my_coll.insert_many(
+            ...     [{"a": 10}, {"a": 5}, {"b": [True, False, False]}],
+            ...     ordered=True,
+            ... )
             InsertManyResult(raw_results=..., inserted_ids=['184bb06f-...', '...', '...'])
             >>> my_coll.count_documents({}, upper_bound=100)
             3
             >>> my_coll.insert_many(
             ...     [{"seq": i} for i in range(50)],
-            ...     ordered=False,
             ...     concurrency=5,
             ... )
             InsertManyResult(raw_results=..., inserted_ids=[... ...])
             >>> my_coll.count_documents({}, upper_bound=100)
             53
 
-            # The following are three equivalent statements:
+            >>> # The following are three equivalent statements:
             >>> my_coll.insert_many(
             ...     [{"tag": "a"}, {"tag": "b"}],
             ...     vectors=[[1, 2], [3, 4]],
             ... )
             InsertManyResult(...)
             >>> my_coll.insert_many(
             ...     [{"tag": "a", "$vector": [1, 2]}, {"tag": "b"}],
@@ -718,17 +794,18 @@
         if _concurrency > 1 and ordered:
             raise ValueError("Cannot run ordered insert_many concurrently.")
         if chunk_size is None:
             _chunk_size = MAX_INSERT_NUM_DOCUMENTS
         else:
             _chunk_size = chunk_size
         _documents = _collate_vectors_to_documents(documents, vectors, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"inserting {len(_documents)} documents in '{self.name}'")
         raw_results: List[Dict[str, Any]] = []
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         if ordered:
             options = {"ordered": True}
             inserted_ids: List[Any] = []
             for i in range(0, len(_documents), _chunk_size):
                 logger.info(f"inserting a chunk of documents in '{self.name}'")
                 chunk_response = self._astra_db_collection.insert_many(
                     documents=_documents[i : i + _chunk_size],
@@ -867,23 +944,32 @@
         option in a non-vector-search manner.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the documents being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             skip: with this integer parameter, what would be the first `skip`
                 documents returned by the query are discarded, and the results
                 start from the (skip+1)-th document.
                 This parameter can be used only in conjunction with an explicit
                 `sort` criterion of the ascending/descending type (i.e. it cannot
                 be used when not sorting, nor with vector-based ANN search).
             limit: this (integer) parameter sets a limit over how many documents
@@ -896,26 +982,26 @@
                 criteria can be specified. Moreover, there is an upper bound
                 to the number of documents that can be returned. For details,
                 see the Note about upper bounds and the Data API documentation.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             include_similarity: a boolean to request the numeric value of the
                 similarity to be returned as an added "$similarity" key in each
                 returned document. Can only be used for vector ANN search, i.e.
                 when either `vector` is supplied or the `sort` parameter has the
                 shape {"$vector": ...}.
             sort: with this dictionary parameter one can control the order
                 the documents are returned. See the Note about sorting, as well as
                 the one about upper bounds, for details.
             max_time_ms: a timeout, in milliseconds, for each single one
                 of the underlying HTTP requests used to fetch documents as the
                 cursor is iterated over.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a Cursor object representing iterations over the matching documents
             (see the Cursor object for how to use it. The simplest thing is to
             run a for loop: `for document in collection.sort(...):`).
 
         Examples:
@@ -952,15 +1038,15 @@
             ...         {},
             ...         limit=3,
             ...         vector=[3, 3],
             ...     )
             ... ]
             >>> ann_tags
             ['A', 'B', 'C']
-            # (assuming the collection has metric VectorMetric.COSINE)
+            >>> # (assuming the collection has metric VectorMetric.COSINE)
 
         Note:
             The following are example values for the `sort` parameter.
             When no particular order is required:
                 sort={}  # (default when parameter not provided)
             When sorting by a certain value in ascending/descending order:
                 sort={"field": SortDocuments.ASCENDING}
@@ -996,24 +1082,25 @@
             It should be noted that the behavior of the cursor in the case documents
             have been added/removed after the `find` was started depends on database
             internals and it is not guaranteed, nor excluded, that such "real-time"
             changes in the data would be picked up by the cursor.
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         if include_similarity is not None and not _is_vector_sort(_sort):
             raise ValueError(
                 "Cannot use `include_similarity` when not searching through `vector`."
             )
         return (
             Cursor(
                 collection=self,
                 filter=filter,
                 projection=projection,
-                max_time_ms=max_time_ms,
+                max_time_ms=_max_time_ms,
                 overall_max_time_ms=None,
             )
             .skip(skip)
             .limit(limit)
             .sort(_sort)
             .include_similarity(include_similarity)
         )
@@ -1034,42 +1121,51 @@
         provided filters, if any is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the documents being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to perform vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), extracting the most
                 similar document in the collection matching the filter.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             include_similarity: a boolean to request the numeric value of the
                 similarity to be returned as an added "$similarity" key in the
                 returned document. Can only be used for vector ANN search, i.e.
                 when either `vector` is supplied or the `sort` parameter has the
                 shape {"$vector": ...}.
             sort: with this dictionary parameter one can control the order
                 the documents are returned. See the Note about sorting for details.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary expressing the required document, otherwise None.
 
         Examples:
             >>> my_coll.find_one({})
             {'_id': '68d1e515-...', 'seq': 37}
@@ -1080,32 +1176,33 @@
             >>> my_coll.find_one({}, projection={"seq": False})
             {'_id': '68d1e515-...'}
             >>> my_coll.find_one(
             ...     {},
             ...     sort={"seq": astrapy.constants.SortDocuments.DESCENDING},
             ... )
             {'_id': '97e85f81-...', 'seq': 69}
-            >>> my_coll.find_one({}, vector=[1, 0])
+            >>> my_coll.find_one({}, vector=[1, 0], projection={"*": True})
             {'_id': '...', 'tag': 'D', '$vector': [4.0, 1.0]}
 
         Note:
             See the `find` method for more details on the accepted parameters
             (whereas `skip` and `limit` are not valid parameters for `find_one`).
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         fo_cursor = self.find(
             filter=filter,
             projection=projection,
             skip=None,
             limit=1,
             vector=vector,
             vectorize=vectorize,
             include_similarity=include_similarity,
             sort=sort,
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         try:
             document = fo_cursor.__next__()
             return document  # type: ignore[no-any-return]
         except StopIteration:
             return None
 
@@ -1130,18 +1227,19 @@
                     "field.3.subfield"
                 If lists are encountered and no numeric index is specified,
                 all items in the list are visited.
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            max_time_ms: a timeout, in milliseconds, for the operation.
+            max_time_ms: a timeout, in milliseconds, with the same meaning as for `find`.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a list of all different values for `key` found across the documents
             that match the filter. The result list has no repeated items.
 
         Example:
             >>> my_coll.insert_many(
@@ -1173,20 +1271,21 @@
 
         Note:
             For details on the behaviour of "distinct" in conjunction with
             real-time changes in the collection contents, see the
             Note of the `find` command.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         f_cursor = Cursor(
             collection=self,
             filter=filter,
             projection={key: True},
             max_time_ms=None,
-            overall_max_time_ms=max_time_ms,
+            overall_max_time_ms=_max_time_ms,
         )
         return f_cursor.distinct(key)  # type: ignore[no-any-return]
 
     @recast_method_sync
     def count_documents(
         self,
         filter: Dict[str, Any],
@@ -1198,24 +1297,25 @@
         Count the documents in the collection matching the specified filter.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             upper_bound: a required ceiling on the result of the count operation.
                 If the actual number of documents exceeds this value,
                 an exception will be raised.
                 Furthermore, if the actual number of documents exceeds the maximum
                 count that the Data API can reach (regardless of upper_bound),
                 an exception will be raised.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             the exact count of matching documents.
 
         Example:
             >>> my_coll.insert_many([{"seq": i} for i in range(20)])
             InsertManyResult(...)
@@ -1235,18 +1335,19 @@
             for sizeable amounts of documents (i.e. in the thousands and more)
             is discouraged in favor of alternative application-specific solutions.
             Keep in mind that the Data API has a hard upper limit on the amount
             of documents it will count, and that an exception will be thrown
             by this method if this limit is encountered.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info("calling count_documents")
         cd_response = self._astra_db_collection.count_documents(
             filter=filter,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info("finished calling count_documents")
         if "count" in cd_response.get("status", {}):
             count: int = cd_response["status"]["count"]
             if cd_response["status"].get("moreData", False):
                 raise TooManyDocumentsToCountException(
                     text=f"Document count exceeds {count}, the maximum allowed by the server",
@@ -1274,25 +1375,27 @@
         """
         Query the API server for an estimate of the document count in the collection.
 
         Contrary to `count_documents`, this method has no filtering parameters.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a server-provided estimate count of the documents in the collection.
 
         Example:
             >>> my_coll.estimated_document_count()
             35700
         """
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         ed_response = self.command(
             {"estimatedDocumentCount": {}},
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         if "count" in ed_response.get("status", {}):
             count: int = ed_response["status"]["count"]
             return count
         else:
             raise DataAPIFaultyResponseException(
                 text="Faulty response from estimated_document_count API command.",
@@ -1318,50 +1421,59 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             replacement: the new document to write into the collection.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 replaced one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, `replacement` is inserted as a new document
                 if no matches are found on the collection. If False,
                 the operation silently does nothing in case of no matches.
             return_document: a flag controlling what document is returned:
                 if set to `ReturnDocument.BEFORE`, or the string "before",
                 the document found on database is returned; if set to
                 `ReturnDocument.AFTER`, or the string "after", the new
                 document is returned. The default is "before".
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             A document (or a projection thereof, as required), either the one
             before the replace operation or the one after that.
             Alternatively, the method returns None to represent
             that no matching document was found, or that no replacement
             was inserted (depending on the `return_document` parameter).
@@ -1397,22 +1509,23 @@
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "returnDocument": return_document,
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_replace on '{self.name}'")
         fo_response = self._astra_db_collection.find_one_and_replace(
             replacement=replacement,
             filter=filter,
             projection=normalize_optional_projection(projection),
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_replace on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             ret_document = fo_response.get("data", {}).get("document")
             if ret_document is None:
                 return None
             else:
@@ -1440,39 +1553,39 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             replacement: the new document to write into the collection.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 replaced one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, `replacement` is inserted as a new document
                 if no matches are found on the collection. If False,
                 the operation silently does nothing in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an UpdateResult object summarizing the outcome of the replace operation.
 
         Example:
             >>> my_coll.insert_one({"Marco": "Polo"})
             InsertOneResult(...)
@@ -1487,20 +1600,21 @@
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "upsert": upsert,
         }
         logger.info(f"calling find_one_and_replace on '{self.name}'")
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         fo_response = self._astra_db_collection.find_one_and_replace(
             replacement=replacement,
             filter=filter,
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_replace on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             fo_status = fo_response.get("status") or {}
             _update_info = _prepare_update_info([fo_status])
             return UpdateResult(
                 raw_results=[fo_response],
@@ -1531,41 +1645,49 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the document, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 updated one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a new document (resulting from applying the `update`
                 to an empty document) is inserted if no matches are found on
@@ -1573,14 +1695,15 @@
                 in case of no matches.
             return_document: a flag controlling what document is returned:
                 if set to `ReturnDocument.BEFORE`, or the string "before",
                 the document found on database is returned; if set to
                 `ReturnDocument.AFTER`, or the string "after", the new
                 document is returned. The default is "before".
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             A document (or a projection thereof, as required), either the one
             before the replace operation or the one after that.
             Alternatively, the method returns None to represent
             that no matching document was found, or that no update
             was applied (depending on the `return_document` parameter).
@@ -1616,22 +1739,23 @@
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "returnDocument": return_document,
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_update on '{self.name}'")
         fo_response = self._astra_db_collection.find_one_and_update(
             update=update,
             filter=filter,
             projection=normalize_optional_projection(projection),
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_update on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             ret_document = fo_response.get("data", {}).get("document")
             if ret_document is None:
                 return None
             else:
@@ -1659,16 +1783,16 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the document, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
@@ -1679,25 +1803,25 @@
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 updated one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a new document (resulting from applying the `update`
                 to an empty document) is inserted if no matches are found on
                 the collection. If False, the operation silently does nothing
                 in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an UpdateResult object summarizing the outcome of the update operation.
 
         Example:
             >>> my_coll.insert_one({"Marco": "Polo"})
             InsertOneResult(...)
@@ -1709,21 +1833,22 @@
             UpdateResult(raw_results=..., update_info={'n': 1, 'updatedExisting': False, 'ok': 1.0, 'nModified': 0, 'upserted': '2a45ff60-...'})
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_update on '{self.name}'")
         fo_response = self._astra_db_collection.find_one_and_update(
             update=update,
             sort=_sort,
             filter=filter,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_update on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             fo_status = fo_response.get("status") or {}
             _update_info = _prepare_update_info([fo_status])
             return UpdateResult(
                 raw_results=[fo_response],
@@ -1749,29 +1874,33 @@
         optionally inserting one documents in absence of matches.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the documents, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a single new document (resulting from applying `update`
                 to an empty document) is inserted if no matches are found on
                 the collection. If False, the operation silently does nothing
                 in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the operation.
+                If not passed, the collection-level setting is used instead:
+                if a large number of document updates is anticipated, it is suggested
+                to specify a larger timeout than in most other operations as the
+                update will span several HTTP calls to the API in sequence.
 
         Returns:
             an UpdateResult object summarizing the outcome of the update operation.
 
         Example:
             >>> my_coll.insert_many([{"c": "red"}, {"c": "green"}, {"c": "blue"}])
             InsertManyResult(...)
@@ -1791,25 +1920,26 @@
             running this command while, at the same time, another process is
             inserting new documents which match the filter of the `update_many`
             can result in an unpredictable fraction of these documents being updated.
             In other words, it cannot be easily predicted whether a given
             newly-inserted document will be picked up by the update_many command or not.
         """
 
-        base_options = {
+        api_options = {
             "upsert": upsert,
         }
         page_state_options: Dict[str, str] = {}
         um_responses: List[Dict[str, Any]] = []
         um_statuses: List[Dict[str, Any]] = []
         must_proceed = True
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"starting update_many on '{self.name}'")
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         while must_proceed:
-            options = {**base_options, **page_state_options}
+            options = {**api_options, **page_state_options}
             logger.info(f"calling update_many on '{self.name}'")
             this_um_response = self._astra_db_collection.update_many(
                 update=update,
                 filter=filter,
                 options=options,
                 timeout_info=timeout_manager.remaining_timeout_info(),
             )
@@ -1868,42 +1998,49 @@
         however, is the return value of the method.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                Note that the `_id` field will be returned with the document
-                in any case, regardless of what the provided `projection` requires.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 deleted one. See the `find` method for more on sorting.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             Either the document (or a projection thereof, as requested), or None
             if no matches were found in the first place.
 
         Example:
             >>> my_coll.insert_many(
@@ -1921,19 +2058,20 @@
             >>> my_coll.find_one_and_delete({"species": {"$ne": "frog"}})
             >>> # (returns None for no matches)
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         _projection = normalize_optional_projection(projection)
         logger.info(f"calling find_one_and_delete on '{self.name}'")
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         fo_response = self._astra_db_collection.find_one_and_delete(
             sort=_sort,
             filter=filter,
             projection=_projection,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_delete on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             document = fo_response["data"]["document"]
             return document  # type: ignore[no-any-return]
         else:
             deleted_count = fo_response.get("status", {}).get("deletedCount")
@@ -1961,34 +2099,34 @@
         of the number of matches to the provided filters.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 deleted one. See the `find` method for more on sorting.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a DeleteResult object summarizing the outcome of the delete operation.
 
         Example:
             >>> my_coll.insert_many([{"seq": 1}, {"seq": 0}, {"seq": 2}])
             InsertManyResult(...)
@@ -2004,17 +2142,18 @@
             >>> my_coll.distinct("seq")
             [0]
             >>> my_coll.delete_one({"seq": 2})
             DeleteResult(raw_results=..., deleted_count=0)
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling delete_one_by_predicate on '{self.name}'")
         do_response = self._astra_db_collection.delete_one_by_predicate(
-            filter=filter, timeout_info=base_timeout_info(max_time_ms), sort=_sort
+            filter=filter, timeout_info=base_timeout_info(_max_time_ms), sort=_sort
         )
         logger.info(f"finished calling delete_one_by_predicate on '{self.name}'")
         if "deletedCount" in do_response.get("status", {}):
             deleted_count = do_response["status"]["deletedCount"]
             if deleted_count == -1:
                 return DeleteResult(
                     deleted_count=None,
@@ -2043,20 +2182,25 @@
         Delete all documents matching a provided filter.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
                 The `delete_many` method does not accept an empty filter: see
                 `delete_all` to completely erase all contents of a collection
             max_time_ms: a timeout, in milliseconds, for the operation.
+                If not passed, the collection-level setting is used instead:
+                keep in mind that this method entails successive HTTP requests
+                to the API, depending on how many documents are to be deleted.
+                For this reason, in most cases it is suggested to relax the
+                timeout compared to other method calls.
 
         Returns:
             a DeleteResult object summarizing the outcome of the delete operation.
 
         Example:
             >>> my_coll.insert_many([{"seq": 1}, {"seq": 0}, {"seq": 2}])
             InsertManyResult(...)
@@ -2082,15 +2226,16 @@
                 "empty. In order to completely clear the contents of a "
                 "collection, please use the `delete_all` method."
             )
 
         dm_responses: List[Dict[str, Any]] = []
         deleted_count = 0
         must_proceed = True
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         logger.info(f"starting delete_many on '{self.name}'")
         while must_proceed:
             logger.info(f"calling delete_many on '{self.name}'")
             this_dm_response = self._astra_db_collection.delete_many(
                 filter=filter,
                 skip_error_check=True,
                 timeout_info=timeout_manager.remaining_timeout_info(),
@@ -2128,14 +2273,15 @@
     @recast_method_sync
     def delete_all(self, *, max_time_ms: Optional[int] = None) -> Dict[str, Any]:
         """
         Delete all documents in a collection.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary of the form {"ok": 1} to signal successful deletion.
 
         Example:
             >>> my_coll.distinct("seq")
             [2, 1, 0]
@@ -2146,17 +2292,18 @@
             >>> my_coll.count_documents({}, upper_bound=100)
             0
 
         Note:
             Use with caution.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling unfiltered delete_many on '{self.name}'")
         dm_response = self._astra_db_collection.delete_many(
-            filter={}, timeout_info=base_timeout_info(max_time_ms)
+            filter={}, timeout_info=base_timeout_info(_max_time_ms)
         )
         logger.info(f"finished calling unfiltered delete_many on '{self.name}'")
         deleted_count = dm_response["status"]["deletedCount"]
         if deleted_count == -1:
             return {"ok": 1}
         else:
             raise DataAPIFaultyResponseException(
@@ -2164,15 +2311,15 @@
                 raw_response=dm_response,
             )
 
     def bulk_write(
         self,
         requests: Iterable[BaseOperation],
         *,
-        ordered: bool = True,
+        ordered: bool = False,
         concurrency: Optional[int] = None,
         max_time_ms: Optional[int] = None,
     ) -> BulkWriteResult:
         """
         Execute an arbitrary amount of operations such as inserts, updates, deletes
         either sequentially or concurrently.
 
@@ -2184,22 +2331,25 @@
             requests: an iterable over concrete subclasses of `BaseOperation`,
                 such as `InsertMany` or `ReplaceOne`. Each such object
                 represents an operation ready to be executed on a collection,
                 and is instantiated by passing the same parameters as one
                 would the corresponding collection method.
             ordered: whether to launch the `requests` one after the other or
                 in arbitrary order, possibly in a concurrent fashion. For
-                performance reasons, `ordered=False` should be preferred
+                performance reasons, False (default) should be preferred
                 when compatible with the needs of the application flow.
             concurrency: maximum number of concurrent operations executing at
                 a given time. It cannot be more than one for ordered bulk writes.
             max_time_ms: a timeout, in milliseconds, for the whole bulk write.
                 Remember that, if the method call times out, then there's no
                 guarantee about what portion of the bulk write has been received
                 and successfully executed by the Data API.
+                If not passed, the collection-level setting is used instead:
+                in most cases, however, one should pass a relaxed timeout
+                if longer sequences of operations are to be executed in bulk.
 
         Returns:
             A single BulkWriteResult summarizing the whole list of requested
             operations. The keys in the map attributes of BulkWriteResult
             (when present) are the integer indices of the corresponding operation
             in the `requests` iterable.
 
@@ -2223,16 +2373,17 @@
                 _concurrency = 1
             else:
                 _concurrency = DEFAULT_BULK_WRITE_CONCURRENCY
         else:
             _concurrency = concurrency
         if _concurrency > 1 and ordered:
             raise ValueError("Cannot run ordered bulk_write concurrently.")
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"startng a bulk write on '{self.name}'")
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         if ordered:
             bulk_write_results: List[BulkWriteResult] = []
             for operation_i, operation in enumerate(requests):
                 try:
                     this_bw_result = operation.execute(
                         self,
                         index_in_bulk_write=operation_i,
@@ -2340,14 +2491,15 @@
     def drop(self, *, max_time_ms: Optional[int] = None) -> Dict[str, Any]:
         """
         Drop the collection, i.e. delete it from the database along with
         all the documents it contains.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
                 Remember there is not guarantee that a request that has
                 timed out us not in fact honored.
 
         Returns:
             a dictionary of the form {"ok": 1} to signal successful deletion.
 
         Example:
@@ -2359,32 +2511,25 @@
             Traceback (most recent call last):
                 ... ...
             astrapy.exceptions.DataAPIResponseException: Collection does not exist, collection name: my_collection
 
         Note:
             Use with caution.
 
-
-        Note:
-            Once the method succeeds, methods on this object can still be invoked:
-            however, this hardly makes sense as the underlying actual collection
-            is no more.
-            It is responsibility of the developer to design a correct flow
-            which avoids using a deceased collection any further.
-
         Note:
             Once the method succeeds, methods on this object can still be invoked:
             however, this hardly makes sense as the underlying actual collection
             is no more.
             It is responsibility of the developer to design a correct flow
             which avoids using a deceased collection any further.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"dropping collection '{self.name}' (self)")
-        drop_result = self.database.drop_collection(self, max_time_ms=max_time_ms)
+        drop_result = self.database.drop_collection(self, max_time_ms=_max_time_ms)
         logger.info(f"finished dropping collection '{self.name}' (self)")
         return drop_result  # type: ignore[no-any-return]
 
     def command(
         self,
         body: Dict[str, Any],
         *,
@@ -2393,29 +2538,31 @@
         """
         Send a POST request to the Data API for this collection with
         an arbitrary, caller-provided payload.
 
         Args:
             body: a JSON-serializable dictionary, the payload of the request.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary with the response of the HTTP request.
 
         Example:
             >>> my_coll.command({"countDocuments": {}})
             {'status': {'count': 123}}
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling command on '{self.name}'")
         command_result = self.database.command(
             body=body,
             namespace=self.namespace,
             collection_name=self.name,
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         logger.info(f"finished calling command on '{self.name}'")
         return command_result  # type: ignore[no-any-return]
 
 
 class AsyncCollection:
     """
@@ -2429,14 +2576,16 @@
     Args:
         database: a Database object, instantiated earlier. This represents
             the database the collection belongs to.
         name: the collection name. This parameter should match an existing
             collection on the database.
         namespace: this is the namespace to which the collection belongs.
             If not specified, the database's working namespace is used.
+        api_options: An instance of `astrapy.api_options.CollectionAPIOptions`
+            providing the general settings for interacting with the Data API.
         caller_name: name of the application, or framework, on behalf of which
             the Data API calls are performed. This ends up in the request user-agent.
         caller_version: version of the caller.
 
     Examples:
         >>> from astrapy import DataAPIClient, AsyncCollection
         >>> my_client = astrapy.DataAPIClient("AstraCS:...")
@@ -2463,38 +2612,56 @@
 
     def __init__(
         self,
         database: AsyncDatabase,
         name: str,
         *,
         namespace: Optional[str] = None,
+        api_options: Optional[CollectionAPIOptions] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> None:
+        if api_options is None:
+            self.api_options = CollectionAPIOptions()
+        else:
+            self.api_options = api_options
+        additional_headers = {
+            k: v
+            for k, v in {
+                DEFAULT_VECTORIZE_SECRET_HEADER: self.api_options.embedding_api_key,
+            }.items()
+            if v is not None
+        }
         self._astra_db_collection: AsyncAstraDBCollection = AsyncAstraDBCollection(
             collection_name=name,
             astra_db=database._astra_db,
             namespace=namespace,
             caller_name=caller_name,
             caller_version=caller_version,
+            additional_headers=additional_headers,
         )
         # this comes after the above, lets AstraDBCollection resolve namespace
         self._database = database._copy(
             namespace=self._astra_db_collection.astra_db.namespace
         )
 
     def __repr__(self) -> str:
         return (
             f'{self.__class__.__name__}(name="{self.name}", '
             f'namespace="{self.namespace}", database={self.database})'
         )
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, AsyncCollection):
-            return self._astra_db_collection == other._astra_db_collection
+            return all(
+                [
+                    self._astra_db_collection == other._astra_db_collection,
+                    self.api_options == other.api_options,
+                ]
+            )
         else:
             return False
 
     def __call__(self, *pargs: Any, **kwargs: Any) -> None:
         raise TypeError(
             f"'{self.__class__.__name__}' object is not callable. If you "
             f"meant to call the '{self.name}' method on a "
@@ -2504,65 +2671,89 @@
 
     def _copy(
         self,
         *,
         database: Optional[AsyncDatabase] = None,
         name: Optional[str] = None,
         namespace: Optional[str] = None,
+        api_options: Optional[CollectionAPIOptions] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> AsyncCollection:
         return AsyncCollection(
             database=database or self.database._copy(),
             name=name or self.name,
             namespace=namespace or self.namespace,
+            api_options=self.api_options.with_override(api_options),
             caller_name=caller_name or self._astra_db_collection.caller_name,
             caller_version=caller_version or self._astra_db_collection.caller_version,
         )
 
     def with_options(
         self,
         *,
         name: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> AsyncCollection:
         """
         Create a clone of this collection with some changed attributes.
 
         Args:
             name: the name of the collection. This parameter is useful to
                 quickly spawn AsyncCollection instances each pointing to a different
                 collection existing in the same namespace.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
 
         Returns:
             a new AsyncCollection instance.
 
         Example:
             >>> my_other_async_coll = my_async_coll.with_options(
             ...     name="the_other_coll",
             ...     caller_name="caller_identity",
             ... )
         """
 
+        _api_options = CollectionAPIOptions(
+            embedding_api_key=embedding_api_key,
+            max_time_ms=collection_max_time_ms,
+        )
+
         return self._copy(
             name=name,
+            api_options=_api_options,
             caller_name=caller_name,
             caller_version=caller_version,
         )
 
     def to_sync(
         self,
         *,
         database: Optional[Database] = None,
         name: Optional[str] = None,
         namespace: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> Collection:
         """
         Create a Collection from this one. Save for the arguments
         explicitly provided as overrides, everything else is kept identical
         to this collection in the copy (the database is converted into
@@ -2571,30 +2762,48 @@
         Args:
             database: a Database object, instantiated earlier.
                 This represents the database the new collection belongs to.
             name: the collection name. This parameter should match an existing
                 collection on the database.
             namespace: this is the namespace to which the collection belongs.
                 If not specified, the database's working namespace is used.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
 
         Returns:
             the new copy, a Collection instance.
 
         Example:
             >>> my_async_coll.to_sync().count_documents({}, upper_bound=100)
             77
         """
 
+        _api_options = CollectionAPIOptions(
+            embedding_api_key=embedding_api_key,
+            max_time_ms=collection_max_time_ms,
+        )
+
         return Collection(
             database=database or self.database.to_sync(),
             name=name or self.name,
             namespace=namespace or self.namespace,
+            api_options=self.api_options.with_override(_api_options),
             caller_name=caller_name or self._astra_db_collection.caller_name,
             caller_version=caller_version or self._astra_db_collection.caller_version,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
@@ -2625,29 +2834,31 @@
 
         The method issues a request to the Data API each time is invoked,
         without caching mechanisms: this ensures up-to-date information
         for usages such as real-time collection validation by the application.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a CollectionOptions instance describing the collection.
             (See also the database `list_collections` method.)
 
         Example:
             >>> asyncio.run(my_async_coll.options())
             CollectionOptions(vector=CollectionVectorOptions(dimension=3, metric='cosine'))
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"getting collections in search of '{self.name}'")
         self_descriptors = [
             coll_desc
             async for coll_desc in self.database.list_collections(
-                max_time_ms=max_time_ms
+                max_time_ms=_max_time_ms
             )
             if coll_desc.name == self.name
         ]
         logger.info(f"finished getting collections in search of '{self.name}'")
         if self_descriptors:
             return self_descriptors[0].options  # type: ignore[no-any-return]
         else:
@@ -2750,23 +2961,23 @@
 
         Args:
             document: the dictionary expressing the document to insert.
                 The `_id` field of the document can be left out, in which
                 case it will be created automatically.
             vector: a vector (a list of numbers appropriate for the collection)
                 for the document. Passing this parameter is equivalent to
-                providing the vector in the "$vector" field of the document itself,
+                providing a `$vector` field within the document itself,
                 however the two are mutually exclusive.
             vectorize: a string to be made into a vector, if such a service
                 is configured for the collection. Passing this parameter is
                 equivalent to providing a `$vectorize` field in the document itself,
                 however the two are mutually exclusive.
                 Moreover, this parameter cannot coexist with `vector`.
-                NOTE: This feature is under current development.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an InsertOneResult object.
 
         Example:
             >>> async def write_and_count(acol: AsyncCollection) -> None:
             ...     count0 = await acol.count_documents({}, upper_bound=10)
@@ -2793,18 +3004,19 @@
         Note:
             If an `_id` is explicitly provided, which corresponds to a document
             that exists already in the collection, an error is raised and
             the insertion fails.
         """
 
         _document = _collate_vector_to_document(document, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"inserting one document in '{self.name}'")
         io_response = await self._astra_db_collection.insert_one(
             _document,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished inserting one document in '{self.name}'")
         if "insertedIds" in io_response.get("status", {}):
             if io_response["status"]["insertedIds"]:
                 inserted_id = io_response["status"]["insertedIds"][0]
                 return InsertOneResult(
                     raw_results=[io_response],
@@ -2824,15 +3036,15 @@
     @recast_method_async
     async def insert_many(
         self,
         documents: Iterable[DocumentType],
         *,
         vectors: Optional[Iterable[Optional[VectorType]]] = None,
         vectorize: Optional[Iterable[Optional[str]]] = None,
-        ordered: bool = True,
+        ordered: bool = False,
         chunk_size: Optional[int] = None,
         concurrency: Optional[int] = None,
         max_time_ms: Optional[int] = None,
     ) -> InsertManyResult:
         """
         Insert a list of documents into the collection.
         This is not an atomic operation.
@@ -2850,57 +3062,61 @@
                 Passing vectors this way is indeed equivalent to the "$vector" field
                 of the documents, however the two are mutually exclusive.
             vectorize: an optional list of strings to be made into as many vectors
                 (one per document), if such a service is configured for the collection.
                 Passing this parameter is equivalent to providing a `$vectorize`
                 field in the documents themselves, however the two are mutually exclusive.
                 For any given document, this parameter cannot coexist with the
-                corresponding `vector` entry.
-                NOTE: This feature is under current development.
-            ordered: if True (default), the insertions are processed sequentially.
-                If False, they can occur in arbitrary order and possibly concurrently.
+                corresponding entry in `vectors`.
+            ordered: if False (default), the insertions can occur in arbitrary order
+                and possibly concurrently. If True, they are processed sequentially.
+                If there are no specific reasons against it, unordered insertions are to
+                be preferred as they complete much faster.
             chunk_size: how many documents to include in a single API request.
                 Exceeding the server maximum allowed value results in an error.
                 Leave it unspecified (recommended) to use the system default.
             concurrency: maximum number of concurrent requests to the API at
                 a given time. It cannot be more than one for ordered insertions.
             max_time_ms: a timeout, in milliseconds, for the operation.
-
+                If not passed, the collection-level setting is used instead:
+                If many documents are being inserted, this method corresponds
+                to several HTTP requests: in such cases one may want to specify
+                a more tolerant timeout here.
         Returns:
             an InsertManyResult object.
 
         Examples:
             >>> async def write_and_count(acol: AsyncCollection) -> None:
             ...             count0 = await acol.count_documents({}, upper_bound=10)
             ...             print("count0", count0)
             ...             im_result1 = await acol.insert_many(
             ...                 [
             ...                     {"a": 10},
             ...                     {"a": 5},
             ...                     {"b": [True, False, False]},
             ...                 ],
+            ...                 ordered=True,
             ...             )
             ...             print("inserted1", im_result1.inserted_ids)
             ...             count1 = await acol.count_documents({}, upper_bound=100)
             ...             print("count1", count1)
             ...             await acol.insert_many(
             ...                 [{"seq": i} for i in range(50)],
-            ...                 ordered=False,
             ...                 concurrency=5,
             ...             )
             ...             count2 = await acol.count_documents({}, upper_bound=100)
             ...             print("count2", count2)
             ...
             >>> asyncio.run(write_and_count(my_async_coll))
             count0 0
             inserted1 ['e3c2a684-...', '1de4949f-...', '167dacc3-...']
             count1 3
             count2 53
 
-            # The following are three equivalent statements:
+            >>> # The following are three equivalent statements:
             >>> asyncio.run(my_async_coll.insert_many(
             ...     [{"tag": "a"}, {"tag": "b"}],
             ...     vectors=[[1, 2], [3, 4]],
             ... ))
             InsertManyResult(...)
             >>> asyncio.run(my_async_coll.insert_many(
             ...     [{"tag": "a", "$vector": [1, 2]}, {"tag": "b"}],
@@ -2953,17 +3169,18 @@
         if _concurrency > 1 and ordered:
             raise ValueError("Cannot run ordered insert_many concurrently.")
         if chunk_size is None:
             _chunk_size = MAX_INSERT_NUM_DOCUMENTS
         else:
             _chunk_size = chunk_size
         _documents = _collate_vectors_to_documents(documents, vectors, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"inserting {len(_documents)} documents in '{self.name}'")
         raw_results: List[Dict[str, Any]] = []
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         if ordered:
             options = {"ordered": True}
             inserted_ids: List[Any] = []
             for i in range(0, len(_documents), _chunk_size):
                 logger.info(f"inserting a chunk of documents in '{self.name}'")
                 chunk_response = await self._astra_db_collection.insert_many(
                     documents=_documents[i : i + _chunk_size],
@@ -3094,23 +3311,32 @@
         option in a non-vector-search manner.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the documents being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             skip: with this integer parameter, what would be the first `skip`
                 documents returned by the query are discarded, and the results
                 start from the (skip+1)-th document.
                 This parameter can be used only in conjunction with an explicit
                 `sort` criterion of the ascending/descending type (i.e. it cannot
                 be used when not sorting, nor with vector-based ANN search).
             limit: this (integer) parameter sets a limit over how many documents
@@ -3123,26 +3349,26 @@
                 criteria can be specified. Moreover, there is an upper bound
                 to the number of documents that can be returned. For details,
                 see the Note about upper bounds and the Data API documentation.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             include_similarity: a boolean to request the numeric value of the
                 similarity to be returned as an added "$similarity" key in each
                 returned document. Can only be used for vector ANN search, i.e.
                 when either `vector` is supplied or the `sort` parameter has the
                 shape {"$vector": ...}.
             sort: with this dictionary parameter one can control the order
                 the documents are returned. See the Note about sorting, as well as
                 the one about upper bounds, for details.
             max_time_ms: a timeout, in milliseconds, for each single one
                 of the underlying HTTP requests used to fetch documents as the
                 cursor is iterated over.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an AsyncCursor object representing iterations over the matching documents
             (see the AsyncCursor object for how to use it. The simplest thing is to
             run a for loop: `for document in collection.sort(...):`).
 
         Examples:
@@ -3188,15 +3414,15 @@
             ...             vector=[3, 3],
             ...         )
             ...     ]
             ...     return ann_tags
             ...
             >>> asyncio.run(run_vector_finds(my_async_coll))
             ['A', 'B', 'C']
-            # (assuming the collection has metric VectorMetric.COSINE)
+            >>> # (assuming the collection has metric VectorMetric.COSINE)
 
         Note:
             The following are example values for the `sort` parameter.
             When no particular order is required:
                 sort={}
             When sorting by a certain value in ascending/descending order:
                 sort={"field": SortDocuments.ASCENDING}
@@ -3232,24 +3458,25 @@
             It should be noted that the behavior of the cursor in the case documents
             have been added/removed after the `find` was started depends on database
             internals and it is not guaranteed, nor excluded, that such "real-time"
             changes in the data would be picked up by the cursor.
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         if include_similarity is not None and not _is_vector_sort(_sort):
             raise ValueError(
                 "Cannot use `include_similarity` when not searching through `vector`."
             )
         return (
             AsyncCursor(
                 collection=self,
                 filter=filter,
                 projection=projection,
-                max_time_ms=max_time_ms,
+                max_time_ms=_max_time_ms,
                 overall_max_time_ms=None,
             )
             .skip(skip)
             .limit(limit)
             .sort(_sort)
             .include_similarity(include_similarity)
         )
@@ -3270,42 +3497,51 @@
         provided filters, if any is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the documents being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to perform vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), extracting the most
                 similar document in the collection matching the filter.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             include_similarity: a boolean to request the numeric value of the
                 similarity to be returned as an added "$similarity" key in the
                 returned document. Can only be used for vector ANN search, i.e.
                 when either `vector` is supplied or the `sort` parameter has the
                 shape {"$vector": ...}.
             sort: with this dictionary parameter one can control the order
                 the documents are returned. See the Note about sorting for details.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary expressing the required document, otherwise None.
 
         Example:
             >>> async def demo_find_one(acol: AsyncCollection) -> None:
             ....    print("Count:", await acol.count_documents({}, upper_bound=100))
@@ -3328,32 +3564,37 @@
             Count: 50
             result0 {'_id': '479c7ce8-...', 'seq': 48}
             result1 {'_id': '93e992c4-...', 'seq': 10}
             result2 None
             result3 {'_id': '479c7ce8-...'}
             result4 {'_id': 'd656cd9d-...', 'seq': 49}
 
-            >>> asyncio.run(my_async_coll.find_one({}, vector=[1, 0]))
+            >>> asyncio.run(my_async_coll.find_one(
+            ...     {},
+            ...     vector=[1, 0],
+            ...     projection={"*": True},
+            ... ))
             {'_id': '...', 'tag': 'D', '$vector': [4.0, 1.0]}
 
         Note:
             See the `find` method for more details on the accepted parameters
             (whereas `skip` and `limit` are not valid parameters for `find_one`).
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         fo_cursor = self.find(
             filter=filter,
             projection=projection,
             skip=None,
             limit=1,
             vector=vector,
             vectorize=vectorize,
             include_similarity=include_similarity,
             sort=sort,
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         try:
             document = await fo_cursor.__anext__()
             return document  # type: ignore[no-any-return]
         except StopAsyncIteration:
             return None
 
@@ -3378,18 +3619,19 @@
                     "field.3.subfield"
                 If lists are encountered and no numeric index is specified,
                 all items in the list are visited.
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            max_time_ms: a timeout, in milliseconds, for the operation.
+            max_time_ms: a timeout, in milliseconds, with the same meaning as for `find`.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a list of all different values for `key` found across the documents
             that match the filter. The result list has no repeated items.
 
         Example:
             >>> async def run_distinct(acol: AsyncCollection) -> None:
@@ -3429,20 +3671,21 @@
 
         Note:
             For details on the behaviour of "distinct" in conjunction with
             real-time changes in the collection contents, see the
             Note of the `find` command.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         f_cursor = AsyncCursor(
             collection=self,
             filter=filter,
             projection={key: True},
             max_time_ms=None,
-            overall_max_time_ms=max_time_ms,
+            overall_max_time_ms=_max_time_ms,
         )
         return await f_cursor.distinct(key)  # type: ignore[no-any-return]
 
     @recast_method_async
     async def count_documents(
         self,
         filter: Dict[str, Any],
@@ -3454,24 +3697,25 @@
         Count the documents in the collection matching the specified filter.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             upper_bound: a required ceiling on the result of the count operation.
                 If the actual number of documents exceeds this value,
                 an exception will be raised.
                 Furthermore, if the actual number of documents exceeds the maximum
                 count that the Data API can reach (regardless of upper_bound),
                 an exception will be raised.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             the exact count of matching documents.
 
         Example:
             >>> async def do_count_docs(acol: AsyncCollection) -> None:
             ...     await acol.insert_many([{"seq": i} for i in range(20)])
@@ -3496,18 +3740,19 @@
             for sizeable amounts of documents (i.e. in the thousands and more)
             is discouraged in favor of alternative application-specific solutions.
             Keep in mind that the Data API has a hard upper limit on the amount
             of documents it will count, and that an exception will be thrown
             by this method if this limit is encountered.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info("calling count_documents")
         cd_response = await self._astra_db_collection.count_documents(
             filter=filter,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info("finished calling count_documents")
         if "count" in cd_response.get("status", {}):
             count: int = cd_response["status"]["count"]
             if cd_response["status"].get("moreData", False):
                 raise TooManyDocumentsToCountException(
                     text=f"Document count exceeds {count}, the maximum allowed by the server",
@@ -3535,25 +3780,27 @@
         """
         Query the API server for an estimate of the document count in the collection.
 
         Contrary to `count_documents`, this method has no filtering parameters.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a server-provided estimate count of the documents in the collection.
 
         Example:
             >>> asyncio.run(my_async_coll.estimated_document_count())
             35700
         """
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         ed_response = await self.command(
             {"estimatedDocumentCount": {}},
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         if "count" in ed_response.get("status", {}):
             count: int = ed_response["status"]["count"]
             return count
         else:
             raise DataAPIFaultyResponseException(
                 text="Faulty response from estimated_document_count API command.",
@@ -3580,50 +3827,59 @@
 
         Args:
 
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             replacement: the new document to write into the collection.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 replaced one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, `replacement` is inserted as a new document
                 if no matches are found on the collection. If False,
                 the operation silently does nothing in case of no matches.
             return_document: a flag controlling what document is returned:
                 if set to `ReturnDocument.BEFORE`, or the string "before",
                 the document found on database is returned; if set to
                 `ReturnDocument.AFTER`, or the string "after", the new
                 document is returned. The default is "before".
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             A document, either the one before the replace operation or the
             one after that. Alternatively, the method returns None to represent
             that no matching document was found, or that no replacement
             was inserted (depending on the `return_document` parameter).
 
@@ -3664,22 +3920,23 @@
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "returnDocument": return_document,
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_replace on '{self.name}'")
         fo_response = await self._astra_db_collection.find_one_and_replace(
             replacement=replacement,
             filter=filter,
             projection=normalize_optional_projection(projection),
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_replace on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             ret_document = fo_response.get("data", {}).get("document")
             if ret_document is None:
                 return None
             else:
@@ -3707,39 +3964,39 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             replacement: the new document to write into the collection.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 replaced one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, `replacement` is inserted as a new document
                 if no matches are found on the collection. If False,
                 the operation silently does nothing in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an UpdateResult object summarizing the outcome of the replace operation.
 
         Example:
             >>> async def do_replace_one(acol: AsyncCollection) -> None:
             ...     await acol.insert_one({"Marco": "Polo"})
@@ -3769,21 +4026,22 @@
             result2.update_info {'n': 1, 'updatedExisting': False, 'ok': 1.0, 'nModified': 0, 'upserted': '30e34e00-...'}
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_replace on '{self.name}'")
         fo_response = await self._astra_db_collection.find_one_and_replace(
             replacement=replacement,
             filter=filter,
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_replace on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             fo_status = fo_response.get("status") or {}
             _update_info = _prepare_update_info([fo_status])
             return UpdateResult(
                 raw_results=[fo_response],
@@ -3814,41 +4072,49 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the document, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 updated one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a new document (resulting from applying the `update`
                 to an empty document) is inserted if no matches are found on
@@ -3856,14 +4122,15 @@
                 in case of no matches.
             return_document: a flag controlling what document is returned:
                 if set to `ReturnDocument.BEFORE`, or the string "before",
                 the document found on database is returned; if set to
                 `ReturnDocument.AFTER`, or the string "after", the new
                 document is returned. The default is "before".
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             A document (or a projection thereof, as required), either the one
             before the replace operation or the one after that.
             Alternatively, the method returns None to represent
             that no matching document was found, or that no update
             was applied (depending on the `return_document` parameter).
@@ -3905,22 +4172,23 @@
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "returnDocument": return_document,
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_update on '{self.name}'")
         fo_response = await self._astra_db_collection.find_one_and_update(
             update=update,
             filter=filter,
             projection=normalize_optional_projection(projection),
             sort=_sort,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_update on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             ret_document = fo_response.get("data", {}).get("document")
             if ret_document is None:
                 return None
             else:
@@ -3948,16 +4216,16 @@
         optionally inserting a new one if no match is found.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the document, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
@@ -3968,25 +4236,25 @@
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 updated one. See the `find` method for more on sorting.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a new document (resulting from applying the `update`
                 to an empty document) is inserted if no matches are found on
                 the collection. If False, the operation silently does nothing
                 in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             an UpdateResult object summarizing the outcome of the update operation.
 
         Example:
             >>> async def do_update_one(acol: AsyncCollection) -> None:
             ...     await acol.insert_one({"Marco": "Polo"})
@@ -4013,21 +4281,22 @@
             result2.update_info {'n': 1, 'updatedExisting': False, 'ok': 1.0, 'nModified': 0, 'upserted': '75748092-...'}
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         options = {
             "upsert": upsert,
         }
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_update on '{self.name}'")
         fo_response = await self._astra_db_collection.find_one_and_update(
             update=update,
             sort=_sort,
             filter=filter,
             options=options,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_update on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             fo_status = fo_response.get("status") or {}
             _update_info = _prepare_update_info([fo_status])
             return UpdateResult(
                 raw_results=[fo_response],
@@ -4053,29 +4322,33 @@
         optionally inserting one documents in absence of matches.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             update: the update prescription to apply to the documents, expressed
                 as a dictionary as per Data API syntax. Examples are:
                     {"$set": {"field": "value}}
                     {"$inc": {"counter": 10}}
                     {"$unset": {"field": ""}}
                 See the Data API documentation for the full syntax.
             upsert: this parameter controls the behavior in absence of matches.
                 If True, a single new document (resulting from applying `update`
                 to an empty document) is inserted if no matches are found on
                 the collection. If False, the operation silently does nothing
                 in case of no matches.
             max_time_ms: a timeout, in milliseconds, for the operation.
+                If not passed, the collection-level setting is used instead:
+                if a large number of document updates is anticipated, it is suggested
+                to specify a larger timeout than in most other operations as the
+                update will span several HTTP calls to the API in sequence.
 
         Returns:
             an UpdateResult object summarizing the outcome of the update operation.
 
         Example:
             >>> async def do_update_many(acol: AsyncCollection) -> None:
             ...     await acol.insert_many([{"c": "red"}, {"c": "green"}, {"c": "blue"}])
@@ -4106,25 +4379,26 @@
             running this command while, at the same time, another process is
             inserting new documents which match the filter of the `update_many`
             can result in an unpredictable fraction of these documents being updated.
             In other words, it cannot be easily predicted whether a given
             newly-inserted document will be picked up by the update_many command or not.
         """
 
-        base_options = {
+        api_options = {
             "upsert": upsert,
         }
         page_state_options: Dict[str, str] = {}
         um_responses: List[Dict[str, Any]] = []
         um_statuses: List[Dict[str, Any]] = []
         must_proceed = True
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"starting update_many on '{self.name}'")
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         while must_proceed:
-            options = {**base_options, **page_state_options}
+            options = {**api_options, **page_state_options}
             logger.info(f"calling update_many on '{self.name}'")
             this_um_response = await self._astra_db_collection.update_many(
                 update=update,
                 filter=filter,
                 options=options,
                 timeout_info=timeout_manager.remaining_timeout_info(),
             )
@@ -4183,42 +4457,49 @@
         however, is the return value of the method.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
-            projection: used to select a subset of fields in the document being
-                returned. The projection can be: an iterable over the field names
-                to return; a dictionary {field_name: True} to positively select
-                certain fields; or a dictionary {field_name: False} if one wants
-                to discard some fields from the response.
-                Note that the `_id` field will be returned with the document
-                in any case, regardless of what the provided `projection` requires.
-                The default is to return the whole documents.
+            projection: it controls which parts of the document are returned.
+                It can be an allow-list: `{"f1": True, "f2": True}`,
+                or a deny-list: `{"fx": False, "fy": False}`, but not a mixture
+                (except for the `_id` field, which can be associated to both
+                True or False independently of the rest of the specification).
+                The special star-projections `{"*": True}` and `{"*": False}`
+                have the effect of returning the whole document and `{}` respectively.
+                For lists in documents, slice directives can be passed to select
+                portions of the list: for instance, `{"array": {"$slice": 2}}`,
+                `{"array": {"$slice": -2}}`, `{"array": {"$slice": [4, 2]}}` or
+                `{"array": {"$slice": [-4, 2]}}`.
+                An iterable over strings will be treated implicitly as an allow-list.
+                The default projection if this parameter is not passed) does not
+                necessarily include "special" fields such as `$vector` or `$vectorize`.
+                See the Data API documentation for more on projections.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 deleted one. See the `find` method for more on sorting.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             Either the document (or a projection thereof, as requested), or None
             if no matches were found in the first place.
 
         Example:
             >>> async def do_find_one_and_delete(acol: AsyncCollection) -> None:
@@ -4241,20 +4522,21 @@
             >>> asyncio.run(do_find_one_and_delete(my_async_coll))
             delete_result0 {'_id': 'f335cd0f-...', 'species': 'swan'}
             delete_result1 None
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
         _projection = normalize_optional_projection(projection)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling find_one_and_delete on '{self.name}'")
         fo_response = await self._astra_db_collection.find_one_and_delete(
             sort=_sort,
             filter=filter,
             projection=_projection,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
         )
         logger.info(f"finished calling find_one_and_delete on '{self.name}'")
         if "document" in fo_response.get("data", {}):
             document = fo_response["data"]["document"]
             return document  # type: ignore[no-any-return]
         else:
             deleted_count = fo_response.get("status", {}).get("deletedCount")
@@ -4282,34 +4564,34 @@
         of the number of matches to the provided filters.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
             vector: a suitable vector, i.e. a list of float numbers of the appropriate
                 dimensionality, to use vector search (i.e. ANN,
                 or "approximate nearest-neighbours" search), as the sorting criterion.
                 In this way, the matched document (if any) will be the one
                 that is most similar to the provided vector.
                 This parameter cannot be used together with `sort`.
                 See the `find` method for more details on this parameter.
             vectorize: a string to be made into a vector to perform vector search.
                 This can be supplied in (exclusive) alternative to `vector`,
                 provided such a service is configured for the collection,
                 and achieves the same effect.
-                NOTE: This feature is under current development.
             sort: with this dictionary parameter one can control the sorting
                 order of the documents matching the filter, effectively
                 determining what document will come first and hence be the
                 deleted one. See the `find` method for more on sorting.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a DeleteResult object summarizing the outcome of the delete operation.
 
         Example:
             >>> my_coll.insert_many([{"seq": 1}, {"seq": 0}, {"seq": 2}])
             InsertManyResult(...)
@@ -4325,18 +4607,19 @@
             >>> my_coll.distinct("seq")
             [0]
             >>> my_coll.delete_one({"seq": 2})
             DeleteResult(raw_results=..., deleted_count=0)
         """
 
         _sort = _collate_vector_to_sort(sort, vector, vectorize)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling delete_one_by_predicate on '{self.name}'")
         do_response = await self._astra_db_collection.delete_one_by_predicate(
             filter=filter,
-            timeout_info=base_timeout_info(max_time_ms),
+            timeout_info=base_timeout_info(_max_time_ms),
             sort=_sort,
         )
         logger.info(f"finished calling delete_one_by_predicate on '{self.name}'")
         if "deletedCount" in do_response.get("status", {}):
             deleted_count = do_response["status"]["deletedCount"]
             if deleted_count == -1:
                 return DeleteResult(
@@ -4366,20 +4649,25 @@
         Delete all documents matching a provided filter.
 
         Args:
             filter: a predicate expressed as a dictionary according to the
                 Data API filter syntax. Examples are:
                     {}
                     {"name": "John"}
-                    {"price": {"$le": 100}}
-                    {"$and": [{"name": "John"}, {"price": {"$le": 100}}]}
+                    {"price": {"$lt": 100}}
+                    {"$and": [{"name": "John"}, {"price": {"$lt": 100}}]}
                 See the Data API documentation for the full set of operators.
                 The `delete_many` method does not accept an empty filter: see
                 `delete_all` to completely erase all contents of a collection
             max_time_ms: a timeout, in milliseconds, for the operation.
+                If not passed, the collection-level setting is used instead:
+                keep in mind that this method entails successive HTTP requests
+                to the API, depending on how many documents are to be deleted.
+                For this reason, in most cases it is suggested to relax the
+                timeout compared to other method calls.
 
         Returns:
             a DeleteResult object summarizing the outcome of the delete operation.
 
         Example:
             >>> async def do_delete_many(acol: AsyncCollection) -> None:
             ...     await acol.insert_many([{"seq": 1}, {"seq": 0}, {"seq": 2}])
@@ -4410,15 +4698,16 @@
                 "empty. In order to completely clear the contents of a "
                 "collection, please use the `delete_all` method."
             )
 
         dm_responses: List[Dict[str, Any]] = []
         deleted_count = 0
         must_proceed = True
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         logger.info(f"starting delete_many on '{self.name}'")
         while must_proceed:
             logger.info(f"calling delete_many on '{self.name}'")
             this_dm_response = await self._astra_db_collection.delete_many(
                 filter=filter,
                 skip_error_check=True,
                 timeout_info=timeout_manager.remaining_timeout_info(),
@@ -4456,14 +4745,15 @@
     @recast_method_async
     async def delete_all(self, *, max_time_ms: Optional[int] = None) -> Dict[str, Any]:
         """
         Delete all documents in a collection.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary of the form {"ok": 1} to signal successful deletion.
 
         Example:
             >>> async def do_delete_all(acol: AsyncCollection) -> None:
             ...     distinct0 = await acol.distinct("seq")
@@ -4479,26 +4769,20 @@
             distinct0 [4, 2, 3, 0, 1]
             count1 5
             delete_result2 {'ok': 1}
             count3 0
 
         Note:
             Use with caution.
-
-        Note:
-            Once the method succeeds, methods on this object can still be invoked:
-            however, this hardly makes sense as the underlying actual collection
-            is no more.
-            It is responsibility of the developer to design a correct flow
-            which avoids using a deceased collection any further.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling unfiltered delete_many on '{self.name}'")
         dm_response = await self._astra_db_collection.delete_many(
-            filter={}, timeout_info=base_timeout_info(max_time_ms)
+            filter={}, timeout_info=base_timeout_info(_max_time_ms)
         )
         logger.info(f"finished calling unfiltered delete_many on '{self.name}'")
         deleted_count = dm_response["status"]["deletedCount"]
         if deleted_count == -1:
             return {"ok": 1}
         else:
             raise DataAPIFaultyResponseException(
@@ -4506,15 +4790,15 @@
                 raw_response=dm_response,
             )
 
     async def bulk_write(
         self,
         requests: Iterable[AsyncBaseOperation],
         *,
-        ordered: bool = True,
+        ordered: bool = False,
         concurrency: Optional[int] = None,
         max_time_ms: Optional[int] = None,
     ) -> BulkWriteResult:
         """
         Execute an arbitrary amount of operations such as inserts, updates, deletes
         either sequentially or concurrently.
 
@@ -4526,22 +4810,25 @@
             requests: an iterable over concrete subclasses of `BaseOperation`,
                 such as `AsyncInsertMany` or `AsyncReplaceOne`. Each such object
                 represents an operation ready to be executed on a collection,
                 and is instantiated by passing the same parameters as one
                 would the corresponding collection method.
             ordered: whether to launch the `requests` one after the other or
                 in arbitrary order, possibly in a concurrent fashion. For
-                performance reasons, `ordered=False` should be preferred
+                performance reasons, False (default) should be preferred
                 when compatible with the needs of the application flow.
             concurrency: maximum number of concurrent operations executing at
                 a given time. It cannot be more than one for ordered bulk writes.
             max_time_ms: a timeout, in milliseconds, for the whole bulk write.
                 Remember that, if the method call times out, then there's no
                 guarantee about what portion of the bulk write has been received
                 and successfully executed by the Data API.
+                If not passed, the collection-level setting is used instead:
+                in most cases, however, one should pass a relaxed timeout
+                if longer sequences of operations are to be executed in bulk.
 
         Returns:
             A single BulkWriteResult summarizing the whole list of requested
             operations. The keys in the map attributes of BulkWriteResult
             (when present) are the integer indices of the corresponding operation
             in the `requests` iterable.
 
@@ -4581,16 +4868,17 @@
                 _concurrency = 1
             else:
                 _concurrency = DEFAULT_BULK_WRITE_CONCURRENCY
         else:
             _concurrency = concurrency
         if _concurrency > 1 and ordered:
             raise ValueError("Cannot run ordered bulk_write concurrently.")
-        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=max_time_ms)
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"startng a bulk write on '{self.name}'")
+        timeout_manager = MultiCallTimeoutManager(overall_max_time_ms=_max_time_ms)
         if ordered:
             bulk_write_results: List[BulkWriteResult] = []
             for operation_i, operation in enumerate(requests):
                 try:
                     this_bw_result = await operation.execute(
                         self,
                         index_in_bulk_write=operation_i,
@@ -4691,14 +4979,15 @@
     async def drop(self, *, max_time_ms: Optional[int] = None) -> Dict[str, Any]:
         """
         Drop the collection, i.e. delete it from the database along with
         all the documents it contains.
 
         Args:
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
                 Remember there is not guarantee that a request that has
                 timed out us not in fact honored.
 
         Returns:
             a dictionary of the form {"ok": 1} to signal successful deletion.
 
         Example:
@@ -4723,16 +5012,19 @@
             Once the method succeeds, methods on this object can still be invoked:
             however, this hardly makes sense as the underlying actual collection
             is no more.
             It is responsibility of the developer to design a correct flow
             which avoids using a deceased collection any further.
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"dropping collection '{self.name}' (self)")
-        drop_result = await self.database.drop_collection(self, max_time_ms=max_time_ms)
+        drop_result = await self.database.drop_collection(
+            self, max_time_ms=_max_time_ms
+        )
         logger.info(f"finished dropping collection '{self.name}' (self)")
         return drop_result  # type: ignore[no-any-return]
 
     async def command(
         self,
         body: Dict[str, Any],
         *,
@@ -4741,25 +5033,27 @@
         """
         Send a POST request to the Data API for this collection with
         an arbitrary, caller-provided payload.
 
         Args:
             body: a JSON-serializable dictionary, the payload of the request.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+                If not passed, the collection-level setting is used instead.
 
         Returns:
             a dictionary with the response of the HTTP request.
 
         Example:
             >>> asyncio.await(my_async_coll.command({"countDocuments": {}}))
             {'status': {'count': 123}}
         """
 
+        _max_time_ms = max_time_ms or self.api_options.max_time_ms
         logger.info(f"calling command on '{self.name}'")
         command_result = await self.database.command(
             body=body,
             namespace=self.namespace,
             collection_name=self.name,
-            max_time_ms=max_time_ms,
+            max_time_ms=_max_time_ms,
         )
         logger.info(f"finished calling command on '{self.name}'")
         return command_result  # type: ignore[no-any-return]
```

### Comparing `astrapy-1.1.0/astrapy/constants.py` & `astrapy-1.2.0/astrapy/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,39 +14,36 @@
 
 from __future__ import annotations
 
 from typing import Any, Dict, Iterable, Optional, Union
 
 
 DocumentType = Dict[str, Any]
-ProjectionType = Union[Iterable[str], Dict[str, bool]]
+# ["field1", "field2"] allowed, but also:
+# {"field": True/False}
+# {"array_field": {"$slice": n}
+# {"array_field": {"$slice": [n, m]}
+ProjectionType = Union[
+    Iterable[str], Dict[str, Union[bool, Dict[str, Union[int, Iterable[int]]]]]
+]
 SortType = Dict[str, Any]
 FilterType = Dict[str, Any]
 VectorType = Iterable[float]
 
 
 def normalize_optional_projection(
     projection: Optional[ProjectionType],
-    ensure_fields: Iterable[str] = set(),
-) -> Optional[Dict[str, bool]]:
-    _ensure_fields = set(ensure_fields)
+) -> Optional[Dict[str, Union[bool, Dict[str, Union[int, Iterable[int]]]]]]:
     if projection:
         if isinstance(projection, dict):
-            if any(bool(v) for v in projection.values()):
-                # positive projection: {a: True, b: True ...}
-                return {
-                    k: projection.get(k, True)
-                    for k in list(projection.keys()) + list(_ensure_fields)
-                }
-            else:
-                # negative projection: {x: False, y: False, ...}
-                return {k: v for k, v in projection.items() if k not in _ensure_fields}
+            # already a dictionary
+            return projection
         else:
-            # an iterable over strings
-            return {field: True for field in list(projection) + list(_ensure_fields)}
+            # an iterable over strings: coerce to allow-list projection
+            return {field: True for field in projection}
     else:
         return None
 
 
 class ReturnDocument:
     """
     Admitted values for the `return_document` parameter in
@@ -100,10 +97,29 @@
     UUID = "uuid"
     OBJECTID = "objectId"
     UUIDV6 = "uuidv6"
     UUIDV7 = "uuidv7"
     DEFAULT = "uuid"
 
 
+class Environment:
+    """
+    Admitted values for `environment` property,
+    denoting the targeted API deployment type.
+    """
+
+    def __init__(self) -> None:
+        raise NotImplementedError
+
+    PROD = "prod"
+    DEV = "dev"
+    TEST = "test"
+    DSE = "dse"
+    OTHER = "other"
+
+    values = {PROD, DEV, TEST, DSE, OTHER}
+    astra_db_values = {PROD, DEV, TEST}
+
+
 __pdoc__ = {
     "normalize_optional_projection": False,
 }
```

### Comparing `astrapy-1.1.0/astrapy/core/__init__.py` & `astrapy-1.2.0/astrapy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/core/api.py` & `astrapy-1.2.0/astrapy/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,27 +45,29 @@
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> httpx.Response:
     return make_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
         timeout=timeout,
+        additional_headers=additional_headers,
     )
 
 
 def process_raw_api_response(
     raw_response: httpx.Response,
     skip_error_check: bool,
     json_data: Optional[Dict[str, Any]],
@@ -97,27 +99,29 @@
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     skip_error_check: bool,
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> API_RESPONSE:
     raw_response = raw_api_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
         timeout=timeout,
+        additional_headers=additional_headers,
     )
     raw_response.raise_for_status()
     return process_raw_api_response(
         raw_response, skip_error_check=skip_error_check, json_data=json_data
     )
 
 
@@ -130,27 +134,29 @@
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> httpx.Response:
     return await amake_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
         timeout=timeout,
+        additional_headers=additional_headers,
     )
 
 
 async def async_process_raw_api_response(
     raw_response: httpx.Response,
     skip_error_check: bool,
     json_data: Optional[Dict[str, Any]],
@@ -182,27 +188,29 @@
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     skip_error_check: bool,
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> API_RESPONSE:
     raw_response = await async_raw_api_request(
         client=client,
         base_url=base_url,
         auth_header=auth_header,
         token=token,
         method=method,
         json_data=json_data,
         url_params=url_params,
         path=path,
         caller_name=caller_name,
         caller_version=caller_version,
         timeout=timeout,
+        additional_headers=additional_headers,
     )
     raw_response.raise_for_status()
     return await async_process_raw_api_response(
         raw_response,
         skip_error_check=skip_error_check,
         json_data=json_data,
     )
```

### Comparing `astrapy-1.1.0/astrapy/core/core_types.py` & `astrapy-1.2.0/astrapy/core/core_types.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/core/db.py` & `astrapy-1.2.0/astrapy/core/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,28 +80,32 @@
         collection_name: str,
         astra_db: Optional[AstraDB] = None,
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        additional_headers: Dict[str, str] = {},
     ) -> None:
         """
         Initialize an AstraDBCollection instance.
 
         Args:
             collection_name (str): The name of the collection.
             astra_db (AstraDB, optional): An instance of Astra DB.
             token (str, optional): Authentication token for Astra DB.
             api_endpoint (str, optional): API endpoint URL.
             namespace (str, optional): Namespace for the database.
             caller_name (str, optional): identity of the caller ("my_framework")
                 If passing a client, its caller is used as fallback
             caller_version (str, optional): version of the caller code ("1.0.3")
                 If passing a client, its caller is used as fallback
+            additional_headers (Dict[str, str]): any further set of headers,
+                in the form of key-value pairs, to be passed with the HTTP
+                requests by this collection instance.
         """
         # Check for presence of the Astra DB object
         if astra_db is None:
             if token is None or api_endpoint is None:
                 raise AssertionError("Must provide token and api_endpoint")
 
             astra_db = AstraDB(
@@ -121,28 +125,30 @@
                 caller_version=caller_version,
             )
 
         # Set the remaining instance attributes
         self.astra_db = astra_db
         self.caller_name: Optional[str] = self.astra_db.caller_name
         self.caller_version: Optional[str] = self.astra_db.caller_version
+        self.additional_headers = additional_headers
         self.collection_name = collection_name
         self.base_path: str = f"{self.astra_db.base_path}/{self.collection_name}"
 
     def __repr__(self) -> str:
         return f'AstraDBCollection[astra_db="{self.astra_db}", collection_name="{self.collection_name}"]'
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, AstraDBCollection):
             return all(
                 [
                     self.collection_name == other.collection_name,
                     self.astra_db == other.astra_db,
                     self.caller_name == other.caller_name,
                     self.caller_version == other.caller_version,
+                    self.additional_headers == other.additional_headers,
                 ]
             )
         else:
             return False
 
     def copy(
         self,
@@ -151,36 +157,39 @@
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        additional_headers: Optional[Dict[str, str]] = None,
     ) -> AstraDBCollection:
         return AstraDBCollection(
             collection_name=collection_name or self.collection_name,
             astra_db=self.astra_db.copy(
                 token=token,
                 api_endpoint=api_endpoint,
                 api_path=api_path,
                 api_version=api_version,
                 namespace=namespace,
                 caller_name=caller_name,
                 caller_version=caller_version,
             ),
             caller_name=caller_name or self.caller_name,
             caller_version=caller_version or self.caller_version,
+            additional_headers=additional_headers or self.additional_headers,
         )
 
     def to_async(self) -> AsyncAstraDBCollection:
         return AsyncAstraDBCollection(
             collection_name=self.collection_name,
             astra_db=self.astra_db.to_async(),
             caller_name=self.caller_name,
             caller_version=self.caller_version,
+            additional_headers=self.additional_headers,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> None:
@@ -209,14 +218,15 @@
             json_data=normalize_for_api(json_data),
             url_params=url_params,
             path=path,
             skip_error_check=skip_error_check,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers=self.additional_headers,
         )
         response = restore_from_api(direct_response)
         return response
 
     def post_raw_request(
         self, body: Dict[str, Any], timeout_info: TimeoutInfoWideType = None
     ) -> API_RESPONSE:
@@ -1451,28 +1461,32 @@
         collection_name: str,
         astra_db: Optional[AsyncAstraDB] = None,
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        additional_headers: Dict[str, str] = {},
     ) -> None:
         """
         Initialize an AstraDBCollection instance.
 
         Args:
             collection_name (str): The name of the collection.
             astra_db (AstraDB, optional): An instance of Astra DB.
             token (str, optional): Authentication token for Astra DB.
             api_endpoint (str, optional): API endpoint URL.
             namespace (str, optional): Namespace for the database.
             caller_name (str, optional): identity of the caller ("my_framework")
                 If passing a client, its caller is used as fallback
             caller_version (str, optional): version of the caller code ("1.0.3")
                 If passing a client, its caller is used as fallback
+            additional_headers (Dict[str, str]): any further set of headers,
+                in the form of key-value pairs, to be passed with the HTTP
+                requests by this collection instance.
         """
         # Check for presence of the Astra DB object
         if astra_db is None:
             if token is None or api_endpoint is None:
                 raise AssertionError("Must provide token and api_endpoint")
 
             astra_db = AsyncAstraDB(
@@ -1492,14 +1506,15 @@
                 caller_version=caller_version,
             )
 
         # Set the remaining instance attributes
         self.astra_db: AsyncAstraDB = astra_db
         self.caller_name: Optional[str] = self.astra_db.caller_name
         self.caller_version: Optional[str] = self.astra_db.caller_version
+        self.additional_headers = additional_headers
         self.client = astra_db.client
         self.collection_name = collection_name
         self.base_path: str = f"{self.astra_db.base_path}/{self.collection_name}"
 
     def __repr__(self) -> str:
         return f'AsyncAstraDBCollection[astra_db="{self.astra_db}", collection_name="{self.collection_name}"]'
 
@@ -1507,14 +1522,15 @@
         if isinstance(other, AsyncAstraDBCollection):
             return all(
                 [
                     self.collection_name == other.collection_name,
                     self.astra_db == other.astra_db,
                     self.caller_name == other.caller_name,
                     self.caller_version == other.caller_version,
+                    self.additional_headers == other.additional_headers,
                 ]
             )
         else:
             return False
 
     def copy(
         self,
@@ -1523,28 +1539,30 @@
         token: Optional[str] = None,
         api_endpoint: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        additional_headers: Optional[Dict[str, str]] = None,
     ) -> AsyncAstraDBCollection:
         return AsyncAstraDBCollection(
             collection_name=collection_name or self.collection_name,
             astra_db=self.astra_db.copy(
                 token=token,
                 api_endpoint=api_endpoint,
                 api_path=api_path,
                 api_version=api_version,
                 namespace=namespace,
                 caller_name=caller_name,
                 caller_version=caller_version,
             ),
             caller_name=caller_name or self.caller_name,
             caller_version=caller_version or self.caller_version,
+            additional_headers=additional_headers or self.additional_headers,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
     ) -> None:
@@ -1557,14 +1575,15 @@
 
     def to_sync(self) -> AstraDBCollection:
         return AstraDBCollection(
             collection_name=self.collection_name,
             astra_db=self.astra_db.to_sync(),
             caller_name=self.caller_name,
             caller_version=self.caller_version,
+            additional_headers=self.additional_headers,
         )
 
     async def _request(
         self,
         method: str = http_methods.POST,
         path: Optional[str] = None,
         json_data: Optional[Dict[str, Any]] = None,
@@ -1582,14 +1601,15 @@
             json_data=normalize_for_api(json_data),
             url_params=url_params,
             path=path,
             skip_error_check=skip_error_check,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers=self.additional_headers,
         )
         response = restore_from_api(adirect_response)
         return response
 
     async def post_raw_request(
         self, body: Dict[str, Any], timeout_info: TimeoutInfoWideType = None
     ) -> API_RESPONSE:
@@ -2827,22 +2847,31 @@
 
         self.api_endpoint = api_endpoint
 
         # Set the Base URL for the API calls
         self.base_url = self.api_endpoint.strip("/")
 
         # Set the API version and path from the call
-        self.api_path = (api_path or DEFAULT_JSON_API_PATH).strip("/")
-        self.api_version = (api_version or DEFAULT_JSON_API_VERSION).strip("/")
+        self.api_path = (DEFAULT_JSON_API_PATH if api_path is None else api_path).strip(
+            "/"
+        )
+        self.api_version = (
+            DEFAULT_JSON_API_VERSION if api_version is None else api_version
+        ).strip("/")
 
         # Set the namespace
         self.namespace = namespace
 
         # Finally, construct the full base path
-        self.base_path: str = f"/{self.api_path}/{self.api_version}/{self.namespace}"
+        base_path_components = [
+            comp
+            for comp in (self.api_path, self.api_version, self.namespace)
+            if comp != ""
+        ]
+        self.base_path: str = f"/{'/'.join(base_path_components)}"
 
     def __repr__(self) -> str:
         return f'AstraDB[endpoint="{self.base_url}", keyspace="{self.namespace}"]'
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, AstraDB):
             # work on the "normalized" quantities (stripped, etc)
@@ -2916,14 +2945,15 @@
             json_data=normalize_for_api(json_data),
             url_params=url_params,
             path=path,
             skip_error_check=skip_error_check,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         response = restore_from_api(direct_response)
         return response
 
     def post_raw_request(
         self, body: Dict[str, Any], timeout_info: TimeoutInfoWideType = None
     ) -> API_RESPONSE:
@@ -2997,15 +3027,14 @@
 
         Args:
             collection_name (str): The name of the collection to create.
             options (dict, optional): Options for the collection.
             dimension (int, optional): Dimension for vector search.
             metric (str, optional): Metric choice for vector search.
             service_dict (dict, optional): a definition for the $vectorize service
-                NOTE: This feature is under current development.
             timeout_info: a float, or a TimeoutInfo dict, for the HTTP request.
                 Note that a 'read' timeout event will not block the action taken
                 by the API server if it has received the request already.
 
         Returns:
             AstraDBCollection: The created collection object.
         """
@@ -3163,22 +3192,31 @@
 
         self.api_endpoint = api_endpoint
 
         # Set the Base URL for the API calls
         self.base_url = self.api_endpoint.strip("/")
 
         # Set the API version and path from the call
-        self.api_path = (api_path or DEFAULT_JSON_API_PATH).strip("/")
-        self.api_version = (api_version or DEFAULT_JSON_API_VERSION).strip("/")
+        self.api_path = (DEFAULT_JSON_API_PATH if api_path is None else api_path).strip(
+            "/"
+        )
+        self.api_version = (
+            DEFAULT_JSON_API_VERSION if api_version is None else api_version
+        ).strip("/")
 
         # Set the namespace
         self.namespace = namespace
 
         # Finally, construct the full base path
-        self.base_path: str = f"/{self.api_path}/{self.api_version}/{self.namespace}"
+        base_path_components = [
+            comp
+            for comp in (self.api_path, self.api_version, self.namespace)
+            if comp != ""
+        ]
+        self.base_path: str = f"/{'/'.join(base_path_components)}"
 
     def __repr__(self) -> str:
         return f'AsyncAstraDB[endpoint="{self.base_url}", keyspace="{self.namespace}"]'
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, AsyncAstraDB):
             # work on the "normalized" quantities (stripped, etc)
@@ -3263,14 +3301,15 @@
             json_data=normalize_for_api(json_data),
             url_params=url_params,
             path=path,
             skip_error_check=skip_error_check,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         response = restore_from_api(adirect_response)
         return response
 
     async def post_raw_request(
         self, body: Dict[str, Any], timeout_info: TimeoutInfoWideType = None
     ) -> API_RESPONSE:
@@ -3347,15 +3386,14 @@
 
         Args:
             collection_name (str): The name of the collection to create.
             options (dict, optional): Options for the collection.
             dimension (int, optional): Dimension for vector search.
             metric (str, optional): Metric choice for vector search.
             service_dict (dict, optional): a definition for the $vectorize service
-                NOTE: This feature is under current development.
             timeout_info: a float, or a TimeoutInfo dict, for the HTTP request.
                 Note that a 'read' timeout event will not block the action taken
                 by the API server if it has received the request already.
 
         Returns:
             AsyncAstraDBCollection: The created collection object.
         """
```

### Comparing `astrapy-1.1.0/astrapy/core/defaults.py` & `astrapy-1.2.0/astrapy/core/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,9 @@
 
 DEFAULT_TIMEOUT = 30000
 DEFAULT_AUTH_HEADER = "Token"
 DEFAULT_KEYSPACE_NAME = "default_keyspace"
 DEFAULT_REGION = "us-east1"
 
 MAX_INSERT_NUM_DOCUMENTS = 20
+
+DEFAULT_VECTORIZE_SECRET_HEADER = "x-embedding-api-key"
```

### Comparing `astrapy-1.1.0/astrapy/core/ids.py` & `astrapy-1.2.0/astrapy/core/ids.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/core/ops.py` & `astrapy-1.2.0/astrapy/core/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,15 @@
             method=method,
             json_data=json_data,
             url_params=_options,
             path=path,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         return raw_response
 
     async def _async_ops_request(
         self,
         method: str,
         path: str,
@@ -165,14 +166,15 @@
             method=method,
             json_data=json_data,
             url_params=_options,
             path=path,
             caller_name=self.caller_name,
             caller_version=self.caller_version,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         return raw_response
 
     def _json_ops_request(
         self,
         method: str,
         path: str,
@@ -191,14 +193,15 @@
             json_data=json_data,
             url_params=_options,
             path=path,
             skip_error_check=False,
             caller_name=None,
             caller_version=None,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         return response
 
     async def _async_json_ops_request(
         self,
         method: str,
         path: str,
@@ -217,14 +220,15 @@
             json_data=json_data,
             url_params=_options,
             path=path,
             skip_error_check=False,
             caller_name=None,
             caller_version=None,
             timeout=to_httpx_timeout(timeout_info),
+            additional_headers={},
         )
         return response
 
     def get_databases(
         self,
         options: Optional[Dict[str, Any]] = None,
         timeout_info: TimeoutInfoWideType = None,
```

### Comparing `astrapy-1.1.0/astrapy/core/utils.py` & `astrapy-1.2.0/astrapy/core/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,19 @@
 import datetime
 import logging
 import copy
 
 import httpx
 
 from astrapy import __version__
-from astrapy.core.defaults import DEFAULT_AUTH_HEADER, DEFAULT_TIMEOUT
+from astrapy.core.defaults import (
+    DEFAULT_AUTH_HEADER,
+    DEFAULT_VECTORIZE_SECRET_HEADER,
+    DEFAULT_TIMEOUT,
+)
 from astrapy.core.core_types import API_RESPONSE
 from astrapy.core.ids import ObjectId, UUID
 
 
 class CustomLogger(logging.Logger):
     def trace(self, msg: str, *args: Any, **kwargs: Any) -> None:
         if self.isEnabledFor(5):
@@ -99,15 +103,17 @@
     logger.debug(f"Request url: {url}")
     logger.debug(f"Request method: {method}")
     logger.debug(f"Request params: {params}")
 
     # Redact the token from the request headers
     headers_log = copy.deepcopy(headers)
     if DEFAULT_AUTH_HEADER in headers_log:
-        headers_log[DEFAULT_AUTH_HEADER] = "AstraCS:<...>"
+        headers_log[DEFAULT_AUTH_HEADER] = "***"
+    if DEFAULT_VECTORIZE_SECRET_HEADER in headers_log:
+        headers_log[DEFAULT_VECTORIZE_SECRET_HEADER] = "***"
 
     logger.debug(f"Request headers: {headers_log}")
 
     if json_data:
         logger.trace(f"Request payload: {json_data}")  # type: ignore
 
 
@@ -119,23 +125,30 @@
         r (requests.Response): The response object from the HTTP request.
     """
     logger.debug(f"Response status code: {r.status_code}")
     logger.debug(f"Response headers: {r.headers}")
     logger.debug(f"Response content: {r.text}")
 
 
-def compose_user_agent(
+def user_agent_string(
     caller_name: Optional[str], caller_version: Optional[str]
-) -> str:
-    user_agent_caller: Optional[str] = None
+) -> Optional[str]:
     if caller_name:
         if caller_version:
-            user_agent_caller = f"{caller_name}/{caller_version}"
+            return f"{caller_name}/{caller_version}"
         else:
-            user_agent_caller = f"{caller_name}"
+            return f"{caller_name}"
+    else:
+        return None
+
+
+def compose_user_agent(
+    caller_name: Optional[str], caller_version: Optional[str]
+) -> str:
+    user_agent_caller = user_agent_string(caller_name, caller_version)
     all_user_agents = [
         ua_block
         for ua_block in [
             user_agent_rs,
             user_agent_caller,
             user_agent_astrapy,
         ]
@@ -175,14 +188,15 @@
     method: str,
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     path: Optional[str],
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> httpx.Response:
     """
     Make an HTTP request to a specified URL.
 
     Args:
         client (httpx): The httpx client for the request.
         base_url (str): The base URL for the request.
@@ -194,16 +208,19 @@
         url_params (dict, optional): URL parameters to be sent with the request.
 
     Returns:
         requests.Response: The response from the HTTP request.
     """
     # Build the request headers from the token and user agent
     request_headers = {
-        auth_header: token,
-        "User-Agent": compose_user_agent(caller_name, caller_version),
+        **{
+            auth_header: token,
+            "User-Agent": compose_user_agent(caller_name, caller_version),
+        },
+        **additional_headers,
     }
 
     # Log the parameters of the request accordingly
     log_request(method, f"{base_url}{path}", url_params, request_headers, json_data)
 
     # Make the request
     r = client.request(
@@ -229,14 +246,15 @@
     method: str,
     path: Optional[str],
     json_data: Optional[Dict[str, Any]],
     url_params: Optional[Dict[str, Any]],
     caller_name: Optional[str],
     caller_version: Optional[str],
     timeout: Optional[Union[httpx.Timeout, float]],
+    additional_headers: Dict[str, str],
 ) -> httpx.Response:
     """
     Make an HTTP request to a specified URL.
 
     Args:
         client (httpx): The httpx client for the request.
         base_url (str): The base URL for the request.
@@ -248,16 +266,19 @@
         url_params (dict, optional): URL parameters to be sent with the request.
 
     Returns:
         requests.Response: The response from the HTTP request.
     """
     # Build the request headers from the token and user agent
     request_headers = {
-        auth_header: token,
-        "User-Agent": compose_user_agent(caller_name, caller_version),
+        **{
+            auth_header: token,
+            "User-Agent": compose_user_agent(caller_name, caller_version),
+        },
+        **additional_headers,
     }
 
     # Log the parameters of the request accordingly
     log_request(method, f"{base_url}{path}", url_params, request_headers, json_data)
 
     # Make the request
     r = await client.request(
```

### Comparing `astrapy-1.1.0/astrapy/cursors.py` & `astrapy-1.2.0/astrapy/cursors.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,17 +565,17 @@
                 "skip": self._skip,
                 "includeSimilarity": self._include_similarity,
             }.items()
             if v is not None
         }
 
         # recast parameters for paginated_find call
-        pf_projection: Optional[Dict[str, bool]] = normalize_optional_projection(
-            self._projection
-        )
+        pf_projection: Optional[
+            Dict[str, Union[bool, Dict[str, Union[int, Iterable[int]]]]]
+        ] = normalize_optional_projection(self._projection)
         pf_sort: Optional[Dict[str, int]]
         if self._sort:
             pf_sort = dict(self._sort)
         else:
             pf_sort = None
 
         logger.info(f"creating iterator on '{self._collection.name}'")
@@ -773,17 +773,17 @@
                 "skip": self._skip,
                 "includeSimilarity": self._include_similarity,
             }.items()
             if v is not None
         }
 
         # recast parameters for paginated_find call
-        pf_projection: Optional[Dict[str, bool]] = normalize_optional_projection(
-            self._projection
-        )
+        pf_projection: Optional[
+            Dict[str, Union[bool, Dict[str, Union[int, Iterable[int]]]]]
+        ] = normalize_optional_projection(self._projection)
         pf_sort: Optional[Dict[str, int]]
         if self._sort:
             pf_sort = dict(self._sort)
         else:
             pf_sort = None
 
         logger.info(f"creating iterator on '{self._collection.name}'")
```

### Comparing `astrapy-1.1.0/astrapy/database.py` & `astrapy-1.2.0/astrapy/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import logging
 
 from types import TracebackType
 from typing import Any, Dict, List, Optional, Type, Union, TYPE_CHECKING
 
 from astrapy.core.db import AstraDB, AsyncAstraDB
+from astrapy.api_options import CollectionAPIOptions
 from astrapy.exceptions import (
     CollectionAlreadyExistsException,
     DataAPIFaultyResponseException,
     DevOpsAPIException,
     MultiCallTimeoutManager,
     recast_method_sync,
     recast_method_async,
@@ -31,19 +32,25 @@
 )
 from astrapy.cursors import AsyncCommandCursor, CommandCursor
 from astrapy.info import (
     DatabaseInfo,
     CollectionDescriptor,
     CollectionVectorServiceOptions,
 )
-from astrapy.admin import parse_api_endpoint, fetch_database_info
+from astrapy.constants import Environment
+from astrapy.admin import (
+    parse_api_endpoint,
+    fetch_database_info,
+    API_PATH_ENV_MAP,
+    API_VERSION_ENV_MAP,
+)
 
 if TYPE_CHECKING:
     from astrapy.collection import AsyncCollection, Collection
-    from astrapy.admin import AstraDBDatabaseAdmin
+    from astrapy.admin import DatabaseAdmin
 
 
 logger = logging.getLogger(__name__)
 
 
 def _validate_create_collection_options(
     dimension: Optional[int],
@@ -84,34 +91,40 @@
             "Cannot specify `metric` for non-vector collections in the "
             "create_collection method."
         )
 
 
 class Database:
     """
-    A Data API database. This is the entry-point object for doing database-level
+    A Data API database. This is the object for doing database-level
     DML, such as creating/deleting collections, and for obtaining Collection
     objects themselves. This class has a synchronous interface.
 
-    A Database comes with an "API Endpoint", which implies a Database object
-    instance reaches a specific region (relevant point in case of multi-region
-    databases).
+    The usual way of obtaining one Database is through the `get_database`
+    method of a `DataAPIClient`.
+
+    On Astra DB, a Database comes with an "API Endpoint", which implies
+    a Database object instance reaches a specific region (relevant point in
+    case of multi-region databases).
 
     Args:
         api_endpoint: the full "API Endpoint" string used to reach the Data API.
             Example: "https://<database_id>-<region>.apps.astra.datastax.com"
         token: an Access Token to the database. Example: "AstraCS:xyz..."
         namespace: this is the namespace all method calls will target, unless
             one is explicitly specified in the call. If no namespace is supplied
             when creating a Database, the name "default_namespace" is set.
         caller_name: name of the application, or framework, on behalf of which
             the Data API calls are performed. This ends up in the request user-agent.
         caller_version: version of the caller.
+        environment: a string representing the target Data API environment.
+            It can be left unspecified for the default value of `Environment.PROD`;
+            other values include `Environment.OTHER`, `Environment.DSE`.
         api_path: path to append to the API Endpoint. In typical usage, this
-            should be left to its default of "/api/json".
+            should be left to its default (sensibly chosen based on the environment).
         api_version: version specifier to append to the API path. In typical
             usage, this should be left to its default of "v1".
 
     Example:
         >>> from astrapy import DataAPIClient
         >>> my_client = astrapy.DataAPIClient("AstraCS:...")
         >>> my_db = my_client.get_database_by_api_endpoint(
@@ -128,22 +141,35 @@
         self,
         api_endpoint: str,
         token: str,
         *,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> None:
+        self.environment = (environment or Environment.PROD).lower()
+        #
+        _api_path: Optional[str]
+        _api_version: Optional[str]
+        if api_path is None:
+            _api_path = API_PATH_ENV_MAP.get(self.environment)
+        else:
+            _api_path = api_path
+        if api_version is None:
+            _api_version = API_VERSION_ENV_MAP.get(self.environment)
+        else:
+            _api_version = api_version
         self._astra_db = AstraDB(
             token=token,
             api_endpoint=api_endpoint,
-            api_path=api_path,
-            api_version=api_version,
+            api_path=_api_path,
+            api_version=_api_version,
             namespace=namespace,
             caller_name=caller_name,
             caller_version=caller_version,
         )
         self._name: Optional[str] = None
 
     def __getattr__(self, collection_name: str) -> Collection:
@@ -168,23 +194,25 @@
         self,
         *,
         api_endpoint: Optional[str] = None,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> Database:
         return Database(
             api_endpoint=api_endpoint or self._astra_db.api_endpoint,
             token=token or self._astra_db.token,
             namespace=namespace or self._astra_db.namespace,
             caller_name=caller_name or self._astra_db.caller_name,
             caller_version=caller_version or self._astra_db.caller_version,
+            environment=environment or self.environment,
             api_path=api_path or self._astra_db.api_path,
             api_version=api_version or self._astra_db.api_version,
         )
 
     def with_options(
         self,
         *,
@@ -224,14 +252,15 @@
         self,
         *,
         api_endpoint: Optional[str] = None,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> AsyncDatabase:
         """
         Create an AsyncDatabase from this one. Save for the arguments
         explicitly provided as overrides, everything else is kept identical
         to this database in the copy.
@@ -242,14 +271,17 @@
             token: an Access Token to the database. Example: "AstraCS:xyz..."
             namespace: this is the namespace all method calls will target, unless
                 one is explicitly specified in the call. If no namespace is supplied
                 when creating a Database, the name "default_namespace" is set.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
+            environment: a string representing the target Data API environment.
+                Values are, for example, `Environment.PROD`, `Environment.OTHER`,
+                or `Environment.DSE`.
             api_path: path to append to the API Endpoint. In typical usage, this
                 should be left to its default of "/api/json".
             api_version: version specifier to append to the API path. In typical
                 usage, this should be left to its default of "v1".
 
         Returns:
             the new copy, an `AsyncDatabase` instance.
@@ -261,14 +293,15 @@
 
         return AsyncDatabase(
             api_endpoint=api_endpoint or self._astra_db.api_endpoint,
             token=token or self._astra_db.token,
             namespace=namespace or self._astra_db.namespace,
             caller_name=caller_name or self._astra_db.caller_name,
             caller_version=caller_version or self._astra_db.caller_version,
+            environment=environment or self.environment,
             api_path=api_path or self._astra_db.api_path,
             api_version=api_version or self._astra_db.api_version,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
@@ -372,15 +405,20 @@
             >>> my_db.namespace
             'the_keyspace'
         """
 
         return self._astra_db.namespace
 
     def get_collection(
-        self, name: str, *, namespace: Optional[str] = None
+        self,
+        name: str,
+        *,
+        namespace: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
     ) -> Collection:
         """
         Spawn a `Collection` object instance representing a collection
         on this database.
 
         Creating a `Collection` instance does not have any effect on the
         actual state of the database: in other words, for the created
@@ -388,14 +426,26 @@
         must exist already (for instance, it should have been created
         previously by calling the `create_collection` method).
 
         Args:
             name: the name of the collection.
             namespace: the namespace containing the collection. If no namespace
                 is specified, the general setting for this database is used.
+        embedding_api_key: an optional API key for interacting with the collection.
+            If an embedding service is configured, and this attribute is set,
+            each Data API call will include a "x-embedding-api-key" header
+            with the value of this attribute.
+        collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+            operation on the collection. Individual timeouts can be provided to
+            each collection method call and will take precedence, with this value
+            being an overall default.
+            Note that for some methods involving multiple API calls (such as
+            `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+            to provide a specific timeout as the default one likely wouldn't make
+            much sense.
 
         Returns:
             a `Collection` instance, representing the desired collection
                 (but without any form of validation).
 
         Example:
             >>> my_col = my_db.get_collection("my_collection")
@@ -410,15 +460,23 @@
                 my_db["coll_name"]
         """
 
         # lazy importing here against circular-import error
         from astrapy.collection import Collection
 
         _namespace = namespace or self._astra_db.namespace
-        return Collection(self, name, namespace=_namespace)
+        return Collection(
+            self,
+            name,
+            namespace=_namespace,
+            api_options=CollectionAPIOptions(
+                embedding_api_key=embedding_api_key,
+                max_time_ms=collection_max_time_ms,
+            ),
+        )
 
     @recast_method_sync
     def create_collection(
         self,
         name: str,
         *,
         namespace: Optional[str] = None,
@@ -426,14 +484,16 @@
         metric: Optional[str] = None,
         service: Optional[Union[CollectionVectorServiceOptions, Dict[str, Any]]] = None,
         indexing: Optional[Dict[str, Any]] = None,
         default_id_type: Optional[str] = None,
         additional_options: Optional[Dict[str, Any]] = None,
         check_exists: Optional[bool] = None,
         max_time_ms: Optional[int] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
     ) -> Collection:
         """
         Creates a collection on the database and return the Collection
         instance that represents it.
 
         This is a blocking operation: the method returns when the collection
         is ready to be used. As opposed to the `get_collection` instance,
@@ -447,15 +507,14 @@
                 (i.e. the number of their components).
             metric: the similarity metric used for vector searches.
                 Allowed values are `VectorMetric.DOT_PRODUCT`, `VectorMetric.EUCLIDEAN`
                 or `VectorMetric.COSINE` (default).
             service: a dictionary describing a service for
                 embedding computation, e.g. `{"provider": "ab", "modelName": "xy"}`.
                 Alternatively, a CollectionVectorServiceOptions object to the same effect.
-                NOTE: This feature is under current development.
             indexing: optional specification of the indexing options for
                 the collection, in the form of a dictionary such as
                     {"deny": [...]}
                 or
                     {"allow": [...]}
             default_id_type: this sets what type of IDs the API server will
                 generate when inserting documents that do not specify their
@@ -470,14 +529,26 @@
                 name before attempting to create the collection:
                 If check_exists is True, an error is raised when creating
                 an existing collection.
                 If it is False, the creation is attempted. In this case, for
                 preexisting collections, the command will succeed or fail
                 depending on whether the options match or not.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
 
         Returns:
             a (synchronous) `Collection` instance, representing the
             newly-created collection.
 
         Example:
             >>> new_col = my_db.create_collection("my_v_col", dimension=3)
@@ -542,15 +613,20 @@
             options=_options,
             dimension=dimension,
             metric=metric,
             service_dict=service_dict,
             timeout_info=timeout_manager.remaining_timeout_info(),
         )
         logger.info(f"finished creating collection '{name}'")
-        return self.get_collection(name, namespace=namespace)
+        return self.get_collection(
+            name,
+            namespace=namespace,
+            embedding_api_key=embedding_api_key,
+            collection_max_time_ms=collection_max_time_ms,
+        )
 
     @recast_method_sync
     def drop_collection(
         self,
         name_or_collection: Union[str, Collection],
         *,
         max_time_ms: Optional[int] = None,
@@ -751,76 +827,108 @@
 
     def get_database_admin(
         self,
         *,
         token: Optional[str] = None,
         dev_ops_url: Optional[str] = None,
         dev_ops_api_version: Optional[str] = None,
-    ) -> AstraDBDatabaseAdmin:
+    ) -> DatabaseAdmin:
         """
-        Return an AstraDBDatabaseAdmin object corresponding to this database, for
+        Return a DatabaseAdmin object corresponding to this database, for
         use in admin tasks such as managing namespaces.
 
+        This method, depending on the environment where the database resides,
+        returns an appropriate subclass of DatabaseAdmin.
+
         Args:
             token: an access token with enough permission on the database to
                 perform the desired tasks. If omitted (as it can generally be done),
                 the token of this Database is used.
             dev_ops_url: in case of custom deployments, this can be used to specify
                 the URL to the DevOps API, such as "https://api.astra.datastax.com".
                 Generally it can be omitted. The environment (prod/dev/...) is
                 determined from the API Endpoint.
+                Note that this parameter is allowed only for Astra DB environments.
             dev_ops_api_version: this can specify a custom version of the DevOps API
                 (such as "v2"). Generally not needed.
+                Note that this parameter is allowed only for Astra DB environments.
 
         Returns:
-            An AstraDBDatabaseAdmin instance targeting this database.
+            A DatabaseAdmin instance targeting this database. More precisely,
+            for Astra DB an instance of `AstraDBDatabaseAdmin` is returned;
+            for other environments, an instance of `DataAPIDatabaseAdmin` is returned.
 
         Example:
             >>> my_db_admin = my_db.get_database_admin()
             >>> if "new_namespace" not in my_db_admin.list_namespaces():
             ...     my_db_admin.create_namespace("new_namespace")
             >>> my_db_admin.list_namespaces()
             ['default_keyspace', 'new_namespace']
         """
 
         # lazy importing here to avoid circular dependency
-        from astrapy.admin import AstraDBDatabaseAdmin
+        from astrapy.admin import AstraDBDatabaseAdmin, DataAPIDatabaseAdmin
 
-        return AstraDBDatabaseAdmin.from_api_endpoint(
-            api_endpoint=self._astra_db.api_endpoint,
-            token=token or self._astra_db.token,
-            caller_name=self._astra_db.caller_name,
-            caller_version=self._astra_db.caller_version,
-            dev_ops_url=dev_ops_url,
-            dev_ops_api_version=dev_ops_api_version,
-        )
+        if self.environment in Environment.astra_db_values:
+            return AstraDBDatabaseAdmin.from_api_endpoint(
+                api_endpoint=self._astra_db.api_endpoint,
+                token=token or self._astra_db.token,
+                caller_name=self._astra_db.caller_name,
+                caller_version=self._astra_db.caller_version,
+                dev_ops_url=dev_ops_url,
+                dev_ops_api_version=dev_ops_api_version,
+            )
+        else:
+            if dev_ops_url is not None:
+                raise ValueError(
+                    "Parameter `dev_ops_url` not supported outside of Astra DB."
+                )
+            if dev_ops_api_version is not None:
+                raise ValueError(
+                    "Parameter `dev_ops_api_version` not supported outside of Astra DB."
+                )
+            return DataAPIDatabaseAdmin(
+                api_endpoint=self._astra_db.api_endpoint,
+                token=token or self._astra_db.token,
+                environment=self.environment,
+                api_path=self._astra_db.api_path,
+                api_version=self._astra_db.api_version,
+                caller_name=self._astra_db.caller_name,
+                caller_version=self._astra_db.caller_version,
+            )
 
 
 class AsyncDatabase:
     """
-    A Data API database. This is the entry-point object for doing database-level
+    A Data API database. This is the object for doing database-level
     DML, such as creating/deleting collections, and for obtaining Collection
     objects themselves. This class has an asynchronous interface.
 
-    A Database comes with an "API Endpoint", which implies a Database object
-    instance reaches a specific region (relevant point in case of multi-region
-    databases).
+    The usual way of obtaining one AsyncDatabase is through the `get_async_database`
+    method of a `DataAPIClient`.
+
+    On Astra DB, an AsyncDatabase comes with an "API Endpoint", which implies
+    an AsyncDatabase object instance reaches a specific region (relevant point in
+    case of multi-region databases).
 
     Args:
         api_endpoint: the full "API Endpoint" string used to reach the Data API.
             Example: "https://<database_id>-<region>.apps.astra.datastax.com"
         token: an Access Token to the database. Example: "AstraCS:xyz..."
         namespace: this is the namespace all method calls will target, unless
             one is explicitly specified in the call. If no namespace is supplied
             when creating a Database, the name "default_namespace" is set.
         caller_name: name of the application, or framework, on behalf of which
             the Data API calls are performed. This ends up in the request user-agent.
         caller_version: version of the caller.
+        environment: a string representing the target Data API environment.
+            It can be left unspecified for the default value of `Environment.PROD`;
+            other values include `Environment.OTHER`, `Environment.DSE`.
         api_path: path to append to the API Endpoint. In typical usage, this
-            should be left to its default of "/api/json".
+            should be left to its default (sensibly chosen based on the environment).
         api_version: version specifier to append to the API path. In typical
             usage, this should be left to its default of "v1".
 
     Example:
         >>> from astrapy import DataAPIClient
         >>> my_client = astrapy.DataAPIClient("AstraCS:...")
         >>> my_db = my_client.get_async_database_by_api_endpoint(
@@ -837,22 +945,36 @@
         self,
         api_endpoint: str,
         token: str,
         *,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> None:
+        self.environment = (environment or Environment.PROD).lower()
+        #
+        _api_path: Optional[str]
+        _api_version: Optional[str]
+        if api_path is None:
+            _api_path = API_PATH_ENV_MAP.get(self.environment)
+        else:
+            _api_path = api_path
+        if api_version is None:
+            _api_version = API_VERSION_ENV_MAP.get(self.environment)
+        else:
+            _api_version = api_version
+        #
         self._astra_db = AsyncAstraDB(
             token=token,
             api_endpoint=api_endpoint,
-            api_path=api_path,
-            api_version=api_version,
+            api_path=_api_path,
+            api_version=_api_version,
             namespace=namespace,
             caller_name=caller_name,
             caller_version=caller_version,
         )
         self._name: Optional[str] = None
 
     def __getattr__(self, collection_name: str) -> AsyncCollection:
@@ -892,23 +1014,25 @@
         self,
         *,
         api_endpoint: Optional[str] = None,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> AsyncDatabase:
         return AsyncDatabase(
             api_endpoint=api_endpoint or self._astra_db.api_endpoint,
             token=token or self._astra_db.token,
             namespace=namespace or self._astra_db.namespace,
             caller_name=caller_name or self._astra_db.caller_name,
             caller_version=caller_version or self._astra_db.caller_version,
+            environment=environment or self.environment,
             api_path=api_path or self._astra_db.api_path,
             api_version=api_version or self._astra_db.api_version,
         )
 
     def with_options(
         self,
         *,
@@ -948,14 +1072,15 @@
         self,
         *,
         api_endpoint: Optional[str] = None,
         token: Optional[str] = None,
         namespace: Optional[str] = None,
         caller_name: Optional[str] = None,
         caller_version: Optional[str] = None,
+        environment: Optional[str] = None,
         api_path: Optional[str] = None,
         api_version: Optional[str] = None,
     ) -> Database:
         """
         Create a (synchronous) Database from this one. Save for the arguments
         explicitly provided as overrides, everything else is kept identical
         to this database in the copy.
@@ -966,14 +1091,17 @@
             token: an Access Token to the database. Example: "AstraCS:xyz..."
             namespace: this is the namespace all method calls will target, unless
                 one is explicitly specified in the call. If no namespace is supplied
                 when creating a Database, the name "default_namespace" is set.
             caller_name: name of the application, or framework, on behalf of which
                 the Data API calls are performed. This ends up in the request user-agent.
             caller_version: version of the caller.
+            environment: a string representing the target Data API environment.
+                Values are, for example, `Environment.PROD`, `Environment.OTHER`,
+                or `Environment.DSE`.
             api_path: path to append to the API Endpoint. In typical usage, this
                 should be left to its default of "/api/json".
             api_version: version specifier to append to the API path. In typical
                 usage, this should be left to its default of "v1".
 
         Returns:
             the new copy, a `Database` instance.
@@ -986,14 +1114,15 @@
 
         return Database(
             api_endpoint=api_endpoint or self._astra_db.api_endpoint,
             token=token or self._astra_db.token,
             namespace=namespace or self._astra_db.namespace,
             caller_name=caller_name or self._astra_db.caller_name,
             caller_version=caller_version or self._astra_db.caller_version,
+            environment=environment or self.environment,
             api_path=api_path or self._astra_db.api_path,
             api_version=api_version or self._astra_db.api_version,
         )
 
     def set_caller(
         self,
         caller_name: Optional[str] = None,
@@ -1097,15 +1226,20 @@
             >>> my_async_db.namespace
             'the_keyspace'
         """
 
         return self._astra_db.namespace
 
     async def get_collection(
-        self, name: str, *, namespace: Optional[str] = None
+        self,
+        name: str,
+        *,
+        namespace: Optional[str] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
     ) -> AsyncCollection:
         """
         Spawn an `AsyncCollection` object instance representing a collection
         on this database.
 
         Creating an `AsyncCollection` instance does not have any effect on the
         actual state of the database: in other words, for the created
@@ -1113,14 +1247,26 @@
         must exist already (for instance, it should have been created
         previously by calling the `create_collection` method).
 
         Args:
             name: the name of the collection.
             namespace: the namespace containing the collection. If no namespace
                 is specified, the setting for this database is used.
+        embedding_api_key: an optional API key for interacting with the collection.
+            If an embedding service is configured, and this attribute is set,
+            each Data API call will include a "x-embedding-api-key" header
+            with the value of this attribute.
+        collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+            operation on the collection. Individual timeouts can be provided to
+            each collection method call and will take precedence, with this value
+            being an overall default.
+            Note that for some methods involving multiple API calls (such as
+            `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+            to provide a specific timeout as the default one likely wouldn't make
+            much sense.
 
         Returns:
             an `AsyncCollection` instance, representing the desired collection
                 (but without any form of validation).
 
         Example:
             >>> async def count_docs(adb: AsyncDatabase, c_name: str) -> int:
@@ -1138,15 +1284,23 @@
                 my_async_db["coll_name"]
         """
 
         # lazy importing here against circular-import error
         from astrapy.collection import AsyncCollection
 
         _namespace = namespace or self._astra_db.namespace
-        return AsyncCollection(self, name, namespace=_namespace)
+        return AsyncCollection(
+            self,
+            name,
+            namespace=_namespace,
+            api_options=CollectionAPIOptions(
+                embedding_api_key=embedding_api_key,
+                max_time_ms=collection_max_time_ms,
+            ),
+        )
 
     @recast_method_async
     async def create_collection(
         self,
         name: str,
         *,
         namespace: Optional[str] = None,
@@ -1154,14 +1308,16 @@
         metric: Optional[str] = None,
         service: Optional[Union[CollectionVectorServiceOptions, Dict[str, Any]]] = None,
         indexing: Optional[Dict[str, Any]] = None,
         default_id_type: Optional[str] = None,
         additional_options: Optional[Dict[str, Any]] = None,
         check_exists: Optional[bool] = None,
         max_time_ms: Optional[int] = None,
+        embedding_api_key: Optional[str] = None,
+        collection_max_time_ms: Optional[int] = None,
     ) -> AsyncCollection:
         """
         Creates a collection on the database and return the AsyncCollection
         instance that represents it.
 
         This is a blocking operation: the method returns when the collection
         is ready to be used. As opposed to the `get_collection` instance,
@@ -1175,15 +1331,14 @@
                 (i.e. the number of their components).
             metric: the similarity metric used for vector searches.
                 Allowed values are `VectorMetric.DOT_PRODUCT`, `VectorMetric.EUCLIDEAN`
                 or `VectorMetric.COSINE` (default).
             service: a dictionary describing a service for
                 embedding computation, e.g. `{"provider": "ab", "modelName": "xy"}`.
                 Alternatively, a CollectionVectorServiceOptions object to the same effect.
-                NOTE: This feature is under current development.
             indexing: optional specification of the indexing options for
                 the collection, in the form of a dictionary such as
                     {"deny": [...]}
                 or
                     {"allow": [...]}
             default_id_type: this sets what type of IDs the API server will
                 generate when inserting documents that do not specify their
@@ -1198,14 +1353,26 @@
                 name before attempting to create the collection:
                 If check_exists is True, an error is raised when creating
                 an existing collection.
                 If it is False, the creation is attempted. In this case, for
                 preexisting collections, the command will succeed or fail
                 depending on whether the options match or not.
             max_time_ms: a timeout, in milliseconds, for the underlying HTTP request.
+            embedding_api_key: an optional API key for interacting with the collection.
+                If an embedding service is configured, and this attribute is set,
+                each Data API call will include a "x-embedding-api-key" header
+                with the value of this attribute.
+            collection_max_time_ms: a default timeout, in millisecond, for the duration of each
+                operation on the collection. Individual timeouts can be provided to
+                each collection method call and will take precedence, with this value
+                being an overall default.
+                Note that for some methods involving multiple API calls (such as
+                `find`, `delete_many`, `insert_many` and so on), it is strongly suggested
+                to provide a specific timeout as the default one likely wouldn't make
+                much sense.
 
         Returns:
             an `AsyncCollection` instance, representing the newly-created collection.
 
         Example:
             >>> async def create_and_insert(adb: AsyncDatabase) -> Dict[str, Any]:
             ...     new_a_col = await adb.create_collection("my_v_col", dimension=3)
@@ -1274,15 +1441,20 @@
             options=_options,
             dimension=dimension,
             metric=metric,
             service_dict=service_dict,
             timeout_info=timeout_manager.remaining_timeout_info(),
         )
         logger.info(f"finished creating collection '{name}'")
-        return await self.get_collection(name, namespace=namespace)
+        return await self.get_collection(
+            name,
+            namespace=namespace,
+            embedding_api_key=embedding_api_key,
+            collection_max_time_ms=collection_max_time_ms,
+        )
 
     @recast_method_async
     async def drop_collection(
         self,
         name_or_collection: Union[str, AsyncCollection],
         *,
         max_time_ms: Optional[int] = None,
@@ -1492,45 +1664,71 @@
 
     def get_database_admin(
         self,
         *,
         token: Optional[str] = None,
         dev_ops_url: Optional[str] = None,
         dev_ops_api_version: Optional[str] = None,
-    ) -> AstraDBDatabaseAdmin:
+    ) -> DatabaseAdmin:
         """
-        Return an AstraDBDatabaseAdmin object corresponding to this database, for
+        Return a DatabaseAdmin object corresponding to this database, for
         use in admin tasks such as managing namespaces.
 
+        This method, depending on the environment where the database resides,
+        returns an appropriate subclass of DatabaseAdmin.
+
         Args:
             token: an access token with enough permission on the database to
                 perform the desired tasks. If omitted (as it can generally be done),
                 the token of this Database is used.
             dev_ops_url: in case of custom deployments, this can be used to specify
                 the URL to the DevOps API, such as "https://api.astra.datastax.com".
                 Generally it can be omitted. The environment (prod/dev/...) is
                 determined from the API Endpoint.
+                Note that this parameter is allowed only for Astra DB environments.
             dev_ops_api_version: this can specify a custom version of the DevOps API
                 (such as "v2"). Generally not needed.
+                Note that this parameter is allowed only for Astra DB environments.
 
         Returns:
-            An AstraDBDatabaseAdmin instance targeting this database.
+            A DatabaseAdmin instance targeting this database. More precisely,
+            for Astra DB an instance of `AstraDBDatabaseAdmin` is returned;
+            for other environments, an instance of `DataAPIDatabaseAdmin` is returned.
 
         Example:
             >>> my_db_admin = my_async_db.get_database_admin()
             >>> if "new_namespace" not in my_db_admin.list_namespaces():
             ...     my_db_admin.create_namespace("new_namespace")
             >>> my_db_admin.list_namespaces()
             ['default_keyspace', 'new_namespace']
         """
 
         # lazy importing here to avoid circular dependency
-        from astrapy.admin import AstraDBDatabaseAdmin
+        from astrapy.admin import AstraDBDatabaseAdmin, DataAPIDatabaseAdmin
 
-        return AstraDBDatabaseAdmin.from_api_endpoint(
-            api_endpoint=self._astra_db.api_endpoint,
-            token=token or self._astra_db.token,
-            caller_name=self._astra_db.caller_name,
-            caller_version=self._astra_db.caller_version,
-            dev_ops_url=dev_ops_url,
-            dev_ops_api_version=dev_ops_api_version,
-        )
+        if self.environment in Environment.astra_db_values:
+            return AstraDBDatabaseAdmin.from_api_endpoint(
+                api_endpoint=self._astra_db.api_endpoint,
+                token=token or self._astra_db.token,
+                caller_name=self._astra_db.caller_name,
+                caller_version=self._astra_db.caller_version,
+                dev_ops_url=dev_ops_url,
+                dev_ops_api_version=dev_ops_api_version,
+            )
+        else:
+            if dev_ops_url is not None:
+                raise ValueError(
+                    "Parameter `dev_ops_url` not supported outside of Astra DB."
+                )
+            if dev_ops_api_version is not None:
+                raise ValueError(
+                    "Parameter `dev_ops_api_version` not supported outside of Astra DB."
+                )
+            return DataAPIDatabaseAdmin(
+                api_endpoint=self._astra_db.api_endpoint,
+                token=token or self._astra_db.token,
+                environment=self.environment,
+                api_path=self._astra_db.api_path,
+                api_version=self._astra_db.api_version,
+                caller_name=self._astra_db.caller_name,
+                caller_version=self._astra_db.caller_version,
+            )
```

### Comparing `astrapy-1.1.0/astrapy/db/__init__.py` & `astrapy-1.2.0/astrapy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/exceptions.py` & `astrapy-1.2.0/astrapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/ids.py` & `astrapy-1.2.0/astrapy/ids.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/info.py` & `astrapy-1.2.0/astrapy/info.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
     Attributes:
         id: the database ID.
         region: the ID of the region through which the connection to DB is done.
         namespace: the namespace this DB is set to work with.
         name: the database name. Not necessarily unique: there can be multiple
             databases with the same name.
-        environment: a label, whose value is one of Environment.PROD, Environment.DEV
-            or Environment.TEST.
+        environment: a label, whose value can be `Environment.PROD`,
+            or another value in `Environment.*`.
         raw_info: the full response from the DevOPS API call to get this info.
 
     Note:
         The `raw_info` dictionary usually has a `region` key describing
         the default region as configured in the database, which does not
         necessarily (for multi-region databases) match the region through
         which the connection is established: the latter is the one specified
@@ -162,32 +162,38 @@
 
 @dataclass
 class CollectionVectorServiceOptions:
     """
     The "vector.service" component of the collection options.
     See the Data API specifications for allowed values.
 
-    NOTE: This feature is under current development.
-
     Attributes:
         provider: the name of a service provider for embedding calculation.
         model_name: the name of a specific model for use by the service.
+        authentication: a key-value dictionary for the "authentication" specification,
+            if any, in the vector service options.
+        parameters: a key-value dictionary for the "parameters" specification, if any,
+            in the vector service options.
     """
 
     provider: Optional[str]
     model_name: Optional[str]
+    authentication: Optional[Dict[str, Any]] = None
+    parameters: Optional[Dict[str, Any]] = None
 
     def as_dict(self) -> Dict[str, Any]:
         """Recast this object into a dictionary."""
 
         return {
             k: v
             for k, v in {
                 "provider": self.provider,
                 "modelName": self.model_name,
+                "authentication": self.authentication,
+                "parameters": self.parameters,
             }.items()
             if v is not None
         }
 
     @staticmethod
     def from_dict(
         raw_dict: Optional[Dict[str, Any]]
@@ -197,14 +203,16 @@
         such as one from the Data API.
         """
 
         if raw_dict is not None:
             return CollectionVectorServiceOptions(
                 provider=raw_dict.get("provider"),
                 model_name=raw_dict.get("modelName"),
+                authentication=raw_dict.get("authentication"),
+                parameters=raw_dict.get("parameters"),
             )
         else:
             return None
 
 
 @dataclass
 class CollectionVectorOptions:
@@ -212,16 +220,16 @@
     The "vector" component of the collection options.
     See the Data API specifications for allowed values.
 
     Attributes:
         dimension: an optional positive integer, the dimensionality of the vector space.
         metric: an optional metric among `VectorMetric.DOT_PRODUCT`,
             `VectorMetric.EUCLIDEAN` and `VectorMetric.COSINE`.
-        service: an optional X object in case a service is configured for the collection.
-            NOTE: This feature is under current development.
+        service: an optional CollectionVectorServiceOptions object in case a
+            service is configured for the collection.
     """
 
     dimension: Optional[int]
     metric: Optional[str]
     service: Optional[CollectionVectorServiceOptions]
 
     def as_dict(self) -> Dict[str, Any]:
```

### Comparing `astrapy-1.1.0/astrapy/operations.py` & `astrapy-1.2.0/astrapy/operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 
     Attributes:
         document: the document to insert.
         vector: an optional suitable vector to enrich the document at insertion.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
     """
 
     document: DocumentType
     vector: Optional[VectorType]
     vectorize: Optional[str]
 
     def __init__(
@@ -148,15 +147,14 @@
     See the documentation on the collection method for more information.
 
     Attributes:
         documents: the list document to insert.
         vectors: an optional list of vectors to enrich the documents at insertion.
         vectorize: an optional list of texts achieving the same effect as `vectors`
             except through an embedding service, if one is configured for the collection.
-            NOTE: This feature is under current development.
         ordered: whether the inserts should be done in sequence.
         chunk_size: how many documents to include in a single API request.
             Exceeding the server maximum allowed value results in an error.
             Leave it unspecified (recommended) to use the system default.
         concurrency: maximum number of concurrent requests to the API at
             a given time. It cannot be more than one for ordered insertions.
     """
@@ -220,15 +218,14 @@
     Attributes:
         filter: a filter condition to select a target document.
         update: an update prescription to apply to the document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
         upsert: controls what to do when no documents are found.
     """
 
     filter: Dict[str, Any]
     update: Dict[str, Any]
     vector: Optional[VectorType]
@@ -338,15 +335,14 @@
     Attributes:
         filter: a filter condition to select a target document.
         replacement: the replacement document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
         upsert: controls what to do when no documents are found.
     """
 
     filter: Dict[str, Any]
     replacement: DocumentType
     vector: Optional[VectorType]
@@ -405,15 +401,14 @@
 
     Attributes:
         filter: a filter condition to select a target document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
     """
 
     filter: Dict[str, Any]
     vector: Optional[VectorType]
     vectorize: Optional[str]
     sort: Optional[SortType]
@@ -516,15 +511,14 @@
 
     Attributes:
         document: the document to insert.
         vector: an optional suitable vector to enrich the document at insertion.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
     """
 
     document: DocumentType
     vector: Optional[VectorType]
     vectorize: Optional[str]
 
     def __init__(
@@ -568,15 +562,14 @@
     See the documentation on the collection method for more information.
 
     Attributes:
         documents: the list document to insert.
         vectors: an optional list of vectors to enrich the documents at insertion.
         vectorize: an optional list of texts achieving the same effect as `vectors`
             except through an embedding service, if one is configured for the collection.
-            NOTE: This feature is under current development.
         ordered: whether the inserts should be done in sequence.
         chunk_size: how many documents to include in a single API request.
             Exceeding the server maximum allowed value results in an error.
             Leave it unspecified (recommended) to use the system default.
         concurrency: maximum number of concurrent requests to the API at
             a given time. It cannot be more than one for ordered insertions.
     """
@@ -640,15 +633,14 @@
     Attributes:
         filter: a filter condition to select a target document.
         update: an update prescription to apply to the document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
         upsert: controls what to do when no documents are found.
     """
 
     filter: Dict[str, Any]
     update: Dict[str, Any]
     vector: Optional[VectorType]
@@ -758,15 +750,14 @@
     Attributes:
         filter: a filter condition to select a target document.
         replacement: the replacement document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
         upsert: controls what to do when no documents are found.
     """
 
     filter: Dict[str, Any]
     replacement: DocumentType
     vector: Optional[VectorType]
@@ -825,15 +816,14 @@
 
     Attributes:
         filter: a filter condition to select a target document.
         vector: a vector of numbers to use for ANN (vector-search) sorting.
         vectorize: a string to be made into a vector, with the same result as the
             `vector` attribute, through an embedding service, assuming one is
             configured for the collection.
-            NOTE: This feature is under current development.
         sort: controls ordering of results, hence which document is affected.
     """
 
     filter: Dict[str, Any]
     vector: Optional[VectorType]
     vectorize: Optional[str]
     sort: Optional[SortType]
```

### Comparing `astrapy-1.1.0/astrapy/ops/__init__.py` & `astrapy-1.2.0/astrapy/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/astrapy/results.py` & `astrapy-1.2.0/astrapy/results.py`

 * *Files identical despite different names*

### Comparing `astrapy-1.1.0/pyproject.toml` & `astrapy-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "astrapy"
-version = "1.1.0"
+version = "1.2.0"
 description = "AstraPy is a Pythonic SDK for DataStax Astra and its Data API"
 authors = [
     "Stefano Lottini <stefano.lottini@datastax.com>",
     "Eric Hare <eric.hare@datastax.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `astrapy-1.1.0/PKG-INFO` & `astrapy-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrapy
-Version: 1.1.0
+Version: 1.2.0
 Summary: AstraPy is a Pythonic SDK for DataStax Astra and its Data API
 Home-page: https://github.com/datastax/astrapy
 License: Apache-2.0
 Keywords: DataStax,Astra
 Author: Stefano Lottini
 Author-email: stefano.lottini@datastax.com
 Requires-Python: >=3.8.0,<4.0.0
```

