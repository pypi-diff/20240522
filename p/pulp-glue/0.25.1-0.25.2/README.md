# Comparing `tmp/pulp-glue-0.25.1.tar.gz` & `tmp/pulp-glue-0.25.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-0.25.1.tar", last modified: Tue Apr 30 07:09:05 2024, max compression
+gzip compressed data, was "pulp-glue-0.25.2.tar", last modified: Wed May 22 10:06:51 2024, max compression
```

## Comparing `pulp-glue-0.25.1.tar` & `pulp-glue-0.25.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/ansible/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/ansible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/ansible/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/ansible/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/ansible/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/ansible/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/ansible/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/ansible/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/certguard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/certguard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/certguard/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/certguard/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/certguard/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/certguard/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/certguard/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/certguard/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/common/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51811 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/common/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/common/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/common/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29248 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/container/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/container/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/container/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/container/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/container/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/container/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/container/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:00.000000 pulp-glue-0.25.1/pulp_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20886 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/core/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.359561 pulp-glue-0.25.1/pulp_glue/core/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/core/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/core/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/file/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/file/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/file/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/file/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/file/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/file/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/python/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/python/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/python/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/python/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/python/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/python/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/rpm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/rpm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/rpm/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/rpm/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue/rpm/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/pulp_glue/rpm/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/rpm/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pulp_glue/rpm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 07:09:05.363561 pulp-glue-0.25.1/pulp_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-30 07:09:05.000000 pulp-glue-0.25.1/pulp_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-30 07:09:05.000000 pulp-glue-0.25.1/pulp_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 07:09:05.000000 pulp-glue-0.25.1/pulp_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-30 07:09:05.000000 pulp-glue-0.25.1/pulp_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 07:09:05.000000 pulp-glue-0.25.1/pulp_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-30 07:09:01.000000 pulp-glue-0.25.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 07:09:05.367561 pulp-glue-0.25.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/ansible/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/ansible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/ansible/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/ansible/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/ansible/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/ansible/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/ansible/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/ansible/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/certguard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/certguard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/certguard/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/certguard/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/certguard/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/certguard/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/certguard/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/certguard/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51811 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/common/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/common/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/common/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29229 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/container/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7546 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/container/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/container/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/container/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/container/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/container/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/container/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20886 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/core/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/core/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/core/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/core/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/file/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/file/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/file/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue/file/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/file/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/file/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/pulp_glue/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/python/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/python/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/python/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/pulp_glue/python/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/python/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/python/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/pulp_glue/rpm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/rpm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/rpm/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/rpm/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.345669 pulp-glue-0.25.2/pulp_glue/rpm/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/pulp_glue/rpm/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/rpm/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pulp_glue/rpm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:06:51.349669 pulp-glue-0.25.2/pulp_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 10:06:51.000000 pulp-glue-0.25.2/pulp_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-22 10:06:51.000000 pulp-glue-0.25.2/pulp_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:06:51.000000 pulp-glue-0.25.2/pulp_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 10:06:51.000000 pulp-glue-0.25.2/pulp_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 10:06:51.000000 pulp-glue-0.25.2/pulp_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-05-22 10:06:47.000000 pulp-glue-0.25.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:06:51.353669 pulp-glue-0.25.2/setup.cfg
```

### Comparing `pulp-glue-0.25.1/PKG-INFO` & `pulp-glue-0.25.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.25.1
+Version: 0.25.2
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: documentation, https://docs.pulpproject.org/pulp_cli/
 Project-URL: repository, https://github.com/pulp/pulp-cli
 Project-URL: changelog, https://docs.pulpproject.org/pulp_cli/CHANGES/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulp-glue-0.25.1/pulp_glue/ansible/context.py` & `pulp-glue-0.25.2/pulp_glue/ansible/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/certguard/context.py` & `pulp-glue-0.25.2/pulp_glue/certguard/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/common/context.py` & `pulp-glue-0.25.2/pulp_glue/common/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/common/i18n.py` & `pulp-glue-0.25.2/pulp_glue/common/i18n.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/common/openapi.py` & `pulp-glue-0.25.2/pulp_glue/common/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,16 +148,16 @@
         )
         if cid:
             self._session.headers["Correlation-Id"] = cid
         if headers:
             self._session.headers.update(headers)
         self._session.max_redirects = 0
 
-        verify: t.Optional[t.Union[bool, str]] = (
-            os.environ.get("PULP_CA_BUNDLE") if validate_certs is not False else False
+        verify: t.Optional[t.Union[bool, str]] = validate_certs and os.environ.get(
+            "PULP_CA_BUNDLE", True
         )
         session_settings = self._session.merge_environment_settings(
             base_url, {}, None, verify, None
         )
         self._session.verify = session_settings["verify"]
         self._session.proxies = session_settings["proxies"]
```

### Comparing `pulp-glue-0.25.1/pulp_glue/container/context.py` & `pulp-glue-0.25.2/pulp_glue/container/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/core/context.py` & `pulp-glue-0.25.2/pulp_glue/core/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/file/context.py` & `pulp-glue-0.25.2/pulp_glue/file/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/python/context.py` & `pulp-glue-0.25.2/pulp_glue/python/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue/rpm/context.py` & `pulp-glue-0.25.2/pulp_glue/rpm/context.py`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pulp_glue.egg-info/PKG-INFO` & `pulp-glue-0.25.2/pulp_glue.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue
-Version: 0.25.1
+Version: 0.25.2
 Summary: Version agnostic glue library to talk to pulpcore's REST API.
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: documentation, https://docs.pulpproject.org/pulp_cli/
 Project-URL: repository, https://github.com/pulp/pulp-cli
 Project-URL: changelog, https://docs.pulpproject.org/pulp_cli/CHANGES/
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pulp-glue-0.25.1/pulp_glue.egg-info/SOURCES.txt` & `pulp-glue-0.25.2/pulp_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-glue-0.25.1/pyproject.toml` & `pulp-glue-0.25.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulp-glue"
-version = "0.25.1"
+version = "0.25.2"
 description = "Version agnostic glue library to talk to pulpcore's REST API."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "GPLv2+"}
 authors = [
   {name = "Pulp Team", email = "pulp-list@redhat.com"},
 ]
```

