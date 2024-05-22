# Comparing `tmp/mloggers-1.3.3.tar.gz` & `tmp/mloggers-1.3.4.tar.gz`

## Comparing `mloggers-1.3.3.tar` & `mloggers-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.3/.taplo.toml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 mloggers-1.3.3/log.json
--rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.3/test.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 mloggers-1.3.3/test.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/__init__.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/_log_levels.py
--rw-r--r--   0        0        0     3246 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/console_logger.py
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/file_logger.py
--rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/logger.py
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/multi_logger.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/optional_logger.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/progress.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/utils.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 mloggers-1.3.3/mloggers/wandb_logger.py
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.3/.gitignore
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.3/LICENSE
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.3/README.md
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mloggers-1.3.3/pyproject.toml
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 mloggers-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 mloggers-1.3.4/.taplo.toml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 mloggers-1.3.4/log.json
+-rw-r--r--   0        0        0    23530 2020-02-02 00:00:00.000000 mloggers-1.3.4/test.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 mloggers-1.3.4/test.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/__init__.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/_log_levels.py
+-rw-r--r--   0        0        0     3774 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/console_logger.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/file_logger.py
+-rw-r--r--   0        0        0     9649 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/logger.py
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/multi_logger.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/optional_logger.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/progress.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/utils.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 mloggers-1.3.4/mloggers/wandb_logger.py
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 mloggers-1.3.4/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 mloggers-1.3.4/LICENSE
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 mloggers-1.3.4/README.md
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 mloggers-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 mloggers-1.3.4/PKG-INFO
```

### Comparing `mloggers-1.3.3/log.json` & `mloggers-1.3.4/log.json`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/test.ipynb` & `mloggers-1.3.4/test.ipynb`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/_log_levels.py` & `mloggers-1.3.4/mloggers/_log_levels.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/console_logger.py` & `mloggers-1.3.4/mloggers/console_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import json
 from datetime import datetime
 from typing import Any
 
 import numpy.typing as npt
 from termcolor import colored
 
 from mloggers._log_levels import LogLevel, _log_level_properties
 from mloggers.logger import Logger
+from mloggers.utils import serialize
 
 
 class ConsoleLogger(Logger):
     """Logs to the console (i.e., standard I/O)."""
 
     def __init__(self, default_priority: LogLevel = LogLevel.INFO):  # type:ignore[reportArgumentType]
         super().__init__(default_priority)
@@ -38,31 +38,29 @@
 
             # Color the level string
             if isinstance(level, LogLevel):
                 level_clr = colored(level_str, _log_level_properties[level].color)  # type:ignore[reportArgumentType]
             else:
                 level_clr = colored(level_str, "green")
 
-        # The first level of the dictionary is printed as a multiline
-        # indented message.
-        # The rest of the levels are printed as a single line
-        # prettifyed depending on the type of the value.
+        # The first level of the dictionary is printed as a multiline indented message.
+        # The rest of the levels are printed as a single line prettifyed depending on the type of the value.
 
         # Handle multiple messages
         if len(messages) > 1:
             messages = list(messages)
-            # If the messages are strings, join them into a single string.
+            # If the messages are strings, join them into a single string
             if all(
                 hasattr(message, "__str__")
                 and callable(getattr(message, "__str__"))
                 and not isinstance(message, dict)
                 for message in messages
             ):
                 messages = " ".join([str(message) for message in messages])
-            # If the messages are dictionaries, log them separately.
+            # If the messages are dictionaries, log them separately
             else:
                 for message in messages:
                     self.log(message, level=level)
                 return
         else:
             messages = messages[0]
 
@@ -71,19 +69,32 @@
             for key, value in messages.items():
                 if not first:
                     time = " " * len(time)
                     level_clr = " " * len(level_str)
 
                 if isinstance(value, float):
                     print(f"{level_clr}{time} {key}: {value:.5f}")
-                elif isinstance(value, dict | list):
-                    value = json.dumps(value, indent=4)
-                    print(f"{level_clr}{time} {key}: {value}")
                 elif value is None:  # Used for headers, titles, etc.
                     print(f"{level_clr}{time} {key}")
                 else:
-                    print(f"{level_clr}{time} {key}: {value}")
+                    try:
+                        value = serialize(value)
+                        print(f"{level_clr}{time} {key}: {value}")
+                    except TypeError as e:
+                        print(
+                            f'{colored("[ERROR]", "red")} [ConsoleLogger] Could not convert the message to a JSON serializable format: {e}'
+                        )
+                        continue
 
                 first = False
 
         elif hasattr(messages, "__str__") and callable(getattr(messages, "__str__")):
             print(f"{level_clr}{time} {str(messages)}")
+
+        else:
+            try:
+                serialized = serialize(messages)
+                print(f"{level_clr}{time} {serialized}")
+            except TypeError as e:
+                print(
+                    f'{colored("[ERROR]", "red")} [ConsoleLogger] Could not convert the message to a JSON serializable format: {e}'
+                )
```

### Comparing `mloggers-1.3.3/mloggers/file_logger.py` & `mloggers-1.3.4/mloggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/logger.py` & `mloggers-1.3.4/mloggers/logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/multi_logger.py` & `mloggers-1.3.4/mloggers/multi_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/optional_logger.py` & `mloggers-1.3.4/mloggers/optional_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/progress.py` & `mloggers-1.3.4/mloggers/progress.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/utils.py` & `mloggers-1.3.4/mloggers/utils.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/mloggers/wandb_logger.py` & `mloggers-1.3.4/mloggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/.gitignore` & `mloggers-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/LICENSE` & `mloggers-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/README.md` & `mloggers-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mloggers-1.3.3/pyproject.toml` & `mloggers-1.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mloggers"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     { name = "Sergio Hernandez Gutierrez", email = "contact.sergiohernandez@gmail.com" },
     { name = "Matteo Merler", email = "matteo.merler@gmail.com" },
 ]
 description = "A collection of loggers well-suited for machine learning experiments."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `mloggers-1.3.3/PKG-INFO` & `mloggers-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mloggers
-Version: 1.3.3
+Version: 1.3.4
 Summary: A collection of loggers well-suited for machine learning experiments.
 Project-URL: Homepage, https://github.com/serhez/mloggers
 Project-URL: Issues, https://github.com/serhez/mloggers/issues
 Author-email: Sergio Hernandez Gutierrez <contact.sergiohernandez@gmail.com>, Matteo Merler <matteo.merler@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

