# Comparing `tmp/django_paddle_billing-0.1.2.tar.gz` & `tmp/django_paddle_billing-0.1.3.tar.gz`

## Comparing `django_paddle_billing-0.1.2.tar` & `django_paddle_billing-0.1.3.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.safety-policy.yml
--rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/Makefile
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/requirements.txt
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/.stale.yml
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/release-drafter.yml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/.gitignore
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/dataSources.xml
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/django-paddle-billing.iml
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/misc.xml
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/vcs.xml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/__init__.py
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/manage.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/admin.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/apps.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/models.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/schema.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/tests.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/urls.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/views.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/billing/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/__init__.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/api.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/asgi.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/settings.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/urls.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/example/django_billing/django_billing/wsgi.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/__init__.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/admin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/api.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/apps.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/encoders.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/exceptions.py
--rw-r--r--   0        0        0    25387 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/models.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/settings.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/signals.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/tests.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/urls.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/utils.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/views.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/management/commands/sync_from_paddle.py
--rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/src/django_paddle_billing/migrations/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/tests/test_encoder.py
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/LICENSE
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/README.md
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.safety-policy.yml
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/Makefile
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/requirements.txt
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/.stale.yml
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/release-drafter.yml
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/.gitignore
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/dataSources.xml
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/django-paddle-billing.iml
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/__init__.py
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/manage.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/admin.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/apps.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/models.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/schema.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/tests.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/urls.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/views.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/billing/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/__init__.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/api.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/asgi.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/settings.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/urls.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/example/django_billing/django_billing/wsgi.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/__init__.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/admin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/api.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/apps.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/encoders.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/exceptions.py
+-rw-r--r--   0        0        0    25427 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/models.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/settings.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/signals.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/tests.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/urls.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/utils.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/views.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/management/commands/sync_from_paddle.py
+-rw-r--r--   0        0        0    12471 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0001_initial.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0002_alter_subscription_status.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/tests/test_encoder.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/README.md
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 django_paddle_billing-0.1.3/PKG-INFO
```

### Comparing `django_paddle_billing-0.1.2/.safety-policy.yml` & `django_paddle_billing-0.1.3/.safety-policy.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/CODE_OF_CONDUCT.md` & `django_paddle_billing-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/CONTRIBUTING.md` & `django_paddle_billing-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/Makefile` & `django_paddle_billing-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/requirements.txt` & `django_paddle_billing-0.1.3/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,38 +8,38 @@
     # via pydantic
 api-client==1.3.1
     # via api-client-pydantic
 api-client-pydantic==3.0.0
     # via paddle-billing-client
 asgiref==3.7.2
     # via django
-certifi==2023.11.17
+certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
-django==5.0.1
+django==5.0.4
     # via django-paddle-billing (pyproject.toml)
 django-json-widget==1.1.1
     # via django-paddle-billing (pyproject.toml)
-future==0.18.3
+future==1.0.0
     # via django-json-widget
-idna==3.6
+idna==3.7
     # via requests
-paddle-billing-client==0.2.4
+paddle-billing-client==0.2.6
     # via django-paddle-billing (pyproject.toml)
-pydantic==2.5.3
+pydantic==2.6.4
     # via api-client-pydantic
-pydantic-core==2.14.6
+pydantic-core==2.16.3
     # via pydantic
 requests==2.31.0
     # via api-client
 sqlparse==0.4.4
     # via django
 tenacity==8.2.3
     # via api-client
-typing-extensions==4.9.0
+typing-extensions==4.10.0
     # via
     #   asgiref
     #   pydantic
     #   pydantic-core
-urllib3==2.1.0
+urllib3==2.2.1
     # via requests
```

### Comparing `django_paddle_billing-0.1.2/.github/.stale.yml` & `django_paddle_billing-0.1.3/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/PULL_REQUEST_TEMPLATE.md` & `django_paddle_billing-0.1.3/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/dependabot.yml` & `django_paddle_billing-0.1.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/release-drafter.yml` & `django_paddle_billing-0.1.3/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/ISSUE_TEMPLATE/question.md` & `django_paddle_billing-0.1.3/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.github/workflows/build.yml` & `django_paddle_billing-0.1.3/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,12 +37,12 @@
     steps:
     - uses: actions/download-artifact@v4
       with:
         name: artifacts
         path: dist
 
     - name: Push build artifacts to PyPI
-      uses: pypa/gh-action-pypi-publish@v1.8.11
+      uses: pypa/gh-action-pypi-publish@v1.8.14
       with:
         skip_existing: true
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `django_paddle_billing-0.1.2/.github/workflows/test.yml` & `django_paddle_billing-0.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.idea/dataSources.xml` & `django_paddle_billing-0.1.3/.idea/dataSources.xml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.idea/django-paddle-billing.iml` & `django_paddle_billing-0.1.3/.idea/django-paddle-billing.iml`

 * *Files 16% similar despite different names*

#### Comparing `django_paddle_billing-0.1.2/.idea/django-paddle-billing.iml` & `django_paddle_billing-0.1.3/.idea/django-paddle-billing.iml`

```diff
@@ -9,15 +9,17 @@
         <option name="environment" value="&lt;map/&gt;"/>
         <option name="doNotUseTestRunner" value="false"/>
         <option name="trackFilePattern" value=""/>
       </configuration>
     </facet>
   </component>
   <component name="NewModuleRootManager">
-    <content url="file://$MODULE_DIR$"/>
-    <orderEntry type="jdk" jdkName="Python 3.10 (django-paddle-billing) (2)" jdkType="Python SDK"/>
+    <content url="file://$MODULE_DIR$">
+      <sourceFolder url="file://$MODULE_DIR$/src" isTestSource="false"/>
+    </content>
+    <orderEntry type="jdk" jdkName="Python 3.12 (django-paddle-billing)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="TemplatesService">
     <option name="TEMPLATE_CONFIGURATION" value="Django"/>
   </component>
 </module>
```

### Comparing `django_paddle_billing-0.1.2/.idea/inspectionProfiles/Project_Default.xml` & `django_paddle_billing-0.1.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/manage.py` & `django_paddle_billing-0.1.3/example/django_billing/manage.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/billing/schema.py` & `django_paddle_billing-0.1.3/example/django_billing/billing/schema.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/billing/views.py` & `django_paddle_billing-0.1.3/example/django_billing/billing/views.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/billing/migrations/0001_initial.py` & `django_paddle_billing-0.1.3/example/django_billing/billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/django_billing/api.py` & `django_paddle_billing-0.1.3/example/django_billing/django_billing/api.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/django_billing/settings.py` & `django_paddle_billing-0.1.3/example/django_billing/django_billing/settings.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/example/django_billing/django_billing/urls.py` & `django_paddle_billing-0.1.3/example/django_billing/django_billing/urls.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/admin.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/admin.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/models.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,17 +430,18 @@
     business = models.ForeignKey(
         "Business", on_delete=models.CASCADE, null=True, blank=True, related_name="subscriptions"
     )
     status = models.CharField(
         max_length=10,
         choices=[
             ("active", "Active"),
-            ("trialing", "Trialing"),
+            ("canceled", "Canceled"),
+            ("past_due", "Past Due"),
             ("paused", "Paused"),
-            ("deleted", "Deleted"),
+            ("trialing", "Trialing"),
         ],
     )
     products = models.ManyToManyField(Product, related_name="subscriptions")
 
     class Meta:
         pass
```

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/settings.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/settings.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/signals.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/signals.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/views.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/views.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/management/commands/sync_from_paddle.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/management/commands/sync_from_paddle.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/src/django_paddle_billing/migrations/0001_initial.py` & `django_paddle_billing-0.1.3/src/django_paddle_billing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/tests/test_encoder.py` & `django_paddle_billing-0.1.3/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/.gitignore` & `django_paddle_billing-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/LICENSE` & `django_paddle_billing-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/README.md` & `django_paddle_billing-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/pyproject.toml` & `django_paddle_billing-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_paddle_billing-0.1.2/PKG-INFO` & `django_paddle_billing-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-paddle-billing
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django + Paddle Billing Integration
 Project-URL: Documentation, https://github.com/websideproject/django-paddle-billing#readme
 Project-URL: Issues, https://github.com/websideproject/django-paddle-billing/issues
 Project-URL: Source, https://github.com/websideproject/django-paddle-billing
 Author-email: Benjamin Gervan <benjamin@websideproject.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -16,15 +16,16 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9
 Requires-Dist: django-json-widget
 Requires-Dist: django>=4.2
 Requires-Dist: paddle-billing-client>=0.2.4
 Provides-Extra: all
-Requires-Dist: django-paddle-billing[api,unfold]; extra == 'all'
+Requires-Dist: djangorestframework; extra == 'all'
+Requires-Dist: unfold; extra == 'all'
 Provides-Extra: api
 Requires-Dist: djangorestframework; extra == 'api'
 Provides-Extra: unfold
 Requires-Dist: unfold; extra == 'unfold'
 Description-Content-Type: text/markdown
 
 # Django Paddle Billing
```

