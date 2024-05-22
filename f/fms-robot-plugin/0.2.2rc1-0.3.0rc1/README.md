# Comparing `tmp/fms_robot_plugin-0.2.2rc1.tar.gz` & `tmp/fms_robot_plugin-0.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.2.2rc1.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.3.0rc1.tar", max compression
```

## Comparing `fms_robot_plugin-0.2.2rc1.tar` & `fms_robot_plugin-0.3.0rc1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2024-05-07 04:30:33.640619 fms_robot_plugin-0.2.2rc1/README.md
--rw-r--r--   0        0        0       49 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1485 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/constants.py
--rw-r--r--   0        0        0     1824 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     8909 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3168 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc1/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc1/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-22 02:55:07.504226 fms_robot_plugin-0.3.0rc1/README.md
+-rw-r--r--   0        0        0       49 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/constants.py
+-rw-r--r--   0        0        0     1824 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     9461 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3328 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc1/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc1/PKG-INFO
```

### Comparing `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/constants.py` & `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     on_unload_map = "on_unload_map"
     on_execute_task = "on_execute_task"
     on_resume_task = "on_resume_task"
     on_pause_task = "on_pause_task"
     on_set_priority = "on_set_priority"
     on_robot_info = "on_robot_info"
     on_preview_map = "on_preview_map"
+    on_acquire_lock_response = "on_acquire_lock_response"
 
     # Publisher
     set_camera_feed = "set_camera_feed"
     set_lidar = "set_lidar"
     set_pose = "set_pose"
     set_map_data = "set_map_data"
     set_status = "set_status"
@@ -34,7 +35,8 @@
     set_memory_usage = "set_memory_usage"
     set_battery_usage = "set_battery_usage"
     set_robot_info = "set_robot_info"
     set_decimated_plan = "set_decimated_plan"
     set_result = "set_result"
     set_obstacle_notification = "set_obstacle_notification"
     set_notification_message = "set_notification_message"
+    set_acquire_lock_request = "set_acquire_lock_request"
```

### Comparing `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
     Twist,
     Pose,
     Map,
     RobotInfo,
     Task,
     DecimatedPlan,
     Result,
+    AcquireLockRequest,
+    AcquireLockResponse,
 )
 from fms_robot_plugin.mqtt import MqttClient, MqttConsumer
 
 
 class Robot:
     robot_key: Optional[str]
 
@@ -34,14 +36,15 @@
         capabilities: List[str] = [],
     ):
         self.plugin_name = plugin_name
         self.plugin_version = plugin_version
         self.capabilities = capabilities
         self.robot_key = robot_key
         self.priority: int = 0
+        self.acquire_lock_message_id: Optional[str] = None
 
         self.api_hostname = api_hostname
         self.broker_host = broker_host
         self.broker_port = broker_port
         self.mqtt = MqttClient(broker_host, broker_port)
 
     def run(self):
@@ -114,14 +117,18 @@
         topic = f"robots/{self.robot_key}/info/receive"
         self.consumer(topic).consume(lambda data: cb(RobotInfo(**data)))
 
     def on_preview_map(self, cb: Callable[[], None]):
         topic = f"robots/{self.robot_key}/mapping/import"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
+    def on_acquire_lock_response(self, cb: Callable[[AcquireLockResponse], None]):
+        topic = f"robots/{self.robot_key}/locks/acquire/response"
+        self.consumer(topic).consume(lambda data: cb(AcquireLockResponse(**data)))
+
     """
     Publishers
 
     These methods are called to publish data to the FMS server.
     """
 
     def set_camera_feed(self, data: str):
@@ -192,14 +199,18 @@
 
     def set_obstacle_notification(self, data: bool):
         self.mqtt.publish(f"robots/{self.robot_key}/obstacle", data, serialize=False)
 
     def set_notification_message(self, data: str):
         self.mqtt.publish(f"robots/{self.robot_key}/notification", data, serialize=False)
 
+    def set_acquire_lock_request(self, data: AcquireLockRequest):
+        self.acquire_lock_message_id = data.message_id
+        self.mqtt.publish(f"robots/{self.robot_key}/locks/acquire/request", data.dict())
+
     """
     Utilities
     """
 
     def consumer(self, topic: str):
         return MqttConsumer(topic, self.broker_host, self.broker_port)
```

### Comparing `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/typings.py`

 * *Files 5% similar despite different names*

```diff
@@ -180,7 +180,17 @@
 
     status: StatusResponse
     result: ResultResponse
 
 
 class CheckMap(BaseModel):
     uids: List[str]
+
+
+class AcquireLockRequest(BaseModel):
+    message_id: str
+    node_ids: List[str]
+
+
+class AcquireLockResponse(BaseModel):
+    message_id: str
+    result: bool
```

### Comparing `fms_robot_plugin-0.2.2rc1/pyproject.toml` & `fms_robot_plugin-0.3.0rc1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.2.2rc1"
+version = "0.3.0rc1"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.2.2rc1/setup.py` & `fms_robot_plugin-0.3.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.2.2rc1',
+    'version': '0.3.0rc1',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

