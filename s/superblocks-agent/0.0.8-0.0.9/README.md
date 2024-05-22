# Comparing `tmp/superblocks-agent-0.0.8.tar.gz` & `tmp/superblocks-agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-agent-0.0.8.tar", last modified: Wed May 22 16:03:20 2024, max compression
+gzip compressed data, was "superblocks-agent-0.0.9.tar", last modified: Wed May 22 18:13:19 2024, max compression
```

## Comparing `superblocks-agent-0.0.8.tar` & `superblocks-agent-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.594041 superblocks-agent-0.0.8/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/LICENSE
--rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/MANIFEST.in
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 16:03:20.593856 superblocks-agent-0.0.8/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/README.md
--rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/pyproject.toml
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/requirements.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-22 16:03:20.594113 superblocks-agent-0.0.8/setup.cfg
--rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/setup.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.578521 superblocks-agent-0.0.8/superblocks_agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.582405 superblocks-agent-0.0.8/superblocks_agent/_type/
--rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-22 15:51:41.000000 superblocks-agent-0.0.8/superblocks_agent/_type/BaseEnum.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      452 2024-05-22 15:23:31.000000 superblocks-agent-0.0.8/superblocks_agent/_type/BaseMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-22 15:51:41.000000 superblocks-agent-0.0.8/superblocks_agent/_type/MockFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_type/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_type/client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      232 2024-05-22 15:23:21.000000 superblocks-agent-0.0.8/superblocks_agent/_type/mock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.583083 superblocks-agent-0.0.8/superblocks_agent/_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/_util/convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-22 15:23:54.000000 superblocks-agent-0.0.8/superblocks_agent/_util/generate.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-22 16:03:13.000000 superblocks-agent-0.0.8/superblocks_agent/_version.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.585274 superblocks-agent-0.0.8/superblocks_agent/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)     7018 2024-05-22 15:59:11.000000 superblocks-agent-0.0.8/superblocks_agent/api/Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      735 2024-05-22 15:59:59.000000 superblocks-agent-0.0.8/superblocks_agent/api/Config.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/superblocks_agent/api/ExecutionError.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1939 2024-05-22 16:00:09.000000 superblocks-agent-0.0.8/superblocks_agent/api/ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      293 2024-05-22 16:00:40.000000 superblocks-agent-0.0.8/superblocks_agent/api/Result.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1051 2024-05-22 15:27:02.000000 superblocks-agent-0.0.8/superblocks_agent/api/ViewMode.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      242 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/api/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.586248 superblocks-agent-0.0.8/superblocks_agent/client/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1421 2024-05-22 15:50:24.000000 superblocks-agent-0.0.8/superblocks_agent/client/Client.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      187 2024-05-22 15:27:31.000000 superblocks-agent-0.0.8/superblocks_agent/client/Config.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       70 2024-05-22 15:13:14.000000 superblocks-agent-0.0.8/superblocks_agent/client/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.586670 superblocks-agent-0.0.8/superblocks_agent/step/
--rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-22 15:36:18.000000 superblocks-agent-0.0.8/superblocks_agent/step/Result.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       35 2024-05-22 15:19:35.000000 superblocks-agent-0.0.8/superblocks_agent/step/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.587481 superblocks-agent-0.0.8/superblocks_agent/testing/
--rw-r--r--   0 joeygreco   (501) staff       (20)     1014 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/testing/_MockStepFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2747 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/superblocks_agent/testing/_StepMock.py
--rw-r--r--   0 joeygreco   (501) staff       (20)       34 2024-05-22 15:15:15.000000 superblocks-agent-0.0.8/superblocks_agent/testing/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.579726 superblocks-agent-0.0.8/superblocks_agent.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     1633 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/requires.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-22 16:03:20.000000 superblocks-agent-0.0.8/superblocks_agent.egg-info/top_level.txt
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.576333 superblocks-agent-0.0.8/test_unit/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.589605 superblocks-agent-0.0.8/test_unit/test_api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:29:27.000000 superblocks-agent-0.0.8/test_unit/test_api/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8796 2024-05-22 16:02:27.000000 superblocks-agent-0.0.8/test_unit/test_api/test_Api.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2535 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/test_unit/test_api/test_ExecutionResult.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1383 2024-05-22 15:33:26.000000 superblocks-agent-0.0.8/test_unit/test_api/test_ViewMode.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.591990 superblocks-agent-0.0.8/test_unit/test_client/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:04.000000 superblocks-agent-0.0.8/test_unit/test_client/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      800 2024-05-22 16:02:27.000000 superblocks-agent-0.0.8/test_unit/test_client/test_Client.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.592904 superblocks-agent-0.0.8/test_unit/test_testing/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:42.000000 superblocks-agent-0.0.8/test_unit/test_testing/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      792 2024-05-22 15:32:24.000000 superblocks-agent-0.0.8/test_unit/test_testing/test_MockStepFilters.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4275 2024-05-22 15:51:42.000000 superblocks-agent-0.0.8/test_unit/test_testing/test_StepMock.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 16:03:20.593547 superblocks-agent-0.0.8/test_unit/test_util/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/test_convert.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-22 14:08:48.000000 superblocks-agent-0.0.8/test_unit/test_util/test_generate.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.807402 superblocks-agent-0.0.9/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1068 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/LICENSE
+-rw-r--r--   0 joeygreco   (501) staff       (20)       25 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/MANIFEST.in
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 18:13:19.807190 superblocks-agent-0.0.9/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1940 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/README.md
+-rw-r--r--   0 joeygreco   (501) staff       (20)      298 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/pyproject.toml
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/requirements.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-22 18:13:19.807508 superblocks-agent-0.0.9/setup.cfg
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1025 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/setup.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.793583 superblocks-agent-0.0.9/superblocks_agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)       42 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-22 16:22:09.000000 superblocks-agent-0.0.9/superblocks_agent/_constant.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.795276 superblocks-agent-0.0.9/superblocks_agent/_decorator/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 17:13:46.000000 superblocks-agent-0.0.9/superblocks_agent/_decorator/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      924 2024-05-22 18:06:58.000000 superblocks-agent-0.0.9/superblocks_agent/_decorator/foo_dnc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.796855 superblocks-agent-0.0.9/superblocks_agent/_type/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      363 2024-05-22 15:51:41.000000 superblocks-agent-0.0.9/superblocks_agent/_type/BaseEnum.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      452 2024-05-22 15:23:31.000000 superblocks-agent-0.0.9/superblocks_agent/_type/BaseMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       54 2024-05-22 15:51:41.000000 superblocks-agent-0.0.9/superblocks_agent/_type/MockFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/_type/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      290 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/_type/client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      232 2024-05-22 15:23:21.000000 superblocks-agent-0.0.9/superblocks_agent/_type/mock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.797976 superblocks-agent-0.0.9/superblocks_agent/_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2905 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/_util/convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1060 2024-05-22 18:00:50.000000 superblocks-agent-0.0.9/superblocks_agent/_util/decorator.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       71 2024-05-22 15:23:54.000000 superblocks-agent-0.0.9/superblocks_agent/_util/generate.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       94 2024-05-22 18:13:12.000000 superblocks-agent-0.0.9/superblocks_agent/_version.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.801153 superblocks-agent-0.0.9/superblocks_agent/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7120 2024-05-22 18:12:32.000000 superblocks-agent-0.0.9/superblocks_agent/api/Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      735 2024-05-22 15:59:59.000000 superblocks-agent-0.0.9/superblocks_agent/api/Config.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      404 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/superblocks_agent/api/ExecutionError.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1939 2024-05-22 16:00:09.000000 superblocks-agent-0.0.9/superblocks_agent/api/ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      293 2024-05-22 16:00:40.000000 superblocks-agent-0.0.9/superblocks_agent/api/Result.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1051 2024-05-22 15:27:02.000000 superblocks-agent-0.0.9/superblocks_agent/api/ViewMode.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      242 2024-05-22 15:51:42.000000 superblocks-agent-0.0.9/superblocks_agent/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.802092 superblocks-agent-0.0.9/superblocks_agent/client/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1422 2024-05-22 18:12:32.000000 superblocks-agent-0.0.9/superblocks_agent/client/Client.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      276 2024-05-22 16:27:06.000000 superblocks-agent-0.0.9/superblocks_agent/client/Config.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       70 2024-05-22 15:13:14.000000 superblocks-agent-0.0.9/superblocks_agent/client/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.802788 superblocks-agent-0.0.9/superblocks_agent/step/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      264 2024-05-22 15:36:18.000000 superblocks-agent-0.0.9/superblocks_agent/step/Result.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       35 2024-05-22 15:19:35.000000 superblocks-agent-0.0.9/superblocks_agent/step/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.803558 superblocks-agent-0.0.9/superblocks_agent/testing/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1014 2024-05-22 15:51:42.000000 superblocks-agent-0.0.9/superblocks_agent/testing/_MockStepFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2747 2024-05-22 15:51:42.000000 superblocks-agent-0.0.9/superblocks_agent/testing/_StepMock.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)       34 2024-05-22 15:15:15.000000 superblocks-agent-0.0.9/superblocks_agent/testing/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.794871 superblocks-agent-0.0.9/superblocks_agent.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2318 2024-05-22 18:13:19.000000 superblocks-agent-0.0.9/superblocks_agent.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1782 2024-05-22 18:13:19.000000 superblocks-agent-0.0.9/superblocks_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-22 18:13:19.000000 superblocks-agent-0.0.9/superblocks_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       65 2024-05-22 18:13:19.000000 superblocks-agent-0.0.9/superblocks_agent.egg-info/requires.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       28 2024-05-22 18:13:19.000000 superblocks-agent-0.0.9/superblocks_agent.egg-info/top_level.txt
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.787810 superblocks-agent-0.0.9/test_unit/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.804535 superblocks-agent-0.0.9/test_unit/test_api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:29:27.000000 superblocks-agent-0.0.9/test_unit/test_api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8738 2024-05-22 18:12:32.000000 superblocks-agent-0.0.9/test_unit/test_api/test_Api.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2535 2024-05-22 15:51:42.000000 superblocks-agent-0.0.9/test_unit/test_api/test_ExecutionResult.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1383 2024-05-22 15:33:26.000000 superblocks-agent-0.0.9/test_unit/test_api/test_ViewMode.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.805048 superblocks-agent-0.0.9/test_unit/test_client/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:04.000000 superblocks-agent-0.0.9/test_unit/test_client/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      801 2024-05-22 18:12:32.000000 superblocks-agent-0.0.9/test_unit/test_client/test_Client.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.805792 superblocks-agent-0.0.9/test_unit/test_testing/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 15:30:42.000000 superblocks-agent-0.0.9/test_unit/test_testing/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      792 2024-05-22 15:32:24.000000 superblocks-agent-0.0.9/test_unit/test_testing/test_MockStepFilters.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4275 2024-05-22 15:51:42.000000 superblocks-agent-0.0.9/test_unit/test_testing/test_StepMock.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-22 18:13:19.806499 superblocks-agent-0.0.9/test_unit/test_util/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/test_unit/test_util/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3912 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/test_unit/test_util/test_convert.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      480 2024-05-22 14:08:48.000000 superblocks-agent-0.0.9/test_unit/test_util/test_generate.py
```

### Comparing `superblocks-agent-0.0.8/LICENSE` & `superblocks-agent-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/PKG-INFO` & `superblocks-agent-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.8/README.md` & `superblocks-agent-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/setup.py` & `superblocks-agent-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/_util/convert.py` & `superblocks-agent-0.0.9/superblocks_agent/_util/convert.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/api/Api.py` & `superblocks-agent-0.0.9/superblocks_agent/api/Api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,30 @@
     TwoWayResponse,
 )
 from superblocks_types.api.v1.service_pb2_grpc import ExecutorServiceStub
 from superblocks_types.common.v1.common_pb2 import Profile
 from superblocks_types.common.v1.errors_pb2 import Error
 
 from superblocks_agent._util.convert import from_protobuf_value, to_protobuf_value
+from superblocks_agent._util.decorator import support_sync
 from superblocks_agent._util.generate import get_unique_id_for_object
 from superblocks_agent.api.Config import Config as ApiConfig
 from superblocks_agent.api.ExecutionResult import ExecutionResult
 from superblocks_agent.client import Client
 from superblocks_agent.client import Config as ClientConfig
 from superblocks_agent.testing._StepMock import StepMock
 
 
 class Api:
     def __init__(self, api_id: str, *, config: Optional[ApiConfig] = None):
         self.__api_id = api_id
         self.__config = config
         self.mock_func_lookup: dict[str, callable] = {}
 
+    @support_sync(async_is_default=False)
     async def run(
         self,
         *,
         client: Client,
         inputs: Optional[dict] = None,
         mocks: Optional[list[StepMock]] = None,
     ) -> ExecutionResult:
@@ -40,15 +42,15 @@
         """
         mocks = [] if mocks is None else mocks
         inputs = {} if inputs is None else inputs
 
         # hydrate mock lookup dict so we can reference it later
         self.__hydrate_mock_func_lookup(mocks)
 
-        stream_responses = await client.run(
+        stream_responses = await client._run(
             with_stub=ExecutorServiceStub,
             stub_func_name="TwoWayStream",
             initial_request=TwoWayRequest(
                 execute=self.__build_execute_request(
                     inputs=inputs, mocks=mocks, client_config=client.config
                 )
             ),
```

### Comparing `superblocks-agent-0.0.8/superblocks_agent/api/Config.py` & `superblocks-agent-0.0.9/superblocks_agent/api/Config.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/api/ExecutionResult.py` & `superblocks-agent-0.0.9/superblocks_agent/api/ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/api/ViewMode.py` & `superblocks-agent-0.0.9/superblocks_agent/api/ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/client/Client.py` & `superblocks-agent-0.0.9/superblocks_agent/client/Client.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from superblocks_agent.client import Config
 
 
 class Client:
     def __init__(self, config: Config):
         self.config = config
 
-    async def run(
+    async def _run(
         self,
         *,
         with_stub: object,
         stub_func_name: str,
         initial_request: object,
         response_handler: TwoWayStreamResponseHandler,
     ) -> list[StreamResponse]:
```

### Comparing `superblocks-agent-0.0.8/superblocks_agent/testing/_MockStepFilters.py` & `superblocks-agent-0.0.9/superblocks_agent/testing/_MockStepFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent/testing/_StepMock.py` & `superblocks-agent-0.0.9/superblocks_agent/testing/_StepMock.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/superblocks_agent.egg-info/PKG-INFO` & `superblocks-agent-0.0.9/superblocks_agent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Official Python SDK for Superblocks
 Home-page: https://github.com/superblocksteam/orchestrator/tree/main/clients/python
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks api sdk
 Requires-Python: >=3.10
```

### Comparing `superblocks-agent-0.0.8/superblocks_agent.egg-info/SOURCES.txt` & `superblocks-agent-0.0.9/superblocks_agent.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 superblocks_agent/__init__.py
+superblocks_agent/_constant.py
 superblocks_agent/_version.py
 superblocks_agent.egg-info/PKG-INFO
 superblocks_agent.egg-info/SOURCES.txt
 superblocks_agent.egg-info/dependency_links.txt
 superblocks_agent.egg-info/requires.txt
 superblocks_agent.egg-info/top_level.txt
+superblocks_agent/_decorator/__init__.py
+superblocks_agent/_decorator/foo_dnc.py
 superblocks_agent/_type/BaseEnum.py
 superblocks_agent/_type/BaseMock.py
 superblocks_agent/_type/MockFilters.py
 superblocks_agent/_type/__init__.py
 superblocks_agent/_type/client.py
 superblocks_agent/_type/mock.py
 superblocks_agent/_util/__init__.py
 superblocks_agent/_util/convert.py
+superblocks_agent/_util/decorator.py
 superblocks_agent/_util/generate.py
 superblocks_agent/api/Api.py
 superblocks_agent/api/Config.py
 superblocks_agent/api/ExecutionError.py
 superblocks_agent/api/ExecutionResult.py
 superblocks_agent/api/Result.py
 superblocks_agent/api/ViewMode.py
```

### Comparing `superblocks-agent-0.0.8/test_unit/test_api/test_Api.py` & `superblocks-agent-0.0.9/test_unit/test_api/test_Api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import unittest
 
 import grpc
 from superblocks_types.api.v1.event_pb2 import Event
 from superblocks_types.api.v1.service_pb2 import (
     ExecuteRequest,
     Function,
@@ -24,17 +23,15 @@
 from superblocks_agent.testing._MockStepFilters import MockStepFilters
 from superblocks_agent.testing._StepMock import StepMock
 
 
 class TestApi(unittest.TestCase):
     def test_bad_connection_info(self):
         with self.assertRaises(Exception) as context:
-            asyncio.run(
-                Api(api_id="").run(client=Client(config=ClientConfig(endpoint="", token="")))
-            )
+            Api(api_id="").run(client=Client(config=ClientConfig(endpoint="", token="")))
         self.assertIsInstance(context.exception, grpc._channel._MultiThreadedRendezvous)
 
     def test_build_execute_request(self):
         when_callable = lambda _: True
         api = Api(
             "api_id",
             config=ApiConfig(
```

### Comparing `superblocks-agent-0.0.8/test_unit/test_api/test_ExecutionResult.py` & `superblocks-agent-0.0.9/test_unit/test_api/test_ExecutionResult.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/test_unit/test_api/test_ViewMode.py` & `superblocks-agent-0.0.9/test_unit/test_api/test_ViewMode.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/test_unit/test_client/test_Client.py` & `superblocks-agent-0.0.9/test_unit/test_client/test_Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     def test_init(self):
         Client(Config(endpoint="", token=""))
 
     def test_bad_connection_info(self):
         client = Client(Config(endpoint="", token=""))
         with self.assertRaises(Exception) as context:
             asyncio.run(
-                client.run(
+                client._run(
                     with_stub=ExecutorServiceStub,
                     stub_func_name="TwoWayStream",
                     initial_request={},
                     response_handler=lambda _: True,
                 )
             )
         self.assertIsInstance(context.exception, grpc._channel._MultiThreadedRendezvous)
```

### Comparing `superblocks-agent-0.0.8/test_unit/test_testing/test_MockStepFilters.py` & `superblocks-agent-0.0.9/test_unit/test_testing/test_MockStepFilters.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/test_unit/test_testing/test_StepMock.py` & `superblocks-agent-0.0.9/test_unit/test_testing/test_StepMock.py`

 * *Files identical despite different names*

### Comparing `superblocks-agent-0.0.8/test_unit/test_util/test_convert.py` & `superblocks-agent-0.0.9/test_unit/test_util/test_convert.py`

 * *Files identical despite different names*

