# Comparing `tmp/uitk-1.0.8.tar.gz` & `tmp/uitk-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uitk-1.0.8.tar", last modified: Fri Dec 22 01:09:59 2023, max compression
+gzip compressed data, was "uitk-1.0.9.tar", last modified: Sat Dec 23 01:20:50 2023, max compression
```

## Comparing `uitk-1.0.8.tar` & `uitk-1.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.389319 uitk-1.0.8/
--rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-1.0.8/COPYING.LESSER
--rw-rw-rw-   0        0        0       24 2023-09-06 12:44:13.000000 uitk-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3177 2023-12-22 01:09:59.388318 uitk-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-12-22 01:09:59.389319 uitk-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1487 2023-12-17 13:26:45.000000 uitk-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.316123 uitk-1.0.8/uitk/
--rw-rw-rw-   0        0        0     2585 2023-12-22 01:09:55.000000 uitk-1.0.8/uitk/__init__.py
--rw-rw-rw-   0        0        0    11214 2023-09-18 17:30:57.000000 uitk-1.0.8/uitk/events.py
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.363813 uitk-1.0.8/uitk/example/
--rw-rw-rw-   0        0        0        0 2023-09-12 01:52:27.000000 uitk-1.0.8/uitk/example/__init__.py
--rw-rw-rw-   0        0        0     4811 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/example/example#submenu.ui
--rw-rw-rw-   0        0        0     8508 2023-12-21 17:12:59.000000 uitk-1.0.8/uitk/example/example.ui
--rw-rw-rw-   0        0        0     2494 2023-12-21 22:54:36.000000 uitk-1.0.8/uitk/example/example_slots.py
--rw-rw-rw-   0        0        0    19699 2023-11-14 12:00:24.000000 uitk-1.0.8/uitk/file_manager.py
--rw-rw-rw-   0        0        0     1688 2023-10-25 12:10:50.000000 uitk-1.0.8/uitk/signals.py
--rw-rw-rw-   0        0        0    74730 2023-12-21 22:53:29.000000 uitk-1.0.8/uitk/switchboard.py
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.364813 uitk-1.0.8/uitk/ui/
--rw-rw-rw-   0        0        0     4853 2023-04-21 13:38:34.000000 uitk-1.0.8/uitk/ui/example.ui
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.379318 uitk-1.0.8/uitk/widgets/
--rw-rw-rw-   0        0        0     3204 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/__init__.py
--rw-rw-rw-   0        0        0    15921 2023-09-26 15:05:57.000000 uitk-1.0.8/uitk/widgets/attributeWindow.py
--rw-rw-rw-   0        0        0     5619 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/checkBox.py
--rw-rw-rw-   0        0        0     3643 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/collapsableGroup.py
--rw-rw-rw-   0        0        0    12151 2023-10-25 13:14:39.000000 uitk-1.0.8/uitk/widgets/comboBox.py
--rw-rw-rw-   0        0        0    22493 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/expandableList.py
--rw-rw-rw-   0        0        0    10426 2023-10-06 11:37:03.000000 uitk-1.0.8/uitk/widgets/header.py
--rw-rw-rw-   0        0        0     2536 2023-10-06 11:08:42.000000 uitk-1.0.8/uitk/widgets/label.py
--rw-rw-rw-   0        0        0     3296 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/lineEdit.py
--rw-rw-rw-   0        0        0    20327 2023-10-11 15:53:00.000000 uitk-1.0.8/uitk/widgets/mainWindow.py
--rw-rw-rw-   0        0        0    22471 2023-10-11 13:04:41.000000 uitk-1.0.8/uitk/widgets/menu.py
--rw-rw-rw-   0        0        0     8559 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/messageBox.py
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.387318 uitk-1.0.8/uitk/widgets/mixins/
--rw-rw-rw-   0        0        0     3028 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/mixins/__init__.py
--rw-rw-rw-   0        0        0    13148 2023-09-26 15:43:37.000000 uitk-1.0.8/uitk/widgets/mixins/attributes.py
--rw-rw-rw-   0        0        0     4023 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/mixins/convert.py
--rw-rw-rw-   0        0        0     9499 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/mixins/docking.py
--rw-rw-rw-   0        0        0    49002 2023-12-17 15:08:52.000000 uitk-1.0.8/uitk/widgets/mixins/style_sheet.py
--rw-rw-rw-   0        0        0    58215 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/mixins/task_indicator.gif
--rw-rw-rw-   0        0        0     3409 2023-09-06 12:44:13.000000 uitk-1.0.8/uitk/widgets/mixins/tasks.py
--rw-rw-rw-   0        0        0    10882 2023-09-12 11:16:33.000000 uitk-1.0.8/uitk/widgets/mixins/text.py
--rw-rw-rw-   0        0        0     6426 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/optionBox.py
--rw-rw-rw-   0        0        0     3272 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/progressBar.py
--rw-rw-rw-   0        0        0     2135 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/pushButton.py
--rw-rw-rw-   0        0        0     7907 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/region.py
--rw-rw-rw-   0        0        0     3717 2023-09-18 17:32:03.000000 uitk-1.0.8/uitk/widgets/textEdit.py
-drwxrwxrwx   0        0        0        0 2023-12-22 01:09:59.387318 uitk-1.0.8/uitk.egg-info/
--rw-rw-rw-   0        0        0     3177 2023-12-22 01:09:59.000000 uitk-1.0.8/uitk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4290 2023-04-06 23:46:30.000000 uitk-1.0.8/uitk.egg-info/PKG-INFO.bak
--rw-rw-rw-   0        0        0     1154 2023-12-22 01:09:59.000000 uitk-1.0.8/uitk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      768 2023-04-15 12:45:23.000000 uitk-1.0.8/uitk.egg-info/SOURCES.txt.bak
--rw-rw-rw-   0        0        0        1 2023-12-22 01:09:59.000000 uitk-1.0.8/uitk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-12-22 01:09:59.000000 uitk-1.0.8/uitk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-12-22 01:09:59.000000 uitk-1.0.8/uitk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.615872 uitk-1.0.9/
+-rw-rw-rw-   0        0        0     7815 2023-04-16 12:18:04.000000 uitk-1.0.9/COPYING.LESSER
+-rw-rw-rw-   0        0        0       24 2023-09-06 12:44:13.000000 uitk-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3177 2023-12-23 01:20:50.614872 uitk-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-12-23 01:20:50.615872 uitk-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1487 2023-12-17 13:26:45.000000 uitk-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.559884 uitk-1.0.9/uitk/
+-rw-rw-rw-   0        0        0     2585 2023-12-23 01:20:43.000000 uitk-1.0.9/uitk/__init__.py
+-rw-rw-rw-   0        0        0    11214 2023-09-18 17:30:57.000000 uitk-1.0.9/uitk/events.py
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.593680 uitk-1.0.9/uitk/example/
+-rw-rw-rw-   0        0        0        0 2023-09-12 01:52:27.000000 uitk-1.0.9/uitk/example/__init__.py
+-rw-rw-rw-   0        0        0     4811 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/example/example#submenu.ui
+-rw-rw-rw-   0        0        0     8508 2023-12-21 17:12:59.000000 uitk-1.0.9/uitk/example/example.ui
+-rw-rw-rw-   0        0        0     2494 2023-12-21 22:54:36.000000 uitk-1.0.9/uitk/example/example_slots.py
+-rw-rw-rw-   0        0        0    19699 2023-11-14 12:00:24.000000 uitk-1.0.9/uitk/file_manager.py
+-rw-rw-rw-   0        0        0     1688 2023-10-25 12:10:50.000000 uitk-1.0.9/uitk/signals.py
+-rw-rw-rw-   0        0        0    74781 2023-12-23 00:47:04.000000 uitk-1.0.9/uitk/switchboard.py
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.594686 uitk-1.0.9/uitk/ui/
+-rw-rw-rw-   0        0        0     4853 2023-04-21 13:38:34.000000 uitk-1.0.9/uitk/ui/example.ui
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.608873 uitk-1.0.9/uitk/widgets/
+-rw-rw-rw-   0        0        0     3204 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/__init__.py
+-rw-rw-rw-   0        0        0    15921 2023-09-26 15:05:57.000000 uitk-1.0.9/uitk/widgets/attributeWindow.py
+-rw-rw-rw-   0        0        0     5619 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/checkBox.py
+-rw-rw-rw-   0        0        0     3643 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/collapsableGroup.py
+-rw-rw-rw-   0        0        0    12151 2023-10-25 13:14:39.000000 uitk-1.0.9/uitk/widgets/comboBox.py
+-rw-rw-rw-   0        0        0    22493 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/expandableList.py
+-rw-rw-rw-   0        0        0    10426 2023-10-06 11:37:03.000000 uitk-1.0.9/uitk/widgets/header.py
+-rw-rw-rw-   0        0        0     2536 2023-10-06 11:08:42.000000 uitk-1.0.9/uitk/widgets/label.py
+-rw-rw-rw-   0        0        0     3296 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/lineEdit.py
+-rw-rw-rw-   0        0        0    20327 2023-10-11 15:53:00.000000 uitk-1.0.9/uitk/widgets/mainWindow.py
+-rw-rw-rw-   0        0        0    22471 2023-10-11 13:04:41.000000 uitk-1.0.9/uitk/widgets/menu.py
+-rw-rw-rw-   0        0        0     9623 2023-12-23 01:09:52.000000 uitk-1.0.9/uitk/widgets/messageBox.py
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.613873 uitk-1.0.9/uitk/widgets/mixins/
+-rw-rw-rw-   0        0        0     3028 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/mixins/__init__.py
+-rw-rw-rw-   0        0        0    15319 2023-12-22 18:35:52.000000 uitk-1.0.9/uitk/widgets/mixins/attributes.py
+-rw-rw-rw-   0        0        0     4023 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/mixins/convert.py
+-rw-rw-rw-   0        0        0     9499 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/mixins/docking.py
+-rw-rw-rw-   0        0        0    49002 2023-12-17 15:08:52.000000 uitk-1.0.9/uitk/widgets/mixins/style_sheet.py
+-rw-rw-rw-   0        0        0    58215 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/mixins/task_indicator.gif
+-rw-rw-rw-   0        0        0     3409 2023-09-06 12:44:13.000000 uitk-1.0.9/uitk/widgets/mixins/tasks.py
+-rw-rw-rw-   0        0        0    10882 2023-09-12 11:16:33.000000 uitk-1.0.9/uitk/widgets/mixins/text.py
+-rw-rw-rw-   0        0        0     6426 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/optionBox.py
+-rw-rw-rw-   0        0        0     3272 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/progressBar.py
+-rw-rw-rw-   0        0        0     2135 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/pushButton.py
+-rw-rw-rw-   0        0        0     7907 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/region.py
+-rw-rw-rw-   0        0        0     3717 2023-09-18 17:32:03.000000 uitk-1.0.9/uitk/widgets/textEdit.py
+drwxrwxrwx   0        0        0        0 2023-12-23 01:20:50.613873 uitk-1.0.9/uitk.egg-info/
+-rw-rw-rw-   0        0        0     3177 2023-12-23 01:20:50.000000 uitk-1.0.9/uitk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4290 2023-04-06 23:46:30.000000 uitk-1.0.9/uitk.egg-info/PKG-INFO.bak
+-rw-rw-rw-   0        0        0     1154 2023-12-23 01:20:50.000000 uitk-1.0.9/uitk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      768 2023-04-15 12:45:23.000000 uitk-1.0.9/uitk.egg-info/SOURCES.txt.bak
+-rw-rw-rw-   0        0        0        1 2023-12-23 01:20:50.000000 uitk-1.0.9/uitk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-12-23 01:20:50.000000 uitk-1.0.9/uitk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-12-23 01:20:50.000000 uitk-1.0.9/uitk.egg-info/top_level.txt
```

### Comparing `uitk-1.0.8/COPYING.LESSER` & `uitk-1.0.9/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/PKG-INFO` & `uitk-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 1.0.8
+Version: 1.0.9
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: COPYING.LESSER
 Requires-Dist: PySide2
 Requires-Dist: pythontk==0.7.11
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
-[![Version](https://img.shields.io/badge/Version-1.0.8-blue.svg)](https://pypi.org/project/uitk/)
+[![Version](https://img.shields.io/badge/Version-1.0.9-blue.svg)](https://pypi.org/project/uitk/)
 
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using Python3|PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots, styles, states, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
```

### Comparing `uitk-1.0.8/setup.py` & `uitk-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/__init__.py` & `uitk-1.0.9/uitk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import importlib
 import pkgutil
 import inspect
 from uitk.signals import Signals
 
 
 __package__ = "uitk"
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __path__ = [os.path.abspath(os.path.dirname(__file__))]
 
 
 # Define a dictionary to map class names to their respective modules
 CLASS_TO_MODULE = {}
 
 # Build the CLASS_TO_MODULE dictionary by iterating over all submodules of the package
```

### Comparing `uitk-1.0.8/uitk/events.py` & `uitk-1.0.9/uitk/events.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/example/example#submenu.ui` & `uitk-1.0.9/uitk/example/example#submenu.ui`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/example/example.ui` & `uitk-1.0.9/uitk/example/example.ui`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/example/example_slots.py` & `uitk-1.0.9/uitk/example/example_slots.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/file_manager.py` & `uitk-1.0.9/uitk/file_manager.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/signals.py` & `uitk-1.0.9/uitk/signals.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/switchboard.py` & `uitk-1.0.9/uitk/switchboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1642,38 +1642,44 @@
         if type(value) in (int, float):
             result = abs(value) if value < 0 else -value
         elif type(value) == bool:
             result = True if value else False
 
         return result
 
-    def message_box(self, string, message_type="", location="topMiddle", timeout=4):
-        """Spawns a message box with the given text. Supports HTML formatting.
-        Prints a formatted version of the given string to console, stripped of html tags, to the console.
+    def message_box(self, string, *buttons, location="topMiddle", timeout=3):
+        """Spawns a message box with the given text and optionally sets buttons.
 
         Parameters:
-            message_type (str/optional): The message context type. ex. 'Error', 'Warning', 'Info', 'Result'
-            location (str/QPoint/optional) = move the messagebox to the specified location. default is: 'topMiddle'
-                                            valid: "topMiddle", "bottomRight", "topLeft", "bottomLeft", "center"
-            timeout (int/optional): time in seconds before the messagebox auto closes. default is: 4
-        """
-        if message_type:
-            string = f"{message_type.capitalize()}: {string}"
+            string (str): The message to display.
+            *buttons (str): Variable length argument list of buttons to display.
+            location (str/QPoint, optional): The location to move the messagebox to. Default is 'topMiddle'.
+            timeout (int, optional): Time in seconds before the messagebox auto closes. Default is 3.
 
+        Returns:
+            The result of the message box interaction if buttons are provided, None otherwise.
+        """
         if not hasattr(self, "_messageBox"):
             self._messageBox = self.MessageBox(self.parent())
 
         self._messageBox.location = location
         self._messageBox.timeout = timeout
 
-        # strip everything between '<' and '>' (html tags)
+        self._messageBox.setStandardButtons(*buttons)
+
+        # Log text without HTML tags
         self.logger.info(f"# {re.sub('<.*?>', '', string)}")
 
         self._messageBox.setText(string)
-        self._messageBox.show()  # Use show() instead of exec_()
+
+        if buttons:  # If buttons are provided, use exec_() and return the result
+            return self._messageBox.exec_()
+        else:  # If no buttons, use show() and do not wait for a result
+            self._messageBox.show()
+            return None
 
     @staticmethod
     def file_dialog(
         file_types: Union[str, List[str]] = ["*.*"],
         title: str = "Select files to open",
         directory: str = "/home",
         filter_description: str = "All Files",
```

### Comparing `uitk-1.0.8/uitk/ui/example.ui` & `uitk-1.0.9/uitk/ui/example.ui`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/__init__.py` & `uitk-1.0.9/uitk/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/attributeWindow.py` & `uitk-1.0.9/uitk/widgets/attributeWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/checkBox.py` & `uitk-1.0.9/uitk/widgets/checkBox.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/collapsableGroup.py` & `uitk-1.0.9/uitk/widgets/collapsableGroup.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/comboBox.py` & `uitk-1.0.9/uitk/widgets/comboBox.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/expandableList.py` & `uitk-1.0.9/uitk/widgets/expandableList.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/header.py` & `uitk-1.0.9/uitk/widgets/header.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/label.py` & `uitk-1.0.9/uitk/widgets/label.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/lineEdit.py` & `uitk-1.0.9/uitk/widgets/lineEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mainWindow.py` & `uitk-1.0.9/uitk/widgets/mainWindow.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/menu.py` & `uitk-1.0.9/uitk/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/messageBox.py` & `uitk-1.0.9/uitk/widgets/messageBox.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,37 +8,94 @@
     """Displays a message box with HTML formatting for a set time before closing.
 
     Parameters:
         location (str)(point) = move the messagebox to the specified location. Can be given as a qpoint or string value. default is: 'topMiddle'
         timeout (int): time in seconds before the messagebox auto closes.
     """
 
-    def __init__(self, parent=None, location="topMiddle", timeout=2, **kwargs):
+    buttonMapping = {
+        "Ok": QtWidgets.QMessageBox.Ok,
+        "Open": QtWidgets.QMessageBox.Open,
+        "Save": QtWidgets.QMessageBox.Save,
+        "Cancel": QtWidgets.QMessageBox.Cancel,
+        "Close": QtWidgets.QMessageBox.Close,
+        "Discard": QtWidgets.QMessageBox.Discard,
+        "Apply": QtWidgets.QMessageBox.Apply,
+        "Reset": QtWidgets.QMessageBox.Reset,
+        "RestoreDefaults": QtWidgets.QMessageBox.RestoreDefaults,
+        "Help": QtWidgets.QMessageBox.Help,
+        "SaveAll": QtWidgets.QMessageBox.SaveAll,
+        "Yes": QtWidgets.QMessageBox.Yes,
+        "YesToAll": QtWidgets.QMessageBox.YesToAll,
+        "No": QtWidgets.QMessageBox.No,
+        "NoToAll": QtWidgets.QMessageBox.NoToAll,
+        "Abort": QtWidgets.QMessageBox.Abort,
+        "Retry": QtWidgets.QMessageBox.Retry,
+        "Ignore": QtWidgets.QMessageBox.Ignore,
+        "NoButton": QtWidgets.QMessageBox.NoButton,
+        None: QtWidgets.QMessageBox.NoButton,
+    }
+
+    def __init__(
+        self,
+        parent=None,
+        location="topMiddle",
+        align="left",
+        timeout=None,
+        **kwargs,
+    ):
         QtWidgets.QMessageBox.__init__(self, parent)
 
         self.setWindowModality(QtCore.Qt.NonModal)
         self.setStandardButtons(QtWidgets.QMessageBox.NoButton)
         self.setAttribute(QtCore.Qt.WA_TranslucentBackground)
         self.setWindowFlags(
             QtCore.Qt.WindowType.WindowDoesNotAcceptFocus
             | QtCore.Qt.WindowStaysOnTopHint
             | QtCore.Qt.Tool
             | QtCore.Qt.FramelessWindowHint
         )
 
-        self.menu_timer = QtCore.QTimer()
-        self.menu_timer.setSingleShot(True)
-        self.menu_timer.timeout.connect(self.hide)
-
         self.setTextFormat(QtCore.Qt.RichText)
 
         self.location = location
+        self.align = align
+
+        # Always initialize the timer
+        self.menu_timer = QtCore.QTimer(self)
+        self.menu_timer.setSingleShot(True)
+        self.menu_timer.timeout.connect(self.autoClose)
+
+        # Start the timer only if timeout is set and valid
+        if timeout is not None and timeout > 0:
+            self.timeout = timeout
+        else:
+            self.timeout = None
 
         self.set_attributes(**kwargs)
 
+    def setStandardButtons(self, *buttons):
+        """Set the standard buttons for the message box. Defaults to no buttons if none are provided."""
+        if not buttons:
+            # Set to no buttons if none are provided
+            super().setStandardButtons(QtWidgets.QMessageBox.NoButton)
+            return
+
+        standardButtons = QtWidgets.QMessageBox.StandardButtons()
+        for button in buttons:
+            if isinstance(button, str):
+                button = button.capitalize()  # Normalize the string
+                standardButtons |= self.buttonMapping.get(
+                    button, QtWidgets.QMessageBox.NoButton
+                )
+            elif isinstance(button, QtWidgets.QMessageBox.StandardButton):
+                standardButtons |= button
+
+        super().setStandardButtons(standardButtons)
+
     def move_(self, location) -> None:
         # Get the screen's geometry
         screen = QtWidgets.QApplication.screens()[0]
         rect = screen.geometry()
 
         offset_x = self.sizeHint().width() / 2
         offset_y = self.sizeHint().height() / 2
@@ -55,19 +112,15 @@
             point = QtCore.QPoint(
                 rect.width() / 2 - offset_x, rect.height() / 2 - offset_y
             )
 
         self.move(point)
 
     def _setPrefixStyle(self, string) -> str:
-        """Set style for specific keywords in the given string.
-
-        Returns:
-                (str)
-        """
+        """Set style for specific keywords in the given string."""
         style = {
             "Error:": '<hl style="color:red;">Error:</hl>',
             "Warning:": '<hl style="color:yellow;">Warning:</hl>',
             "Note:": '<hl style="color:blue;">Note:</hl>',
             "Result:": '<hl style="color:green;">Result:</hl>',
         }
 
@@ -78,15 +131,15 @@
 
     def _setHTML(self, string) -> str:
         """<p style="font-size:160%;">text</p>
         <p style="text-align:center;">Centered paragraph.</p>
         <p style="font-family:courier;">This is a paragraph.</p>
 
         Returns:
-                (str)
+            (str)
         """
         style = {
             "<p>": '<p style="color:white;">',  # paragraph <p>' </p>'
             "<hl>": '<hl style="color:yellow; font-weight: bold;">',  # heading <h1>' </h1>'
             "<body>": '<body style="color;">',  # body <body> </body>
             "<b>": '<b style="font-weight: bold;">',  # bold <b> </b>
             "<strong>": '<strong style="font-weight: bold;">',  # <strong> </strong>
@@ -95,151 +148,105 @@
 
         for k, v in style.items():
             string = string.replace(k, v)
 
         return string
 
     def _setFontColor(self, string, color) -> str:
-        """
-        Returns:
-                (str)
-        """
+        """ """
         return "<font color=" + color + ">" + string + "</font>"
 
     def _setBackgroundColor(self, string, color):
-        """
-        Returns:
-                (str)
-        """
+        """ """
         return '<mark style="background-color:' + color + '">' + string + "</mark>"
 
     def _setFontSize(self, string, size) -> str:
-        """
-        Returns:
-                (str)
-        """
+        """ """
         return "<font size=" + str(size) + ">" + string + "</font>"
 
     def setText(
         self, string, fontColor="white", backgroundColor="rgb(50,50,50)", fontSize=5
     ) -> None:
-        """Set the text to be displayed.
+        """Set the text to be displayed with the specified alignment unless overridden by HTML.
 
         Parameters:
-                fontColor (str): text color.
-                backgroundColor (str): text background color.
-                fontSize (int): text size.
-        """
+            string (str): The text or HTML content to display.
+            fontColor (str): The text color.
+            backgroundColor (str): The background color of the text.
+            fontSize (int): The font size of the text.
+        """
+        # Apply default alignment if not overridden in the HTML
+        if "align=" not in string:
+            string = f"<div align='{self.align}'>{string}</div>"
+
         s = self._setPrefixStyle(string)
         s = self._setHTML(s)
         s = self._setFontColor(s, fontColor)
         s = self._setBackgroundColor(s, backgroundColor)
         s = self._setFontSize(s, fontSize)
 
         super().setText(s)
 
-    def showEvent(self, event) -> None:
-        """ """
-        self.menu_timer.start(1000)  # 5000 milliseconds = 5 seconds
+    def autoClose(self):
+        # Close the MessageBox if no standard buttons are set
+        if self.standardButtons() == QtWidgets.QMessageBox.NoButton:
+            self.accept()
+
+    def showEvent(self, event):
+        # Start the timer when the MessageBox is shown and a timeout is set
+        if self.timeout is not None:
+            self.menu_timer.start(
+                self.timeout * 1000
+            )  # Convert seconds to milliseconds
         self.move_(self.location)
-
         super().showEvent(event)
 
-    def hideEvent(self, event) -> None:
-        """ """
+    def hideEvent(self, event):
+        # Stop the timer when the MessageBox is hidden
         self.menu_timer.stop()
-
         super().hideEvent(event)
 
+    def exec_(self):
+        # Call the original exec_ method and store the result
+        resultEnum = super().exec_()
+
+        # Convert the enum result to a string using the buttonMapping
+        resultString = next(
+            (k for k, v in MessageBox.buttonMapping.items() if v == resultEnum),
+            None,
+        )
+
+        # Return the string representation of the result
+        return resultString
+
 
 # --------------------------------------------------------------------------------------------
 
 if __name__ == "__main__":
     import sys
 
     # Return the existing QApplication object, or create a new one if none exists.
     app = QtWidgets.QApplication.instance() or QtWidgets.QApplication(sys.argv)
 
     w = MessageBox()
-    w.setText("Warning: Backface Culling is now <hl>Off</hl>")
+    w.setText("Warning: Backface Culling is now <hl>OFF</hl>")
     w.show()
 
     sys.exit(app.exec_())
 
 # --------------------------------------------------------------------------------------------
 # Notes
 # --------------------------------------------------------------------------------------------
 
 """
 Promoting a widget in designer to use a custom class:
->   In Qt Designer, select all the widgets you want to replace, 
-        then right-click them and select 'Promote to...'. 
+>   In Qt Designer, select all the widgets you want to replace,
+        then right-click them and select 'Promote to...'.
 
 >   In the dialog:
         Base Class:     Class from which you inherit. ie. QWidget
         Promoted Class: Name of the class. ie. "MyWidget"
         Header File:    Path of the file (changing the extension .py to .h)  ie. myfolder.mymodule.mywidget.h
 
->   Then click "Add", "Promote", 
+>   Then click "Add", "Promote",
         and you will see the class change from "QWidget" to "MyWidget" in the Object Inspector pane.
 """
-
-# deprecated: -----------------------------------
-
-
-# class ShowMessageBox(MessageBox):
-#     """Spawns a message box with the given text.
-#     Supports HTML formatting.
-#     Prints a formatted version of the given string to console, stripped of html tags, to the console.
-
-#     Parameters:
-#         message_type (str/optional): The message context type. ex. 'Error', 'Warning', 'Info', 'Result'
-#         location (str/QPoint/optional) = move the messagebox to the specified location. default is: 'topMiddle'
-#         timeout (int/optional): time in seconds before the messagebox auto closes. default is: 3
-#     """
-
-#     def __init__(
-#         self,
-#         string,
-#         message_type="",
-#         location="topMiddle",
-#         timeout=3,
-#         **kwargs,
-#     ):
-#         super().__init__(
-#             QtWidgets.QApplication.instance(), **kwargs
-#         )  # Set the QApplication instance as the parent
-
-#         if message_type:
-#             string = f"{message_type.capitalize()}: {string}"
-
-#         self.location = location
-#         self.timeout = timeout
-
-#         self.setText(string)
-#         self.setVisible(True)
-
-#         # strip everything between '<' and '>' (html tags)
-#         print(f"# {re.sub('<.*?>', '', string)}")
-
-#     def hideEvent(self, event) -> None:
-#         """ """
-#         self.menu_timer.stop()
-
-#         super().hideEvent(event)
-
-
-# def insertText(self, dict_):
-#   '''
-#   Parameters:
-#       dict_ = {dict} - contents to add.  for each key if there is a value, the key and value pair will be added.
-#   '''
-#   highlight = QtGui.QColor(255, 255, 0)
-#   baseColor = QtGui.QColor(185, 185, 185)
-
-#   #populate the textedit with any values
-#   for key, value in dict_.items():
-#       if value:
-#           self.setTextColor(baseColor)
-#           self.append(key) #textEdit.append(key+str(value))
-#           self.setTextColor(highlight)
-#           self.insertPlainText(str(value))
```

### Comparing `uitk-1.0.8/uitk/widgets/mixins/__init__.py` & `uitk-1.0.9/uitk/widgets/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/attributes.py` & `uitk-1.0.9/uitk/widgets/mixins/attributes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,50 @@
 # !/usr/bin/python
 # coding=utf-8
 from PySide2 import QtCore, QtGui, QtWidgets
 import pythontk as ptk
 
 
 class AttributesMixin:
-    """Methods for setting widget AttributesMixin."""
+    """A mixin class providing a comprehensive interface for setting attributes on Qt widgets.
+    It allows setting of standard widget properties, calling methods, connecting signals to callbacks,
+    and handling custom-defined attributes.
+
+    The class defines several utility methods:
+
+    - set_legal_attribute: Handles setting of attributes even when the attribute names contain illegal characters,
+      by converting these names into legal formats. It can also retain the original attribute name if required.
+
+    - set_attributes: The primary method used for setting a range of attributes on one or more widgets.
+      This method intelligently distinguishes between regular attributes, method calls, and signal connections,
+      routing each type to its specific handling procedure.
+
+    - is_signal: Checks if a given attribute name corresponds to a Qt signal on the widget.
+
+    - connect_signal: Connects Qt signals to specified callback functions.
+
+    - set_attribute_or_call_method: Handles setting standard attributes and calling methods on widgets.
+
+    - set_custom_attribute: A flexible method designed to set custom attributes. This method can be
+      overridden or extended in subclasses to accommodate specific custom attributes beyond the standard Qt attributes.
+
+    Usage:
+    - Objects of this mixin class or its subclasses can set attributes on Qt widgets by calling `set_attributes`
+      with appropriate parameters.
+    - The class is designed to work as a mixin with Qt widgets or other classes in a Qt application,
+      enhancing them with versatile attribute setting capabilities.
+
+    Example:
+    ```
+    class MyWidget(QtWidgets.QWidget, AttributesMixin):
+        def __init__(self):
+            super().__init__()
+            self.set_attributes(self, setWindowTitle="My Application", set_size=(200, 100))
+    ```
+    """
 
     def set_legal_attribute(self, obj, name, value, also_set_original=False):
         """If the original name contains illegal characters, this method sets an attribute using
         a legal name created by replacing illegal characters with underscores. The original name
         attribute is also assigned if also_set_original is True.
 
         Parameters:
@@ -27,40 +62,52 @@
             setattr(obj, legal_name, value)
             if also_set_original:
                 setattr(obj, name, value)
         else:
             setattr(obj, name, value)
 
     def set_attributes(self, *objects, **attributes):
-        """Works with attributes passed in as kwargs.
-        If objects are passed in, attributes are set for each object in turn.
-
-        Parameters:
-            *objects: the child objects or widgetActions to set attributes for. If none are provided, defaults to self.
-            **attributes: The keyword arguments to set as attributes.
-        """
-        if not attributes:  # if no attributes given.
+        if not attributes:
             return
 
         if not objects:
             objects = (self,)
 
         for obj in objects:
             for attr, value in attributes.items():
-                try:
-                    # Check if the attribute is a window attribute
-                    attr_value = getattr(QtCore.Qt, attr)
-                    obj.setAttribute(attr_value, value)
-                except AttributeError:
-                    try:
-                        # Attempt to call the attribute as a method
-                        getattr(obj, attr)(value)
-                    except AttributeError:
-                        # Pass attribute to set_custom_attribute if it does not exist
-                        self.set_custom_attribute(obj, attr, value)
+                if self.is_signal(obj, attr):
+                    self.connect_signal(obj, attr, value)
+                else:
+                    self.set_attribute_or_call_method(obj, attr, value)
+
+    def is_signal(self, obj, attr_name):
+        """Check if an attribute is a signal."""
+        attr = getattr(obj, attr_name, None)
+        return isinstance(attr, QtCore.Signal)
+
+    def connect_signal(self, obj, signal_name, callback):
+        """Connect a signal to a callback function."""
+        signal = getattr(obj, signal_name, None)
+        if signal and isinstance(signal, QtCore.Signal):
+            signal.connect(callback)
+        else:
+            print(f"Error: {obj} has no signal named {signal_name}")
+
+    def set_attribute_or_call_method(self, obj, attr, value):
+        try:
+            # Check if the attribute is a window attribute
+            attr_value = getattr(QtCore.Qt, attr)
+            obj.setAttribute(attr_value, value)
+        except AttributeError:
+            try:
+                # Attempt to call the attribute as a method
+                getattr(obj, attr)(value)
+            except AttributeError:
+                # Pass attribute to set_custom_attribute if it does not exist
+                self.set_custom_attribute(obj, attr, value)
 
     def set_custom_attribute(self, w, attr, value):
         """AttributesMixin that throw an AttributeError in 'set_attributes' are sent here, where they can be assigned a value.
         Custom attributes can be set using a trailing underscore convention to aid readability, and differentiate them from standard attributes.
 
         Parameters:
             w (obj): The child widget or widgetAction to set attributes for.
```

### Comparing `uitk-1.0.8/uitk/widgets/mixins/convert.py` & `uitk-1.0.9/uitk/widgets/mixins/convert.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/docking.py` & `uitk-1.0.9/uitk/widgets/mixins/docking.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/style_sheet.py` & `uitk-1.0.9/uitk/widgets/mixins/style_sheet.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/task_indicator.gif` & `uitk-1.0.9/uitk/widgets/mixins/task_indicator.gif`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/tasks.py` & `uitk-1.0.9/uitk/widgets/mixins/tasks.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/mixins/text.py` & `uitk-1.0.9/uitk/widgets/mixins/text.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/optionBox.py` & `uitk-1.0.9/uitk/widgets/optionBox.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/progressBar.py` & `uitk-1.0.9/uitk/widgets/progressBar.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/pushButton.py` & `uitk-1.0.9/uitk/widgets/pushButton.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/region.py` & `uitk-1.0.9/uitk/widgets/region.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk/widgets/textEdit.py` & `uitk-1.0.9/uitk/widgets/textEdit.py`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk.egg-info/PKG-INFO` & `uitk-1.0.9/uitk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: uitk
-Version: 1.0.8
+Version: 1.0.9
 Home-page: https://github.com/m3trik/uitk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 License: LGPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: COPYING.LESSER
 Requires-Dist: PySide2
 Requires-Dist: pythontk==0.7.11
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0.en.html)
-[![Version](https://img.shields.io/badge/Version-1.0.8-blue.svg)](https://pypi.org/project/uitk/)
+[![Version](https://img.shields.io/badge/Version-1.0.9-blue.svg)](https://pypi.org/project/uitk/)
 
 # UITK: Dynamic UI Management for Python with PySide2
 
 UITK is a comprehensive Python package designed to streamline the creation, management, and interaction of user interfaces (UIs) using Python3|PySide2. With a focus on versatility, UITK leverages a naming convention-based switchboard module to dynamically load UI files, register custom widgets, manage slots, styles, states, and facilitate interaction with widgets. The primary goal of UITK is to simplify the development process of complex UIs and enhance the efficiency of event handling.
 
 ## Key Features
```

### Comparing `uitk-1.0.8/uitk.egg-info/PKG-INFO.bak` & `uitk-1.0.9/uitk.egg-info/PKG-INFO.bak`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk.egg-info/SOURCES.txt` & `uitk-1.0.9/uitk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uitk-1.0.8/uitk.egg-info/SOURCES.txt.bak` & `uitk-1.0.9/uitk.egg-info/SOURCES.txt.bak`

 * *Files identical despite different names*

