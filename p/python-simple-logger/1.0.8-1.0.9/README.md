# Comparing `tmp/python_simple_logger-1.0.8.tar.gz` & `tmp/python_simple_logger-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_simple_logger-1.0.8.tar", max compression
+gzip compressed data, was "python_simple_logger-1.0.9.tar", max compression
```

## Comparing `python_simple_logger-1.0.8.tar` & `python_simple_logger-1.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-10-11 10:21:56.986623 python_simple_logger-1.0.8/LICENSE
--rw-r--r--   0        0        0      713 2023-10-11 10:21:56.986623 python_simple_logger-1.0.8/README.md
--rw-r--r--   0        0        0     1413 2023-10-11 10:22:01.015571 python_simple_logger-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-11 10:21:56.986623 python_simple_logger-1.0.8/simple_logger/__init__.py
--rw-r--r--   0        0        0     3008 2023-10-11 10:21:56.986623 python_simple_logger-1.0.8/simple_logger/logger.py
--rw-r--r--   0        0        0        0 2023-10-11 10:21:56.987623 python_simple_logger-1.0.8/simple_logger/tests/__init__.py
--rw-r--r--   0        0        0      539 2023-10-11 10:21:56.987623 python_simple_logger-1.0.8/simple_logger/tests/test_logger.py
--rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 python_simple_logger-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-28 08:42:18.372920 python_simple_logger-1.0.9/LICENSE
+-rw-r--r--   0        0        0      713 2024-01-28 08:42:18.372920 python_simple_logger-1.0.9/README.md
+-rw-r--r--   0        0        0     1363 2024-01-28 08:42:23.354871 python_simple_logger-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-28 08:42:18.375920 python_simple_logger-1.0.9/simple_logger/__init__.py
+-rw-r--r--   0        0        0     2986 2024-01-28 08:42:18.375920 python_simple_logger-1.0.9/simple_logger/logger.py
+-rw-r--r--   0        0        0        0 2024-01-28 08:42:18.375920 python_simple_logger-1.0.9/simple_logger/tests/__init__.py
+-rw-r--r--   0        0        0      539 2024-01-28 08:42:18.375920 python_simple_logger-1.0.9/simple_logger/tests/test_logger.py
+-rw-r--r--   0        0        0     1716 1970-01-01 00:00:00.000000 python_simple_logger-1.0.9/PKG-INFO
```

### Comparing `python_simple_logger-1.0.8/LICENSE` & `python_simple_logger-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.8/README.md` & `python_simple_logger-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.8/simple_logger/logger.py` & `python_simple_logger-1.0.9/simple_logger/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,17 +81,15 @@
 
         logger_obj.addHandler(hdlr=console_handler)
 
     logger_obj.setLevel(level=level)
     logger_obj.addFilter(filter=DuplicateFilter())
 
     if filename:
-        log_handler = RotatingFileHandler(
-            filename=filename, maxBytes=file_max_bytes, backupCount=file_backup_count
-        )
+        log_handler = RotatingFileHandler(filename=filename, maxBytes=file_max_bytes, backupCount=file_backup_count)
         log_handler.setFormatter(fmt=log_formatter)
         log_handler.setLevel(level=level)
         logger_obj.addHandler(hdlr=log_handler)
 
     logger_obj.propagate = False
     LOGGERS[name] = logger_obj
     return logger_obj
```

### Comparing `python_simple_logger-1.0.8/simple_logger/tests/test_logger.py` & `python_simple_logger-1.0.9/simple_logger/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `python_simple_logger-1.0.8/PKG-INFO` & `python_simple_logger-1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: python-simple-logger
-Version: 1.0.8
+Version: 1.0.9
 Summary: A simple logger for python
 Home-page: https://github.com/RedHatQE/python-simple-logger
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Project-URL: Bug Tracker, https://github.com/RedHatQE/python-simple-logger/issues
 Project-URL: Documentation, https://github.com/RedHatQE/python-simple-logger/blob/main/README.md
 Project-URL: Download, https://pypi.org/project/python-simple-logger/
 Description-Content-Type: text/markdown
 
 # Simple Python logger
```

