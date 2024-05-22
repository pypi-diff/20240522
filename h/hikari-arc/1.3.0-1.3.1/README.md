# Comparing `tmp/hikari_arc-1.3.0.tar.gz` & `tmp/hikari_arc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikari_arc-1.3.0.tar", last modified: Sun May 12 19:49:36 2024, max compression
+gzip compressed data, was "hikari_arc-1.3.1.tar", last modified: Wed May 22 19:36:47 2024, max compression
```

## Comparing `hikari_arc-1.3.0.tar` & `hikari_arc-1.3.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/abc/
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54162 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/concurrency_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/hookable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/limiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/option.py
--rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/abc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/command/
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.035094 hikari_arc-1.3.0/arc/command/option/
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/command/option/custom/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/custom/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/mentionable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/option/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35485 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/slash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/command/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/context/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)    39977 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/ext/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/internal/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/internal/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/concurrency_limiter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.039094 hikari_arc-1.3.0/arc/utils/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/hooks/limiters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/loops.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/arc/utils/ratelimiter.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/cron_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/doc_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.043094 hikari_arc-1.3.0/hikari_arc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:49:35.000000 hikari_arc-1.3.0/hikari_arc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-12 19:49:36.000000 hikari_arc-1.3.0/hikari_arc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/rest_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:49:36.047094 hikari_arc-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:49:36.043094 hikari_arc-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_context_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_di.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_sigparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-12 19:49:31.000000 hikari_arc-1.3.0/tests/test_slash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.381700 hikari_arc-1.3.1/arc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54162 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28769 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/concurrency_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/hookable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12982 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/option.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19703 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/abc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17852 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.385700 hikari_arc-1.3.1/arc/command/option/
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/command/option/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/custom/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/mentionable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/option/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35485 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/slash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5996 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/command/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39977 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13518 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4921 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12965 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/concurrency_limiter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.389700 hikari_arc-1.3.1/arc/utils/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5894 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/hooks/limiters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12064 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/loops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/arc/utils/ratelimiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/cron_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/doc_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.393700 hikari_arc-1.3.1/hikari_arc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 19:36:47.000000 hikari_arc-1.3.1/hikari_arc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/rest_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:36:47.397700 hikari_arc-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:36:47.393700 hikari_arc-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_context_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_di.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_sigparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-05-22 19:36:41.000000 hikari_arc-1.3.1/tests/test_slash.py
```

### Comparing `hikari_arc-1.3.0/LICENSE` & `hikari_arc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/PKG-INFO` & `hikari_arc-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.0
+Version: 1.3.1
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,27 +24,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.21; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.10.0; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.2; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: ruff==0.4.4; extra == "dev"
-Requires-Dist: pyright==1.1.362; extra == "dev"
+Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
 Requires-Dist: typing_extensions==4.11.0; extra == "dev"
-Requires-Dist: pytest==8.2.0; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
+Requires-Dist: pytest==8.2.1; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
 Requires-Dist: croniter==2.0.5; extra == "cron"
 Requires-Dist: types-croniter==2.0.0.20240423; extra == "cron"
```

### Comparing `hikari_arc-1.3.0/README.md` & `hikari_arc-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/__init__.py` & `hikari_arc-1.3.1/arc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/__main__.py` & `hikari_arc-1.3.1/arc/__main__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/__init__.py` & `hikari_arc-1.3.1/arc/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/client.py` & `hikari_arc-1.3.1/arc/abc/client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/command.py` & `hikari_arc-1.3.1/arc/abc/command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/concurrency_limiting.py` & `hikari_arc-1.3.1/arc/abc/concurrency_limiting.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/error_handler.py` & `hikari_arc-1.3.1/arc/abc/error_handler.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/hookable.py` & `hikari_arc-1.3.1/arc/abc/hookable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/limiter.py` & `hikari_arc-1.3.1/arc/abc/limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/option.py` & `hikari_arc-1.3.1/arc/abc/option.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/abc/plugin.py` & `hikari_arc-1.3.1/arc/abc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/client.py` & `hikari_arc-1.3.1/arc/client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/__init__.py` & `hikari_arc-1.3.1/arc/command/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/message.py` & `hikari_arc-1.3.1/arc/command/message.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/__init__.py` & `hikari_arc-1.3.1/arc/command/option/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/attachment.py` & `hikari_arc-1.3.1/arc/command/option/attachment.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/bool.py` & `hikari_arc-1.3.1/arc/command/option/bool.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/channel.py` & `hikari_arc-1.3.1/arc/command/option/channel.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/custom/color.py` & `hikari_arc-1.3.1/arc/command/option/custom/color.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/custom/member.py` & `hikari_arc-1.3.1/arc/command/option/custom/member.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/float.py` & `hikari_arc-1.3.1/arc/command/option/float.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/int.py` & `hikari_arc-1.3.1/arc/command/option/int.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/mentionable.py` & `hikari_arc-1.3.1/arc/command/option/mentionable.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/role.py` & `hikari_arc-1.3.1/arc/command/option/role.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/str.py` & `hikari_arc-1.3.1/arc/command/option/str.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/option/user.py` & `hikari_arc-1.3.1/arc/command/option/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/slash.py` & `hikari_arc-1.3.1/arc/command/slash.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/command/user.py` & `hikari_arc-1.3.1/arc/command/user.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/context/__init__.py` & `hikari_arc-1.3.1/arc/context/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/context/autocomplete.py` & `hikari_arc-1.3.1/arc/context/autocomplete.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/context/base.py` & `hikari_arc-1.3.1/arc/context/base.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/errors.py` & `hikari_arc-1.3.1/arc/errors.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/events.py` & `hikari_arc-1.3.1/arc/events.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/extension.py` & `hikari_arc-1.3.1/arc/extension.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/__init__.py` & `hikari_arc-1.3.1/arc/internal/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/about.py` & `hikari_arc-1.3.1/arc/internal/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import typing as t
 
 __author__: t.Final[str] = "hypergonial"
 __author_email__: t.Final[str] = "git@hypergonial.com"
 __maintainer__: t.Final[str] = "hypergonial"
 __license__: t.Final[str] = "MIT"
 __url__: t.Final[str] = "https://github.com/hypergonial/hikari-arc"
-__version__: t.Final[str] = "1.3.0"
+__version__: t.Final[str] = "1.3.1"
 
 # MIT License
 #
 # Copyright (c) 2023-present hypergonial
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
```

### Comparing `hikari_arc-1.3.0/arc/internal/deprecation.py` & `hikari_arc-1.3.1/arc/internal/deprecation.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/options.py` & `hikari_arc-1.3.1/arc/internal/options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/sigparse.py` & `hikari_arc-1.3.1/arc/internal/sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/sync.py` & `hikari_arc-1.3.1/arc/internal/sync.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/types.py` & `hikari_arc-1.3.1/arc/internal/types.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/internal/version.py` & `hikari_arc-1.3.1/arc/internal/version.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/locale.py` & `hikari_arc-1.3.1/arc/locale.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/plugin.py` & `hikari_arc-1.3.1/arc/plugin.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/__init__.py` & `hikari_arc-1.3.1/arc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/concurrency_limiter.py` & `hikari_arc-1.3.1/arc/utils/concurrency_limiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/hooks/__init__.py` & `hikari_arc-1.3.1/arc/utils/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/hooks/basic.py` & `hikari_arc-1.3.1/arc/utils/hooks/basic.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/hooks/limiters.py` & `hikari_arc-1.3.1/arc/utils/hooks/limiters.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/arc/utils/loops.py` & `hikari_arc-1.3.1/arc/utils/loops.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,21 @@
 
     See Also
     --------
     - [`IntervalLoop`][arc.utils.loops.IntervalLoop]
     - [`CronLoop`][arc.utils.loops.CronLoop]
     """
 
-    __slots__ = ("_coro", "_task", "_failed", "_stop_next")
+    __slots__ = ("_coro", "_task", "_failed", "_stop_next", "_run_on_start")
 
-    def __init__(self, callback: t.Callable[P, t.Awaitable[None]]) -> None:
+    def __init__(self, callback: t.Callable[P, t.Awaitable[None]], *, run_on_start: bool = True) -> None:
         self._coro = callback
         self._task: asyncio.Task[None] | None = None
         self._failed: int = 0
+        self._run_on_start: bool = run_on_start
         self._stop_next: bool = False
 
         if not inspect.iscoroutinefunction(self._coro):
             raise TypeError("Expected a coroutine function.")
 
     async def __call__(self, *args: P.args, **kwargs: P.kwargs) -> None:
         """Call the underlying coroutine."""
@@ -47,31 +48,36 @@
 
         Returns
         -------
         float
             The number of seconds to wait before running the coroutine again.
         """
 
+    async def _call_callback(self, *args: P.args, **kwargs: P.kwargs) -> None:
+        """Call the callback and handle exceptions."""
+        try:
+            await self._coro(*args, **kwargs)
+        except Exception as e:
+            traceback_msg = "\n".join(traceback.format_exception(type(e), e, e.__traceback__))
+            print(f"Loop encountered exception: {e}", file=sys.stderr)
+            print(traceback_msg, file=sys.stderr)
+
+            if self._failed < 3:
+                self._failed += 1
+            else:
+                raise RuntimeError(f"Loop failed repeatedly, stopping it. Exception: {e}")
+
     async def _loopy_loop(self, *args: P.args, **kwargs: P.kwargs) -> None:
         """Main loop logic."""
+        if self._run_on_start:
+            await self._call_callback(*args, **kwargs)
+
         while not self._stop_next:
-            try:
-                await self._coro(*args, **kwargs)
-            except Exception as e:
-                traceback_msg = "\n".join(traceback.format_exception(type(e), e, e.__traceback__))
-                print(f"Loop encountered exception: {e}", file=sys.stderr)
-                print(traceback_msg, file=sys.stderr)
-
-                if self._failed < 3:
-                    self._failed += 1
-                    await asyncio.sleep(self._get_next_run())
-                else:
-                    raise RuntimeError(f"Loop failed repeatedly, stopping it. Exception: {e}")
-            else:
-                await asyncio.sleep(self._get_next_run())
+            await asyncio.sleep(self._get_next_run())
+            await self._call_callback(*args, **kwargs)
         self.cancel()
 
     def _create_task(self, *args: P.args, **kwargs: P.kwargs) -> asyncio.Task[None]:
         """Create the task for the loop."""
         task = asyncio.create_task(self._loopy_loop(*args, **kwargs))
         task.add_done_callback(self._handle_result)
         return task
@@ -131,14 +137,17 @@
         The number of seconds to wait before running the coroutine again.
     minutes : float, optional
         The number of minutes to wait before running the coroutine again.
     hours : float, optional
         The number of hours to wait before running the coroutine again.
     days : float, optional
         The number of days to wait before running the coroutine again.
+    run_on_start : bool, optional
+        Whether to run the callback immediately after starting the loop.
+        If set to false, the loop will wait for the specified interval before first running the callback.
 
     Raises
     ------
     ValueError
         If no interval is specified.
     TypeError
         If the passed function is not a coroutine function.
@@ -160,16 +169,17 @@
         self,
         callback: t.Callable[P, t.Awaitable[None]],
         *,
         seconds: float | None = None,
         minutes: float | None = None,
         hours: float | None = None,
         days: float | None = None,
+        run_on_start: bool = True,
     ) -> None:
-        super().__init__(callback)
+        super().__init__(callback, run_on_start=run_on_start)
         if not seconds and not minutes and not hours and not days:
             raise ValueError("At least one of 'seconds', 'minutes', 'hours' or 'days' must be not None.")
         else:
             seconds = seconds or 0
             minutes = minutes or 0
             hours = hours or 0
             days = hours or 0
@@ -192,14 +202,16 @@
 
     Parameters
     ----------
     callback : t.Callable[P, t.Awaitable[None]]
         The coroutine to run at the specified interval.
     cron_format : str
         The cron format to use. See https://en.wikipedia.org/wiki/Cron for more information.
+    timezone : datetime.timezone
+        The timezone to use for the cron format. Defaults to UTC.
 
     Raises
     ------
     ImportError
         If the `croniter` package is not installed.
     croniter.CroniterBadCronError
         If the cron format is invalid.
@@ -213,28 +225,38 @@
     loop.start()
     ```
 
     You may also use the decorator [`@arc.utils.cron_loop`][arc.utils.loops.cron_loop] to
     create a [`CronLoop`][arc.utils.loops.CronLoop] from a coroutine function.
     """
 
-    __slots__ = ("_iter",)
+    __slots__ = ("_iter", "_tz")
 
-    def __init__(self, callback: t.Callable[P, t.Awaitable[None]], cron_format: str) -> None:
-        super().__init__(callback)
+    def __init__(
+        self,
+        callback: t.Callable[P, t.Awaitable[None]],
+        cron_format: str,
+        *,
+        timezone: datetime.timezone = datetime.timezone.utc,
+    ) -> None:
+        super().__init__(callback, run_on_start=False)
+        self._tz = timezone
 
         try:
             import croniter
 
-            self._iter = croniter.croniter(cron_format, datetime.datetime.now())
+            self._iter = croniter.croniter(cron_format)
         except ImportError:
             raise ImportError("Missing dependency for CronLoop: 'croniter'")
 
     def _get_next_run(self) -> float:
-        return self._iter.get_next(float) - datetime.datetime.now().timestamp()
+        return (
+            self._iter.get_next(float, start_time=datetime.datetime.now(self._tz))
+            - datetime.datetime.now(self._tz).timestamp()
+        )
 
 
 def interval_loop(
     *, seconds: float | None = None, minutes: float | None = None, hours: float | None = None, days: float | None = None
 ) -> t.Callable[[t.Callable[P, t.Awaitable[None]]], IntervalLoop[P]]:
     """A decorator to create an [`IntervalLoop`][arc.utils.loops.IntervalLoop] out of a coroutine function.
```

### Comparing `hikari_arc-1.3.0/arc/utils/ratelimiter.py` & `hikari_arc-1.3.1/arc/utils/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/hikari_arc.egg-info/PKG-INFO` & `hikari_arc-1.3.1/hikari_arc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hikari-arc
-Version: 1.3.0
+Version: 1.3.1
 Summary: A command handler for hikari with a focus on type-safety and correctness.
 Home-page: https://github.com/hypergonial/hikari-arc
 Author: hypergonial
 Author-email: git@hypergonial.com
 Maintainer: hypergonial
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
@@ -24,27 +24,27 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: hikari>=2.0.0.dev122
 Requires-Dist: alluka<0.4,>=0.3.0
 Requires-Dist: attrs>=23.1
 Requires-Dist: colorama; sys_platform == "win32"
 Provides-Extra: docs
-Requires-Dist: mkdocs-material[imaging]~=9.5.21; extra == "docs"
+Requires-Dist: mkdocs-material[imaging]~=9.5.24; extra == "docs"
 Requires-Dist: mkdocs~=1.6.0; extra == "docs"
-Requires-Dist: mkdocstrings-python~=1.10.0; extra == "docs"
+Requires-Dist: mkdocstrings-python~=1.10.2; extra == "docs"
 Requires-Dist: black~=24.4.2; extra == "docs"
 Requires-Dist: griffe-inherited-docstrings~=1.0.0; extra == "docs"
 Requires-Dist: mkdocs-glightbox~=0.4.0; extra == "docs"
 Provides-Extra: dev
 Requires-Dist: ruff==0.4.4; extra == "dev"
-Requires-Dist: pyright==1.1.362; extra == "dev"
+Requires-Dist: pyright==1.1.364; extra == "dev"
 Requires-Dist: nox==2024.4.15; extra == "dev"
 Requires-Dist: typing_extensions==4.11.0; extra == "dev"
-Requires-Dist: pytest==8.2.0; extra == "dev"
-Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
+Requires-Dist: pytest==8.2.1; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.7; extra == "dev"
 Requires-Dist: slotscheck==0.19.0; extra == "dev"
 Provides-Extra: rest
 Requires-Dist: hikari[server]>=2.0.0.dev122; extra == "rest"
 Provides-Extra: cron
 Requires-Dist: croniter==2.0.5; extra == "cron"
 Requires-Dist: types-croniter==2.0.0.20240423; extra == "cron"
```

### Comparing `hikari_arc-1.3.0/hikari_arc.egg-info/SOURCES.txt` & `hikari_arc-1.3.1/hikari_arc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/pyproject.toml` & `hikari_arc-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/setup.py` & `hikari_arc-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_client.py` & `hikari_arc-1.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_context_command.py` & `hikari_arc-1.3.1/tests/test_context_command.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_di.py` & `hikari_arc-1.3.1/tests/test_di.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_inheritance.py` & `hikari_arc-1.3.1/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_options.py` & `hikari_arc-1.3.1/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_sigparse.py` & `hikari_arc-1.3.1/tests/test_sigparse.py`

 * *Files identical despite different names*

### Comparing `hikari_arc-1.3.0/tests/test_slash.py` & `hikari_arc-1.3.1/tests/test_slash.py`

 * *Files identical despite different names*

