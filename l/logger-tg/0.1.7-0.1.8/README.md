# Comparing `tmp/logger-tg-0.1.7.tar.gz` & `tmp/logger-tg-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logger-tg-0.1.7.tar", last modified: Thu Apr  4 16:35:25 2024, max compression
+gzip compressed data, was "logger-tg-0.1.8.tar", last modified: Wed May 22 12:40:34 2024, max compression
```

## Comparing `logger-tg-0.1.7.tar` & `logger-tg-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 16:35:25.173758 logger-tg-0.1.7/
--rw-rw-rw-   0        0        0     1095 2024-02-25 01:30:39.000000 logger-tg-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     6065 2024-04-04 16:35:25.171704 logger-tg-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     4896 2024-04-04 15:15:06.000000 logger-tg-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 16:35:25.157979 logger-tg-0.1.7/logger_tg.egg-info/
--rw-rw-rw-   0        0        0     6065 2024-04-04 16:35:25.000000 logger-tg-0.1.7/logger_tg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      395 2024-04-04 16:35:25.000000 logger-tg-0.1.7/logger_tg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 16:35:25.000000 logger-tg-0.1.7/logger_tg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 16:35:25.000000 logger-tg-0.1.7/logger_tg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-04 16:35:25.000000 logger-tg-0.1.7/logger_tg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-04 16:35:25.174183 logger-tg-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     3729 2024-02-25 02:12:45.000000 logger-tg-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:35:25.165259 logger-tg-0.1.7/tg_logger/
--rw-rw-rw-   0        0        0       78 2024-04-04 15:15:40.000000 logger-tg-0.1.7/tg_logger/__init__.py
--rw-rw-rw-   0        0        0       66 2024-04-04 16:35:20.000000 logger-tg-0.1.7/tg_logger/__version__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 16:35:25.170560 logger-tg-0.1.7/tg_logger/logger/
--rw-rw-rw-   0        0        0        0 2024-02-24 23:38:14.000000 logger-tg-0.1.7/tg_logger/logger/__init__.py
--rw-rw-rw-   0        0        0     3583 2024-02-25 17:28:02.000000 logger-tg-0.1.7/tg_logger/logger/logger_warner.py
--rw-rw-rw-   0        0        0     8080 2024-04-04 15:09:02.000000 logger-tg-0.1.7/tg_logger/logger/loggers.py
--rw-rw-rw-   0        0        0     1405 2024-04-04 16:35:20.000000 logger-tg-0.1.7/tg_logger/logger/utils.py
--rw-rw-rw-   0        0        0     1186 2024-02-25 00:07:47.000000 logger-tg-0.1.7/tg_logger/settings.py
--rw-rw-rw-   0        0        0      131 2024-02-24 22:52:51.000000 logger-tg-0.1.7/tg_logger/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:40:34.903439 logger-tg-0.1.8/
+-rw-rw-rw-   0        0        0     1095 2024-02-25 01:30:39.000000 logger-tg-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     6065 2024-05-22 12:40:34.903439 logger-tg-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4896 2024-04-04 15:15:06.000000 logger-tg-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:40:34.887811 logger-tg-0.1.8/logger_tg.egg-info/
+-rw-rw-rw-   0        0        0     6065 2024-05-22 12:40:34.000000 logger-tg-0.1.8/logger_tg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2024-05-22 12:40:34.000000 logger-tg-0.1.8/logger_tg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:40:34.000000 logger-tg-0.1.8/logger_tg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 12:40:34.000000 logger-tg-0.1.8/logger_tg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 12:40:34.000000 logger-tg-0.1.8/logger_tg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:40:34.911447 logger-tg-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     3729 2024-02-25 02:12:45.000000 logger-tg-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:40:34.903439 logger-tg-0.1.8/tg_logger/
+-rw-rw-rw-   0        0        0       78 2024-04-04 15:15:40.000000 logger-tg-0.1.8/tg_logger/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-05-22 12:35:35.000000 logger-tg-0.1.8/tg_logger/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:40:34.903439 logger-tg-0.1.8/tg_logger/logger/
+-rw-rw-rw-   0        0        0        0 2024-02-24 23:38:14.000000 logger-tg-0.1.8/tg_logger/logger/__init__.py
+-rw-rw-rw-   0        0        0     3583 2024-02-25 17:28:02.000000 logger-tg-0.1.8/tg_logger/logger/logger_warner.py
+-rw-rw-rw-   0        0        0     8684 2024-05-22 12:35:35.000000 logger-tg-0.1.8/tg_logger/logger/loggers.py
+-rw-rw-rw-   0        0        0     1405 2024-04-04 16:35:20.000000 logger-tg-0.1.8/tg_logger/logger/utils.py
+-rw-rw-rw-   0        0        0     1186 2024-02-25 00:07:47.000000 logger-tg-0.1.8/tg_logger/settings.py
+-rw-rw-rw-   0        0        0      131 2024-02-24 22:52:51.000000 logger-tg-0.1.8/tg_logger/utils.py
```

### Comparing `logger-tg-0.1.7/LICENSE` & `logger-tg-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.7/PKG-INFO` & `logger-tg-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-tg
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asynchronous Telegram logging for Python applications
 Home-page: https://github.com/Nezhinskiy/logger-tg
 Author: Mikhail Nezhinsky
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Keywords: logger logging telegram async asyncio telegram_logger tg_logger python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `logger-tg-0.1.7/README.md` & `logger-tg-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.7/logger_tg.egg-info/PKG-INFO` & `logger-tg-0.1.8/logger_tg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logger-tg
-Version: 0.1.7
+Version: 0.1.8
 Summary: Asynchronous Telegram logging for Python applications
 Home-page: https://github.com/Nezhinskiy/logger-tg
 Author: Mikhail Nezhinsky
 Author-email: mikhail.nezhinsky@gmail.com
 License: MIT
 Keywords: logger logging telegram async asyncio telegram_logger tg_logger python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `logger-tg-0.1.7/setup.py` & `logger-tg-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.7/tg_logger/logger/logger_warner.py` & `logger-tg-0.1.8/tg_logger/logger/logger_warner.py`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.7/tg_logger/logger/loggers.py` & `logger-tg-0.1.8/tg_logger/logger/loggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,30 @@
                 'You must configure the logger using "configure_logger" or '
                 'provide "bot_token" and "recipient_id" during initialization.'
             ) from AttributeError
         else:
             settings = TgLoggerSettings(bot_token, recipient_id)
             return ClientLogger(settings, self.logger)
 
+    def log(self, level: int, msg=shrug, *args, **kwargs):
+        """
+        Log 'msg % args' with the integer severity 'level'.
+
+        To pass exception information, use the keyword argument exc_info with
+        a true value, e.g.
+
+        logger.log(level, "We have a %s", "mysterious problem", exc_info=1)
+        """
+        if not isinstance(level, int):
+            raise TypeError("level must be an integer")
+
+        if self.logger.isEnabledFor(level):
+            level_name = logging.getLevelName(level).lower()
+            getattr(self, level_name)(msg, *args, **kwargs)
+
     def critical(self, message: str) -> None:
         """
         Logs a critical message and sends it to the configured Telegram chat.
 
         Parameters:
         - message (str): The critical message.
         """
```

### Comparing `logger-tg-0.1.7/tg_logger/logger/utils.py` & `logger-tg-0.1.8/tg_logger/logger/utils.py`

 * *Files identical despite different names*

### Comparing `logger-tg-0.1.7/tg_logger/settings.py` & `logger-tg-0.1.8/tg_logger/settings.py`

 * *Files identical despite different names*

