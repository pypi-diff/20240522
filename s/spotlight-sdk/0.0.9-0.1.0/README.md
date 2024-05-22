# Comparing `tmp/spotlight-sdk-0.0.9.tar.gz` & `tmp/spotlight-sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotlight-sdk-0.0.9.tar", last modified: Mon Feb 12 17:02:44 2024, max compression
+gzip compressed data, was "spotlight-sdk-0.1.0.tar", last modified: Wed May 22 02:07:47 2024, max compression
```

## Comparing `spotlight-sdk-0.0.9.tar` & `spotlight-sdk-0.1.0.tar`

### file list

```diff
@@ -1,96 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.577653 spotlight-sdk-0.0.9/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-02-12 17:02:44.576653 spotlight-sdk-0.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-12 17:02:44.577653 spotlight-sdk-0.0.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.560652 spotlight-sdk-0.0.9/spotlight/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.561652 spotlight-sdk-0.0.9/spotlight/admin/
--rw-rw-rw-   0 root         (0) root         (0)      955 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     7658 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     6877 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/admin/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.561652 spotlight-sdk-0.0.9/spotlight/api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.562652 spotlight-sdk-0.0.9/spotlight/api/auth/
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2263 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.563652 spotlight-sdk-0.0.9/spotlight/api/data/
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3081 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/asynchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.564652 spotlight-sdk-0.0.9/spotlight/api/data/barchart/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/model.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/barchart/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1406 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2811 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/data/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.565652 spotlight-sdk-0.0.9/spotlight/api/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/__util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.567653 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3141 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2805 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     2748 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2446 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.568652 spotlight-sdk-0.0.9/spotlight/api/dataset/view/
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)     1370 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/dataset/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.569653 spotlight-sdk-0.0.9/spotlight/api/permission/
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3008 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/api/permission/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.569653 spotlight-sdk-0.0.9/spotlight/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.571653 spotlight-sdk-0.0.9/spotlight/core/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      231 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.572653 spotlight-sdk-0.0.9/spotlight/core/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2417 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.572653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.573653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3921 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.574653 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      191 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1381 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1400 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4795 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.574653 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.575653 spotlight-sdk-0.0.9/spotlight/core/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4689 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3788 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      242 2024-02-12 17:02:31.000000 spotlight-sdk-0.0.9/spotlight/core/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-12 17:02:44.576653 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1264 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2782 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      176 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-12 17:02:44.000000 spotlight-sdk-0.0.9/spotlight_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.365738 spotlight-sdk-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-05-22 02:07:47.365738 spotlight-sdk-0.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      709 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 02:07:47.365738 spotlight-sdk-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.353737 spotlight-sdk-0.1.0/spotlight/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.353737 spotlight-sdk-0.1.0/spotlight/admin/
+-rw-rw-rw-   0 root         (0) root         (0)      955 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/admin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/admin/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     7658 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/admin/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     6877 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/admin/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.354737 spotlight-sdk-0.1.0/spotlight/api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.354737 spotlight-sdk-0.1.0/spotlight/api/alert/
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/alert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/alert/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/alert/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/alert/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2788 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/alert/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.355737 spotlight-sdk-0.1.0/spotlight/api/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2263 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.355737 spotlight-sdk-0.1.0/spotlight/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3081 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/asynchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.356737 spotlight-sdk-0.1.0/spotlight/api/data/barchart/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/barchart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/barchart/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/barchart/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      303 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/barchart/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/barchart/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1406 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/data/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.357737 spotlight-sdk-0.1.0/spotlight/api/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/__util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.358737 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3172 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2836 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     2779 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2477 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.358737 spotlight-sdk-0.1.0/spotlight/api/dataset/view/
+-rw-rw-rw-   0 root         (0) root         (0)      271 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1370 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/dataset/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.359737 spotlight-sdk-0.1.0/spotlight/api/permission/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3039 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2687 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/permission/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.359737 spotlight-sdk-0.1.0/spotlight/api/rule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.360738 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.361738 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      154 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/api/rule/data_rule_result/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.361738 spotlight-sdk-0.1.0/spotlight/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.362738 spotlight-sdk-0.1.0/spotlight/core/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      231 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2978 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.362738 spotlight-sdk-0.1.0/spotlight/core/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2417 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.362738 spotlight-sdk-0.1.0/spotlight/core/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.363738 spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3921 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.363738 spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      191 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1381 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1400 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1117 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4795 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.364738 spotlight-sdk-0.1.0/spotlight/core/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.364738 spotlight-sdk-0.1.0/spotlight/core/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4693 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3792 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      242 2024-05-22 02:07:33.000000 spotlight-sdk-0.1.0/spotlight/core/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:07:47.365738 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1264 2024-05-22 02:07:47.000000 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3424 2024-05-22 02:07:47.000000 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 02:07:47.000000 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      176 2024-05-22 02:07:47.000000 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 02:07:47.000000 spotlight-sdk-0.1.0/spotlight_sdk.egg-info/top_level.txt
```

### Comparing `spotlight-sdk-0.0.9/PKG-INFO` & `spotlight-sdk-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.0.9/README.md` & `spotlight-sdk-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/setup.py` & `spotlight-sdk-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ],
     python_requires=">=3.7",
     packages=setuptools.find_packages(
         include=['spotlight*'],
         exclude=['tests.*']
     ),
     install_requires=[
-        "requests==2.28.1",
+        "requests==2.31.0",
         "aiohttp>=3.8.4",
         "pandas>=2.0.1",
         "duckdb>=0.7.1",
         "trycast>=1.0.0",
         "pydash>=7.0.3",
         "cachetools>=5.3.0",
         "pydantic>=1.10.7",
```

### Comparing `spotlight-sdk-0.0.9/spotlight/admin/__init__.py` & `spotlight-sdk-0.1.0/spotlight/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/admin/__util.py` & `spotlight-sdk-0.1.0/spotlight/admin/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/admin/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/admin/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/admin/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/admin/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/auth/__util.py` & `spotlight-sdk-0.1.0/spotlight/api/auth/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/auth/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/auth/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/__util.py` & `spotlight-sdk-0.1.0/spotlight/api/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/barchart/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/data/barchart/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/barchart/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/data/barchart/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/model.py` & `spotlight-sdk-0.1.0/spotlight/api/data/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/data/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/__util.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/__util.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/asynchronous.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     Returns:
         Dict[str, Any]: Abstract dataset response
     """
     request_info = _update_abstract_dataset_request_info(id, request)
     return await __async_post_request(**request_info)
 
 
-@async_data_request()
+@async_data_request(processor=lambda response: None)
 async def async_delete_abstract_dataset(id: str) -> None:
     """
     Asynchronously delete abstract dataset by ID.
 
     Args:
         id (str): Abstract dataset ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/model.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/abstract/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/abstract/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Returns:
         Dict[str, Any]: Abstract dataset response
     """
     request_info = _update_abstract_dataset_request_info(id, request)
     return __post_request(**request_info)
 
 
-@data_request()
+@data_request(processor=lambda response: None)
 def delete_abstract_dataset(id: str) -> None:
     """
     Delete abstract dataset by ID.
 
     Args:
         id (str): Abstract dataset ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/asynchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Returns:
         Dict[str, Any]: Dataset response
     """
     request_info = _update_dataset_request_info(id, request)
     return await __async_post_request(**request_info)
 
 
-@async_data_request()
+@async_data_request(processor=lambda response: None)
 async def async_delete_dataset(id: str) -> None:
     """
     Asynchronously delete dataset by ID.
 
     Args:
         id (str): Dataset ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/model.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/synchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     Returns:
         Dict[str, Any]: Dataset response
     """
     request_info = _update_dataset_request_info(id, request)
     return __post_request(**request_info)
 
 
-@data_request()
+@data_request(processor=lambda response: None)
 def delete_dataset(id: str) -> None:
     """
     Delete dataset by ID.
 
     Args:
         id (str): Dataset ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/view/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/view/model.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/view/model.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/dataset/view/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/dataset/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/permission/__util.py` & `spotlight-sdk-0.1.0/spotlight/api/permission/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/api/permission/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/permission/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     Returns:
         Dict[str, Any]: Permission response
     """
     request_info = _update_permission_request_info(id, request)
     return await __async_post_request(**request_info)
 
 
-@async_data_request()
+@async_data_request(processor=lambda response: None)
 async def async_delete_permission(id: str) -> None:
     """
     Asynchronously delete permission by ID.
 
     Args:
         id: (str): Permission ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/api/permission/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/api/permission/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     Returns:
         Dict[str, Any]: Permission response
     """
     request_info = _update_permission_request_info(id, request)
     return __post_request(**request_info)
 
 
-@data_request()
+@data_request(processor=lambda response: None)
 def delete_permission(id: str) -> None:
     """
     Delete permission by ID.
 
     Args:
         id: (str): Permission ID
```

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/base.py` & `spotlight-sdk-0.1.0/spotlight/core/common/base.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/config.py` & `spotlight-sdk-0.1.0/spotlight/core/common/config.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/date/function.py` & `spotlight-sdk-0.1.0/spotlight/core/common/date/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/__util.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/authorization/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/__util.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/data/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/decorators/timeit.py` & `spotlight-sdk-0.1.0/spotlight/core/common/decorators/timeit.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/errors.py` & `spotlight-sdk-0.1.0/spotlight/core/common/errors.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/function.py` & `spotlight-sdk-0.1.0/spotlight/core/common/function.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/metaclass/singleton.py` & `spotlight-sdk-0.1.0/spotlight/core/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/requests/asynchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/requests/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @async_authenticated_request
 async def __async_get_request(
     endpoint: str,
     url_key: str = "spotlight",
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for asynchronous get requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -48,15 +48,15 @@
     endpoint: str,
     url_key: str = "spotlight",
     data=None,
     json=None,
     files=None,
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for asynchronous put requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -92,15 +92,15 @@
     endpoint: str,
     url_key: str = "spotlight",
     files=None,
     data=None,
     json=None,
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for asynchronous post requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -133,15 +133,15 @@
 
 @async_authenticated_request
 async def __async_delete_request(
     endpoint: str,
     url_key: str = "spotlight",
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for asynchronous delete requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
```

### Comparing `spotlight-sdk-0.0.9/spotlight/core/common/requests/synchronous.py` & `spotlight-sdk-0.1.0/spotlight/core/common/requests/synchronous.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @authenticated_request
 def __get_request(
     endpoint: str,
     url_key: str = "spotlight",
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for get requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -43,15 +43,15 @@
     endpoint: str,
     url_key: str = "spotlight",
     data=None,
     json=None,
     files=None,
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for put requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -81,15 +81,15 @@
     endpoint: str,
     url_key: str = "spotlight",
     files=None,
     data=None,
     json=None,
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for post requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
@@ -116,15 +116,15 @@
 
 @authenticated_request
 def __delete_request(
     endpoint: str,
     url_key: str = "spotlight",
     headers: Optional[dict] = None,
     params: Optional[dict] = None,
-    timeout: int = 30,
+    timeout: int = 120,
 ) -> Response:
     """
     Wrapper method for delete requests.
 
     Args:
         endpoint (str): API endpoint
         url_key (str): Key for looking up the url from the environment config
```

### Comparing `spotlight-sdk-0.0.9/spotlight_sdk.egg-info/PKG-INFO` & `spotlight-sdk-0.1.0/spotlight_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotlight-sdk
-Version: 0.0.9
+Version: 0.1.0
 Summary: Spotlight Python SDK
 Home-page: https://spotlight.dev
 Author: Spotlight
 Author-email: hello@spotlight.dev
 License: UNKNOWN
 Description: # Spotlight: The OTC Commodity Research Platform
```

### Comparing `spotlight-sdk-0.0.9/spotlight_sdk.egg-info/SOURCES.txt` & `spotlight-sdk-0.1.0/spotlight_sdk.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 setup.py
 spotlight/__init__.py
 spotlight/admin/__init__.py
 spotlight/admin/__util.py
 spotlight/admin/asynchronous.py
 spotlight/admin/synchronous.py
 spotlight/api/__init__.py
+spotlight/api/alert/__init__.py
+spotlight/api/alert/__util.py
+spotlight/api/alert/asynchronous.py
+spotlight/api/alert/model.py
+spotlight/api/alert/synchronous.py
 spotlight/api/auth/__init__.py
 spotlight/api/auth/__util.py
 spotlight/api/auth/asynchronous.py
 spotlight/api/auth/synchronous.py
 spotlight/api/data/__init__.py
 spotlight/api/data/__util.py
 spotlight/api/data/asynchronous.py
@@ -37,14 +42,25 @@
 spotlight/api/dataset/view/synchronous.py
 spotlight/api/permission/__init__.py
 spotlight/api/permission/__util.py
 spotlight/api/permission/asynchronous.py
 spotlight/api/permission/enum.py
 spotlight/api/permission/model.py
 spotlight/api/permission/synchronous.py
+spotlight/api/rule/__init__.py
+spotlight/api/rule/data_rule/__init__.py
+spotlight/api/rule/data_rule/__util.py
+spotlight/api/rule/data_rule/asynchronous.py
+spotlight/api/rule/data_rule/model.py
+spotlight/api/rule/data_rule/synchronous.py
+spotlight/api/rule/data_rule_result/__init__.py
+spotlight/api/rule/data_rule_result/__util.py
+spotlight/api/rule/data_rule_result/asynchronous.py
+spotlight/api/rule/data_rule_result/model.py
+spotlight/api/rule/data_rule_result/synchronous.py
 spotlight/core/__init__.py
 spotlight/core/common/__init__.py
 spotlight/core/common/base.py
 spotlight/core/common/base_enum.py
 spotlight/core/common/config.py
 spotlight/core/common/enum.py
 spotlight/core/common/errors.py
```

