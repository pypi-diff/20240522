# Comparing `tmp/jemma-0.1.422.tar.gz` & `tmp/jemma-0.1.423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jemma-0.1.422.tar", last modified: Fri Apr 12 00:35:57 2024, max compression
+gzip compressed data, was "jemma-0.1.423.tar", last modified: Fri Apr 12 01:59:58 2024, max compression
```

## Comparing `jemma-0.1.422.tar` & `jemma-0.1.423.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.242475 jemma-0.1.422/
--rw-r--r--   0 tolitius   (503) staff       (20)      125 2024-04-12 00:35:57.240575 jemma-0.1.422/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.422/README.md
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.215776 jemma-0.1.422/jemma/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2353 2024-04-11 19:01:08.000000 jemma-0.1.422/jemma/huddle.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.221649 jemma-0.1.422/jemma/prompt/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/__init__.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.223277 jemma-0.1.422/jemma/prompt/business/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/business/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)    19657 2024-04-11 22:22:14.000000 jemma-0.1.422/jemma/prompt/business/owner.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.226685 jemma-0.1.422/jemma/prompt/engineer/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/clarify.py
--rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/engineer/code.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.228933 jemma-0.1.422/jemma/prompt/tester/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/tester/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/prompt/tester/test.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.230940 jemma-0.1.422/jemma/requirements/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/requirements/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/requirements/feature.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.236673 jemma-0.1.422/jemma/team/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4881 2024-04-11 20:01:12.000000 jemma-0.1.422/jemma/team/business_owner.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/engineer.py
--rw-r--r--   0 tolitius   (503) staff       (20)     8229 2024-04-11 20:34:07.000000 jemma-0.1.422/jemma/team/project_manager.py
--rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/team/tester.py
--rw-r--r--   0 tolitius   (503) staff       (20)     6803 2024-04-11 20:04:04.000000 jemma-0.1.422/jemma/thinker.py
--rw-r--r--   0 tolitius   (503) staff       (20)     4584 2024-04-11 18:12:49.000000 jemma-0.1.422/jemma/tools.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.239236 jemma-0.1.422/jemma/work/
--rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.422/jemma/work/__init__.py
--rw-r--r--   0 tolitius   (503) staff       (20)     2904 2024-04-12 00:33:39.000000 jemma-0.1.422/jemma/work/flow.py
-drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 00:35:57.220692 jemma-0.1.422/jemma.egg-info/
--rw-r--r--   0 tolitius   (503) staff       (20)      125 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/PKG-INFO
--rw-r--r--   0 tolitius   (503) staff       (20)      736 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/SOURCES.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/dependency_links.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/entry_points.txt
--rw-r--r--   0 tolitius   (503) staff       (20)      109 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/requires.txt
--rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-12 00:35:57.000000 jemma-0.1.422/jemma.egg-info/top_level.txt
--rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-12 00:35:57.242767 jemma-0.1.422/setup.cfg
--rw-r--r--   0 tolitius   (503) staff       (20)      532 2024-04-12 00:35:47.000000 jemma-0.1.422/setup.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.780647 jemma-0.1.423/
+-rw-r--r--   0 tolitius   (503) staff       (20)     5879 2024-04-12 01:59:58.779983 jemma-0.1.423/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)     5201 2024-04-10 21:53:43.000000 jemma-0.1.423/README.md
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.759095 jemma-0.1.423/jemma/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2427 2024-04-12 01:40:24.000000 jemma-0.1.423/jemma/huddle.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.764379 jemma-0.1.423/jemma/prompt/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/__init__.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.765463 jemma-0.1.423/jemma/prompt/business/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/business/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    19657 2024-04-11 22:22:14.000000 jemma-0.1.423/jemma/prompt/business/owner.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.768426 jemma-0.1.423/jemma/prompt/engineer/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/engineer/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1672 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/engineer/clarify.py
+-rw-r--r--   0 tolitius   (503) staff       (20)    15193 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/engineer/code.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.770465 jemma-0.1.423/jemma/prompt/tester/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/tester/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1869 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/prompt/tester/test.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.772210 jemma-0.1.423/jemma/requirements/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-12 01:11:05.000000 jemma-0.1.423/jemma/requirements/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1302 2024-04-12 01:04:43.000000 jemma-0.1.423/jemma/requirements/feature.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.776946 jemma-0.1.423/jemma/team/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/team/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4881 2024-04-11 20:01:12.000000 jemma-0.1.423/jemma/team/business_owner.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4888 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/team/engineer.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     8229 2024-04-11 20:34:07.000000 jemma-0.1.423/jemma/team/project_manager.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     1606 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/team/tester.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     6803 2024-04-11 20:04:04.000000 jemma-0.1.423/jemma/thinker.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     4584 2024-04-11 18:12:49.000000 jemma-0.1.423/jemma/tools.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.778365 jemma-0.1.423/jemma/work/
+-rw-r--r--   0 tolitius   (503) staff       (20)        0 2024-04-10 04:55:56.000000 jemma-0.1.423/jemma/work/__init__.py
+-rw-r--r--   0 tolitius   (503) staff       (20)     2904 2024-04-12 00:33:39.000000 jemma-0.1.423/jemma/work/flow.py
+drwxr-xr-x   0 tolitius   (503) staff       (20)        0 2024-04-12 01:59:58.779284 jemma-0.1.423/jemma.egg-info/
+-rw-r--r--   0 tolitius   (503) staff       (20)     5879 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/PKG-INFO
+-rw-r--r--   0 tolitius   (503) staff       (20)      742 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/SOURCES.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        1 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/dependency_links.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)       44 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/entry_points.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)      125 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/requires.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)        6 2024-04-12 01:59:58.000000 jemma-0.1.423/jemma.egg-info/top_level.txt
+-rw-r--r--   0 tolitius   (503) staff       (20)      890 2024-04-12 01:56:50.000000 jemma-0.1.423/pyproject.toml
+-rw-r--r--   0 tolitius   (503) staff       (20)       38 2024-04-12 01:59:58.780760 jemma-0.1.423/setup.cfg
```

### Comparing `jemma-0.1.422/README.md` & `jemma-0.1.423/README.md`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/huddle.py` & `jemma-0.1.423/jemma/huddle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse
+import argparse, os
 from dotenv import load_dotenv
 
 from jemma.tools import parse_cli_arguments
 from jemma.requirements.feature import Feature
 from jemma.team.business_owner import BusinessOwner
 from jemma.team.engineer import Engineer
 from jemma.team.tester import Tester
@@ -10,15 +10,17 @@
 import jemma.work.flow as flow
 
 import jemma.thinker as thinker
 
 def main():
 
     ## ----------------------------- setup
-    load_dotenv()
+    env_path = os.path.join(os.getcwd(), '.env')
+    load_dotenv(dotenv_path=env_path)
+
     args = parse_cli_arguments()
     brain = thinker.make_brain(args)
 
     ## ----------------------------- create a feature
     # read requirements from the file
     requirements = ""
     if args.requirements:
```

### Comparing `jemma-0.1.422/jemma/prompt/business/owner.py` & `jemma-0.1.423/jemma/prompt/business/owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/prompt/engineer/clarify.py` & `jemma-0.1.423/jemma/prompt/engineer/clarify.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/prompt/engineer/code.py` & `jemma-0.1.423/jemma/prompt/engineer/code.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/prompt/tester/test.py` & `jemma-0.1.423/jemma/prompt/tester/test.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/requirements/feature.py` & `jemma-0.1.423/jemma/requirements/feature.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/team/business_owner.py` & `jemma-0.1.423/jemma/team/business_owner.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/team/engineer.py` & `jemma-0.1.423/jemma/team/engineer.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/team/project_manager.py` & `jemma-0.1.423/jemma/team/project_manager.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/team/tester.py` & `jemma-0.1.423/jemma/team/tester.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/thinker.py` & `jemma-0.1.423/jemma/thinker.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/tools.py` & `jemma-0.1.423/jemma/tools.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma/work/flow.py` & `jemma-0.1.423/jemma/work/flow.py`

 * *Files identical despite different names*

### Comparing `jemma-0.1.422/jemma.egg-info/SOURCES.txt` & `jemma-0.1.423/jemma.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 README.md
-setup.py
+pyproject.toml
 jemma/__init__.py
 jemma/huddle.py
 jemma/thinker.py
 jemma/tools.py
 jemma.egg-info/PKG-INFO
 jemma.egg-info/SOURCES.txt
 jemma.egg-info/dependency_links.txt
```

