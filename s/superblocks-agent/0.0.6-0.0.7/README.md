# Comparing `tmp/superblocks-agent-0.0.6.tar.gz` & `tmp/superblocks-agent-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-agent-0.0.6.tar", last modified: Tue May 21 19:26:48 2024, max compression
+gzip compressed data, was "superblocks-agent-0.0.7.tar", last modified: Wed May 22 13:11:18 2024, max compression
```

## Comparing `superblocks-agent-0.0.6.tar` & `superblocks-agent-0.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.415529 superblocks-agent-0.0.6/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.6/LICENSE
--rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.6/MANIFEST.in
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-21 19:26:48.415351 superblocks-agent-0.0.6/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-20 13:15:54.000000 superblocks-agent-0.0.6/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.6/pyproject.toml
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-21 18:02:15.000000 superblocks-agent-0.0.6/requirements.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-21 19:26:48.415592 superblocks-agent-0.0.6/setup.cfg
--rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.6/setup.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.402732 superblocks-agent-0.0.6/superblocks_agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.6/superblocks_agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.404623 superblocks-agent-0.0.6/superblocks_agent/_type/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/_type/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/_type/client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      265 2024-05-21 18:56:05.000000 superblocks-agent-0.0.6/superblocks_agent/_type/mock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.405515 superblocks-agent-0.0.6/superblocks_agent/_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/_util/convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/_util/generate.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-21 19:26:35.000000 superblocks-agent-0.0.6/superblocks_agent/_version.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.406888 superblocks-agent-0.0.6/superblocks_agent/core/
--rw-r--r--   0 joeygreco   (501) staff       (20)     6635 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/superblocks_agent/core/Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1444 2024-05-21 19:23:48.000000 superblocks-agent-0.0.6/superblocks_agent/core/Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2755 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/superblocks_agent/core/_StepMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       64 2024-05-21 18:47:59.000000 superblocks-agent-0.0.6/superblocks_agent/core/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.407842 superblocks-agent-0.0.6/superblocks_agent/enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1058 2024-05-21 18:53:18.000000 superblocks-agent-0.0.6/superblocks_agent/enumeration/ViewMode.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-21 18:54:58.000000 superblocks-agent-0.0.6/superblocks_agent/enumeration/_BaseEnum.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       39 2024-05-21 18:53:29.000000 superblocks-agent-0.0.6/superblocks_agent/enumeration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.410968 superblocks-agent-0.0.6/superblocks_agent/model/
--rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/model/Agent.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      725 2024-05-21 18:54:49.000000 superblocks-agent-0.0.6/superblocks_agent/model/ApiConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      310 2024-05-21 19:03:38.000000 superblocks-agent-0.0.6/superblocks_agent/model/ApiResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/model/Auth.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      238 2024-05-21 19:06:08.000000 superblocks-agent-0.0.6/superblocks_agent/model/ClientConfig.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/model/ExecutionError.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1839 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/superblocks_agent/model/ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      389 2024-05-21 19:19:09.000000 superblocks-agent-0.0.6/superblocks_agent/model/StepResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1024 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/superblocks_agent/model/_MockStepFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      340 2024-05-21 19:18:26.000000 superblocks-agent-0.0.6/superblocks_agent/model/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.411911 superblocks-agent-0.0.6/superblocks_agent/model/_abstract/
--rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-21 19:23:31.000000 superblocks-agent-0.0.6/superblocks_agent/model/_abstract/BaseMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/model/_abstract/MockFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.6/superblocks_agent/model/_abstract/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.403866 superblocks-agent-0.0.6/superblocks_agent.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-21 19:26:48.000000 superblocks-agent-0.0.6/superblocks_agent.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1774 2024-05-21 19:26:48.000000 superblocks-agent-0.0.6/superblocks_agent.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-21 19:26:48.000000 superblocks-agent-0.0.6/superblocks_agent.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-21 19:26:48.000000 superblocks-agent-0.0.6/superblocks_agent.egg-info/requires.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-21 19:26:48.000000 superblocks-agent-0.0.6/superblocks_agent.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.400591 superblocks-agent-0.0.6/test_unit/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.413027 superblocks-agent-0.0.6/test_unit/test_core/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.6/test_unit/test_core/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8672 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/test_unit/test_core/test_Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      912 2024-05-21 19:06:08.000000 superblocks-agent-0.0.6/test_unit/test_core/test_Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4270 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/test_unit/test_core/test_StepMock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.413492 superblocks-agent-0.0.6/test_unit/test_enumeration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.6/test_unit/test_enumeration/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1391 2024-05-21 18:54:37.000000 superblocks-agent-0.0.6/test_unit/test_enumeration/test_ViewMode.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.414242 superblocks-agent-0.0.6/test_unit/test_model/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.6/test_unit/test_model/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2450 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/test_unit/test_model/test_ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      790 2024-05-21 19:25:04.000000 superblocks-agent-0.0.6/test_unit/test_model/test_MockStepFilters.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-21 19:26:48.414952 superblocks-agent-0.0.6/test_unit/test_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.6/test_unit/test_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-21 19:24:53.000000 superblocks-agent-0.0.6/test_unit/test_util/test_convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-21 19:24:37.000000 superblocks-agent-0.0.6/test_unit/test_util/test_generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.666845 superblocks-agent-0.0.7/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-06 19:43:05.000000 superblocks-agent-0.0.7/LICENSE
+-rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-15 16:03:40.000000 superblocks-agent-0.0.7/MANIFEST.in
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 13:11:18.666604 superblocks-agent-0.0.7/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-20 13:15:54.000000 superblocks-agent-0.0.7/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-15 14:39:28.000000 superblocks-agent-0.0.7/pyproject.toml
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-21 18:02:15.000000 superblocks-agent-0.0.7/requirements.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-22 13:11:18.666920 superblocks-agent-0.0.7/setup.cfg
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-10 20:19:54.000000 superblocks-agent-0.0.7/setup.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.652389 superblocks-agent-0.0.7/superblocks_agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-06 20:42:01.000000 superblocks-agent-0.0.7/superblocks_agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.654568 superblocks-agent-0.0.7/superblocks_agent/_type/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_type/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_type/client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      265 2024-05-21 18:56:05.000000 superblocks-agent-0.0.7/superblocks_agent/_type/mock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.655486 superblocks-agent-0.0.7/superblocks_agent/_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/_util/generate.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-22 13:10:57.000000 superblocks-agent-0.0.7/superblocks_agent/_version.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.657109 superblocks-agent-0.0.7/superblocks_agent/core/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6635 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/core/Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1444 2024-05-21 19:23:48.000000 superblocks-agent-0.0.7/superblocks_agent/core/Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2755 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/core/_StepMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       64 2024-05-21 18:47:59.000000 superblocks-agent-0.0.7/superblocks_agent/core/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.658324 superblocks-agent-0.0.7/superblocks_agent/enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1058 2024-05-21 18:53:18.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/ViewMode.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-21 18:54:58.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/_BaseEnum.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       39 2024-05-21 18:53:29.000000 superblocks-agent-0.0.7/superblocks_agent/enumeration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.661907 superblocks-agent-0.0.7/superblocks_agent/model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      181 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/Agent.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      725 2024-05-21 18:54:49.000000 superblocks-agent-0.0.7/superblocks_agent/model/ApiConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      310 2024-05-21 19:03:38.000000 superblocks-agent-0.0.7/superblocks_agent/model/ApiResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      124 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/Auth.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      238 2024-05-21 19:06:08.000000 superblocks-agent-0.0.7/superblocks_agent/model/ClientConfig.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/ExecutionError.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1839 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/model/ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      389 2024-05-21 19:19:09.000000 superblocks-agent-0.0.7/superblocks_agent/model/StepResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1024 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/superblocks_agent/model/_MockStepFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      340 2024-05-21 19:18:26.000000 superblocks-agent-0.0.7/superblocks_agent/model/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.662856 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      475 2024-05-21 19:23:31.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/BaseMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/MockFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:31:35.000000 superblocks-agent-0.0.7/superblocks_agent/model/_abstract/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.653791 superblocks-agent-0.0.7/superblocks_agent.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1774 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/requires.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-22 13:11:18.000000 superblocks-agent-0.0.7/superblocks_agent.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.649959 superblocks-agent-0.0.7/test_unit/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.663848 superblocks-agent-0.0.7/test_unit/test_core/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_core/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8672 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_core/test_Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      912 2024-05-21 19:06:08.000000 superblocks-agent-0.0.7/test_unit/test_core/test_Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4270 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_core/test_StepMock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.664380 superblocks-agent-0.0.7/test_unit/test_enumeration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_enumeration/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1391 2024-05-21 18:54:37.000000 superblocks-agent-0.0.7/test_unit/test_enumeration/test_ViewMode.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.665357 superblocks-agent-0.0.7/test_unit/test_model/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_model/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2450 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_model/test_ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      790 2024-05-21 19:25:04.000000 superblocks-agent-0.0.7/test_unit/test_model/test_MockStepFilters.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 13:11:18.666126 superblocks-agent-0.0.7/test_unit/test_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-17 13:32:57.000000 superblocks-agent-0.0.7/test_unit/test_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-21 19:24:53.000000 superblocks-agent-0.0.7/test_unit/test_util/test_convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-21 19:24:37.000000 superblocks-agent-0.0.7/test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.6/LICENSE` & `superblocks-agent-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/PKG-INFO` & `superblocks-agent-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.6/README.md` & `superblocks-agent-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/setup.py` & `superblocks-agent-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/_util/convert.py` & `superblocks-agent-0.0.7/superblocks_agent/_util/convert.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/core/Api.py` & `superblocks-agent-0.0.7/superblocks_agent/core/Api.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/core/Client.py` & `superblocks-agent-0.0.7/superblocks_agent/core/Client.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/core/_StepMock.py` & `superblocks-agent-0.0.7/superblocks_agent/core/_StepMock.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/enumeration/ViewMode.py` & `superblocks-agent-0.0.7/superblocks_agent/enumeration/ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/model/ApiConfig.py` & `superblocks-agent-0.0.7/superblocks_agent/model/ApiConfig.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/model/ExecutionResult.py` & `superblocks-agent-0.0.7/superblocks_agent/model/ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent/model/_MockStepFilters.py` & `superblocks-agent-0.0.7/superblocks_agent/model/_MockStepFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/superblocks_agent.egg-info/PKG-INFO` & `superblocks-agent-0.0.7/superblocks_agent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.6
+Version: 0.0.7
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.6/superblocks_agent.egg-info/SOURCES.txt` & `superblocks-agent-0.0.7/superblocks_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_core/test_Api.py` & `superblocks-agent-0.0.7/test_unit/test_core/test_Api.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_core/test_Client.py` & `superblocks-agent-0.0.7/test_unit/test_core/test_Client.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_core/test_StepMock.py` & `superblocks-agent-0.0.7/test_unit/test_core/test_StepMock.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_enumeration/test_ViewMode.py` & `superblocks-agent-0.0.7/test_unit/test_enumeration/test_ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_model/test_ExecutionResult.py` & `superblocks-agent-0.0.7/test_unit/test_model/test_ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_model/test_MockStepFilters.py` & `superblocks-agent-0.0.7/test_unit/test_model/test_MockStepFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.6/test_unit/test_util/test_convert.py` & `superblocks-agent-0.0.7/test_unit/test_util/test_convert.py`

 * *Files identical despite different names*

