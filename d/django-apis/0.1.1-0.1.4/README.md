# Comparing `tmp/django-apis-0.1.1.tar.gz` & `tmp/django-apis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-apis-0.1.1.tar", last modified: Wed May 15 15:36:23 2024, max compression
+gzip compressed data, was "django-apis-0.1.4.tar", last modified: Wed May 22 12:30:42 2024, max compression
```

## Comparing `django-apis-0.1.1.tar` & `django-apis-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.907294 django-apis-0.1.1/
--rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-14 02:29:47.000000 django-apis-0.1.1/LICENSE
--rw-r--r--   0 test       (501) staff       (20)      235 2024-05-14 02:42:56.000000 django-apis-0.1.1/MANIFEST.in
--rw-r--r--   0 test       (501) staff       (20)     2158 2024-05-15 15:36:23.907171 django-apis-0.1.1/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)     1586 2024-05-15 15:30:32.000000 django-apis-0.1.1/README.md
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.904388 django-apis-0.1.1/django_apis/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 00:56:35.000000 django-apis-0.1.1/django_apis/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-14 00:56:35.000000 django-apis-0.1.1/django_apis/admin.py
--rw-r--r--   0 test       (501) staff       (20)      153 2024-05-14 00:56:35.000000 django-apis-0.1.1/django_apis/apps.py
--rw-r--r--   0 test       (501) staff       (20)     1177 2024-05-14 09:30:29.000000 django-apis-0.1.1/django_apis/exceptions.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.905279 django-apis-0.1.1/django_apis/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 00:56:35.000000 django-apis-0.1.1/django_apis/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2024-05-14 00:56:35.000000 django-apis-0.1.1/django_apis/models.py
--rw-r--r--   0 test       (501) staff       (20)     2172 2024-05-14 09:31:09.000000 django-apis-0.1.1/django_apis/response.py
--rw-r--r--   0 test       (501) staff       (20)      639 2024-05-15 15:30:29.000000 django-apis-0.1.1/django_apis/settings.py
--rw-r--r--   0 test       (501) staff       (20)      580 2024-05-14 08:00:52.000000 django-apis-0.1.1/django_apis/tests.py
--rw-r--r--   0 test       (501) staff       (20)      734 2024-05-15 15:19:33.000000 django-apis-0.1.1/django_apis/utils.py
--rw-r--r--   0 test       (501) staff       (20)     5288 2024-05-15 15:33:45.000000 django-apis-0.1.1/django_apis/views.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.905168 django-apis-0.1.1/django_apis.egg-info/
--rw-r--r--   0 test       (501) staff       (20)     2158 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/PKG-INFO
--rw-r--r--   0 test       (501) staff       (20)      754 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/SOURCES.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/dependency_links.txt
--rw-r--r--   0 test       (501) staff       (20)        1 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/not-zip-safe
--rw-r--r--   0 test       (501) staff       (20)       16 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/requires.txt
--rw-r--r--   0 test       (501) staff       (20)       30 2024-05-15 15:36:23.000000 django-apis-0.1.1/django_apis.egg-info/top_level.txt
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.906772 django-apis-0.1.1/django_apis_debug/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 02:40:17.000000 django-apis-0.1.1/django_apis_debug/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       63 2024-05-14 02:40:17.000000 django-apis-0.1.1/django_apis_debug/admin.py
--rw-r--r--   0 test       (501) staff       (20)      164 2024-05-14 02:40:17.000000 django-apis-0.1.1/django_apis_debug/apps.py
-drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-15 15:36:23.907007 django-apis-0.1.1/django_apis_debug/migrations/
--rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 02:40:17.000000 django-apis-0.1.1/django_apis_debug/migrations/__init__.py
--rw-r--r--   0 test       (501) staff       (20)       57 2024-05-14 02:40:17.000000 django-apis-0.1.1/django_apis_debug/models.py
--rw-r--r--   0 test       (501) staff       (20)     1740 2024-05-14 07:59:29.000000 django-apis-0.1.1/django_apis_debug/tests.py
--rw-r--r--   0 test       (501) staff       (20)      222 2024-05-14 02:43:36.000000 django-apis-0.1.1/django_apis_debug/urls.py
--rw-r--r--   0 test       (501) staff       (20)      804 2024-05-14 08:14:55.000000 django-apis-0.1.1/django_apis_debug/views.py
--rw-r--r--   0 test       (501) staff       (20)       16 2024-05-14 07:46:12.000000 django-apis-0.1.1/requirements.txt
--rw-r--r--   0 test       (501) staff       (20)       38 2024-05-15 15:36:23.907340 django-apis-0.1.1/setup.cfg
--rw-r--r--   0 test       (501) staff       (20)     1357 2024-05-15 15:26:06.000000 django-apis-0.1.1/setup.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.338970 django-apis-0.1.4/
+-rw-r--r--   0 test       (501) staff       (20)     1036 2024-05-14 02:29:47.000000 django-apis-0.1.4/LICENSE
+-rw-r--r--   0 test       (501) staff       (20)      235 2024-05-14 02:42:56.000000 django-apis-0.1.4/MANIFEST.in
+-rw-r--r--   0 test       (501) staff       (20)     2321 2024-05-22 12:30:42.338843 django-apis-0.1.4/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)     1749 2024-05-21 07:30:26.000000 django-apis-0.1.4/README.md
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.335898 django-apis-0.1.4/django_apis/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 00:56:35.000000 django-apis-0.1.4/django_apis/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-14 00:56:35.000000 django-apis-0.1.4/django_apis/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      153 2024-05-14 00:56:35.000000 django-apis-0.1.4/django_apis/apps.py
+-rw-r--r--   0 test       (501) staff       (20)     1305 2024-05-21 06:33:36.000000 django-apis-0.1.4/django_apis/exceptions.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.336844 django-apis-0.1.4/django_apis/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 00:56:35.000000 django-apis-0.1.4/django_apis/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2024-05-14 00:56:35.000000 django-apis-0.1.4/django_apis/models.py
+-rw-r--r--   0 test       (501) staff       (20)     2172 2024-05-14 09:31:09.000000 django-apis-0.1.4/django_apis/response.py
+-rw-r--r--   0 test       (501) staff       (20)      639 2024-05-15 15:30:29.000000 django-apis-0.1.4/django_apis/settings.py
+-rw-r--r--   0 test       (501) staff       (20)      580 2024-05-14 08:00:52.000000 django-apis-0.1.4/django_apis/tests.py
+-rw-r--r--   0 test       (501) staff       (20)     1285 2024-05-21 07:29:13.000000 django-apis-0.1.4/django_apis/utils.py
+-rw-r--r--   0 test       (501) staff       (20)     5784 2024-05-22 12:08:48.000000 django-apis-0.1.4/django_apis/views.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.336720 django-apis-0.1.4/django_apis.egg-info/
+-rw-r--r--   0 test       (501) staff       (20)     2321 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/PKG-INFO
+-rw-r--r--   0 test       (501) staff       (20)      781 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 test       (501) staff       (20)        1 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/not-zip-safe
+-rw-r--r--   0 test       (501) staff       (20)       16 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/requires.txt
+-rw-r--r--   0 test       (501) staff       (20)       30 2024-05-22 12:30:42.000000 django-apis-0.1.4/django_apis.egg-info/top_level.txt
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.338467 django-apis-0.1.4/django_apis_debug/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 02:40:17.000000 django-apis-0.1.4/django_apis_debug/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       63 2024-05-14 02:40:17.000000 django-apis-0.1.4/django_apis_debug/admin.py
+-rw-r--r--   0 test       (501) staff       (20)      164 2024-05-14 02:40:17.000000 django-apis-0.1.4/django_apis_debug/apps.py
+-rw-r--r--   0 test       (501) staff       (20)      147 2024-05-21 06:40:15.000000 django-apis-0.1.4/django_apis_debug/forms.py
+drwxr-xr-x   0 test       (501) staff       (20)        0 2024-05-22 12:30:42.338684 django-apis-0.1.4/django_apis_debug/migrations/
+-rw-r--r--   0 test       (501) staff       (20)        0 2024-05-14 02:40:17.000000 django-apis-0.1.4/django_apis_debug/migrations/__init__.py
+-rw-r--r--   0 test       (501) staff       (20)       57 2024-05-14 02:40:17.000000 django-apis-0.1.4/django_apis_debug/models.py
+-rw-r--r--   0 test       (501) staff       (20)     1740 2024-05-14 07:59:29.000000 django-apis-0.1.4/django_apis_debug/tests.py
+-rw-r--r--   0 test       (501) staff       (20)      222 2024-05-14 02:43:36.000000 django-apis-0.1.4/django_apis_debug/urls.py
+-rw-r--r--   0 test       (501) staff       (20)      683 2024-05-21 06:42:47.000000 django-apis-0.1.4/django_apis_debug/views.py
+-rw-r--r--   0 test       (501) staff       (20)       16 2024-05-14 07:46:12.000000 django-apis-0.1.4/requirements.txt
+-rw-r--r--   0 test       (501) staff       (20)       38 2024-05-22 12:30:42.339011 django-apis-0.1.4/setup.cfg
+-rw-r--r--   0 test       (501) staff       (20)     1357 2024-05-21 07:30:28.000000 django-apis-0.1.4/setup.py
```

### Comparing `django-apis-0.1.1/LICENSE` & `django-apis-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-apis-0.1.1/PKG-INFO` & `django-apis-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apis
-Version: 0.1.1
+Version: 0.1.4
 Summary: Django简易json api接口封装。
 Author: Xie DongCong
 Maintainer: Xie DongCong
 License: MIT
 Keywords: django apis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,47 +27,55 @@
 ```
 
 ## 使用
 
 ### 简单的接口开发
 
 - 所有视图参数按django标准，添加request或其它路径参数。
-- 可以定义Form来完成请求参数的校验。在检验不通过的情况下，抛出`django_apis.exceptions.ValidationError`。`django_apis.exceptions.ValidationError`会把django的异常信息转化为文本格式。
-- `apiview`中`methods`参数表示允许的HTTP请求类型。可以是字符串，也可以是字符串数组。
+- 可以定义Form来完成请求参数的校验。
+    - 在检验不通过的情况下，抛出`django_apis.exceptions.InputValidationError`。
+    - `django_apis.exceptions.InputValidationError`会把django的异常信息转化为文本格式。
+- `apiview`中`methods`参数表示允许的HTTP请求类型。
+    - 可以是字符串，如：`"get"`。
+    - 也可以是字符串数组，如：`["get", "post"]`。
+    - 大小写均可。
 
+
+*forms.py*
 ```
 from django.forms import Form
 from django.forms.fields import CharField
 
 
+class EchoInput(Form):
+    msg = CharField(max_length=16, required=True)
+```
+
+*views.py*
+```
 from django_apis.views import get_apiview
 from django_apis.views import get_json_payload
-from django_apis.exceptions import ValidationError
-
+from django_apis.exceptions import InputValidationError
+from .forms import EchoInput
 
 apiview = get_apiview()
 
 
 @apiview(methods="GET")
 def ping(request):
     return "pong"
 
 
-class EchoInput(Form):
-    msg = CharField(max_length=16, required=True)
-
-
 @apiview(methods="POST")
 def echo(request):
     payload = get_json_payload(request)
     form = EchoInput(payload)
-    if form.is_valid():
-        return form.cleaned_data["msg"]
-    else:
-        raise ValidationError(form)
+    if not form.is_valid():
+        raise InputValidationError(form)
+    return form.cleaned_data["msg"]
 
 
 @apiview(methods="GET")
 def getRequestInfo(request):
     result = {}
     for key, value in request.META.items():
         if isinstance(value, str):
@@ -81,11 +89,11 @@
 - DJANGO_APIS_ALLOWED_METHODS
 - DJANGO_APIS_APIVIEW
 - DJANGO_APIS_ENABLE_REQUEST_LOG
 - DJANGO_APIS_REQUEST_LOG_NAME
 
 ## 版本记录
 
-### v0.1.1
+### v0.1.4
 
 - 版本首发。
```

### Comparing `django-apis-0.1.1/README.md` & `django-apis-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,47 +10,55 @@
 ```
 
 ## 使用
 
 ### 简单的接口开发
 
 - 所有视图参数按django标准，添加request或其它路径参数。
-- 可以定义Form来完成请求参数的校验。在检验不通过的情况下，抛出`django_apis.exceptions.ValidationError`。`django_apis.exceptions.ValidationError`会把django的异常信息转化为文本格式。
-- `apiview`中`methods`参数表示允许的HTTP请求类型。可以是字符串，也可以是字符串数组。
+- 可以定义Form来完成请求参数的校验。
+    - 在检验不通过的情况下，抛出`django_apis.exceptions.InputValidationError`。
+    - `django_apis.exceptions.InputValidationError`会把django的异常信息转化为文本格式。
+- `apiview`中`methods`参数表示允许的HTTP请求类型。
+    - 可以是字符串，如：`"get"`。
+    - 也可以是字符串数组，如：`["get", "post"]`。
+    - 大小写均可。
 
+
+*forms.py*
 ```
 from django.forms import Form
 from django.forms.fields import CharField
 
 
+class EchoInput(Form):
+    msg = CharField(max_length=16, required=True)
+```
+
+*views.py*
+```
 from django_apis.views import get_apiview
 from django_apis.views import get_json_payload
-from django_apis.exceptions import ValidationError
-
+from django_apis.exceptions import InputValidationError
+from .forms import EchoInput
 
 apiview = get_apiview()
 
 
 @apiview(methods="GET")
 def ping(request):
     return "pong"
 
 
-class EchoInput(Form):
-    msg = CharField(max_length=16, required=True)
-
-
 @apiview(methods="POST")
 def echo(request):
     payload = get_json_payload(request)
     form = EchoInput(payload)
-    if form.is_valid():
-        return form.cleaned_data["msg"]
-    else:
-        raise ValidationError(form)
+    if not form.is_valid():
+        raise InputValidationError(form)
+    return form.cleaned_data["msg"]
 
 
 @apiview(methods="GET")
 def getRequestInfo(request):
     result = {}
     for key, value in request.META.items():
         if isinstance(value, str):
@@ -64,11 +72,11 @@
 - DJANGO_APIS_ALLOWED_METHODS
 - DJANGO_APIS_APIVIEW
 - DJANGO_APIS_ENABLE_REQUEST_LOG
 - DJANGO_APIS_REQUEST_LOG_NAME
 
 ## 版本记录
 
-### v0.1.1
+### v0.1.4
 
 - 版本首发。
```

### Comparing `django-apis-0.1.1/django_apis/exceptions.py` & `django-apis-0.1.4/django_apis/exceptions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,16 @@
-class ValidationError(RuntimeError):
+class UnknownError(RuntimeError):
+    args = (-1, "系统开小差了，请联系管理员或稍候再试 ^_^")
+
+
+class BusinessError(RuntimeError):
+    args = (2, "业务逻辑错误")
+
+
+class InputValidationError(BusinessError):
     """请求参数验证失败。"""
 
     def __init__(self, form):
         self.form = form
 
     def json(self):
         messages = []
@@ -16,22 +24,21 @@
                 for message in error.messages:
                     message = str(message)
                     if message not in infos:
                         infos.append(message)
             message = "".join(infos)
             messages.append(f"{field_name}: {message}")
         return {
-            "code": 11,
+            "code": 201,
             "message": "\n".join(messages),
         }
 
 
-class JsonPayloadDecodeError(RuntimeError):
-    args = (12, "请求体不是有效的json格式，无法正常解析。")
+ValidationError = InputValidationError
 
 
-class RequestMethodNotAllowed(RuntimeError):
-    args = (13, "不允许的HTTP请求类型。")
+class JsonPayloadDecodeError(BusinessError):
+    args = (202, "请求体不是有效的json格式，无法正常解析。")
 
 
-class SystemError(RuntimeError):
-    args = (2, "系统开小差了，请联系管理员或稍候再试 ^_^")
+class RequestMethodNotAllowed(BusinessError):
+    args = (203, "不允许的HTTP请求类型。")
```

### Comparing `django-apis-0.1.1/django_apis/response.py` & `django-apis-0.1.4/django_apis/response.py`

 * *Files identical despite different names*

### Comparing `django-apis-0.1.1/django_apis/settings.py` & `django-apis-0.1.4/django_apis/settings.py`

 * *Files identical despite different names*

### Comparing `django-apis-0.1.1/django_apis/tests.py` & `django-apis-0.1.4/django_apis/tests.py`

 * *Files identical despite different names*

### Comparing `django-apis-0.1.1/django_apis/views.py` & `django-apis-0.1.4/django_apis/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import json
 import inspect
 import logging
 import functools
 from zenutils import importutils
 from django.conf import settings
-from django.http import HttpResponse
-from django.http import JsonResponse
+from django.http.response import HttpResponseBase
+from django.http.response import JsonResponse
 from django.urls import reverse
 from django.utils import timezone
 from django.views.decorators.csrf import csrf_exempt
 from .exceptions import JsonPayloadDecodeError
 from .exceptions import RequestMethodNotAllowed
+from .exceptions import BusinessError
+from .exceptions import UnknownError
 from .settings import DJANGO_APIS_ALLOWED_METHODS
 from .settings import DJANGO_APIS_APIVIEW
 from .settings import DJANGO_APIS_ENABLE_REQUEST_LOG
 from .settings import DJANGO_APIS_REQUEST_LOG_NAME
 from .response import SimpleJsonResponsePackage
 from .utils import get_time_string
 from .utils import get_request_headers
 from .utils import get_request_log_text
+from .utils import get_response_log_data
+
+_logger = logging.getLogger(__name__)
 
 
 class Apiview(object):
     def __init__(
         self,
         default_methods=None,
         response_package_class=None,
@@ -62,15 +67,15 @@
     def get_request_log(self, request, response_data):
         """Access日志内容。"""
         return {
             "time": get_time_string(),
             "method": request.method,
             "path": request.path,
             "params": dict(request.GET),
-            "body": get_request_log_text(request.body),
+            "body": get_request_log_text(request),
             "response": response_data,
             "headers": get_request_headers(request),
         }
 
     def write_request_log(self, request, response_data):
         """记录Access日志。"""
         if self.enable_request_log:
@@ -93,23 +98,28 @@
                     # 检查请求类型
                     if request.method not in methods:
                         raise RequestMethodNotAllowed()
                     # 执行实际的视图
                     result = real_view_func(request, *args, **kwargs)
                     error = None
                     success = True
-                except Exception as err:
+                except BusinessError as err:  # 只有BusinessError才允许回显给用户
                     result = None
                     error = err
                     success = False
-                if isinstance(result, HttpResponse):
+                except Exception as err:  # 未知错误不允许回显给用户
+                    _logger.exception("apiview got unknown error: error=%s", err)
+                    result = None
+                    error = UnknownError()
+                    success = False
+                if isinstance(result, HttpResponseBase):
                     # 已经是完整的响应体
                     response = result
                     # @todo: 需要进一步检查是否安全
-                    response_data = get_request_log_text(response.content)
+                    response_data = get_response_log_data(response)
                 else:
                     # 结果封装和返回
                     response_data = self.response_package_class(
                         result, error, success
                     ).pack()
                     response = JsonResponse(
                         response_data,
```

### Comparing `django-apis-0.1.1/django_apis.egg-info/PKG-INFO` & `django-apis-0.1.4/django_apis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-apis
-Version: 0.1.1
+Version: 0.1.4
 Summary: Django简易json api接口封装。
 Author: Xie DongCong
 Maintainer: Xie DongCong
 License: MIT
 Keywords: django apis
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -27,47 +27,55 @@
 ```
 
 ## 使用
 
 ### 简单的接口开发
 
 - 所有视图参数按django标准，添加request或其它路径参数。
-- 可以定义Form来完成请求参数的校验。在检验不通过的情况下，抛出`django_apis.exceptions.ValidationError`。`django_apis.exceptions.ValidationError`会把django的异常信息转化为文本格式。
-- `apiview`中`methods`参数表示允许的HTTP请求类型。可以是字符串，也可以是字符串数组。
+- 可以定义Form来完成请求参数的校验。
+    - 在检验不通过的情况下，抛出`django_apis.exceptions.InputValidationError`。
+    - `django_apis.exceptions.InputValidationError`会把django的异常信息转化为文本格式。
+- `apiview`中`methods`参数表示允许的HTTP请求类型。
+    - 可以是字符串，如：`"get"`。
+    - 也可以是字符串数组，如：`["get", "post"]`。
+    - 大小写均可。
 
+
+*forms.py*
 ```
 from django.forms import Form
 from django.forms.fields import CharField
 
 
+class EchoInput(Form):
+    msg = CharField(max_length=16, required=True)
+```
+
+*views.py*
+```
 from django_apis.views import get_apiview
 from django_apis.views import get_json_payload
-from django_apis.exceptions import ValidationError
-
+from django_apis.exceptions import InputValidationError
+from .forms import EchoInput
 
 apiview = get_apiview()
 
 
 @apiview(methods="GET")
 def ping(request):
     return "pong"
 
 
-class EchoInput(Form):
-    msg = CharField(max_length=16, required=True)
-
-
 @apiview(methods="POST")
 def echo(request):
     payload = get_json_payload(request)
     form = EchoInput(payload)
-    if form.is_valid():
-        return form.cleaned_data["msg"]
-    else:
-        raise ValidationError(form)
+    if not form.is_valid():
+        raise InputValidationError(form)
+    return form.cleaned_data["msg"]
 
 
 @apiview(methods="GET")
 def getRequestInfo(request):
     result = {}
     for key, value in request.META.items():
         if isinstance(value, str):
@@ -81,11 +89,11 @@
 - DJANGO_APIS_ALLOWED_METHODS
 - DJANGO_APIS_APIVIEW
 - DJANGO_APIS_ENABLE_REQUEST_LOG
 - DJANGO_APIS_REQUEST_LOG_NAME
 
 ## 版本记录
 
-### v0.1.1
+### v0.1.4
 
 - 版本首发。
```

### Comparing `django-apis-0.1.1/django_apis.egg-info/SOURCES.txt` & `django-apis-0.1.4/django_apis.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -19,12 +19,13 @@
 django_apis.egg-info/not-zip-safe
 django_apis.egg-info/requires.txt
 django_apis.egg-info/top_level.txt
 django_apis/migrations/__init__.py
 django_apis_debug/__init__.py
 django_apis_debug/admin.py
 django_apis_debug/apps.py
+django_apis_debug/forms.py
 django_apis_debug/models.py
 django_apis_debug/tests.py
 django_apis_debug/urls.py
 django_apis_debug/views.py
 django_apis_debug/migrations/__init__.py
```

### Comparing `django-apis-0.1.1/django_apis_debug/tests.py` & `django-apis-0.1.4/django_apis_debug/tests.py`

 * *Files identical despite different names*

### Comparing `django-apis-0.1.1/django_apis_debug/views.py` & `django-apis-0.1.4/django_apis_debug/views.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,27 @@
-from django.forms import Form
-from django.forms.fields import CharField
-
-
 from django_apis.views import get_apiview
 from django_apis.views import get_json_payload
-from django_apis.exceptions import ValidationError
-
+from django_apis.exceptions import InputValidationError
+from .forms import EchoInput
 
 apiview = get_apiview()
 
 
 @apiview(methods="GET")
 def ping(request):
     return "pong"
 
 
-class EchoInput(Form):
-    msg = CharField(max_length=16, required=True)
-
-
 @apiview(methods="POST")
 def echo(request):
     payload = get_json_payload(request)
     form = EchoInput(payload)
-    if form.is_valid():
-        return form.cleaned_data["msg"]
-    else:
-        raise ValidationError(form)
+    if not form.is_valid():
+        raise InputValidationError(form)
+    return form.cleaned_data["msg"]
 
 
 @apiview(methods="GET")
 def getRequestInfo(request):
     result = {}
     for key, value in request.META.items():
         if isinstance(value, str):
```

### Comparing `django-apis-0.1.1/setup.py` & `django-apis-0.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     long_description = fobj.read()
 
 with open(os.path.join(here, "requirements.txt"), "r", encoding="utf-8") as fobj:
     requires = [x.strip() for x in fobj.readlines() if x.strip()]
 
 setup(
     name="django-apis",
-    version="0.1.1",
+    version="0.1.4",
     description="Django简易json api接口封装。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Xie DongCong",
     maintainer="Xie DongCong",
     license="MIT",
     classifiers=[
```

