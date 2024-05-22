# Comparing `tmp/switch_api-0.5.8.tar.gz` & `tmp/switch_api-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.5.8.tar", last modified: Tue May 21 04:00:38 2024, max compression
+gzip compressed data, was "switch_api-0.5.9.tar", last modified: Wed May 22 07:12:40 2024, max compression
```

## Comparing `switch_api-0.5.8.tar` & `switch_api-0.5.9.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.759275 switch_api-0.5.8/
--rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-21 04:00:30.000000 switch_api-0.5.8/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (127)    36960 2024-05-21 04:00:30.000000 switch_api-0.5.8/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-21 04:00:30.000000 switch_api-0.5.8/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-21 04:00:30.000000 switch_api-0.5.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)    38234 2024-05-21 04:00:38.759275 switch_api-0.5.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-21 04:00:30.000000 switch_api-0.5.8/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-21 04:00:30.000000 switch_api-0.5.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-21 04:00:38.759275 switch_api-0.5.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-21 04:00:30.000000 switch_api-0.5.8/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.751274 switch_api-0.5.8/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.751274 switch_api-0.5.8/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.751274 switch_api-0.5.8/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.751274 switch_api-0.5.8/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/_guide/
--rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_guide/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_guide/main.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_guide/processor.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4205 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_utils/_marketplace.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14655 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/controls/
--rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/controls/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/controls/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12443 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/controls/_mqtt.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/controls/controls.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/email/
--rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/email/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/email/email_sender.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.755275 switch_api-0.5.8/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)   117297 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.759275 switch_api-0.5.8/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (127)     3377 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    88430 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30536 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.759275 switch_api-0.5.8/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-21 04:00:30.000000 switch_api-0.5.8/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 04:00:38.751274 switch_api-0.5.8/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)    38234 2024-05-21 04:00:38.000000 switch_api-0.5.8/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1848 2024-05-21 04:00:38.000000 switch_api-0.5.8/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 04:00:38.000000 switch_api-0.5.8/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-21 04:00:38.000000 switch_api-0.5.8/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-21 04:00:38.000000 switch_api-0.5.8/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.804542 switch_api-0.5.9/
+-rw-r--r--   0 vsts      (1001) docker     (127)      249 2024-05-22 07:12:32.000000 switch_api-0.5.9/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)    37065 2024-05-22 07:12:32.000000 switch_api-0.5.9/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (127)     1093 2024-05-22 07:12:32.000000 switch_api-0.5.9/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-05-22 07:12:32.000000 switch_api-0.5.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)    38339 2024-05-22 07:12:40.804542 switch_api-0.5.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      590 2024-05-22 07:12:32.000000 switch_api-0.5.9/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      113 2024-05-22 07:12:32.000000 switch_api-0.5.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       62 2024-05-22 07:12:40.804542 switch_api-0.5.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1448 2024-05-22 07:12:32.000000 switch_api-0.5.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1508 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (127)      391 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8127 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (127)      393 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5851 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (127)      361 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8752 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api/_guide/
+-rw-r--r--   0 vsts      (1001) docker     (127)      455 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_guide/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3108 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_guide/main.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2093 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_guide/processor.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.796542 switch_api-0.5.9/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)      462 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4205 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5952 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_utils/_marketplace.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14920 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23502 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.796542 switch_api-0.5.9/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (127)      642 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14709 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.796542 switch_api-0.5.9/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (127)      480 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6985 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.796542 switch_api-0.5.9/switch_api/controls/
+-rw-r--r--   0 vsts      (1001) docker     (127)      487 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/controls/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      803 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/controls/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12443 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/controls/_mqtt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13320 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/controls/controls.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.796542 switch_api-0.5.9/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (127)      558 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7724 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.800542 switch_api-0.5.9/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (127)      472 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4935 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.800542 switch_api-0.5.9/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2066 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15754 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.800542 switch_api-0.5.9/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1038 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7519 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1652 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2970 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1406 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3359 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.800542 switch_api-0.5.9/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1872 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12939 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    36653 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   117297 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.804542 switch_api-0.5.9/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (127)     3377 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    88430 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35931 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30536 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.804542 switch_api-0.5.9/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (127)      542 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2214 2024-05-22 07:12:32.000000 switch_api-0.5.9/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-22 07:12:40.792542 switch_api-0.5.9/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    38339 2024-05-22 07:12:40.000000 switch_api-0.5.9/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1848 2024-05-22 07:12:40.000000 switch_api-0.5.9/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-22 07:12:40.000000 switch_api-0.5.9/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      148 2024-05-22 07:12:40.000000 switch_api-0.5.9/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       11 2024-05-22 07:12:40.000000 switch_api-0.5.9/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.5.8/HISTORY.md` & `switch_api-0.5.9/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # History
 
+## 0.5.8
+### Fixed
+In the `analytics` module: 
+- Fixed bug on AU datacentre API endpoint construction. 
+
 ## 0.5.7
 ### Modified
 In the `controls` module: 
 - Modified `submit_control` method
   - Returns sensor control values upon control request acknowledgement
 
 ## 0.5.5
```

### Comparing `switch_api-0.5.8/LICENCE` & `switch_api-0.5.9/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/PKG-INFO` & `switch_api-0.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch_api
-Version: 0.5.8
+Version: 0.5.9
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,19 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.8
+### Fixed
+In the `analytics` module: 
+- Fixed bug on AU datacentre API endpoint construction. 
+
 ## 0.5.7
 ### Modified
 In the `controls` module: 
 - Modified `submit_control` method
   - Returns sensor control values upon control request acknowledgement
 
 ## 0.5.5
```

### Comparing `switch_api-0.5.8/README.md` & `switch_api-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/setup.py` & `switch_api-0.5.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() +
     '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.5.8",
+    version="0.5.9",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus',
                       'msal>=1.11.0', 'paho-mqtt==1.6.1', 'uvicorn==0.22.0', 'fastapi==0.98.0', 'pyodbc==4.0.39'],
     python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
```

### Comparing `switch_api-0.5.8/switch_api/__init__.py` & `switch_api-0.5.9/switch_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,8 @@
 # _ch.setLevel(logging.INFO)  # sets the handler info
 # _ch.setFormatter(logging.Formatter(INFOFORMATTER))  # sets the handler formatting
 #
 # # adds the handler to the global variable: log
 # log.addHandler(_ch)
 # https://dev.to/joaomcteixeira/setting-up-python-logging-for-a-library-app-6ml
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
```

### Comparing `switch_api-0.5.8/switch_api/_authentication/_authentication.py` & `switch_api-0.5.9/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.5.9/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.5.9/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_guide/main.py` & `switch_api-0.5.9/switch_api/_guide/main.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_guide/processor.py` & `switch_api-0.5.9/switch_api/_guide/processor.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_utils/_constants.py` & `switch_api-0.5.9/switch_api/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_utils/_marketplace.py` & `switch_api-0.5.9/switch_api/_utils/_marketplace.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_utils/_platform.py` & `switch_api-0.5.9/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/_utils/_utils.py` & `switch_api-0.5.9/switch_api/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/analytics/__init__.py` & `switch_api-0.5.9/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/analytics/analytics.py` & `switch_api-0.5.9/switch_api/analytics/analytics.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,17 @@
         schema_error = err.failure_cases
         return False, schema_error
 
     headers = api_inputs.api_headers.default
 
     datacentre = api_inputs.api_base_url.split('-', 1)[1].split('.')[0]
 
+    if datacentre == 'ae':
+        datacentre = 'au'
+
     base_url = f"https://platformapi-{datacentre}-staging.switchautomation.com"
 
     # url = f"{api_inputs.api_projects_endpoint}/{api_inputs.api_project_id}/benchmarking/performanceProjects/{performance_project_id}/standards/{standard_id}/sites/statistics"
 
     url = f"{base_url}/api/1.0/projects/{api_inputs.api_project_id}/benchmarking/performanceProjects/{performance_project_id}/standards/{standard_id}/sites/statistics"
 
     logger.info("Sending request: PUT %s", url)
```

### Comparing `switch_api-0.5.8/switch_api/cache/cache.py` & `switch_api-0.5.9/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/controls/_constants.py` & `switch_api-0.5.9/switch_api/controls/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/controls/_mqtt.py` & `switch_api-0.5.9/switch_api/controls/_mqtt.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/controls/controls.py` & `switch_api-0.5.9/switch_api/controls/controls.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/dataset/__init__.py` & `switch_api-0.5.9/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/dataset/dataset.py` & `switch_api-0.5.9/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/email/email_sender.py` & `switch_api-0.5.9/switch_api/email/email_sender.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/error_handlers/__init__.py` & `switch_api-0.5.9/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/error_handlers/error_handlers.py` & `switch_api-0.5.9/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/extensions/__init__.py` & `switch_api-0.5.9/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/extensions/extensions.py` & `switch_api-0.5.9/switch_api/extensions/extensions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/extensions/field_meta.py` & `switch_api-0.5.9/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/extensions/helpers.py` & `switch_api-0.5.9/switch_api/extensions/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/extensions/pipeline.py` & `switch_api-0.5.9/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/initialize.py` & `switch_api-0.5.9/switch_api/initialize.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/integration/__init__.py` & `switch_api-0.5.9/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/integration/_utils.py` & `switch_api-0.5.9/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/integration/helpers.py` & `switch_api-0.5.9/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/integration/integration.py` & `switch_api-0.5.9/switch_api/integration/integration.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/pipeline/__init__.py` & `switch_api-0.5.9/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/pipeline/automation.py` & `switch_api-0.5.9/switch_api/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/pipeline/definitions.py` & `switch_api-0.5.9/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/pipeline/pipeline.py` & `switch_api-0.5.9/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/platform_insights/__init__.py` & `switch_api-0.5.9/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api/platform_insights/platform_insights.py` & `switch_api-0.5.9/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.5.8/switch_api.egg-info/PKG-INFO` & `switch_api-0.5.9/switch_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: switch-api
-Version: 0.5.8
+Version: 0.5.9
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,19 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.5.8
+### Fixed
+In the `analytics` module: 
+- Fixed bug on AU datacentre API endpoint construction. 
+
 ## 0.5.7
 ### Modified
 In the `controls` module: 
 - Modified `submit_control` method
   - Returns sensor control values upon control request acknowledgement
 
 ## 0.5.5
```

### Comparing `switch_api-0.5.8/switch_api.egg-info/SOURCES.txt` & `switch_api-0.5.9/switch_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

