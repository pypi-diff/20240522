# Comparing `tmp/smartlink-local-0.0.8.tar.gz` & `tmp/smartlink-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartlink-local-0.0.8.tar", last modified: Sun Jan  7 10:04:07 2024, max compression
+gzip compressed data, was "smartlink-local-0.0.9.tar", last modified: Mon Jan  8 04:53:33 2024, max compression
```

## Comparing `smartlink-local-0.0.8.tar` & `smartlink-local-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/smartlink_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-07 10:04:07.000000 smartlink-local-0.0.8/smartlink_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-07 10:04:07.000000 smartlink-local-0.0.8/smartlink_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 10:04:07.000000 smartlink-local-0.0.8/smartlink_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-07 10:04:07.000000 smartlink-local-0.0.8/smartlink_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-07 10:04:07.000000 smartlink-local-0.0.8/smartlink_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/src/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/src/smartlink.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:04:07.524066 smartlink-local-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-07 10:03:31.000000 smartlink-local-0.0.8/tests/test_smart_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:53:33.984648 smartlink-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-08 04:53:33.984648 smartlink-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 04:53:33.984648 smartlink-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:53:33.984648 smartlink-local-0.0.9/smartlink_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-01-08 04:53:33.000000 smartlink-local-0.0.9/smartlink_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-01-08 04:53:33.000000 smartlink-local-0.0.9/smartlink_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 04:53:33.000000 smartlink-local-0.0.9/smartlink_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-08 04:53:33.000000 smartlink-local-0.0.9/smartlink_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-08 04:53:33.000000 smartlink-local-0.0.9/smartlink_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:53:33.980648 smartlink-local-0.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/src/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/src/smartlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 04:53:33.980648 smartlink-local-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-01-08 04:52:55.000000 smartlink-local-0.0.9/tests/test_smart_link.py
```

### Comparing `smartlink-local-0.0.8/PKG-INFO` & `smartlink-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlink-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles smart link Python
 Home-page: https://github.com/circles-zone/smartlink-restapi-python-serverless-com
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `smartlink-local-0.0.8/pyproject.toml` & `smartlink-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartlink-local-0.0.8/setup.py` & `smartlink-local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "smartlink-local"
 package_name_to_import = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles smart link Python",
     long_description="PyPI Package for Circles smart link Python",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/smartlink-restapi-python-serverless-com",
     packages=[package_name_to_import],
```

### Comparing `smartlink-local-0.0.8/smartlink_local.egg-info/PKG-INFO` & `smartlink-local-0.0.9/smartlink_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartlink-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles smart link Python
 Home-page: https://github.com/circles-zone/smartlink-restapi-python-serverless-com
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `smartlink-local-0.0.8/src/handler.py` & `smartlink-local-0.0.9/src/handler.py`

 * *Files identical despite different names*

### Comparing `smartlink-local-0.0.8/src/smartlink.py` & `smartlink-local-0.0.9/src/smartlink.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # from circles_local_database_python.generic_crud import GenericCRUD
 from logger_local.Logger import Logger
 from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from message_local.Recipient import Recipient
 from queue_worker_local.queue_worker import QueueWorker
 from user_context_remote.user_context import UserContext
+# from email_address_local.email_address import EmailAddressesLocal
 
 from .utils import generate_random_string
 
 SMARTLINK_COMPONENT_ID = 258
 SMARTLINK_COMPONENT_NAME = "smartlink"
 DEVELOPER_EMAIL = "akiva.s@circ.zone"
 logger_object = {
@@ -24,22 +25,18 @@
 VERIFY_EMAIL_ADDRESS_ACTION_ID = 17
 SMARTLINK_ENTITY_TYPE_ID = 18
 
 
 class SmartLinkLocal(QueueWorker):
     def __init__(self) -> None:
         # QueueWorker is a subclass of GenericCRUD.
-        # GenericCRUD.__init__(self, default_schema_name="smartlink",
-        #                      default_table_name="smartlink_table",
-        #                      default_view_table_name="smartlink_view",
-        #                      default_id_column_name="magic_link_id")
         QueueWorker.__init__(self, schema_name="smartlink", table_name="smartlink_table",
                              id_column_name="smartlink_id", view_name="smartlink_view",
                              action_boolean_column="is_smartlink_action")
-        self.user = UserContext().login_using_user_identification_and_password()
+        self.user = UserContext()
 
     # We use primitive types for parameters and return value because we want to be able to call this function from srvls
     def insert(self, smartlink_type_id: int, campaign_id: int,
                from_recipient: dict = None, to_recipient: dict = None) -> int:
         # TODO should have an expiration parameter with a default of 7 days in case of email invitation,
         #  a few hours for sending pin code
         # TODO add support of multiple criteria per campaign
@@ -89,15 +86,14 @@
 
     # REST API GET request with GET parameter id=GsMgEP7rQJWRZUNWV4ES which executes a function based on action_id
     # from action_table with all fields that are not null in starlink_table (similar to queue worker but sync)
     # and get back from the action json with return-code, redirection url, stdout, stderr...
     # call api_management.incoming_api() which will call api_call.insert()
 
     def execute(self, smartlink_identifier: str) -> str | None:
-        # TODO: test
         session_id = generate_random_string(length=32)
         logger.start(object={"session_id": session_id,
                              "smartlink_identifier": smartlink_identifier})
         results = self.select_one_dict_by_id(id_column_name="smartlink_identifier",
                                              id_column_value=smartlink_identifier)
         if not results:
             logger.error(message=f"smartlink_id {smartlink_identifier} not found",
@@ -117,14 +113,15 @@
             "action_id": results["action_id"],
             "smartlink_id": smartlink_identifier,
             "function_parameters_json": json.dumps(
                 action_to_parameters[results["action_id"]]["function_parameters_json"]),
             "class_parameters_json": json.dumps(
                 action_to_parameters[results["action_id"]]["class_parameters_json"]),
             "session_id": session_id,
+            # "user_jwt": self.user.get_user_jwt(),
         }
         # TODO: save redirection url (how?)
         # AWS Lambda environment is read-only, so we can't install packages.
         super().execute(execution_details=execution_details, install_packages=False,
                         working_directory=None)
 
         logger.end(object={"session_id": session_id, "execution_details": execution_details})
```

### Comparing `smartlink-local-0.0.8/tests/test_smart_link.py` & `smartlink-local-0.0.9/tests/test_smart_link.py`

 * *Files identical despite different names*

