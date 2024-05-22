# Comparing `tmp/superblocks-agent-0.0.7.tar.gz` & `tmp/superblocks-agent-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-agent-0.0.7.tar", last modified: Wed May 22 13:11:18 2024, max compression
+gzip compressed data, was "superblocks-agent-0.0.8.tar", last modified: Wed May 22 16:03:20 2024, max compression
```

## Comparing `superblocks-agent-0.0.7.tar` & `superblocks-agent-0.0.8.tar`

### file list

```diff
@@ -1,67 +1,65 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.666845 superblocks-agent-0.0.7/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.7/LICENSE
--rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.7/MANIFEST.in
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 13:11:18.666604 superblocks-agent-0.0.7/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-20 13:15:54.000000 superblocks-agent-0.0.7/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.7/pyproject.toml
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-21 18:02:15.000000 superblocks-agent-0.0.7/requirements.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-22 13:11:18.666920 superblocks-agent-0.0.7/setup.cfg
--rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.7/setup.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.652389 superblocks-agent-0.0.7/superblocks_agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.7/superblocks_agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.654568 superblocks-agent-0.0.7/superblocks_agent/_type/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_type/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_type/client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      265 2024-05-21 18:56:05.000000 superblocks-agent-0.0.7/superblocks_agent/_type/mock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.655486 superblocks-agent-0.0.7/superblocks_agent/_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/generate.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-22 13:10:57.000000 superblocks-agent-0.0.7/superblocks_agent/_version.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.657109 superblocks-agent-0.0.7/superblocks_agent/core/
--rw-r--r--   0 joeygreco   (501) staff       (20)     6635 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/core/Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1444 2024-05-21 19:23:48.000000 superblocks-agent-0.0.7/superblocks_agent/core/Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2755 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/core/_StepMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       64 2024-05-21 18:47:59.000000 superblocks-agent-0.0.7/superblocks_agent/core/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.658324 superblocks-agent-0.0.7/superblocks_agent/enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1058 2024-05-21 18:53:18.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/ViewMode.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-21 18:54:58.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/_BaseEnum.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       39 2024-05-21 18:53:29.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.661907 superblocks-agent-0.0.7/superblocks_agent/model/
--rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/Agent.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      725 2024-05-21 18:54:49.000000 superblocks-agent-0.0.7/superblocks_agent/model/ApiConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      310 2024-05-21 19:03:38.000000 superblocks-agent-0.0.7/superblocks_agent/model/ApiResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/Auth.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      238 2024-05-21 19:06:08.000000 superblocks-agent-0.0.7/superblocks_agent/model/ClientConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/ExecutionError.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1839 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/model/ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      389 2024-05-21 19:19:09.000000 superblocks-agent-0.0.7/superblocks_agent/model/StepResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1024 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/model/_MockStepFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      340 2024-05-21 19:18:26.000000 superblocks-agent-0.0.7/superblocks_agent/model/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.662856 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/
--rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-21 19:23:31.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/BaseMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/MockFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.653791 superblocks-agent-0.0.7/superblocks_agent.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1774 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/requires.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.649959 superblocks-agent-0.0.7/test_unit/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.663848 superblocks-agent-0.0.7/test_unit/test_core/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_core/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8672 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_core/test_Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      912 2024-05-21 19:06:08.000000 superblocks-agent-0.0.7/test_unit/test_core/test_Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4270 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_core/test_StepMock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.664380 superblocks-agent-0.0.7/test_unit/test_enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_enumeration/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1391 2024-05-21 18:54:37.000000 superblocks-agent-0.0.7/test_unit/test_enumeration/test_ViewMode.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.665357 superblocks-agent-0.0.7/test_unit/test_model/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_model/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2450 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_model/test_ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      790 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_model/test_MockStepFilters.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.666126 superblocks-agent-0.0.7/test_unit/test_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-21 19:24:53.000000 superblocks-agent-0.0.7/test_unit/test_util/test_convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-21 19:24:37.000000 superblocks-agent-0.0.7/test_unit/test_util/test_generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.594041 superblocks-agent-0.0.8/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/LICENSE
+-rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/MANIFEST.in
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 16:03:20.593856 superblocks-agent-0.0.8/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/pyproject.toml
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/requirements.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-22 16:03:20.594113 superblocks-agent-0.0.8/setup.cfg
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/setup.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.578521 superblocks-agent-0.0.8/superblocks_agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.582405 superblocks-agent-0.0.8/superblocks_agent/_type/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-22 15:51:41.000000 superblocks-agent-0.0.8/superblocks_agent/_type/BaseEnum.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      452 2024-05-22 15:23:31.000000 superblocks-agent-0.0.8/superblocks_agent/_type/BaseMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-22 15:51:41.000000 superblocks-agent-0.0.8/superblocks_agent/_type/MockFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_type/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_type/client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      232 2024-05-22 15:23:21.000000 superblocks-agent-0.0.8/superblocks_agent/_type/mock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.583083 superblocks-agent-0.0.8/superblocks_agent/_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_util/convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-22 15:23:54.000000 superblocks-agent-0.0.8/superblocks_agent/_util/generate.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-22 16:03:13.000000 superblocks-agent-0.0.8/superblocks_agent/_version.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.585274 superblocks-agent-0.0.8/superblocks_agent/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7018 2024-05-22 15:59:11.000000 superblocks-agent-0.0.8/superblocks_agent/api/Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      735 2024-05-22 15:59:59.000000 superblocks-agent-0.0.8/superblocks_agent/api/Config.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/api/ExecutionError.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1939 2024-05-22 16:00:09.000000 superblocks-agent-0.0.8/superblocks_agent/api/ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      293 2024-05-22 16:00:40.000000 superblocks-agent-0.0.8/superblocks_agent/api/Result.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1051 2024-05-22 15:27:02.000000 superblocks-agent-0.0.8/superblocks_agent/api/ViewMode.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      242 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.586248 superblocks-agent-0.0.8/superblocks_agent/client/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1421 2024-05-22 15:50:24.000000 superblocks-agent-0.0.8/superblocks_agent/client/Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      187 2024-05-22 15:27:31.000000 superblocks-agent-0.0.8/superblocks_agent/client/Config.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       70 2024-05-22 15:13:14.000000 superblocks-agent-0.0.8/superblocks_agent/client/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.586670 superblocks-agent-0.0.8/superblocks_agent/step/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-22 15:36:18.000000 superblocks-agent-0.0.8/superblocks_agent/step/Result.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       35 2024-05-22 15:19:35.000000 superblocks-agent-0.0.8/superblocks_agent/step/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.587481 superblocks-agent-0.0.8/superblocks_agent/testing/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1014 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/testing/_MockStepFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2747 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/testing/_StepMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       34 2024-05-22 15:15:15.000000 superblocks-agent-0.0.8/superblocks_agent/testing/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.579726 superblocks-agent-0.0.8/superblocks_agent.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1633 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/requires.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.576333 superblocks-agent-0.0.8/test_unit/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.589605 superblocks-agent-0.0.8/test_unit/test_api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:29:27.000000 superblocks-agent-0.0.8/test_unit/test_api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8796 2024-05-22 16:02:27.000000 superblocks-agent-0.0.8/test_unit/test_api/test_Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2535 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/test_unit/test_api/test_ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1383 2024-05-22 15:33:26.000000 superblocks-agent-0.0.8/test_unit/test_api/test_ViewMode.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.591990 superblocks-agent-0.0.8/test_unit/test_client/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:04.000000 superblocks-agent-0.0.8/test_unit/test_client/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      800 2024-05-22 16:02:27.000000 superblocks-agent-0.0.8/test_unit/test_client/test_Client.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.592904 superblocks-agent-0.0.8/test_unit/test_testing/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:42.000000 superblocks-agent-0.0.8/test_unit/test_testing/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      792 2024-05-22 15:32:24.000000 superblocks-agent-0.0.8/test_unit/test_testing/test_MockStepFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4275 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/test_unit/test_testing/test_StepMock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.593547 superblocks-agent-0.0.8/test_unit/test_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/test_convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.7/LICENSE` & `superblocks-agent-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.7/PKG-INFO` & `superblocks-agent-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.7/README.md` & `superblocks-agent-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.7/setup.py` & `superblocks-agent-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.7/superblocks_agent/_util/convert.py` & `superblocks-agent-0.0.8/superblocks_agent/_util/convert.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.7/superblocks_agent/core/Api.py` & `superblocks-agent-0.0.8/superblocks_agent/api/Api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# TODO: (joey) some of these imports are weird
+
 from typing import Optional
 
 from superblocks_types.api.v1.service_pb2 import (
     ExecuteRequest,
     Function,
     StreamResponse,
     TwoWayRequest,
@@ -9,17 +11,19 @@
 )
 from superblocks_types.api.v1.service_pb2_grpc import ExecutorServiceStub
 from superblocks_types.common.v1.common_pb2 import Profile
 from superblocks_types.common.v1.errors_pb2 import Error
 
 from superblocks_agent._util.convert import from_protobuf_value, to_protobuf_value
 from superblocks_agent._util.generate import get_unique_id_for_object
-from superblocks_agent.core import Client
-from superblocks_agent.core._StepMock import StepMock
-from superblocks_agent.model import ApiConfig, ExecutionResult
+from superblocks_agent.api.Config import Config as ApiConfig
+from superblocks_agent.api.ExecutionResult import ExecutionResult
+from superblocks_agent.client import Client
+from superblocks_agent.client import Config as ClientConfig
+from superblocks_agent.testing._StepMock import StepMock
 
 
 class Api:
     def __init__(self, api_id: str, *, config: Optional[ApiConfig] = None):
         self.__api_id = api_id
         self.__config = config
         self.mock_func_lookup: dict[str, callable] = {}
@@ -40,15 +44,17 @@
         # hydrate mock lookup dict so we can reference it later
         self.__hydrate_mock_func_lookup(mocks)
 
         stream_responses = await client.run(
             with_stub=ExecutorServiceStub,
             stub_func_name="TwoWayStream",
             initial_request=TwoWayRequest(
-                execute=self.__build_execute_request(inputs=inputs, mocks=mocks)
+                execute=self.__build_execute_request(
+                    inputs=inputs, mocks=mocks, client_config=client.config
+                )
             ),
             response_handler=self.__get_handle_two_way_response_func(),
         )
         return ExecutionResult.from_proto_stream_responses(stream_responses)
 
     def __hydrate_mock_func_lookup(self, mocks: list[StepMock]) -> None:
         """
@@ -107,15 +113,17 @@
                 case _ if response.HasField("stream"):
                     return None, response
                 case _:
                     raise Exception(f"got unexpected type: {type(response)}")
 
         return handle_two_way_response
 
-    def __build_execute_request(self, *, inputs: dict, mocks: list[StepMock]) -> ExecuteRequest:
+    def __build_execute_request(
+        self, *, inputs: dict, mocks: list[StepMock], client_config: ClientConfig
+    ) -> ExecuteRequest:
         """
         Returns a hydrated ExecuteRequest object.
         """
         execute_request = ExecuteRequest()
         for input_key, input_value in inputs.items():
             value = to_protobuf_value(input_value)
             execute_request.inputs[input_key].CopyFrom(value)
@@ -129,24 +137,25 @@
         # NOTE: (joey) do we need to set any other ExecuteRequest.Options fields?
 
         # set inputs
         for k, v in inputs.items():
             execute_request.inputs[k].CopyFrom(to_protobuf_value(v))
 
         # set fetch
-        execute_request.fetch.CopyFrom(self.__to_proto_fetch())
+        execute_request.fetch.CopyFrom(self.__to_proto_fetch(client_config))
 
         return execute_request
 
-    def __to_proto_fetch(self) -> ExecuteRequest.Fetch:
+    def __to_proto_fetch(self, client_config: ClientConfig) -> ExecuteRequest.Fetch:
         """
         Returns a hydrated Fetch object to be used in an ExecuteRequest.
         """
         fetch = ExecuteRequest.Fetch()
         fetch.id = self.__api_id
+        fetch.token = f"Bearer {client_config.token}"
         if self.__config is not None:
             if self.__config.profile_name is not None:
                 profile = Profile()
                 profile.name = self.__config.profile_name
                 fetch.profile.CopyFrom(profile)
             if self.__config.view_mode is not None:
                 fetch.view_mode = self.__config.view_mode.to_proto_view_mode()
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/core/Client.py` & `superblocks-agent-0.0.8/superblocks_agent/client/Client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import queue
 
 import grpc
 from superblocks_types.api.v1.service_pb2 import StreamResponse
 
 from superblocks_agent._type.client import TwoWayStreamResponseHandler
-from superblocks_agent.model import ClientConfig
+from superblocks_agent.client import Config
 
 
 class Client:
-    def __init__(self, config: ClientConfig):
-        self.__config = config
+    def __init__(self, config: Config):
+        self.config = config
 
     async def run(
         self,
         *,
         with_stub: object,
         stub_func_name: str,
         initial_request: object,
         response_handler: TwoWayStreamResponseHandler,
     ) -> list[StreamResponse]:
         # TODO: (joey) throw clear errors here for auth/connection issues
-        stub = with_stub(channel=grpc.insecure_channel(target=self.__config.agent.endpoint))
+        stub = with_stub(channel=grpc.insecure_channel(target=self.config.endpoint))
         stub_function = getattr(stub, stub_func_name)
 
         stream_responses = []
         q = queue.Queue()
 
         q.put(initial_request)
 
-        def get_responses():
+        def get_requests():
             while True:
                 yield q.get()
 
         try:
-            responses = stub_function(get_responses())
+            responses = stub_function(get_requests())
 
             for response in responses:
                 next_request, two_way_response = response_handler(response)
                 if two_way_response is not None:
                     stream_responses.append(two_way_response.stream)
                 if next_request is not None:
                     q.put(next_request)
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/core/_StepMock.py` & `superblocks-agent-0.0.8/superblocks_agent/testing/_StepMock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from typing import Optional
 
 from superblocks_types.api.v1.service_pb2 import Mock
 
+from superblocks_agent._type.BaseMock import BaseMock
 from superblocks_agent._type.mock import FilteredDictCallable, WhenCallable
 from superblocks_agent._util.convert import Mock_, to_protobuf_value
 from superblocks_agent._util.generate import get_unique_id_for_object
-from superblocks_agent.model._abstract.BaseMock import BaseMock
-from superblocks_agent.model._MockStepFilters import MockStepFilters
+from superblocks_agent.testing._MockStepFilters import MockStepFilters
 
 
 class StepMock(BaseMock):
     def __init__(
         self, filters: Optional[MockStepFilters] = None, *, when: Optional[WhenCallable] = None
     ):
         self.__on_filters = filters
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/enumeration/ViewMode.py` & `superblocks-agent-0.0.8/superblocks_agent/api/ViewMode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from superblocks_types.api.v1.service_pb2 import ViewMode as ViewModeProto
 
-from superblocks_agent.enumeration._BaseEnum import BaseEnum
+from superblocks_agent._type.BaseEnum import BaseEnum
 
 
 class ViewMode(BaseEnum):
     DEPLOYED = "deployed"
     EDITOR = "editor"
     PREVIEW = "preview"
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/model/ApiConfig.py` & `superblocks-agent-0.0.8/superblocks_agent/api/Config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from __future__ import annotations
+# TODO: (joey) some of these imports are weird
 
 from dataclasses import dataclass
 from typing import Optional
 
-from superblocks_agent.enumeration import ViewMode
+from superblocks_agent.api.ViewMode import ViewMode
 
 
 @dataclass(kw_only=True, eq=False)
-class ApiConfig:
+class Config:
     # The application id used to provide a default scope.
     application_id: Optional[str] = None
     # The default branch to use.
     branch_name: Optional[str] = None
     # The id of the commit to use.
     commit_id: Optional[str] = None
     # The default profile to use. If not set, the default for view_mode will be used.
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/model/ExecutionResult.py` & `superblocks-agent-0.0.8/superblocks_agent/api/ExecutionResult.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+# TODO: (joey) some of these imports are weird
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 from superblocks_types.api.v1.event_pb2 import BlockStatus
 from superblocks_types.api.v1.service_pb2 import StreamResponse
 
 from superblocks_agent._util.convert import from_protobuf_value
-from superblocks_agent.model import ApiResult, ExecutionError, StepResult
+from superblocks_agent.api.ExecutionError import ExecutionError
+from superblocks_agent.api.Result import Result as ApiResult
+from superblocks_agent.step import Result as StepResult
 
 
 @dataclass(kw_only=True)
 class ExecutionResult:
     step_results: list[StepResult] = field(default_factory=list)
     api_result: ApiResult = field(default_factory=ApiResult)
 
@@ -27,15 +30,14 @@
                 step_error = None
                 if stream_response.event.end.is_response_block:
                     api_output = from_protobuf_value(stream_response.event.end.output.result)
                 if stream_response.event.end.status == BlockStatus.BLOCK_STATUS_ERRORED:
                     api_error = step_error = ExecutionError.from_proto_error(
                         stream_response.event.end.error
                     )
-                # TODO: (joey) no "." here
                 step_results.append(
-                    StepResult.StepResult(
+                    StepResult(
                         step_name=stream_response.event.name, output=step_output, error=step_error
                     )
                 )
         api_result = ApiResult(output=api_output, error=api_error)
         return ExecutionResult(step_results=step_results, api_result=api_result)
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent/model/_MockStepFilters.py` & `superblocks-agent-0.0.8/superblocks_agent/testing/_MockStepFilters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
 from superblocks_types.api.v1.service_pb2 import Mock
 
+from superblocks_agent._type.MockFilters import MockFilters
 from superblocks_agent._util.convert import to_protobuf_value
-from superblocks_agent.model._abstract.MockFilters import MockFilters
 
 
 @dataclass(kw_only=True)
 class MockStepFilters(MockFilters):
     # Filter on integrations with this type
     integration_type: Optional[str] = None
     # Filter on steps with this name
```

### Comparing `superblocks-agent-0.0.7/superblocks_agent.egg-info/PKG-INFO` & `superblocks-agent-0.0.8/superblocks_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.7
+Version: 0.0.8
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_core/test_Api.py` & `superblocks-agent-0.0.8/test_unit/test_api/test_Api.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,28 +12,28 @@
     TwoWayResponse,
 )
 from superblocks_types.common.v1.common_pb2 import Profile
 from superblocks_types.common.v1.errors_pb2 import Error
 
 from superblocks_agent._util.convert import Mock_, to_protobuf_value
 from superblocks_agent._util.generate import get_unique_id_for_object
-from superblocks_agent.core import Api, Client
-from superblocks_agent.core._StepMock import StepMock
-from superblocks_agent.enumeration import ViewMode
-from superblocks_agent.model import Agent, ApiConfig, Auth, ClientConfig
-from superblocks_agent.model._MockStepFilters import MockStepFilters
+from superblocks_agent.api import Api
+from superblocks_agent.api import Config as ApiConfig
+from superblocks_agent.api import ViewMode
+from superblocks_agent.client import Client
+from superblocks_agent.client import Config as ClientConfig
+from superblocks_agent.testing._MockStepFilters import MockStepFilters
+from superblocks_agent.testing._StepMock import StepMock
 
 
 class TestApi(unittest.TestCase):
     def test_bad_connection_info(self):
         with self.assertRaises(Exception) as context:
             asyncio.run(
-                Api(api_id="").run(
-                    client=Client(ClientConfig(agent=Agent(endpoint=""), auth=Auth(token="")))
-                )
+                Api(api_id="").run(client=Client(config=ClientConfig(endpoint="", token="")))
             )
         self.assertIsInstance(context.exception, grpc._channel._MultiThreadedRendezvous)
 
     def test_build_execute_request(self):
         when_callable = lambda _: True
         api = Api(
             "api_id",
@@ -60,14 +60,15 @@
                 "int_var": 1,
                 "bool_var": True,
                 "list_var": ["foo", 1, True, {}, []],
                 "dict_var": {"foo": "bar"},
                 "null_var": None,
             },
             mocks=[api_mock],
+            client_config=ClientConfig(endpoint="", token="token"),
         )
 
         expected = ExecuteRequest(
             inputs={
                 "str_var": to_protobuf_value("foo"),
                 "int_var": to_protobuf_value(1),
                 "bool_var": to_protobuf_value(True),
@@ -78,14 +79,15 @@
             options=ExecuteRequest.Options(include_event_outputs=True, include_events=True),
             fetch=ExecuteRequest.Fetch(
                 id="api_id",
                 profile=Profile(name="profile_name"),
                 view_mode=ViewMode.DEPLOYED.to_proto_view_mode(),
                 commit_id="commit_id",
                 branch_name="branch_name",
+                token="Bearer token",
             ),
             mocks=[
                 Mock_(
                     on=Mock.On(
                         static=Mock.Params(
                             integration_type="integration_type",
                             step_name="step_name",
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_core/test_Client.py` & `superblocks-agent-0.0.8/test_unit/test_client/test_Client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import asyncio
 import unittest
 
 import grpc
 from superblocks_types.api.v1.service_pb2_grpc import ExecutorServiceStub
 
-from superblocks_agent.core import Client
-from superblocks_agent.model import Agent, Auth, ClientConfig
+from superblocks_agent.client import Client, Config
 
 
 class TestClient(unittest.TestCase):
     def test_init(self):
-        Client(ClientConfig(agent=Agent(endpoint=""), auth=Auth(token="")))
+        Client(Config(endpoint="", token=""))
 
     def test_bad_connection_info(self):
-        client = Client(ClientConfig(agent=Agent(endpoint=""), auth=Auth(token="")))
+        client = Client(Config(endpoint="", token=""))
         with self.assertRaises(Exception) as context:
             asyncio.run(
                 client.run(
                     with_stub=ExecutorServiceStub,
                     stub_func_name="TwoWayStream",
                     initial_request={},
                     response_handler=lambda _: True,
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_core/test_StepMock.py` & `superblocks-agent-0.0.8/test_unit/test_testing/test_StepMock.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 from superblocks_types.api.v1.service_pb2 import Mock
 
 from superblocks_agent._util.convert import Mock_, to_protobuf_value
 from superblocks_agent._util.generate import get_unique_id_for_object
-from superblocks_agent.core._StepMock import StepMock, on
-from superblocks_agent.model._MockStepFilters import MockStepFilters
+from superblocks_agent.testing._MockStepFilters import MockStepFilters
+from superblocks_agent.testing._StepMock import StepMock, on
 
 
 class TestStepMock(unittest.TestCase):
     def test_return_(self):
         # overwrites existing return val
         api_mock = StepMock().return_({"old": "value"})
         self.assertEqual({"old": "value"}, api_mock.get_return_value())
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_enumeration/test_ViewMode.py` & `superblocks-agent-0.0.8/test_unit/test_api/test_ViewMode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from aenum import extend_enum
 from superblocks_types.api.v1.service_pb2 import ViewMode as ViewModeProto
 
-from superblocks_agent.enumeration import ViewMode
+from superblocks_agent.api import ViewMode
 
 
 class TestViewMode(unittest.TestCase):
     def test_items(self):
         self.assertEqual(
             [
                 (ViewMode.DEPLOYED, "DEPLOYED"),
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_model/test_ExecutionResult.py` & `superblocks-agent-0.0.8/test_unit/test_api/test_ExecutionResult.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import unittest
 
 from superblocks_types.api.v1.event_pb2 import BlockStatus, Event, Output
 from superblocks_types.api.v1.service_pb2 import StreamResponse
 from superblocks_types.common.v1.errors_pb2 import Error
 
 from superblocks_agent._util.convert import to_protobuf_value
-from superblocks_agent.model import ApiResult, ExecutionError, ExecutionResult, StepResult
+from superblocks_agent.api import ExecutionError, ExecutionResult
+from superblocks_agent.api import Result as ApiResult
+from superblocks_agent.step import Result as StepResult
 
 
 class TestExecutionResult(unittest.TestCase):
     def test_from_proto_stream_responses__empty_list(self):
         actual = ExecutionResult.from_proto_stream_responses([])
         self.assertEqual(ExecutionResult(step_results=[], api_result=ApiResult()), actual)
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_model/test_MockStepFilters.py` & `superblocks-agent-0.0.8/test_unit/test_testing/test_MockStepFilters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from superblocks_types.api.v1.service_pb2 import Mock
 
 from superblocks_agent._util.convert import to_protobuf_value
-from superblocks_agent.model._MockStepFilters import MockStepFilters
+from superblocks_agent.testing._MockStepFilters import MockStepFilters
 
 
 class TestMockStepFilters(unittest.TestCase):
     def test_to_proto_params(self):
         self.assertEqual(Mock.Params(), MockStepFilters().to_proto_params())
         self.assertEqual(
             Mock.Params(
```

### Comparing `superblocks-agent-0.0.7/test_unit/test_util/test_convert.py` & `superblocks-agent-0.0.8/test_unit/test_util/test_convert.py`

 * *Files identical despite different names*

