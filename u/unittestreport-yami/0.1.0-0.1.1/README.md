# Comparing `tmp/unittestreport_yami-0.1.0.tar.gz` & `tmp/unittestreport_yami-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittestreport_yami-0.1.0.tar", last modified: Wed May 22 03:19:30 2024, max compression
+gzip compressed data, was "unittestreport_yami-0.1.1.tar", last modified: Wed May 22 05:43:20 2024, max compression
```

## Comparing `unittestreport_yami-0.1.0.tar` & `unittestreport_yami-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.715623 unittestreport_yami-0.1.0/
--rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2111 2024-05-22 03:19:30.713615 unittestreport_yami-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 03:19:30.716618 unittestreport_yami-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      714 2024-05-22 03:19:15.000000 unittestreport_yami-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.659612 unittestreport_yami-0.1.0/unittestreport_yami/
--rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.0/unittestreport_yami/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.699616 unittestreport_yami-0.1.0/unittestreport_yami/core/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/__init__.py
--rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/dataDriver.py
--rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/parameterized.py
--rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/reRun.py
--rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/resultPush.py
--rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/sendEmail.py
--rw-rw-rw-   0        0        0     7090 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/testResult.py
--rw-rw-rw-   0        0        0    12904 2024-05-22 02:30:51.000000 unittestreport_yami-0.1.0/unittestreport_yami/core/testRunner.py
-drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.709611 unittestreport_yami-0.1.0/unittestreport_yami/templates/
--rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/__init__.py
--rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/dingtalk.md
--rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates.html
--rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates03.html
--rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates2.html
--rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.0/unittestreport_yami/templates/templates3.html
-drwxrwxrwx   0        0        0        0 2024-05-22 03:19:30.683613 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/
--rw-rw-rw-   0        0        0     2111 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      859 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-22 03:19:30.000000 unittestreport_yami-0.1.0/unittestreport_yami.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 05:43:20.467932 unittestreport_yami-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2111 2024-05-22 05:43:20.466328 unittestreport_yami-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1686 2024-05-22 03:00:51.000000 unittestreport_yami-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 05:43:20.467932 unittestreport_yami-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      714 2024-05-22 05:43:17.000000 unittestreport_yami-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:43:20.353884 unittestreport_yami-0.1.1/unittestreport_yami/
+-rw-rw-rw-   0        0        0      145 2024-05-22 02:31:24.000000 unittestreport_yami-0.1.1/unittestreport_yami/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:43:20.443179 unittestreport_yami-0.1.1/unittestreport_yami/core/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/__init__.py
+-rw-rw-rw-   0        0        0     2755 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/dataDriver.py
+-rw-rw-rw-   0        0        0    22987 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/parameterized.py
+-rw-rw-rw-   0        0        0     1009 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/reRun.py
+-rw-rw-rw-   0        0        0     4996 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/resultPush.py
+-rw-rw-rw-   0        0        0     2500 2024-05-22 02:30:52.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/sendEmail.py
+-rw-rw-rw-   0        0        0     7000 2024-05-22 05:42:46.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/testResult.py
+-rw-rw-rw-   0        0        0    12904 2024-05-22 02:30:51.000000 unittestreport_yami-0.1.1/unittestreport_yami/core/testRunner.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:43:20.462331 unittestreport_yami-0.1.1/unittestreport_yami/templates/
+-rw-rw-rw-   0        0        0        0 2024-05-22 02:30:53.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/__init__.py
+-rw-rw-rw-   0        0        0      318 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/dingtalk.md
+-rw-rw-rw-   0        0        0    18656 2024-04-05 03:28:31.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/templates.html
+-rw-rw-rw-   0        0        0     2464 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/templates03.html
+-rw-rw-rw-   0        0        0    25462 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/templates2.html
+-rw-rw-rw-   0        0        0   197083 2024-04-05 03:24:28.000000 unittestreport_yami-0.1.1/unittestreport_yami/templates/templates3.html
+drwxrwxrwx   0        0        0        0 2024-05-22 05:43:20.417221 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/
+-rw-rw-rw-   0        0        0     2111 2024-05-22 05:43:19.000000 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      859 2024-05-22 05:43:20.000000 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 05:43:19.000000 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-22 05:43:19.000000 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-22 05:43:19.000000 unittestreport_yami-0.1.1/unittestreport_yami.egg-info/top_level.txt
```

### Comparing `unittestreport_yami-0.1.0/LICENSE` & `unittestreport_yami-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/PKG-INFO` & `unittestreport_yami-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport_yami
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.0/README.md` & `unittestreport_yami-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/setup.py` & `unittestreport_yami-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 setup(
     name="unittestreport_yami",
-    version="0.1.0",
+    version="0.1.1",
     author="Ethan",
     author_email="ethan.liu@yamibuy.com",
     url="https://github.com/EthanLiuInyami/UnitTestReport",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["Jinja2==3.0.3", "PyYAML==5.3.1", "requests==2.32.2"],
```

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/dataDriver.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/dataDriver.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/parameterized.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/parameterized.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/reRun.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/reRun.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/resultPush.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/resultPush.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/sendEmail.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/sendEmail.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/testResult.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/testResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,14 @@
             test.run(self)
         else:
             super().addFailure(test, err)
             if test.count != 0:
                 sys.stderr.write(
                     f"================重运行{test.count}次完毕================\n"
                 )
-        self._add_screen_shot_in_test(test)
 
     def addError(self, test, err):
         if not hasattr(test, "count"):
             test.count = 0
         if test.count < self.count:
             test.count += 1
             sys.stderr.write("{}执行——>【错误Error】\n".format(test))
@@ -209,8 +208,7 @@
             test.run(self)
         else:
             super().addError(test, err)
             if test.count != 0:
                 sys.stderr.write(
                     f"================重运行{test.count}次完毕================\n"
                 )
-        self._add_screen_shot_in_test(test)
```

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/core/testRunner.py` & `unittestreport_yami-0.1.1/unittestreport_yami/core/testRunner.py`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates.html` & `unittestreport_yami-0.1.1/unittestreport_yami/templates/templates.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates03.html` & `unittestreport_yami-0.1.1/unittestreport_yami/templates/templates03.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates2.html` & `unittestreport_yami-0.1.1/unittestreport_yami/templates/templates2.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami/templates/templates3.html` & `unittestreport_yami-0.1.1/unittestreport_yami/templates/templates3.html`

 * *Files identical despite different names*

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami.egg-info/PKG-INFO` & `unittestreport_yami-0.1.1/unittestreport_yami.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittestreport-yami
-Version: 0.1.0
+Version: 0.1.1
 Home-page: https://github.com/EthanLiuInyami/UnitTestReport
 Author: Ethan
 Author-email: ethan.liu@yamibuy.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `unittestreport_yami-0.1.0/unittestreport_yami.egg-info/SOURCES.txt` & `unittestreport_yami-0.1.1/unittestreport_yami.egg-info/SOURCES.txt`

 * *Files identical despite different names*

