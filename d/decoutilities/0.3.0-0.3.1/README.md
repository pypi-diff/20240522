# Comparing `tmp/decoutilities-0.3.0.tar.gz` & `tmp/decoutilities-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.3.0.tar", last modified: Tue May 21 11:51:47 2024, max compression
+gzip compressed data, was "decoutilities-0.3.1.tar", last modified: Wed May 22 10:32:12 2024, max compression
```

## Comparing `decoutilities-0.3.0.tar` & `decoutilities-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.610144 decoutilities-0.3.0/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.3.0/LICENSE
--rw-rw-rw-   0        0        0    17243 2024-05-21 11:51:47.598144 decoutilities-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    16760 2024-05-21 11:50:42.000000 decoutilities-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.205405 decoutilities-0.3.0/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.3.0/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.389418 decoutilities-0.3.0/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.3.0/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.3.0/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.3.0/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.436144 decoutilities-0.3.0/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.3.0/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.3.0/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.3.0/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.459145 decoutilities-0.3.0/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.3.0/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.3.0/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.475147 decoutilities-0.3.0/decoutilities/logger/
--rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.3.0/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.505145 decoutilities-0.3.0/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.3.0/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.520144 decoutilities-0.3.0/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.3.0/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 11:51:47.560145 decoutilities-0.3.0/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    17243 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 11:51:46.000000 decoutilities-0.3.0/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 11:51:47.613144 decoutilities-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-21 06:49:21.000000 decoutilities-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.674676 decoutilities-0.3.1/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0    19893 2024-05-22 10:32:12.658675 decoutilities-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    19410 2024-05-22 10:30:33.000000 decoutilities-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.102678 decoutilities-0.3.1/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.3.1/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.325675 decoutilities-0.3.1/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.3.1/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.3.1/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.3.1/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.449679 decoutilities-0.3.1/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.3.1/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.3.1/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.3.1/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.507673 decoutilities-0.3.1/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.3.1/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.3.1/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.551674 decoutilities-0.3.1/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.3.1/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.597676 decoutilities-0.3.1/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.3.1/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.614677 decoutilities-0.3.1/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.3.1/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:32:12.627679 decoutilities-0.3.1/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    19893 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-22 10:32:11.000000 decoutilities-0.3.1/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:32:12.675674 decoutilities-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-22 10:30:56.000000 decoutilities-0.3.1/setup.py
```

### Comparing `decoutilities-0.3.0/LICENSE` & `decoutilities-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/PKG-INFO` & `decoutilities-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.3.0
+Version: 0.3.1
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -506,17 +506,81 @@
 
 selected = features.display()
 
 print(selected)
 
 ```
 
+
 ### Input
 
-This feature is still under development.
+The `Input` class is a utility for creating interactive console inputs with validation rules. 
+
+#### Importing the Class
+
+```python
+from decoutilities.components import Input
+```
+
+#### Creating an Instance
+
+```python
+name = Input('Password', '', 'REQUIRED|PASSWORD', 'The text is hidden')
+```
+
+#### Displaying the Input
+
+```python
+name.display()
+```
+
+#### Validation Rules
+
+The `Input` class supports a variety of validation rules. These rules are passed as a string when creating an instance of the class. Multiple rules can be combined using the pipe character (`|`).
+
+Here are the available rules and their usage:
+
+- `REQUIRED`: The input must not be empty.
+- `PASSWORD`: The input will be hidden.
+- `EMAIL`: The input must be a valid email address.
+- `NUMBER`: The input must be a number.
+- `STRING`: The input must be a string.
+- `MIN:<number>`: The input must be at least `<number>` characters long.
+- `MAX:<number>`: The input must be at most `<number>` characters long.
+- `LENGTH:<number>`: The input must be exactly `<number>` characters long.
+- `REGEX:<pattern>`: The input must match the regex `<pattern>`.
+- `CONTAINS:<value>`: The input must contain `<value>`.
+- `NOT_CONTAINS:<value>`: The input must not contain `<value>`.
+- `IN:<value1,value2,...>`: The input must be one of the specified values.
+- `NOT_IN:<value1,value2,...>`: The input must not be one of the specified values.
+- `EQUALS:<value>`: The input must be equal to `<value>`.
+- `NOT_EQUALS:<value>`: The input must not be equal to `<value>`.
+- `HIGHER:<number>`: The input must be higher than `<number>`.
+- `LOWER:<number>`: The input must be lower than `<number>`.
+- `HIGHER_OR_EQUAL:<number>`: The input must be higher or equal to `<number>`.
+- `LOWER_OR_EQUAL:<number>`: The input must be lower or equal to `<number>`.
+- `FLOAT`: The input must be a float.
+- `BOOLEAN`: The input must be a boolean (`true` or `false`).
+- `JSON`: The input must be a valid JSON string.
+- `IP`: The input must be a valid IP address.
+- `URL`: The input must be a valid URL.
+- `DATE`: The input must be a valid date (`YYYY-MM-DD`).
+- `TIME`: The input must be a valid time (`HH:MM:SS`).
+- `DATETIME`: The input must be a valid datetime (`YYYY-MM-DD HH:MM:SS`).
+- `PHONE`: The input must be a valid phone number (10 digits).
+- `PASSWORD`: The input must be a valid password (Minimum eight characters, at least one uppercase letter, one lowercase letter, one number and one special character).
+
+#### Example
+
+```python
+email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
+email.display()
+```
+
+This will create an input that requires a valid email address.
 
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
```

### Comparing `decoutilities-0.3.0/README.md` & `decoutilities-0.3.1/decoutilities.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: decoutilities
+Version: 0.3.1
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
 
 A simple python package that allows using decorators for multiple things like easily setting up a singleton or a configuration file for your app.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -461,15 +474,15 @@
 
 The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
 
 If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
 
 ## Components
 
-´decoutilities´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
+Â´decoutilitiesÂ´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
 
 ### Selector
 
 The `Selector` component allows to make selections of only ONE item, here is a piece of code.
 
 ```python
 from decoutilities.components import Selector
@@ -485,25 +498,89 @@
 ### Checkmarks
 
 Also, as the `Selector` feature, this one works the same way.
 
 ```python
 from decoutilities.components import Checkmark
 
-features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| 🟩", "| ⬛"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
+features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| ðŸŸ©", "| â¬›"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
 
 selected = features.display()
 
 print(selected)
 
 ```
 
+
 ### Input
 
-This feature is still under development.
+The `Input` class is a utility for creating interactive console inputs with validation rules. 
+
+#### Importing the Class
+
+```python
+from decoutilities.components import Input
+```
+
+#### Creating an Instance
+
+```python
+name = Input('Password', '', 'REQUIRED|PASSWORD', 'The text is hidden')
+```
+
+#### Displaying the Input
+
+```python
+name.display()
+```
+
+#### Validation Rules
+
+The `Input` class supports a variety of validation rules. These rules are passed as a string when creating an instance of the class. Multiple rules can be combined using the pipe character (`|`).
+
+Here are the available rules and their usage:
+
+- `REQUIRED`: The input must not be empty.
+- `PASSWORD`: The input will be hidden.
+- `EMAIL`: The input must be a valid email address.
+- `NUMBER`: The input must be a number.
+- `STRING`: The input must be a string.
+- `MIN:<number>`: The input must be at least `<number>` characters long.
+- `MAX:<number>`: The input must be at most `<number>` characters long.
+- `LENGTH:<number>`: The input must be exactly `<number>` characters long.
+- `REGEX:<pattern>`: The input must match the regex `<pattern>`.
+- `CONTAINS:<value>`: The input must contain `<value>`.
+- `NOT_CONTAINS:<value>`: The input must not contain `<value>`.
+- `IN:<value1,value2,...>`: The input must be one of the specified values.
+- `NOT_IN:<value1,value2,...>`: The input must not be one of the specified values.
+- `EQUALS:<value>`: The input must be equal to `<value>`.
+- `NOT_EQUALS:<value>`: The input must not be equal to `<value>`.
+- `HIGHER:<number>`: The input must be higher than `<number>`.
+- `LOWER:<number>`: The input must be lower than `<number>`.
+- `HIGHER_OR_EQUAL:<number>`: The input must be higher or equal to `<number>`.
+- `LOWER_OR_EQUAL:<number>`: The input must be lower or equal to `<number>`.
+- `FLOAT`: The input must be a float.
+- `BOOLEAN`: The input must be a boolean (`true` or `false`).
+- `JSON`: The input must be a valid JSON string.
+- `IP`: The input must be a valid IP address.
+- `URL`: The input must be a valid URL.
+- `DATE`: The input must be a valid date (`YYYY-MM-DD`).
+- `TIME`: The input must be a valid time (`HH:MM:SS`).
+- `DATETIME`: The input must be a valid datetime (`YYYY-MM-DD HH:MM:SS`).
+- `PHONE`: The input must be a valid phone number (10 digits).
+- `PASSWORD`: The input must be a valid password (Minimum eight characters, at least one uppercase letter, one lowercase letter, one number and one special character).
+
+#### Example
+
+```python
+email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
+email.display()
+```
+
+This will create an input that requires a valid email address.
 
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
@@ -525,8 +602,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.3.0/decoutilities/__init__.py` & `decoutilities-0.3.1/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/config/config.py` & `decoutilities-0.3.1/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/config/configContainer.py` & `decoutilities-0.3.1/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/data/dataEncryptor.py` & `decoutilities-0.3.1/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/data/keyManager.py` & `decoutilities-0.3.1/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/inject/injector.py` & `decoutilities-0.3.1/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/logger/__init__.py` & `decoutilities-0.3.1/decoutilities/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/queue/__init__.py` & `decoutilities-0.3.1/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities/textUtils/__init__.py` & `decoutilities-0.3.1/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: decoutilities
-Version: 0.3.0
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
 
 A simple python package that allows using decorators for multiple things like easily setting up a singleton or a configuration file for your app.
 
 ## Installation
 
 You can install `decoutilities` using pip:
@@ -474,15 +461,15 @@
 
 The `Logger` class uses the `textUtils` class to format the messages. The format of the messages can be specified when creating a `Logger` instance with the `format` parameter. The `{event}` placeholder in the format string is replaced with the event type (e.g., "INFO", "WARNING"), and the `{message}` placeholder is replaced with the actual message.
 
 If a `log` parameter is provided when creating a `Logger` instance, the logged messages will also be written to the specified log file.
 
 ## Components
 
-Â´decoutilitiesÂ´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
+´decoutilities´ includes a basic component feature that replaces Python default inputs in certain situations. Altrough this feature was not tested on Linux and MacOS, I suppose it should work.
 
 ### Selector
 
 The `Selector` component allows to make selections of only ONE item, here is a piece of code.
 
 ```python
 from decoutilities.components import Selector
@@ -498,25 +485,89 @@
 ### Checkmarks
 
 Also, as the `Selector` feature, this one works the same way.
 
 ```python
 from decoutilities.components import Checkmark
 
-features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| ðŸŸ©", "| â¬›"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
+features = Checkmark("Which features would you like to install?", ["Dark Mode", "SSR Support"]) # TIP: Add ["| 🟩", "| ⬛"] as the third argument to customize the prefixes of the selected (0) and unselected (1) options.
 
 selected = features.display()
 
 print(selected)
 
 ```
 
+
 ### Input
 
-This feature is still under development.
+The `Input` class is a utility for creating interactive console inputs with validation rules. 
+
+#### Importing the Class
+
+```python
+from decoutilities.components import Input
+```
+
+#### Creating an Instance
+
+```python
+name = Input('Password', '', 'REQUIRED|PASSWORD', 'The text is hidden')
+```
+
+#### Displaying the Input
+
+```python
+name.display()
+```
+
+#### Validation Rules
+
+The `Input` class supports a variety of validation rules. These rules are passed as a string when creating an instance of the class. Multiple rules can be combined using the pipe character (`|`).
+
+Here are the available rules and their usage:
+
+- `REQUIRED`: The input must not be empty.
+- `PASSWORD`: The input will be hidden.
+- `EMAIL`: The input must be a valid email address.
+- `NUMBER`: The input must be a number.
+- `STRING`: The input must be a string.
+- `MIN:<number>`: The input must be at least `<number>` characters long.
+- `MAX:<number>`: The input must be at most `<number>` characters long.
+- `LENGTH:<number>`: The input must be exactly `<number>` characters long.
+- `REGEX:<pattern>`: The input must match the regex `<pattern>`.
+- `CONTAINS:<value>`: The input must contain `<value>`.
+- `NOT_CONTAINS:<value>`: The input must not contain `<value>`.
+- `IN:<value1,value2,...>`: The input must be one of the specified values.
+- `NOT_IN:<value1,value2,...>`: The input must not be one of the specified values.
+- `EQUALS:<value>`: The input must be equal to `<value>`.
+- `NOT_EQUALS:<value>`: The input must not be equal to `<value>`.
+- `HIGHER:<number>`: The input must be higher than `<number>`.
+- `LOWER:<number>`: The input must be lower than `<number>`.
+- `HIGHER_OR_EQUAL:<number>`: The input must be higher or equal to `<number>`.
+- `LOWER_OR_EQUAL:<number>`: The input must be lower or equal to `<number>`.
+- `FLOAT`: The input must be a float.
+- `BOOLEAN`: The input must be a boolean (`true` or `false`).
+- `JSON`: The input must be a valid JSON string.
+- `IP`: The input must be a valid IP address.
+- `URL`: The input must be a valid URL.
+- `DATE`: The input must be a valid date (`YYYY-MM-DD`).
+- `TIME`: The input must be a valid time (`HH:MM:SS`).
+- `DATETIME`: The input must be a valid datetime (`YYYY-MM-DD HH:MM:SS`).
+- `PHONE`: The input must be a valid phone number (10 digits).
+- `PASSWORD`: The input must be a valid password (Minimum eight characters, at least one uppercase letter, one lowercase letter, one number and one special character).
+
+#### Example
+
+```python
+email = Input('Email', '', 'REQUIRED|EMAIL', 'Enter your email')
+email.display()
+```
+
+This will create an input that requires a valid email address.
 
 ## Experimental Features
 
 All features marked as in `BETA` or being `EXPERIMENTAL` are untested, what means they were only tested below specific condititons and not with all case of uses.
 
 Please report any issues or contribute by making a PR (look for [CONTRIBUTING](CONTRIBUTING) section for details).
 
@@ -538,8 +589,8 @@
 - FEATURE: For new features, include a explanation mentioning why it should be inside `decoutilities`.
 - BUGFIX: For general bugfixes.
 - SECURITY: For fixes related with security issues.
 - QoL: For QoL improvements
 
 ## Author
 
-- [Hugo Torres](https://github.com/Reddishye)
+- [Hugo Torres](https://github.com/Reddishye)
```

### Comparing `decoutilities-0.3.0/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.3.1/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.3.0/setup.py` & `decoutilities-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.3.0',
+version='0.3.1',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

