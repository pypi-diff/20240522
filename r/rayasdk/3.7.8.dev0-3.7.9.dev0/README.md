# Comparing `tmp/rayasdk-3.7.8.dev0.tar.gz` & `tmp/rayasdk-3.7.9.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rayasdk-3.7.8.dev0.tar", last modified: Mon Jan 22 23:07:28 2024, max compression
+gzip compressed data, was "rayasdk-3.7.9.dev0.tar", last modified: Tue Jan 23 23:45:33 2024, max compression
```

## Comparing `rayasdk-3.7.8.dev0.tar` & `rayasdk-3.7.9.dev0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/
--rw-rw-r--   0 prod      (1001) prod      (1001)     8700 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)     6219 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/README.md
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk/
--rw-rw-r--   0 prod      (1001) prod      (1001)      546 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/__init__.py
--rwxrwxr-x   0 prod      (1001) prod      (1001)     7502 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/__main__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)       25 2024-01-22 23:07:24.000000 rayasdk-3.7.8.dev0/rayasdk/_version.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     5729 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/connect.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3829 2024-01-09 19:20:01.000000 rayasdk-3.7.8.dev0/rayasdk/constants.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk/container_handlers/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 13:54:19.000000 rayasdk-3.7.8.dev0/rayasdk/container_handlers/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     8600 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/container_handlers/docker_handler.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      434 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/exceptions.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     2163 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/executioner_command.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3102 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/initializer.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1481 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/killer.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     4167 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/logger.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1977 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/messages.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     6713 2024-01-09 19:20:01.000000 rayasdk-3.7.8.dev0/rayasdk/runner.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     4835 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/scanner.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     7074 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/simulator.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk/skills/
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/skills/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     5002 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/skills/dependencies_installer.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3970 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/skills/installer.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1412 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/skills_manager.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     4640 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/sshKeyGen.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk/template/
--rw-rw-r--   0 prod      (1001) prod      (1001)      244 2024-01-05 13:54:19.000000 rayasdk-3.7.8.dev0/rayasdk/template/__main__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      551 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/template/app.py
--rw-rw-r--   0 prod      (1001) prod      (1001)      399 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/template/launch.json
--rw-rw-r--   0 prod      (1001) prod      (1001)      303 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/template/manifest.json
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk/tools/
--rw-rw-r--   0 prod      (1001) prod      (1001)     4182 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/tools/FSM_creation.py
--rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/tools/__init__.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     1257 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/tools_command.py
--rw-rw-r--   0 prod      (1001) prod      (1001)     3046 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/utils.py
--rw-rw-r--   0 prod      (1001) prod      (1001)    11930 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/rayasdk/vcs.py
-drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/rayasdk.egg-info/
--rw-rw-r--   0 prod      (1001) prod      (1001)     8700 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/PKG-INFO
--rw-rw-r--   0 prod      (1001) prod      (1001)      959 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/SOURCES.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        1 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/dependency_links.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)       51 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/entry_points.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)      120 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/requires.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)        8 2024-01-22 23:07:28.000000 rayasdk-3.7.8.dev0/rayasdk.egg-info/top_level.txt
--rw-rw-r--   0 prod      (1001) prod      (1001)       79 2024-01-22 23:07:28.837831 rayasdk-3.7.8.dev0/setup.cfg
--rw-rw-r--   0 prod      (1001) prod      (1001)     1417 2024-01-05 14:00:59.000000 rayasdk-3.7.8.dev0/setup.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8700 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6219 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/README.md
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      546 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/__init__.py
+-rwxrwxr-x   0 prod      (1001) prod      (1001)     7502 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/__main__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)       25 2024-01-23 23:45:28.000000 rayasdk-3.7.9.dev0/rayasdk/_version.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     5729 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/connect.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3829 2024-01-09 19:20:01.000000 rayasdk-3.7.9.dev0/rayasdk/constants.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk/container_handlers/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 13:54:19.000000 rayasdk-3.7.9.dev0/rayasdk/container_handlers/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8600 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/container_handlers/docker_handler.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      434 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/exceptions.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     2163 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/executioner_command.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3102 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/initializer.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1481 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/killer.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4167 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/logger.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1977 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/messages.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     6713 2024-01-09 19:20:01.000000 rayasdk-3.7.9.dev0/rayasdk/runner.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4835 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/scanner.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     7074 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/simulator.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk/skills/
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/skills/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     5002 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/skills/dependencies_installer.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3970 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/skills/installer.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1412 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/skills_manager.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4640 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/sshKeyGen.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk/template/
+-rw-rw-r--   0 prod      (1001) prod      (1001)      244 2024-01-05 13:54:19.000000 rayasdk-3.7.9.dev0/rayasdk/template/__main__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      551 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/template/app.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)      399 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/template/launch.json
+-rw-rw-r--   0 prod      (1001) prod      (1001)      303 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/template/manifest.json
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk/tools/
+-rw-rw-r--   0 prod      (1001) prod      (1001)     4182 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/tools/FSM_creation.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)        0 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/tools/__init__.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1257 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/tools_command.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)     3046 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/utils.py
+-rw-rw-r--   0 prod      (1001) prod      (1001)    11930 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/rayasdk/vcs.py
+drwxrwxr-x   0 prod      (1001) prod      (1001)        0 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/rayasdk.egg-info/
+-rw-rw-r--   0 prod      (1001) prod      (1001)     8700 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/PKG-INFO
+-rw-rw-r--   0 prod      (1001) prod      (1001)      959 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        1 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)       51 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/entry_points.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)      120 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/requires.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)        8 2024-01-23 23:45:33.000000 rayasdk-3.7.9.dev0/rayasdk.egg-info/top_level.txt
+-rw-rw-r--   0 prod      (1001) prod      (1001)       79 2024-01-23 23:45:33.156120 rayasdk-3.7.9.dev0/setup.cfg
+-rw-rw-r--   0 prod      (1001) prod      (1001)     1417 2024-01-05 14:00:59.000000 rayasdk-3.7.9.dev0/setup.py
```

### Comparing `rayasdk-3.7.8.dev0/PKG-INFO` & `rayasdk-3.7.9.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 3.7.8.dev0
+Version: 3.7.9.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Description: # Documentation
```

### Comparing `rayasdk-3.7.8.dev0/README.md` & `rayasdk-3.7.9.dev0/README.md`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/__init__.py` & `rayasdk-3.7.9.dev0/rayasdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/__main__.py` & `rayasdk-3.7.9.dev0/rayasdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/connect.py` & `rayasdk-3.7.9.dev0/rayasdk/connect.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/constants.py` & `rayasdk-3.7.9.dev0/rayasdk/constants.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/container_handlers/docker_handler.py` & `rayasdk-3.7.9.dev0/rayasdk/container_handlers/docker_handler.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/executioner_command.py` & `rayasdk-3.7.9.dev0/rayasdk/executioner_command.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/initializer.py` & `rayasdk-3.7.9.dev0/rayasdk/initializer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/killer.py` & `rayasdk-3.7.9.dev0/rayasdk/killer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/logger.py` & `rayasdk-3.7.9.dev0/rayasdk/logger.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/messages.py` & `rayasdk-3.7.9.dev0/rayasdk/messages.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/runner.py` & `rayasdk-3.7.9.dev0/rayasdk/runner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/scanner.py` & `rayasdk-3.7.9.dev0/rayasdk/scanner.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/simulator.py` & `rayasdk-3.7.9.dev0/rayasdk/simulator.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/skills/dependencies_installer.py` & `rayasdk-3.7.9.dev0/rayasdk/skills/dependencies_installer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/skills/installer.py` & `rayasdk-3.7.9.dev0/rayasdk/skills/installer.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/skills_manager.py` & `rayasdk-3.7.9.dev0/rayasdk/skills_manager.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/sshKeyGen.py` & `rayasdk-3.7.9.dev0/rayasdk/sshKeyGen.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/template/app.py` & `rayasdk-3.7.9.dev0/rayasdk/template/app.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/tools/FSM_creation.py` & `rayasdk-3.7.9.dev0/rayasdk/tools/FSM_creation.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/tools_command.py` & `rayasdk-3.7.9.dev0/rayasdk/tools_command.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/utils.py` & `rayasdk-3.7.9.dev0/rayasdk/utils.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk/vcs.py` & `rayasdk-3.7.9.dev0/rayasdk/vcs.py`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/rayasdk.egg-info/PKG-INFO` & `rayasdk-3.7.9.dev0/rayasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rayasdk
-Version: 3.7.8.dev0
+Version: 3.7.9.dev0
 Summary: Raya SDK - Unlimited Robotics Software Development Kit
 Home-page: UNKNOWN
 Author: Unlimited Robotics
 Author-email: camilo@unlimited-robotics.com
 License: MIT
 Description: # Documentation
```

### Comparing `rayasdk-3.7.8.dev0/rayasdk.egg-info/SOURCES.txt` & `rayasdk-3.7.9.dev0/rayasdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rayasdk-3.7.8.dev0/setup.py` & `rayasdk-3.7.9.dev0/setup.py`

 * *Files identical despite different names*

