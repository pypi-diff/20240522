# Comparing `tmp/brainchain-0.6.6.tar.gz` & `tmp/brainchain-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.6.6.tar", max compression
+gzip compressed data, was "brainchain-0.6.7.tar", max compression
```

## Comparing `brainchain-0.6.6.tar` & `brainchain-0.6.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.6/brainchain/README.md
--rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.6/brainchain/__init__.py
--rw-r--r--   0        0        0    13624 2024-05-07 16:51:46.070229 brainchain-0.6.6/brainchain/assistants.py
--rw-r--r--   0        0        0    11851 2024-05-10 18:23:33.058953 brainchain-0.6.6/brainchain/brainchain.py
--rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.6/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.6/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.6/brainchain/embeddings.py
--rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.6.6/brainchain/graph/base.py
--rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.6/brainchain/graph/schema.py
--rw-r--r--   0        0        0     3426 2024-05-07 16:51:46.072116 brainchain-0.6.6/brainchain/logger.py
--rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.6/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.6/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.6/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.6/brainchain/search_v2.py
--rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.6/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.6/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.6/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.6/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.6/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.6/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.6/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.6/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.6/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    21273 2024-05-07 16:51:46.073960 brainchain-0.6.6/brainchain/tools/tools.py
--rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.6/brainchain/tools/web.py
--rw-r--r--   0        0        0      731 2024-04-23 19:21:58.552351 brainchain-0.6.6/brainchain/tools.py
--rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.6/brainchain/webapp/__init__.py
--rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.6/brainchain/webapp/agents.py
--rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.6/brainchain/webapp/base.py
--rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.6/brainchain/webapp/business_ideas.py
--rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.6/brainchain/webapp/contents.py
--rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.6/brainchain/webapp/conversations.py
--rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.6/brainchain/webapp/embedding_models.py
--rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.6/brainchain/webapp/embeddings.py
--rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.6/brainchain/webapp/files.py
--rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.6/brainchain/webapp/health.py
--rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.6/brainchain/webapp/language_models.py
--rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.6/brainchain/webapp/laws.py
--rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.6/brainchain/webapp/messages.py
--rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.6/brainchain/webapp/namespaces.py
--rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.6/brainchain/webapp/programs.py
--rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.6/brainchain/webapp/tasks.py
--rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.6/brainchain/webapp/tools.py
--rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.6/brainchain/webapp/users.py
--rw-r--r--   0        0        0      538 2024-05-11 18:02:06.987486 brainchain-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.7/brainchain/README.md
+-rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.6.7/brainchain/__init__.py
+-rw-r--r--   0        0        0    13624 2024-05-21 22:55:20.072457 brainchain-0.6.7/brainchain/assistants.py
+-rw-r--r--   0        0        0    11893 2024-05-21 21:07:38.845805 brainchain-0.6.7/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.6.7/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.7/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.7/brainchain/embeddings.py
+-rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.6.7/brainchain/graph/base.py
+-rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.6.7/brainchain/graph/schema.py
+-rw-r--r--   0        0        0     3791 2024-05-21 23:31:49.871373 brainchain-0.6.7/brainchain/logger.py
+-rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.6.7/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.7/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.6.7/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.7/brainchain/search_v2.py
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.7/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.6.7/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.6.7/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.7/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.7/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.7/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.7/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.7/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.7/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    21273 2024-05-21 21:16:24.442049 brainchain-0.6.7/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.6.7/brainchain/tools/web.py
+-rw-r--r--   0        0        0      734 2024-05-21 22:23:01.506213 brainchain-0.6.7/brainchain/tools.py
+-rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.6.7/brainchain/webapp/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.6.7/brainchain/webapp/agents.py
+-rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.6.7/brainchain/webapp/base.py
+-rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.6.7/brainchain/webapp/business_ideas.py
+-rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.6.7/brainchain/webapp/contents.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.6.7/brainchain/webapp/conversations.py
+-rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.6.7/brainchain/webapp/embedding_models.py
+-rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.6.7/brainchain/webapp/embeddings.py
+-rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.6.7/brainchain/webapp/files.py
+-rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.6.7/brainchain/webapp/health.py
+-rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.6.7/brainchain/webapp/language_models.py
+-rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.6.7/brainchain/webapp/laws.py
+-rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.6.7/brainchain/webapp/messages.py
+-rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.6.7/brainchain/webapp/namespaces.py
+-rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.6.7/brainchain/webapp/programs.py
+-rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.6.7/brainchain/webapp/tasks.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.6.7/brainchain/webapp/tools.py
+-rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.6.7/brainchain/webapp/users.py
+-rw-r--r--   0        0        0      538 2024-05-21 23:31:57.633720 brainchain-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.7/PKG-INFO
```

### Comparing `brainchain-0.6.6/brainchain/README.md` & `brainchain-0.6.7/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/__init__.py` & `brainchain-0.6.7/brainchain/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/assistants.py` & `brainchain-0.6.7/brainchain/assistants.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/brainchain.py` & `brainchain-0.6.7/brainchain/brainchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     Tools,
     Users,
 )
 
 from .products import keepa_datetime_to_int, keepa_int_to_datetime
 from .products import ProductsAPI
 
-from .assistants import *
 from .assistants import AssistantClient as AssistantsAPI
 class FunctionSchema:
     def __init__(self, name: str, description: str, parameters: dict, returns: dict):
         self.name = name
         self.description = description
         self.parameters = parameters
         self.returns = returns
@@ -65,28 +64,29 @@
         return component_cls(self.session, self.base_url, self.user_id)
 
     def __init__(
         self,
         env: str = "prod",
         # brainchain_api_key: str = os.environ["BRAINCHAIN_API_KEY"],
         salesintel_api_key: str = os.environ["SALESINTEL_API_KEY"],
-        base_url: str = os.getenv("API_HOST", "https://api.brainchain.cloud"),
+        api_host: str = os.getenv("API_HOST", "https://api.brainchain.cloud"),
         assistants_api_host: str = os.getenv("ASSISTANTS_API_HOST", "https://assistants-api.brainchain.cloud")
     ):
         if env == "prod":
-            self.base_url = base_url
+            self.api_host = api_host
+            self.assistants_api_host = assistants_api_host
             print("Brainchain API URL: ", self.base_url)
         elif env == "dev":
-            self.base_url = "http://localhost:8000"
+            self.api_host = "http://localhost:8000"
+            self.assistants_api_host = "http://localhost:42069"
             print("Brainchain API URL: ", self.base_url)
         elif env == "test":
-            self.base_url = self.base_url.replace("api", "api-test")
+            self.api_host = self.base_url.replace("api", "api-test")
             print("Brainchain API URL: ", self.base_url)
 
-        self.assistants_api_host = assistants_api_host
         self.web_data_client = WebDataClient()
         self.session = requests.Session()
         self.access_token = None
         self.user_id = None
         self.user_email = None
 
         if not os.path.exists(os.path.expanduser("~/.config/brainchain")):
```

### Comparing `brainchain-0.6.6/brainchain/carnivore.py` & `brainchain-0.6.7/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/coredata.py` & `brainchain-0.6.7/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/embeddings.py` & `brainchain-0.6.7/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/graph/base.py` & `brainchain-0.6.7/brainchain/graph/base.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/graph/schema.py` & `brainchain-0.6.7/brainchain/graph/schema.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/logger.py` & `brainchain-0.6.7/brainchain/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import asyncio
 import functools
 import logging
 import os
 import time
 
-import datadog
-import watchtower
+
+try:
+    import datadog
+except:
+    datadog_enabled = False
+    pass
+
+try:
+    import watchtower
+except:
+    watchtower_enabled = False
+    pass
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 # Configure AWS credentials
 aws_access_key_id = os.environ.get("AWS_ACCESS_KEY_ID")
 aws_secret_access_key = os.environ.get("AWS_SECRET_ACCESS_KEY")
@@ -19,86 +29,88 @@
 log_group_name = os.environ.get("LOG_GROUP_NAME")
 log_stream_name = os.environ.get("LOG_STREAM_NAME")
 
 try:
     # Check if Datadog environment variables are present
     datadog_api_key = os.environ.get("DATADOG_API_KEY")
     datadog_app_key = os.environ.get("DATADOG_APP_KEY")
-    datadog_enabled = datadog_api_key is not None and datadog_app_key is not None
+    datadog_enabled = datadog_api_key is not None and datadog_app_key is not None and datadog_enabled
     # Initialize Datadog if the environment variables are present
     if datadog_enabled:
         datadog.initialize(api_key=datadog_api_key, app_key=datadog_app_key)
 except:
     pass
 
 # Initialize Datadog if the environment variables are present
 if datadog_enabled:
     datadog.initialize(api_key=datadog_api_key, app_key=datadog_app_key)
 
-# Set up the logger to send logs to CloudWatch
-handler = watchtower.CloudWatchLogHandler(
-    log_group=log_group_name, stream_name=log_stream_name
-)
-handler.setFormatter(
-    logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-)
-
-logger.addHandler(handler)
-
-def log_function_info(func):
-    if asyncio.iscoroutinefunction(func):
-
-        @functools.wraps(func)
-        async def async_wrapper(*args, **kwargs):
-            # Log function name and parameters at the beginning
-            logger.info(f"Calling {func.__name__} with args: {args}, kwargs: {kwargs}")
-
-            # Increment a counter in Datadog if enabled
-            if datadog_enabled:
-                datadog.statsd.increment(f"{func.__name__}.calls")
-
-            start_time = time.time()
-
-            try:
-                result = await func(*args, **kwargs)
-            except Exception as e:
-                logger.exception(f"Exception in {func.__name__}: {e}")
-                raise
-            finally:
-                end_time = time.time()
-                elapsed_time = end_time - start_time
-                logger.info(f"{func.__name__} completed in {elapsed_time:.4f} seconds")
 
-                # Send the timing to Datadog if enabled
-                if datadog_enabled:
-                    datadog.statsd.timing(f"{func.__name__}.time", elapsed_time)
+if watchtower_enabled:
+    # Set up the logger to send logs to CloudWatch
+    handler = watchtower.CloudWatchLogHandler(
+        log_group=log_group_name, stream_name=log_stream_name
+    )
+    handler.setFormatter(
+        logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+    )
+
+    logger.addHandler(handler)
+
+    def log_function_info(func):
+        if asyncio.iscoroutinefunction(func):
+
+            @functools.wraps(func)
+            async def async_wrapper(*args, **kwargs):
+                # Log function name and parameters at the beginning
+                logger.info(f"Calling {func.__name__} with args: {args}, kwargs: {kwargs}")
 
-            return result
+                # Increment a counter in Datadog if enabled
+                if datadog_enabled:
+                    datadog.statsd.increment(f"{func.__name__}.calls")
 
-        return async_wrapper
-    else:
+                start_time = time.time()
 
-        @functools.wraps(func)
-        def sync_wrapper(*args, **kwargs):
-            logger.info(f"Calling {func.__name__} with args: {args}, kwargs: {kwargs}")
-
-            if datadog_enabled:
-                datadog.statsd.increment(f"{func.__name__}.calls")
-
-            start_time = time.time()
-
-            try:
-                result = func(*args, **kwargs)
-            except Exception as e:
-                logger.exception(f"Exception in {func.__name__}: {e}")
-                raise
-            finally:
-                end_time = time.time()
-                elapsed_time = end_time - start_time
-                logger.info(f"{func.__name__} completed in {elapsed_time:.4f} seconds")
+                try:
+                    result = await func(*args, **kwargs)
+                except Exception as e:
+                    logger.exception(f"Exception in {func.__name__}: {e}")
+                    raise
+                finally:
+                    end_time = time.time()
+                    elapsed_time = end_time - start_time
+                    logger.info(f"{func.__name__} completed in {elapsed_time:.4f} seconds")
+
+                    # Send the timing to Datadog if enabled
+                    if datadog_enabled:
+                        datadog.statsd.timing(f"{func.__name__}.time", elapsed_time)
+
+                return result
+
+            return async_wrapper
+        else:
+
+            @functools.wraps(func)
+            def sync_wrapper(*args, **kwargs):
+                logger.info(f"Calling {func.__name__} with args: {args}, kwargs: {kwargs}")
 
                 if datadog_enabled:
-                    datadog.statsd.timing(f"{func.__name__}.time", elapsed_time)
+                    datadog.statsd.increment(f"{func.__name__}.calls")
+
+                start_time = time.time()
+
+                try:
+                    result = func(*args, **kwargs)
+                except Exception as e:
+                    logger.exception(f"Exception in {func.__name__}: {e}")
+                    raise
+                finally:
+                    end_time = time.time()
+                    elapsed_time = end_time - start_time
+                    logger.info(f"{func.__name__} completed in {elapsed_time:.4f} seconds")
+
+                    if datadog_enabled:
+                        datadog.statsd.timing(f"{func.__name__}.time", elapsed_time)
 
-            return result
+                return result
 
-        return sync_wrapper
+            return sync_wrapper
```

### Comparing `brainchain-0.6.6/brainchain/products.py` & `brainchain-0.6.7/brainchain/products.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/requirements.txt` & `brainchain-0.6.7/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/sales_intel.py` & `brainchain-0.6.7/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/search_v2.py` & `brainchain-0.6.7/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/__init__.py` & `brainchain-0.6.7/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/coding.py` & `brainchain-0.6.7/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/diffbot.py` & `brainchain-0.6.7/brainchain/tools/diffbot.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/factual.py` & `brainchain-0.6.7/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/fts.py` & `brainchain-0.6.7/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/graph.py` & `brainchain-0.6.7/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/memory.py` & `brainchain-0.6.7/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/plan.py` & `brainchain-0.6.7/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/tokens.py` & `brainchain-0.6.7/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/tools.py` & `brainchain-0.6.7/brainchain/tools/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools/web.py` & `brainchain-0.6.7/brainchain/tools/web.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/tools.py` & `brainchain-0.6.7/brainchain/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 from brainchain.tools.memory import insert_memory, lookup_similar_memories, delete_memories
 from brainchain.tools.tokens import encode_text, decode_tokens
 from brainchain.tools.fts import fts_ingest_document, fts_search_index, fts_document_qa, fts_extract, fts_indices, fts_health_check
 from brainchain.tools.graph import execute_cypher_query, graph_query
 from brainchain.tools.factual import fact_check
 from brainchain.tools.diffbot import diffbot_analyze
 from brainchain.tools.plan import generate_plan, improve_plan, execute_plan
-from brainchain.tools import functions
+from brainchain.tools import tool_schemas
```

### Comparing `brainchain-0.6.6/brainchain/webapp/__init__.py` & `brainchain-0.6.7/brainchain/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/business_ideas.py` & `brainchain-0.6.7/brainchain/webapp/business_ideas.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/contents.py` & `brainchain-0.6.7/brainchain/webapp/contents.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/conversations.py` & `brainchain-0.6.7/brainchain/webapp/conversations.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/embeddings.py` & `brainchain-0.6.7/brainchain/webapp/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/files.py` & `brainchain-0.6.7/brainchain/webapp/files.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/laws.py` & `brainchain-0.6.7/brainchain/webapp/laws.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/messages.py` & `brainchain-0.6.7/brainchain/webapp/messages.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/namespaces.py` & `brainchain-0.6.7/brainchain/webapp/namespaces.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/programs.py` & `brainchain-0.6.7/brainchain/webapp/programs.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/tasks.py` & `brainchain-0.6.7/brainchain/webapp/tasks.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/tools.py` & `brainchain-0.6.7/brainchain/webapp/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/brainchain/webapp/users.py` & `brainchain-0.6.7/brainchain/webapp/users.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.6.6/pyproject.toml` & `brainchain-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.6.6"
+version = "0.6.7"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
```

### Comparing `brainchain-0.6.6/PKG-INFO` & `brainchain-0.6.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.6.6
+Version: 0.6.7
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

