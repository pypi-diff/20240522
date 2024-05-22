# Comparing `tmp/soarca_fin_library-0.0.1rc5.tar.gz` & `tmp/soarca_fin_library-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soarca_fin_library-0.0.1rc5.tar", max compression
+gzip compressed data, was "soarca_fin_library-1.0.0.tar", max compression
```

## Comparing `soarca_fin_library-0.0.1rc5.tar` & `soarca_fin_library-1.0.0.tar`

### file list

```diff
@@ -1,42 +1,40 @@
--rw-r--r--   0        0        0    11332 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/LICENSE
--rw-r--r--   0        0        0     2066 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/README.md
--rw-r--r--   0        0        0      735 2024-04-02 13:24:59.411511 soarca_fin_library-0.0.1rc5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/__init__.py
--rw-r--r--   0        0        0      211 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_executor.py
--rw-r--r--   0        0        0      671 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_mqtt_client.py
--rw-r--r--   0        0        0      255 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_parser.py
--rw-r--r--   0        0        0      469 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_soarca_fin.py
--rw-r--r--   0        0        0        0 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/__init__.py
--rw-r--r--   0        0        0      120 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/ack_status_enum.py
--rw-r--r--   0        0        0      134 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/auth_type_enum.py
--rw-r--r--   0        0        0      101 2024-04-02 13:24:34.935340 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/dispatcher_task_enum.py
--rw-r--r--   0        0        0      102 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/timeout_status_enum.py
--rw-r--r--   0        0        0      411 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/variable_type_enum.py
--rw-r--r--   0        0        0      298 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/enums/workflow_step_enum.py
--rw-r--r--   0        0        0     9098 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/executor.py
--rw-r--r--   0        0        0     2835 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/main.py
--rw-r--r--   0        0        0     7488 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/message_factory.py
--rw-r--r--   0        0        0        0 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/__init__.py
--rw-r--r--   0        0        0      152 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/ack.py
--rw-r--r--   0        0        0      109 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/agent_structure.py
--rw-r--r--   0        0        0      601 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/authentication_information.py
--rw-r--r--   0        0        0      464 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/capability_structure.py
--rw-r--r--   0        0        0      349 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/command.py
--rw-r--r--   0        0        0      475 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/command_sub_structure.py
--rw-r--r--   0        0        0      259 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/context.py
--rw-r--r--   0        0        0      289 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/external_reference.py
--rw-r--r--   0        0        0       93 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/message.py
--rw-r--r--   0        0        0       93 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/meta.py
--rw-r--r--   0        0        0      153 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/nack.py
--rw-r--r--   0        0        0      489 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/register.py
--rw-r--r--   0        0        0      333 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/result.py
--rw-r--r--   0        0        0      262 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/result_structure.py
--rw-r--r--   0        0        0      102 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/security.py
--rw-r--r--   0        0        0      283 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/step_structure.py
--rw-r--r--   0        0        0      288 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/unregister.py
--rw-r--r--   0        0        0      112 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/unregister_self.py
--rw-r--r--   0        0        0      256 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/variable.py
--rw-r--r--   0        0        0     2832 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/mqtt_client.py
--rw-r--r--   0        0        0     2466 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/parser.py
--rw-r--r--   0        0        0     5626 2024-04-02 13:24:34.939339 soarca_fin_library-0.0.1rc5/soarca_fin_python_library/soarca_fin.py
--rw-r--r--   0        0        0     2717 1970-01-01 00:00:00.000000 soarca_fin_library-0.0.1rc5/PKG-INFO
+-rw-r--r--   0        0        0    11332 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2588 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/README.md
+-rw-r--r--   0        0        0      729 2024-05-22 07:53:38.221860 soarca_fin_library-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/abstract_classes/i_executor.py
+-rw-r--r--   0        0        0      671 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/abstract_classes/i_mqtt_client.py
+-rw-r--r--   0        0        0      255 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/abstract_classes/i_parser.py
+-rw-r--r--   0        0        0      469 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/abstract_classes/i_soarca_fin.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/ack_status_enum.py
+-rw-r--r--   0        0        0      134 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/auth_type_enum.py
+-rw-r--r--   0        0        0      101 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/dispatcher_task_enum.py
+-rw-r--r--   0        0        0      102 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/timeout_status_enum.py
+-rw-r--r--   0        0        0      411 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/variable_type_enum.py
+-rw-r--r--   0        0        0      298 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/enums/workflow_step_enum.py
+-rw-r--r--   0        0        0     9508 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/executor.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/ack.py
+-rw-r--r--   0        0        0      109 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/agent_structure.py
+-rw-r--r--   0        0        0      601 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/authentication_information.py
+-rw-r--r--   0        0        0      464 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/capability_structure.py
+-rw-r--r--   0        0        0      349 2024-05-22 07:53:26.169699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/command.py
+-rw-r--r--   0        0        0      475 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/command_sub_structure.py
+-rw-r--r--   0        0        0      259 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/context.py
+-rw-r--r--   0        0        0      289 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/external_reference.py
+-rw-r--r--   0        0        0       93 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/message.py
+-rw-r--r--   0        0        0       93 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/meta.py
+-rw-r--r--   0        0        0      153 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/nack.py
+-rw-r--r--   0        0        0      489 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/register.py
+-rw-r--r--   0        0        0      333 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/result.py
+-rw-r--r--   0        0        0      262 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/result_structure.py
+-rw-r--r--   0        0        0      102 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/security.py
+-rw-r--r--   0        0        0      289 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/step_structure.py
+-rw-r--r--   0        0        0      288 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/unregister.py
+-rw-r--r--   0        0        0      112 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/unregister_self.py
+-rw-r--r--   0        0        0      256 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/models/variable.py
+-rw-r--r--   0        0        0     2908 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/mqtt_client.py
+-rw-r--r--   0        0        0     2480 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/parser.py
+-rw-r--r--   0        0        0     5632 2024-05-22 07:53:26.173699 soarca_fin_library-1.0.0/soarca_fin_python_library/soarca_fin.py
+-rw-r--r--   0        0        0     3236 1970-01-01 00:00:00.000000 soarca_fin_library-1.0.0/PKG-INFO
```

### Comparing `soarca_fin_library-0.0.1rc5/LICENSE` & `soarca_fin_library-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1rc5/pyproject.toml` & `soarca_fin_library-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soarca-fin-library"
-version = "0.0.1-pre.5"
+version = "1.0.0"
 description = "SOARCA FIN lib allows for extending custom SOARCA capabilities through a python library"
 authors = ["Maarten de Kruijf","RabbITCybErSeC","xncz8h (Ivo)"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [{include = "soarca_fin_python_library"}]
  
 [tool.poetry-dynamic-versioning]
```

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/abstract_classes/i_mqtt_client.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/abstract_classes/i_mqtt_client.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/executor.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 from soarca_fin_python_library.models.unregister_self import UnregisterSelf
 from soarca_fin_python_library.models.result_structure import ResultStructure
 from soarca_fin_python_library.models.meta import Meta
 
 
 class Executor(IExecutor):
 
-    def __init__(self, id: str, callback, queue: Queue, mqttc: Client):
+    def __init__(self, executor_id: str, callback, queue: Queue, mqttc: Client):
         self.queue: Queue[Message] = queue
         self.mqttc: Client = mqttc
         self.acks: list[str] = []
-        self.id = id
+        self.id = executor_id
         self.callback = callback
         self.TIMEOUT = 30
         self.running = True
 
     # Add message to queue.
     def queue_message(self, message: Message) -> None:
         self.queue.put(message)
@@ -38,45 +38,45 @@
     # Stop the executor by stoping the queue polling.
     def stop_executor(self):
         self.running = False
 
     # Main executor loop. Polls for messages in the queue and parsers them.
     def start_executor(self):
 
-        log.info(f"Thread started for {self.id}")
+        log.info("Thread started for %s", self.id)
         self.running = True
 
         while self.running:
             try:
                 # This method is blocking
                 message = self._get_message_from_queue(timeout=10)
                 match message:
                     case Ack() | Nack():
                         # Check if we are expecting this (n)ack
                         if message.message_id in self.acks:
                             self._put_message_in_queue(message)
                         else:
                             log.debug(
-                                f"Received unknown (n)ack with message_id: {message.message_id}")
+                                "Received unknown (n)ack with message_id: %s", message.message_id)
                     case Register():
                         self._handle_register_message(message)
                     case Unregister():
                         self._handle_unregister_message(message)
                     case UnregisterSelf():
                         self._handle_unregister_self_message(message)
                     case Command():
                         self._handle_command_message(message)
                     case _:
                         # Send Nack?
-                        log.warn(
-                            f"Unimplemented command: {message.model_dump_json()}")
-            except Empty as e:
+                        log.warning(
+                            "Unimplemented command: %s", message.model_dump_json())
+            except Empty:
                 pass
 
-        log.info(f"Thread ended for {self.id}")
+        log.info("Thread ended for %s", self.id)
 
     # Gets message form queue. Is blocking.
     def _get_message_from_queue(self, timeout: float = None) -> Message:
         return self.queue.get(timeout=timeout)
 
     # Helper functtion to put messages in the queue with a timeout.
     def _put_message_in_queue(self, message: Message, timeout: float = None):
@@ -102,22 +102,24 @@
         retries = 3
         while retries > 0:
             try:
                 self._wait_for_ack(message.message_id)
                 self.callback(message)
                 return
             except (Empty, TimeoutError) as e:
+                log.debug(e)
                 self._send_message_as_json(message, topic="soarca")
             except RuntimeError as e:
+                log.debug(e)
                 self._send_message_as_json(message, topic="soarca")
             finally:
                 retries -= 1
                 if retries == 0:
-                    log.error(
-                        f"Did not receive an ack for message {message.message_id}. Aborting...")
+                    log.fatal(
+                        "Did not receive an ack for message %s. Aborting...", message.message_id)
                     exit(-1)
 
     # Handles self generated register message.
     # First sends a register message, then waits for acks.
     # If there is no successful acknowledgement, exit.
     def _handle_register_message(self, message: Register):
         # Send command message to soarca
@@ -128,26 +130,28 @@
         while retries > 0:
             try:
                 # Send Ack and wait for a response
                 self._wait_for_ack(message.message_id)
                 return
             # Did not get a response in time
             except (Empty, TimeoutError) as e:
+                log.debug(e)
                 # Resend message
                 self._send_message_as_json(message, topic="soarca")
 
             # Receive a response but the message failed (Nack)
-            except RuntimeError as e:
+            except RuntimeError:
+                log.debug(e)
                 # Resend message
                 self._send_message_as_json(message, topic="soarca")
             finally:
                 retries -= 1
                 if retries == 0:
-                    log.error(
-                        f"Did not receive an ack for message {message.message_id}. Aborting...")
+                    log.fatal(
+                        "Did not receive an ack for message %s. Aborting...", message.message_id)
                     exit(-1)
 
     # Handles a command message from SOARCA.
     # First sends an acknowledgement back, then calls capability callback function with the command as argument.
     # Callback should return a result.
     # Send result back to SOARCA and wait for an acknowledgement
     def _handle_command_message(self, message: Command):
@@ -169,21 +173,26 @@
         # Wait for ack
         retries = 3
         while retries > 0:
             try:
                 self._wait_for_ack(result.message_id)
                 break
             except (Empty, TimeoutError) as e:
+                log.debug(e)
                 self._send_message_as_json(result)
             except RuntimeError as e:
+                log.debug(e)
                 self._send_message_as_json(result)
             finally:
                 retries -= 1
-                if retries == 0:
-                    break
+            if retries == 0:
+                self.acks.remove(message_id)
+                log.error(
+                    "Did not receive an acknowledgement for message %s. Skipping message...", result.message_id)
+                break
 
     # Publishes a message as JSON on a topic. Default topic is self.id.
     def _send_message_as_json(self, message: Message, topic: str = None):
         json_message = message.model_dump_json()
         if topic:
             self.mqttc.publish(topic, payload=json_message)
         else:
@@ -205,21 +214,22 @@
 
                     message = self._get_message_from_queue(timeout=timeout)
 
                 # Notify executor that we received ack
                 self.acks.remove(message_id)
                 match message:
                     case Ack():
-                        log.info(f"Receive ack for message {message_id}")
+                        log.info("Received ack for message: %s", message_id)
                         return
                     case Nack():
-                        log.warn(f"Receive nack for message {message_id}")
-                        raise RuntimeError("Receive a nack")
+                        log.warning(
+                            "Received nack for message: %s", message_id)
+                        raise RuntimeError("Received a nack")
                     case _:
                         raise TypeError(
                             f"Unexpected message type {message.model_dump_json()}")
 
             except Empty as e:
-                log.warn("Did not receive an ack")
+                log.warning("Did not receive an ack")
                 raise e
 
         raise TimeoutError(f"Timeout for message with id {message_id}")
```

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/models/authentication_information.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/models/authentication_information.py`

 * *Files identical despite different names*

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/mqtt_client.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/mqtt_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from json import JSONDecodeError
 import threading
 import logging as log
 from paho.mqtt.client import Client, ConnectFlags, MQTTMessage
 from paho.mqtt.properties import Properties
 from paho.mqtt.reasoncodes import ReasonCode
 import paho.mqtt.client as mqtt
 from paho.mqtt.subscribeoptions import SubscribeOptions
@@ -12,25 +13,25 @@
 from soarca_fin_python_library.executor import Executor
 
 
 class MQTTClient(IMQTTClient):
 
     def __init__(
             self,
-            id: str,
+            client_id: str,
             mqttc: mqtt.Client,
             callback,
             executor: IExecutor,
             parser: IParser):
-        self.id: str = id
+        self.id: str = client_id
         self.mqttc: mqtt.Client = mqttc
         self.callback = callback
         self.executor: Executor = executor
         self.parser = parser
-        self._executor_thread = None
+        self.executor_thread = None
 
     # On connect callback function for Paho MQTT client
     def on_connect(
             self,
             client: Client,
             userdata,
             connect_flags: ConnectFlags,
@@ -42,16 +43,16 @@
     def on_message(self, client: Client, userdata, message: MQTTMessage):
         try:
             # Parse message to check message type
             msg = self.parser.parse_on_message(message)
             # If we should process the message, send it to the executor
             if msg:
                 self.executor.queue_message(msg)
-        except Exception as e:
-            log.error(f"Something went wrong when parsing messag:\n{e}")
+        except (LookupError, JSONDecodeError, TypeError) as e:
+            log.error("Something went wrong when parsing messag:\n%s", e)
 
     # Start the MQTT client by registering mqtt callbacks, subscribing to
     # topic and launching executor
     def start(self):
         # Set mqttc callback functions
         self.mqttc.on_connect = self.on_connect
         self.mqttc.on_message = self.on_message
@@ -61,20 +62,20 @@
         self.mqttc.subscribe(
             self.id, options=SubscribeOptions(qos=1, noLocal=True))
 
         # Start callback loops for mqtt in the background
         self.mqttc.loop_start()
 
         # Start executor thread
-        self._executor_thread = threading.Thread(
+        self.executor_thread = threading.Thread(
             target=self.executor.start_executor,
             name=f"executor-thread-{self.id}")
-        self._executor_thread.daemon = True
+        self.executor_thread.daemon = True
 
-        self._executor_thread.start()
+        self.executor_thread.start()
 
     # Stop MQTT client by unsubscribing, stopping mqtt callbacks and exiting
     # executor
     def stop(self):
         self.mqttc.unsubscribe(self.id)
         self.mqttc.loop_stop()
         self.executor.stop_executor()
```

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/parser.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 from soarca_fin_python_library.models.command import Command
 
 # Parser class to convert MQTT messages to Fin protocol messages.
 
 
 class Parser(IParser):
 
-    def __init__(self, id: str):
-        self.id = id
+    def __init__(self, parser_id: str):
+        self.id = parser_id
 
     def parse_on_message(self, message: mqtt.MQTTMessage) -> Message:
         # Check if we did not receive an empty MQTT message.
         if not message.payload:
-            log.error(f"Received a message with an empty payload")
+            log.error("Received a message with an empty payload")
             raise LookupError("Could not receive payload from message")
         content = ""
         # Try to convert MQTT payload to utf8 and load is as a JSON object.
         try:
             content = json.loads(message.payload.decode('utf8'))
         except Exception as e:
-            log.error(f"Could not parse the payload as json format: {e}")
+            log.error("Could not parse the payload as json format: %s", e)
             raise e
         # Check for attribute 'type'. Is required to parse the message further.
         if "type" not in content:
             log.error("Error, no message type found in payload")
             raise LookupError("No type attribute in payload")
 
         # Check for attribute 'message_id'. Is required for a valid message.
```

### Comparing `soarca_fin_library-0.0.1rc5/soarca_fin_python_library/soarca_fin.py` & `soarca_fin_library-1.0.0/soarca_fin_python_library/soarca_fin.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,33 +78,33 @@
 
         # Start the control fin
         self.fin.start()
 
         # Send register message to the MQTT broker
         register_msg = self._create_register_message()
         self.fin.executor.queue_message(register_msg)
-        self.fin._executor_thread.join()
+        self.fin.executor_thread.join()
 
     # Callback function for the control fin such that is can control the
     # capability fins
     def fin_control_callback(self, message: Message):
         match message:
             case Unregister() | UnregisterSelf():
                 if message.all or message.fin_id == self.fin:
                     for capability in self.capabilities.values():
                         capability.stop()
                     self.fin.stop()
-                    log.warn("Stopping in 10 seconds...")
+                    log.warning("Stopping in 10 seconds...")
                     time.sleep(10)
                 elif message.capability_id in self.capabilities:
                     self.capabilities[message.capability_id].stop()
                     del self.capabilities[message.capability_id]
                     del self.capability_structure[message.capability_id]
-                    log.warn(
-                        f"Stopping capability with id {message.capability_id} in 10 seconds...")
+                    log.warning(
+                        "Stopping capability with id %s in 10 seconds...", message.capability_id)
                     time.sleep(10)
                 else:
                     log.debug("Unregister not for this fin")
             case _:
                 log.error("Unknown message")
 
     # Helper function to generate a register message from  registered
```

