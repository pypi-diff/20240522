# Comparing `tmp/talus-1.0.0rc8.tar.gz` & `tmp/talus-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc8.tar", last modified: Wed May 22 14:24:36 2024, max compression
+gzip compressed data, was "talus-1.0.0rc9.tar", last modified: Wed May 22 17:16:31 2024, max compression
```

## Comparing `talus-1.0.0rc8.tar` & `talus-1.0.0rc9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 14:24:23.000000 talus-1.0.0rc8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 14:24:23.000000 talus-1.0.0rc8/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 14:24:23.000000 talus-1.0.0rc8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-22 14:24:23.000000 talus-1.0.0rc8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 14:24:36.440673 talus-1.0.0rc8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-22 14:24:23.000000 talus-1.0.0rc8/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-22 14:24:23.000000 talus-1.0.0rc8/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-22 14:24:23.000000 talus-1.0.0rc8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 14:24:36.440673 talus-1.0.0rc8/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.436673 talus-1.0.0rc8/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4667 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-22 14:24:23.000000 talus-1.0.0rc8/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 17:16:12.000000 talus-1.0.0rc9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 17:16:12.000000 talus-1.0.0rc9/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 17:16:12.000000 talus-1.0.0rc9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-22 17:16:12.000000 talus-1.0.0rc9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 17:16:31.005180 talus-1.0.0rc9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-22 17:16:12.000000 talus-1.0.0rc9/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-22 17:16:12.000000 talus-1.0.0rc9/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-22 17:16:12.000000 talus-1.0.0rc9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 17:16:31.005180 talus-1.0.0rc9/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.001180 talus-1.0.0rc9/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 17:16:12.000000 talus-1.0.0rc9/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 17:16:31.005180 talus-1.0.0rc9/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 17:16:30.000000 talus-1.0.0rc9/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-22 17:16:12.000000 talus-1.0.0rc9/tox.ini
```

### Comparing `talus-1.0.0rc8/.gitignore` & `talus-1.0.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/.pre-commit-config.yaml` & `talus-1.0.0rc9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/LICENSE` & `talus-1.0.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/PKG-INFO` & `talus-1.0.0rc9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc8/README.rst` & `talus-1.0.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/bitbucket-pipelines.yml` & `talus-1.0.0rc9/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/pyproject.toml` & `talus-1.0.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/base.py` & `talus-1.0.0rc9/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/consumer.py` & `talus-1.0.0rc9/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/models/binding.py` & `talus-1.0.0rc9/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/models/connection_parameters.py` & `talus-1.0.0rc9/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/models/exchange.py` & `talus-1.0.0rc9/talus/models/exchange.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/models/message.py` & `talus-1.0.0rc9/talus/models/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     >>> queue_bindings = Binding(queue=queue, message=OutboundMessage)
     >>> with DurableProducer(queue_bindings=queue_bindings, publish_exchange=exchange) as producer:
     >>>     body = {"objectName": "object", "bucket": "bucket"}
     >>>     producer.publish(OutboundMessage(body))
     """
 
     default_routing_key: str = "default.m"
-    headers: dict[str, str] | None = (None,)
+    headers: dict[str, str] | None = None
 
     def __init__(
         self,
         body: bytes | dict | str | MessageBodyBase,
     ):
         super().__init__(self.default_routing_key, body)
```

### Comparing `talus-1.0.0rc8/talus/models/processor.py` & `talus-1.0.0rc9/talus/models/processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/models/retryer.py` & `talus-1.0.0rc9/talus/models/retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/producer.py` & `talus-1.0.0rc9/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/conftest.py` & `talus-1.0.0rc9/talus/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,17 +51,23 @@
             return message_data
         case "json-body":
             return json.dumps(message_data)
         case _:
             raise NotImplementedError("body type not implemented")
 
 
-@pytest.fixture()
-def headers() -> dict[str, str]:
-    return {"header1": "value1"}
+@pytest.fixture(params=["no-headers", "headers"])
+def headers(request) -> dict[str, str] | None:
+    match request.param:
+        case "no-headers":
+            return None
+        case "headers":
+            return {"header1": "value1"}
+        case _:
+            raise NotImplementedError("headers parameter not implemented")
 
 
 @pytest.fixture()
 def properties(headers) -> pika.spec.BasicProperties:
     return pika.spec.BasicProperties(headers=headers)
```

### Comparing `talus-1.0.0rc8/talus/tests/models/test_binding.py` & `talus-1.0.0rc9/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/models/test_message.py` & `talus-1.0.0rc9/talus/tests/models/test_message.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/models/test_processor.py` & `talus-1.0.0rc9/talus/tests/models/test_processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/models/test_queue.py` & `talus-1.0.0rc9/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/models/test_retryer.py` & `talus-1.0.0rc9/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/test_base.py` & `talus-1.0.0rc9/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/test_consumer.py` & `talus-1.0.0rc9/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus/tests/test_producer.py` & `talus-1.0.0rc9/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/talus.egg-info/PKG-INFO` & `talus-1.0.0rc9/talus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc8/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc9/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc8/tox.ini` & `talus-1.0.0rc9/tox.ini`

 * *Files identical despite different names*

