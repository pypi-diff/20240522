# Comparing `tmp/setup_django_apex-0.1.0.tar.gz` & `tmp/setup_django_apex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup_django_apex-0.1.0.tar", last modified: Wed May 22 05:16:00 2024, max compression
+gzip compressed data, was "setup_django_apex-0.1.1.tar", last modified: Wed May 22 05:30:29 2024, max compression
```

## Comparing `setup_django_apex-0.1.0.tar` & `setup_django_apex-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 05:16:00.766220 setup_django_apex-0.1.0/
--rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      857 2024-05-22 05:16:00.760493 setup_django_apex-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 05:16:00.767009 setup_django_apex-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1117 2024-05-22 05:15:49.000000 setup_django_apex-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 05:16:00.724282 setup_django_apex-0.1.0/setup_django_apex/
--rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.0/setup_django_apex/__init__.py
--rw-rw-rw-   0        0        0     1892 2024-05-22 05:12:38.000000 setup_django_apex-0.1.0/setup_django_apex/installer.py
--rw-rw-rw-   0        0        0      191 2024-05-22 05:12:29.000000 setup_django_apex-0.1.0/setup_django_apex/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 05:16:00.758117 setup_django_apex-0.1.0/setup_django_apex.egg-info/
--rw-rw-rw-   0        0        0      857 2024-05-22 05:16:00.000000 setup_django_apex-0.1.0/setup_django_apex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2024-05-22 05:16:00.000000 setup_django_apex-0.1.0/setup_django_apex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 05:16:00.000000 setup_django_apex-0.1.0/setup_django_apex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 05:16:00.000000 setup_django_apex-0.1.0/setup_django_apex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-22 05:16:00.000000 setup_django_apex-0.1.0/setup_django_apex.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 05:16:00.752763 setup_django_apex-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.0/tests/mytest.py
--rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.0/tests/test_installer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.547876 setup_django_apex-0.1.1/
+-rw-rw-rw-   0        0        0     1174 2024-05-22 04:46:04.000000 setup_django_apex-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      857 2024-05-22 05:30:29.542948 setup_django_apex-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-22 04:34:11.000000 setup_django_apex-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 05:30:29.547876 setup_django_apex-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1117 2024-05-22 05:30:15.000000 setup_django_apex-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.499935 setup_django_apex-0.1.1/setup_django_apex/
+-rw-rw-rw-   0        0        0        0 2024-05-22 04:26:15.000000 setup_django_apex-0.1.1/setup_django_apex/__init__.py
+-rw-rw-rw-   0        0        0     1892 2024-05-22 05:12:38.000000 setup_django_apex-0.1.1/setup_django_apex/installer.py
+-rw-rw-rw-   0        0        0      281 2024-05-22 05:30:18.000000 setup_django_apex-0.1.1/setup_django_apex/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.538388 setup_django_apex-0.1.1/setup_django_apex.egg-info/
+-rw-rw-rw-   0        0        0      857 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      376 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-22 05:30:29.000000 setup_django_apex-0.1.1/setup_django_apex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 05:30:29.530849 setup_django_apex-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-22 03:09:42.000000 setup_django_apex-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     2111 2024-05-22 04:43:14.000000 setup_django_apex-0.1.1/tests/mytest.py
+-rw-rw-rw-   0        0        0     1195 2024-05-22 04:34:28.000000 setup_django_apex-0.1.1/tests/test_installer.py
```

### Comparing `setup_django_apex-0.1.0/LICENSE` & `setup_django_apex-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.0/PKG-INFO` & `setup_django_apex-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `setup_django_apex-0.1.0/setup.py` & `setup_django_apex-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class CustomInstallCommand(install):
     def run(self):
         install.run(self)
         subprocess.check_call(['python', '-m', 'setup_django_apex.installer'])
 
 setup(
     name='setup_django_apex',
-    version='0.1.0',
+    version='0.1.1',
     author='Anirudha Udgirkar',
     author_email='anirudhaudgirkar.work.email@example.com',
     description='A library to set up Django projects with multiple apps',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Anirudha1821/setup_django_apex',
     packages=find_packages(),
```

### Comparing `setup_django_apex-0.1.0/setup_django_apex/installer.py` & `setup_django_apex-0.1.1/setup_django_apex/installer.py`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.0/setup_django_apex.egg-info/PKG-INFO` & `setup_django_apex-0.1.1/setup_django_apex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup_django_apex
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to set up Django projects with multiple apps
 Home-page: https://github.com/Anirudha1821/setup_django_apex
 Author: Anirudha Udgirkar
 Author-email: anirudhaudgirkar.work.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `setup_django_apex-0.1.0/tests/mytest.py` & `setup_django_apex-0.1.1/tests/mytest.py`

 * *Files identical despite different names*

### Comparing `setup_django_apex-0.1.0/tests/test_installer.py` & `setup_django_apex-0.1.1/tests/test_installer.py`

 * *Files identical despite different names*

