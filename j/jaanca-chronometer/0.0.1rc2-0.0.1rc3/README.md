# Comparing `tmp/jaanca_chronometer-0.0.1rc2.tar.gz` & `tmp/jaanca_chronometer-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.0.1rc2.tar", last modified: Wed May 22 01:03:39 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.0.1rc3.tar", last modified: Wed May 22 01:19:40 2024, max compression
```

## Comparing `jaanca_chronometer-0.0.1rc2.tar` & `jaanca_chronometer-0.0.1rc3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.291732 jaanca_chronometer-0.0.1rc2/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/LICENSE.txt
--rw-rw-rw-   0        0        0     4480 2024-05-22 01:03:39.291732 jaanca_chronometer-0.0.1rc2/PKG-INFO
--rw-rw-rw-   0        0        0     3216 2024-05-22 01:02:56.000000 jaanca_chronometer-0.0.1rc2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.272710 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.283722 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.287723 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:03:39.289723 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     4480 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 01:03:39.000000 jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 01:03:39.293732 jaanca_chronometer-0.0.1rc2/setup.cfg
--rw-rw-rw-   0        0        0     1598 2024-05-22 01:03:18.000000 jaanca_chronometer-0.0.1rc2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.027385 jaanca_chronometer-0.0.1rc3/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/LICENSE.txt
+-rw-rw-rw-   0        0        0     4498 2024-05-22 01:19:40.026370 jaanca_chronometer-0.0.1rc3/PKG-INFO
+-rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.0.1rc3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.007658 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.017629 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.021366 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:19:40.025366 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     4498 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 01:19:39.000000 jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:19:40.029367 jaanca_chronometer-0.0.1rc3/setup.cfg
+-rw-rw-rw-   0        0        0     1627 2024-05-22 01:19:19.000000 jaanca_chronometer-0.0.1rc3/setup.py
```

### Comparing `jaanca_chronometer-0.0.1rc2/LICENSE.txt` & `jaanca_chronometer-0.0.1rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc2/PKG-INFO` & `jaanca_chronometer-0.0.1rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
-Home-page: https://github.com/jaanca/python-libraries
+Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -23,22 +23,19 @@
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
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
-
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
 
@@ -111,15 +108,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.0.1rc1] - 2024-05-21
+## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.0] - 2024-05-21
 ### Added
```

### Comparing `jaanca_chronometer-0.0.1rc2/README.md` & `jaanca_chronometer-0.0.1rc3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
----
-
-# What's libraries
+# What libraries
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
-
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
 
@@ -82,15 +79,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.0.1rc1] - 2024-05-21
+## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.0] - 2024-05-21
 ### Added
```

### Comparing `jaanca_chronometer-0.0.1rc2/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.0.1rc3/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.0.1rc2/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.0.1rc3/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.0.1rc2
+Version: 0.0.1rc3
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
-Home-page: https://github.com/jaanca/python-libraries
+Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -23,22 +23,19 @@
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
 
 * **Python library**: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 * **Analyze results in database**: The output format can be inserted in an INTERVAL attribute for example in PostgreSQL and add the time of several processes.
 
-
 ---
 
 # library installation
 ```console
 pip install jaanca-chronometer --upgrade
 ```
 
@@ -111,15 +108,15 @@
 - Added for new features.
 - Changed for changes in existing functionality.
 - Deprecated for soon-to-be removed features.
 - Removed for now removed features.
 - Fixed for any bug fixes.
 - Security in case of vulnerabilities.
 
-## [0.0.1rc1] - 2024-05-21
+## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
 ## [0.1.0] - 2024-05-21
 ### Added
```

### Comparing `jaanca_chronometer-0.0.1rc2/setup.py` & `jaanca_chronometer-0.0.1rc3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.0.1rc2"
+VERSION = "0.0.1rc3"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     author='Andres Cardona',
     author_email='jacardona@outlook.com',
-    url='https://github.com/jaanca/python-libraries',
+    url='https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer',
     keywords="timer stopwatch in interval format for databases",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
```

