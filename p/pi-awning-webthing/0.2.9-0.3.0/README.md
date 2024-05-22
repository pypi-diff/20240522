# Comparing `tmp/pi_awning_webthing-0.2.9.tar.gz` & `tmp/pi_awning_webthing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pi_awning_webthing-0.2.9.tar", last modified: Thu Apr 14 06:02:57 2022, max compression
+gzip compressed data, was "dist/pi_awning_webthing-0.3.0.tar", last modified: Wed May 22 04:09:33 2024, max compression
```

## Comparing `pi_awning_webthing-0.2.9.tar` & `pi_awning_webthing-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4739 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/
--rw-r--r--   0 runner    (1001) docker     (121)     2418 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5995 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     7154 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/awning.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/awning_webthing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/motor_tb6612Fng.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/pi_awning_webthing/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6512 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-14 06:02:57.000000 pi_awning_webthing-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-04-14 06:02:49.000000 pi_awning_webthing-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4716 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/awning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/awning_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/motor_tb6612Fng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/pi_awning_webthing/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 04:09:33.000000 pi_awning_webthing-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-22 04:09:24.000000 pi_awning_webthing-0.3.0/setup.py
```

### Comparing `pi_awning_webthing-0.2.9/PKG-INFO` & `pi_awning_webthing-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pi_awning_webthing
-Version: 0.2.9
+Version: 0.3.0
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
-        A web connected terrace awning controller on Raspberry Pi
+        A web based patio awning control on Raspberry Pi.
         
-        Currently supported are [TB6612FNG driven](https://www.pololu.com/product/713) motors such 
-        as [DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396). 
-        The concrete motor configuration(s) are defined by using a config file such s shown below. 
+        Currently supported are [TB6612FNG powered](https://www.pololu.com/product/713) motors as
+        [DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396).
+        The specific motor configuration(s) are defined using a configuration file as shown below.
         ```
         # name, gpio_forward, gpio_backward, step_duration_in_sec
         lane1, 2, 3, 0.5
         lane2, 19, 26, 0.5
         lane3, 5, 6, 0.5
         lane4, 10, 9, 0.5
         ```
-        For TB6612FNG driven motors the filename has to include the term *tb6612fng* such as tb6612fng_motors.config. Regarding the 
-        hardware setup and wiring please refer [example hardware setup](doc/dgo-3512ada.md)
+        For motors with TB6612FNG, the file name must contain the term *tb6612fng*, e.g. tb6612fng_motors.config. Concerning the
+        hardware setup and wiring please read [Example Hardware Setup](doc/dgo-3512ada.md).
         
-        To install this software you may use [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+        To install this software, you can use the [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager as shown below
         
         **Docker approach**
         ```
         sudo docker run --privileged -p 9500:9500 -v /etc/awning/:/etc/awning/ -e filename=/etc/awning/tb6612fng_motors.config  grro/pi_awning_webthing:0.2.0
         ```
         
         **PIP approach**
         ```
         sudo pip install pi-awning-webthing
         ```
         
-        After this installation you may start the webthing http endpoint inside your python code or via command line using
+        After installation, you can start the Webthing http endpoint in your Python code or from the command line by typing
         ```
         sudo awning --command listen--port 9500 --filename /etc/awning/tb6612fng_motors.config
         ```
-        Here, the webthing API will be bind on the local port 9500 
+        This binds the Webthing API to the local port 9500.
         
-        Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit. 
-        By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary. 
+        As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+        This will automatically start the webthing service at boot time. Starting the server manually with the *listen* command is no longer necessary.
         ```
         sudo awning --command register --port 9500 --filename /etc/awning/tb6612fng_motors.config 
         ```
         
-        The awning service exposes an http webthing endpoint supporting the awning properties. E.g. 
+        The awning service provides an http webthing endpoint that supports the awning properties. E.g. 
         ```
         # webthing has been started on host 192.168.0.23
         
         curl http://192.168.0.23:9500/properties 
         
         {
          [
```

### Comparing `pi_awning_webthing-0.2.9/README.md` & `pi_awning_webthing-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # pi_awning_webthing
-A web connected terrace awning controller on Raspberry Pi
+A web based patio awning control on Raspberry Pi.
 
-Currently supported are [TB6612FNG driven](https://www.pololu.com/product/713) motors such 
-as [DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396). 
-The concrete motor configuration(s) are defined by using a config file such s shown below. 
+Currently supported are [TB6612FNG powered](https://www.pololu.com/product/713) motors as
+[DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396).
+The specific motor configuration(s) are defined using a configuration file as shown below.
 ```
 # name, gpio_forward, gpio_backward, step_duration_in_sec
 lane1, 2, 3, 0.5
 lane2, 19, 26, 0.5
 lane3, 5, 6, 0.5
 lane4, 10, 9, 0.5
 ```
-For TB6612FNG driven motors the filename has to include the term *tb6612fng* such as tb6612fng_motors.config. Regarding the 
-hardware setup and wiring please refer [example hardware setup](doc/dgo-3512ada.md)
+For motors with TB6612FNG, the file name must contain the term *tb6612fng*, e.g. tb6612fng_motors.config. Concerning the
+hardware setup and wiring please read [Example Hardware Setup](doc/dgo-3512ada.md).
 
-To install this software you may use [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+To install this software, you can use the [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager as shown below
 
 **Docker approach**
 ```
 sudo docker run --privileged -p 9500:9500 -v /etc/awning/:/etc/awning/ -e filename=/etc/awning/tb6612fng_motors.config  grro/pi_awning_webthing:0.2.0
 ```
 
 **PIP approach**
 ```
 sudo pip install pi-awning-webthing
 ```
 
-After this installation you may start the webthing http endpoint inside your python code or via command line using
+After installation, you can start the Webthing http endpoint in your Python code or from the command line by typing
 ```
 sudo awning --command listen--port 9500 --filename /etc/awning/tb6612fng_motors.config
 ```
-Here, the webthing API will be bind on the local port 9500 
+This binds the Webthing API to the local port 9500.
 
-Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit. 
-By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary. 
+As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+This will automatically start the webthing service at boot time. Starting the server manually with the *listen* command is no longer necessary.
 ```
 sudo awning --command register --port 9500 --filename /etc/awning/tb6612fng_motors.config 
 ```
 
-The awning service exposes an http webthing endpoint supporting the awning properties. E.g. 
+The awning service provides an http webthing endpoint that supports the awning properties. E.g. 
 ```
 # webthing has been started on host 192.168.0.23
 
 curl http://192.168.0.23:9500/properties 
 
 {
  [
```

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing/__init__.py` & `pi_awning_webthing-0.3.0/pi_awning_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing/app.py` & `pi_awning_webthing-0.3.0/pi_awning_webthing/app.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing/awning.py` & `pi_awning_webthing-0.3.0/pi_awning_webthing/awning.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,44 @@
 import logging
 import sys
 import time
 from datetime import datetime
+from typing import List
 from abc import ABC, abstractmethod
 from threading import Thread, Lock
 
 
+
+
+class Awning(ABC):
+
+    def __init__(self, name: str):
+        self.name = name
+        self.__listeners = set()
+
+    @abstractmethod
+    def is_target_reached(self) -> bool:
+        pass
+
+    @abstractmethod
+    def get_position(self) -> int:
+        pass
+
+    @abstractmethod
+    def set_position(self, new_position: int):
+        pass
+
+    def add_listener(self, listener):
+        self.__listeners.add(listener)
+
+    def _notify_listeners(self):
+        for listener in self.__listeners:
+            listener()
+
+
 class Motor(ABC):
 
     @abstractmethod
     def stop(self):
         pass
 
     @abstractmethod
@@ -27,26 +56,14 @@
 
     @property
     @abstractmethod
     def sec_per_step(self) -> float:
         pass
 
 
-class AwningPropertyListener:
-
-    def on_current_pos_updated(self, current_position: int):
-        pass
-
-    def on_retracting_updated(self, retracting: bool):
-        pass
-
-    def on_extenting_updated(self, extenting: bool):
-        pass
-
-
 class Movement:
     SLOT_TOLERANCE = 7
 
     def __init__(self, motor: Motor, start_pos: int, num_slots: int, sec_per_slot: float, is_positive: bool, awning):
         self.start_time = datetime.now()
         self.awning = awning
         self.motor = motor
@@ -80,15 +97,15 @@
             num_processed = elapsed_sec / self.sec_per_slot
         return int(num_processed)
 
     def process(self):
         if self.is_target_reached():
             return Idling(self.motor, self.get_target_pos(), self.sec_per_slot, self.awning)
         else:
-            self.awning.listener.on_current_pos_updated(self.get_current_pos())
+            self.awning.on_updated()
             return self
 
     def drive_to(self, new_position: int):
         if new_position > 100:
             new_position = 100
         elif new_position < 0:
             new_position = 0
@@ -105,16 +122,15 @@
 
 
 class Idling(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, 0, sec_per_slot, True, awning)
         self.motor.stop()
-        self.awning.listener.on_extenting_updated(False)
-        self.awning.listener.on_retracting_updated(False)
+        self.awning.on_updated()
 
     def get_pause_sec(self):
         pause_sec = int(self.SLOT_TOLERANCE * self.sec_per_slot * 1.4)
         if pause_sec < 3:
             pause_sec = 3
         return pause_sec
 
@@ -123,94 +139,119 @@
 
 
 class Forward(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, new_position: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, new_position - start_pos, sec_per_slot, True, awning)
         self.motor.forward()
-        self.awning.listener.on_extenting_updated(True)
-        self.awning.listener.on_retracting_updated(False)
+        self.awning.on_updated()
 
 
 class Backward(Movement):
 
     def __init__(self, motor: Motor, start_pos: int, new_position: int, sec_per_slot: float, awning):
         Movement.__init__(self, motor, start_pos, start_pos - new_position, sec_per_slot, False, awning)
         self.motor.backward()
-        self.awning.listener.on_retracting_updated(True)
-        self.awning.listener.on_extenting_updated(False)
+        self.awning.on_updated()
 
 
-class Awning:
+class PiAwning(Awning):
     PERIODIC_CALIBRATE_ON_HOUR = 3
     PERIODIC_CALIBRATE_ON_MINUTE = 10
 
     def __init__(self, motor: Motor):
         self.sec_per_slot = motor.sec_per_step
-        self.listener = AwningPropertyListener()
         self.motor = motor
         self.__lock = Lock()
         self.movement = Idling(self.motor, 0, self.sec_per_slot, self)
-        self.set_target_position(0)
+        self.set_position(0)
+        super().__init__(self.motor.name)
         Thread(name=self.name + "_move", target=self.__process_move, daemon=False).start()
         Thread(target=self.__periodic_calibrate, daemon=True).start()
 
-    @property
-    def name(self) -> str:
-        return self.motor.name
+    def on_updated(self):
+        self._notify_listeners()
 
     def __periodic_calibrate(self):
         time.sleep(60)
         self.calibrate()
         already_scheduled = False
         while True:
-            now = datetime.now()
-            if self.PERIODIC_CALIBRATE_ON_HOUR <= now.hour < (self.PERIODIC_CALIBRATE_ON_HOUR + 1) and now.minute >= self.PERIODIC_CALIBRATE_ON_MINUTE:
-                if not already_scheduled:
-                    self.calibrate()
-                already_scheduled = True
-            else:
-                already_scheduled = False
+            try:
+                now = datetime.now()
+                if self.PERIODIC_CALIBRATE_ON_HOUR <= now.hour < (self.PERIODIC_CALIBRATE_ON_HOUR + 1) and now.minute >= self.PERIODIC_CALIBRATE_ON_MINUTE:
+                    if not already_scheduled:
+                        self.calibrate()
+                    already_scheduled = True
+                else:
+                    already_scheduled = False
+            except Exception as e:
+                logging.warning("error occurred on calibrating " + str(e))
             time.sleep(10 * 60)
 
-    def register_listener(self, listener: AwningPropertyListener):
-        self.listener = listener
-
     def calibrate(self):
-        saved_target_pos = self.get_target_position()
+        saved_target_pos = self.get_position()
         logging.info("calibrating")
         self.movement = Idling(self.motor, 100, self.sec_per_slot, self) # set position to 100%
-        self.set_target_position(0)   # and backward to position 0. This ensures that the awning is calibrated with position 0
+        self.set_position(0)   # and backward to position 0. This ensures that the awning is calibrated with position 0
         # wait until completed
         for i in range (0, 60):
             if self.is_target_reached():
                 break
             else:
                 time.sleep(5)
-        if self.get_current_position() != saved_target_pos:
+        if self.__get_current_position() != saved_target_pos:
             logging.info("move to previous target position " + str(saved_target_pos))
-            self.set_target_position(saved_target_pos)
+            self.set_position(saved_target_pos)
+
+    def __get_current_position(self) -> int:
+        return self.movement.get_current_pos()
 
     def is_target_reached(self) -> bool:
         return self.movement.is_target_reached()
 
-    def get_current_position(self) -> int:
-        return self.movement.get_current_pos()
-
-    def get_target_position(self) -> int:
+    def get_position(self) -> int:
         return self.movement.get_target_pos()
 
-    def set_target_position(self, new_position: int):
+    def set_position(self, new_position: int):
         with self.__lock:
             self.movement = self.movement.drive_to(new_position)
 
     def __process_move(self):
         while True:
             with self.__lock:
                 try:
                     self.movement = self.movement.process()
                 except:
                     self.movement = Idling(self.motor, 0, self.sec_per_slot, self)
                     logging.warning('move operation failed ' + str(sys.exc_info()))
                 finally:
                     pause_sec = self.movement.get_pause_sec()
             time.sleep(pause_sec)
+
+
+
+class Awnings(Awning):
+
+    def __init__(self, name: str, awnings: List[Awning]):
+        self.__awnings = awnings
+        [awning.add_listener(self._notify_listeners) for awning in awnings]
+        super().__init__(name)
+
+    def is_target_reached(self) -> bool:
+        for awning in self.__awnings:
+            if not awning.is_target_reached():
+                return False
+        return True
+
+    def get_position(self) -> int:
+        positions = [awning.get_position() for awning in self.__awnings]
+        total = sum(positions)
+        if total == 0:
+            return 0
+        else:
+            return int(total/len(positions))
+
+    def set_position(self, target_position: int):
+        [awning.set_position(target_position) for awning in self.__awnings]
+
+
```

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing/motor_tb6612Fng.py` & `pi_awning_webthing-0.3.0/pi_awning_webthing/motor_tb6612Fng.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing/switch.py` & `pi_awning_webthing-0.3.0/pi_awning_webthing/switch.py`

 * *Files identical despite different names*

### Comparing `pi_awning_webthing-0.2.9/pi_awning_webthing.egg-info/PKG-INFO` & `pi_awning_webthing-0.3.0/pi_awning_webthing.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 Metadata-Version: 2.1
 Name: pi-awning-webthing
-Version: 0.2.9
+Version: 0.3.0
 Summary: A web connected terrace awning controller on Raspberry Pi
 Home-page: https://github.com/grro/pi_awning_webthing
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 License: MIT
 Description: # pi_awning_webthing
-        A web connected terrace awning controller on Raspberry Pi
+        A web based patio awning control on Raspberry Pi.
         
-        Currently supported are [TB6612FNG driven](https://www.pololu.com/product/713) motors such 
-        as [DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396). 
-        The concrete motor configuration(s) are defined by using a config file such s shown below. 
+        Currently supported are [TB6612FNG powered](https://www.pololu.com/product/713) motors as
+        [DGO-3512ADA](https://www.ebay.co.uk/itm/Gear-Motor-Direct-Current-6-12V-Electric-With-Removable-Crank-DGO-3512ADA-/183375290396).
+        The specific motor configuration(s) are defined using a configuration file as shown below.
         ```
         # name, gpio_forward, gpio_backward, step_duration_in_sec
         lane1, 2, 3, 0.5
         lane2, 19, 26, 0.5
         lane3, 5, 6, 0.5
         lane4, 10, 9, 0.5
         ```
-        For TB6612FNG driven motors the filename has to include the term *tb6612fng* such as tb6612fng_motors.config. Regarding the 
-        hardware setup and wiring please refer [example hardware setup](doc/dgo-3512ada.md)
+        For motors with TB6612FNG, the file name must contain the term *tb6612fng*, e.g. tb6612fng_motors.config. Concerning the
+        hardware setup and wiring please read [Example Hardware Setup](doc/dgo-3512ada.md).
         
-        To install this software you may use [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+        To install this software, you can use the [Docker](https://phoenixnap.com/kb/docker-on-raspberry-pi) or [PIP](https://realpython.com/what-is-pip/) package manager as shown below
         
         **Docker approach**
         ```
         sudo docker run --privileged -p 9500:9500 -v /etc/awning/:/etc/awning/ -e filename=/etc/awning/tb6612fng_motors.config  grro/pi_awning_webthing:0.2.0
         ```
         
         **PIP approach**
         ```
         sudo pip install pi-awning-webthing
         ```
         
-        After this installation you may start the webthing http endpoint inside your python code or via command line using
+        After installation, you can start the Webthing http endpoint in your Python code or from the command line by typing
         ```
         sudo awning --command listen--port 9500 --filename /etc/awning/tb6612fng_motors.config
         ```
-        Here, the webthing API will be bind on the local port 9500 
+        This binds the Webthing API to the local port 9500.
         
-        Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit. 
-        By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary. 
+        As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+        This will automatically start the webthing service at boot time. Starting the server manually with the *listen* command is no longer necessary.
         ```
         sudo awning --command register --port 9500 --filename /etc/awning/tb6612fng_motors.config 
         ```
         
-        The awning service exposes an http webthing endpoint supporting the awning properties. E.g. 
+        The awning service provides an http webthing endpoint that supports the awning properties. E.g. 
         ```
         # webthing has been started on host 192.168.0.23
         
         curl http://192.168.0.23:9500/properties 
         
         {
          [
```

### Comparing `pi_awning_webthing-0.2.9/setup.py` & `pi_awning_webthing-0.3.0/setup.py`

 * *Files identical despite different names*

