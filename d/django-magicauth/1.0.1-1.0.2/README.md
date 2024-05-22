# Comparing `tmp/django-magicauth-1.0.1.tar.gz` & `tmp/django-magicauth-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magicauth-1.0.1.tar", last modified: Thu Feb  1 08:28:35 2024, max compression
+gzip compressed data, was "django-magicauth-1.0.2.tar", last modified: Wed May 22 12:29:59 2024, max compression
```

## Comparing `django-magicauth-1.0.1.tar` & `django-magicauth-1.0.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.409098 django-magicauth-1.0.1/
--rw-rw-r--   0 augier    (1000) augier    (1000)     1068 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/LICENSE
--rw-rw-r--   0 augier    (1000) augier    (1000)       74 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/MANIFEST.in
--rw-r--r--   0 augier    (1000) augier    (1000)     8053 2024-02-01 08:28:35.409098 django-magicauth-1.0.1/PKG-INFO
--rw-r--r--   0 augier    (1000) augier    (1000)     7396 2024-01-31 15:40:41.000000 django-magicauth-1.0.1/README.md
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.403098 django-magicauth-1.0.1/django_magicauth.egg-info/
--rw-r--r--   0 augier    (1000) augier    (1000)     8053 2024-02-01 08:28:35.000000 django-magicauth-1.0.1/django_magicauth.egg-info/PKG-INFO
--rw-r--r--   0 augier    (1000) augier    (1000)      956 2024-02-01 08:28:35.000000 django-magicauth-1.0.1/django_magicauth.egg-info/SOURCES.txt
--rw-r--r--   0 augier    (1000) augier    (1000)        1 2024-02-01 08:28:35.000000 django-magicauth-1.0.1/django_magicauth.egg-info/dependency_links.txt
--rw-r--r--   0 augier    (1000) augier    (1000)       16 2024-02-01 08:28:35.000000 django-magicauth-1.0.1/django_magicauth.egg-info/top_level.txt
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.405098 django-magicauth-1.0.1/magicauth/
--rw-r--r--   0 augier    (1000) augier    (1000)        0 2022-04-04 13:45:02.000000 django-magicauth-1.0.1/magicauth/__init__.py
--rw-rw-r--   0 augier    (1000) augier    (1000)      212 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/admin.py
--rw-rw-r--   0 augier    (1000) augier    (1000)      125 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/apps.py
--rw-r--r--   0 augier    (1000) augier    (1000)      704 2022-04-04 13:45:02.000000 django-magicauth-1.0.1/magicauth/forms.py
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.406098 django-magicauth-1.0.1/magicauth/migrations/
--rw-rw-r--   0 augier    (1000) augier    (1000)     1364 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/migrations/0001_initial.py
--rw-rw-r--   0 augier    (1000) augier    (1000)        0 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/migrations/__init__.py
--rw-r--r--   0 augier    (1000) augier    (1000)      668 2022-04-04 13:45:02.000000 django-magicauth-1.0.1/magicauth/models.py
--rw-rw-r--   0 augier    (1000) augier    (1000)     1691 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/next_url.py
--rw-r--r--   0 augier    (1000) augier    (1000)     1576 2023-03-06 11:17:46.000000 django-magicauth-1.0.1/magicauth/otp_forms.py
--rw-r--r--   0 augier    (1000) augier    (1000)     2772 2023-06-05 13:48:50.000000 django-magicauth-1.0.1/magicauth/send_token.py
--rw-r--r--   0 augier    (1000) augier    (1000)     5324 2023-06-05 13:36:21.000000 django-magicauth-1.0.1/magicauth/settings.py
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.402098 django-magicauth-1.0.1/magicauth/templates/
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.407098 django-magicauth-1.0.1/magicauth/templates/magicauth/
--rw-r--r--   0 augier    (1000) augier    (1000)    10163 2022-04-05 13:57:32.000000 django-magicauth-1.0.1/magicauth/templates/magicauth/email.html
--rw-r--r--   0 augier    (1000) augier    (1000)      373 2022-04-05 13:57:32.000000 django-magicauth-1.0.1/magicauth/templates/magicauth/email.txt
--rw-rw-r--   0 augier    (1000) augier    (1000)      972 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/templates/magicauth/email_sent.html
--rw-rw-r--   0 augier    (1000) augier    (1000)     1995 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/templates/magicauth/login.html
--rw-rw-r--   0 augier    (1000) augier    (1000)      934 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/templates/magicauth/wait.html
--rw-rw-r--   0 augier    (1000) augier    (1000)      698 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/magicauth/urls.py
--rw-r--r--   0 augier    (1000) augier    (1000)      423 2021-07-07 13:42:08.000000 django-magicauth-1.0.1/magicauth/utils.py
--rw-r--r--   0 augier    (1000) augier    (1000)     7119 2024-02-01 08:19:47.000000 django-magicauth-1.0.1/magicauth/views.py
--rw-r--r--   0 augier    (1000) augier    (1000)       38 2024-02-01 08:28:35.409098 django-magicauth-1.0.1/setup.cfg
--rw-r--r--   0 augier    (1000) augier    (1000)     1089 2024-02-01 08:25:56.000000 django-magicauth-1.0.1/setup.py
-drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-02-01 08:28:35.409098 django-magicauth-1.0.1/tests/
--rw-rw-r--   0 augier    (1000) augier    (1000)        0 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/__init__.py
--rw-rw-r--   0 augier    (1000) augier    (1000)      572 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/factories.py
--rw-r--r--   0 augier    (1000) augier    (1000)     2055 2023-03-06 11:17:46.000000 django-magicauth-1.0.1/tests/test_1_GET_login_view.py
--rw-r--r--   0 augier    (1000) augier    (1000)     5281 2022-04-04 13:44:55.000000 django-magicauth-1.0.1/tests/test_2_POST_login_view.py
--rw-rw-r--   0 augier    (1000) augier    (1000)      912 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/test_3_email_sent_view.py
--rw-rw-r--   0 augier    (1000) augier    (1000)     2109 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/test_4_wait_view.py
--rw-rw-r--   0 augier    (1000) augier    (1000)     4235 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/test_5_validate_token_view.py
--rw-r--r--   0 augier    (1000) augier    (1000)      869 2022-04-05 13:57:32.000000 django-magicauth-1.0.1/tests/test_settings.py
--rw-rw-r--   0 augier    (1000) augier    (1000)      247 2021-07-07 12:46:35.000000 django-magicauth-1.0.1/tests/test_url.py
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.778228 django-magicauth-1.0.2/
+-rw-rw-r--   0 augier    (1000) augier    (1000)     1068 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/LICENSE
+-rw-rw-r--   0 augier    (1000) augier    (1000)       74 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/MANIFEST.in
+-rw-r--r--   0 augier    (1000) augier    (1000)     8053 2024-05-22 12:29:59.777228 django-magicauth-1.0.2/PKG-INFO
+-rw-r--r--   0 augier    (1000) augier    (1000)     7396 2024-01-31 15:40:41.000000 django-magicauth-1.0.2/README.md
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.771228 django-magicauth-1.0.2/django_magicauth.egg-info/
+-rw-r--r--   0 augier    (1000) augier    (1000)     8053 2024-05-22 12:29:59.000000 django-magicauth-1.0.2/django_magicauth.egg-info/PKG-INFO
+-rw-r--r--   0 augier    (1000) augier    (1000)      956 2024-05-22 12:29:59.000000 django-magicauth-1.0.2/django_magicauth.egg-info/SOURCES.txt
+-rw-r--r--   0 augier    (1000) augier    (1000)        1 2024-05-22 12:29:59.000000 django-magicauth-1.0.2/django_magicauth.egg-info/dependency_links.txt
+-rw-r--r--   0 augier    (1000) augier    (1000)       16 2024-05-22 12:29:59.000000 django-magicauth-1.0.2/django_magicauth.egg-info/top_level.txt
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.774228 django-magicauth-1.0.2/magicauth/
+-rw-r--r--   0 augier    (1000) augier    (1000)        0 2022-04-04 13:45:02.000000 django-magicauth-1.0.2/magicauth/__init__.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)      212 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/admin.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)      125 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/apps.py
+-rw-r--r--   0 augier    (1000) augier    (1000)      704 2022-04-04 13:45:02.000000 django-magicauth-1.0.2/magicauth/forms.py
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.774228 django-magicauth-1.0.2/magicauth/migrations/
+-rw-rw-r--   0 augier    (1000) augier    (1000)     1364 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/migrations/0001_initial.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)        0 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/migrations/__init__.py
+-rw-r--r--   0 augier    (1000) augier    (1000)      668 2022-04-04 13:45:02.000000 django-magicauth-1.0.2/magicauth/models.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)     1691 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/next_url.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     2481 2024-05-22 12:20:29.000000 django-magicauth-1.0.2/magicauth/otp_forms.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     2772 2023-06-05 13:48:50.000000 django-magicauth-1.0.2/magicauth/send_token.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     5324 2023-06-05 13:36:21.000000 django-magicauth-1.0.2/magicauth/settings.py
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.769228 django-magicauth-1.0.2/magicauth/templates/
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.775228 django-magicauth-1.0.2/magicauth/templates/magicauth/
+-rw-r--r--   0 augier    (1000) augier    (1000)    10163 2022-04-05 13:57:32.000000 django-magicauth-1.0.2/magicauth/templates/magicauth/email.html
+-rw-r--r--   0 augier    (1000) augier    (1000)      373 2022-04-05 13:57:32.000000 django-magicauth-1.0.2/magicauth/templates/magicauth/email.txt
+-rw-rw-r--   0 augier    (1000) augier    (1000)      972 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/templates/magicauth/email_sent.html
+-rw-rw-r--   0 augier    (1000) augier    (1000)     1995 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/templates/magicauth/login.html
+-rw-rw-r--   0 augier    (1000) augier    (1000)      934 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/templates/magicauth/wait.html
+-rw-rw-r--   0 augier    (1000) augier    (1000)      698 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/magicauth/urls.py
+-rw-r--r--   0 augier    (1000) augier    (1000)      423 2021-07-07 13:42:08.000000 django-magicauth-1.0.2/magicauth/utils.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     7736 2024-05-22 12:20:29.000000 django-magicauth-1.0.2/magicauth/views.py
+-rw-r--r--   0 augier    (1000) augier    (1000)       38 2024-05-22 12:29:59.778228 django-magicauth-1.0.2/setup.cfg
+-rw-r--r--   0 augier    (1000) augier    (1000)     1089 2024-05-22 12:26:52.000000 django-magicauth-1.0.2/setup.py
+drwxr-xr-x   0 augier    (1000) augier    (1000)        0 2024-05-22 12:29:59.777228 django-magicauth-1.0.2/tests/
+-rw-rw-r--   0 augier    (1000) augier    (1000)        0 2024-05-21 13:38:07.000000 django-magicauth-1.0.2/tests/__init__.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)      572 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/tests/factories.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     2055 2024-05-21 13:18:26.000000 django-magicauth-1.0.2/tests/test_1_GET_login_view.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     5971 2024-05-22 12:20:29.000000 django-magicauth-1.0.2/tests/test_2_POST_login_view.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)      912 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/tests/test_3_email_sent_view.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)     2109 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/tests/test_4_wait_view.py
+-rw-r--r--   0 augier    (1000) augier    (1000)     4440 2024-05-21 11:33:44.000000 django-magicauth-1.0.2/tests/test_5_validate_token_view.py
+-rw-r--r--   0 augier    (1000) augier    (1000)      869 2022-04-05 13:57:32.000000 django-magicauth-1.0.2/tests/test_settings.py
+-rw-rw-r--   0 augier    (1000) augier    (1000)      247 2021-07-07 12:46:35.000000 django-magicauth-1.0.2/tests/test_url.py
```

### Comparing `django-magicauth-1.0.1/LICENSE` & `django-magicauth-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/PKG-INFO` & `django-magicauth-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magicauth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Password-less authentication: login by clicking on a magic link received by email.
 Home-page: 
 Author: 
 Author-email: 
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django-magicauth-1.0.1/README.md` & `django-magicauth-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/django_magicauth.egg-info/PKG-INFO` & `django-magicauth-1.0.2/django_magicauth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magicauth
-Version: 1.0.1
+Version: 1.0.2
 Summary: Password-less authentication: login by clicking on a magic link received by email.
 Home-page: 
 Author: 
 Author-email: 
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
```

### Comparing `django-magicauth-1.0.1/django_magicauth.egg-info/SOURCES.txt` & `django-magicauth-1.0.2/django_magicauth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/forms.py` & `django-magicauth-1.0.2/magicauth/forms.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/migrations/0001_initial.py` & `django-magicauth-1.0.2/magicauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/models.py` & `django-magicauth-1.0.2/magicauth/models.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/next_url.py` & `django-magicauth-1.0.2/magicauth/next_url.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/otp_forms.py` & `django-magicauth-1.0.2/magicauth/otp_forms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+from datetime import timedelta
+
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import RegexValidator
+from django.utils import timezone
 from django.utils.translation import gettext as _
 
-try:
-    from django_otp import user_has_device, devices_for_user
-except ImportError:
-    pass
-
+from magicauth.models import MagicToken
 from magicauth import settings as magicauth_settings
 
 
 class OTPForm(forms.Form):
     OTP_NUM_DIGITS = magicauth_settings.OTP_NUM_DIGITS
     otp_token = forms.CharField(
         max_length=OTP_NUM_DIGITS,
         min_length=OTP_NUM_DIGITS,
         validators=[RegexValidator(r"^\d{6}$")],
         label=_(
             "Entrez le code à %(OTP_NUM_DIGITS)s chiffres généré par votre téléphone ou votre carte OTP"
-        ) % {"OTP_NUM_DIGITS": OTP_NUM_DIGITS},
+        )
+        % {"OTP_NUM_DIGITS": OTP_NUM_DIGITS},
         widget=forms.TextInput(attrs={"autocomplete": "off"}),
     )
 
     def __init__(self, user, *args, **kwargs):
         super(OTPForm, self).__init__(*args, **kwargs)
         self.user = user
 
     def clean_otp_token(self):
+        from django_otp import user_has_device, devices_for_user
+
         otp_token = self.cleaned_data["otp_token"]
         user = self.user
         if not user_has_device(user):
             raise ValidationError(
                 _(
                     "Le système n'a pas trouvé d'appareil (carte OTP ou générateur sur téléphone) pour votre compte. "
                     "Contactez le support pour en ajouter un."
@@ -39,7 +41,27 @@
             )
 
         for device in devices_for_user(user):
             if device.verify_is_allowed() and device.verify_token(otp_token):
                 return otp_token
 
         raise ValidationError(_("Ce code n'est pas valide."))
+
+
+class TokenValidationForm(forms.Form):
+    token = forms.CharField()
+
+    def clean_token(self):
+        token = self.cleaned_data.get("token")
+        try:
+            token = MagicToken.objects.get(key=token)
+            if token.created < timezone.now() - timedelta(
+                seconds=magicauth_settings.TOKEN_DURATION_SECONDS
+            ):
+                # Do not raise here as we still want to cache the token in cleaned_data
+                # for further manipulations
+                self.add_error("token", ValidationError("", code="token_expired"))
+            return token
+        except MagicToken.DoesNotExist:
+            raise ValidationError("", code="token_does_not_exist")
+        except MagicToken.MultipleObjectsReturned:
+            raise ValidationError("", code="multiple_token_returned")
```

### Comparing `django-magicauth-1.0.1/magicauth/send_token.py` & `django-magicauth-1.0.2/magicauth/send_token.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/settings.py` & `django-magicauth-1.0.2/magicauth/settings.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/templates/magicauth/email.html` & `django-magicauth-1.0.2/magicauth/templates/magicauth/email.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/templates/magicauth/email_sent.html` & `django-magicauth-1.0.2/magicauth/templates/magicauth/email_sent.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/templates/magicauth/login.html` & `django-magicauth-1.0.2/magicauth/templates/magicauth/login.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/templates/magicauth/wait.html` & `django-magicauth-1.0.2/magicauth/templates/magicauth/wait.html`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/urls.py` & `django-magicauth-1.0.2/magicauth/urls.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/magicauth/views.py` & `django-magicauth-1.0.2/magicauth/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from datetime import timedelta
 import logging
 
 from django.contrib import messages
 from django.contrib.auth import login
+from django.forms.utils import ErrorList
 from django.shortcuts import redirect
 from django.urls import reverse_lazy, reverse
 from django.utils import timezone
+from django.utils.decorators import method_decorator
+from django.views.decorators.http import require_GET
 from django.views.generic import View, FormView, TemplateView
 from django.contrib.auth import get_user_model
 from magicauth import settings as magicauth_settings
 from magicauth.forms import EmailForm
 
 from magicauth.models import MagicToken
 from magicauth.next_url import NextUrlMixin
 from magicauth.send_token import SendTokenMixin
 
 try:
-    from magicauth.otp_forms import OTPForm
+    from magicauth.otp_forms import OTPForm, TokenValidationForm
 except ImportError:
     pass  # OTP form class is optional
 
 
 logger = logging.getLogger()
 
 
@@ -38,23 +41,22 @@
     def get(self, request, *args, **kwargs):
         if request.user.is_authenticated:
             next_url = self.get_next_url(self.request)
             return redirect(next_url)
         return super(LoginView, self).get(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
-        context = super(LoginView, self).get_context_data(**kwargs)
-        context[
-            "LOGGED_IN_REDIRECT_URL_NAME"
-        ] = magicauth_settings.LOGGED_IN_REDIRECT_URL_NAME
-        context["LOGOUT_URL_NAME"] = magicauth_settings.LOGOUT_URL_NAME
-        context["OTP_enabled"] = magicauth_settings.ENABLE_2FA
-        if magicauth_settings.ENABLE_2FA:
-            context["OTP_form"] = self.get_otp_form(self.request.user)
-        return context
+        if magicauth_settings.ENABLE_2FA and "OTP_form" not in kwargs:
+            kwargs["OTP_form"] = self.get_otp_form()
+        return super(LoginView, self).get_context_data(
+            **kwargs,
+            LOGGED_IN_REDIRECT_URL_NAME=magicauth_settings.LOGGED_IN_REDIRECT_URL_NAME,
+            LOGOUT_URL_NAME=magicauth_settings.LOGOUT_URL_NAME,
+            OTP_enabled=magicauth_settings.ENABLE_2FA,
+        )
 
     def get_success_url(self, **kwargs):
         url = reverse_lazy("magicauth-email-sent")
         # Use encoded next URL before including it in a string
         next_url_quoted = self.get_next_url_encoded(self.request)
         return f"{url}?next={next_url_quoted}"
 
@@ -74,25 +76,28 @@
     def get_user(self, user_email):
         email_field = "%s__iexact" % magicauth_settings.EMAIL_FIELD
         return get_user_model().objects.get(**{email_field: user_email})
 
     def otp_form_invalid(self, form, otp_form):
         for error in otp_form.errors["otp_token"]:
             form.add_error("email", error)
-        return self.form_invalid(form)
+
+        return self.render_to_response(
+            self.get_context_data(form=form, OTP_form=otp_form)
+        )
 
     def get_otp_form_class(self):
         return self.otp_form_class
 
-    def get_otp_form(self, user):
+    def get_otp_form(self, user=None):
         return self.get_otp_form_class()(**self.get_otp_form_kwargs(user))
 
     def get_otp_form_kwargs(self, user=None):
         kwargs = {
-            "user": user,
+            "user": user or self.request.user,
             "initial": self.get_initial(),
             "prefix": self.get_prefix(),
         }
 
         if self.request.method in ("POST", "PUT"):
             kwargs.update(
                 {
@@ -132,66 +137,77 @@
         )
         next_url_quoted = self.get_next_url_encoded(self.request)
         context["next_step_url"] = f"{validate_token_url}?next={next_url_quoted}"
         context["WAIT_SECONDS"] = magicauth_settings.WAIT_SECONDS
         return context
 
 
-class ValidateTokenView(NextUrlMixin, View):
+@method_decorator(require_GET, name="dispatch")
+class ValidateTokenView(NextUrlMixin, FormView):
+    form_class = TokenValidationForm
     """
     Step 5 of login process : you visit the ValidateTokenView that validates the token, logs you in,
     and redirects you to the url in the "next" param (or the default view if no next).
 
     Either you clicked a link to this page in your email, or you got redirected from step 4
     (WaitView).
 
     If the token is invalid, you are not logged in, and you are redirected to LoginView (step 1) to
     start over.
     """
 
-    @staticmethod
-    def get_valid_token(key):
-        duration = magicauth_settings.TOKEN_DURATION_SECONDS
-        try:
-            token = MagicToken.objects.get(key=key)
-        except MagicToken.DoesNotExist:
-            return None
-        except MagicToken.MultipleObjectsReturned:
-            return None
+    def dispatch(self, request, *args, **kwargs):
+        if request.user.is_authenticated:
+            return redirect(self.get_success_url())
+        return super().dispatch(request, *args, **kwargs)
 
-        if token.created < timezone.now() - timedelta(seconds=duration):
-            token.delete()
-            return None
-        return token
+    def get_form_kwargs(self):
+        return {**super().get_form_kwargs(), "data": {"token": self.kwargs.get("key")}}
 
     def get(self, request, *args, **kwargs):
-        if request.user.is_authenticated:
-            url = self.get_next_url(request)
-            return redirect(url)
-        token_key = kwargs.get("key")
-        token = self.get_valid_token(token_key)
-        if not token:
-            messages.warning(
-                self.request,
-                "Ce lien de connexion ne fonctionne plus. "
-                "Pour en recevoir un nouveau, nous vous invitons à renseigner "
-                "votre email ci-dessous puis à cliquer sur valider.",
-            )
-            return redirect("magicauth-login")
-        url = self.get_next_url(request)
+        form = self.get_form()
+        if form.is_valid():
+            return self.form_valid(form)
+        else:
+            return self.form_invalid(form)
+
+    def form_invalid(self, form):
+        token = form.cleaned_data.get("token")
+        error_codes = [err.code for err in form.errors.get("token", ErrorList()).data]
+        if "token_expired" in error_codes:
+            token.delete()
+
+        return self.token_invalid()
+
+    def token_invalid(self):
+        messages.warning(
+            self.request,
+            "Ce lien de connexion ne fonctionne plus. "
+            "Pour en recevoir un nouveau, nous vous invitons à renseigner "
+            "votre email ci-dessous puis à cliquer sur valider.",
+        )
+        return redirect(reverse("magicauth-login"))
+
+    def form_valid(self, form):
+        # Early compute success URL for validation before login
+        success_url = self.get_success_url()
+
+        token = form.cleaned_data["token"]
         try:
             login(
                 self.request,
                 token.user,
                 backend=magicauth_settings.DEFAULT_AUTHENTICATION_BACKEND,
             )
         except ValueError as e:
             raise ValueError(
-                "You have multiple authentication backends configured and therefore must "
-                "define the MAGICAUTH_DEFAULT_AUTHENTICATION_BACKEND setting. "
+                "You have multiple authentication backends configured and therefore "
+                "must define the MAGICAUTH_DEFAULT_AUTHENTICATION_BACKEND setting. "
                 "MAGICAUTH_DEFAULT_AUTHENTICATION_BACKEND should be a "
                 "dotted import path string."
             ) from e
-        MagicToken.objects.filter(
-            user=token.user
-        ).delete()  # Remove them all for this user
-        return redirect(url)
+        # Remove them all for this user
+        MagicToken.objects.filter(user=token.user).delete()
+        return redirect(success_url)
+
+    def get_success_url(self):
+        return self.get_next_url(self.request)
```

### Comparing `django-magicauth-1.0.1/setup.py` & `django-magicauth-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name="django-magicauth",
-    version="1.0.1",
+    version="1.0.2",
     packages=find_packages(),
     include_package_data=True,
     license="",
     description=(
         "Password-less authentication: login by clicking on "
         "a magic link received by email."),
     long_description=README,
```

### Comparing `django-magicauth-1.0.1/tests/factories.py` & `django-magicauth-1.0.2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/tests/test_1_GET_login_view.py` & `django-magicauth-1.0.2/tests/test_1_GET_login_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/tests/test_2_POST_login_view.py` & `django-magicauth-1.0.2/tests/test_2_POST_login_view.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from django.core import mail
 from django.shortcuts import reverse
 from faker import Factory as FakerFactory
 from magicauth import settings
 from magicauth.models import MagicToken
 from tests import factories
 
-'''
+"""
 Step 2 of login process : see doc in magicauth/views.py for step details
-'''
+"""
 
 pytestmark = mark.django_db
 
 
 def post_email(client, email):
     url = reverse("magicauth-login")
     return client.post(url, data={"email": email})
@@ -82,20 +82,22 @@
     assert "invalid" in str(response.content)
 
 
 def test_posting_unknown_email_does_not_send_email(client):
     post_email(client, "unknown@email.com")
     assert len(mail.outbox) == 0
 
+
 # Tests with OTPs
 def post_email_and_OTP(client, email, OTP):
     url = reverse("magicauth-login")
     data = {"email": email, "otp_token": OTP}
     return client.post(url, data=data)
 
+
 def test_posting_good_email_and_good_totp_success(client):
     settings.ENABLE_2FA = True
     token = factories.MagicTokenFactory()
     thierry = token.user
     device = thierry.staticdevice_set.create()
     device.token_set.create(token="123456")
 
@@ -111,15 +113,19 @@
     thierry = token.user
     device = thierry.staticdevice_set.create()
     device.token_set.create(token="123456")
 
     response = post_email_and_OTP(client, thierry.email, "567654")
 
     assert response.status_code == 200
-    assert "Ce code n&#x27;est pas valide." in str(response.content)
+    assert len(response.context_data["OTP_form"].errors) == 1
+    assert (
+        response.context_data["OTP_form"].errors["otp_token"][0]
+        == "Ce code n'est pas valide."
+    )
     assert len(mail.outbox) == 0
 
 
 def test_posting_wrong_email_and_wrong_otp_error(client):
     settings.ENABLE_2FA = True
     token = factories.MagicTokenFactory()
     thierry = token.user
@@ -128,28 +134,45 @@
 
     response = post_email_and_OTP(client, "unknown@email.com", "567654")
 
     assert response.status_code == 200
     assert "invalid" in str(response.content)
     assert len(mail.outbox) == 0
 
+
+def test_posting_good_email_and_has_not_otp_error(client):
+    settings.ENABLE_2FA = True
+    user = factories.UserFactory()
+
+    response = post_email_and_OTP(client, user.email, "567654")
+
+    assert response.status_code == 200
+    assert len(response.context_data["OTP_form"].errors) == 1
+    assert response.context_data["OTP_form"].errors["otp_token"][0] == (
+        "Le système n'a pas trouvé d'appareil (carte OTP ou générateur sur téléphone) "
+        "pour votre compte. Contactez le support pour en ajouter un."
+    )
+    assert len(mail.outbox) == 0
+
+
 def test_thierry_has_several_devices_first_device(client):
     settings.ENABLE_2FA = True
     token = factories.MagicTokenFactory()
     thierry = token.user
     device_1 = thierry.staticdevice_set.create()
     device_1.token_set.create(token="123456")
     device_2 = thierry.staticdevice_set.create()
     device_2.token_set.create(token="111111")
 
     response = post_email_and_OTP(client, thierry.email, "123456")
 
     assert response.status_code == 302
     assert len(mail.outbox) == 1
 
+
 def test_thierry_has_several_devices_second_device(client):
     settings.ENABLE_2FA = True
     token = factories.MagicTokenFactory()
     thierry = token.user
     device_1 = thierry.staticdevice_set.create()
     device_1.token_set.create(token="123456")
     device_2 = thierry.staticdevice_set.create()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `django-magicauth-1.0.1/tests/test_3_email_sent_view.py` & `django-magicauth-1.0.2/tests/test_3_email_sent_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/tests/test_4_wait_view.py` & `django-magicauth-1.0.2/tests/test_4_wait_view.py`

 * *Files identical despite different names*

### Comparing `django-magicauth-1.0.1/tests/test_5_validate_token_view.py` & `django-magicauth-1.0.2/tests/test_5_validate_token_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 def test_opening_magic_link_with_valid_token_redirects(client):
     token = factories.MagicTokenFactory()
     response = open_magic_link(client, token)
     assert response.status_code == 302
     assert response.url == "/landing/"
 
 
+def test_post_trigger_http_405(client):
+    token = factories.MagicTokenFactory()
+    response = client.post(reverse("magicauth-validate-token", args=[token.key]))
+    assert response.status_code == 405
+
+
 def test_opening_magic_link_with_a_next_sets_a_new_url(client):
     token = factories.MagicTokenFactory()
     next_url_raw = "/test_dashboard/?a=test&b=test"
     response = open_magic_link(client, token, next_url_raw)
     assert response.status_code == 302
     assert response.url == next_url_raw
```

### Comparing `django-magicauth-1.0.1/tests/test_settings.py` & `django-magicauth-1.0.2/tests/test_settings.py`

 * *Files identical despite different names*

