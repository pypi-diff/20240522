# Comparing `tmp/robot_folders-0.4.1.tar.gz` & `tmp/robot_folders-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_folders-0.4.1.tar", last modified: Wed May 15 13:07:39 2024, max compression
+gzip compressed data, was "robot_folders-0.5.0.tar", last modified: Wed May 22 16:17:56 2024, max compression
```

## Comparing `robot_folders-0.4.1.tar` & `robot_folders-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.407915 robot_folders-0.4.1/
--rw-r--r--   0 mauch     (1000) mauch     (1000)     2688 2024-05-15 13:07:39.407915 robot_folders-0.4.1/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2368 2024-05-15 08:09:11.000000 robot_folders-0.4.1/README.rst
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.402915 robot_folders-0.4.1/bin/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1989 2024-05-15 08:09:11.000000 robot_folders-0.4.1/bin/rob_folders-complete.sh
--rwxrwxr-x   0 mauch     (1000) mauch     (1000)     1854 2024-05-15 08:09:11.000000 robot_folders-0.4.1/bin/rob_folders_get_source_command.py
--rwxrwxr-x   0 mauch     (1000) mauch     (1000)     7454 2024-05-15 08:09:11.000000 robot_folders-0.4.1/bin/rob_folders_source.sh
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     9814 2024-05-15 08:09:11.000000 robot_folders-0.4.1/bin/source_environment.sh
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2024-05-15 13:07:39.407915 robot_folders-0.4.1/setup.cfg
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1200 2024-05-15 13:05:06.000000 robot_folders-0.4.1/setup.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.401915 robot_folders-0.4.1/src/
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.402915 robot_folders-0.4.1/src/robot_folders/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.4.1/src/robot_folders/__init__.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.404915 robot_folders-0.4.1/src/robot_folders/commands/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.4.1/src/robot_folders/commands/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1823 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/active_environment.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)    16526 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/adapt_environment.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)    15448 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/add_environment.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3411 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/cd.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3623 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/change_environment.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3174 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/clean.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     6057 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/delete_environment.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1406 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/get_checkout_base_dir.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3317 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/make.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2083 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/manage_underlays.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3129 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/run.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5991 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/commands/scrape_environment.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.405915 robot_folders-0.4.1/src/robot_folders/helpers/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3024 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/ConfigParser.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.4.1/src/robot_folders/helpers/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)    11993 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/build_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     4544 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/clean_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1831 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/compilation_db_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5610 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/config_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     8318 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/directory_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)    13567 2024-05-15 12:52:38.000000 robot_folders-0.4.1/src/robot_folders/helpers/environment_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1534 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/exceptions.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3580 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/repository_helpers.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.405915 robot_folders-0.4.1/src/robot_folders/helpers/resources/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.4.1/src/robot_folders/helpers/resources/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1594 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/resources/userconfig_distribute.yaml
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2728 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/ros_version_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2806 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/underlays.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1847 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/which.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2370 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/helpers/workspace_chooser.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3783 2024-05-15 08:09:11.000000 robot_folders-0.4.1/src/robot_folders/main.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.406915 robot_folders-0.4.1/src/robot_folders.egg-info/
--rw-r--r--   0 mauch     (1000) mauch     (1000)     2688 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1843 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/SOURCES.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/dependency_links.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       55 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/entry_points.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       45 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/requires.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       14 2024-05-15 13:07:39.000000 robot_folders-0.4.1/src/robot_folders.egg-info/top_level.txt
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-15 13:07:39.406915 robot_folders-0.4.1/tests/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     3539 2024-05-15 08:09:11.000000 robot_folders-0.4.1/tests/test_add_delete.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1345 2024-05-15 08:09:11.000000 robot_folders-0.4.1/tests/test_functionality.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1533 2024-05-15 08:09:11.000000 robot_folders-0.4.1/tests/test_get_checkout_base_dir.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2024-05-15 08:09:11.000000 robot_folders-0.4.1/tests/test_which.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.277289 robot_folders-0.5.0/
+-rw-r--r--   0 mauch     (1000) mauch     (1000)     2907 2024-05-22 16:17:56.277289 robot_folders-0.5.0/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2587 2024-05-21 09:32:22.000000 robot_folders-0.5.0/README.rst
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.271288 robot_folders-0.5.0/bin/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1989 2024-05-15 08:09:11.000000 robot_folders-0.5.0/bin/rob_folders-complete.sh
+-rwxrwxr-x   0 mauch     (1000) mauch     (1000)     1854 2024-05-15 08:09:11.000000 robot_folders-0.5.0/bin/rob_folders_get_source_command.py
+-rwxrwxr-x   0 mauch     (1000) mauch     (1000)     8235 2024-05-22 16:10:30.000000 robot_folders-0.5.0/bin/rob_folders_source.sh
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     9814 2024-05-15 08:09:11.000000 robot_folders-0.5.0/bin/source_environment.sh
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2024-05-22 16:17:56.277289 robot_folders-0.5.0/setup.cfg
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1200 2024-05-22 16:11:15.000000 robot_folders-0.5.0/setup.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.270288 robot_folders-0.5.0/src/
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.271288 robot_folders-0.5.0/src/robot_folders/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.5.0/src/robot_folders/__init__.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.274289 robot_folders-0.5.0/src/robot_folders/commands/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.5.0/src/robot_folders/commands/__init__.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1823 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/active_environment.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)    16526 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/adapt_environment.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)    15448 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/add_environment.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3411 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/cd.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3623 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/change_environment.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3174 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/clean.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     6057 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/delete_environment.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1406 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/get_checkout_base_dir.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3317 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/make.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2083 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/manage_underlays.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3129 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/run.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     5991 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/commands/scrape_environment.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.276289 robot_folders-0.5.0/src/robot_folders/helpers/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3024 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/ConfigParser.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.5.0/src/robot_folders/helpers/__init__.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)    11993 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/build_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     4544 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/clean_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1831 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/compilation_db_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     5610 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/config_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     8318 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/directory_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)    13567 2024-05-15 12:52:38.000000 robot_folders-0.5.0/src/robot_folders/helpers/environment_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1534 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/exceptions.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3580 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/repository_helpers.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.276289 robot_folders-0.5.0/src/robot_folders/helpers/resources/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2024-05-15 12:34:59.000000 robot_folders-0.5.0/src/robot_folders/helpers/resources/__init__.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1594 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/resources/userconfig_distribute.yaml
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2728 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/ros_version_helpers.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2806 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/underlays.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1847 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/which.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     2370 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/helpers/workspace_chooser.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3783 2024-05-15 08:09:11.000000 robot_folders-0.5.0/src/robot_folders/main.py
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.276289 robot_folders-0.5.0/src/robot_folders.egg-info/
+-rw-r--r--   0 mauch     (1000) mauch     (1000)     2907 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/PKG-INFO
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1843 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       55 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/entry_points.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       45 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/requires.txt
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)       14 2024-05-22 16:17:56.000000 robot_folders-0.5.0/src/robot_folders.egg-info/top_level.txt
+drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2024-05-22 16:17:56.276289 robot_folders-0.5.0/tests/
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     3539 2024-05-15 08:09:11.000000 robot_folders-0.5.0/tests/test_add_delete.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1345 2024-05-15 08:09:11.000000 robot_folders-0.5.0/tests/test_functionality.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1533 2024-05-15 08:09:11.000000 robot_folders-0.5.0/tests/test_get_checkout_base_dir.py
+-rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2024-05-15 08:09:11.000000 robot_folders-0.5.0/tests/test_which.py
```

### Comparing `robot_folders-0.4.1/PKG-INFO` & `robot_folders-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: robot_folders
-Version: 0.4.1
+Version: 0.5.0
 Summary: robot_folders is your workspace handling utility around the ROS ecosystem.
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Requires-Dist: Click>=8.0
 Requires-Dist: gitpython
 Requires-Dist: inquirer
 Requires-Dist: PyYaml
 Requires-Dist: vcstool
 
+|license_badge| |codecov_badge| |doc_badge|
+
+
 Robot Folders
 =============
 
 Welcome to ``robot_folders``! ``robot_folders`` is a collection of utility scripts designed to
 streamline and facilitate the management of workspaces used for (ROS) development. It is designed
 to enhance efficiency in handling different environments, consisting of multiple workspaces like a
 ``catkin_workspace`` and ``colcon_workspace`` or a plain CMake workspace.
 
 It focuses on optimizing the management of various subworkspaces, contributing
 to a seamless development experience.
 
 
+Documentation
+-------------
+Documentation can be found on `our GH pages <https://fzi-forschungszentrum-informatik.github.io/robot_folders/>`_.
+
+
 Quick start
 ------------
 
 It is recommended to install robot_folders using ``pipx`` (You can install ``pipx`` using ``sudo apt
-install pipx``). Please note: With pipx versions < 1.0 you'll have to provide the `--spec` flag
+install pipx``).
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
-   pipx install git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx install --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
+   pipx install robot-folders
 
 Upgrade
--------
+^^^^^^^
 
 To upgrade robot_folders using ``pipx`` do
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
    pipx upgrade robot-folders
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx upgrade --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
 
 Shell setup
------------
+^^^^^^^^^^^
 
 In order to use ``robot_folders`` you'll have to call its source file. How to do this depends on
 the way you installed ``robot_folders`` and on the version of the installation tool.
 
 In case you have installed
 ``robot_folders`` using ``pipx`` as described above (and given you use the bash shell), do:
 
@@ -63,21 +65,31 @@
    # pipx >= 1.3.0
    echo "source ${HOME}/.local/share/pipx/venvs/robot-folders/bin/rob_folders_source.sh" >> ~/.bashrc
 
 In case you manually installed ``robot_folders`` using a python virtualenv the path is similarly
 
 .. code:: bash
 
-   echo "source <your-vurtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
+   echo "source <your-virtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
 
 
 Basic usage
------------
+^^^^^^^^^^^
 
 After installation open up a new terminal to use robot_folders. The main
 command for using robot_folders is ``fzirob``. Type
 
 .. code:: bash
 
    fzirob --help
 
 to get an overview over all available commands.
+
+
+
+.. |license_badge| image:: https://img.shields.io/github/license/fzi-forschungszentrum-informatik/robot_folders?color=yellow
+   :alt: GitHub License
+
+.. |codecov_badge| image:: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders/graph/badge.svg?token=85HNG0NCEI
+ :target: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders
+.. |doc_badge| image:: https://img.shields.io/badge/Documentation-Github_Pages-blue
+ :target: https://fzi-forschungszentrum-informatik.github.io/robot_folders/index.html
```

### Comparing `robot_folders-0.4.1/README.rst` & `robot_folders-0.5.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,48 @@
+|license_badge| |codecov_badge| |doc_badge|
+
+
 Robot Folders
 =============
 
 Welcome to ``robot_folders``! ``robot_folders`` is a collection of utility scripts designed to
 streamline and facilitate the management of workspaces used for (ROS) development. It is designed
 to enhance efficiency in handling different environments, consisting of multiple workspaces like a
 ``catkin_workspace`` and ``colcon_workspace`` or a plain CMake workspace.
 
 It focuses on optimizing the management of various subworkspaces, contributing
 to a seamless development experience.
 
 
+Documentation
+-------------
+Documentation can be found on `our GH pages <https://fzi-forschungszentrum-informatik.github.io/robot_folders/>`_.
+
+
 Quick start
 ------------
 
 It is recommended to install robot_folders using ``pipx`` (You can install ``pipx`` using ``sudo apt
-install pipx``). Please note: With pipx versions < 1.0 you'll have to provide the `--spec` flag
+install pipx``).
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
-   pipx install git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx install --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
+   pipx install robot-folders
 
 Upgrade
--------
+^^^^^^^
 
 To upgrade robot_folders using ``pipx`` do
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
    pipx upgrade robot-folders
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx upgrade --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
 
 Shell setup
------------
+^^^^^^^^^^^
 
 In order to use ``robot_folders`` you'll have to call its source file. How to do this depends on
 the way you installed ``robot_folders`` and on the version of the installation tool.
 
 In case you have installed
 ``robot_folders`` using ``pipx`` as described above (and given you use the bash shell), do:
 
@@ -51,21 +53,31 @@
    # pipx >= 1.3.0
    echo "source ${HOME}/.local/share/pipx/venvs/robot-folders/bin/rob_folders_source.sh" >> ~/.bashrc
 
 In case you manually installed ``robot_folders`` using a python virtualenv the path is similarly
 
 .. code:: bash
 
-   echo "source <your-vurtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
+   echo "source <your-virtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
 
 
 Basic usage
------------
+^^^^^^^^^^^
 
 After installation open up a new terminal to use robot_folders. The main
 command for using robot_folders is ``fzirob``. Type
 
 .. code:: bash
 
    fzirob --help
 
 to get an overview over all available commands.
+
+
+
+.. |license_badge| image:: https://img.shields.io/github/license/fzi-forschungszentrum-informatik/robot_folders?color=yellow
+   :alt: GitHub License
+
+.. |codecov_badge| image:: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders/graph/badge.svg?token=85HNG0NCEI
+ :target: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders
+.. |doc_badge| image:: https://img.shields.io/badge/Documentation-Github_Pages-blue
+ :target: https://fzi-forschungszentrum-informatik.github.io/robot_folders/index.html
```

### Comparing `robot_folders-0.4.1/bin/rob_folders-complete.sh` & `robot_folders-0.5.0/bin/rob_folders-complete.sh`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/bin/rob_folders_get_source_command.py` & `robot_folders-0.5.0/bin/rob_folders_get_source_command.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/bin/rob_folders_source.sh` & `robot_folders-0.5.0/bin/rob_folders_source.sh`

 * *Files 3% similar despite different names*

```diff
@@ -156,29 +156,44 @@
       echo "rob_folders $@"
 
       rob_folders $@
 
       if [ $? -eq 0 ]; then
         if [ $1 = "change_environment" ] && [ "$2" != "--help"  ]; then
           checkout_dir=$(rob_folders get_checkout_base_dir)
+
           if [ -f ${checkout_dir}/.cur_env ]; then
-            export ROB_FOLDERS_ACTIVE_ENV=$(cat ${checkout_dir}/.cur_env)
+            # Since the python command writes the .cur_env file there is a race condition when
+            # running change_environment commands in parallel. Thus it can happen that reading the
+            # file returns an empty value. This race condition only occurs on a very high io load
+            # and usually this while look should only be entered once.
+            while [ -z "$ROB_FOLDERS_ACTIVE_ENV" ]; do
+              export ROB_FOLDERS_ACTIVE_ENV=$(cat ${checkout_dir}/.cur_env)
+            done
             environment_dir="${checkout_dir}/${ROB_FOLDERS_ACTIVE_ENV}"
             if [ -f ${environment_dir}/setup.sh ]; then
               source ${environment_dir}/setup.sh
             elif [ -f ${environment_dir}/setup.zsh ]; then
               source ${environment_dir}/setup.zsh
             elif [ -f ${environment_dir}/setup.bash ]; then
               source ${environment_dir}/setup.bash
             else
               source ${ROB_FOLDERS_BASE_DIR}/bin/source_environment.sh
             fi
             # declare environment-specific aliases
             env_aliases
             #check_env
+            # Write current env to prompt
+            if [ -z "${ROB_FOLDERS_DISABLE_PROMPT_MODIFICATION:-}" ] ; then
+                env_prompt="[${ROB_FOLDERS_ACTIVE_ENV}]"
+                if [ -n "${PS1##*"$env_prompt"*}" ]; then
+                  PS1="${env_prompt} ${PS1:-}"
+                  export PS1
+                fi
+            fi
           else
             echo "Could not change environment"
           fi
         elif [ $1 = "add_environment" ] && [ "$2" != "--help"  ]; then
           if [ -z "$ROB_FOLDERS_ACTIVE_ENV" ]; then
             fzirob change_environment
             echo "Sourced new environment"
```

### Comparing `robot_folders-0.4.1/bin/source_environment.sh` & `robot_folders-0.5.0/bin/source_environment.sh`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/setup.py` & `robot_folders-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.rst").read_text()
 
 setup(
     name="robot_folders",
-    version="0.4.1",
+    version="0.5.0",
     python_requires=">=3",
     description="robot_folders is your workspace handling utility around the ROS ecosystem.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=[
         "robot_folders",
         "robot_folders.commands",
```

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/active_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/active_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/adapt_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/adapt_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/add_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/add_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/cd.py` & `robot_folders-0.5.0/src/robot_folders/commands/cd.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/change_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/change_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/clean.py` & `robot_folders-0.5.0/src/robot_folders/commands/clean.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/delete_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/delete_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/get_checkout_base_dir.py` & `robot_folders-0.5.0/src/robot_folders/commands/get_checkout_base_dir.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/make.py` & `robot_folders-0.5.0/src/robot_folders/commands/make.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/manage_underlays.py` & `robot_folders-0.5.0/src/robot_folders/commands/manage_underlays.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/run.py` & `robot_folders-0.5.0/src/robot_folders/commands/run.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/commands/scrape_environment.py` & `robot_folders-0.5.0/src/robot_folders/commands/scrape_environment.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/ConfigParser.py` & `robot_folders-0.5.0/src/robot_folders/helpers/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/build_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/build_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/clean_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/clean_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/compilation_db_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/compilation_db_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/config_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/config_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/directory_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/directory_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/environment_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/environment_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/exceptions.py` & `robot_folders-0.5.0/src/robot_folders/helpers/exceptions.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/repository_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/repository_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/resources/userconfig_distribute.yaml` & `robot_folders-0.5.0/src/robot_folders/helpers/resources/userconfig_distribute.yaml`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/ros_version_helpers.py` & `robot_folders-0.5.0/src/robot_folders/helpers/ros_version_helpers.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/underlays.py` & `robot_folders-0.5.0/src/robot_folders/helpers/underlays.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/which.py` & `robot_folders-0.5.0/src/robot_folders/helpers/which.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/helpers/workspace_chooser.py` & `robot_folders-0.5.0/src/robot_folders/helpers/workspace_chooser.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders/main.py` & `robot_folders-0.5.0/src/robot_folders/main.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/src/robot_folders.egg-info/PKG-INFO` & `robot_folders-0.5.0/src/robot_folders.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 Metadata-Version: 2.1
 Name: robot_folders
-Version: 0.4.1
+Version: 0.5.0
 Summary: robot_folders is your workspace handling utility around the ROS ecosystem.
 Requires-Python: >=3
 Description-Content-Type: text/x-rst
 Requires-Dist: Click>=8.0
 Requires-Dist: gitpython
 Requires-Dist: inquirer
 Requires-Dist: PyYaml
 Requires-Dist: vcstool
 
+|license_badge| |codecov_badge| |doc_badge|
+
+
 Robot Folders
 =============
 
 Welcome to ``robot_folders``! ``robot_folders`` is a collection of utility scripts designed to
 streamline and facilitate the management of workspaces used for (ROS) development. It is designed
 to enhance efficiency in handling different environments, consisting of multiple workspaces like a
 ``catkin_workspace`` and ``colcon_workspace`` or a plain CMake workspace.
 
 It focuses on optimizing the management of various subworkspaces, contributing
 to a seamless development experience.
 
 
+Documentation
+-------------
+Documentation can be found on `our GH pages <https://fzi-forschungszentrum-informatik.github.io/robot_folders/>`_.
+
+
 Quick start
 ------------
 
 It is recommended to install robot_folders using ``pipx`` (You can install ``pipx`` using ``sudo apt
-install pipx``). Please note: With pipx versions < 1.0 you'll have to provide the `--spec` flag
+install pipx``).
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
-   pipx install git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx install --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
+   pipx install robot-folders
 
 Upgrade
--------
+^^^^^^^
 
 To upgrade robot_folders using ``pipx`` do
 
 .. code:: bash
 
-   # pipx >= 1.0 (from ubuntu 22.04 on)
    pipx upgrade robot-folders
-   # pipx < 1.0 (ubuntu 20.04)
-   pipx upgrade --spec git+https://github.com/fzi-forschungszentrum-informatik/robot_folders.git robot-folders
 
 Shell setup
------------
+^^^^^^^^^^^
 
 In order to use ``robot_folders`` you'll have to call its source file. How to do this depends on
 the way you installed ``robot_folders`` and on the version of the installation tool.
 
 In case you have installed
 ``robot_folders`` using ``pipx`` as described above (and given you use the bash shell), do:
 
@@ -63,21 +65,31 @@
    # pipx >= 1.3.0
    echo "source ${HOME}/.local/share/pipx/venvs/robot-folders/bin/rob_folders_source.sh" >> ~/.bashrc
 
 In case you manually installed ``robot_folders`` using a python virtualenv the path is similarly
 
 .. code:: bash
 
-   echo "source <your-vurtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
+   echo "source <your-virtualenv-path>/bin/rob_folders_source.sh" >> ~/.bashrc
 
 
 Basic usage
------------
+^^^^^^^^^^^
 
 After installation open up a new terminal to use robot_folders. The main
 command for using robot_folders is ``fzirob``. Type
 
 .. code:: bash
 
    fzirob --help
 
 to get an overview over all available commands.
+
+
+
+.. |license_badge| image:: https://img.shields.io/github/license/fzi-forschungszentrum-informatik/robot_folders?color=yellow
+   :alt: GitHub License
+
+.. |codecov_badge| image:: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders/graph/badge.svg?token=85HNG0NCEI
+ :target: https://codecov.io/gh/fzi-forschungszentrum-informatik/robot_folders
+.. |doc_badge| image:: https://img.shields.io/badge/Documentation-Github_Pages-blue
+ :target: https://fzi-forschungszentrum-informatik.github.io/robot_folders/index.html
```

### Comparing `robot_folders-0.4.1/src/robot_folders.egg-info/SOURCES.txt` & `robot_folders-0.5.0/src/robot_folders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/tests/test_add_delete.py` & `robot_folders-0.5.0/tests/test_add_delete.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/tests/test_functionality.py` & `robot_folders-0.5.0/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/tests/test_get_checkout_base_dir.py` & `robot_folders-0.5.0/tests/test_get_checkout_base_dir.py`

 * *Files identical despite different names*

### Comparing `robot_folders-0.4.1/tests/test_which.py` & `robot_folders-0.5.0/tests/test_which.py`

 * *Files identical despite different names*

