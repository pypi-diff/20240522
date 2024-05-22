# Comparing `tmp/psychopy_bbtk-0.0.8.tar.gz` & `tmp/psychopy_bbtk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy_bbtk-0.0.8.tar", last modified: Wed May 15 16:32:31 2024, max compression
+gzip compressed data, was "psychopy_bbtk-0.0.9.tar", last modified: Wed May 22 12:01:32 2024, max compression
```

## Comparing `psychopy_bbtk-0.0.8.tar` & `psychopy_bbtk-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/docs_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/docs_src/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/docs_src/generatePages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk/
--rw-r--r--   0 runner    (1001) docker     (127)    19359 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk/components/
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/components/tpad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/forcePad.py
--rw-r--r--   0 runner    (1001) docker     (127)    18017 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/psychopy_bbtk/tpad.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-15 16:32:31.000000 psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 16:32:31.196690 psychopy_bbtk-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/test_builder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_builder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:31.192690 psychopy_bbtk-0.0.8/tests/test_coder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-15 16:32:20.000000 psychopy_bbtk-0.0.8/tests/test_coder/test_running_via_liaison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.017969 psychopy_bbtk-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 12:01:32.017969 psychopy_bbtk-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.013969 psychopy_bbtk-0.0.9/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/docs_src/generatePages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.013969 psychopy_bbtk-0.0.9/psychopy_bbtk/
+-rw-r--r--   0 runner    (1001) docker     (127)    19359 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/psychopy_bbtk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.013969 psychopy_bbtk-0.0.9/psychopy_bbtk/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/psychopy_bbtk/components/tpad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/psychopy_bbtk/forcePad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/psychopy_bbtk/tpad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.017969 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 12:01:32.000000 psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:01:32.017969 psychopy_bbtk-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.013969 psychopy_bbtk-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.013969 psychopy_bbtk-0.0.9/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/tests/test_builder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:32.017969 psychopy_bbtk-0.0.9/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/tests/test_coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-22 12:01:24.000000 psychopy_bbtk-0.0.9/tests/test_coder/test_running_via_liaison.py
```

### Comparing `psychopy_bbtk-0.0.8/LICENSE` & `psychopy_bbtk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/PKG-INFO` & `psychopy_bbtk-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
```

### Comparing `psychopy_bbtk-0.0.8/README.md` & `psychopy_bbtk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/docs_src/conf.py` & `psychopy_bbtk-0.0.9/docs_src/conf.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/docs_src/generatePages.py` & `psychopy_bbtk-0.0.9/docs_src/generatePages.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk/__init__.py` & `psychopy_bbtk-0.0.9/psychopy_bbtk/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk/components/tpad.py` & `psychopy_bbtk-0.0.9/psychopy_bbtk/components/tpad.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk/forcePad.py` & `psychopy_bbtk-0.0.9/psychopy_bbtk/forcePad.py`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk/tpad.py` & `psychopy_bbtk-0.0.9/psychopy_bbtk/tpad.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from psychopy.hardware import base, serialdevice as sd, photodiode, button
-from psychopy.hardware.manager import deviceManager, DeviceManager
+from psychopy.hardware.manager import deviceManager, DeviceManager, ManagedDeviceError
 from psychopy import logging, layout
 from psychopy.tools import systemtools as st
 import serial
 import re
 import sys
 
 # possible values for self.channel
@@ -47,29 +47,19 @@
 def splitTPadMessage(message):
     return re.match(messageFormat, message).groups()
 
 
 class TPadPhotodiodeGroup(photodiode.BasePhotodiodeGroup):
     def __init__(self, pad, channels, threshold=None, pos=None, size=None, units=None):
         _requestedPad = pad
-        # try to get associated tpad
-        if isinstance(_requestedPad, str):
-            # try getting by name
-            pad = DeviceManager.getDevice(pad)
-            # if failed, try getting by port
-            if pad is None:
-                pad = DeviceManager.getDeviceBy("portString", _requestedPad, deviceClass="psychopy_bbtk.tpad.TPad")
-        # if still failed, make one
-        if pad is None:
-            pad = TPad(port=_requestedPad)
-
+        # get associated tpad
+        self.parent = TPad.resolve(pad)
         # reference self in pad
-        pad.nodes.append(self)
+        self.parent.nodes.append(self)
         # initialise base class
-        self.parent = pad
         photodiode.BasePhotodiodeGroup.__init__(
             self, channels=channels, threshold=threshold, pos=pos, size=size, units=units
         )
 
     def isSameDevice(self, other):
         """
         Determine whether this object represents the same physical device as a given other object.
@@ -112,15 +102,15 @@
     def _setThreshold(self, threshold, channel):
         if threshold is None:
             return
         # enter command mode
         self.parent.setMode(0)
         # send command to set threshold
         self.parent.sendMessage(f"AAO{channel+1} {threshold}")
-        resp = self.parent.awaitResponse()
+        resp = self.parent.awaitResponse(timeout=0.1)
         # with this threshold, is the photodiode returning True?
         measurement = None
         if resp is not None:
             if resp.strip() == "1":
                 measurement = True
             if resp.strip() == "0":
                 measurement = False
@@ -138,14 +128,25 @@
 
         Returns
         -------
         bool
             True if request sent successfully
         """
         self.parent.dispatchMessages()
+    
+    def hasUnfinishedMessage(self):
+        """
+        Is the parent TPad waiting for an end-of-line character?
+        
+        Returns
+        -------
+        bool
+            True if there is a partial message waiting for an end-of-line
+        """
+        return self.parent.hasUnfinishedMessage()
 
     def parseMessage(self, message):
         # if given a string, split according to regex
         if isinstance(message, str):
             message = splitTPadMessage(message)
         # split into variables
         # assert isinstance(message, (tuple, list)) and len(message) == 4
@@ -165,22 +166,22 @@
         # create PhotodiodeResponse object
         resp = photodiode.PhotodiodeResponse(
             t=time, channel=channel, value=state, threshold=self.getThreshold(channel-1)
         )
 
         return resp
 
-    def findPhotodiode(self, win, channel):
+    def findPhotodiode(self, win, channel=None):
         # set mode to 3
         self.parent.setMode(3)
         self.parent.pause()
         # continue as normal
         return photodiode.BasePhotodiodeGroup.findPhotodiode(self, win, channel)
 
-    def findThreshold(self, win, channel):
+    def findThreshold(self, win, channel=None):
         # set mode to 0 and lock it so mode doesn't change during setThreshold calls
         self.parent.setMode(0)
         self.parent.lockMode()
         # continue as normal
         resp = photodiode.BasePhotodiodeGroup.findThreshold(self, win, channel)
         self._setThreshold(0, channel=1)
         # set back to mode 3
@@ -188,31 +189,20 @@
         self.parent.setMode(3)
 
         return resp
 
 
 class TPadButtonGroup(button.BaseButtonGroup):
     def __init__(self, pad, channels=9):
-        _requestedPad = pad
-        # try to get associated tpad
-        if isinstance(_requestedPad, str):
-            # try getting by name
-            pad = DeviceManager.getDevice(pad)
-            # if failed, try getting by port
-            if pad is None:
-                pad = DeviceManager.getDeviceBy("portString", _requestedPad, deviceClass="psychopy_bbtk.tpad.TPad")
-        # if still failed, make one
-        if pad is None:
-            pad = TPad(port=_requestedPad)
-
+        # get associated tpad
+        self.parent = TPad.resolve(pad)
         # reference self in pad
-        pad.nodes.append(self)
+        self.parent.nodes.append(self)
         # initialise base class
         button.BaseButtonGroup.__init__(self, channels=channels)
-        self.parent = pad
 
     def isSameDevice(self, other):
         """
         Determine whether this object represents the same physical device as a given other object.
 
         Parameters
         ----------
@@ -242,14 +232,25 @@
 
         Returns
         -------
         bool
             True if request sent successfully
         """
         self.parent.dispatchMessages()
+    
+    def hasUnfinishedMessage(self):
+        """
+        Is the parent TPad waiting for an end-of-line character?
+        
+        Returns
+        -------
+        bool
+            True if there is a partial message waiting for an end-of-line
+        """
+        return self.parent.hasUnfinishedMessage()
 
     def parseMessage(self, message):
         # if given a string, split according to regex
         if isinstance(message, str):
             message = splitTPadMessage(message)
         # split into variables
         # assert isinstance(message, (tuple, list)) and len(message) == 4
@@ -323,14 +324,17 @@
             parity=parity,  # 'N'one, 'E'ven, 'O'dd, 'M'ask,
             eol=eol,
             maxAttempts=maxAttempts, pauseDuration=pauseDuration,
             checkAwake=checkAwake
         )
         # reset timer
         self.resetTimer()
+    
+    def __del__(self):
+        self.close()
 
     def close(self):
         # set mode to 0 on exit
         self.setMode(0)
         # close
         sd.SerialDevice.close(self)
 
@@ -365,14 +369,53 @@
                 devices.append({
                     'deviceName': profile['deviceName'],
                     'port': profile['port'],
                 })
 
         return devices
 
+    @classmethod
+    def resolve(cls, requested):
+        """
+        Take a value given to a device which has a TPad as its parent and, from it, 
+        find/make the associated TPad object.
+
+        Parameters
+        ----------
+        requested : str, int or TPad
+            Value to resolve
+        """
+        # if requested is already a handle, return as is
+        if isinstance(requested, cls):
+            return requested
+        # try to get by name
+        if isinstance(requested, str):
+            pad = DeviceManager.getDevice(requested)
+            # if found, return
+            if pad is not None:
+                return pad
+        # if requested looks like a port number, turn it into a port string
+        if isinstance(requested, int):
+            requested = f"COM{requested}"
+        # try to get by port
+        if isinstance(requested, str):
+            pad = DeviceManager.getDeviceBy("portString", requested, deviceClass="psychopy_bbtk.tpad.TPad")
+            # if found, return
+            if pad is not None:
+                return pad
+        # if given port of a not-yet setup device, set one up
+        if requested is None or isinstance(requested, str):
+            return DeviceManager.addDevice(
+                deviceClass="psychopy_bbtk.tpad.TPad",
+                deviceName=f"TPad@{requested}",
+                port=requested
+            )
+        # if still not found, raise error
+        raise ManagedDeviceError(f"Could not find/create any {cls.__name__} object from the value {requested}")
+
     def addListener(self, listener):
         """
         Add a listener, which will receive all the messages dispatched by this TPad.
 
         Parameters
         ----------
         listener : hardware.listener.BaseListener
@@ -428,14 +471,39 @@
                     # dispatch to node
                     message = node.parseMessage(parts)
                     node.receiveMessage(message)
                 else:
                     logging.debug(f"Received unparsable message from TPad: {line}")
         # mark that a dispatch has finished
         self._dispatchInProgress = False
+    
+    def hasUnfinishedMessage(self):
+        """
+        We don't wait for an end-of-line from the TPad device before continuing, as 
+        dispatchMessages is often called in a frame loop so waiting for messages would 
+        ruin the frame rate. If just the start of a message has been received, this 
+        function will return True.
+
+        Usage
+        -----
+        If you want to be certain that all events have been dispatched, you can do:
+        ```
+        timeout = Clock()
+        while myTPad.hasUnfinishedMessage() and timeout.getTime() < 0.1:
+            myTPad.dispatchMessages()
+        ```
+        (the purpose of the `timeout` clock is to avoid getting into an infinite loop 
+        if the TPad sends anything unexpected)
+        
+        Returns
+        -------
+        bool
+            True if there is a partial message waiting for an end-of-line
+        """
+        return bool(self._lastLine)
 
     @staticmethod
     def _detectComPort():
         # find available devices
         available = TPad.getAvailableDevices()
         # error if there are none
         if not available:
```

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/PKG-INFO` & `psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychopy-bbtk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Extension package for adding support for BlackBoxToolkit devices to PsychoPy.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: homepage, https://github.com/psychopy/psychopy-bbtk
 Project-URL: changelog, https://github.com/psychopy/psychopy-bbtk/blob/main/CHANGELOG.txt
 Project-URL: documentation, https://pages.github.com/psychopy/psychopy-bbtk
 Project-URL: repository, https://github.com/psychopy/psychopy-bbtk
```

### Comparing `psychopy_bbtk-0.0.8/psychopy_bbtk.egg-info/SOURCES.txt` & `psychopy_bbtk-0.0.9/psychopy_bbtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psychopy_bbtk-0.0.8/pyproject.toml` & `psychopy_bbtk-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-bbtk"
-version = "0.0.8"
+version = "0.0.9"
 description = "Extension package for adding support for BlackBoxToolkit devices to PsychoPy."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = {text = "GNU General Public License v3 (GPLv3)"}
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
```

### Comparing `psychopy_bbtk-0.0.8/tests/test_coder/test_running_via_liaison.py` & `psychopy_bbtk-0.0.9/tests/test_coder/test_running_via_liaison.py`

 * *Files identical despite different names*

