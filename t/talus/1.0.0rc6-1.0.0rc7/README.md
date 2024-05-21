# Comparing `tmp/talus-1.0.0rc6.tar.gz` & `tmp/talus-1.0.0rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talus-1.0.0rc6.tar", last modified: Mon May 20 18:15:24 2024, max compression
+gzip compressed data, was "talus-1.0.0rc7.tar", last modified: Tue May 21 22:06:00 2024, max compression
```

## Comparing `talus-1.0.0rc6.tar` & `talus-1.0.0rc7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-20 18:15:11.000000 talus-1.0.0rc6/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-20 18:15:11.000000 talus-1.0.0rc6/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-20 18:15:11.000000 talus-1.0.0rc6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-20 18:15:11.000000 talus-1.0.0rc6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-20 18:15:24.281118 talus-1.0.0rc6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2300 2024-05-20 18:15:11.000000 talus-1.0.0rc6/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-20 18:15:11.000000 talus-1.0.0rc6/bitbucket-pipelines.yml
--rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-20 18:15:11.000000 talus-1.0.0rc6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-20 18:15:24.281118 talus-1.0.0rc6/setup.cfg
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.277118 talus-1.0.0rc6/talus/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4013 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/base.py
--rw-rw-rw-   0 root         (0) root         (0)     6256 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/consumer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/binding.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/exchange.py
--rw-rw-rw-   0 root         (0) root         (0)     2368 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/processor.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/queue.py
--rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/models/retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     4703 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus/tests/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_binding.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_connection_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)     7784 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_processor.py
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_queue.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/models/test_retryer.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_consumer.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-20 18:15:11.000000 talus-1.0.0rc6/talus/tests/test_producer.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-20 18:15:24.281118 talus-1.0.0rc6/talus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3201 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-20 18:15:23.000000 talus-1.0.0rc6/talus.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-20 18:15:24.000000 talus-1.0.0rc6/talus.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-20 18:15:11.000000 talus-1.0.0rc6/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-21 22:05:47.000000 talus-1.0.0rc7/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-21 22:05:47.000000 talus-1.0.0rc7/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-21 22:05:47.000000 talus-1.0.0rc7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      460 2024-05-21 22:05:47.000000 talus-1.0.0rc7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-21 22:06:00.292630 talus-1.0.0rc7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3987 2024-05-21 22:05:47.000000 talus-1.0.0rc7/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1830 2024-05-21 22:05:47.000000 talus-1.0.0rc7/bitbucket-pipelines.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1849 2024-05-21 22:05:47.000000 talus-1.0.0rc7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-21 22:06:00.292630 talus-1.0.0rc7/setup.cfg
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.288629 talus-1.0.0rc7/talus/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4081 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7571 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/consumer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/binding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2063 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/exchange.py
+-rw-rw-rw-   0 root         (0) root         (0)     4721 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7942 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     2672 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/models/retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     5770 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4667 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus/tests/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_binding.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_connection_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     7010 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/models/test_retryer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4005 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_consumer.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2024-05-21 22:05:47.000000 talus-1.0.0rc7/talus/tests/test_producer.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-21 22:06:00.292630 talus-1.0.0rc7/talus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4888 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      964 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-21 22:05:59.000000 talus-1.0.0rc7/talus.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-21 22:06:00.000000 talus-1.0.0rc7/talus.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1184 2024-05-21 22:05:47.000000 talus-1.0.0rc7/tox.ini
```

### Comparing `talus-1.0.0rc6/.gitignore` & `talus-1.0.0rc7/.gitignore`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/.pre-commit-config.yaml` & `talus-1.0.0rc7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/LICENSE` & `talus-1.0.0rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/bitbucket-pipelines.yml` & `talus-1.0.0rc7/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/pyproject.toml` & `talus-1.0.0rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus/base.py` & `talus-1.0.0rc7/talus/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,26 +41,22 @@
         else:  # factory
             self.connection_retryer = connection_retryer()
         self.connection: pika.BlockingConnection | None = None
         self.channel: pika.adapters.blocking_connection.BlockingChannel | None = None
 
     def connect(self):
         """
-        Retries as configured the connection to the RabbitMQ server.
-
-        :return: None
+        Connect to the RabbitMQ server retrying errors configured in the connection_retryer.
         """
         if not self.is_connected:
             self.connection_retryer(self._connect)
 
     def _connect(self):
         """
         Configures and initiates connection to the RabbitMQ server.
-
-        :return: None
         """
         logger.debug(
             f"Attempt to connect to RabbitMQ: connection_params={self.connection_parameters}"
         )
         self.connection = pika.BlockingConnection(self.connection_parameters)
         logger.info(f"Connection Created")
         self.channel = self.connection.channel()
@@ -77,44 +73,45 @@
         if self.connection is not None:
             return self.connection.is_open
         return False
 
     def disconnect(self):
         """
         Closes connection and related channels to the RabbitMQ Server.
-
-        :return: None
         """
+
         if self.is_connected:
             self.connection.close()
         logger.info(f"Disconnected from RabbitMQ: " f"connection={self.connection_parameters}")
 
     def create_queue(self, queue: Queue):
+        """
+        Create a queue on an already opened connection.
+        """
         self.channel.queue_declare(
             queue=queue.name,
             durable=queue.durable,
             passive=queue.passive,
             auto_delete=queue.auto_delete,
             exclusive=queue.exclusive,
             arguments=queue.arguments,
         )
         logger.info(f"Queue Created: queue={queue.name}")
 
     def __enter__(self):
         """
-        Entry for with context manager.
+        Entry for context manager.
 
         :return: connected instance of self
         """
         self.connect()
         return self
 
     def __exit__(self, exc_type, value, traceback):
         """
-        Exit for with context manager.  Disconnects from rabbitmq
-
-        :return: None
+        Exit for context manager which disconnects from rabbitmq
         """
         self.disconnect()
 
     def __repr__(self):
+        """Representation of the DurableConnection object"""
         return f"{self.__class__.__name__}(connection_parameters={self.connection_parameters!r}), connection_retryer={self.connection_retryer!r})"
```

### Comparing `talus-1.0.0rc6/talus/consumer.py` & `talus-1.0.0rc7/talus/consumer.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,14 +26,27 @@
     None,
 ]
 
 
 class DurableConsumer(DurableConnection):
     """
     RabbitMQ connector for consuming from a single queue in RabbitMQ.
+    >>> from talus.models.queue import Queue
+    >>> from talus.models.connection_parameters import ConsumerConnectionParameterFactory
+    >>> from talus.models.retryer import ConnectionRetryerFactory
+    >>> from talus.consumer import DurableConsumer
+    >>> from talus.models.processor import MessageProcessorBase
+    >>> from talus.models.message import ConsumeMessageBase
+    >>> consume_queue = Queue(name="test_queue")
+    >>> class MessageProcessor(MessageProcessorBase):
+    >>>     def process_message(message: ConsumeMessageBase):
+    >>>         print(message)
+    >>> with DurableConsumer(consume_queue=consume_queue, prefetch_count=1, connection_parameters=ConsumerConnectionParameterFactory(), connection_retryer=ConnectionRetryerFactory()) as consumer:
+    >>>     with MessageProcessor() as message_processor:
+    >>>         consumer.listen(message_processor)
     """
 
     def __init__(
         self,
         consume_queue: Queue,
         prefetch_count: int = 1,
         connection_parameters: pika.ConnectionParameters
@@ -58,16 +71,16 @@
             connection_retryer=connection_retryer,
         )
         self.consume_queue = consume_queue
         self.prefetch_count = prefetch_count
 
     def _connect(self) -> None:
         """
-        Configures and initiates consumer connection to the RabbitMQ server.
-        :return:
+        Configures and initiates consumer connection to the RabbitMQ server which includes
+        setting up the queue to consume from and the prefetch count.
         """
         super()._connect()
         self.channel.basic_qos(prefetch_count=self.prefetch_count)
         self.create_queue(queue=self.consume_queue)
 
     def _listen(self, callback: LISTEN_CALLBACK_TYPE) -> None:
         """
@@ -75,43 +88,41 @@
 
         :param callback: Function to execute when a message is received. with the signature
         (ch, method, properties, body).
         ch: Copy of the channel used to acknowledge receipt (pika.Channel)
         method: Management keys for the delivered message e.g. delivery mode (pika.spec.Basic.Deliver)
         properties: Message properties (pika.spec.BasicProperties)
         body: Message body for a transfer message (bytes)
-
-        :return: None
         """
         self.connect()
         logger.info(f"Starting Listener on Queue: consumer_queue={self.consume_queue}")
         self.channel.basic_consume(queue=self.consume_queue.name, on_message_callback=callback)
         self.channel.start_consuming()
 
     def listen(self, message_processor: LISTEN_CALLBACK_TYPE) -> None:
         """
-        Retries calls to _listen
-
+        Retries calls to _listen and executes the message_processor callback when a message is received.
+        This method is blocking and will not return until the connection is closed.
         :param message_processor: Callable to execute when a message is received. with the signature
         (channel, method, properties, body).
         channel: Copy of the channel used to acknowledge receipt (pika.Channel)
         method: Management keys for the delivered message e.g. delivery mode (pika.spec.Basic.Deliver)
         properties: Message properties (pika.spec.BasicProperties)
         body: Message body for a transfer message (bytes)
         and returns None.
-        :return: None
         """
         self.connection_retryer(self._listen, callback=message_processor)
 
     def consume_generator(self, auto_ack=False, inactivity_timeout: float = 0.1) -> Generator:
         """
         Creates a generator for messages that are on the instance consumer_queue.
         Retry logic is not applied to prevent the resetting of the generator cursor
 
-        :param inactivity_timeout:
+        :param auto_ack: Automatically acknowledge messages
+        :param inactivity_timeout: Number of seconds to wait for a message before returning None
 
         :return: Generator of (method, properties, body)
         """
         self.connect()
         logger.info(f"Creating consumer generator on Queue: consumer_queue={self.consume_queue}")
         return self.channel.consume(
             queue=self.consume_queue.name, auto_ack=auto_ack, inactivity_timeout=inactivity_timeout
@@ -129,39 +140,40 @@
         """
         Record a message as acknowledged.
         Retry logic is not applied since creating a new channel would be unable
         to acknowledge the message received on the now dead channel
 
         :param delivery_tag: method.delivery_tag
 
-        :param multiple:
+        :param multiple: Acknowledge multiple messages by setting to True and acknowledging the last message
 
         :return: None
         """
         self.channel.basic_ack(delivery_tag, multiple)
 
     def reject_message(self, delivery_tag) -> None:
         """
         Record a message as rejected.  Will go to dead letter exchange if configured on the server.
         Retry logic is not applied since creating a new channel would be unable
-        to acknowledge the message received on the now dead channel
+        to use the delivery tag received on the now dead channel
 
         :param delivery_tag: method.delivery_tag
 
         :return: None
         """
         self.channel.basic_reject(delivery_tag=delivery_tag, requeue=False)
 
     def requeue_message(self, delivery_tag) -> None:
         """
         Return message back to the queue.
         Retry logic is not applied since creating a new channel would be unable
-        to acknowledge the message received on the now dead channel
+        to use the delivery tag received on the now dead channel
 
         :param delivery_tag: method.delivery_tag
 
         :return: None
         """
         self.channel.basic_nack(delivery_tag=delivery_tag, requeue=True)
 
     def __repr__(self):
+        """Representation of the DurableConsumer instance."""
         return f"{self.__class__.__name__}(consume_queue={self.consume_queue !r}, prefetch_count={self.prefetch_count}, connection_parameters={self.connection_parameters!r}, connection_retryer={self.connection_retryer!r})"
```

### Comparing `talus-1.0.0rc6/talus/models/binding.py` & `talus-1.0.0rc7/talus/models/binding.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,27 +9,38 @@
 from typing_extensions import Annotated
 
 from talus.models.message import PublishMessageBase
 from talus.models.queue import Queue
 
 
 def validate_routing_key(message: Type[PublishMessageBase]):
-    if not message.routing_key:
-        raise ValueError("routing_key must not be empty")
+    """Custom pydantic validator to ensure that the routing key is not empty."""
+    if not message.default_routing_key:
+        raise ValueError("default_routing_key must not be empty")
     return message
 
 
 class Binding(BaseModel):
-    """Binding configuration."""
+    """
+    Binding configuration.
+
+    >>> from talus.models.binding import Binding
+    >>> from talus.models.message import PublishMessageBase
+    >>> from talus.models.queue import Queue
+    >>> queue = Queue(name="my.queue")
+    >>> class PublishMessage(PublishMessageBase):
+    >>>     default_routing_key = "my.routing.key"
+    >>> binding = Binding(message=PublishMessage, queue=queue)
+    """
 
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     message: Annotated[Type[PublishMessageBase], AfterValidator(validate_routing_key)]
     queue: Queue
 
     @property
     def routing_key(self) -> str:
-        return self.message.routing_key
+        return self.message.default_routing_key
 
     @property
     def queue_name(self) -> str:
         return self.queue.name
```

### Comparing `talus-1.0.0rc6/talus/models/retryer.py` & `talus-1.0.0rc7/talus/models/retryer.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,21 @@
 from tenacity import wait_exponential
 from tenacity import wait_random
 
 logger = logging.getLogger(__name__)
 
 
 class RetryerFactory(BaseModel):
-    """Translator for the retry configuration to a tenacity.Retrying object."""
+    """
+    Translator for the retry configuration to a tenacity.Retrying object.
+
+    >>> from talus.models.retryer import RetryerFactory
+    >>> factory = RetryerFactory()
+    >>> retryer = factory()
+    """
 
     delay_min: int = 1
     delay_max: int = 300
     jitter_min: int = 1
     jitter_max: int = 10
     attempts: int = -1  # -1 means retry forever
     exceptions: type[Exception] | tuple[type[Exception], ...] = type(
@@ -71,8 +77,10 @@
     InvalidChannelNumber,
     UnexpectedFrameError,
     ChannelError,
 )
 
 
 class ConnectionRetryerFactory(RetryerFactory):
+    """Retryer Factory for connection exceptions."""
+
     exceptions: type[Exception] | tuple[type[Exception], ...] = DEFAULT_CONNECTION_EXCEPTIONS
```

### Comparing `talus-1.0.0rc6/talus/producer.py` & `talus-1.0.0rc7/talus/producer.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,29 @@
         :param publish_exchange: Name of the exchange that the  producer will publish to.
 
         :param connection_parameters: A pika.ConnectionParameters object or one resulting
             from a callable that returns a ConnectionParameters object.
 
         :param connection_retryer: A tenacity.Retrying object or one resulting from a callable that returns
             a Retrying object.
+
+        >>> from talus.models.binding import Binding
+        >>> from talus.models.exchange import Exchange
+        >>> from talus.producer import DurableProducer
+        >>> from talus.models.retryer import ConnectionRetryerFactory
+        >>> from talus.models.connection_parameters import ProducerConnectionParameterFactory
+        >>> from talus.models.queue import Queue
+        >>> from talus.models.message import PublishMessageBase
+        >>> queue = Queue(name="test_queue")
+        >>> exchange = Exchange(name="test_exchange")
+        >>> # Bind the queue to the routing key on message.
+        >>> queue_bindings = Binding(queue=queue, message=PublishMessageBase)
+        >>> with DurableProducer(queue_bindings=queue_bindings, publish_exchange=exchange, connection_parameters=ProducerConnectionParameterFactory(), connection_retryer=ConnectionRetryerFactory()) as producer:
+        >>>     producer.publish(PublishMessageBase(body={"test": "test"}))
+
         """
         super().__init__(
             connection_parameters=connection_parameters, connection_retryer=connection_retryer
         )
         if isinstance(queue_bindings, Binding):
             queue_bindings = [queue_bindings]
         self.queue_bindings = queue_bindings
@@ -92,31 +107,32 @@
                 f"Bindings configured: exchange={self.publish_exchange}, "
                 f"queue={binding.queue.name}, "
                 f"routing_key={binding.routing_key} "
             )
 
     def _publish(self, message: PublishMessageBase) -> None:
         """
-        Post message to the exchange configured on the producer instance
+        Publish message to the exchange configured on the producer
 
-        :param message: TODO
+        :param message: Message to publish
         :return: None
         """
         self.connect()
         self.publish_retryer(
             self.channel.basic_publish,
             exchange=self.publish_exchange.name,
             routing_key=message.routing_key,
             body=message.body.model_dump_json(by_alias=True),
             properties=message.properties,
             mandatory=True,  # paired with channel.confirm_delivery() to ensure message persistence
         )
 
     def publish(self, message: PublishMessageBase) -> None:
         """
-        Publish a message using an object constructed with the talus.message.message_class decorator
+        Publish message to the exchange configured on the producer retrying connection errors configured in the connection_retryer.
         :return: None
         """
         self.connection_retryer(self._publish, message=message)
 
     def __repr__(self):
+        """Representation of the DurableProducer instance."""
         return f"{self.__class__.__name__}(queue_bindings={self.queue_bindings !r}, exchange={self.publish_exchange!r}, connection_parameters={self.connection_parameters!r}, connection_retryer={self.connection_retryer!r})"
```

### Comparing `talus-1.0.0rc6/talus/tests/conftest.py` & `talus-1.0.0rc7/talus/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 @pytest.fixture
 def publish_message_cls(routing_key, headers) -> Type[PublishMessageBase]:
     """A test publish message class."""
     rk = routing_key
     h = headers
 
     class PublishMessage(PublishMessageBase):
-        routing_key: str = rk
+        default_routing_key: str = rk
         headers: dict[str, str] = h
 
     return PublishMessage
 
 
 @pytest.fixture()
 def direct_exchange() -> Exchange:
```

### Comparing `talus-1.0.0rc6/talus/tests/models/test_binding.py` & `talus-1.0.0rc7/talus/tests/models/test_binding.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 @pytest.fixture()
 def consume_message(body, method, properties) -> ConsumeMessageBase:
     return ConsumeMessageBase(method=method, properties=properties, body=body)
 
 
 class BadPublishMessage(PublishMessageBase):
-    routing_key = ""
+    default_routing_key = ""
 
 
 @pytest.mark.parametrize(
     "message, queue",
     [
         pytest.param(
             ConsumeMessageBase,
```

### Comparing `talus-1.0.0rc6/talus/tests/models/test_message.py` & `talus-1.0.0rc7/talus/tests/models/test_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     assert (
         message.body.model_dump() == {"conversationId": message.body.conversationId} | message_data
     )
 
 
 class PublishMessage(PublishMessageBase):
     message_body_cls = ExampleMessageBody
-    routing_key = "test.m"
+    default_routing_key = "test.m"
 
 
 @pytest.mark.parametrize(
     "invalid_body",
     [
         pytest.param(
             json.dumps({"required_str": 1, "required_int": "zz"}).encode("utf-8"),
```

### Comparing `talus-1.0.0rc6/talus/tests/models/test_processor.py` & `talus-1.0.0rc7/talus/tests/models/test_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 
     class SuccessfulMessageProcessor(MessageProcessorBase):
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
 
         def process_message(self, message: ConsumeMessageBase):
             self._message_was_processed = True
 
-    with SuccessfulMessageProcessor() as processor:
-        yield processor
+    yield SuccessfulMessageProcessor()
 
 
 @pytest.fixture()
 def consumed_message(
     publish_message_cls,
     producer,
     consumer,
@@ -71,16 +70,15 @@
     class ErroringMessageProcessor(MessageProcessorBase):
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
         dead_letter_exceptions: Type[Exception] = ValueError
 
         def process_message(self, message: ConsumeMessageBase):
             raise RuntimeError("A bad message processor raised an exception that is not DLQ'd.")
 
-    with ErroringMessageProcessor() as processor:
-        yield processor
+    yield ErroringMessageProcessor()
 
 
 def test_message_processor_failure(erroring_message_processor, consumed_message, consumer):
     """
     :given: A message processor that raises an exception.
     :when: The message processor is called.
     :then: Expected exception is raised.
@@ -104,16 +102,15 @@
         message_cls: Type[ConsumeMessageBase] = consume_message_cls
         dead_letter_exceptions: Type[Exception] = RuntimeError
 
         def process_message(self, message: ConsumeMessageBase):
             self._raised_run_time_error = True
             raise RuntimeError("A bad message processor raised an exception that is DLQ'd.")
 
-    with AutoDLQMessageProcessor() as processor:
-        yield processor
+    yield AutoDLQMessageProcessor()
 
 
 def test_dlq_message_processor(dlq_message_processor, consumed_message, consumer):
     """
     :given: A message processor that raises an exception identified as for DLQ.
     :when: The message processor is called.
     :then: The message processor should DLQ the message.
@@ -192,31 +189,7 @@
         message_cls: Type[ConsumeMessageBase] = ConsumeMessageBase
         producer: DurableProducer = Field(default_factory=lambda: durable_producer)
 
         def process_message(self, message: ConsumeMessageBase):
             pass
 
     return MessageProcessorWithProducer
-
-
-@pytest.mark.parametrize(
-    "connect_producer",
-    [
-        pytest.param(True, id="connect_producer"),
-        pytest.param(False, id="no_connect_producer"),
-    ],
-)
-def test_message_processor_producer_disconnect(
-    message_processor_cls_with_producer, producer, connect_producer
-):
-    """
-    :given: A message processor that has a producer.
-    :when: The message processor is exited.
-    :then: The producer should be disconnected.
-    """
-    # given
-    with message_processor_cls_with_producer() as processor:
-        # when
-        if connect_producer:
-            processor.producer.connect()
-    # then
-    assert producer.connection.is_closed
```

### Comparing `talus-1.0.0rc6/talus/tests/models/test_queue.py` & `talus-1.0.0rc7/talus/tests/models/test_queue.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus/tests/models/test_retryer.py` & `talus-1.0.0rc7/talus/tests/models/test_retryer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus/tests/test_base.py` & `talus-1.0.0rc7/talus/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus/tests/test_consumer.py` & `talus-1.0.0rc7/talus/tests/test_consumer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus/tests/test_producer.py` & `talus-1.0.0rc7/talus/tests/test_producer.py`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/talus.egg-info/SOURCES.txt` & `talus-1.0.0rc7/talus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `talus-1.0.0rc6/tox.ini` & `talus-1.0.0rc7/tox.ini`

 * *Files identical despite different names*

