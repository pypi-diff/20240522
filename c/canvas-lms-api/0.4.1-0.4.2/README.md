# Comparing `tmp/canvas-lms-api-0.4.1.tar.gz` & `tmp/canvas-lms-api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/canvas-lms-api-0.4.1.tar", last modified: Mon Aug 24 22:59:32 2020, max compression
+gzip compressed data, was "canvas-lms-api-0.4.2.tar", last modified: Wed May 22 01:14:13 2024, max compression
```

## Comparing `canvas-lms-api-0.4.1.tar` & `canvas-lms-api-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 hotdog    (1000) hotdog    (1000)        0 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)     5019 2020-08-24 22:59:27.000000 canvas-lms-api-0.4.1/README.md
-drwxr-xr-x   0 hotdog    (1000) hotdog    (1000)        0 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)      282 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/SOURCES.txt
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)     6554 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/PKG-INFO
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)        1 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/dependency_links.txt
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)        9 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/requires.txt
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)       15 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api.egg-info/top_level.txt
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)      752 2020-08-24 22:58:55.000000 canvas-lms-api-0.4.1/setup.py
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)     6554 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/PKG-INFO
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)       38 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/setup.cfg
-drwxr-xr-x   0 hotdog    (1000) hotdog    (1000)        0 2020-08-24 22:59:32.000000 canvas-lms-api-0.4.1/canvas_lms_api/
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)     1248 2020-08-24 22:40:28.000000 canvas-lms-api-0.4.1/canvas_lms_api/test.py
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)    28894 2020-08-24 22:40:05.000000 canvas-lms-api-0.4.1/canvas_lms_api/canvas.py
--rw-r--r--   0 hotdog    (1000) hotdog    (1000)       41 2019-08-30 18:00:49.000000 canvas-lms-api-0.4.1/canvas_lms_api/__init__.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-22 01:14:13.429798 canvas-lms-api-0.4.2/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6554 2024-05-22 01:14:13.429798 canvas-lms-api-0.4.2/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)     5019 2024-05-22 01:14:10.000000 canvas-lms-api-0.4.2/README.md
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-22 01:14:13.425798 canvas-lms-api-0.4.2/canvas_lms_api/
+-rw-rw-r--   0 pi        (1000) pi        (1000)       42 2024-05-22 01:10:47.000000 canvas-lms-api-0.4.2/canvas_lms_api/__init__.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)    30216 2024-05-22 01:10:47.000000 canvas-lms-api-0.4.2/canvas_lms_api/canvas.py
+-rw-rw-r--   0 pi        (1000) pi        (1000)     1293 2024-05-22 01:10:47.000000 canvas-lms-api-0.4.2/canvas_lms_api/test.py
+drwxrwxr-x   0 pi        (1000) pi        (1000)        0 2024-05-22 01:14:13.429798 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/
+-rw-rw-r--   0 pi        (1000) pi        (1000)     6554 2024-05-22 01:14:13.000000 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/PKG-INFO
+-rw-rw-r--   0 pi        (1000) pi        (1000)      282 2024-05-22 01:14:13.000000 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        1 2024-05-22 01:14:13.000000 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)        9 2024-05-22 01:14:13.000000 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/requires.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       15 2024-05-22 01:14:13.000000 canvas-lms-api-0.4.2/canvas_lms_api.egg-info/top_level.txt
+-rw-rw-r--   0 pi        (1000) pi        (1000)       38 2024-05-22 01:14:13.429798 canvas-lms-api-0.4.2/setup.cfg
+-rw-rw-r--   0 pi        (1000) pi        (1000)      752 2024-05-22 01:14:10.000000 canvas-lms-api-0.4.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `canvas-lms-api-0.4.1/README.md` & `canvas-lms-api-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `canvas-lms-api-0.4.1/canvas_lms_api.egg-info/PKG-INFO` & `canvas-lms-api-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-lms-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pip installable canvas API used by GT classes
 Home-page: https://github.gatech.edu/omscs-ta/canvas_lms_api
 Author: Tyson Bailey
 Author-email: tyson@onaclovtech.com
 License: UNKNOWN
 Description: # Installation
```

### Comparing `canvas-lms-api-0.4.1/setup.py` & `canvas-lms-api-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="canvas-lms-api",
-    version="0.4.1",
+    version="0.4.2",
     author="Tyson Bailey",
     author_email="tyson@onaclovtech.com",
     description="Pip installable canvas API used by GT classes",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.gatech.edu/omscs-ta/canvas_lms_api",
 #    packages=setuptools.find_packages(),
```

### Comparing `canvas-lms-api-0.4.1/PKG-INFO` & `canvas-lms-api-0.4.2/canvas_lms_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-lms-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pip installable canvas API used by GT classes
 Home-page: https://github.gatech.edu/omscs-ta/canvas_lms_api
 Author: Tyson Bailey
 Author-email: tyson@onaclovtech.com
 License: UNKNOWN
 Description: # Installation
```

### Comparing `canvas-lms-api-0.4.1/canvas_lms_api/test.py` & `canvas-lms-api-0.4.2/canvas_lms_api/test.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-import yaml
-import os
-from canvas import Canvas
-import time
-import requests
-
-def load_config(path='.'):
-    _organization_name = "gatech"
-    config_file_name = _organization_name + "-conf.yml"
-    _config = ""
-    with open(os.path.join(path, config_file_name)) as config_file:
-        config = yaml.load(config_file)
-        _config= config
-    return _config
-
-
-_config = load_config(os.path.expanduser("~/.ta"))
-grader = Canvas(base=_config["base"], token=_config["canvas_api"], course=_config["canvas_course"])
-
-#for conference in grader.GetConferences():
-#    if len(conference["recordings"]) > 0:
-#        for i in conference["recordings"]:
-#            print (i["recording_id"])
-
-#student_id = str()
-#assignment_id = str(4683)
-#score = "75"
-#comment = "The student failed to complete the assignment\nAnd they got thse points wrong\n(-10) for poor guessing"
-#grader.SubmitGrade(assignment_id, student_id, score, comment, visibility=False)
- 
-
-print (grader.GetCourseModules(True))
-
-
-#for assignment in grader.GetAssignments():
-#   print (assignment)
-
-#for student in grader.GetCourseUsers():
-#    print (student)
-
-#print (grader.GetAllStudentUserNames())
-#x = grader.GetEmails()
-#for i in x:
-#    print (i)
-#print  (grader.GetExternalTools())
+import yaml
+import os
+from canvas import Canvas
+import time
+import requests
+
+def load_config(path='.'):
+    _organization_name = "gatech"
+    config_file_name = _organization_name + "-conf.yml"
+    _config = ""
+    with open(os.path.join(path, config_file_name)) as config_file:
+        config = yaml.load(config_file)
+        _config= config
+    return _config
+
+
+_config = load_config(os.path.expanduser("~/.ta"))
+grader = Canvas(base=_config["base"], token=_config["canvas_api"], course=_config["canvas_course"])
+
+#for conference in grader.GetConferences():
+#    if len(conference["recordings"]) > 0:
+#        for i in conference["recordings"]:
+#            print (i["recording_id"])
+
+#student_id = str()
+#assignment_id = str(4683)
+#score = "75"
+#comment = "The student failed to complete the assignment\nAnd they got thse points wrong\n(-10) for poor guessing"
+#grader.SubmitGrade(assignment_id, student_id, score, comment, visibility=False)
+ 
+
+print (grader.GetCourseModules(True))
+
+
+#for assignment in grader.GetAssignments():
+#   print (assignment)
+
+#for student in grader.GetCourseUsers():
+#    print (student)
+
+#print (grader.GetAllStudentUserNames())
+#x = grader.GetEmails()
+#for i in x:
+#    print (i)
+#print  (grader.GetExternalTools())
```

