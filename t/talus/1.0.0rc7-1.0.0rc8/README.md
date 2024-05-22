# Comparing `tmp/talus-1.0.0rc7.tar.gz` & `tmp/talus-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc7.tar", last modified: Tue May 21 22:06:00 2024, max compression
+gzip compressed data, was "talus-1.0.0rc8.tar", last modified: Wed May 22 14:24:36 2024, max compression
```

## Comparing `talus-1.0.0rc7.tar` & `talus-1.0.0rc8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-21 22:05:47.000000 talus-1.0.0rc7/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-21 22:05:47.000000 talus-1.0.0rc7/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-21 22:05:47.000000 talus-1.0.0rc7/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-21 22:05:47.000000 talus-1.0.0rc7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-21 22:06:00.292630 talus-1.0.0rc7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-21 22:05:47.000000 talus-1.0.0rc7/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-21 22:05:47.000000 talus-1.0.0rc7/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-21 22:05:47.000000 talus-1.0.0rc7/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-21 22:06:00.292630 talus-1.0.0rc7/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.288629 talus-1.0.0rc7/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     4721 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4667 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4888 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-21 22:05:59.000000 talus-1.0.0rc7/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-21 22:05:47.000000 talus-1.0.0rc7/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 14:24:23.000000 talus-1.0.0rc8/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 14:24:23.000000 talus-1.0.0rc8/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 14:24:23.000000 talus-1.0.0rc8/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-22 14:24:23.000000 talus-1.0.0rc8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 14:24:36.440673 talus-1.0.0rc8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-22 14:24:23.000000 talus-1.0.0rc8/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-22 14:24:23.000000 talus-1.0.0rc8/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-22 14:24:23.000000 talus-1.0.0rc8/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 14:24:36.440673 talus-1.0.0rc8/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.436673 talus-1.0.0rc8/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4567 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4667 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3391 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-22 14:24:23.000000 talus-1.0.0rc8/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:24:36.440673 talus-1.0.0rc8/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-22 14:24:36.000000 talus-1.0.0rc8/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-22 14:24:23.000000 talus-1.0.0rc8/tox.ini
```

### Comparing `talus-1.0.0rc7/.gitignore` & `talus-1.0.0rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/.pre-commit-config.yaml` & `talus-1.0.0rc8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/LICENSE` & `talus-1.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/PKG-INFO` & `talus-1.0.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc7/README.rst` & `talus-1.0.0rc8/README.rst`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/bitbucket-pipelines.yml` & `talus-1.0.0rc8/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/pyproject.toml` & `talus-1.0.0rc8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/base.py` & `talus-1.0.0rc8/talus/base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/consumer.py` & `talus-1.0.0rc8/talus/consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/models/binding.py` & `talus-1.0.0rc8/talus/models/binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/models/connection_parameters.py` & `talus-1.0.0rc8/talus/models/connection_parameters.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/models/exchange.py` & `talus-1.0.0rc8/talus/models/exchange.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/models/message.py` & `talus-1.0.0rc8/talus/models/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,20 +36,14 @@
     def __init__(self, routing_key: str, body: bytes | dict | str | MessageBodyBase):
         self.routing_key = routing_key
         if isinstance(body, dict | BaseModel):
             self.body: MessageBodyBase = self.message_body_cls.model_validate(body)
         else:  # str | bytes
             self.body: MessageBodyBase = self.message_body_cls.model_validate_json(body)
 
-    def __str__(self):
-        return str(self.body)
-
-    def __repr__(self):
-        return f"s{self.__class__.__name__}(routing_key={self.routing_key}, body={self.body!r})"
-
 
 class ConsumeMessageBase(_MessageBase):
     """
     Base class for messages consumed from a DurableConsumer MessageProcessor.  Each instance
     correlates with a single consumed message.  The body of the message is validated against the
     message_body_cls class attribute.
     >>> class ObjectBucketBody(MessageBodyBase):
@@ -79,15 +73,15 @@
         return self.method.delivery_tag
 
     @property
     def headers(self) -> dict | None:
         return self.properties.headers
 
     def __repr__(self):
-        return f"s{self.__class__.__name__}(method={self.method!r}, properties={self.properties!r}, body={self.body!r})"
+        return f"{self.__class__.__name__}(method={self.method!r}, properties={self.properties!r}, body={self.body!r})"
 
 
 class PublishMessageBase(_MessageBase):
     """
     Base class for messages published to with a DurableProducer.
     Each instance correlates with a single message to publish.  The body of the message is validated
     against the class defined in message_body_cls class attribute.  Additional class attributes for
@@ -124,8 +118,8 @@
             priority=0,
             delivery_mode=pika.DeliveryMode.Persistent,
             content_encoding="UTF-8",
             headers=self.headers,
         )
 
     def __repr__(self):
-        return f"s{self.__class__.__name__}(body={self.body!r})"
+        return f"{self.__class__.__name__}(body={self.body!r}) # {self.routing_key = }"
```

### Comparing `talus-1.0.0rc7/talus/models/processor.py` & `talus-1.0.0rc8/talus/models/processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/models/retryer.py` & `talus-1.0.0rc8/talus/models/retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/producer.py` & `talus-1.0.0rc8/talus/producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/conftest.py` & `talus-1.0.0rc8/talus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/models/test_binding.py` & `talus-1.0.0rc8/talus/tests/models/test_binding.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/models/test_message.py` & `talus-1.0.0rc8/talus/tests/models/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     assert message.properties == properties
     assert message.routing_key == routing_key
     assert message.headers == headers
     assert message.delivery_tag == delivery_tag
     assert (
         message.body.model_dump() == {"conversationId": message.body.conversationId} | message_data
     )
+    assert repr(message)
 
 
 class ExampleMessageBody(MessageBodyBase):
     required_str: str
     required_int: int
 
 
@@ -75,14 +76,15 @@
     assert message.routing_key == routing_key
     assert message.headers == headers
     assert isinstance(message.properties, pika.spec.BasicProperties)
     assert message.properties.headers == headers
     assert (
         message.body.model_dump() == {"conversationId": message.body.conversationId} | message_data
     )
+    assert repr(message)
 
 
 class PublishMessage(PublishMessageBase):
     message_body_cls = ExampleMessageBody
     default_routing_key = "test.m"
```

### Comparing `talus-1.0.0rc7/talus/tests/models/test_processor.py` & `talus-1.0.0rc8/talus/tests/models/test_processor.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/models/test_queue.py` & `talus-1.0.0rc8/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/models/test_retryer.py` & `talus-1.0.0rc8/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/test_base.py` & `talus-1.0.0rc8/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/test_consumer.py` & `talus-1.0.0rc8/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus/tests/test_producer.py` & `talus-1.0.0rc8/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/talus.egg-info/PKG-INFO` & `talus-1.0.0rc8/talus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talus
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: A wrapper for connecting to RabbitMQ which constrains clients to a single purpose channel (producer or consumer) with healing for intermittent connectivity.
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/interservice-bus-adapter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `talus-1.0.0rc7/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc8/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc7/tox.ini` & `talus-1.0.0rc8/tox.ini`

 * *Files identical despite different names*

