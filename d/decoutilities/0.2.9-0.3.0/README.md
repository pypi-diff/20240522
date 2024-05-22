# Comparing `tmp/decoutilities-0.2.9.tar.gz` & `tmp/decoutilities-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.9.tar", last modified: Tue May 21 06:17:47 2024, max compression
+gzip compressed data, was "decoutilities-0.3.0.tar", last modified: Tue May 21 11:51:47 2024, max compression
```

## Comparing `decoutilities-0.2.9.tar` & `decoutilities-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.777485 decoutilities-0.2.9/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.9/LICENSE
--rw-rw-rw-   0        0        0    15668 2024-05-21 06:17:47.765488 decoutilities-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.342487 decoutilities-0.2.9/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.9/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.507487 decoutilities-0.2.9/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.9/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.9/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.9/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.577489 decoutilities-0.2.9/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.9/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.9/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.9/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.613488 decoutilities-0.2.9/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.9/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.9/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.625488 decoutilities-0.2.9/decoutilities/logger/
--rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.2.9/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.682487 decoutilities-0.2.9/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.9/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.701488 decoutilities-0.2.9/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.2.9/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.720487 decoutilities-0.2.9/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    15668 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-21 06:17:47.000000 decoutilities-0.2.9/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 06:17:47.778488 decoutilities-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-21 05:29:14.000000 decoutilities-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.610144 decoutilities-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    17243 2024-05-21 11:51:47.598144 decoutilities-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    16760 2024-05-21 11:50:42.000000 decoutilities-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.205405 decoutilities-0.3.0/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.3.0/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.389418 decoutilities-0.3.0/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.3.0/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.3.0/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.3.0/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.436144 decoutilities-0.3.0/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.3.0/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.3.0/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.3.0/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.459145 decoutilities-0.3.0/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.3.0/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.3.0/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.475147 decoutilities-0.3.0/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.3.0/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.505145 decoutilities-0.3.0/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.3.0/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.520144 decoutilities-0.3.0/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.3.0/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.560145 decoutilities-0.3.0/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    17243 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 11:51:47.613144 decoutilities-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-21 06:49:21.000000 decoutilities-0.3.0/setup.py
```

### Comparing `decoutilities-0.2.9/LICENSE` & `decoutilities-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/PKG-INFO` & `decoutilities-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.9
+Version: 0.3.0
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # decoutilities
 
-A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
+A simple python package that allows using decorators for multiple things like easily setting up a singleton or a configuration file for your app.
 
 ## Installation
 
 You can install `decoutilities` using pip:
 
 ```bash
 pip install decoutilities
@@ -387,54 +387,59 @@
 
 ## Text Utilities
 
 The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
 
 ### Usage
 
-To use this class, you first need to create an instance of `textUtils`:
+To use this class, you must not initialize it, otherwise it will throw an error.
 
 ```python
-text_utils = textUtils()
-```
+from decoutilities.textUtils import color, formated, decorate
+from decoutilities.textUtils import format as textFormat # Recommended importing with other name to prevent conflicts with python's default format funcion
 
-You can then use the `color`, `decorate`, and `format` methods to format your text:
+print(color("red", "This is a red-colored text!"))
+print(decorate("bold", "This is a bold text!"))
 
-```python
-# Color text
-colored_text = text_utils.color('red', 'Hello, World!')
+# You can make also a function always output a formated string
+@formated
+def pig()
+    return "{purple}Oink Oink!"
 
-# Decorate text
-bold_text = text_utils.decorate('bold', 'Hello, World!')
+print(pig())
 
-# Format text
-formatted_text = text_utils.format('bold red Hello, World!')
+# Or use the format function!
+print(textFormat("Hello my {red}red{reset}friends! Ready for a {bold}new {reset}adventure?"))
 ```
 
 ### Methods
 
 - `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
 
 - `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
 
 - `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
 
+- `@formated`: Decorator used to make a function's output return always a colorful string.
+
 ### Notes
 
 The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
 
 ## Logger
 
 The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
 
 ### Usage
 
 To use this class, you first need to create an instance of `Logger`:
 
 ```python
+from decoutilities.logger import Logger
+
 logger = Logger(prefix='MyApp', debug=True, log='app.log')
 ```
 
 You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
 
 ```python
 # Log an info message
@@ -467,14 +472,52 @@
 
 ### Notes
 
 The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
 
 If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
 
+## Components
+
+Â´decoutilitiesÂ´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
+
+### Selector
+
+The `Selector` component allows to make selections of only ONE item, here is a piece of code.
+
+```python
+from decoutilities.components import Selector
+from decoutilities.textUtils import format as color # The method to import directly was added on 0.2.9
+
+database = Selector("Please choose a database:", ["{green}MongoDB", "{blue}MariaDB", "{gold}MySQL"])
+
+result = database.display()
+
+print(color("{bold}You selected: "+result))
+```
+
+### Checkmarks
+
+Also, as the `Selector` feature, this one works the same way.
+
+```python
+from decoutilities.components import Checkmark
+
+features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| ðŸŸ©", "| â¬›"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
+
+selected = features.display()
+
+print(selected)
+
+```
+
+### Input
+
+This feature is still under development.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoutilities-0.2.9/README.md` & `decoutilities-0.3.0/decoutilities.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,23 @@
+Metadata-Version: 2.1
+Name: decoutilities
+Version: 0.3.0
+Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
+Author: Hugo Torres
+Author-email: contact@redactado.es
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # decoutilities
 
-A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
+A simple python package that allows using decorators for multiple things like easily setting up a singleton or a configuration file for your app.
 
 ## Installation
 
 You can install `decoutilities` using pip:
 
 ```bash
 pip install decoutilities
@@ -374,54 +387,59 @@
 
 ## Text Utilities
 
 The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
 
 ### Usage
 
-To use this class, you first need to create an instance of `textUtils`:
+To use this class, you must not initialize it, otherwise it will throw an error.
 
 ```python
-text_utils = textUtils()
-```
+from decoutilities.textUtils import color, formated, decorate
+from decoutilities.textUtils import format as textFormat # Recommended importing with other name to prevent conflicts with python's default format funcion
 
-You can then use the `color`, `decorate`, and `format` methods to format your text:
+print(color("red", "This is a red-colored text!"))
+print(decorate("bold", "This is a bold text!"))
 
-```python
-# Color text
-colored_text = text_utils.color('red', 'Hello, World!')
+# You can make also a function always output a formated string
+@formated
+def pig()
+    return "{purple}Oink Oink!"
 
-# Decorate text
-bold_text = text_utils.decorate('bold', 'Hello, World!')
+print(pig())
 
-# Format text
-formatted_text = text_utils.format('bold red Hello, World!')
+# Or use the format function!
+print(textFormat("Hello my {red}red{reset}friends! Ready for a {bold}new {reset}adventure?"))
 ```
 
 ### Methods
 
 - `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
 
 - `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
 
 - `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
 
+- `@formated`: Decorator used to make a function's output return always a colorful string.
+
 ### Notes
 
 The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
 
 ## Logger
 
 The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
 
 ### Usage
 
 To use this class, you first need to create an instance of `Logger`:
 
 ```python
+from decoutilities.logger import Logger
+
 logger = Logger(prefix='MyApp', debug=True, log='app.log')
 ```
 
 You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
 
 ```python
 # Log an info message
@@ -454,14 +472,52 @@
 
 ### Notes
 
 The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
 
 If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
 
+## Components
+
+Â´decoutilitiesÂ´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
+
+### Selector
+
+The `Selector` component allows to make selections of only ONE item, here is a piece of code.
+
+```python
+from decoutilities.components import Selector
+from decoutilities.textUtils import format as color # The method to import directly was added on 0.2.9
+
+database = Selector("Please choose a database:", ["{green}MongoDB", "{blue}MariaDB", "{gold}MySQL"])
+
+result = database.display()
+
+print(color("{bold}You selected: "+result))
+```
+
+### Checkmarks
+
+Also, as the `Selector` feature, this one works the same way.
+
+```python
+from decoutilities.components import Checkmark
+
+features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| ðŸŸ©", "| â¬›"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
+
+selected = features.display()
+
+print(selected)
+
+```
+
+### Input
+
+This feature is still under development.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
@@ -482,8 +538,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoutilities-0.2.9/decoutilities/__init__.py` & `decoutilities-0.3.0/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/config/config.py` & `decoutilities-0.3.0/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/config/configContainer.py` & `decoutilities-0.3.0/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/data/dataEncryptor.py` & `decoutilities-0.3.0/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/data/keyManager.py` & `decoutilities-0.3.0/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/inject/injector.py` & `decoutilities-0.3.0/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/logger/__init__.py` & `decoutilities-0.3.0/decoutilities/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/queue/__init__.py` & `decoutilities-0.3.0/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities/textUtils/__init__.py` & `decoutilities-0.3.0/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,10 @@
-Metadata-Version: 2.1
-Name: decoutilities
-Version: 0.2.9
-Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
-Author: Hugo Torres
-Author-email: contact@redactado.es
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # decoutilities
 
-A simple python package that allows using decorators for multiple things like easily setting up singleton or config files.
+A simple python package that allows using decorators for multiple things like easily setting up a singleton or a configuration file for your app.
 
 ## Installation
 
 You can install `decoutilities` using pip:
 
 ```bash
 pip install decoutilities
@@ -387,54 +374,59 @@
 
 ## Text Utilities
 
 The `textUtils` class provides methods for formatting and decorating text in the console. It includes methods for coloring text, adding decorations such as bold, underline, and italic, and a general format method that replaces aliases with their corresponding ANSI escape codes.
 
 ### Usage
 
-To use this class, you first need to create an instance of `textUtils`:
+To use this class, you must not initialize it, otherwise it will throw an error.
 
 ```python
-text_utils = textUtils()
-```
+from decoutilities.textUtils import color, formated, decorate
+from decoutilities.textUtils import format as textFormat # Recommended importing with other name to prevent conflicts with python's default format funcion
 
-You can then use the `color`, `decorate`, and `format` methods to format your text:
+print(color("red", "This is a red-colored text!"))
+print(decorate("bold", "This is a bold text!"))
 
-```python
-# Color text
-colored_text = text_utils.color('red', 'Hello, World!')
+# You can make also a function always output a formated string
+@formated
+def pig()
+    return "{purple}Oink Oink!"
 
-# Decorate text
-bold_text = text_utils.decorate('bold', 'Hello, World!')
+print(pig())
 
-# Format text
-formatted_text = text_utils.format('bold red Hello, World!')
+# Or use the format function!
+print(textFormat("Hello my {red}red{reset}friends! Ready for a {bold}new {reset}adventure?"))
 ```
 
 ### Methods
 
 - `color(color, text)`: Colors the text with the specified color. The available colors are: red, green, yellow, blue, purple, cyan, white, dark_red, dark_green, gold, gray, dark_gray, black, and reset.
 
 - `decorate(decoration, text)`: Decorates the text with the specified decoration. The available decorations are: bold, underline, and italic.
 
 - `format(text)`: Replaces aliases in the text with their corresponding ANSI escape codes. The available aliases are the same as the colors and decorations listed above.
 
+- `@formated`: Decorator used to make a function's output return always a colorful string.
+
 ### Notes
 
 The `format` method applies the ANSI escape codes in the order they appear in the text. If the same alias appears multiple times in the text, all instances will be replaced. The `reset` alias resets all formatting, so it can be used to stop the effect of a previous alias.
 
 ## Logger
 
 The `Logger` class provides methods for logging events and messages with different levels of severity. It includes methods for logging info, warning, error, success, debug, and announcement messages. The messages can be formatted using the `textUtils` class and can optionally be written to a log file.
 
 ### Usage
 
 To use this class, you first need to create an instance of `Logger`:
 
 ```python
+from decoutilities.logger import Logger
+
 logger = Logger(prefix='MyApp', debug=True, log='app.log')
 ```
 
 You can then use the `info`, `warning`, `error`, `success`, `debug`, and `announce` methods to log messages:
 
 ```python
 # Log an info message
@@ -467,14 +459,52 @@
 
 ### Notes
 
 The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
 
 If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
 
+## Components
+
+´decoutilities´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
+
+### Selector
+
+The `Selector` component allows to make selections of only ONE item, here is a piece of code.
+
+```python
+from decoutilities.components import Selector
+from decoutilities.textUtils import format as color # The method to import directly was added on 0.2.9
+
+database = Selector("Please choose a database:", ["{green}MongoDB", "{blue}MariaDB", "{gold}MySQL"])
+
+result = database.display()
+
+print(color("{bold}You selected: "+result))
+```
+
+### Checkmarks
+
+Also, as the `Selector` feature, this one works the same way.
+
+```python
+from decoutilities.components import Checkmark
+
+features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| 🟩", "| ⬛"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
+
+selected = features.display()
+
+print(selected)
+
+```
+
+### Input
+
+This feature is still under development.
+
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
 ### REMEMBER:
@@ -495,8 +525,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `decoutilities-0.2.9/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.3.0/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.9/setup.py` & `decoutilities-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.9',
+version='0.3.0',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

