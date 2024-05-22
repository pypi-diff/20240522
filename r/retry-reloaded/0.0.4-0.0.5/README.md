# Comparing `tmp/retry_reloaded-0.0.4.tar.gz` & `tmp/retry_reloaded-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry_reloaded-0.0.4.tar", last modified: Tue May  7 10:47:32 2024, max compression
+gzip compressed data, was "retry_reloaded-0.0.5.tar", last modified: Wed May 22 07:46:45 2024, max compression
```

## Comparing `retry_reloaded-0.0.4.tar` & `retry_reloaded-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.452273 retry_reloaded-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/retry_reloaded/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/retry_reloaded/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/retry_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-07 10:47:32.000000 retry_reloaded-0.0.4/retry_reloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 10:47:32.452273 retry_reloaded-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 10:47:32.448273 retry_reloaded-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-07 10:47:27.000000 retry_reloaded-0.0.4/tests/test_retry_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:46:45.394004 retry_reloaded-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-22 07:46:45.390004 retry_reloaded-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:46:45.390004 retry_reloaded-0.0.5/retry_reloaded/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/retry_reloaded/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:46:45.390004 retry_reloaded-0.0.5/retry_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-22 07:46:45.000000 retry_reloaded-0.0.5/retry_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-22 07:46:45.000000 retry_reloaded-0.0.5/retry_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:46:45.000000 retry_reloaded-0.0.5/retry_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 07:46:45.000000 retry_reloaded-0.0.5/retry_reloaded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:46:45.394004 retry_reloaded-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:46:45.390004 retry_reloaded-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 07:46:39.000000 retry_reloaded-0.0.5/tests/test_retry_args.py
```

### Comparing `retry_reloaded-0.0.4/LICENSE` & `retry_reloaded-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/PKG-INFO` & `retry_reloaded-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `retry_reloaded-0.0.4/README.md` & `retry_reloaded-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/retry_reloaded/__init__.py` & `retry_reloaded-0.0.5/retry_reloaded/__init__.py`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/retry_reloaded/_exceptions.py` & `retry_reloaded-0.0.5/retry_reloaded/_exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
-from typing import Callable
-
+from typing import Callable, Optional
 
 MAX_RETRIES_MESSAGE_TEMPLATE = (
     "Have reached max number of retries ({max_retries}) for function {fname}, aborting."
 )
 TIMEOUT_MESSAGE_TEMPLATE = (
     "Have been retrying function {fname} for {elapsed_time} secs. Exceeded timeout of {timeout} secs, aborting."
 )
@@ -16,93 +15,97 @@
 class BaseRetryException(Exception):
     """
     Base class for retry-related exceptions.
 
     Args:
         logger (logging.Logger): Logger object to use for logging the exception message.
         message (str): Message describing the exception.
-        failure_callback (Callable): Callback function to execute upon raising the exception.
+        failure_callback (Optional[Callable]): Callback function to execute upon raising the exception.
     """
+
     def __init__(
         self,
         logger: logging.Logger,
         message: str,
-        failure_callback: Callable
-    ):
+        failure_callback: Optional[Callable] = None
+    ) -> None:
         super().__init__(message)
         if logger:
             logger.error(message)
         if failure_callback:
             failure_callback()
 
 
 class MaxRetriesException(BaseRetryException):
     """
-    Exception raised when maximum number of retries is reached.
+    Exception raised when the maximum number of retries is reached.
 
     Args:
         logger (logging.Logger): Logger object to use for logging the exception message.
         fname (str): Name of the function for which maximum retries were reached.
-        failure_callback (Callable): Callback function to execute upon raising the exception.
+        failure_callback (Optional[Callable]): Callback function to execute upon raising the exception.
         max_retries (int): Maximum number of retries that have been attempted.
     """
+
     def __init__(
         self,
         logger: logging.Logger,
         fname: str,
-        failure_callback: Callable,
         max_retries: int,
-    ):
+        failure_callback: Optional[Callable] = None
+    ) -> None:
         message = MAX_RETRIES_MESSAGE_TEMPLATE.format(
             fname=fname, max_retries=max_retries
         )
         super().__init__(logger, message, failure_callback)
 
 
 class RetriesTimeoutException(BaseRetryException):
     """
-    Exception raised when retry operation exceeds timeout.
+    Exception raised when retry operation exceeds the timeout.
 
     Args:
         logger (logging.Logger): Logger object to use for logging the exception message.
         fname (str): Name of the function for which retry operation exceeded timeout.
-        failure_callback (Callable): Callback function to execute upon raising the exception.
-        elapsed_time (float): Time elapsed during retry operation in seconds.
+        failure_callback (Optional[Callable]): Callback function to execute upon raising the exception.
+        elapsed_time (float): Time elapsed during the retry operation in seconds.
         timeout (float): Timeout value in seconds.
     """
+
     def __init__(
         self,
         logger: logging.Logger,
         fname: str,
-        failure_callback: Callable,
         elapsed_time: float,
         timeout: float,
-    ):
+        failure_callback: Optional[Callable] = None
+    ) -> None:
         message = TIMEOUT_MESSAGE_TEMPLATE.format(
             fname=fname, elapsed_time=elapsed_time, timeout=timeout
         )
         super().__init__(logger, message, failure_callback)
 
 
 class RetriesDeadlineException(BaseRetryException):
     """
-    Exception raised when retry operation exceeds deadline.
+    Exception raised when retry operation exceeds the deadline.
 
     Args:
         logger (logging.Logger): Logger object to use for logging the exception message.
         fname (str): Name of the function for which retry operation exceeded deadline.
-        failure_callback (Callable): Callback function to execute upon raising the exception.
-        elapsed_time (float): Time elapsed during retry operation in seconds.
+        failure_callback (Optional[Callable]): Callback function to execute upon raising the exception.
+        elapsed_time (float): Time elapsed during the retry operation in seconds.
         deadline (float): Deadline value in seconds.
     """
+
     def __init__(
         self,
         logger: logging.Logger,
         fname: str,
-        failure_callback: Callable,
         elapsed_time: float,
-        deadline: float
-    ):
+        deadline: float,
+        failure_callback: Optional[Callable] = None,
+    ) -> None:
         message = DEADLINE_MESSAGE_TEMPLATE.format(
             fname=fname, elapsed_time=elapsed_time, deadline=deadline
         )
         super().__init__(logger, message, failure_callback)
```

### Comparing `retry_reloaded-0.0.4/retry_reloaded/_logging.py` & `retry_reloaded-0.0.5/retry_reloaded/_logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-from typing import Union, Optional
+from typing import Optional
 from time import time
 import logging
 
 
-def _init_logger(name):
+def _init_logger(name: str) -> logging.Logger:
     """
     Initialize logger for retry function.
 
+    Args:
+        name (str): Name for the logger.
+
     Returns:
         logging.Logger: Logger object configured for retry logging.
     """
     _retry_logger = logging.getLogger(name)
     _retry_logger.setLevel(logging.DEBUG)
     console_handler = logging.StreamHandler()
     console_handler.setLevel(logging.DEBUG)
@@ -20,52 +23,50 @@
     console_handler.setFormatter(formatter)
     _retry_logger.addHandler(console_handler)
     _retry_logger.propagate = False
     return _retry_logger
 
 
 def _log_retry(
-    logger: logging.Logger,
+    logger: Optional[logging.Logger],
     fname: str,
-    max_retries: Union[int, None],
+    max_retries: Optional[int],
     retries: int,
-    timeout: float,
-    deadline: float,
+    timeout: Optional[float],
+    deadline: Optional[float],
     start_time: float,
     delay: float,
-    exc_info: Optional[Exception]
-):
+    exc_info: Optional[Exception] = None
+) -> None:
     """
     Log retry information.
 
     Args:
-        logger (logging.Logger): Logger object to use for logging.
+        logger (Optional[logging.Logger]): Logger object to use for logging. If None, logging is skipped.
         fname (str): Name of the function being retried.
-        max_retries (Union[int, None]): Maximum number of retries allowed, or None if unlimited.
+        max_retries (Optional[int]): Maximum number of retries allowed, or None if unlimited.
         retries (int): Number of retries attempted so far.
-        timeout (float): Timeout value for the retry operation.
-        deadline (float): Deadline for the retry operation.
+        timeout (Optional[float]): Timeout value for the retry operation in seconds.
+        deadline (Optional[float]): Deadline for the retry operation in seconds.
         start_time (float): Start time of the retry operation.
-        delay (float): Delay until the next retry.
+        delay (float): Delay until the next retry in seconds.
         exc_info (Optional[Exception]): Information about the exception that triggered the retry.
 
     Returns:
         None
     """
     if not logger:
         return
 
     base_message = "Will retry function {fname}."
     remaining_retries_message = "Remaining retries: {remaining_retries}."
     remaining_time_message = "Remaining time: {remaining_time} secs."
     next_delay_message = "Next retry in {delay} secs."
 
-    messages = []
-
-    messages.append(base_message.format(fname=fname))
+    messages = [base_message.format(fname=fname)]
 
     if max_retries is not None:
         messages.append(
             remaining_retries_message.format(remaining_retries=max_retries - retries)
         )
 
     if timeout or deadline:
```

### Comparing `retry_reloaded-0.0.4/retry_reloaded/callback.py` & `retry_reloaded-0.0.5/retry_reloaded/callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import wraps
 from typing import Callable
 import inspect
 
 
-class CallbackFactory:
+class CallbackFactory():
     def __init__(self, func: Callable, *args, **kwargs):
         """
         Initialize the CallbackFactory.
 
         Parameters:
             func (Callable): The callable function to be wrapped.
             *args: Positional arguments to be passed to the function.
@@ -20,15 +20,20 @@
             raise TypeError("The 'func' argument must be callable")
 
         self.func = func
         self.kwargs = kwargs
 
         if len(args) > 0:
             func_args = inspect.getfullargspec(func).args
-            self.kwargs.update({func_args[i]: a for i, a in enumerate(args)})
+            self.kwargs.update(
+                {
+                    func_args[i]: a
+                    for i, a in enumerate(args)
+                }
+            )
 
     def __call__(self, **override_kwargs):
         """
         Call the wrapped function with provided keyword arguments.
         If no arguments are provided during calling,
         then the stored ones (during instance creation) are used.
 
@@ -56,15 +61,19 @@
         TypeError: If `func` is not a callable object.
     """
     if not callable(func):
         raise TypeError("The 'func' argument must be callable")
 
     if len(args) > 0:
         func_args = inspect.getfullargspec(func).args
-        kwargs.update({func_args[i]: a for i, a in enumerate(args)})
+        kwargs.update(
+            {
+                func_args[i]: a
+                for i, a in enumerate(args)
+            }
+        )
 
     @wraps(func)
     def wrapped_func(**override_kwargs):
         runtime_kwargs = {**kwargs, **override_kwargs}
         return func(**runtime_kwargs)
-
     return wrapped_func
```

### Comparing `retry_reloaded-0.0.4/retry_reloaded/retry.py` & `retry_reloaded-0.0.5/retry_reloaded/retry.py`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/retry_reloaded.egg-info/PKG-INFO` & `retry_reloaded-0.0.5/retry_reloaded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.4
+Version: 0.0.5
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `retry_reloaded-0.0.4/setup.py` & `retry_reloaded-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="retry-reloaded",
-    version="0.0.4",
+    version="0.0.5",
     description="A simple Python library for retrying functions \
         with various backoff and callback strategies.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/chrisK824/retry",
     author="Chris Karvouniaris",
     author_email="christos.karvouniaris247@gmail.com",
```

### Comparing `retry_reloaded-0.0.4/tests/test_callback.py` & `retry_reloaded-0.0.5/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/tests/test_retry.py` & `retry_reloaded-0.0.5/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `retry_reloaded-0.0.4/tests/test_retry_args.py` & `retry_reloaded-0.0.5/tests/test_retry_args.py`

 * *Files identical despite different names*

