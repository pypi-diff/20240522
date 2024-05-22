# Comparing `tmp/fms_robot_plugin-0.3.0rc1.tar.gz` & `tmp/fms_robot_plugin-0.3.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fms_robot_plugin-0.3.0rc1.tar", max compression
+gzip compressed data, was "fms_robot_plugin-0.3.0rc2.tar", max compression
```

## Comparing `fms_robot_plugin-0.3.0rc1.tar` & `fms_robot_plugin-0.3.0rc2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       26 2024-05-22 02:55:07.504226 fms_robot_plugin-0.3.0rc1/README.md
--rw-r--r--   0        0        0       49 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/__init__.py
--rw-r--r--   0        0        0     1601 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/constants.py
--rw-r--r--   0        0        0     1824 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/mqtt.py
--rw-r--r--   0        0        0     9461 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/robot.py
--rw-r--r--   0        0        0     3328 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/fms_robot_plugin/typings.py
--rw-r--r--   0        0        0      657 2024-05-22 02:55:07.508226 fms_robot_plugin-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc1/setup.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       26 2024-05-22 04:48:23.944060 fms_robot_plugin-0.3.0rc2/README.md
+-rw-r--r--   0        0        0       49 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/fms_robot_plugin/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/fms_robot_plugin/constants.py
+-rw-r--r--   0        0        0     1824 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/fms_robot_plugin/mqtt.py
+-rw-r--r--   0        0        0     9461 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/fms_robot_plugin/robot.py
+-rw-r--r--   0        0        0     3468 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/fms_robot_plugin/typings.py
+-rw-r--r--   0        0        0      657 2024-05-22 04:48:23.948060 fms_robot_plugin-0.3.0rc2/pyproject.toml
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc2/setup.py
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 fms_robot_plugin-0.3.0rc2/PKG-INFO
```

### Comparing `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/constants.py` & `fms_robot_plugin-0.3.0rc2/fms_robot_plugin/constants.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/mqtt.py` & `fms_robot_plugin-0.3.0rc2/fms_robot_plugin/mqtt.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/robot.py` & `fms_robot_plugin-0.3.0rc2/fms_robot_plugin/robot.py`

 * *Files identical despite different names*

### Comparing `fms_robot_plugin-0.3.0rc1/fms_robot_plugin/typings.py` & `fms_robot_plugin-0.3.0rc2/fms_robot_plugin/typings.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 class TaskType(str, enum.Enum):
     """
     Possible types of tasks in FMS2
     """
 
     Waypoint = "WAYPOINT"
+    WaypointTraffic = "WAYPOINT_TRAFFIC"
     CustomTask = "CUSTOM_TASK"
     AuxTask = "AUX_TASK"
     DynamicTask = "DYNAMIC_TASK"
 
 
 class ConnectionStatus(str, enum.Enum):
     """
@@ -140,22 +141,27 @@
     velocity_covariance: List[float]
 
 
 class Waypoint(BaseModel):
     poses: List[Pose]
 
 
+class WaypointTraffic(BaseModel):
+    poses: List[Pose]
+    node_ids: List[str]
+
+
 class DynamicTask(BaseModel):
     payloads: List[dict]
 
 
 class Task(BaseModel):
     id: str
     type: TaskType
-    data: Union[Waypoint, DynamicTask, dict]
+    data: Union[Waypoint, WaypointTraffic, DynamicTask, dict]
     map_id: str
     linear_velocity: Optional[float] = None
     angular_velocity: Optional[float] = None
 
 
 class DecimatedPlan(BaseModel):
     poses: List[Pose]
```

### Comparing `fms_robot_plugin-0.3.0rc1/pyproject.toml` & `fms_robot_plugin-0.3.0rc2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fms-robot-plugin"
-version = "0.3.0rc1"
+version = "0.3.0rc2"
 description = ""
 authors = [
   "Dionesius Agung <dionesius@movel.ai>",
   "Steven Hansel <steven@movel.ai>"
 ]
 readme = "README.md"
 packages = [{include = "fms_robot_plugin"}]
```

### Comparing `fms_robot_plugin-0.3.0rc1/setup.py` & `fms_robot_plugin-0.3.0rc2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['paho-mqtt>=1.6.1,<2.0.0', 'pydantic>=2.3.0,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'fms-robot-plugin',
-    'version': '0.3.0rc1',
+    'version': '0.3.0rc2',
     'description': '',
     'long_description': '# FMS Robot Plugin Library',
     'author': 'Dionesius Agung',
     'author_email': 'dionesius@movel.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

