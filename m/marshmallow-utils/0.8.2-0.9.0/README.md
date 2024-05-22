# Comparing `tmp/marshmallow-utils-0.8.2.tar.gz` & `tmp/marshmallow-utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marshmallow-utils-0.8.2.tar", last modified: Mon Dec 11 13:40:33 2023, max compression
+gzip compressed data, was "dist/marshmallow-utils-0.9.0.tar", last modified: Wed May 22 16:33:52 2024, max compression
```

## Comparing `marshmallow-utils-0.8.2.tar` & `marshmallow-utils-0.9.0.tar`

### file list

```diff
@@ -1,232 +1,237 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      417 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.github/workflows/i18n-pull.yml
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.github/workflows/i18n-push.yml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7453 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      254 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/babel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/edtfdatestring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/generated.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/isodate.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/isolanguage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/nestedattr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/sanitizedhtml.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/sanitizedunicode.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/strippedhtml.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/trimmed.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/tzdatetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/fields/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/schemas/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/schemas/identifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/af/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/af/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/af/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ar/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/bg/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ca/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/da/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/da/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/da/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/de_DE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/el/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      821 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_AT/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_AT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_AT/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/en_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_CU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_CU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      875 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_CU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_MX/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_MX/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/es_MX/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et_EE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et_EE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/et_EE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fa_IR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      873 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_CI/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_CI/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_CI/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_FR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_FR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_FR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/gl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/gl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/gl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hi_IN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hi_IN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hi_IN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu_HU/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu_HU/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/hu_HU/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      862 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ka/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ka/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/lt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/lt/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ne/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ne/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ne/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/no/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/no/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/no/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/rw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/rw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/rw/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv_SE/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv_SE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/sv_SE/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk_UA/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk_UA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/uk_UA/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      963 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_CN/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_TW/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      393 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-11 13:40:32.000000 marshmallow-utils-0.8.2/marshmallow_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      559 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/fields/test_identifier_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/fields/test_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-11 13:40:33.000000 marshmallow-utils-0.8.2/tests/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_identifier_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_multipoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/schemas/test_schema_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_babel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_contrib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_edtfdatestring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_isolanguage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_marshmallow_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-11 13:40:25.000000 marshmallow-utils-0.8.2/tests/test_nestedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.github/workflows/i18n-pull.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.github/workflows/i18n-push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/.tx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7453 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/babel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/edtfdatestring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/isodate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/isolanguage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/nestedattr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/sanitizedhtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/sanitizedunicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/strippedhtml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/trimmed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/tzdatetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/fields/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/schemas/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/schemas/identifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/af/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/af/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/af/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ar/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/bg/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ca/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/da/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/da/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/da/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/de_DE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/el/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_AT/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_AT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_AT/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/en_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_CU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_CU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_CU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_MX/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_MX/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/es_MX/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et_EE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et_EE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/et_EE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fa_IR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_CI/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_CI/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_CI/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_FR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_FR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/gl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/gl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/gl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hi_IN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hi_IN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hi_IN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu_HU/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/hu_HU/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ka/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ka/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/lt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/lt/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ne/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ne/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ne/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/no/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/no/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/no/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/rw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/rw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/rw/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv_SE/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv_SE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/sv_SE/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk_UA/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk_UA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/uk_UA/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_CN/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_TW/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/marshmallow_utils/validators/oneof.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5012 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 16:33:51.000000 marshmallow-utils-0.9.0/marshmallow_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      559 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/fields/test_identifier_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/fields/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_identifier_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/schemas/test_schema_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_babel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_contrib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_edtfdatestring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_isolanguage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_marshmallow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/test_nestedattr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:33:52.000000 marshmallow-utils-0.9.0/tests/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-22 16:33:47.000000 marshmallow-utils-0.9.0/tests/validators/test_lazyoneof.py
```

### Comparing `marshmallow-utils-0.8.2/.editorconfig` & `marshmallow-utils-0.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/.github/workflows/pypi-publish.yml` & `marshmallow-utils-0.9.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/.tx/config` & `marshmallow-utils-0.9.0/.tx/config`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/CHANGES.rst` & `marshmallow-utils-0.9.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 ..
-    Copyright (C) 2020-2021 CERN.
+    Copyright (C) 2020-2024 CERN.
     Copyright (C) 2020-2021 Northwestern University.
 
     Marshmallow-Utils is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version 0.9.0 (released 2024-05-22)
+
+- validators: implement LazyOneOf
+
 Version 0.8.2 (released 2023-12-11)
 
 - html: remove "class" from allowed html attributes
 
 Version 0.8.1 (released 2023-11-29)
 
 - html: allow table tags
```

### Comparing `marshmallow-utils-0.8.2/CONTRIBUTING.rst` & `marshmallow-utils-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/LICENSE` & `marshmallow-utils-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/MANIFEST.in` & `marshmallow-utils-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/PKG-INFO` & `marshmallow-utils-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow-utils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Extras and utilities for Marshmallow.
 Home-page: https://github.com/inveniosoftware/marshmallow-utils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -34,24 +34,28 @@
         
         Extras and utilities for Marshmallow
         
         Further documentation is available on
         https://marshmallow-utils.readthedocs.io/
         
         ..
-            Copyright (C) 2020-2021 CERN.
+            Copyright (C) 2020-2024 CERN.
             Copyright (C) 2020-2021 Northwestern University.
         
             Marshmallow-Utils is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 0.9.0 (released 2024-05-22)
+        
+        - validators: implement LazyOneOf
+        
         Version 0.8.2 (released 2023-12-11)
         
         - html: remove "class" from allowed html attributes
         
         Version 0.8.1 (released 2023-11-29)
         
         - html: allow table tags
```

### Comparing `marshmallow-utils-0.8.2/README.rst` & `marshmallow-utils-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/docs/Makefile` & `marshmallow-utils-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/docs/conf.py` & `marshmallow-utils-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/docs/index.rst` & `marshmallow-utils-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/docs/make.bat` & `marshmallow-utils-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/__init__.py` & `marshmallow-utils-0.9.0/marshmallow_utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2020-2022 CERN.
+# Copyright (C) 2020-2024 CERN.
 #
 # Marshmallow-Utils is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 r"""Extras and utilities for Marshmallow.
 
 Currently, this library contains a couple of extra fields that helps with
@@ -39,10 +39,10 @@
   `ftfy <https://pypi.org/project/ftfy/>`_ for fixing broken unicode text.
 - :py:class:`~fields.SanitizedHTML`: Integrates the
   `bleach <https://pypi.org/project/bleach/>`_ for HTML sanitization.
 - :py:class:`~fields.ISODateString`: Integrates the
   `arrow <https://pypi.org/project/arrow/>`_ for date parsing.
 """
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 __all__ = ("__version__",)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-# -*- coding: utf-8 -*- # # Copyright (C) 2020-2022 CERN. # # Marshmallow-Utils
+# -*- coding: utf-8 -*- # # Copyright (C) 2020-2024 CERN. # # Marshmallow-Utils
 is free software; you can redistribute it and/or modify # it under the terms of
 the MIT License; see LICENSE file for more details. r"""Extras and utilities
 for Marshmallow. Currently, this library contains a couple of extra fields that
 helps with sanitizing data as shown in the following example: >>> from
 marshmallow_utils import fields >>> from marshmallow import Schema >>> class
 MySchema(Schema): ... trim = fields.TrimmedString() ... html =
 fields.SanitizedHTML() ... text = fields.SanitizedUnicode() ... isodate =
@@ -12,9 +12,9 @@
 10-27', ... }) >>> data['trim'] 'whitespace' >>> data['html'] 'evil()' >>> data
 ['text'] 'PDF copy/paste' >>> data['isodate'] '1999-10-27' Fields: - :py:class:
 `~fields.SanitizedUnicode`: Integrates the `ftfy
 pypi.org/project/ftfy/>`_ for fixing broken unicode text. - :py:class:
 `~fields.SanitizedHTML`: Integrates the `bleach
 pypi.org/project/bleach/>`_ for HTML sanitization. - :py:class:
 `~fields.ISODateString`: Integrates the `arrow
-pypi.org/project/arrow/>`_ for date parsing. """ __version__ = "0.8.2" __all__
+pypi.org/project/arrow/>`_ for date parsing. """ __version__ = "0.9.0" __all__
 = ("__version__",)
```

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/__init__.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/babel.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/babel.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/contrib.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/contrib.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/edtfdatestring.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/edtfdatestring.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/generated.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/generated.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/identifier.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/identifier.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/isodate.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/isodate.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/isolanguage.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/isolanguage.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/links.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/links.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/nestedattr.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/nestedattr.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/sanitizedhtml.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/sanitizedhtml.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/sanitizedunicode.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/sanitizedunicode.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/strippedhtml.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/strippedhtml.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/trimmed.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/trimmed.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/tzdatetime.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/tzdatetime.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/fields/url.py` & `marshmallow-utils-0.9.0/marshmallow_utils/fields/url.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/html.py` & `marshmallow-utils-0.9.0/marshmallow_utils/html.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/links.py` & `marshmallow-utils-0.9.0/marshmallow_utils/links.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/permissions.py` & `marshmallow-utils-0.9.0/marshmallow_utils/permissions.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/schemas/geojson.py` & `marshmallow-utils-0.9.0/marshmallow_utils/schemas/geojson.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/schemas/identifier.py` & `marshmallow-utils-0.9.0/marshmallow_utils/schemas/identifier.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/af/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/af/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ar/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ar/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/bg/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/bg/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ca/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ca/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/cs/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/da/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/da/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/de/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/de_AT/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/de_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/de_DE/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/de_DE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/el/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/en_AT/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/en_AT/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/en_HU/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/en_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/es/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/es_CU/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/es_CU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/es_MX/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/es_MX/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/et/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/et/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/et_EE/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/et_EE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/fa/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/fa/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/fa_IR/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/fa_IR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/fr/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_CI/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_CI/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/fr_FR/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/fr_FR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/gl/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/gl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/hi_IN/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/hi_IN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/hr/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/hr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/hu/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/hu/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/hu_HU/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/hu_HU/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/it/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ja/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ja/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ka/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ka/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/lt/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/lt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/messages.pot` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ne/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ne/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/no/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/no/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/pl/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/pt/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ro/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/ru/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/rw/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/rw/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/sk/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/sk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/sv/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/sv/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/sv_SE/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/sv_SE/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/tr/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/uk/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/uk/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/uk_UA/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/uk_UA/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_CN/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_CN/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils/translations/zh_TW/LC_MESSAGES/messages.po` & `marshmallow-utils-0.9.0/marshmallow_utils/translations/zh_TW/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils.egg-info/PKG-INFO` & `marshmallow-utils-0.9.0/marshmallow_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marshmallow-utils
-Version: 0.8.2
+Version: 0.9.0
 Summary: Extras and utilities for Marshmallow.
 Home-page: https://github.com/inveniosoftware/marshmallow-utils
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2020 CERN.
@@ -34,24 +34,28 @@
         
         Extras and utilities for Marshmallow
         
         Further documentation is available on
         https://marshmallow-utils.readthedocs.io/
         
         ..
-            Copyright (C) 2020-2021 CERN.
+            Copyright (C) 2020-2024 CERN.
             Copyright (C) 2020-2021 Northwestern University.
         
             Marshmallow-Utils is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version 0.9.0 (released 2024-05-22)
+        
+        - validators: implement LazyOneOf
+        
         Version 0.8.2 (released 2023-12-11)
         
         - html: remove "class" from allowed html attributes
         
         Version 0.8.1 (released 2023-11-29)
         
         - html: allow table tags
```

### Comparing `marshmallow-utils-0.8.2/marshmallow_utils.egg-info/SOURCES.txt` & `marshmallow-utils-0.9.0/marshmallow_utils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 marshmallow_utils/translations/sv/LC_MESSAGES/messages.po
 marshmallow_utils/translations/sv_SE/LC_MESSAGES/messages.po
 marshmallow_utils/translations/tr/LC_MESSAGES/messages.po
 marshmallow_utils/translations/uk/LC_MESSAGES/messages.po
 marshmallow_utils/translations/uk_UA/LC_MESSAGES/messages.po
 marshmallow_utils/translations/zh_CN/LC_MESSAGES/messages.po
 marshmallow_utils/translations/zh_TW/LC_MESSAGES/messages.po
+marshmallow_utils/validators/__init__.py
+marshmallow_utils/validators/oneof.py
 tests/conftest.py
 tests/test_babel.py
 tests/test_contrib.py
 tests/test_edtfdatestring.py
 tests/test_fields.py
 tests/test_isolanguage.py
 tests/test_links.py
@@ -119,8 +121,9 @@
 tests/fields/test_identifier_field.py
 tests/fields/test_url.py
 tests/schemas/test_geojson.py
 tests/schemas/test_identifier_schema.py
 tests/schemas/test_multipoint.py
 tests/schemas/test_point.py
 tests/schemas/test_polygon.py
-tests/schemas/test_schema_permissions.py
+tests/schemas/test_schema_permissions.py
+tests/validators/test_lazyoneof.py
```

### Comparing `marshmallow-utils-0.8.2/run-tests.sh` & `marshmallow-utils-0.9.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/setup.cfg` & `marshmallow-utils-0.9.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	marshmallow-oneofschema>=2.1.0
 	pycountry>=18.12.8
 	uritemplate>=3.0.1
 	werkzeug>=1.0.0
 
 [options.extras_require]
 tests = 
-	pytest-black>=0.3.0,<0.3.10
+	pytest-black-ng>=0.4.0
 	check-manifest>=0.42
 	coverage>=5.2.1
 	pytest-cov>=2.10.1
 	pytest-isort>=1.2.0
 	pytest-pydocstyle>=2.2.0
 	pytest>=6.0
 	Sphinx>=4.2.0
```

### Comparing `marshmallow-utils-0.8.2/tests/conftest.py` & `marshmallow-utils-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/fields/test_identifier_field.py` & `marshmallow-utils-0.9.0/tests/fields/test_identifier_field.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/fields/test_url.py` & `marshmallow-utils-0.9.0/tests/fields/test_url.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_geojson.py` & `marshmallow-utils-0.9.0/tests/schemas/test_geojson.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_identifier_schema.py` & `marshmallow-utils-0.9.0/tests/schemas/test_identifier_schema.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_multipoint.py` & `marshmallow-utils-0.9.0/tests/schemas/test_multipoint.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_point.py` & `marshmallow-utils-0.9.0/tests/schemas/test_point.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_polygon.py` & `marshmallow-utils-0.9.0/tests/schemas/test_polygon.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/schemas/test_schema_permissions.py` & `marshmallow-utils-0.9.0/tests/schemas/test_schema_permissions.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_babel.py` & `marshmallow-utils-0.9.0/tests/test_babel.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_contrib.py` & `marshmallow-utils-0.9.0/tests/test_contrib.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_edtfdatestring.py` & `marshmallow-utils-0.9.0/tests/test_edtfdatestring.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_fields.py` & `marshmallow-utils-0.9.0/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_isolanguage.py` & `marshmallow-utils-0.9.0/tests/test_isolanguage.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_links.py` & `marshmallow-utils-0.9.0/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `marshmallow-utils-0.8.2/tests/test_nestedattr.py` & `marshmallow-utils-0.9.0/tests/test_nestedattr.py`

 * *Files identical despite different names*

