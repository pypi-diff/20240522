# Comparing `tmp/pi_awning_webthing-0.3.0.tar.gz` & `tmp/pi_awning_webthing-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pi_awning_webthing-0.3.0.tar", last modified: Wed May 22 04:09:33 2024, max compression
+gzip compressed data, was "dist/pi_awning_webthing-0.3.1.tar", last modified: Wed May 22 04:19:37 2024, max compression
```

## Comparing `pi_awning_webthing-0.3.0.tar` & `pi_awning_webthing-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/awning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/awning_webthing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/motor_tb6612Fng.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/awning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/awning_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/motor_tb6612Fng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/pi_awning_webthing/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:19:36.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:19:36.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 04:19:36.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 04:19:36.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 04:19:36.000000 pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:19:37.000000 pi_awning_webthing-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-22 04:19:21.000000 pi_awning_webthing-0.3.1/setup.py
```

### Comparing `pi_awning_webthing-0.3.0/PKG-INFO` & `pi_awning_webthing-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi_awning_webthing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.0/README.md` & `pi_awning_webthing-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/__init__.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/app.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/app.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/awning.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/awning.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -155,20 +155,20 @@
 
 
 class PiAwning(Awning):
     PERIODIC_CALIBRATE_ON_HOUR = 3
     PERIODIC_CALIBRATE_ON_MINUTE = 10
 
     def __init__(self, motor: Motor):
-        self.sec_per_slot = motor.sec_per_step
         self.motor = motor
+        super().__init__(self.motor.name)
+        self.sec_per_slot = motor.sec_per_step
         self.__lock = Lock()
         self.movement = Idling(self.motor, 0, self.sec_per_slot, self)
         self.set_position(0)
-        super().__init__(self.motor.name)
         Thread(name=self.name + "_move", target=self.__process_move, daemon=False).start()
         Thread(target=self.__periodic_calibrate, daemon=True).start()
 
     def on_updated(self):
         self._notify_listeners()
 
     def __periodic_calibrate(self):
```

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/awning_webthing.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/awning_webthing.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/motor_tb6612Fng.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/motor_tb6612Fng.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing/switch.py` & `pi_awning_webthing-0.3.1/pi_awning_webthing/switch.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/PKG-INFO` & `pi_awning_webthing-0.3.1/pi_awning_webthing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-awning-webthing
-Version: 0.3.0
+Version: 0.3.1
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
         A web based patio awning control on Raspberry Pi.
```

### Comparing `pi_awning_webthing-0.3.0/setup.py` & `pi_awning_webthing-0.3.1/setup.py`

 * *Files identical despite different names*

