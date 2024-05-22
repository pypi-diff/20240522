# Comparing `tmp/django-logikal-3.1.0.tar.gz` & `tmp/django_logikal-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-logikal-3.1.0.tar", last modified: Sat Jan 27 14:10:33 2024, max compression
+gzip compressed data, was "django_logikal-3.2.0.tar", last modified: Wed May 22 10:14:52 2024, max compression
```

## Comparing `django-logikal-3.1.0.tar` & `django_logikal-3.2.0.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.361858 django-logikal-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-27 14:10:11.000000 django-logikal-3.1.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-27 14:10:11.000000 django-logikal-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-27 14:10:11.000000 django-logikal-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-01-27 14:10:33.361858 django-logikal-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-27 14:10:11.000000 django-logikal-3.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-27 14:10:11.000000 django-logikal-3.1.0/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/babel/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/babel/django.ini
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/babel/djangojs.ini
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/bibliography.py
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/email.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/local_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/management/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/management/commands/syncdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/management/commands/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.337859 django-logikal-3.1.0/django_logikal/settings/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/common/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/common/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/common/production.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/common/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.341858 django-logikal-3.1.0/django_logikal/settings/dynamic_site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/dynamic_site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/dynamic_site/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/dynamic_site/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/dynamic_site/production.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/dynamic_site/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.341858 django-logikal-3.1.0/django_logikal/settings/static_site/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/static_site/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/static_site/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/static_site/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/settings/static_site/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/sitemap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.329859 django-logikal-3.1.0/django_logikal/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.341858 django-logikal-3.1.0/django_logikal/static/django_logikal/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   617492 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   310884 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff
--rw-r--r--   0 runner    (1001) docker     (127)   181500 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   628640 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   325296 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   192916 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   614256 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   312952 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
--rw-r--r--   0 runner    (1001) docker     (127)   184076 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   630852 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   327188 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   195128 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   610876 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   306060 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
--rw-r--r--   0 runner    (1001) docker     (127)   180576 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   628352 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   323532 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)   191804 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    87008 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53528 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    94148 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    93904 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    58800 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86908 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    53252 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    40672 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/fonts.css
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static/django_logikal/validation_error.css
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/templates/debug_toolbar/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/debug_toolbar/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/templates/django_logikal/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/django_logikal/base.html.j
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal/templates/django_logikal/email/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/django_logikal/email/base.html.j
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/django_logikal/validation_error.html.j
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/processors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/templates/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-27 14:10:11.000000 django-logikal-3.1.0/django_logikal/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/django_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-27 14:10:33.000000 django-logikal-3.1.0/django_logikal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-01-27 14:10:11.000000 django-logikal-3.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 14:10:33.357859 django-logikal-3.1.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/extras/bibliography.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/extras/dynamic.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-01-27 14:10:11.000000 django-logikal-3.1.0/requirements/extras/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 14:10:33.361858 django-logikal-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 10:14:37.000000 django_logikal-3.2.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 10:14:37.000000 django_logikal-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 10:14:37.000000 django_logikal-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 10:14:52.178026 django_logikal-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 10:14:37.000000 django_logikal-3.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-22 10:14:37.000000 django_logikal-3.2.0/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.154025 django_logikal-3.2.0/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/babel/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/babel/django.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/babel/djangojs.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/bibliography.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/local_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/syncdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/management/commands/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/common/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/dynamic_site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/dynamic_site/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/settings/static_site/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/settings/static_site/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/sitemap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.150025 django_logikal-3.2.0/django_logikal/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.158026 django_logikal-3.2.0/django_logikal/static/django_logikal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   600856 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309728 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184912 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   622572 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323344 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   193308 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   639388 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   328412 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195704 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   617492 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   310884 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   181500 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   628640 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   325296 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   192916 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   607720 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   309192 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   182708 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   614256 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   312952 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   184076 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   630852 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   327188 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   195128 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   610876 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   306060 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   180576 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   628352 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   323532 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   191804 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    87008 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53528 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    40688 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    94148 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    59380 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44824 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    93904 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    58800 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    44544 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86908 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    53252 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    40672 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/fonts.css
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static/django_logikal/validation_error.css
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/debug_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/debug_toolbar/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.174026 django_logikal-3.2.0/django_logikal/templates/django_logikal/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/base.html.j
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/django_logikal/templates/django_logikal/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/email/base.html.j
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/django_logikal/validation_error.html.j
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/processors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/templates/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-22 10:14:37.000000 django_logikal-3.2.0/django_logikal/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/django_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:14:52.000000 django_logikal-3.2.0/django_logikal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-22 10:14:37.000000 django_logikal-3.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:14:52.178026 django_logikal-3.2.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/bibliography.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/dynamic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 10:14:37.000000 django_logikal-3.2.0/requirements/extras/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:14:52.178026 django_logikal-3.2.0/setup.cfg
```

### Comparing `django-logikal-3.1.0/.copier-answers.yml` & `django_logikal-3.2.0/.copier-answers.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is an answers file generated by Copier.
 ##
 ###################################################################################################
-_src_path: ../python-package-template/
+_commit: v1.0.4
+_src_path: git@github.com:logikal-io/python-package-template.git
 audience: Developers
 classifiers:
 - 'Framework :: Django'
 - 'Framework :: Django :: 4'
 - 'Topic :: Software Development'
 - 'Topic :: Utilities'
 cloud: true
@@ -22,8 +23,7 @@
 - django
 license: mit
 name: django-logikal
 scripts:
 - run
 - manage
 title: django-logikal
-
```

### Comparing `django-logikal-3.1.0/LICENSE.txt` & `django_logikal-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/PKG-INFO` & `django_logikal-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 3.1.0
+Version: 3.2.0
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -37,35 +37,35 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Django~=4.2
 Requires-Dist: django-stubs-ext~=4.2
-Requires-Dist: django-debug-toolbar~=4.2
+Requires-Dist: django-debug-toolbar~=4.3
 Requires-Dist: django-debug-toolbar-template-profiler~=2.1
 Requires-Dist: django-mail-panel~=4.0
-Requires-Dist: django-csp~=3.7
+Requires-Dist: django-csp~=3.8
 Requires-Dist: django-robots~=6.1
 Requires-Dist: psycopg~=3.1
-Requires-Dist: Babel~=2.14
-Requires-Dist: black~=24.1
+Requires-Dist: Babel~=2.15
+Requires-Dist: black~=24.4
 Requires-Dist: termcolor~=2.4
-Requires-Dist: google-cloud-logging~=3.9
+Requires-Dist: google-cloud-logging~=3.10
 Requires-Dist: Jinja2~=3.1
-Requires-Dist: logikal-utils[docker]~=1.0
-Requires-Dist: Pygments~=2.17
-Requires-Dist: types-Pygments~=2.17
+Requires-Dist: logikal-utils[docker]~=1.1
+Requires-Dist: Pygments~=2.18
+Requires-Dist: types-Pygments~=2.18
 Provides-Extra: static
 Requires-Dist: django-distill~=3.1; extra == "static"
 Provides-Extra: dynamic
 Requires-Dist: whitenoise[brotli]~=6.6; extra == "dynamic"
 Requires-Dist: stormware[amazon,google]~=1.2; extra == "dynamic"
 Requires-Dist: antimarkdown~=1.0; extra == "dynamic"
-Requires-Dist: django-anymail[amazon-ses]~=10.2; extra == "dynamic"
+Requires-Dist: django-anymail[amazon-ses]~=10.3; extra == "dynamic"
 Requires-Dist: premailer~=3.10; extra == "dynamic"
 Provides-Extra: bibliography
 Requires-Dist: pybtex==0.24.0; extra == "bibliography"
 
 django-logikal
 ==============
 Django utilities used at Logikal.
```

### Comparing `django-logikal-3.1.0/compose.yml` & `django_logikal-3.2.0/compose.yml`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/apps.py` & `django_logikal-3.2.0/django_logikal/apps.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/bibliography.py` & `django_logikal-3.2.0/django_logikal/bibliography.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/email.py` & `django_logikal-3.2.0/django_logikal/email.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/logging.py` & `django_logikal-3.2.0/django_logikal/logging.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/management/commands/generate.py` & `django_logikal-3.2.0/django_logikal/management/commands/generate.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/management/commands/syncdb.py` & `django_logikal-3.2.0/django_logikal/management/commands/syncdb.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/management/commands/translate.py` & `django_logikal-3.2.0/django_logikal/management/commands/translate.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/migrations.py` & `django_logikal-3.2.0/django_logikal/migrations.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/run.py` & `django_logikal-3.2.0/django_logikal/run.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/security.py` & `django_logikal-3.2.0/django_logikal/security.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/__init__.py` & `django_logikal-3.2.0/django_logikal/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/common/base.py` & `django_logikal-3.2.0/django_logikal/settings/common/base.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/common/dev.py` & `django_logikal-3.2.0/django_logikal/settings/common/dev.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from logikal_utils.docker import Service
 
 from django_logikal.env import get_option, option_is_set
 from django_logikal.logging import logging_config
 from django_logikal.settings import Settings, SettingsUpdate
 
 
@@ -17,19 +19,22 @@
     SECRET_KEY = 'dev'  # nosec: only used for development
 
     # Core settings
     DEBUG = option_is_set('dev_run')
     DATABASES = {
         'default': {
             'ENGINE': 'django.db.backends.postgresql',
-            'HOST': '127.0.0.1',
-            'PORT': Service('postgres').container_port('5432/tcp'),
-            'NAME': 'dev',
-            'USER': 'dev',
-            'PASSWORD': 'dev',
+            'HOST': os.getenv('DJANGO_DATABASE_HOST', '127.0.0.1'),
+            'PORT': os.getenv(
+                'DJANGO_DATABASE_PORT',
+                Service('postgres').container_port('5432/tcp'),
+            ),
+            'NAME': os.getenv('DJANGO_DATABASE_NAME', 'dev'),
+            'USER': os.getenv('DJANGO_DATABASE_USER', 'dev'),
+            'PASSWORD': os.getenv('DJANGO_DATABASE_USER', 'dev'),
         },
     }
 
     # Migration linter
     MIGRATION_LINTER_OPTIONS = {'exclude_apps': ['sites', 'robots']}
     MIGRATION_LINTER_OVERRIDE_MAKEMIGRATIONS = True
```

### Comparing `django-logikal-3.1.0/django_logikal/settings/common/production.py` & `django_logikal-3.2.0/django_logikal/settings/common/production.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/common/testing.py` & `django_logikal-3.2.0/django_logikal/settings/common/testing.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/dynamic_site/base.py` & `django_logikal-3.2.0/django_logikal/settings/dynamic_site/base.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/dynamic_site/dev.py` & `django_logikal-3.2.0/django_logikal/settings/dynamic_site/dev.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/dynamic_site/production.py` & `django_logikal-3.2.0/django_logikal/settings/dynamic_site/production.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/dynamic_site/testing.py` & `django_logikal-3.2.0/django_logikal/settings/dynamic_site/testing.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/settings/static_site/base.py` & `django_logikal-3.2.0/django_logikal/settings/static_site/base.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/sitemap.py` & `django_logikal-3.2.0/django_logikal/sitemap.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Light.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-LightItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-README.txt` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-README.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Semibold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-SemiboldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-Thin.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/Lato-ThinItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Italic.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts/RobotoMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/fonts.css` & `django_logikal-3.2.0/django_logikal/static/django_logikal/fonts.css`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static/django_logikal/validation_error.css` & `django_logikal-3.2.0/django_logikal/static/django_logikal/validation_error.css`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/static.py` & `django_logikal-3.2.0/django_logikal/static.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/django_logikal/base.html.j` & `django_logikal-3.2.0/django_logikal/templates/django_logikal/base.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/django_logikal/validation_error.html.j` & `django_logikal-3.2.0/django_logikal/templates/django_logikal/validation_error.html.j`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/extensions.py` & `django_logikal-3.2.0/django_logikal/templates/extensions.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/filters.py` & `django_logikal-3.2.0/django_logikal/templates/filters.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/functions.py` & `django_logikal-3.2.0/django_logikal/templates/functions.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/jinja.py` & `django_logikal-3.2.0/django_logikal/templates/jinja.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/templates/template.py` & `django_logikal-3.2.0/django_logikal/templates/template.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/urls.py` & `django_logikal-3.2.0/django_logikal/urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     for url in urls:
         for url_item in getattr(url, 'url_patterns', [url]):
             url_item.callback = public(url_item.callback)
     return include((urls, debug_toolbar.APP_NAME))
 
 
 def utility_paths(
-    sitemaps: Optional[Mapping[str, Union[Sitemap[Any], Type[Sitemap[Any]]]]],
+    sitemaps: Optional[Mapping[str, Union[Sitemap[Any], Type[Sitemap[Any]]]]] = None,
     static: bool = False,
 ) -> List[URLType]:
     """
     Return the common utility paths.
 
     Includes the admin paths, sitemap and robots paths and the Django debug toolbar paths (when
     appropriate). Also includes the standard error paths when running locally.
```

### Comparing `django-logikal-3.1.0/django_logikal/validation.py` & `django_logikal-3.2.0/django_logikal/validation.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal/views.py` & `django_logikal-3.2.0/django_logikal/views.py`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/django_logikal.egg-info/PKG-INFO` & `django_logikal-3.2.0/django_logikal.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-logikal
-Version: 3.1.0
+Version: 3.2.0
 Summary: Django utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -37,35 +37,35 @@
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: Django~=4.2
 Requires-Dist: django-stubs-ext~=4.2
-Requires-Dist: django-debug-toolbar~=4.2
+Requires-Dist: django-debug-toolbar~=4.3
 Requires-Dist: django-debug-toolbar-template-profiler~=2.1
 Requires-Dist: django-mail-panel~=4.0
-Requires-Dist: django-csp~=3.7
+Requires-Dist: django-csp~=3.8
 Requires-Dist: django-robots~=6.1
 Requires-Dist: psycopg~=3.1
-Requires-Dist: Babel~=2.14
-Requires-Dist: black~=24.1
+Requires-Dist: Babel~=2.15
+Requires-Dist: black~=24.4
 Requires-Dist: termcolor~=2.4
-Requires-Dist: google-cloud-logging~=3.9
+Requires-Dist: google-cloud-logging~=3.10
 Requires-Dist: Jinja2~=3.1
-Requires-Dist: logikal-utils[docker]~=1.0
-Requires-Dist: Pygments~=2.17
-Requires-Dist: types-Pygments~=2.17
+Requires-Dist: logikal-utils[docker]~=1.1
+Requires-Dist: Pygments~=2.18
+Requires-Dist: types-Pygments~=2.18
 Provides-Extra: static
 Requires-Dist: django-distill~=3.1; extra == "static"
 Provides-Extra: dynamic
 Requires-Dist: whitenoise[brotli]~=6.6; extra == "dynamic"
 Requires-Dist: stormware[amazon,google]~=1.2; extra == "dynamic"
 Requires-Dist: antimarkdown~=1.0; extra == "dynamic"
-Requires-Dist: django-anymail[amazon-ses]~=10.2; extra == "dynamic"
+Requires-Dist: django-anymail[amazon-ses]~=10.3; extra == "dynamic"
 Requires-Dist: premailer~=3.10; extra == "dynamic"
 Provides-Extra: bibliography
 Requires-Dist: pybtex==0.24.0; extra == "bibliography"
 
 django-logikal
 ==============
 Django utilities used at Logikal.
```

### Comparing `django-logikal-3.1.0/django_logikal.egg-info/SOURCES.txt` & `django_logikal-3.2.0/django_logikal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-logikal-3.1.0/pyproject.toml` & `django_logikal-3.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -81,14 +81,17 @@
 [tool.django_logikal]
 DJANGO_SETTINGS_MODULE = 'tests.dynamic_site.settings.dev'
 
 [tool.django_logikal.translate]
 apps = ['dynamic_site']
 contact = 'Gergely Kalmár <contact@logikal.io>'
 
+[tool.browser.versions]
+chrome = '124.0.6367.207'
+
 [tool.mypy]
 plugins = ['mypy_django_plugin.main']
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
   'antimarkdown.*',
```

### Comparing `django-logikal-3.1.0/requirements/build.txt.lock` & `django_logikal-3.2.0/requirements/build.txt.lock`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 5cb1a368e35962412e4230ef67a622b3ed950d02d59c40d132b27e3a685ef8f8
+##  Requirements hash: 8706de2163a25299dbe1d5d6f26df03b6aaaad435e67227452ee6c0b2b97aea0
 ##
 ###################################################################################################
-build==1.0.3
-certifi==2023.7.22
+backports.tarfile==1.1.1
+build==1.2.1
+certifi==2024.2.2
 cffi==1.16.0
-charset-normalizer==3.3.0
-cryptography==41.0.4
+charset-normalizer==3.3.2
+cryptography==42.0.7
 docutils==0.20.1
-idna==3.4
-importlib-metadata==6.8.0
-importlib-resources==6.1.0
-jaraco.classes==3.3.0
+idna==3.7
+importlib_metadata==7.1.0
+importlib_resources==6.4.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-keyring==24.2.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
-more-itertools==10.1.0
-nh3==0.2.14
-packaging==23.2
-pip==23.2.1
-pkginfo==1.9.6
-pycparser==2.21
-Pygments==2.16.1
-pyproject_hooks==1.0.0
-readme-renderer==42.0
-requests==2.31.0
+more-itertools==10.2.0
+nh3==0.2.17
+packaging==24.0
+pip==24.0
+pkginfo==1.10.0
+pycparser==2.22
+Pygments==2.18.0
+pyproject_hooks==1.1.0
+readme_renderer==43.0
+requests==2.32.2
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.6.0
+rich==13.7.1
 SecretStorage==3.3.3
-setuptools==68.2.2
+setuptools==70.0.0
 tomli==2.0.1
-twine==4.0.2
-typing_extensions==4.8.0
-urllib3==2.0.6
-wheel==0.41.2
-zipp==3.17.0
+twine==5.1.0
+typing_extensions==4.11.0
+urllib3==2.2.1
+wheel==0.43.0
+zipp==3.18.2
```

### Comparing `django-logikal-3.1.0/requirements/dev.txt.lock` & `django_logikal-3.2.0/requirements/dev.txt.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,216 +1,220 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 00d39e412677a1e6ccf71ca5ae527a0e02cfbf2f1d2f830355f7930f6d97d729
+##  Requirements hash: 2d84e85edd8d0ecc6628982d9b9a4864d4bd8f7215044d5789af433611f6b585
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 antimarkdown==1.0.2
 appdirs==1.4.4
-asgiref==3.7.2
-astroid==3.0.2
+asgiref==3.8.1
+astroid==3.2.2
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
+backports.tarfile==1.1.1
 backports.zoneinfo==0.2.1
-bandit==1.7.7
-black==24.1.0
+bandit==1.7.8
+black==24.4.2
 boto3==1.34.29
 boto3-stubs==1.34.29
-botocore==1.34.29
-botocore-stubs==1.34.29
-Bottleneck==1.3.7
+botocore==1.34.110
+botocore-stubs==1.34.94
+Bottleneck==1.3.8
 Brotli==1.1.0
-build==1.0.3
-cachetools==5.3.2
-certifi==2023.11.17
+build==1.2.1
+cachetools==5.3.3
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.1
-cryptography==42.0.1
-cssbeautifier==1.14.11
+coverage==7.5.1
+cryptography==42.0.7
+cssbeautifier==1.15.1
 cssselect==1.2.0
-cssutils==2.9.0
+cssutils==2.11.0
 db-dtypes==1.2.0
-dill==0.3.7
-Django==4.2.9
-django-anymail==10.2
-django-csp==3.7
-django-debug-toolbar==4.2.0
+dill==0.3.8
+Django==4.2.13
+django-anymail==10.3
+django-debug-toolbar==4.3.0
 django-debug-toolbar-template-profiler==2.1.0
 django-distill==3.1.3
-django-mail-panel==4.0.3
-django-migration-linter==5.0.0
+django-mail-panel==4.0.4
+django-migration-linter==5.1.0
 django-robots==6.1
 django-stubs==4.2.7
 django-stubs-ext==4.2.7
+django_csp==3.8
 djlint==1.34.1
 docker==7.0.0
 docutils==0.20.1
-EditorConfig==0.12.3
-exceptiongroup==1.2.0
-execnet==2.0.2
+EditorConfig==0.12.4
+exceptiongroup==1.2.1
+execnet==2.1.1
 factory-boy==3.3.0
-Faker==22.5.1
-filelock==3.13.1
-flaky==3.7.0
-freezegun==1.4.0
-google-api-core==2.15.0
+Faker==25.2.0
+filelock==3.14.0
+flaky==3.8.1
+freezegun==1.5.1
+google-api-core==2.19.0
 google-api-python-client==2.115.0
 google-api-python-client-stubs==1.23.0
 google-auth==2.27.0
 google-auth-httplib2==0.2.0
 google-auth-stubs==0.2.0
-google-cloud-appengine-logging==1.4.0
+google-cloud-appengine-logging==1.4.3
 google-cloud-audit-log==0.2.5
-google-cloud-bigquery==3.17.1
+google-cloud-bigquery==3.23.1
 google-cloud-core==2.4.1
-google-cloud-logging==3.9.0
+google-cloud-logging==3.10.0
 google-cloud-secret-manager==2.17.0
 google-crc32c==1.5.0
 google-resumable-media==2.7.0
-googleapis-common-protos==1.62.0
+googleapis-common-protos==1.63.0
 grpc-google-iam-v1==0.13.0
 grpc-stubs==1.53.0.5
-grpcio==1.60.0
-grpcio-status==1.60.0
+grpcio==1.64.0
+grpcio-status==1.62.2
 h11==0.14.0
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 httplib2==0.22.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
-importlib-resources==6.1.1
+importlib_metadata==7.1.0
+importlib_resources==6.4.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.13.2
-jaraco.classes==3.3.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-Jinja2==3.1.3
+Jinja2==3.1.4
 jmespath==1.0.1
-jsbeautifier==1.14.11
-json5==0.9.14
-keyring==24.3.0
-latexcodec==2.0.1
+jsbeautifier==1.15.1
+json5==0.9.25
+keyring==25.2.1
+latexcodec==3.0.0
 llvmlite==0.41.1
 logikal-docs==1.1.4
-logikal-utils==1.0.1
-lxml==5.1.0
+logikal-utils==1.1.0
+lxml==5.2.2
 markdown-it-py==3.0.0
-MarkupSafe==2.1.4
+MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-mypy==1.8.0
+mypy==1.10.0
 mypy-extensions==1.0.0
-nh3==0.2.15
+nh3==0.2.17
 numba==0.58.1
 numexpr==2.8.6
 numpy==1.24.4
 outcome==1.3.0.post0
 packaging==23.2
 pandas==2.0.3
 pandas-stubs==2.0.3.230814
 pathspec==0.12.1
 pbr==6.0.0
-pillow==10.2.0
-pip==23.3.2
-pip-licenses==4.3.4
-pkginfo==1.9.6
-platformdirs==4.1.0
-pluggy==1.3.0
+pillow==10.3.0
+pip==24.0
+pip-licenses==4.4.0
+pkginfo==1.10.0
+platformdirs==4.2.2
+pluggy==1.5.0
 premailer==3.10.0
-prettytable==3.9.0
+prettytable==3.10.0
 proto-plus==1.23.0
-protobuf==4.25.2
+protobuf==4.25.3
 psutil==5.9.8
-psycopg==3.1.17
-pyarrow==15.0.0
-pyasn1==0.5.1
-pyasn1-modules==0.3.0
+psycopg==3.1.19
+pyarrow==16.1.0
+pyasn1==0.6.0
+pyasn1_modules==0.4.0
 pybtex==0.24.0
 pycodestyle==2.11.1
-pycparser==2.21
+pycparser==2.22
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.0.3
+Pygments==2.18.0
+pylint==3.2.2
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
-pyparsing==3.1.1
-pyproject_hooks==1.0.0
+pyparsing==3.1.2
+pyproject_hooks==1.1.0
 PySocks==1.7.1
-pytest==7.4.4
-pytest-cov==4.1.0
-pytest-django==4.7.0
-pytest-factoryboy==2.6.0
-pytest-logikal==2.0.2
-pytest-mock==3.12.0
+pytest==8.2.1
+pytest-cov==5.0.0
+pytest-django==4.8.0
+pytest-factoryboy==2.7.0
+pytest-logikal==3.1.0
+pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
+pytest-xdist==3.6.1
 pytest_freezer==0.4.8
-python-dateutil==2.8.2
-pytz==2023.3.post1
+python-dateutil==2.9.0.post0
+pytz==2024.1
 PyYAML==6.0.1
-readme-renderer==42.0
+readme_renderer==43.0
 regex==2023.12.25
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
+rich==13.7.1
 rsa==4.9
-s3transfer==0.10.0
+s3transfer==0.10.1
 SecretStorage==3.3.3
-selenium==4.17.2
-setuptools==69.0.3
+selenium==4.21.0
+setuptools==70.0.0
 six==1.16.0
-sniffio==1.3.0
+sniffio==1.3.1
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.4
-stevedore==5.1.0
+sqlparse==0.5.0
+stevedore==5.2.0
 stormware==1.2.1
 termcolor==2.4.0
 toml==0.10.2
 tomli==2.0.1
-tomlkit==0.12.3
-tqdm==4.66.1
-trio==0.24.0
+tomlkit==0.12.5
+tqdm==4.66.4
+trio==0.25.1
 trio-websocket==0.11.1
-twine==4.0.2
-types-awscrt==0.20.3
-types-docutils==0.20.0.20240126
-types-httplib2==0.22.0.2
-types-psutil==5.9.5.20240106
-types-Pygments==2.17.0.20240106
-types-pytz==2023.3.1.1
-types-PyYAML==6.0.12.12
+twine==5.1.0
+types-awscrt==0.20.9
+types-docutils==0.21.0.20240423
+types-httplib2==0.22.0.20240310
+types-psutil==5.9.5.20240516
+types-Pygments==2.18.0.20240506
+types-pytz==2024.1.0.20240417
+types-PyYAML==6.0.12.20240311
 types-requests==2.31.0.6
-types-s3transfer==0.10.0
-types-setuptools==69.0.0.20240125
+types-s3transfer==0.10.1
+types-setuptools==69.5.0.20240522
+types-tqdm==4.66.0.20240417
 types-urllib3==1.26.25.14
-typing_extensions==4.9.0
-tzdata==2023.4
+typing_extensions==4.11.0
+tzdata==2024.1
 uritemplate==4.1.1
 urllib3==1.26.18
 wcwidth==0.2.13
-wheel==0.42.0
+wheel==0.43.0
 whitenoise==6.6.0
 wrapt==1.16.0
 wsproto==1.2.0
 xdg==5.1.1
-zipp==3.17.0
+zipp==3.18.2
```

### Comparing `django-logikal-3.1.0/requirements/docs.txt.lock` & `django_logikal-3.2.0/requirements/docs.txt.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,189 +1,186 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 737089a8fc24faeeaf29d61dd6808a6a47dbc701d58f77c007d2c2abd1bdabdc
+##  Requirements hash: d5d78316d3c50511405d486dcf0b51722a543889459da628d86421d9dc3c6fd9
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 antimarkdown==1.0.2
 appdirs==1.4.4
-asgiref==3.7.2
-astroid==3.0.2
+asgiref==3.8.1
+astroid==3.2.2
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
 backports.zoneinfo==0.2.1
-bandit==1.7.7
-black==24.1.0
+bandit==1.7.8
+black==24.4.2
 boto3==1.34.29
 boto3-stubs==1.34.29
-botocore==1.34.29
-botocore-stubs==1.34.29
-Bottleneck==1.3.7
+botocore==1.34.110
+botocore-stubs==1.34.94
+Bottleneck==1.3.8
 Brotli==1.1.0
-cachetools==5.3.2
-certifi==2023.11.17
-cffi==1.16.0
+cachetools==5.3.3
+certifi==2024.2.2
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
-coverage==7.4.1
-cryptography==42.0.1
-cssbeautifier==1.14.11
+coverage==7.5.1
+cssbeautifier==1.15.1
 cssselect==1.2.0
-cssutils==2.9.0
+cssutils==2.11.0
 db-dtypes==1.2.0
-dill==0.3.7
-Django==4.2.9
-django-anymail==10.2
-django-csp==3.7
-django-debug-toolbar==4.2.0
+dill==0.3.8
+Django==4.2.13
+django-anymail==10.3
+django-debug-toolbar==4.3.0
 django-debug-toolbar-template-profiler==2.1.0
 django-distill==3.1.3
-django-mail-panel==4.0.3
-django-migration-linter==5.0.0
+django-mail-panel==4.0.4
+django-migration-linter==5.1.0
 django-robots==6.1
 django-stubs==4.2.7
 django-stubs-ext==4.2.7
+django_csp==3.8
 djlint==1.34.1
 docker==7.0.0
 docutils==0.20.1
-EditorConfig==0.12.3
-exceptiongroup==1.2.0
-execnet==2.0.2
+EditorConfig==0.12.4
+exceptiongroup==1.2.1
+execnet==2.1.1
 factory-boy==3.3.0
-Faker==22.5.1
-filelock==3.13.1
-google-api-core==2.15.0
+Faker==25.2.0
+filelock==3.14.0
+google-api-core==2.19.0
 google-api-python-client==2.115.0
 google-api-python-client-stubs==1.23.0
 google-auth==2.27.0
 google-auth-httplib2==0.2.0
 google-auth-stubs==0.2.0
-google-cloud-appengine-logging==1.4.0
+google-cloud-appengine-logging==1.4.3
 google-cloud-audit-log==0.2.5
-google-cloud-bigquery==3.17.1
+google-cloud-bigquery==3.23.1
 google-cloud-core==2.4.1
-google-cloud-logging==3.9.0
+google-cloud-logging==3.10.0
 google-cloud-secret-manager==2.17.0
 google-crc32c==1.5.0
 google-resumable-media==2.7.0
-googleapis-common-protos==1.62.0
+googleapis-common-protos==1.63.0
 grpc-google-iam-v1==0.13.0
 grpc-stubs==1.53.0.5
-grpcio==1.60.0
-grpcio-status==1.60.0
+grpcio==1.64.0
+grpcio-status==1.62.2
 html-tag-names==0.1.2
 html-void-elements==0.1.0
 httplib2==0.22.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
+importlib_metadata==7.1.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.13.2
-Jinja2==3.1.3
+Jinja2==3.1.4
 jmespath==1.0.1
-jsbeautifier==1.14.11
-json5==0.9.14
-latexcodec==2.0.1
+jsbeautifier==1.15.1
+json5==0.9.25
+latexcodec==3.0.0
 llvmlite==0.41.1
 logikal-docs==1.1.4
-logikal-utils==1.0.1
-lxml==5.1.0
+logikal-utils==1.1.0
+lxml==5.2.2
 markdown-it-py==3.0.0
-MarkupSafe==2.1.4
+MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
-mypy==1.8.0
+mypy==1.10.0
 mypy-extensions==1.0.0
 numba==0.58.1
 numexpr==2.8.6
 numpy==1.24.4
 packaging==23.2
 pandas==2.0.3
 pandas-stubs==2.0.3.230814
 pathspec==0.12.1
 pbr==6.0.0
-pillow==10.2.0
-pip==23.3.2
-pip-licenses==4.3.4
-platformdirs==4.1.0
-pluggy==1.3.0
+pillow==10.3.0
+pip==24.0
+pip-licenses==4.4.0
+platformdirs==4.2.2
+pluggy==1.5.0
 premailer==3.10.0
-prettytable==3.9.0
+prettytable==3.10.0
 proto-plus==1.23.0
-protobuf==4.25.2
+protobuf==4.25.3
 psutil==5.9.8
-psycopg==3.1.17
-pyarrow==15.0.0
-pyasn1==0.5.1
-pyasn1-modules==0.3.0
+psycopg==3.1.19
+pyarrow==16.1.0
+pyasn1==0.6.0
+pyasn1_modules==0.4.0
 pybtex==0.24.0
 pycodestyle==2.11.1
-pycparser==2.21
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.0.3
+Pygments==2.18.0
+pylint==3.2.2
 pylint-django==2.5.5
 pylint-plugin-utils==0.8.2
 pyorbs==2.1.0
-pyparsing==3.1.1
-pytest==7.4.4
-pytest-cov==4.1.0
-pytest-django==4.7.0
-pytest-factoryboy==2.6.0
-pytest-logikal==2.0.2
-pytest-mock==3.12.0
+pyparsing==3.1.2
+pytest==8.2.1
+pytest-cov==5.0.0
+pytest-django==4.8.0
+pytest-factoryboy==2.7.0
+pytest-logikal==3.1.0
+pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
-python-dateutil==2.8.2
-pytz==2023.3.post1
+pytest-xdist==3.6.1
+python-dateutil==2.9.0.post0
+pytz==2024.1
 PyYAML==6.0.1
 regex==2023.12.25
 requests==2.31.0
-rich==13.7.0
+rich==13.7.1
 rsa==4.9
-s3transfer==0.10.0
-setuptools==69.0.3
+s3transfer==0.10.1
+setuptools==70.0.0
 six==1.16.0
 snowballstemmer==2.2.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.4
-stevedore==5.1.0
+sqlparse==0.5.0
+stevedore==5.2.0
 stormware==1.2.1
 termcolor==2.4.0
 toml==0.10.2
 tomli==2.0.1
-tomlkit==0.12.3
-tqdm==4.66.1
-types-awscrt==0.20.3
-types-docutils==0.20.0.20240126
-types-httplib2==0.22.0.2
-types-Pygments==2.17.0.20240106
-types-pytz==2023.3.1.1
-types-PyYAML==6.0.12.12
+tomlkit==0.12.5
+tqdm==4.66.4
+types-awscrt==0.20.9
+types-docutils==0.21.0.20240423
+types-httplib2==0.22.0.20240310
+types-Pygments==2.18.0.20240506
+types-pytz==2024.1.0.20240417
+types-PyYAML==6.0.12.20240311
 types-requests==2.31.0.6
-types-s3transfer==0.10.0
-types-setuptools==69.0.0.20240125
+types-s3transfer==0.10.1
+types-setuptools==69.5.0.20240522
 types-urllib3==1.26.25.14
-typing_extensions==4.9.0
-tzdata==2023.4
+typing_extensions==4.11.0
+tzdata==2024.1
 uritemplate==4.1.1
 urllib3==1.26.18
 wcwidth==0.2.13
-wheel==0.42.0
+wheel==0.43.0
 whitenoise==6.6.0
 wrapt==1.16.0
 xdg==5.1.1
-zipp==3.17.0
+zipp==3.18.2
```

