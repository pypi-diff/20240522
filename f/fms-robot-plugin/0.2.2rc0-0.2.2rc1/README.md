# Comparing `tmp/fms_robot_plugin-0.2.2rc0.tar.gz` & `tmp/fms_robot_plugin-0.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.2.2rc0.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.2.2rc1.tar", max compression
```

## Comparing `fms_robot_plugin-0.2.2rc0.tar` & `fms_robot_plugin-0.2.2rc1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       26 2024-04-12 08:08:58.136799 fms_robot_plugin-0.2.2rc0/README.md
--rw-r--r--   0        0        0       49 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     8727 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3168 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-04-12 08:08:58.140799 fms_robot_plugin-0.2.2rc0/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc0/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-07 04:30:33.640619 fms_robot_plugin-0.2.2rc1/README.md
+-rw-r--r--   0        0        0       49 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1485 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/constants.py
+-rw-r--r--   0        0        0     1824 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     8909 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3168 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-05-07 04:30:33.644619 fms_robot_plugin-0.2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc1/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.2.2rc1/PKG-INFO
```

### Comparing `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/robot.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,17 +27,19 @@
         self,
         plugin_name: str,
         plugin_version: str,
         robot_key: str,
         broker_host: str = "broker.movelrobotics.com",
         broker_port: int = 1883,
         api_hostname: str = "api.movelrobotics.com",
+        capabilities: List[str] = [],
     ):
         self.plugin_name = plugin_name
         self.plugin_version = plugin_version
+        self.capabilities = capabilities
         self.robot_key = robot_key
         self.priority: int = 0
 
         self.api_hostname = api_hostname
         self.broker_host = broker_host
         self.broker_port = broker_port
         self.mqtt = MqttClient(broker_host, broker_port)
@@ -68,28 +70,28 @@
         topic = f"robots/{self.robot_key}/mapping/save"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
     def on_localize(self, cb: Callable[[str, Pose], None]):
         topic = f"robots/{self.robot_key}/localize"
         self.consumer(topic).consume(lambda data: cb(data["map_id"], Pose(**data["initial_pose"])))
 
-    def on_load_map_pgm(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/pgm"
+    def on_load_navigation_map_pgm(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/navigation_pgm"
         self.consumer(topic).consume(lambda pgm, url_params: cb(pgm, url_params["map_id"]), serialize=False)
 
-    def on_load_map_yaml(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/yaml"
+    def on_load_navigation_map_yaml(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/navigation_yaml"
         self.consumer(topic).consume(lambda yaml, url_params: cb(yaml, url_params["map_id"]), serialize=False)
 
-    def on_load_map_localization_pgm(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization/pgm"
+    def on_load_localization_map_pgm(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization_pgm"
         self.consumer(topic).consume(lambda pgm, url_params: cb(pgm, url_params["map_id"]), serialize=False)
 
-    def on_load_map_localization_yaml(self, cb: Callable[[bytes, str], None]):
-        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization/yaml"
+    def on_load_localization_map_yaml(self, cb: Callable[[bytes, str], None]):
+        topic = f"robots/{self.robot_key}/maps/:map_id/load/localization_yaml"
         self.consumer(topic).consume(lambda yaml, url_params: cb(yaml, url_params["map_id"]), serialize=False)
 
     def on_unload_map(self, cb: Callable[[], None]):
         topic = f"robots/{self.robot_key}/maps/unload"
         self.consumer(topic).consume(lambda _: cb(), serialize=False)
 
     def on_execute_task(self, cb: Callable[[Task], None]):
@@ -216,14 +218,15 @@
                 connection_topic,
                 payload=json.dumps(
                     {
                         "status": ConnectionStatus.Connected.value,
                         "sent_at": datetime.datetime.utcnow().isoformat(),
                         "name": self.plugin_name,
                         "version": self.plugin_version,
+                        "capabilities": self.capabilities,
                     }
                 ),
             )
 
         client.on_connect = on_connect
         client.will_set(
             connection_topic,
```

### Comparing `fms_robot_plugin-0.2.2rc0/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.2.2rc1/fms_robot_plugin/typings.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.2.2rc0/pyproject.toml` & `fms_robot_plugin-0.2.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.2.2rc0"
+version = "0.2.2rc1"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.2.2rc0/setup.py` & `fms_robot_plugin-0.2.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.2.2rc0',
+    'version': '0.2.2rc1',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

