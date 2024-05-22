# Comparing `tmp/django_ses-4.0.0.tar.gz` & `tmp/django_ses-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-4.0.0.tar", max compression
+gzip compressed data, was "django_ses-4.1.0.tar", max compression
```

## Comparing `django_ses-4.0.0.tar` & `django_ses-4.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2024-04-19 16:37:59.173368 django_ses-4.0.0/LICENSE
--rw-r--r--   0        0        0    23987 2024-04-19 16:37:59.173368 django_ses-4.0.0/README.rst
--rw-r--r--   0        0        0    14050 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/admin.py
--rw-r--r--   0        0        0      181 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/apps.py
--rw-r--r--   0        0        0       65 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/models.py
--rw-r--r--   0        0        0     2677 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/settings.py
--rw-r--r--   0        0        0      290 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      156 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/urls.py
--rw-r--r--   0        0        0     9957 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/utils.py
--rw-r--r--   0        0        0    20556 2024-04-19 16:37:59.173368 django_ses-4.0.0/django_ses/views.py
--rw-r--r--   0        0        0        0 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/__init__.py
--rw-r--r--   0        0        0      103 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/middleware.py
--rw-r--r--   0        0        0     2173 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/settings.py
--rw-r--r--   0        0        0      295 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/base.html
--rw-r--r--   0        0        0      220 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/index.html
--rw-r--r--   0        0        0      756 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/templates/send-email.html
--rw-r--r--   0        0        0      772 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/urls.py
--rw-r--r--   0        0        0      885 2024-04-19 16:37:59.173368 django_ses-4.0.0/example/views.py
--rw-r--r--   0        0        0     2540 2024-04-19 16:37:59.177368 django_ses-4.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/__init__.py
--rw-r--r--   0        0        0    16378 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_commands.py
--rw-r--r--   0        0        0     2636 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_stats.py
--rw-r--r--   0        0        0      345 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_urls.py
--rw-r--r--   0        0        0    13660 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_verifier.py
--rw-r--r--   0        0        0    13740 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/test_views.py
--rw-r--r--   0        0        0      115 2024-04-19 16:37:59.177368 django_ses-4.0.0/tests/utils.py
--rw-r--r--   0        0        0    25733 1970-01-01 00:00:00.000000 django_ses-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-05-22 16:35:41.568851 django_ses-4.1.0/LICENSE
+-rw-r--r--   0        0        0    24114 2024-05-22 16:35:41.568851 django_ses-4.1.0/README.rst
+-rw-r--r--   0        0        0    14352 2024-05-22 16:35:41.568851 django_ses-4.1.0/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/models.py
+-rw-r--r--   0        0        0     2768 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      156 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/urls.py
+-rw-r--r--   0        0        0     9957 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/utils.py
+-rw-r--r--   0        0        0    20556 2024-05-22 16:35:41.572851 django_ses-4.1.0/django_ses/views.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/__init__.py
+-rw-r--r--   0        0        0      103 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/middleware.py
+-rw-r--r--   0        0        0     2173 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/settings.py
+-rw-r--r--   0        0        0      295 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/templates/base.html
+-rw-r--r--   0        0        0      220 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/templates/index.html
+-rw-r--r--   0        0        0      756 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/templates/send-email.html
+-rw-r--r--   0        0        0      772 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/urls.py
+-rw-r--r--   0        0        0      885 2024-05-22 16:35:41.572851 django_ses-4.1.0/example/views.py
+-rw-r--r--   0        0        0     2540 2024-05-22 16:35:41.572851 django_ses-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/__init__.py
+-rw-r--r--   0        0        0    16448 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_commands.py
+-rw-r--r--   0        0        0     2636 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_stats.py
+-rw-r--r--   0        0        0      345 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_urls.py
+-rw-r--r--   0        0        0    13660 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_verifier.py
+-rw-r--r--   0        0        0    13740 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/test_views.py
+-rw-r--r--   0        0        0      115 2024-05-22 16:35:41.572851 django_ses-4.1.0/tests/utils.py
+-rw-r--r--   0        0        0    25860 1970-01-01 00:00:00.000000 django_ses-4.1.0/PKG-INFO
```

### Comparing `django_ses-4.0.0/LICENSE` & `django_ses-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/README.rst` & `django_ses-4.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,19 @@
 
     pip install django-ses[events]
 
 Add the following to your settings.py::
 
     EMAIL_BACKEND = 'django_ses.SESBackend'
 
-    # These are optional -- if they're set as environment variables they won't
-    # need to be set here as well
+    # These are optional if you are using AWS IAM Roles https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html
     AWS_ACCESS_KEY_ID = 'YOUR-ACCESS-KEY-ID'
     AWS_SECRET_ACCESS_KEY = 'YOUR-SECRET-ACCESS-KEY'
-
+    # https://docs.aws.amazon.com/cli/v1/userguide/cli-configure-files.html
+    AWS_SESSION_PROFILE = 'YOUR-PROFILE-NAME'
     # Additionally, if you are not using the default AWS region of us-east-1,
     # you need to specify a region, like so:
     AWS_SES_REGION_NAME = 'us-west-2'
     AWS_SES_REGION_ENDPOINT = 'email.us-west-2.amazonaws.com'
 
     # If you want to use the SESv2 client
     USE_SES_V2 = True
```

### Comparing `django_ses-4.0.0/django_ses/__init__.py` & `django_ses-4.1.0/django_ses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,25 @@
     return float(val)
 
 
 class SESBackend(BaseEmailBackend):
     """A Django Email backend that uses Amazon's Simple Email Service.
     """
 
-    def __init__(self, fail_silently=False, aws_access_key=None,
+    def __init__(self, fail_silently=False,aws_session_profile=None, aws_access_key=None,
                  aws_secret_key=None, aws_session_token=None, aws_region_name=None,
                  aws_region_endpoint=None, aws_auto_throttle=None, aws_config=None,
                  dkim_domain=None, dkim_key=None, dkim_selector=None, dkim_headers=None,
                  ses_source_arn=None, ses_from_arn=None, ses_return_path_arn=None,
                  use_ses_v2=False,
-                 **kwargs):
+        **kwargs
+    ):
 
         super(SESBackend, self).__init__(fail_silently=fail_silently, **kwargs)
+        self._session_profile = aws_session_profile or settings.AWS_SESSION_PROFILE
         self._access_key_id = aws_access_key or settings.ACCESS_KEY
         self._access_key = aws_secret_key or settings.SECRET_KEY
         self._session_token = aws_session_token or settings.SESSION_TOKEN
         self._region_name = aws_region_name if aws_region_name else settings.AWS_SES_REGION_NAME
         self._endpoint_url = aws_region_endpoint if aws_region_endpoint else settings.AWS_SES_REGION_ENDPOINT_URL
         self._throttle = cast_nonzero_to_float(aws_auto_throttle or settings.AWS_SES_AUTO_THROTTLE)
         self._config = aws_config or settings.AWS_SES_CONFIG
@@ -82,30 +84,37 @@
         self.ses_from_arn = ses_from_arn or settings.AWS_SES_FROM_ARN
         self.ses_return_path_arn = ses_return_path_arn or settings.AWS_SES_RETURN_PATH_ARN
 
         self._use_ses_v2 = use_ses_v2 or settings.USE_SES_V2
 
         self.connection = None
 
+    def create_session(self) -> boto3.Session:
+        if self._session_profile:
+            return boto3.Session(profile_name=self._session_profile)
+
+        return boto3.Session(
+            aws_access_key_id=self._access_key_id,
+            aws_secret_access_key=self._access_key,
+            aws_session_token=self._session_token,
+        )
+
     def open(self):
         """Create a connection to the AWS API server. This can be reused for
         sending multiple emails.
         """
         if self.connection:
             return False
 
         try:
-            self.connection = boto3.client(
-                'sesv2' if self._use_ses_v2 else 'ses',
-                aws_access_key_id=self._access_key_id,
-                aws_secret_access_key=self._access_key,
-                aws_session_token=self._session_token,
+            self.connection = self.create_session().client(
+                "sesv2" if self._use_ses_v2 else "ses",
                 region_name=self._region_name,
                 endpoint_url=self._endpoint_url,
-                config=self._config
+                config=self._config,
             )
 
         except Exception:
             if not self.fail_silently:
                 raise
 
     def close(self):
```

### Comparing `django_ses-4.0.0/django_ses/management/commands/get_ses_statistics.py` & `django_ses-4.1.0/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/django_ses/management/commands/ses_email_address.py` & `django_ses-4.1.0/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/django_ses/migrations/0001_initial.py` & `django_ses-4.1.0/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/django_ses/settings.py` & `django_ses-4.1.0/django_ses/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from django.conf import settings
 
-__all__ = ('ACCESS_KEY', 'SECRET_KEY', 'AWS_SES_REGION_NAME',
+__all__ = ('AWS_SESSION_PROFILE','ACCESS_KEY', 'SECRET_KEY', 'AWS_SES_REGION_NAME',
            'AWS_SES_REGION_ENDPOINT', 'AWS_SES_AUTO_THROTTLE',
            'AWS_SES_CONFIG',  'AWS_SES_RETURN_PATH',
            'DKIM_DOMAIN', 'DKIM_PRIVATE_KEY',
            'DKIM_SELECTOR', 'DKIM_HEADERS', 'TIME_ZONE')
 
+AWS_SESSION_PROFILE = getattr(settings, "AWS_SESSION_PROFILE", None)
 ACCESS_KEY = getattr(settings, 'AWS_SES_ACCESS_KEY_ID',
                      getattr(settings, 'AWS_ACCESS_KEY_ID', None))
 
 SECRET_KEY = getattr(settings, 'AWS_SES_SECRET_ACCESS_KEY',
                      getattr(settings, 'AWS_SECRET_ACCESS_KEY', None))
 
 SESSION_TOKEN = getattr(settings, 'AWS_SES_SESSION_TOKEN',
```

### Comparing `django_ses-4.0.0/django_ses/templates/django_ses/send_stats.html` & `django_ses-4.1.0/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/django_ses/utils.py` & `django_ses-4.1.0/django_ses/utils.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/django_ses/views.py` & `django_ses-4.1.0/django_ses/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/example/settings.py` & `django_ses-4.1.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/example/templates/send-email.html` & `django_ses-4.1.0/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/example/urls.py` & `django_ses-4.1.0/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/example/views.py` & `django_ses-4.1.0/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/pyproject.toml` & `django_ses-4.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ses"
-version = "4.0.0"
+version = "4.1.0"
 description = "A Django email backend for Amazon's Simple Email Service (SES)"
 authors = [
     "Harry Marr <harry@hmarr.com>",
     "Wes Winham <winhamwr@gmail.com>",
     "Ross Lawley <ross.lawley@gmail.com>",
     "Paul Craciunoiu <paul@craciunoiu.net>",
 ]
```

### Comparing `django_ses-4.0.0/tests/test_backend.py` & `django_ses-4.1.0/tests/test_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,30 +74,36 @@
         return {
             'MessageId': 'fake_message_id',
             'ResponseMetadata': {
                 'RequestId': 'fake_request_id',
                 },
             }
 
+    @classmethod
+    def client(cls, *args, **kwargs):
+        return cls(args, kwargs)
+
 
 class FakeSESBackend(django_ses.SESBackend):
     """
     A fake SES backend for testing purposes. It overrides the real SESBackend's
     get_rate_limit method so we can run tests without valid AWS credentials.
     """
 
     def get_rate_limit(self):
         return 10
 
+    def create_session(self) -> FakeSESConnection:
+        return FakeSESConnection
+
 
 class SESBackendTest(TestCase):
     def setUp(self):
         # TODO: Fix this -- this is going to cause side effects
-        django_settings.EMAIL_BACKEND = 'tests.test_backend.FakeSESBackend'
-        django_ses.boto3.client = FakeSESConnection
+        django_settings.EMAIL_BACKEND = "tests.test_backend.FakeSESBackend"
         self.outbox = FakeSESConnection.outbox
 
     def tearDown(self):
         # Empty outbox every time test finishes
         FakeSESConnection.outbox = []
 
     def _rfc2047_helper(self, value_to_encode):
@@ -173,15 +179,14 @@
 
 class SESV2BackendTest(TestCase):
     def setUp(self):
         django_settings.EMAIL_BACKEND = 'tests.test_backend.FakeSESBackend'
         settings.USE_SES_V2 = True
         settings.AWS_SES_FROM_ARN = None
         settings.AWS_SES_SOURCE_ARN = None
-        django_ses.boto3.client = FakeSESConnection
         self.outbox = FakeSESConnection.outbox
 
     def tearDown(self):
         # Empty outbox every time test finishes
         settings.USE_SES_V2 = False
         FakeSESConnection.outbox = []
```

### Comparing `django_ses-4.0.0/tests/test_commands.py` & `django_ses-4.1.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/tests/test_settings.py` & `django_ses-4.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/tests/test_stats.py` & `django_ses-4.1.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/tests/test_verifier.py` & `django_ses-4.1.0/tests/test_verifier.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/tests/test_views.py` & `django_ses-4.1.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ses-4.0.0/PKG-INFO` & `django_ses-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ses
-Version: 4.0.0
+Version: 4.1.0
 Summary: A Django email backend for Amazon's Simple Email Service (SES)
 Home-page: https://github.com/django-ses/django-ses
 License: MIT
 Author: Harry Marr
 Author-email: harry@hmarr.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -104,19 +104,19 @@
 
     pip install django-ses[events]
 
 Add the following to your settings.py::
 
     EMAIL_BACKEND = 'django_ses.SESBackend'
 
-    # These are optional -- if they're set as environment variables they won't
-    # need to be set here as well
+    # These are optional if you are using AWS IAM Roles https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html
     AWS_ACCESS_KEY_ID = 'YOUR-ACCESS-KEY-ID'
     AWS_SECRET_ACCESS_KEY = 'YOUR-SECRET-ACCESS-KEY'
-
+    # https://docs.aws.amazon.com/cli/v1/userguide/cli-configure-files.html
+    AWS_SESSION_PROFILE = 'YOUR-PROFILE-NAME'
     # Additionally, if you are not using the default AWS region of us-east-1,
     # you need to specify a region, like so:
     AWS_SES_REGION_NAME = 'us-west-2'
     AWS_SES_REGION_ENDPOINT = 'email.us-west-2.amazonaws.com'
 
     # If you want to use the SESv2 client
     USE_SES_V2 = True
```

