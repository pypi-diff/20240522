# Comparing `tmp/jaanca-0.0.1rc2.tar.gz` & `tmp/jaanca-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.0.1rc2.tar", last modified: Wed May 22 01:13:38 2024, max compression
+gzip compressed data, was "jaanca-0.1.0.tar", last modified: Wed May 22 01:30:30 2024, max compression
```

## Comparing `jaanca-0.0.1rc2.tar` & `jaanca-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:13:38.433592 jaanca-0.0.1rc2/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca-0.0.1rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     1407 2024-05-22 01:13:38.432591 jaanca-0.0.1rc2/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-22 01:11:16.000000 jaanca-0.0.1rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 01:13:38.413580 jaanca-0.0.1rc2/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.0.1rc2/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:13:38.424593 jaanca-0.0.1rc2/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.0.1rc2/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:13:38.427594 jaanca-0.0.1rc2/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.0.1rc2/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.0.1rc2/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:13:38.431593 jaanca-0.0.1rc2/jaanca.egg-info/
--rw-rw-rw-   0        0        0     1407 2024-05-22 01:13:38.000000 jaanca-0.0.1rc2/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-22 01:13:38.000000 jaanca-0.0.1rc2/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:13:38.000000 jaanca-0.0.1rc2/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 01:13:38.000000 jaanca-0.0.1rc2/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 01:13:38.434598 jaanca-0.0.1rc2/setup.cfg
--rw-rw-rw-   0        0        0     1491 2024-05-22 01:13:27.000000 jaanca-0.0.1rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.041350 jaanca-0.1.0/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1412 2024-05-22 01:30:30.040349 jaanca-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-22 01:20:56.000000 jaanca-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.024632 jaanca-0.1.0/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.0/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.032642 jaanca-0.1.0/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.0/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.035641 jaanca-0.1.0/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.0/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.0/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.038348 jaanca-0.1.0/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     1412 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-22 01:30:30.000000 jaanca-0.1.0/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:30:30.042350 jaanca-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-05-22 01:29:32.000000 jaanca-0.1.0/setup.py
```

### Comparing `jaanca-0.0.1rc2/LICENSE.txt` & `jaanca-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca-0.0.1rc2/PKG-INFO` & `jaanca-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.0.1rc2
+Version: 0.1.0
 Summary: A tool library created by jaanca.
-Home-page: https://github.com/jaanca/python-libraries
+Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -23,17 +23,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
----
-
-# What's libraries
+# What libraries
 
 * **Python library**: A tool library created by jaanca.
 
 ---
 
 # Here is a non-exhaustive list of related packages:
```

### Comparing `jaanca-0.0.1rc2/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.0/jaanca/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca-0.0.1rc2/jaanca.egg-info/PKG-INFO` & `jaanca-0.1.0/jaanca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.0.1rc2
+Version: 0.1.0
 Summary: A tool library created by jaanca.
-Home-page: https://github.com/jaanca/python-libraries
+Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -23,17 +23,15 @@
 Classifier: Topic :: System :: Monitoring
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
----
-
-# What's libraries
+# What libraries
 
 * **Python library**: A tool library created by jaanca.
 
 ---
 
 # Here is a non-exhaustive list of related packages:
```

### Comparing `jaanca-0.0.1rc2/setup.py` & `jaanca-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.0.1rc2"
+VERSION = "0.1.0"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Andres Cardona',
     author_email='jacardona@outlook.com',
-    url='https://github.com/jaanca/python-libraries',
+    url='https://github.com/jaanca/python-libraries/tree/main/jaanca',
     keywords="python tools, libraries",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
```

