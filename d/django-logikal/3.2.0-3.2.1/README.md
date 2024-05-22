# Comparing `tmp/django_logikal-3.2.0.tar.gz` & `tmp/django_logikal-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_logikal-3.2.0.tar", last modified: Wed May 22 10:14:52 2024, max compression
+gzip compressed data, was "django_logikal-3.2.1.tar", last modified: Wed May 22 11:37:07 2024, max compression
```

## Comparing `django_logikal-3.2.0.tar` & `django_logikal-3.2.1.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 10:14:37.000000 django_logikal-3.2.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 10:14:37.000000 django_logikal-3.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 10:14:37.000000 django_logikal-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 10:14:52.178026 django_logikal-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 10:14:37.000000 django_logikal-3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 10:14:37.000000 django_logikal-3.2.0/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.154025 django_logikal-3.2.0/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/babel/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/babel/django.ini
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/babel/djangojs.ini
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/bibliography.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/local_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/syncdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/production.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/dynamic_site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/production.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/static_site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.150025 django_logikal-3.2.0/django_logikal/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/static/django_logikal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   617492 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   310884 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff
--rw-r--r--   0 runner    (1001) docker     (127)   181500 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   628640 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   325296 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   192916 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   614256 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   312952 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184076 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   630852 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   327188 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195128 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   610876 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   306060 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (127)   180576 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   628352 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323532 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   191804 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    87008 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53528 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    94148 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    93904 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    58800 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86908 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53252 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    40672 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/validation_error.css
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/debug_toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/debug_toolbar/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/base.html.j
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/django_logikal/templates/django_logikal/email/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/email/base.html.j
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/validation_error.html.j
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/django_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-22 10:14:37.000000 django_logikal-3.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/bibliography.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/dynamic.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:14:52.178026 django_logikal-3.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.374435 django_logikal-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 11:36:53.000000 django_logikal-3.2.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 11:36:53.000000 django_logikal-3.2.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 11:36:53.000000 django_logikal-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 11:37:07.374435 django_logikal-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 11:36:53.000000 django_logikal-3.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 11:36:53.000000 django_logikal-3.2.1/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/babel/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/babel/django.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/babel/djangojs.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/bibliography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/local_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/management/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/management/commands/syncdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/management/commands/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.350435 django_logikal-3.2.1/django_logikal/settings/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/common/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/common/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/common/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.354435 django_logikal-3.2.1/django_logikal/settings/dynamic_site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/dynamic_site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/dynamic_site/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/dynamic_site/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/dynamic_site/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/dynamic_site/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.354435 django_logikal-3.2.1/django_logikal/settings/static_site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/static_site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/static_site/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/static_site/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/settings/static_site/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.346435 django_logikal-3.2.1/django_logikal/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.354435 django_logikal-3.2.1/django_logikal/static/django_logikal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   617492 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   310884 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   181500 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   628640 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   325296 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   192916 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   614256 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   312952 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184076 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   630852 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   327188 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195128 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   610876 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   306060 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   180576 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   628352 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323532 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   191804 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    87008 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53528 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    94148 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    93904 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    58800 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86908 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53252 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    40672 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static/django_logikal/validation_error.css
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/templates/debug_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/debug_toolbar/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/templates/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/django_logikal/base.html.j
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/django_logikal/templates/django_logikal/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/django_logikal/email/base.html.j
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/django_logikal/validation_error.html.j
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/templates/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-22 11:36:53.000000 django_logikal-3.2.1/django_logikal/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.374435 django_logikal-3.2.1/django_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 11:37:07.000000 django_logikal-3.2.1/django_logikal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-22 11:36:53.000000 django_logikal-3.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.370435 django_logikal-3.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:37:07.374435 django_logikal-3.2.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/extras/bibliography.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/extras/dynamic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 11:36:53.000000 django_logikal-3.2.1/requirements/extras/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:37:07.374435 django_logikal-3.2.1/setup.cfg
```

### Comparing `django_logikal-3.2.0/.copier-answers.yml` & `django_logikal-3.2.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/LICENSE.txt` & `django_logikal-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/PKG-INFO` & `django_logikal-3.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 3.2.0
+Version: 3.2.1
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django_logikal-3.2.0/compose.yml` & `django_logikal-3.2.1/compose.yml`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/apps.py` & `django_logikal-3.2.1/django_logikal/apps.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/bibliography.py` & `django_logikal-3.2.1/django_logikal/bibliography.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/email.py` & `django_logikal-3.2.1/django_logikal/email.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/logging.py` & `django_logikal-3.2.1/django_logikal/logging.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/management/commands/generate.py` & `django_logikal-3.2.1/django_logikal/management/commands/generate.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/management/commands/syncdb.py` & `django_logikal-3.2.1/django_logikal/management/commands/syncdb.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/management/commands/translate.py` & `django_logikal-3.2.1/django_logikal/management/commands/translate.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/migrations.py` & `django_logikal-3.2.1/django_logikal/migrations.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/run.py` & `django_logikal-3.2.1/django_logikal/run.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/security.py` & `django_logikal-3.2.1/django_logikal/security.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/__init__.py` & `django_logikal-3.2.1/django_logikal/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/common/base.py` & `django_logikal-3.2.1/django_logikal/settings/common/base.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/common/dev.py` & `django_logikal-3.2.1/django_logikal/settings/common/dev.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
     # Core settings
     DEBUG = option_is_set('dev_run')
     DATABASES = {
         'default': {
             'ENGINE': 'django.db.backends.postgresql',
             'HOST': os.getenv('DJANGO_DATABASE_HOST', '127.0.0.1'),
-            'PORT': os.getenv(
-                'DJANGO_DATABASE_PORT',
-                Service('postgres').container_port('5432/tcp'),
+            'PORT': (
+                os.getenv('DJANGO_DATABASE_PORT')
+                or Service('postgres').container_port('5432/tcp')
             ),
             'NAME': os.getenv('DJANGO_DATABASE_NAME', 'dev'),
             'USER': os.getenv('DJANGO_DATABASE_USER', 'dev'),
             'PASSWORD': os.getenv('DJANGO_DATABASE_USER', 'dev'),
         },
     }
```

### Comparing `django_logikal-3.2.0/django_logikal/settings/common/production.py` & `django_logikal-3.2.1/django_logikal/settings/common/production.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/common/testing.py` & `django_logikal-3.2.1/django_logikal/settings/common/testing.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/dynamic_site/base.py` & `django_logikal-3.2.1/django_logikal/settings/dynamic_site/base.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/dynamic_site/dev.py` & `django_logikal-3.2.1/django_logikal/settings/dynamic_site/dev.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/dynamic_site/production.py` & `django_logikal-3.2.1/django_logikal/settings/dynamic_site/production.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/dynamic_site/testing.py` & `django_logikal-3.2.1/django_logikal/settings/dynamic_site/testing.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/settings/static_site/base.py` & `django_logikal-3.2.1/django_logikal/settings/static_site/base.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/sitemap.py` & `django_logikal-3.2.1/django_logikal/sitemap.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Light.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-README.txt` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-README.txt`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts.css` & `django_logikal-3.2.1/django_logikal/static/django_logikal/fonts.css`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static/django_logikal/validation_error.css` & `django_logikal-3.2.1/django_logikal/static/django_logikal/validation_error.css`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/static.py` & `django_logikal-3.2.1/django_logikal/static.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/django_logikal/base.html.j` & `django_logikal-3.2.1/django_logikal/templates/django_logikal/base.html.j`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/django_logikal/validation_error.html.j` & `django_logikal-3.2.1/django_logikal/templates/django_logikal/validation_error.html.j`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/extensions.py` & `django_logikal-3.2.1/django_logikal/templates/extensions.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/filters.py` & `django_logikal-3.2.1/django_logikal/templates/filters.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/functions.py` & `django_logikal-3.2.1/django_logikal/templates/functions.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/jinja.py` & `django_logikal-3.2.1/django_logikal/templates/jinja.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/templates/template.py` & `django_logikal-3.2.1/django_logikal/templates/template.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/urls.py` & `django_logikal-3.2.1/django_logikal/urls.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/validation.py` & `django_logikal-3.2.1/django_logikal/validation.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal/views.py` & `django_logikal-3.2.1/django_logikal/views.py`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/django_logikal.egg-info/PKG-INFO` & `django_logikal-3.2.1/django_logikal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 3.2.0
+Version: 3.2.1
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `django_logikal-3.2.0/django_logikal.egg-info/SOURCES.txt` & `django_logikal-3.2.1/django_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/pyproject.toml` & `django_logikal-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/requirements/build.txt.lock` & `django_logikal-3.2.1/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/requirements/dev.txt.lock` & `django_logikal-3.2.1/requirements/dev.txt.lock`

 * *Files identical despite different names*

### Comparing `django_logikal-3.2.0/requirements/docs.txt.lock` & `django_logikal-3.2.1/requirements/docs.txt.lock`

 * *Files identical despite different names*

