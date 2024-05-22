# Comparing `tmp/agi_med_utils-0.0.5.tar.gz` & `tmp/agi_med_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agi_med_utils-0.0.5.tar", last modified: Tue May 21 08:50:14 2024, max compression
+gzip compressed data, was "agi_med_utils-0.0.6.tar", last modified: Tue May 21 11:26:00 2024, max compression
```

## Comparing `agi_med_utils-0.0.5.tar` & `agi_med_utils-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.5/MANIFEST.in
--rw-r--r--   0 ivan      (1000) ivan      (1000)      721 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      422 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/README.md
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.753810 agi_med_utils-0.0.5/agi_med_utils/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-21 08:49:45.000000 agi_med_utils-0.0.5/agi_med_utils/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      382 2024-05-13 10:18:02.000000 agi_med_utils-0.0.5/agi_med_utils/abstract_client.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils/config/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.5/agi_med_utils/config/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.5/agi_med_utils/config/config.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.5/agi_med_utils/config/singleton.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils/llm/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.5/agi_med_utils/llm/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2004 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/agi_med_utils/llm/giga_access.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)     2538 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/agi_med_utils/llm/yandex_access.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/agi_med_utils.egg-info/
--rw-r--r--   0 ivan      (1000) ivan      (1000)      721 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      538 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       98 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/requires.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-21 08:50:14.000000 agi_med_utils-0.0.5/agi_med_utils.egg-info/top_level.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       98 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/requirements.txt
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/setup.cfg
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.5/setup.py
-drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 08:50:14.757810 agi_med_utils-0.0.5/test/
--rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.5/test/__init__.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)       61 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/test/test_base.py
--rw-rw-r--   0 ivan      (1000) ivan      (1000)      843 2024-05-21 08:24:29.000000 agi_med_utils-0.0.5/test/test_llm.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       25 2024-05-13 08:33:25.000000 agi_med_utils-0.0.6/MANIFEST.in
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      583 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      379 2024-05-21 11:23:57.000000 agi_med_utils-0.0.6/README.md
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/agi_med_utils/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       22 2024-05-21 11:16:32.000000 agi_med_utils-0.0.6/agi_med_utils/__init__.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/agi_med_utils/config/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.6/agi_med_utils/config/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      523 2024-05-13 09:00:12.000000 agi_med_utils-0.0.6/agi_med_utils/config/config.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      232 2024-05-13 09:00:59.000000 agi_med_utils-0.0.6/agi_med_utils/config/singleton.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/agi_med_utils/llm/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-13 08:25:13.000000 agi_med_utils-0.0.6/agi_med_utils/llm/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2004 2024-05-21 08:24:29.000000 agi_med_utils-0.0.6/agi_med_utils/llm/giga_access.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)     2538 2024-05-21 08:24:29.000000 agi_med_utils-0.0.6/agi_med_utils/llm/yandex_access.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/agi_med_utils.egg-info/
+-rw-r--r--   0 ivan      (1000) ivan      (1000)      583 2024-05-21 11:26:00.000000 agi_med_utils-0.0.6/agi_med_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      505 2024-05-21 11:26:00.000000 agi_med_utils-0.0.6/agi_med_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        1 2024-05-21 11:26:00.000000 agi_med_utils-0.0.6/agi_med_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       48 2024-05-21 11:26:00.000000 agi_med_utils-0.0.6/agi_med_utils.egg-info/requires.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       19 2024-05-21 11:26:00.000000 agi_med_utils-0.0.6/agi_med_utils.egg-info/top_level.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       48 2024-05-21 11:23:49.000000 agi_med_utils-0.0.6/requirements.txt
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       38 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/setup.cfg
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      778 2024-05-13 08:36:40.000000 agi_med_utils-0.0.6/setup.py
+drwxrwxr-x   0 ivan      (1000) ivan      (1000)        0 2024-05-21 11:26:00.974815 agi_med_utils-0.0.6/test/
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)        0 2024-05-20 10:22:34.000000 agi_med_utils-0.0.6/test/__init__.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)       61 2024-05-21 08:24:29.000000 agi_med_utils-0.0.6/test/test_base.py
+-rw-rw-r--   0 ivan      (1000) ivan      (1000)      843 2024-05-21 08:24:29.000000 agi_med_utils-0.0.6/test/test_llm.py
```

### Comparing `agi_med_utils-0.0.5/PKG-INFO` & `agi_med_utils-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: agi_med_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utils for agi-med team
 Author: AGI-MED-TEAM
-Requires-Dist: grpcio==1.62.1
-Requires-Dist: grpcio-tools==1.62.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: gigachat==0.1.17
 Requires-Dist: requests==2.31.0
-Requires-Dist: pytest==8.2.1
 
 # agi-med-utils
 
 Стандартизация компонент общей библиотеки отдела
 
 ## Ответственный разработчик
 
@@ -20,13 +17,12 @@
 
 ## Общая информация
 
 ### Фичи: 
 
 - Доступ к Yandex_GPT, Gigachat
 - Стандартный конфиг
-- Абстрактный grpc клиент
 
 ## Тесты
 
 - `sudo docker-compose -f docker-compose.yaml up --build`
```

### Comparing `agi_med_utils-0.0.5/agi_med_utils/config/config.py` & `agi_med_utils-0.0.6/agi_med_utils/config/config.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.5/agi_med_utils/llm/giga_access.py` & `agi_med_utils-0.0.6/agi_med_utils/llm/giga_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.5/agi_med_utils/llm/yandex_access.py` & `agi_med_utils-0.0.6/agi_med_utils/llm/yandex_access.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.5/agi_med_utils.egg-info/PKG-INFO` & `agi_med_utils-0.0.6/agi_med_utils.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 Metadata-Version: 2.1
 Name: agi_med_utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Utils for agi-med team
 Author: AGI-MED-TEAM
-Requires-Dist: grpcio==1.62.1
-Requires-Dist: grpcio-tools==1.62.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: gigachat==0.1.17
 Requires-Dist: requests==2.31.0
-Requires-Dist: pytest==8.2.1
 
 # agi-med-utils
 
 Стандартизация компонент общей библиотеки отдела
 
 ## Ответственный разработчик
 
@@ -20,13 +17,12 @@
 
 ## Общая информация
 
 ### Фичи: 
 
 - Доступ к Yandex_GPT, Gigachat
 - Стандартный конфиг
-- Абстрактный grpc клиент
 
 ## Тесты
 
 - `sudo docker-compose -f docker-compose.yaml up --build`
```

### Comparing `agi_med_utils-0.0.5/setup.py` & `agi_med_utils-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `agi_med_utils-0.0.5/test/test_llm.py` & `agi_med_utils-0.0.6/test/test_llm.py`

 * *Files identical despite different names*

