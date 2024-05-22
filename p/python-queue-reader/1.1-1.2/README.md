# Comparing `tmp/python_queue_reader-1.1.tar.gz` & `tmp/python_queue_reader-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_queue_reader-1.1.tar", last modified: Wed May 22 19:12:21 2024, max compression
+gzip compressed data, was "python_queue_reader-1.2.tar", last modified: Wed May 22 19:25:24 2024, max compression
```

## Comparing `python_queue_reader-1.1.tar` & `python_queue_reader-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:12:21.474477 python_queue_reader-1.1/
--rw-r--r--   0 glenn      (502) staff       (20)     4602 2024-05-22 19:12:21.474024 python_queue_reader-1.1/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)     4336 2024-05-22 13:37:08.000000 python_queue_reader-1.1/README.md
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:12:21.471373 python_queue_reader-1.1/python_queue_reader/
--rw-r--r--   0 glenn      (502) staff       (20)    13285 2024-05-22 17:25:21.000000 python_queue_reader-1.1/python_queue_reader/MessageBrokers.py
--rw-r--r--   0 glenn      (502) staff       (20)       17 2024-05-22 18:34:06.000000 python_queue_reader-1.1/python_queue_reader/__init__.py
-drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:12:21.473623 python_queue_reader-1.1/python_queue_reader.egg-info/
--rw-r--r--   0 glenn      (502) staff       (20)     4602 2024-05-22 19:12:21.000000 python_queue_reader-1.1/python_queue_reader.egg-info/PKG-INFO
--rw-r--r--   0 glenn      (502) staff       (20)      302 2024-05-22 19:12:21.000000 python_queue_reader-1.1/python_queue_reader.egg-info/SOURCES.txt
--rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-22 19:12:21.000000 python_queue_reader-1.1/python_queue_reader.egg-info/dependency_links.txt
--rw-r--r--   0 glenn      (502) staff       (20)      180 2024-05-22 19:12:21.000000 python_queue_reader-1.1/python_queue_reader.egg-info/requires.txt
--rw-r--r--   0 glenn      (502) staff       (20)       20 2024-05-22 19:12:21.000000 python_queue_reader-1.1/python_queue_reader.egg-info/top_level.txt
--rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-22 19:12:21.474651 python_queue_reader-1.1/setup.cfg
--rw-r--r--   0 glenn      (502) staff       (20)      483 2024-05-22 19:12:10.000000 python_queue_reader-1.1/setup.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:25:24.060199 python_queue_reader-1.2/
+-rw-r--r--   0 glenn      (502) staff       (20)     4733 2024-05-22 19:25:24.059955 python_queue_reader-1.2/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)     4467 2024-05-22 19:21:21.000000 python_queue_reader-1.2/README.md
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:25:24.057718 python_queue_reader-1.2/python_queue_reader/
+-rw-r--r--   0 glenn      (502) staff       (20)    13285 2024-05-22 17:25:21.000000 python_queue_reader-1.2/python_queue_reader/MessageBrokers.py
+-rw-r--r--   0 glenn      (502) staff       (20)       17 2024-05-22 18:34:06.000000 python_queue_reader-1.2/python_queue_reader/__init__.py
+drwxr-xr-x   0 glenn      (502) staff       (20)        0 2024-05-22 19:25:24.059606 python_queue_reader-1.2/python_queue_reader.egg-info/
+-rw-r--r--   0 glenn      (502) staff       (20)     4733 2024-05-22 19:25:24.000000 python_queue_reader-1.2/python_queue_reader.egg-info/PKG-INFO
+-rw-r--r--   0 glenn      (502) staff       (20)      302 2024-05-22 19:25:24.000000 python_queue_reader-1.2/python_queue_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 glenn      (502) staff       (20)        1 2024-05-22 19:25:24.000000 python_queue_reader-1.2/python_queue_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 glenn      (502) staff       (20)      180 2024-05-22 19:25:24.000000 python_queue_reader-1.2/python_queue_reader.egg-info/requires.txt
+-rw-r--r--   0 glenn      (502) staff       (20)       20 2024-05-22 19:25:24.000000 python_queue_reader-1.2/python_queue_reader.egg-info/top_level.txt
+-rw-r--r--   0 glenn      (502) staff       (20)       38 2024-05-22 19:25:24.060289 python_queue_reader-1.2/setup.cfg
+-rw-r--r--   0 glenn      (502) staff       (20)      483 2024-05-22 19:24:43.000000 python_queue_reader-1.2/setup.py
```

### Comparing `python_queue_reader-1.1/PKG-INFO` & `python_queue_reader-1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,26 @@
-Metadata-Version: 2.1
-Name: python_queue_reader
-Version: 1.1
-Summary: Queue reader for python abstracting message brokers such as RabbitMQ
-Home-page: UNKNOWN
-Author: uug.ai
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # MessageBrokers
 
 MessageBrokers is a Python library that provides a simple and efficient way to work with message brokers. It abstracts away the complexities of interacting with different message broker systems, allowing you to focus on writing your application logic.
 
 ## Installation
 To install MessageBrokers, you can use pip:
-...
+`pip install python_queue_reader`
+
+importing in python via:
+`from python_queue_reader import MessageBrokers`
 
 ## Example usage
 The code snippet provided demonstrates the usage of the MessageBrokers library in Python. It showcases how to initialize a connection to a message broker system, receive messages from a queue, send a message to the queue, and close the connection. The library abstracts away the complexities of interacting with different message broker systems, allowing developers to focus on writing their application logic. Let's dive into the details of each feature and method.
 
 ```
-from MessageBrokers import RabbitMQ
+from python_queue_reader import MessageBrokers
 
 # Initialize a connection to RabbitMQ message broker
-rabbitmq = RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
+rabbitmq = MessageBrokers.RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
 
 # Receive messages from the queue
 messages = rabbitmq.ReceiveMessages()
 
 for message in messages:
     # Process the received message
     print(f"Received message: {message}")
@@ -70,9 +62,7 @@
 This method takes a single parameter message, which is a string representing the content of the message you want to send. You can use this method to publish messages to the message broker system, allowing other applications or services to consume and process them.
 
 ### Close
 The `Close()` method is a part of the MessageBrokers library in Python. It is used to close the connection to the message broker system that you have initialized.
 
 After you have finished using the message broker system and no longer need to receive or send messages, you can call the `Close()` method to gracefully close the connection. This ensures that any resources used by the message broker system are properly released.
 
-
-
```

### Comparing `python_queue_reader-1.1/README.md` & `python_queue_reader-1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,37 @@
+Metadata-Version: 2.1
+Name: python_queue_reader
+Version: 1.2
+Summary: Queue reader for python abstracting message brokers such as RabbitMQ
+Home-page: UNKNOWN
+Author: uug.ai
+Author-email: 
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # MessageBrokers
 
 MessageBrokers is a Python library that provides a simple and efficient way to work with message brokers. It abstracts away the complexities of interacting with different message broker systems, allowing you to focus on writing your application logic.
 
 ## Installation
 To install MessageBrokers, you can use pip:
-...
+`pip install python_queue_reader`
+
+importing in python via:
+`from python_queue_reader import MessageBrokers`
 
 ## Example usage
 The code snippet provided demonstrates the usage of the MessageBrokers library in Python. It showcases how to initialize a connection to a message broker system, receive messages from a queue, send a message to the queue, and close the connection. The library abstracts away the complexities of interacting with different message broker systems, allowing developers to focus on writing their application logic. Let's dive into the details of each feature and method.
 
 ```
-from MessageBrokers import RabbitMQ
+from python_queue_reader import MessageBrokers
 
 # Initialize a connection to RabbitMQ message broker
-rabbitmq = RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
+rabbitmq = MessageBrokers.RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
 
 # Receive messages from the queue
 messages = rabbitmq.ReceiveMessages()
 
 for message in messages:
     # Process the received message
     print(f"Received message: {message}")
@@ -59,7 +73,9 @@
 This method takes a single parameter message, which is a string representing the content of the message you want to send. You can use this method to publish messages to the message broker system, allowing other applications or services to consume and process them.
 
 ### Close
 The `Close()` method is a part of the MessageBrokers library in Python. It is used to close the connection to the message broker system that you have initialized.
 
 After you have finished using the message broker system and no longer need to receive or send messages, you can call the `Close()` method to gracefully close the connection. This ensures that any resources used by the message broker system are properly released.
 
+
+
```

### Comparing `python_queue_reader-1.1/python_queue_reader/MessageBrokers.py` & `python_queue_reader-1.2/python_queue_reader/MessageBrokers.py`

 * *Files identical despite different names*

### Comparing `python_queue_reader-1.1/python_queue_reader.egg-info/PKG-INFO` & `python_queue_reader-1.2/python_queue_reader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: python-queue-reader
-Version: 1.1
+Version: 1.2
 Summary: Queue reader for python abstracting message brokers such as RabbitMQ
 Home-page: UNKNOWN
 Author: uug.ai
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # MessageBrokers
 
 MessageBrokers is a Python library that provides a simple and efficient way to work with message brokers. It abstracts away the complexities of interacting with different message broker systems, allowing you to focus on writing your application logic.
 
 ## Installation
 To install MessageBrokers, you can use pip:
-...
+`pip install python_queue_reader`
+
+importing in python via:
+`from python_queue_reader import MessageBrokers`
 
 ## Example usage
 The code snippet provided demonstrates the usage of the MessageBrokers library in Python. It showcases how to initialize a connection to a message broker system, receive messages from a queue, send a message to the queue, and close the connection. The library abstracts away the complexities of interacting with different message broker systems, allowing developers to focus on writing their application logic. Let's dive into the details of each feature and method.
 
 ```
-from MessageBrokers import RabbitMQ
+from python_queue_reader import MessageBrokers
 
 # Initialize a connection to RabbitMQ message broker
-rabbitmq = RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
+rabbitmq = MessageBrokers.RabbitMQ(queue_name='my_queue', target_queue_name = 'my_target_queue', exchange='my_exchange', host='host', username='guest', password='guest')
 
 # Receive messages from the queue
 messages = rabbitmq.ReceiveMessages()
 
 for message in messages:
     # Process the received message
     print(f"Received message: {message}")
```

