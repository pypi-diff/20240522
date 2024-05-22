# Comparing `tmp/unittestreport_yami-0.1.2.tar.gz` & `tmp/unittestreport_yami-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.1.2.tar", last modified: Wed May 22 07:07:29 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.3.tar", last modified: Wed May 22 07:21:04 2024, max compression
```

## Comparing `unittestreport_yami-0.1.2.tar` & `unittestreport_yami-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:07:29.261409 unittestreport_yami-0.1.2/
--rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2111 2024-05-22 07:07:29.257019 unittestreport_yami-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 07:07:29.261409 unittestreport_yami-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-22 07:07:26.000000 unittestreport_yami-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:07:29.200329 unittestreport_yami-0.1.2/unittestreport_yami/
--rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.2/unittestreport_yami/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:07:29.245278 unittestreport_yami-0.1.2/unittestreport_yami/core/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/parameterized.py
--rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/reRun.py
--rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/resultPush.py
--rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/sendEmail.py
--rw-rw-rw-   0        0        0     6998 2024-05-22 06:25:58.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/testResult.py
--rw-rw-rw-   0        0        0    12886 2024-05-22 06:26:24.000000 unittestreport_yami-0.1.2/unittestreport_yami/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:07:29.256906 unittestreport_yami-0.1.2/unittestreport_yami/templates/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/dingtalk.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.2/unittestreport_yami/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-05-22 07:07:29.228132 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2111 2024-05-22 07:07:29.000000 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2024-05-22 07:07:29.000000 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:07:29.000000 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-22 07:07:29.000000 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-22 07:07:29.000000 unittestreport_yami-0.1.2/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:04.126145 unittestreport_yami-0.1.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-22 07:21:04.126145 unittestreport_yami-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:21:04.132997 unittestreport_yami-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-22 07:20:19.000000 unittestreport_yami-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:04.032635 unittestreport_yami-0.1.3/unittestreport_yami/
+-rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.3/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:04.106941 unittestreport_yami-0.1.3/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     6999 2024-05-22 07:19:43.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    12886 2024-05-22 06:26:24.000000 unittestreport_yami-0.1.3/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:04.126145 unittestreport_yami-0.1.3/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.3/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:04.060060 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-22 07:21:03.000000 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2024-05-22 07:21:03.000000 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:21:03.000000 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-22 07:21:03.000000 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-22 07:21:03.000000 unittestreport_yami-0.1.3/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.1.2/LICENSE` & `unittestreport_yami-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/PKG-INFO` & `unittestreport_yami-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.2/README.md` & `unittestreport_yami-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/setup.py` & `unittestreport_yami-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="unittestreport_yami",
-    version="0.1.2",
+    version="0.1.3",
     author="Ethan",
     author_email="ethan.liu@yamibuy.com",
     url="https://github.com/EthanLiuInyami/UnitTestReport",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["Jinja2==3.0.3", "PyYAML==5.3.1", "requests==2.32.2"],
```

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/dataDriver.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/parameterized.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/reRun.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/reRun.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/resultPush.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/resultPush.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/sendEmail.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/sendEmail.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/testResult.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/testResult.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             sys.stdout = self.sys_stdout
             sys.stderr = self.sys_stderr
             self.sys_stdout = None
             self.sys_stderr = None
         return self.outputBuffer.getvalue()
 
     def stopTest(self, test):
-        test.run_time = "{:.2f}s".format(time.time() - self.starttime)
+        test.run_time = "{:.2f}s".format(time.time() - self.start_time)
         test.class_name = test.__class__.__qualname__
         test.method_name = test.__dict__["_testMethodName"]
         test.method_doc = test.shortDescription()
         self.fields["results"].append(test)
         self.fields["testClass"].add(test.class_name)
         self.complete_output()
```

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/core/testRunner.py` & `unittestreport_yami-0.1.3/unittestreport_yami/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/templates/templates.html` & `unittestreport_yami-0.1.3/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/templates/templates03.html` & `unittestreport_yami-0.1.3/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/templates/templates2.html` & `unittestreport_yami-0.1.3/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami/templates/templates3.html` & `unittestreport_yami-0.1.3/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.3/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.2/unittestreport_yami.egg-info/SOURCES.txt` & `unittestreport_yami-0.1.3/unittestreport_yami.egg-info/SOURCES.txt`

 * *Files identical despite different names*
