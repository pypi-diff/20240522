# Comparing `tmp/nb2workflow-1.3.8.tar.gz` & `tmp/nb2workflow-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb2workflow-1.3.8.tar", last modified: Mon Nov 29 14:42:54 2021, max compression
+gzip compressed data, was "nb2workflow-1.3.9.tar", last modified: Mon Nov 29 16:12:34 2021, max compression
```

## Comparing `nb2workflow-1.3.8.tar` & `nb2workflow-1.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.129363 nb2workflow-1.3.8/
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.117363 nb2workflow-1.3.8/.github/
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.121363 nb2workflow-1.3.8/.github/workflows/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1508 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/.github/workflows/python-package.yml
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      307 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/.gitignore
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      554 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/Dockerfile
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    34951 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/LICENSE
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      204 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/MANIFEST
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      399 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/Makefile
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 14:42:54.129363 nb2workflow-1.3.8/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      660 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/Pipfile
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1069 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/README.md
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/TODO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        6 2021-11-29 14:42:50.000000 nb2workflow-1.3.8/VERSION
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.121363 nb2workflow-1.3.8/docs/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      608 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/docs/Makefile
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5129 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/docs/conf.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      449 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/docs/index.rst
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.125363 nb2workflow-1.3.8/nb2workflow/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      149 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/__init__.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     7158 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/container.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5227 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/cwl.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1585 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/health.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1459 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/logstash.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       72 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/model.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    23465 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/nbadapter.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     4125 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/ontology.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      872 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/publish.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      310 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/schedule.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    25215 2021-11-29 14:25:34.000000 nb2workflow-1.3.8/nb2workflow/service.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5154 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/nb2workflow/workflows.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.125363 nb2workflow-1.3.8/nb2workflow.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      865 2021-11-29 14:42:54.000000 nb2workflow-1.3.8/nb2workflow.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      330 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/entry_points.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/not-zip-safe
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      276 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/requires.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       12 2021-11-29 14:42:53.000000 nb2workflow-1.3.8/nb2workflow.egg-info/top_level.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      355 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/requirements.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      489 2021-11-29 14:42:54.129363 nb2workflow-1.3.8/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2120 2021-11-29 14:42:50.000000 nb2workflow-1.3.8/setup.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 14:42:54.129363 nb2workflow-1.3.8/tests/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3408 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/conftest.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      446 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/test_cwl.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3904 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/test_nbadapter.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      665 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/test_ontology.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1385 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/test_run.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3273 2021-11-29 14:24:34.000000 nb2workflow-1.3.8/tests/test_service.py
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2574 2021-05-31 07:24:07.000000 nb2workflow-1.3.8/tests/test_workflows.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.528756 nb2workflow-1.3.9/.github/
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.528756 nb2workflow-1.3.9/.github/workflows/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1508 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/.github/workflows/python-package.yml
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      307 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/.gitignore
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      554 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Dockerfile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    34951 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/LICENSE
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      204 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/MANIFEST
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      399 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Makefile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      660 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/Pipfile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1069 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/README.md
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       38 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/TODO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        6 2021-11-29 16:12:31.000000 nb2workflow-1.3.9/VERSION
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/docs/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      608 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/Makefile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5129 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/conf.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      449 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/docs/index.rst
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/nb2workflow/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      149 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/__init__.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     7158 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/container.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5227 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/cwl.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1585 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/health.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1459 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/logstash.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       72 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/model.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    23465 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/nbadapter.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     4125 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/ontology.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      872 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/publish.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      310 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/nb2workflow/schedule.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)    25401 2021-11-29 15:39:20.000000 nb2workflow-1.3.9/nb2workflow/service.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     5350 2021-11-29 15:40:28.000000 nb2workflow-1.3.9/nb2workflow/workflows.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/nb2workflow.egg-info/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      499 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      865 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      330 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/entry_points.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2021-11-29 14:42:53.000000 nb2workflow-1.3.9/nb2workflow.egg-info/not-zip-safe
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      276 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/requires.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       12 2021-11-29 16:12:34.000000 nb2workflow-1.3.9/nb2workflow.egg-info/top_level.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      355 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/requirements.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      489 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/setup.cfg
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2120 2021-11-29 16:12:31.000000 nb2workflow-1.3.9/setup.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2021-11-29 16:12:34.532756 nb2workflow-1.3.9/tests/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3408 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/conftest.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      446 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_cwl.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3904 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_nbadapter.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      665 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_ontology.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1385 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_run.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     3273 2021-11-29 14:24:34.000000 nb2workflow-1.3.9/tests/test_service.py
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     2574 2021-05-31 07:24:07.000000 nb2workflow-1.3.9/tests/test_workflows.py
```

### Comparing `nb2workflow-1.3.8/.github/workflows/python-package.yml` & `nb2workflow-1.3.9/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/Dockerfile` & `nb2workflow-1.3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/LICENSE` & `nb2workflow-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/Pipfile` & `nb2workflow-1.3.9/Pipfile`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/README.md` & `nb2workflow-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/docs/Makefile` & `nb2workflow-1.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/docs/conf.py` & `nb2workflow-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/container.py` & `nb2workflow-1.3.9/nb2workflow/container.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/cwl.py` & `nb2workflow-1.3.9/nb2workflow/cwl.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/health.py` & `nb2workflow-1.3.9/nb2workflow/health.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/logstash.py` & `nb2workflow-1.3.9/nb2workflow/logstash.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/nbadapter.py` & `nb2workflow-1.3.9/nb2workflow/nbadapter.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/ontology.py` & `nb2workflow-1.3.9/nb2workflow/ontology.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/publish.py` & `nb2workflow-1.3.9/nb2workflow/publish.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/nb2workflow/service.py` & `nb2workflow-1.3.9/nb2workflow/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,14 @@
     def __init__(self, worker_id):
         self.worker_id = worker_id
         super(AsyncWorker, self).__init__()
 
     def run(self):
         while True:
             self.run_one()
-
             time.sleep(5)
 
     def run_one(self):
         logger.info("worker_id %s", self.worker_id)
         async_workflow = async_queue.get(block=True)
         async_workflow.run()
 
@@ -150,15 +149,19 @@
         self.params = params
         self.callback = callback
 
     def run(self):
         try:
             self._run()
         except Exception as e:
-            print("failed", e)
+            logger.error("run failed unexplicably: %s", repr(e))
+            app.async_workflows[self.key] = dict(
+                output={}, 
+                exceptions=[serialize_workflow_exception(e)]
+            )
 
     def note(self, *args, **kwargs):
         if not hasattr(self, 'notes'):
             self.notes = []
 
         self.notes.append(dict(
             time=time.time(),
```

### Comparing `nb2workflow-1.3.8/nb2workflow/workflows.py` & `nb2workflow-1.3.9/nb2workflow/workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,26 @@
     sentry_sdk = None
 
 
 class WorkflowException(Exception):
     pass
 
 def serialize_workflow_exception(e):
-    return dict(
-                ename = e[0].ename,
-                evalue = e[0].evalue,
-                edump = e[1][0],
-            )
+    try:
+        return dict(
+                    ename = e[0].ename,
+                    evalue = e[0].evalue,
+                    edump = e[1][0],
+                )
+    except TypeError:
+        return dict(
+                    ename = repr(e),
+                    evalue = "",
+                    edump = repr(e)
+                )
 
     
 def reroute(router, *args, **kwargs):
     workflow_routes = dict([ r.split("=") for r in os.environ.get('WORKFLOW_ROUTES','').split(",") if len(r.split("=")) == 2 ])
 
     workflow = args[0]
```

### Comparing `nb2workflow-1.3.8/nb2workflow.egg-info/SOURCES.txt` & `nb2workflow-1.3.9/nb2workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/setup.py` & `nb2workflow-1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 
 setup_requires = ['setuptools >= 30.3.0', 'setuptools-git-version']
 if {'pytest', 'test', 'ptr'}.intersection(sys.argv):
     setup_requires.append('pytest-runner')
 
 setup(name='nb2workflow',
-      version = '1.3.8',
+      version = '1.3.9',
       description='convert notebook to workflow',
       author='Volodymyr Savchenko',
       author_email='contact@volodymyrsavchenko.com',
       license='GPLv3',
       packages=['nb2workflow'],
       zip_safe=False,
```

### Comparing `nb2workflow-1.3.8/tests/conftest.py` & `nb2workflow-1.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/tests/test_nbadapter.py` & `nb2workflow-1.3.9/tests/test_nbadapter.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/tests/test_ontology.py` & `nb2workflow-1.3.9/tests/test_ontology.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/tests/test_run.py` & `nb2workflow-1.3.9/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/tests/test_service.py` & `nb2workflow-1.3.9/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `nb2workflow-1.3.8/tests/test_workflows.py` & `nb2workflow-1.3.9/tests/test_workflows.py`

 * *Files identical despite different names*

