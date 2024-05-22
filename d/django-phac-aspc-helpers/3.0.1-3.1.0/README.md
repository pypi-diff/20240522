# Comparing `tmp/django_phac_aspc_helpers-3.0.1.tar.gz` & `tmp/django_phac_aspc_helpers-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_phac_aspc_helpers-3.0.1.tar", last modified: Tue May 21 18:51:15 2024, max compression
+gzip compressed data, was "django_phac_aspc_helpers-3.1.0.tar", last modified: Wed May 22 19:01:41 2024, max compression
```

## Comparing `django_phac_aspc_helpers-3.0.1.tar` & `django_phac_aspc_helpers-3.1.0.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24964 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 18:51:15.000000 django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/comma_separated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4869 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_utils/include_from_dtl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.100214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/language.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/configure_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/json_post_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/ready.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.108214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.104214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.112214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/localization_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/localization.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/localization_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configuration_verification_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/env_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/is_running_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/wet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/phac_aspc/vanilla.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-21 18:51:15.120214 django_phac_aspc_helpers-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/jinja2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/model_factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:15.116214 django_phac_aspc_helpers-3.0.1/testapp/tests/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_comma_separated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    12721 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_excel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_phac_aspc_wet.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_vanilla_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/pytest_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-21 18:51:02.000000 django_phac_aspc_helpers-3.0.1/testapp/tests/test_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24964 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26234 2024-05-22 19:01:41.000000 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-22 19:01:41.000000 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:01:41.000000 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 19:01:41.000000 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 19:01:41.000000 django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.355286 django_phac_aspc_helpers-3.1.0/phac_aspc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.355286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.355286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/decorators/admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/comma_separated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15719 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/jinja_dtl_interop_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/jinja_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/jinja_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/jinja_utils/include_from_dtl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/en_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/language.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8225 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/configure_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/json_post_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/ready/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/ready/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/ready/ready.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.359286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.351286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.363286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/urls/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/urls/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/urls/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/views/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/decorators/localization_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/localization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/localization_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/logging_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/security_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/configuration_verification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/configure_settings_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/env_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/is_running_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/wet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/phac_aspc/vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.367286 django_phac_aspc_helpers-3.1.0/testapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/jinja2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/model_factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/testapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:41.371286 django_phac_aspc_helpers-3.1.0/testapp/tests/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_comma_separated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14757 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_excel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_phac_aspc_wet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_vanilla_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/pytest_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-22 19:01:30.000000 django_phac_aspc_helpers-3.1.0/testapp/tests/test_rules.py
```

### Comparing `django_phac_aspc_helpers-3.0.1/LICENSE` & `django_phac_aspc_helpers-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/PKG-INFO` & `django_phac_aspc_helpers-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 3.0.1
+Version: 3.1.0
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_phac_aspc_helpers-3.0.1/README.md` & `django_phac_aspc_helpers-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/PKG-INFO` & `django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 3.0.1
+Version: 3.1.0
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django_phac_aspc_helpers-3.0.1/django_phac_aspc_helpers.egg-info/SOURCES.txt` & `django_phac_aspc_helpers-3.1.0/django_phac_aspc_helpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/admin/decorators/admin_decorators.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/admin/decorators/admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/comma_separated_field.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/comma_separated_field.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/excel.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/excel.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import csv
 from django.core.paginator import Paginator
 from django.db.models import QuerySet
 from django.views import View
 from django.http import HttpResponse
 from django.utils.functional import Promise
 from django.utils.safestring import SafeString
+from openpyxl.cell import WriteOnlyCell
+
+from openpyxl.utils import get_column_letter
 
 try:
     import openpyxl
     from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
     from openpyxl.utils import escape as escapeSvc
 except (ImportError, ModuleNotFoundError) as exc:
     raise ImportError("must install openpyxl==3.0.10 to use excel helpers") from exc
@@ -73,35 +76,49 @@
 
 
 class Column:
     """
     Base class to write columns in a sheet
     """
 
+    style = None
+    column_width = None
+
+    def __init__(self, style=None, column_width=None):
+        self.style = style
+        self.column_width = column_width
+
     def get_header(self):
         """return a header string for the column"""
         raise NotImplementedError()
 
     def get_value(self, record):
         """return this column's intended cell value for a record"""
         raise NotImplementedError()
 
     def serialize_value(self, value):
         return serialize_value(value)
 
     def get_serialized_value(self, record):
         return self.serialize_value(self.get_value(record))
 
+    def get_style(self):
+        return self.style
+
+    def get_column_width(self):
+        return self.column_width
+
 
 class ModelColumn(Column):
     """
     shorthand for defining a column that writes a scalar model field (non foreign-key)
     """
 
-    def __init__(self, model_cls, field_name, header_value=None):
+    def __init__(self, model_cls, field_name, header_value=None, **kwargs):
+        super().__init__(**kwargs)
         self.header_value = header_value
         self.model_cls = model_cls
         self.field_name = field_name
         self.get_val = create_field_val_getter(field_name)
 
     def get_header(self):
         # pylint: disable=protected-access
@@ -112,15 +129,16 @@
         return escape_for_xlsx(header_value)
 
     def get_value(self, record):
         return self.get_val(record)
 
 
 class ChoiceColumn(Column):
-    def __init__(self, model_cls, field_name, header_value=None):
+    def __init__(self, model_cls, field_name, header_value=None, **kwargs):
+        super().__init__(**kwargs)
         self.header_value = header_value
         self.model_cls = model_cls
         self.field_name = field_name
 
     def get_header(self):
         # pylint: disable=protected-access
         header_value = (
@@ -131,15 +149,16 @@
 
     def get_value(self, record):
         method_name = "get_" + self.field_name + "_display"
         return getattr(record, method_name)()
 
 
 class CustomColumn(Column):
-    def __init__(self, header, get_val):
+    def __init__(self, header, get_val, **kwargs):
+        super().__init__(**kwargs)
         self.header = header
         self.get_val = get_val
 
     def get_header(self):
         return self.header
 
     def get_value(self, record):
@@ -151,15 +170,17 @@
     def __init__(
         self,
         model: type,
         field_name: str,
         get_related_str: callable = None,
         delimiter: str = ", ",
         header=None,
+        **kwargs,
     ):
+        super().__init__(**kwargs)
         self.model = model
         self.field_name = field_name
         self.header = header
         if get_related_str:
             self.get_related_str = get_related_str
         else:
             self.get_related_str = lambda x, *args: str(x)
@@ -291,14 +312,15 @@
     pass
 
 
 class AbstractSheetWriter(AbstractWriter):
     # pylint: disable=W0223
 
     sheet_name = None
+    header_style = None
 
     def __init__(self, *args, workbook=None, sheet_name=None, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.workbook = workbook
 
         if sheet_name:
@@ -308,25 +330,60 @@
         if not self.sheet_name:
             raise NotImplementedError(
                 "must override get_sheet_name() or pass a sheet_name"
             )
 
         return self.sheet_name
 
+    def get_header_style(self):
+        """
+        To be overwritten by child classes when a style is to be applied to the
+        header row.  If overwritten, should return a Style object.
+        """
+        return self.header_style
+
+    def get_column_widths(self):
+        """
+        Returns an array of column widths as set in the get_column_configs.
+        """
+        return [col.get_column_width() for col in self.get_column_configs()]
+
     def write(self):
         worksheet = self.workbook.create_sheet(title=self.get_sheet_name())
 
-        worksheet.append(self.get_header_row())
+        for col_index, column_width in enumerate(self.get_column_widths()):
+            if column_width is not None:
+                column_letter = get_column_letter(col_index + 1)
+                worksheet.column_dimensions[column_letter].width = column_width
+
+        header_labels = self.get_header_row()
+        # pylint: disable=E1128
+        header_style = self.get_header_style()
+
+        header_row = []
+        for label in header_labels:
+            cell = WriteOnlyCell(worksheet, value=label)
+
+            if header_style:
+                cell.style = header_style
+            header_row.append(cell)
+
+        worksheet.append(header_row)
 
         iterator = self.get_iterator()
+
         for record in iterator:
             xl_row = []
             for col in self.get_column_configs():
                 xl_val = col.get_serialized_value(record)
-                xl_row.append(xl_val)
+                cell = WriteOnlyCell(worksheet, value=xl_val)
+                style = col.get_style()
+                if style:
+                    cell.style = style
+                xl_row.append(cell)
 
             worksheet.append(xl_row)
 
 
 class ModelToSheetWriter(AbstractSheetWriter, AbstractModelWriter):
     def get_sheet_name(self):
         try:
```

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/fields.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         for attr in migration_ignored_attrs:
             kwargs.pop(attr, None)
         return name, path, args, kwargs
 
 
+# pylint: disable=abstract-method
 class ManyToManyField(DescriptionMixin, models.ManyToManyField):
     pass
 
 
 class EmptyToNullMixin:
     """
     Replace NULL values with empty string ""
@@ -102,14 +103,15 @@
         # according to django docs, TextField char-limits are not enforced at the DB level
         name, path, args, kwargs = super().deconstruct()
         kwargs.pop("max_length", None)
 
         return name, path, args, kwargs
 
 
+# pylint: disable=abstract-method
 class ForeignKey(DescriptionMixin, models.ForeignKey):
     pass
 
 
 choices_by_type = {
     "yes_or_no": ((True, "yes"), (False, "no")),
     "true_or_false": ((True, "true"), (False, "false")),
@@ -149,14 +151,15 @@
     pass
 
 
 class SlugField(DescriptionMixin, models.SlugField):
     pass
 
 
+# pylint: disable=abstract-method
 class OneToOneField(DescriptionMixin, models.OneToOneField):
     pass
 
 
 class AutoField(DescriptionMixin, models.AutoField):
     pass
```

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/apps.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/apps.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/backend.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/backend.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/auth/views.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/auth/views.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/jinja_dtl_interop_utils.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/jinja_dtl_interop_utils.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/en_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/locale/language.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/locale/language.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/configure_logging.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/configure_logging.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/json_post_handlers.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/json_post_handlers.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/logging/utils.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/logging/utils.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/ready/__init__.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/ready/__init__.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en-fr__dark.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/en__dark.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr-en__dark.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/static/phac_aspc_helpers/phac_logos/fr__dark.svg`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/__init__.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_include_from_jinja.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_inline_svg.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/urls/auth.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/urls/auth.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/helpers/views/wet.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/helpers/views/wet.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/localization/decorators/localization_decorators.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/localization/decorators/localization_decorators.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/logging.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/logging_env.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/logging_env.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/security.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/security_env.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/security_env.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configuration_verification_utils.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/configuration_verification_utils.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/configure_settings_for_tests.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/configure_settings_for_tests.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/django/settings/utils/env_utils.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/django/settings/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/rules.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/rules.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/phac_aspc/vanilla.py` & `django_phac_aspc_helpers-3.1.0/phac_aspc/vanilla.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/setup.cfg` & `django_phac_aspc_helpers-3.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-phac_aspc-helpers
-version = 3.0.1
+version = 3.1.0
 description = Set of helpers for Django used at PHAC-ASPC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-phac_aspc-helpers
 author = Luc Belliveau
 author_email = luc.belliveau@phac-aspc.gc.ca
 license = MIT
```

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/migrations/0001_initial.py` & `django_phac_aspc_helpers-3.1.0/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/model_factories.py` & `django_phac_aspc_helpers-3.1.0/testapp/model_factories.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/models.py` & `django_phac_aspc_helpers-3.1.0/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/settings.py` & `django_phac_aspc_helpers-3.1.0/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/conftest.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/conftest.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_admin_decorators.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_comma_separated_field.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_comma_separated_field.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_excel_utils.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_excel_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 from django.test import RequestFactory
 import random
 
 from openpyxl import Workbook
 from testapp.models import Book, Author
 from testapp.model_factories import TagFactory, BookFactory, AuthorFactory
 
+from openpyxl.styles import (
+    Font,
+    NamedStyle,
+    Alignment,
+    PatternFill,
+    Border,
+    Side,
+)
+
 
 def make_request():
     req_factory = RequestFactory()
     return req_factory.get("/fake-url")
 
 
 def instantiate_view(ViewClass):
@@ -59,15 +68,15 @@
 
     class BookSheetWriter(ModelToSheetWriter):
 
         def get_column_configs(self):
             return columns
 
     with django_assert_max_num_queries(4):
-        wb = Workbook()
+        wb = Workbook(write_only=True)
         writer = BookSheetWriter(
             workbook=wb,
             queryset=Book.objects.all().prefetch_related("author", "tags"),
             sheet_name="books",
         )
         writer.write()
 
@@ -291,15 +300,15 @@
     constructor_spy.assert_called_with(iterator=qs, workbook=wbInstanceMock)
     write_spy.assert_called_once()
     wbInstanceMock.save.assert_called_once()
     wbInstanceMock.save.assert_called_with(response)
 
 
 def test_various_writer_apis():
-    wb = Workbook()
+    wb = Workbook(write_only=True)
     qs = Book.objects.all().prefetch_related("author", "tags")
 
     class BookWriter(ModelToSheetWriter):
         model = Book
 
     with pytest.raises(WriterConfigException):
         # iterator kwarg should fail at __init__
@@ -346,15 +355,15 @@
         sheet_name = "books"
 
     BookWriterWithGetIteratorMethodAndSheetName(workbook=wb).write()
 
 
 def test_writer_attr_precedence():
     # sheet_name and queryset kwargs take precedence over class attributes
-    wb = Workbook()
+    wb = Workbook(write_only=True)
     book_qs = Book.objects.all().prefetch_related("author", "tags")
 
     author_qs = Author.objects.all()
 
     class BookWriter(ModelToSheetWriter):
         queryset = book_qs
         sheet_name = "books"
@@ -362,15 +371,15 @@
     author_writer = BookWriter(workbook=wb, queryset=author_qs, sheet_name="authors")
     assert author_writer.queryset == author_qs
     assert author_writer.sheet_name == "authors"
 
 
 def test_writer_get_columns_api():
     create_data()
-    wb = Workbook()
+    wb = Workbook(write_only=True)
     qs = Book.objects.all().prefetch_related("author", "tags")
 
     column_defs = [
         ModelColumn(Book, "title"),
         CustomColumn("Author", lambda x: f"{x.author.first_name} {x.author.last_name}"),
         ManyToManyColumn(Book, "tags"),
     ]
@@ -417,7 +426,66 @@
 
     # non-model writers should raise error if no column configs are provided
     class NonModelWriter(AbstractSheetWriter):
         pass
 
     with pytest.raises(NotImplementedError):
         NonModelWriter(workbook=wb, sheet_name="abc").get_column_configs()
+
+
+def test_sheetwriter_with_column_styles():
+    create_data()
+    wb = Workbook(write_only=True)
+    qs = Book.objects.all().prefetch_related("author", "tags")
+
+    bold_style = NamedStyle(name="bold", font=Font(bold=True))
+    # bold_style.font = Font(bold=True)
+
+    class BookWriterWithStyles(ModelToSheetWriter):
+        columns = [
+            ModelColumn(Book, "title", style=bold_style, column_width=50),
+            CustomColumn(
+                "Author", lambda x: f"{x.author.first_name} {x.author.last_name}"
+            ),
+            ManyToManyColumn(Book, "tags"),
+        ]
+
+    writer = BookWriterWithStyles(workbook=wb, queryset=qs)
+    writer.write()
+
+
+def test_sheetwriter_with_header_style():
+
+    create_data()
+    wb = Workbook(write_only=True)
+    qs = Book.objects.all().prefetch_related("author", "tags")
+
+    border_side = Side(style="thin", color="000000")
+    style = NamedStyle(
+        name="header",
+        font=Font(bold=True),
+        alignment=Alignment(horizontal="center"),
+        fill=PatternFill("solid", fgColor="00C0C0C0"),
+        border=Border(
+            left=border_side,
+            top=border_side,
+            right=border_side,
+            bottom=border_side,
+        ),
+    )
+    # header_style.font = Font(bold=True)
+    # header_style.alignment = Alignment(horizontal="center")
+    # header_style.fill = PatternFill("solid", fgColor="00C0C0C0")
+    # header_style.border = Border(left=bd, top=bd, right=bd, bottom=bd)
+
+    class BookWriterWithHeaderStyle(ModelToSheetWriter):
+        header_style = style
+
+        columns = [
+            ModelColumn(Book, "title"),
+            CustomColumn(
+                "Author", lambda x: f"{x.author.first_name} {x.author.last_name}"
+            ),
+            ManyToManyColumn(Book, "tags"),
+        ]
+
+    BookWriterWithHeaderStyle(workbook=wb, queryset=qs).write()
```

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_phac_aspc_wet.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_ready.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_ready.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/django/test_vanilla_utils.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/django/test_vanilla_utils.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/pytest_runner.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `django_phac_aspc_helpers-3.0.1/testapp/tests/test_rules.py` & `django_phac_aspc_helpers-3.1.0/testapp/tests/test_rules.py`

 * *Files identical despite different names*

