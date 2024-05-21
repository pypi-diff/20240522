# Comparing `tmp/rbfly-0.8.3.tar.gz` & `tmp/rbfly-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rbfly-0.8.3.tar", last modified: Sat May  4 07:35:24 2024, max compression
+gzip compressed data, was "rbfly-0.8.4.tar", last modified: Tue May 21 22:38:48 2024, max compression
```

## Comparing `rbfly-0.8.3.tar` & `rbfly-0.8.4.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.951259 rbfly-0.8.3/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2024-01-07 12:33:04.000000 rbfly-0.8.3/COPYING
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-04 07:35:24.951259 rbfly-0.8.3/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.3/README
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      589 2024-04-14 21:14:44.000000 rbfly-0.8.3/pyproject.toml
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.927926 rbfly-0.8.3/rbfly/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      922 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   194660 2024-05-04 07:19:20.000000 rbfly-0.8.3/rbfly/_buffer.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1434 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_buffer.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_buffer.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   185798 2024-05-04 07:19:20.000000 rbfly-0.8.3/rbfly/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.h
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/_codec.pyx
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.931259 rbfly-0.8.3/rbfly/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   742026 2024-05-04 07:35:05.000000 rbfly-0.8.3/rbfly/amqp/_message.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1629 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/_message.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1560 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/amqp/_message.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20670 2024-05-04 07:34:58.000000 rbfly-0.8.3/rbfly/amqp/_message.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4250 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/cm.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/py.typed
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3295 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/slotmap.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1649 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1426495 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_client.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2248 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_client.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    19574 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_client.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   738316 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_codec.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1555 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_codec.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12519 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_codec.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)   516078 2024-05-04 07:19:21.000000 rbfly-0.8.3/rbfly/streams/_mqueue.c
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1065 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pxd
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pyi
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3893 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/_mqueue.pyx
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20151 2024-05-04 00:04:20.000000 rbfly-0.8.3/rbfly/streams/client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8770 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2024-01-08 11:28:18.000000 rbfly-0.8.3/rbfly/streams/const.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1287 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/error.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5197 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    27513 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/protocol.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2363 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4027 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/streams/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/__init__.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/amqp/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/amqp/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10497 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/amqp/test_message.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly/tests/streams/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/__init__.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18746 2024-05-04 00:04:37.000000 rbfly-0.8.3/rbfly/tests/streams/test_client.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)    16771 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_codec.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2267 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_mqueue.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1329 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/streams/test_offset.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3393 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/test_slotmap.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/tests/test_util.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2306 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/types.py
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2024-01-07 12:33:04.000000 rbfly-0.8.3/rbfly/util.py
-drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-04 07:35:24.934592 rbfly-0.8.3/rbfly.egg-info/
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/PKG-INFO
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1306 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/SOURCES.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/dependency_links.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)      259 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/requires.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2024-05-04 07:35:24.000000 rbfly-0.8.3/rbfly.egg-info/top_level.txt
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1222 2024-05-04 07:35:24.954592 rbfly-0.8.3/setup.cfg
--rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1680 2024-01-07 12:33:04.000000 rbfly-0.8.3/setup.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.240177 rbfly-0.8.4/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    35147 2024-01-07 12:33:04.000000 rbfly-0.8.4/COPYING
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-21 22:38:48.240177 rbfly-0.8.4/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.4/README
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      589 2024-04-14 21:14:44.000000 rbfly-0.8.4/pyproject.toml
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.216844 rbfly-0.8.4/rbfly/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      922 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   194660 2024-05-04 07:19:20.000000 rbfly-0.8.4/rbfly/_buffer.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1434 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/_buffer.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1898 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/_buffer.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   185798 2024-05-04 07:19:20.000000 rbfly-0.8.4/rbfly/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1098 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/_codec.h
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1197 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/_codec.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2298 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/_codec.pyx
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.220178 rbfly-0.8.4/rbfly/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      956 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   740581 2024-05-04 07:35:47.000000 rbfly-0.8.4/rbfly/amqp/_message.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1629 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/amqp/_message.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1560 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/amqp/_message.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20652 2024-05-04 07:35:43.000000 rbfly-0.8.4/rbfly/amqp/_message.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4250 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/cm.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1335 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        0 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/py.typed
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3295 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/slotmap.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.223511 rbfly-0.8.4/rbfly/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1649 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)  1426495 2024-05-04 07:19:21.000000 rbfly-0.8.4/rbfly/streams/_client.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2248 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_client.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    19574 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_client.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   738316 2024-05-04 07:19:21.000000 rbfly-0.8.4/rbfly/streams/_codec.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1555 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_codec.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    12519 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_codec.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)   516078 2024-05-04 07:19:21.000000 rbfly-0.8.4/rbfly/streams/_mqueue.c
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1065 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_mqueue.pxd
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1244 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_mqueue.pyi
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3893 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/_mqueue.pyx
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    20151 2024-05-10 10:17:27.000000 rbfly-0.8.4/rbfly/streams/client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     8770 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1894 2024-01-08 11:28:18.000000 rbfly-0.8.4/rbfly/streams/const.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1287 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/error.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     5197 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    27513 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/protocol.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2363 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     4027 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/streams/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.223511 rbfly-0.8.4/rbfly/tests/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/__init__.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.223511 rbfly-0.8.4/rbfly/tests/amqp/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/amqp/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    10497 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/amqp/test_message.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.226844 rbfly-0.8.4/rbfly/tests/streams/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      790 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/streams/__init__.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    18746 2024-05-04 00:04:37.000000 rbfly-0.8.4/rbfly/tests/streams/test_client.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)    16771 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/streams/test_codec.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2267 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/streams/test_mqueue.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1329 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/streams/test_offset.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3393 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/test_slotmap.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     3228 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/tests/test_util.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2306 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/types.py
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2008 2024-01-07 12:33:04.000000 rbfly-0.8.4/rbfly/util.py
+drwxr-xr-x   0 wrobell   (1000) wrobell   (1000)        0 2024-05-21 22:38:48.226844 rbfly-0.8.4/rbfly.egg-info/
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     2663 2024-05-21 22:38:48.000000 rbfly-0.8.4/rbfly.egg-info/PKG-INFO
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1306 2024-05-21 22:38:48.000000 rbfly-0.8.4/rbfly.egg-info/SOURCES.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        1 2024-05-21 22:38:48.000000 rbfly-0.8.4/rbfly.egg-info/dependency_links.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)      259 2024-05-21 22:38:48.000000 rbfly-0.8.4/rbfly.egg-info/requires.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)        6 2024-05-21 22:38:48.000000 rbfly-0.8.4/rbfly.egg-info/top_level.txt
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1222 2024-05-21 22:38:48.243511 rbfly-0.8.4/setup.cfg
+-rw-r--r--   0 wrobell   (1000) wrobell   (1000)     1680 2024-01-07 12:33:04.000000 rbfly-0.8.4/setup.py
```

### Comparing `rbfly-0.8.3/COPYING` & `rbfly-0.8.4/COPYING`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/PKG-INFO` & `rbfly-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.8.3
+Version: 0.8.4
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
@@ -27,15 +27,15 @@
 Requires-Dist: ruff>=0.3.0; extra == "tests"
 Requires-Dist: toml; extra == "tests"
 Requires-Dist: uvloop>=0.19.0; extra == "tests"
 Provides-Extra: performance
 Requires-Dist: msgpack; extra == "performance"
 Requires-Dist: aiokafka==0.8.1; extra == "performance"
 Requires-Dist: rstream==0.13.0; extra == "performance"
-Requires-Dist: uamqp==1.6.5; extra == "performance"
+Requires-Dist: uamqp==1.6.9; extra == "performance"
 Requires-Dist: python-qpid-proton==0.39.0; extra == "performance"
 Provides-Extra: doc
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 RbFly is a library for RabbitMQ Streams using Python asyncio
 
 - https://www.rabbitmq.com/streams.html
```

### Comparing `rbfly-0.8.3/README` & `rbfly-0.8.4/README`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/pyproject.toml` & `rbfly-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/__init__.py` & `rbfly-0.8.4/rbfly/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_buffer.c` & `rbfly-0.8.4/rbfly/_buffer.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_buffer.pxd` & `rbfly-0.8.4/rbfly/_buffer.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_buffer.pyx` & `rbfly-0.8.4/rbfly/_buffer.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_codec.c` & `rbfly-0.8.4/rbfly/_codec.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_codec.h` & `rbfly-0.8.4/rbfly/_codec.h`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_codec.pxd` & `rbfly-0.8.4/rbfly/_codec.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/_codec.pyx` & `rbfly-0.8.4/rbfly/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/amqp/__init__.py` & `rbfly-0.8.4/rbfly/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/amqp/_message.c` & `rbfly-0.8.4/rbfly/amqp/_message.c`

 * *Files 0% similar despite different names*

```diff
@@ -2557,19 +2557,17 @@
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_logger[] = "logger";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_offset[] = "offset";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_return[] = "return";
-static const char __pyx_k_tzinfo[] = "tzinfo";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_logging[] = "logging";
 static const char __pyx_k_message[] = "message";
-static const char __pyx_k_replace[] = "replace";
 static const char __pyx_k_datetime[] = "datetime";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_timezone[] = "timezone";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_bytearray[] = "bytearray";
 static const char __pyx_k_getLogger[] = "getLogger";
@@ -2583,24 +2581,24 @@
 static const char __pyx_k_annotations[] = "annotations";
 static const char __pyx_k_contextvars[] = "contextvars";
 static const char __pyx_k_decode_amqp[] = "decode_amqp";
 static const char __pyx_k_encode_amqp[] = "encode_amqp";
 static const char __pyx_k_initializing[] = "_initializing";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_stringsource[] = "<stringsource>";
+static const char __pyx_k_fromtimestamp[] = "fromtimestamp";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_stream_offset[] = "stream_offset";
 static const char __pyx_k_app_properties[] = "app_properties";
 static const char __pyx_k_get_message_ctx[] = "get_message_ctx";
 static const char __pyx_k_set_message_ctx[] = "set_message_ctx";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_AMQPDecoderError[] = "AMQPDecoderError";
 static const char __pyx_k_RbFlyBufferError[] = "RbFlyBufferError";
 static const char __pyx_k_stream_timestamp[] = "stream_timestamp";
-static const char __pyx_k_utcfromtimestamp[] = "utcfromtimestamp";
 static const char __pyx_k_stream_publish_id[] = "stream_publish_id";
 static const char __pyx_k_Data_too_long_size[] = "Data too long, size={}";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_rbfly_amqp__message[] = "rbfly.amqp._message";
 static const char __pyx_k_rbfly_amqp__message_pyx[] = "rbfly/amqp/_message.pyx";
 static const char __pyx_k_is_set_stream_publish_id[] = "is_set_stream_publish_id";
@@ -2816,14 +2814,15 @@
   PyObject *__pyx_n_s_decode_amqp;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_kp_u_enable;
   PyObject *__pyx_n_s_encode;
   PyObject *__pyx_n_s_encode_amqp;
   PyObject *__pyx_n_s_error;
   PyObject *__pyx_n_s_format;
+  PyObject *__pyx_n_s_fromtimestamp;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get;
   PyObject *__pyx_n_s_getLogger;
   PyObject *__pyx_n_s_get_message_ctx;
   PyObject *__pyx_n_s_getstate;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_initializing;
@@ -2844,15 +2843,14 @@
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_range;
   PyObject *__pyx_n_s_rbfly_amqp__message;
   PyObject *__pyx_kp_s_rbfly_amqp__message_pyx;
   PyObject *__pyx_n_s_reduce;
   PyObject *__pyx_n_s_reduce_cython;
   PyObject *__pyx_n_s_reduce_ex;
-  PyObject *__pyx_n_s_replace;
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_n_s_set;
   PyObject *__pyx_n_s_set_message_ctx;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
   PyObject *__pyx_n_s_size;
@@ -2861,17 +2859,15 @@
   PyObject *__pyx_n_s_stream_publish_id;
   PyObject *__pyx_n_s_stream_timestamp;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_n_s_timestamp;
   PyObject *__pyx_n_s_timezone;
   PyObject *__pyx_n_s_types;
-  PyObject *__pyx_n_s_tzinfo;
   PyObject *__pyx_n_s_utc;
-  PyObject *__pyx_n_s_utcfromtimestamp;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_uuid;
   PyObject *__pyx_int_0;
   PyObject *__pyx_int_10;
   PyObject *__pyx_int_1000;
   PyObject *__pyx_int_2147483648;
   PyObject *__pyx_int_4294967295;
@@ -2984,14 +2980,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_decode_amqp);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode);
   Py_CLEAR(clear_module_state->__pyx_n_s_encode_amqp);
   Py_CLEAR(clear_module_state->__pyx_n_s_error);
   Py_CLEAR(clear_module_state->__pyx_n_s_format);
+  Py_CLEAR(clear_module_state->__pyx_n_s_fromtimestamp);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get);
   Py_CLEAR(clear_module_state->__pyx_n_s_getLogger);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_message_ctx);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
@@ -3012,15 +3009,14 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_range);
   Py_CLEAR(clear_module_state->__pyx_n_s_rbfly_amqp__message);
   Py_CLEAR(clear_module_state->__pyx_kp_s_rbfly_amqp__message_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
-  Py_CLEAR(clear_module_state->__pyx_n_s_replace);
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_n_s_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_set_message_ctx);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_size);
@@ -3029,17 +3025,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_stream_publish_id);
   Py_CLEAR(clear_module_state->__pyx_n_s_stream_timestamp);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_n_s_timestamp);
   Py_CLEAR(clear_module_state->__pyx_n_s_timezone);
   Py_CLEAR(clear_module_state->__pyx_n_s_types);
-  Py_CLEAR(clear_module_state->__pyx_n_s_tzinfo);
   Py_CLEAR(clear_module_state->__pyx_n_s_utc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_utcfromtimestamp);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_uuid);
   Py_CLEAR(clear_module_state->__pyx_int_0);
   Py_CLEAR(clear_module_state->__pyx_int_10);
   Py_CLEAR(clear_module_state->__pyx_int_1000);
   Py_CLEAR(clear_module_state->__pyx_int_2147483648);
   Py_CLEAR(clear_module_state->__pyx_int_4294967295);
@@ -3130,14 +3124,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_decode_amqp);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode);
   Py_VISIT(traverse_module_state->__pyx_n_s_encode_amqp);
   Py_VISIT(traverse_module_state->__pyx_n_s_error);
   Py_VISIT(traverse_module_state->__pyx_n_s_format);
+  Py_VISIT(traverse_module_state->__pyx_n_s_fromtimestamp);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get);
   Py_VISIT(traverse_module_state->__pyx_n_s_getLogger);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_message_ctx);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
@@ -3158,15 +3153,14 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_range);
   Py_VISIT(traverse_module_state->__pyx_n_s_rbfly_amqp__message);
   Py_VISIT(traverse_module_state->__pyx_kp_s_rbfly_amqp__message_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
-  Py_VISIT(traverse_module_state->__pyx_n_s_replace);
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_n_s_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_set_message_ctx);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_size);
@@ -3175,17 +3169,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_stream_publish_id);
   Py_VISIT(traverse_module_state->__pyx_n_s_stream_timestamp);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_n_s_timestamp);
   Py_VISIT(traverse_module_state->__pyx_n_s_timezone);
   Py_VISIT(traverse_module_state->__pyx_n_s_types);
-  Py_VISIT(traverse_module_state->__pyx_n_s_tzinfo);
   Py_VISIT(traverse_module_state->__pyx_n_s_utc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_utcfromtimestamp);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_uuid);
   Py_VISIT(traverse_module_state->__pyx_int_0);
   Py_VISIT(traverse_module_state->__pyx_int_10);
   Py_VISIT(traverse_module_state->__pyx_int_1000);
   Py_VISIT(traverse_module_state->__pyx_int_2147483648);
   Py_VISIT(traverse_module_state->__pyx_int_4294967295);
@@ -3380,14 +3372,15 @@
 #define __pyx_n_s_decode_amqp __pyx_mstate_global->__pyx_n_s_decode_amqp
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
 #define __pyx_n_s_encode __pyx_mstate_global->__pyx_n_s_encode
 #define __pyx_n_s_encode_amqp __pyx_mstate_global->__pyx_n_s_encode_amqp
 #define __pyx_n_s_error __pyx_mstate_global->__pyx_n_s_error
 #define __pyx_n_s_format __pyx_mstate_global->__pyx_n_s_format
+#define __pyx_n_s_fromtimestamp __pyx_mstate_global->__pyx_n_s_fromtimestamp
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get __pyx_mstate_global->__pyx_n_s_get
 #define __pyx_n_s_getLogger __pyx_mstate_global->__pyx_n_s_getLogger
 #define __pyx_n_s_get_message_ctx __pyx_mstate_global->__pyx_n_s_get_message_ctx
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
@@ -3408,15 +3401,14 @@
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_range __pyx_mstate_global->__pyx_n_s_range
 #define __pyx_n_s_rbfly_amqp__message __pyx_mstate_global->__pyx_n_s_rbfly_amqp__message
 #define __pyx_kp_s_rbfly_amqp__message_pyx __pyx_mstate_global->__pyx_kp_s_rbfly_amqp__message_pyx
 #define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
 #define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
-#define __pyx_n_s_replace __pyx_mstate_global->__pyx_n_s_replace
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_n_s_set __pyx_mstate_global->__pyx_n_s_set
 #define __pyx_n_s_set_message_ctx __pyx_mstate_global->__pyx_n_s_set_message_ctx
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
 #define __pyx_n_s_size __pyx_mstate_global->__pyx_n_s_size
@@ -3425,17 +3417,15 @@
 #define __pyx_n_s_stream_publish_id __pyx_mstate_global->__pyx_n_s_stream_publish_id
 #define __pyx_n_s_stream_timestamp __pyx_mstate_global->__pyx_n_s_stream_timestamp
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_n_s_timestamp __pyx_mstate_global->__pyx_n_s_timestamp
 #define __pyx_n_s_timezone __pyx_mstate_global->__pyx_n_s_timezone
 #define __pyx_n_s_types __pyx_mstate_global->__pyx_n_s_types
-#define __pyx_n_s_tzinfo __pyx_mstate_global->__pyx_n_s_tzinfo
 #define __pyx_n_s_utc __pyx_mstate_global->__pyx_n_s_utc
-#define __pyx_n_s_utcfromtimestamp __pyx_mstate_global->__pyx_n_s_utcfromtimestamp
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_uuid __pyx_mstate_global->__pyx_n_s_uuid
 #define __pyx_int_0 __pyx_mstate_global->__pyx_int_0
 #define __pyx_int_10 __pyx_mstate_global->__pyx_int_10
 #define __pyx_int_1000 __pyx_mstate_global->__pyx_int_1000
 #define __pyx_int_2147483648 __pyx_mstate_global->__pyx_int_2147483648
 #define __pyx_int_4294967295 __pyx_mstate_global->__pyx_int_4294967295
@@ -6885,195 +6875,185 @@
     break;
     case 0x83:
 
     /* "rbfly/amqp/_message.pyx":330
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_TIMESTAMP:
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))             # <<<<<<<<<<<<<<
- *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
+ *         body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:
  */
     __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, (sizeof(uint64_t))); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 330, __pyx_L1_error)
     __pyx_t_9 = __pyx_f_5rbfly_6_codec_unpack_uint64(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 330, __pyx_L1_error)
     __pyx_v_ts = ((uint64_t)__pyx_t_9);
 
     /* "rbfly/amqp/_message.pyx":331
  *     elif type_code == TYPE_TIMESTAMP:
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
- *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)             # <<<<<<<<<<<<<<
+ *         body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)             # <<<<<<<<<<<<<<
  *     elif type_code == TYPE_UUID:
  *         body = UUID(bytes=buffer_claim(buffer, 16)[:16])
  */
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_utcfromtimestamp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 331, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fromtimestamp); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = PyFloat_FromDouble((((double)__pyx_v_ts) / 1000.0)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_12 = NULL;
+    __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_datetime); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 331, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_timezone); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 331, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_13);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_13, __pyx_n_s_utc); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 331, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+    __pyx_t_13 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_12)) {
+      __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_13)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_12);
+        __Pyx_INCREF(__pyx_t_13);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+      PyObject *__pyx_callargs[3] = {__pyx_t_13, __pyx_t_3, __pyx_t_12};
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
       if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 331, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_replace); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_datetime); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_timezone); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_12, __pyx_n_s_utc); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_tzinfo, __pyx_t_3) < 0) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 331, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_body = __pyx_t_3;
-    __pyx_t_3 = 0;
+    __pyx_v_body = __pyx_t_1;
+    __pyx_t_1 = 0;
 
     /* "rbfly/amqp/_message.pyx":329
  *     elif type_code == TYPE_MAP32:
  *         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
  *     elif type_code == TYPE_TIMESTAMP:             # <<<<<<<<<<<<<<
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
- *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
+ *         body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)
  */
     break;
     case 0x98:
 
     /* "rbfly/amqp/_message.pyx":333
- *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
+ *         body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:
  *         body = UUID(bytes=buffer_claim(buffer, 16)[:16])             # <<<<<<<<<<<<<<
  *     else:
  *         raise AMQPDecoderError(
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_UUID); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 333, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 333, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_UUID); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 16); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 333, __pyx_L1_error)
-    __pyx_t_2 = __Pyx_PyBytes_FromStringAndSize(__pyx_t_6 + 0, 16 - 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 333, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_bytes, __pyx_t_2) < 0) __PYX_ERR(1, 333, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 333, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 333, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_6 = __pyx_f_5rbfly_7_buffer_buffer_claim(__pyx_v_buffer, 16); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 333, __pyx_L1_error)
+    __pyx_t_12 = __Pyx_PyBytes_FromStringAndSize(__pyx_t_6 + 0, 16 - 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 333, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_bytes, __pyx_t_12) < 0) __PYX_ERR(1, 333, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __pyx_t_12 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_empty_tuple, __pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 333, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_12);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_v_body = __pyx_t_2;
-    __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_v_body = __pyx_t_12;
+    __pyx_t_12 = 0;
 
     /* "rbfly/amqp/_message.pyx":332
  *         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
- *         body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
+ *         body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)
  *     elif type_code == TYPE_UUID:             # <<<<<<<<<<<<<<
  *         body = UUID(bytes=buffer_claim(buffer, 16)[:16])
  *     else:
  */
     break;
     default:
 
     /* "rbfly/amqp/_message.pyx":335
  *         body = UUID(bytes=buffer_claim(buffer, 16)[:16])
  *     else:
  *         raise AMQPDecoderError(             # <<<<<<<<<<<<<<
  *             'Cannot decode message, type code=0x{:02x}'.format(type_code)
  *         )
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 335, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_AMQPDecoderError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 335, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
 
     /* "rbfly/amqp/_message.pyx":336
  *     else:
  *         raise AMQPDecoderError(
  *             'Cannot decode message, type code=0x{:02x}'.format(type_code)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-    __pyx_t_12 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_type_code, __pyx_n_s_format); if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 336, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_12);
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_kp_u_Cannot_decode_message_type_code, __pyx_n_s_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 336, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_13 = __Pyx_PyInt_From_uint8_t(__pyx_v_type_code); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 336, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_13);
     __pyx_t_14 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (likely(PyMethod_Check(__pyx_t_12))) {
-      __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_12);
+    if (likely(PyMethod_Check(__pyx_t_3))) {
+      __pyx_t_14 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_14)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_12);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_14);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_12, function);
+        __Pyx_DECREF_SET(__pyx_t_3, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_14, __pyx_t_13};
-      __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 336, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_3);
-      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 336, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_12 = NULL;
+    __pyx_t_3 = NULL;
     __pyx_t_4 = 0;
     #if CYTHON_UNPACK_METHODS
-    if (unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_12)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_12);
+    if (unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_3)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
         __pyx_t_4 = 1;
       }
     }
     #endif
     {
-      PyObject *__pyx_callargs[2] = {__pyx_t_12, __pyx_t_3};
-      __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
-      __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 335, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
+      PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_1};
+      __pyx_t_12 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 1+__pyx_t_4);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_12)) __PYX_ERR(1, 335, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_12);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
-    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_12, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
     __PYX_ERR(1, 335, __pyx_L1_error)
     break;
   }
 
   /* "rbfly/amqp/_message.pyx":339
  *         )
  * 
@@ -10547,14 +10527,15 @@
     {&__pyx_n_s_decode_amqp, __pyx_k_decode_amqp, sizeof(__pyx_k_decode_amqp), 0, 0, 1, 1},
     {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
     {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
     {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
     {&__pyx_n_s_encode_amqp, __pyx_k_encode_amqp, sizeof(__pyx_k_encode_amqp), 0, 0, 1, 1},
     {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
     {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
+    {&__pyx_n_s_fromtimestamp, __pyx_k_fromtimestamp, sizeof(__pyx_k_fromtimestamp), 0, 0, 1, 1},
     {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
     {&__pyx_n_s_get, __pyx_k_get, sizeof(__pyx_k_get), 0, 0, 1, 1},
     {&__pyx_n_s_getLogger, __pyx_k_getLogger, sizeof(__pyx_k_getLogger), 0, 0, 1, 1},
     {&__pyx_n_s_get_message_ctx, __pyx_k_get_message_ctx, sizeof(__pyx_k_get_message_ctx), 0, 0, 1, 1},
     {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
@@ -10575,15 +10556,14 @@
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
     {&__pyx_n_s_rbfly_amqp__message, __pyx_k_rbfly_amqp__message, sizeof(__pyx_k_rbfly_amqp__message), 0, 0, 1, 1},
     {&__pyx_kp_s_rbfly_amqp__message_pyx, __pyx_k_rbfly_amqp__message_pyx, sizeof(__pyx_k_rbfly_amqp__message_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-    {&__pyx_n_s_replace, __pyx_k_replace, sizeof(__pyx_k_replace), 0, 0, 1, 1},
     {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
     {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
     {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
     {&__pyx_n_s_set_message_ctx, __pyx_k_set_message_ctx, sizeof(__pyx_k_set_message_ctx), 0, 0, 1, 1},
     {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
     {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
@@ -10592,17 +10572,15 @@
     {&__pyx_n_s_stream_publish_id, __pyx_k_stream_publish_id, sizeof(__pyx_k_stream_publish_id), 0, 0, 1, 1},
     {&__pyx_n_s_stream_timestamp, __pyx_k_stream_timestamp, sizeof(__pyx_k_stream_timestamp), 0, 0, 1, 1},
     {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
     {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
     {&__pyx_n_s_timestamp, __pyx_k_timestamp, sizeof(__pyx_k_timestamp), 0, 0, 1, 1},
     {&__pyx_n_s_timezone, __pyx_k_timezone, sizeof(__pyx_k_timezone), 0, 0, 1, 1},
     {&__pyx_n_s_types, __pyx_k_types, sizeof(__pyx_k_types), 0, 0, 1, 1},
-    {&__pyx_n_s_tzinfo, __pyx_k_tzinfo, sizeof(__pyx_k_tzinfo), 0, 0, 1, 1},
     {&__pyx_n_s_utc, __pyx_k_utc, sizeof(__pyx_k_utc), 0, 0, 1, 1},
-    {&__pyx_n_s_utcfromtimestamp, __pyx_k_utcfromtimestamp, sizeof(__pyx_k_utcfromtimestamp), 0, 0, 1, 1},
     {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
     {&__pyx_n_s_uuid, __pyx_k_uuid, sizeof(__pyx_k_uuid), 0, 0, 1, 1},
     {0, 0, 0, 0, 0, 0, 0}
   };
   return __Pyx_InitStrings(__pyx_string_tab);
 }
 /* #### Code section: cached_builtins ### */
```

### Comparing `rbfly-0.8.3/rbfly/amqp/_message.pxd` & `rbfly-0.8.4/rbfly/amqp/_message.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/amqp/_message.pyi` & `rbfly-0.8.4/rbfly/amqp/_message.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/amqp/_message.pyx` & `rbfly-0.8.4/rbfly/amqp/_message.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         body = _decode_compound(_decode_list, _decode_compound_size32, buffer)
     elif type_code == TYPE_MAP8:
         body = _decode_compound(_decode_map, _decode_compound_size8, buffer)
     elif type_code == TYPE_MAP32:
         body = _decode_compound(_decode_map, _decode_compound_size32, buffer)
     elif type_code == TYPE_TIMESTAMP:
         ts = <uint64_t> unpack_uint64(buffer_claim(buffer, sizeof(uint64_t)))
-        body = datetime.datetime.utcfromtimestamp(ts / 1000.0).replace(tzinfo=datetime.timezone.utc)
+        body = datetime.datetime.fromtimestamp(ts / 1000.0, datetime.timezone.utc)
     elif type_code == TYPE_UUID:
         body = UUID(bytes=buffer_claim(buffer, 16)[:16])
     else:
         raise AMQPDecoderError(
             'Cannot decode message, type code=0x{:02x}'.format(type_code)
         )
```

### Comparing `rbfly-0.8.3/rbfly/cm.py` & `rbfly-0.8.4/rbfly/cm.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/error.py` & `rbfly-0.8.4/rbfly/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/slotmap.py` & `rbfly-0.8.4/rbfly/slotmap.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/__init__.py` & `rbfly-0.8.4/rbfly/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_client.c` & `rbfly-0.8.4/rbfly/streams/_client.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_client.pyi` & `rbfly-0.8.4/rbfly/streams/_client.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_client.pyx` & `rbfly-0.8.4/rbfly/streams/_client.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_codec.c` & `rbfly-0.8.4/rbfly/streams/_codec.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_codec.pyi` & `rbfly-0.8.4/rbfly/streams/_codec.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_codec.pyx` & `rbfly-0.8.4/rbfly/streams/_codec.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_mqueue.c` & `rbfly-0.8.4/rbfly/streams/_mqueue.c`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_mqueue.pxd` & `rbfly-0.8.4/rbfly/streams/_mqueue.pxd`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_mqueue.pyi` & `rbfly-0.8.4/rbfly/streams/_mqueue.pyi`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/_mqueue.pyx` & `rbfly-0.8.4/rbfly/streams/_mqueue.pyx`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/client.py` & `rbfly-0.8.4/rbfly/streams/client.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/codec.py` & `rbfly-0.8.4/rbfly/streams/codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/const.py` & `rbfly-0.8.4/rbfly/streams/const.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/error.py` & `rbfly-0.8.4/rbfly/streams/error.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/offset.py` & `rbfly-0.8.4/rbfly/streams/offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/protocol.py` & `rbfly-0.8.4/rbfly/streams/protocol.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/types.py` & `rbfly-0.8.4/rbfly/streams/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/streams/util.py` & `rbfly-0.8.4/rbfly/streams/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/__init__.py` & `rbfly-0.8.4/rbfly/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/amqp/__init__.py` & `rbfly-0.8.4/rbfly/tests/amqp/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/amqp/test_message.py` & `rbfly-0.8.4/rbfly/tests/amqp/test_message.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/streams/__init__.py` & `rbfly-0.8.4/rbfly/tests/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/streams/test_client.py` & `rbfly-0.8.4/rbfly/tests/streams/test_client.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/streams/test_codec.py` & `rbfly-0.8.4/rbfly/tests/streams/test_codec.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/streams/test_mqueue.py` & `rbfly-0.8.4/rbfly/tests/streams/test_mqueue.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/streams/test_offset.py` & `rbfly-0.8.4/rbfly/tests/streams/test_offset.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/test_slotmap.py` & `rbfly-0.8.4/rbfly/tests/test_slotmap.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/tests/test_util.py` & `rbfly-0.8.4/rbfly/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/types.py` & `rbfly-0.8.4/rbfly/types.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly/util.py` & `rbfly-0.8.4/rbfly/util.py`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/rbfly.egg-info/PKG-INFO` & `rbfly-0.8.4/rbfly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbfly
-Version: 0.8.3
+Version: 0.8.4
 Summary: RbFly - a library for RabbitMQ Streams using Python asyncio
 Home-page: https://wrobell.dcmod.org/rbfly/
 Author: Artur Wroblewski
 Author-email: wrobell@riseup.net
 License: GPLv3+
 Project-URL: Source Code, https://gitlab.com/wrobell/rbfly
 Project-URL: Bug tracker, https://gitlab.com/wrobell/rbfly/issues
@@ -27,15 +27,15 @@
 Requires-Dist: ruff>=0.3.0; extra == "tests"
 Requires-Dist: toml; extra == "tests"
 Requires-Dist: uvloop>=0.19.0; extra == "tests"
 Provides-Extra: performance
 Requires-Dist: msgpack; extra == "performance"
 Requires-Dist: aiokafka==0.8.1; extra == "performance"
 Requires-Dist: rstream==0.13.0; extra == "performance"
-Requires-Dist: uamqp==1.6.5; extra == "performance"
+Requires-Dist: uamqp==1.6.9; extra == "performance"
 Requires-Dist: python-qpid-proton==0.39.0; extra == "performance"
 Provides-Extra: doc
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 
 RbFly is a library for RabbitMQ Streams using Python asyncio
 
 - https://www.rabbitmq.com/streams.html
```

### Comparing `rbfly-0.8.3/rbfly.egg-info/SOURCES.txt` & `rbfly-0.8.4/rbfly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rbfly-0.8.3/setup.cfg` & `rbfly-0.8.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rbfly
-version = 0.8.3
+version = 0.8.4
 author = Artur Wroblewski
 author_email = wrobell@riseup.net
 license = GPLv3+
 description = RbFly - a library for RabbitMQ Streams using Python asyncio
 long_description = file: README
 long_description_content_type = text/x-rst
 url = https://wrobell.dcmod.org/rbfly/
@@ -43,15 +43,15 @@
 	ruff >= 0.3.0
 	toml  # required by bandit, not needed when using Python 3.11?
 	uvloop >= 0.19.0
 performance = 
 	msgpack
 	aiokafka == 0.8.1
 	rstream == 0.13.0
-	uamqp == 1.6.5
+	uamqp == 1.6.9
 	python-qpid-proton == 0.39.0
 doc = 
 	sphinx_rtd_theme
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rbfly-0.8.3/setup.py` & `rbfly-0.8.4/setup.py`

 * *Files identical despite different names*

