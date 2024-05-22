# Comparing `tmp/intensity_logger-0.1.0.tar.gz` & `tmp/intensity_logger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intensity_logger-0.1.0.tar", last modified: Mon May 20 16:46:50 2024, max compression
+gzip compressed data, was "intensity_logger-0.1.1.tar", last modified: Wed May 22 07:31:55 2024, max compression
```

## Comparing `intensity_logger-0.1.0.tar` & `intensity_logger-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 16:46:50.575999 intensity_logger-0.1.0/
--rw-rw-rw-   0        0        0     1085 2024-05-20 15:21:41.000000 intensity_logger-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3245 2024-05-20 16:46:50.575003 intensity_logger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2334 2024-05-20 16:45:45.000000 intensity_logger-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 16:46:50.546856 intensity_logger-0.1.0/intensity-logger/
--rw-rw-rw-   0        0        0       26 2024-05-20 15:28:32.000000 intensity_logger-0.1.0/intensity-logger/__init__.py
--rw-rw-rw-   0        0        0     2418 2024-05-20 15:36:18.000000 intensity_logger-0.1.0/intensity-logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-20 16:46:50.573003 intensity_logger-0.1.0/intensity_logger.egg-info/
--rw-rw-rw-   0        0        0     3245 2024-05-20 16:46:50.000000 intensity_logger-0.1.0/intensity_logger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-05-20 16:46:50.000000 intensity_logger-0.1.0/intensity_logger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 16:46:50.000000 intensity_logger-0.1.0/intensity_logger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-20 16:46:50.000000 intensity_logger-0.1.0/intensity_logger.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-20 16:46:50.000000 intensity_logger-0.1.0/intensity_logger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 16:46:50.575999 intensity_logger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1169 2024-05-20 16:44:13.000000 intensity_logger-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.767248 intensity_logger-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-05-22 07:11:41.000000 intensity_logger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3761 2024-05-22 07:31:55.766162 intensity_logger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2785 2024-05-22 07:31:22.000000 intensity_logger-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.741059 intensity_logger-0.1.1/intensity_logger/
+-rw-rw-rw-   0        0        0       26 2024-05-22 07:17:22.000000 intensity_logger-0.1.1/intensity_logger/__init__.py
+-rw-rw-rw-   0        0        0     1523 2024-05-22 07:26:12.000000 intensity_logger-0.1.1/intensity_logger/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:31:55.764791 intensity_logger-0.1.1/intensity_logger.egg-info/
+-rw-rw-rw-   0        0        0     3761 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 07:29:53.000000 intensity_logger-0.1.1/intensity_logger.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-05-22 07:31:55.000000 intensity_logger-0.1.1/intensity_logger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:31:55.767248 intensity_logger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2024-05-22 07:30:34.000000 intensity_logger-0.1.1/setup.py
```

### Comparing `intensity_logger-0.1.0/LICENSE` & `intensity_logger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `intensity_logger-0.1.0/PKG-INFO` & `intensity_logger-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: intensity-logger
-Version: 0.1.0
-Summary: A colorful logging utility for Python applications
-Home-page: https://github.com/idkconsole/ColorLogger
-Author: console
+Version: 0.1.1
+Summary: A logging utility for Python applications with customizable intensity
+Home-page: https://github.com/idkconsole/intensity-logger
+Author: idkconsole, eagledev1337, homicide3301
 Author-email: idkconsole@proton.me
-Keywords: logging logger color logs
+Keywords: logging logger intensity color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,88 +17,95 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ColorLogger
+# Intensity Logger
 
-A simple and flexible logging module with color-coded output for enhanced readability.
+A simple and flexible logging module with customizable intensity and color-coded output for enhanced readability.
 
 ## Table of Contents
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Basic Usage](#basic-usage)
   - [Log Levels](#log-levels)
   - [Performance Timing](#performance-timing)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Introduction
-ColorLogger is a Python logging module designed to provide simple, color-coded logging output. It helps to easily distinguish different log levels, such as success, info, failure, and rate limit warnings.
+Intensity Logger is a Python logging module designed to provide simple, color-coded logging output with customizable intensity. It helps to easily distinguish different log levels, such as debug, info, warning, error, success, and ratelimit.
 
 ## Features
 - Color-coded log messages for easy readability.
-- Support for different log levels: success, info, failure, and ratelimit.
-- Optional performance timing display for operations.
+- Support for different log levels: debug, info, warning, error, success, and ratelimit.
+- Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
-You can install ColorLogger via pip:
+You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger
+pip install intensity-logger==0.1.1
 ```
 
 ## Usage
-Basic Usage
-Here's a basic example to get you started with ColorLogger:
+## Basic Usage
 
-```python
+Here's a basic example to get you started with Intensity Logger:
+
+```py
 from intensity_logger import Logger
 
 logger = Logger()
 
-logger.success("Operation completed successfully.")
-logger.info("This is an informational message.")
-logger.failure("An error occurred.")
-logger.ratelimit("Rate limit reached.")
+logger.debug("This is a debug message.")
+logger.info("This is an info message.")
+logger.warning("Warning issued.")
+logger.error("An error has occurred.")
+logger.success("Operation was successful.")
+logger.ratelimit("Rate limit exceeded.")
 ```
 
-# Log Levels
-ColorLogger supports various log levels, each with a different color:
+## Log Levels
+Intensity Logger supports various log levels, each with a different color:
 
--> Success: Indicates successful operations.
--> Info: Provides informational messages.
--> Failure: Logs errors and failures.
--> Ratelimit: Warnings about rate limiting.
+- Debug: Detailed information, typically of interest only when diagnosing problems.
+- Info: Confirmation that things are working as expected.
+- Warning: An indication that something unexpected happened, or indicative of some problem in the near future.
+- Error: Due to a more serious problem, the software has not been able to perform some function.
+- Success: Indicates successful operations.
+- Ratelimit: Warnings about rate limiting.
 
-# Performance Timing
+## Performance Timing
 You can log the duration of an operation by passing `start` and `end` times:
 
-```python
+```py
 import time
 from intensity_logger import Logger
 
 logger = Logger()
 
 start_time = time.time()
 time.sleep(2)
 end_time = time.time()
 
 logger.success("Operation completed successfully.", start=start_time, end=end_time)
 ```
 
-# Contributing
+## Contributing
+
 Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request on GitHub.
 
 1. Fork the repository.
 2. Create your feature branch.
 3. Commit your changes.
 4. Push to the branch.
 5. Open a pull request.
 
-# License
+## License
+
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `intensity_logger-0.1.0/README.md` & `intensity_logger-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,88 @@
-# ColorLogger
+# Intensity Logger
 
-A simple and flexible logging module with color-coded output for enhanced readability.
+A simple and flexible logging module with customizable intensity and color-coded output for enhanced readability.
 
 ## Table of Contents
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Basic Usage](#basic-usage)
   - [Log Levels](#log-levels)
   - [Performance Timing](#performance-timing)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Introduction
-ColorLogger is a Python logging module designed to provide simple, color-coded logging output. It helps to easily distinguish different log levels, such as success, info, failure, and rate limit warnings.
+Intensity Logger is a Python logging module designed to provide simple, color-coded logging output with customizable intensity. It helps to easily distinguish different log levels, such as debug, info, warning, error, success, and ratelimit.
 
 ## Features
 - Color-coded log messages for easy readability.
-- Support for different log levels: success, info, failure, and ratelimit.
-- Optional performance timing display for operations.
+- Support for different log levels: debug, info, warning, error, success, and ratelimit.
+- Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
-You can install ColorLogger via pip:
+You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger
+pip install intensity-logger==0.1.1
 ```
 
 ## Usage
-Basic Usage
-Here's a basic example to get you started with ColorLogger:
+## Basic Usage
 
-```python
+Here's a basic example to get you started with Intensity Logger:
+
+```py
 from intensity_logger import Logger
 
 logger = Logger()
 
-logger.success("Operation completed successfully.")
-logger.info("This is an informational message.")
-logger.failure("An error occurred.")
-logger.ratelimit("Rate limit reached.")
+logger.debug("This is a debug message.")
+logger.info("This is an info message.")
+logger.warning("Warning issued.")
+logger.error("An error has occurred.")
+logger.success("Operation was successful.")
+logger.ratelimit("Rate limit exceeded.")
 ```
 
-# Log Levels
-ColorLogger supports various log levels, each with a different color:
+## Log Levels
+Intensity Logger supports various log levels, each with a different color:
 
--> Success: Indicates successful operations.
--> Info: Provides informational messages.
--> Failure: Logs errors and failures.
--> Ratelimit: Warnings about rate limiting.
+- Debug: Detailed information, typically of interest only when diagnosing problems.
+- Info: Confirmation that things are working as expected.
+- Warning: An indication that something unexpected happened, or indicative of some problem in the near future.
+- Error: Due to a more serious problem, the software has not been able to perform some function.
+- Success: Indicates successful operations.
+- Ratelimit: Warnings about rate limiting.
 
-# Performance Timing
+## Performance Timing
 You can log the duration of an operation by passing `start` and `end` times:
 
-```python
+```py
 import time
 from intensity_logger import Logger
 
 logger = Logger()
 
 start_time = time.time()
 time.sleep(2)
 end_time = time.time()
 
 logger.success("Operation completed successfully.", start=start_time, end=end_time)
 ```
 
-# Contributing
+## Contributing
+
 Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request on GitHub.
 
 1. Fork the repository.
 2. Create your feature branch.
 3. Commit your changes.
 4. Push to the branch.
 5. Open a pull request.
 
-# License
+## License
+
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `intensity_logger-0.1.0/intensity_logger.egg-info/PKG-INFO` & `intensity_logger-0.1.1/intensity_logger.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: intensity-logger
-Version: 0.1.0
-Summary: A colorful logging utility for Python applications
-Home-page: https://github.com/idkconsole/ColorLogger
-Author: console
+Version: 0.1.1
+Summary: A logging utility for Python applications with customizable intensity
+Home-page: https://github.com/idkconsole/intensity-logger
+Author: idkconsole, eagledev1337, homicide3301
 Author-email: idkconsole@proton.me
-Keywords: logging logger color logs
+Keywords: logging logger intensity color logs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,88 +17,95 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# ColorLogger
+# Intensity Logger
 
-A simple and flexible logging module with color-coded output for enhanced readability.
+A simple and flexible logging module with customizable intensity and color-coded output for enhanced readability.
 
 ## Table of Contents
 - [Introduction](#introduction)
 - [Features](#features)
 - [Installation](#installation)
 - [Usage](#usage)
   - [Basic Usage](#basic-usage)
   - [Log Levels](#log-levels)
   - [Performance Timing](#performance-timing)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Introduction
-ColorLogger is a Python logging module designed to provide simple, color-coded logging output. It helps to easily distinguish different log levels, such as success, info, failure, and rate limit warnings.
+Intensity Logger is a Python logging module designed to provide simple, color-coded logging output with customizable intensity. It helps to easily distinguish different log levels, such as debug, info, warning, error, success, and ratelimit.
 
 ## Features
 - Color-coded log messages for easy readability.
-- Support for different log levels: success, info, failure, and ratelimit.
-- Optional performance timing display for operations.
+- Support for different log levels: debug, info, warning, error, success, and ratelimit.
+- Optional custom intensity to convert messages to uppercase.
 - Lightweight and easy to integrate into any Python project.
 
 ## Installation
-You can install ColorLogger via pip:
+You can install Intensity Logger via pip:
 
 ```bash
-pip install intensity-logger
+pip install intensity-logger==0.1.1
 ```
 
 ## Usage
-Basic Usage
-Here's a basic example to get you started with ColorLogger:
+## Basic Usage
 
-```python
+Here's a basic example to get you started with Intensity Logger:
+
+```py
 from intensity_logger import Logger
 
 logger = Logger()
 
-logger.success("Operation completed successfully.")
-logger.info("This is an informational message.")
-logger.failure("An error occurred.")
-logger.ratelimit("Rate limit reached.")
+logger.debug("This is a debug message.")
+logger.info("This is an info message.")
+logger.warning("Warning issued.")
+logger.error("An error has occurred.")
+logger.success("Operation was successful.")
+logger.ratelimit("Rate limit exceeded.")
 ```
 
-# Log Levels
-ColorLogger supports various log levels, each with a different color:
+## Log Levels
+Intensity Logger supports various log levels, each with a different color:
 
--> Success: Indicates successful operations.
--> Info: Provides informational messages.
--> Failure: Logs errors and failures.
--> Ratelimit: Warnings about rate limiting.
+- Debug: Detailed information, typically of interest only when diagnosing problems.
+- Info: Confirmation that things are working as expected.
+- Warning: An indication that something unexpected happened, or indicative of some problem in the near future.
+- Error: Due to a more serious problem, the software has not been able to perform some function.
+- Success: Indicates successful operations.
+- Ratelimit: Warnings about rate limiting.
 
-# Performance Timing
+## Performance Timing
 You can log the duration of an operation by passing `start` and `end` times:
 
-```python
+```py
 import time
 from intensity_logger import Logger
 
 logger = Logger()
 
 start_time = time.time()
 time.sleep(2)
 end_time = time.time()
 
 logger.success("Operation completed successfully.", start=start_time, end=end_time)
 ```
 
-# Contributing
+## Contributing
+
 Contributions are welcome! If you have ideas for improvements or new features, feel free to open an issue or submit a pull request on GitHub.
 
 1. Fork the repository.
 2. Create your feature branch.
 3. Commit your changes.
 4. Push to the branch.
 5. Open a pull request.
 
-# License
+## License
+
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `intensity_logger-0.1.0/setup.py` & `intensity_logger-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='intensity-logger',
-    version='0.1.0',
-    author='console',
+    version='0.1.1',
+    author='idkconsole, eagledev1337, homicide3301',
     author_email='idkconsole@proton.me',
-    description='A colorful logging utility for Python applications',
+    description='A logging utility for Python applications with customizable intensity',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/idkconsole/ColorLogger',
+    url='https://github.com/idkconsole/intensity-logger',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
@@ -21,12 +21,12 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     install_requires=[],
-    keywords='logging logger color logs',
+    keywords='logging logger intensity color logs',
     package_data={},
     include_package_data=True,
     zip_safe=False
 )
```

