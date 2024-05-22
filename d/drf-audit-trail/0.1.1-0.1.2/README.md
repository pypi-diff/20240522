# Comparing `tmp/drf_audit_trail-0.1.1.tar.gz` & `tmp/drf_audit_trail-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_audit_trail-0.1.1.tar", max compression
+gzip compressed data, was "drf_audit_trail-0.1.2.tar", max compression
```

## Comparing `drf_audit_trail-0.1.1.tar` & `drf_audit_trail-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0       19 2024-05-09 11:24:11.563624 drf_audit_trail-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-09 19:43:15.712433 drf_audit_trail-0.1.1/drf_audit_trail/admin.py
--rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.1/drf_audit_trail/apps.py
--rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.1/drf_audit_trail/integrations/__init__.py
--rw-r--r--   0        0        0      958 2024-05-09 18:44:07.433037 drf_audit_trail-0.1.1/drf_audit_trail/integrations/rest_framework_simplejwt.py
--rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.1/drf_audit_trail/managers/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.1/drf_audit_trail/managers/request_audit_event_manager.py
--rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.1/drf_audit_trail/middleware/__init__.py
--rw-r--r--   0        0        0     5256 2024-05-18 14:23:17.654457 drf_audit_trail-0.1.1/drf_audit_trail/middleware/request_login_audit_event.py
--rw-r--r--   0        0        0     5948 2024-05-09 19:40:49.994054 drf_audit_trail-0.1.1/drf_audit_trail/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/migrations/__init__.py
--rw-r--r--   0        0        0      647 2024-05-09 19:26:04.213917 drf_audit_trail-0.1.1/drf_audit_trail/mixins.py
--rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.1/drf_audit_trail/models/__init__.py
--rw-r--r--   0        0        0      826 2024-05-09 19:29:58.942644 drf_audit_trail-0.1.1/drf_audit_trail/models/login_audit_event.py
--rw-r--r--   0        0        0     1737 2024-05-09 19:29:55.270574 drf_audit_trail-0.1.1/drf_audit_trail/models/request_audit_event.py
--rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.1/drf_audit_trail/settings.py
--rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.1/drf_audit_trail/tests.py
--rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.1/drf_audit_trail/utils.py
--rw-r--r--   0        0        0      516 2024-05-18 14:24:33.979652 drf_audit_trail-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      806 2024-05-22 13:29:24.303659 drf_audit_trail-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.2/drf_audit_trail/__init__.py
+-rw-r--r--   0        0        0     1169 2024-05-21 21:34:03.481866 drf_audit_trail-0.1.2/drf_audit_trail/admin.py
+-rw-r--r--   0        0        0      255 2024-05-10 20:28:23.293537 drf_audit_trail-0.1.2/drf_audit_trail/apps.py
+-rw-r--r--   0        0        0        0 2024-05-08 23:42:25.366271 drf_audit_trail-0.1.2/drf_audit_trail/integrations/__init__.py
+-rw-r--r--   0        0        0     1038 2024-05-21 23:07:13.612121 drf_audit_trail-0.1.2/drf_audit_trail/integrations/rest_framework_simplejwt.py
+-rw-r--r--   0        0        0      106 2024-05-09 18:15:40.126054 drf_audit_trail-0.1.2/drf_audit_trail/managers/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-09 18:19:21.825227 drf_audit_trail-0.1.2/drf_audit_trail/managers/request_audit_event_manager.py
+-rw-r--r--   0        0        0      120 2024-05-09 01:34:50.633399 drf_audit_trail-0.1.2/drf_audit_trail/middleware/__init__.py
+-rw-r--r--   0        0        0     5589 2024-05-21 23:03:26.544696 drf_audit_trail-0.1.2/drf_audit_trail/middleware/request_login_audit_event.py
+-rw-r--r--   0        0        0     5511 2024-05-21 21:41:30.726036 drf_audit_trail-0.1.2/drf_audit_trail/migrations/0001_initial.py
+-rw-r--r--   0        0        0      547 2024-05-22 01:12:33.248504 drf_audit_trail-0.1.2/drf_audit_trail/migrations/0002_alter_loginauditevent_request.py
+-rw-r--r--   0        0        0        0 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.2/drf_audit_trail/migrations/__init__.py
+-rw-r--r--   0        0        0      433 2024-05-21 21:33:32.240334 drf_audit_trail-0.1.2/drf_audit_trail/mixins.py
+-rw-r--r--   0        0        0      150 2024-05-09 17:52:36.716410 drf_audit_trail-0.1.2/drf_audit_trail/models/__init__.py
+-rw-r--r--   0        0        0      792 2024-05-22 01:12:11.888359 drf_audit_trail-0.1.2/drf_audit_trail/models/login_audit_event.py
+-rw-r--r--   0        0        0     1932 2024-05-21 22:15:20.337476 drf_audit_trail-0.1.2/drf_audit_trail/models/request_audit_event.py
+-rw-r--r--   0        0        0      700 2024-05-10 00:12:08.881038 drf_audit_trail-0.1.2/drf_audit_trail/settings.py
+-rw-r--r--   0        0        0       60 2024-05-08 01:49:41.058976 drf_audit_trail-0.1.2/drf_audit_trail/tests.py
+-rw-r--r--   0        0        0      709 2024-05-09 18:22:22.004405 drf_audit_trail-0.1.2/drf_audit_trail/utils.py
+-rw-r--r--   0        0        0      575 2024-05-22 13:29:42.303988 drf_audit_trail-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 drf_audit_trail-0.1.2/PKG-INFO
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/admin.py` & `drf_audit_trail-0.1.2/drf_audit_trail/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,13 @@
             return obj.request.ip_addresses
 
     @admin.display()
     def request__status_code(self, obj):
         if obj.request is not None:
             return obj.request.status_code
 
+    def user(self, obj):
+        if obj.request is not None:
+            return obj.request.user
+
 
 admin.site.register(LoginAuditEvent, LoginAuditEventModelAdmin)
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/integrations/rest_framework_simplejwt.py` & `drf_audit_trail-0.1.2/drf_audit_trail/integrations/rest_framework_simplejwt.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from drf_audit_trail.models import LoginAuditEvent
 
 
 class DRFAuditTrailIntegrationMixin:
     def post(self, request, *args: tuple, **kwargs: dict):
         serializer = self.get_serializer(data=request.data)
         drf_login_audit_event = request.META.get("drf_login_audit_event")
+        drf_request_audit_event = request.META.get("drf_request_audit_event")
 
         try:
             serializer.is_valid(raise_exception=True)
             drf_login_audit_event["status"] = LoginAuditEvent.SIGNIN
-            drf_login_audit_event["user"] = serializer.user
+            drf_request_audit_event["user"] = serializer.user
         except TokenError as e:
             raise InvalidToken(e.args[0])
 
         return Response(serializer.validated_data, status=HTTP_200_OK)
 
 
 class DRFAuditTrailTokenObtainPairView(
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/managers/request_audit_event_manager.py` & `drf_audit_trail-0.1.2/drf_audit_trail/managers/request_audit_event_manager.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/middleware/request_login_audit_event.py` & `drf_audit_trail-0.1.2/drf_audit_trail/middleware/request_login_audit_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     get_ip_addresses,
     get_response_size,
 )
 
 
 class RequestLoginAuditEventMiddleware(MiddlewareMixin):
     def __init__(self, get_response):
-        self.get_response = get_response
+        super().__init__(get_response)
 
         self.drf_request_audit_event = {}
         self.drf_login_audit_event = {}
         self._request_audit_event_enabled = False
 
         self._start_time = None
         self._url = None
@@ -40,46 +40,38 @@
 
         self._schema = request.scheme
         self._url = request.path
         self._method = request.method
         self._query_params = request.META.get("QUERY_STRING")
         self._ip_addresses = get_ip_addresses(request)
 
-        for i in DRF_AUDIT_TRAIL_REQUEST_AUDIT_URLS:
-            if bool(re.match(i, self._url)):
-                self._request_audit_event_enabled = True
-                break
+        if self.__is_auth_url(request):
+            self._request_audit_event_enabled = True
+        else:
+            for i in DRF_AUDIT_TRAIL_REQUEST_AUDIT_URLS:
+                if bool(re.match(i, self._url)):
+                    self._request_audit_event_enabled = True
+                    break
 
         self._start_time = time()
         request.META["drf_audit_event_start_time"] = self._start_time
 
         return self.get_response(request)
 
     def process_view(self, request: HttpRequest, view_func, view_args, view_kwargs):
         if self._request_audit_event_enabled:
             request.META["drf_request_audit_event"] = self.drf_request_audit_event
             request.META["drf_login_audit_event"] = self.drf_login_audit_event
 
-        return None
-
     def process_response(self, request, response):
-        request_audit_event_instance = None
-        authenticated_user = self.__get_authenticated_user(request)
-
         if self._request_audit_event_enabled:
-            request_extra_informations = self.drf_request_audit_event.get(
-                "extra_informations"
+            authenticated_user = self.__get_authenticated_user(request)
+            extra_informations = self._get_extra_informations(
+                self.drf_request_audit_event
             )
-            extra_informations = None
-
-            if request_extra_informations is not None:
-                try:
-                    extra_informations = json_dumps(request_extra_informations)
-                except Exception:
-                    pass
 
             with transaction.atomic():
                 request_audit_event_instance = RequestAuditEvent.objects.create(
                     url=self._url,
                     method=self._method,
                     query_params=self._query_params,
                     ip_addresses=self._ip_addresses,
@@ -92,52 +84,65 @@
                     error_message=self.drf_request_audit_event.get("error_message"),
                     error_stacktrace=self.drf_request_audit_event.get(
                         "error_stacktrace"
                     ),
                     extra_informations=extra_informations,
                 )
 
-        if self.__is_auth_url(request):
-            with transaction.atomic():
-                LoginAuditEvent.objects.create(
-                    user=authenticated_user,
-                    status=self._get_login_status(request, response),
-                    request=request_audit_event_instance,
-                )
+                if self.__is_auth_url(request):
+                    extra_informations = self._get_extra_informations(
+                        self.drf_login_audit_event
+                    )
+
+                    LoginAuditEvent.objects.create(
+                        extra_informations=extra_informations,
+                        status=self._get_login_status(request, response),
+                        request=request_audit_event_instance,
+                    )
 
         return response
 
     def process_exception(self, request, exception: BaseException):
         self.drf_request_audit_event["error_type"] = exception.__class__.__name__
         self.drf_request_audit_event["error_message"] = str(exception)
         self.drf_request_audit_event["error_stacktrace"] = traceback_format_exc()
 
         if self.__is_auth_url(request):
             self.drf_login_audit_event["status"] = LoginAuditEvent.FAILED
 
-        return None
+    def _get_extra_informations(self, instance_dict: dict):
+        request_extra_informations = instance_dict.get("extra_informations")
+        extra_informations = None
+
+        if request_extra_informations is not None:
+            try:
+                extra_informations = json_dumps(request_extra_informations)
+            except Exception:
+                pass
 
-    def __reset(self):
-        self.drf_request_audit_event = {}
-        self.drf_login_audit_event = {}
-        self._request_audit_event_enabled = False
+        return extra_informations
 
     def _get_login_status(self, request, response):
         if response.status_code == DRF_AUDIT_TRAIL_AUTH_STATUS_CODE_FALIED:
             return LoginAuditEvent.FAILED
 
         if self.drf_login_audit_event.get("status") is None:
             if request.user.is_authenticated:
                 return LoginAuditEvent.SIGNIN
             else:
                 return LoginAuditEvent.FAILED
 
         return self.drf_login_audit_event.get("status")
 
+    def __reset(self):
+        self.drf_request_audit_event = {}
+        self.drf_login_audit_event = {}
+        self._request_audit_event_enabled = False
+
     def __is_auth_url(self, request):
         return DRF_AUDIT_TRAIL_AUTH_URL == request.META.get("PATH_INFO")
 
     def __get_authenticated_user(self, request):
         if self.__is_auth_url(request):
-            return self.drf_login_audit_event.get("user")
+            return self.drf_request_audit_event.get("user")
 
         return get_authenticated_user_by_request(request)
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/migrations/0001_initial.py` & `drf_audit_trail-0.1.2/drf_audit_trail/migrations/0001_initial.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.2.13 on 2024-05-09 19:40
+# Generated by Django 4.2.13 on 2024-05-21 21:41
 
 from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
@@ -143,30 +143,18 @@
                         max_length=8,
                         verbose_name="Status",
                     ),
                 ),
                 (
                     "request",
                     models.ForeignKey(
-                        blank=True,
-                        null=True,
                         on_delete=django.db.models.deletion.CASCADE,
                         to="drf_audit_trail.requestauditevent",
                     ),
                 ),
-                (
-                    "user",
-                    models.ForeignKey(
-                        blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.SET_NULL,
-                        to=settings.AUTH_USER_MODEL,
-                        verbose_name="User",
-                    ),
-                ),
             ],
             options={
                 "verbose_name": "Login audit event",
                 "verbose_name_plural": "Login audit events",
                 "db_table": "login_audit_event",
             },
         ),
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/models/login_audit_event.py` & `drf_audit_trail-0.1.2/drf_audit_trail/models/login_audit_event.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,13 @@
     STATUS = (
         (SIGNIN, _("Sign in")),
         (SIGNOUT, _("Sign out")),
         (FAILED, _("Failed")),
     )
 
     status = models.CharField(_("Status"), choices=STATUS, max_length=8)
-    request = models.ForeignKey(
-        RequestAuditEvent, on_delete=models.CASCADE, blank=True, null=True
-    )
+    request = models.OneToOneField(RequestAuditEvent, on_delete=models.CASCADE)
 
     class Meta:
         verbose_name = _("Login audit event")
         verbose_name_plural = _("Login audit events")
         db_table = "login_audit_event"
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/models/request_audit_event.py` & `drf_audit_trail-0.1.2/drf_audit_trail/models/request_audit_event.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+from django.contrib.auth import get_user_model
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from drf_audit_trail.managers import RequestAuditEventManager
 from drf_audit_trail.mixins import BaseModelMixin
 
+User = get_user_model()
+
 
 class RequestAuditEvent(BaseModelMixin):
     """
     This is the model for the request audit trail.
     """
 
+    user = models.ForeignKey(
+        User, null=True, blank=True, on_delete=models.SET_NULL, verbose_name=_("User")
+    )
     ip_addresses = models.CharField(_("Ip addresses"), max_length=50, null=True)
 
     """
         methods: GET, POST, PUT, DELETE, PATCH, OPTIONS
     """
     method = models.CharField(_("Method"), max_length=10)
     url = models.CharField(_("URL"), null=False, max_length=2048)
```

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/settings.py` & `drf_audit_trail-0.1.2/drf_audit_trail/settings.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.1/drf_audit_trail/utils.py` & `drf_audit_trail-0.1.2/drf_audit_trail/utils.py`

 * *Files identical despite different names*

### Comparing `drf_audit_trail-0.1.1/pyproject.toml` & `drf_audit_trail-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "drf-audit-trail"
-version = "0.1.1"
+version = "0.1.2"
 description = "A reusable django [DRF] application that handles auditing of requests and logins"
 authors = ["Talismar Fernandes Costa <talismar788.una@gmail.com>"]
 readme = "README.md"
+repository = "https://github.com/Talismar/drf-audit-trail"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = "^4"
 djangorestframework-simplejwt = "5.2.2"
 djangorestframework = "3.14.0"
```

