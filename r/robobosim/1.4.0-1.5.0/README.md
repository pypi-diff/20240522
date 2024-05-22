# Comparing `tmp/robobosim-1.4.0.tar.gz` & `tmp/robobosim-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robobosim-1.4.0.tar", last modified: Thu Nov  3 14:17:34 2022, max compression
+gzip compressed data, was "robobosim-1.5.0.tar", last modified: Wed May 22 14:38:36 2024, max compression
```

## Comparing `robobosim-1.4.0.tar` & `robobosim-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:34.004858 robobosim-1.4.0/
--rw-rw-rw-   0        0        0     7817 2022-04-06 09:00:47.000000 robobosim-1.4.0/LICENSE
--rw-rw-rw-   0        0        0     1524 2022-11-03 14:17:34.004858 robobosim-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2022-04-27 10:33:49.000000 robobosim-1.4.0/README.md
--rw-rw-rw-   0        0        0       42 2022-11-03 14:17:34.004858 robobosim-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1487 2022-11-03 14:08:01.000000 robobosim-1.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:33.986312 robobosim-1.4.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:33.992728 robobosim-1.4.0/src/robobosim/
--rw-rw-rw-   0        0        0     3562 2022-05-05 13:29:22.000000 robobosim-1.4.0/src/robobosim/RoboboSim.py
--rw-rw-rw-   0        0        0      210 2022-05-05 11:39:42.000000 robobosim-1.4.0/src/robobosim/State.py
--rw-rw-rw-   0        0        0        0 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:34.001704 robobosim-1.4.0/src/robobosim/processors/
--rw-rw-rw-   0        0        0     1313 2022-05-05 13:25:16.000000 robobosim-1.4.0/src/robobosim/processors/AGVProcessor.py
--rw-rw-rw-   0        0        0     1012 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/processors/AbstractProcessor.py
--rw-rw-rw-   0        0        0      482 2022-04-06 11:47:55.000000 robobosim-1.4.0/src/robobosim/processors/ControlProcessor.py
--rw-rw-rw-   0        0        0     1934 2022-05-05 11:40:18.000000 robobosim-1.4.0/src/robobosim/processors/LocationProcessor.py
--rw-rw-rw-   0        0        0        0 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/processors/__init__.py
--rw-rw-rw-   0        0        0     4399 2022-11-03 12:41:00.000000 robobosim-1.4.0/src/robobosim/remotelib.py
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:34.003859 robobosim-1.4.0/src/robobosim/utils/
--rw-rw-rw-   0        0        0      138 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/utils/ConnectionState.py
--rw-rw-rw-   0        0        0      919 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/utils/Message.py
--rw-rw-rw-   0        0        0        0 2022-04-06 09:00:47.000000 robobosim-1.4.0/src/robobosim/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 14:17:33.997713 robobosim-1.4.0/src/robobosim.egg-info/
--rw-rw-rw-   0        0        0     1524 2022-11-03 14:17:33.000000 robobosim-1.4.0/src/robobosim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      630 2022-11-03 14:17:33.000000 robobosim-1.4.0/src/robobosim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-03 14:17:33.000000 robobosim-1.4.0/src/robobosim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-11-03 14:17:33.000000 robobosim-1.4.0/src/robobosim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-03 14:17:33.000000 robobosim-1.4.0/src/robobosim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.036396 robobosim-1.5.0/
+-rw-rw-rw-   0        0        0     7817 2024-05-22 14:36:21.000000 robobosim-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0     1465 2024-05-22 14:38:36.033966 robobosim-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-22 14:36:21.000000 robobosim-1.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:38:36.036396 robobosim-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2024-05-22 14:36:21.000000 robobosim-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:35.971011 robobosim-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:35.985525 robobosim-1.5.0/src/robobosim/
+-rw-rw-rw-   0        0        0     5217 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/RoboboSim.py
+-rw-rw-rw-   0        0        0      246 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/State.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.024919 robobosim-1.5.0/src/robobosim/processors/
+-rw-rw-rw-   0        0        0     1313 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/AGVProcessor.py
+-rw-rw-rw-   0        0        0     1012 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/AbstractProcessor.py
+-rw-rw-rw-   0        0        0      482 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/ControlProcessor.py
+-rw-rw-rw-   0        0        0     1934 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/LocationProcessor.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/processors/__init__.py
+-rw-rw-rw-   0        0        0     5458 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/remotelib.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.032961 robobosim-1.5.0/src/robobosim/utils/
+-rw-rw-rw-   0        0        0      138 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/ConnectionState.py
+-rw-rw-rw-   0        0        0      919 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/Message.py
+-rw-rw-rw-   0        0        0        0 2024-05-22 14:36:21.000000 robobosim-1.5.0/src/robobosim/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:38:36.016580 robobosim-1.5.0/src/robobosim.egg-info/
+-rw-rw-rw-   0        0        0     1465 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      630 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 14:38:35.000000 robobosim-1.5.0/src/robobosim.egg-info/top_level.txt
```

### Comparing `robobosim-1.4.0/LICENSE` & `robobosim-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/PKG-INFO` & `robobosim-1.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: robobosim
-Version: 1.4.0
+Version: 1.5.0
 Summary: Robobo Sim remote control library
-Home-page: UNKNOWN
 Author: The Robobo Project
 Author-email: info@theroboboproject.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -50,8 +47,7 @@
 sim.wait(0.5)
 
 # Reset the simulation
 sim.resetSimulation()
 
 sim.disconnect()
 ```
-
```

### Comparing `robobosim-1.4.0/README.md` & `robobosim-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/setup.py` & `robobosim-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="robobosim",                     # This is the name of the package
-    version="1.4.0",                        # The initial release version
+    version="1.5.0",                        # The initial release version
     author="The Robobo Project",                     # Full name of the author
     author_email='info@theroboboproject.com',
     description="Robobo Sim remote control library",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     #repository_url="https://github.com/mintforpeople/robobosim.py",
     #packages=setuptools.find_packages(),    # List of all python modules to be installed
```

### Comparing `robobosim-1.4.0/src/robobosim/processors/AGVProcessor.py` & `robobosim-1.5.0/src/robobosim/processors/AGVProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/src/robobosim/processors/AbstractProcessor.py` & `robobosim-1.5.0/src/robobosim/processors/AbstractProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/src/robobosim/processors/LocationProcessor.py` & `robobosim-1.5.0/src/robobosim/processors/LocationProcessor.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/src/robobosim/remotelib.py` & `robobosim-1.5.0/src/robobosim/remotelib.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 import sys
 
 from robobosim.State import State
 from robobosim.utils.ConnectionState import ConnectionState
 
 from robobosim.processors.ControlProcessor import ControlProcessor
 from robobosim.processors.LocationProcessor import LocationProcessor
+from robobosim.processors.ObjectLocationProcessor import ObjectLocationProcessor
 from robobosim.processors.AGVProcessor import AGVProcessor
 
 class Remote:
     def __init__(self, ip):
         self.ip = ip
         self.ws = None
         self.password = "REMOTE-SIM"
         self.state = State()
         self.processors = {"CONTROL": ControlProcessor(self.state),
                            "LOCATION": LocationProcessor(self.state),
-                           "AGV": AGVProcessor(self.state)}
+                           "AGV": AGVProcessor(self.state),
+                           "OBJ-LOCATION": ObjectLocationProcessor(self.state)}
 
         self.wsDaemon = None
         self.connectionState = ConnectionState.DISCONNECTED
 
         self.timeout = 3
 
     def disconnect(self):
@@ -88,27 +90,52 @@
         else:
             sys.exit("\nError: Establish connection before sending a message")
 
     def resetSimulation(self):
         msg = self.processors["CONTROL"].resetSimulation()
         self.sendMessage(msg)
     
+    def getRobots(self):
+        try:
+            return self.state.locations.keys()
+        except KeyError as e:
+            return None
+    
     def getRobotLocation(self, robot_id):
         try:
             return self.state.locations[robot_id]
         except KeyError as e:
             return None
     
     def setRobotLocation(self, robot_id, position, rotation):
         try:
             msg = self.processors["LOCATION"].setRobotLocation(robot_id, position, rotation)
             self.sendMessage(msg)
         except KeyError as e:
             pass
     
+    def getObjects(self):
+        try:
+            return self.state.object_locations.keys()
+        except KeyError as e:
+            return None
+    
+    def getObjectLocation(self, object_id):
+        try:
+            return self.state.object_locations[object_id]
+        except KeyError as e:
+            return None
+    
+    def setObjectLocation(self, object_id, position, rotation):
+        try:
+            msg = self.processors["OBJ-LOCATION"].setObjectLocation(object_id, position, rotation)
+            self.sendMessage(msg)
+        except KeyError as e:
+            pass
+    
     def loadItem(self, robot_id):
         try:
             msg = self.processors["AGV"].loadItem(robot_id)
             self.sendMessage(msg)
         except KeyError as e:
             pass
     
@@ -124,11 +151,14 @@
             return self.state.loaded[robot_id]["loaded"]
         except KeyError as e:
             return None
 
     def setLocationCallback(self, callback):
         self.processors["LOCATION"].callbacks["location"] = callback
     
+    def setObjectLocationCallback(self, callback):
+        self.processors["OBJ-LOCATION"].callbacks["object-location"] = callback
+    
     def setLoadedCallback(self, callback):
         self.processors["AGV"].callbacks["loaded"] = callback
```

### Comparing `robobosim-1.4.0/src/robobosim/utils/Message.py` & `robobosim-1.5.0/src/robobosim/utils/Message.py`

 * *Files identical despite different names*

### Comparing `robobosim-1.4.0/src/robobosim.egg-info/PKG-INFO` & `robobosim-1.5.0/src/robobosim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: robobosim
-Version: 1.4.0
+Version: 1.5.0
 Summary: Robobo Sim remote control library
-Home-page: UNKNOWN
 Author: The Robobo Project
 Author-email: info@theroboboproject.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -50,8 +47,7 @@
 sim.wait(0.5)
 
 # Reset the simulation
 sim.resetSimulation()
 
 sim.disconnect()
 ```
-
```

### Comparing `robobosim-1.4.0/src/robobosim.egg-info/SOURCES.txt` & `robobosim-1.5.0/src/robobosim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

