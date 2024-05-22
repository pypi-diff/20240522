# Comparing `tmp/heaserver_trash_aws_s3-1.1.1.tar.gz` & `tmp/heaserver_trash_aws_s3-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_trash_aws_s3-1.1.1.tar", last modified: Sun May  5 21:00:06 2024, max compression
+gzip compressed data, was "heaserver_trash_aws_s3-1.1.2.tar", last modified: Wed May 22 21:03:22 2024, max compression
```

## Comparing `heaserver_trash_aws_s3-1.1.1.tar` & `heaserver_trash_aws_s3-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.438165 heaserver_trash_aws_s3-1.1.1/
--rw-rw-rw-   0        0        0    11625 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.1/LICENSE
--rw-rw-rw-   0        0        0       39 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4699 2024-05-05 21:00:06.437165 heaserver_trash_aws_s3-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3297 2024-05-05 20:54:54.000000 heaserver_trash_aws_s3-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-05 21:00:06.439164 heaserver_trash_aws_s3-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1967 2024-05-05 20:59:19.000000 heaserver_trash_aws_s3-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.383163 heaserver_trash_aws_s3-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.382194 heaserver_trash_aws_s3-1.1.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.392165 heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/
--rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/__init__.py
--rw-rw-rw-   0        0        0    54229 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/service.py
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.395172 heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/wstl/
--rw-rw-rw-   0        0        0     7918 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.436166 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     4699 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 21:00:06.000000 heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.384205 heaserver_trash_aws_s3-1.1.1/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.384205 heaserver_trash_aws_s3-1.1.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 21:00:06.434165 heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/
--rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/__init__.py
--rw-rw-rw-   0        0        0    73394 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/test_all.py
--rw-rw-rw-   0        0        0     6372 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.253119 heaserver_trash_aws_s3-1.1.2/
+-rw-rw-rw-   0        0        0    11625 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4706 2024-05-22 21:03:22.252119 heaserver_trash_aws_s3-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3337 2024-05-22 19:44:35.000000 heaserver_trash_aws_s3-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 21:03:22.253119 heaserver_trash_aws_s3-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1947 2024-05-22 21:02:35.000000 heaserver_trash_aws_s3-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.178353 heaserver_trash_aws_s3-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.177355 heaserver_trash_aws_s3-1.1.2/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.196249 heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/
+-rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/__init__.py
+-rw-rw-rw-   0        0        0    54229 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.197248 heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/wstl/
+-rw-rw-rw-   0        0        0     7918 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.251119 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     4706 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 21:03:22.000000 heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.178353 heaserver_trash_aws_s3-1.1.2/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.179353 heaserver_trash_aws_s3-1.1.2/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 21:03:22.249118 heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/
+-rw-rw-rw-   0        0        0        0 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/__init__.py
+-rw-rw-rw-   0        0        0    73394 2024-04-18 15:25:48.000000 heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/test_all.py
+-rw-rw-rw-   0        0        0     6372 2023-12-18 21:53:00.000000 heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/testcase.py
```

### Comparing `heaserver_trash_aws_s3-1.1.1/LICENSE` & `heaserver_trash_aws_s3-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_trash_aws_s3-1.1.1/PKG-INFO` & `heaserver_trash_aws_s3-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.1.1
+Version: 1.1.2
 Summary: Deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,24 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
-Requires-Dist: heaobject~=1.5.1
+Requires-Dist: heaserver~=1.6.0
 Requires-Dist: aiostream~=0.5.1
 
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.2
+* Minor bug fixes.
+
 ## Version 1.1.1
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.0
 * Added "deleted" date to trash items from their delete marker
 * Return permissions in Collection+JSON objects.
 * Added type_display_name attribute to returned objects.
```

### Comparing `heaserver_trash_aws_s3-1.1.1/README.md` & `heaserver_trash_aws_s3-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.2
+* Minor bug fixes.
+
 ## Version 1.1.1
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.0
 * Added "deleted" date to trash items from their delete marker
 * Return permissions in Collection+JSON objects.
 * Added type_display_name attribute to returned objects.
```

### Comparing `heaserver_trash_aws_s3-1.1.1/setup.py` & `heaserver_trash_aws_s3-1.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-trash-aws-s3',
-    version='1.1.1',
+    version='1.1.2',
     description="Deleted file management",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=['heaserver.trashawss3'],
       package_data={'heaserver.trashawss3': ['wstl/*.json']},
       install_requires=[
-          'heaserver~=1.5.3', 'heaobject~=1.5.1',
+          'heaserver~=1.6.0',
           'aiostream~=0.5.1'
       ],
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Environment :: Console',
           'Intended Audience :: Developers',
           'Natural Language :: English',
```

### Comparing `heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/service.py` & `heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_trash_aws_s3-1.1.1/src/heaserver/trashawss3/wstl/all.json` & `heaserver_trash_aws_s3-1.1.2/src/heaserver/trashawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/PKG-INFO` & `heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-trash-aws-s3
-Version: 1.1.1
+Version: 1.1.2
 Summary: Deleted file management
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-trash-aws-s3,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -21,24 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
-Requires-Dist: heaobject~=1.5.1
+Requires-Dist: heaserver~=1.6.0
 Requires-Dist: aiostream~=0.5.1
 
 # HEA Trash Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Trash Microservice is deleted file management.
 
+## Version 1.1.2
+* Minor bug fixes.
+
 ## Version 1.1.1
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.0
 * Added "deleted" date to trash items from their delete marker
 * Return permissions in Collection+JSON objects.
 * Added type_display_name attribute to returned objects.
```

### Comparing `heaserver_trash_aws_s3-1.1.1/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt` & `heaserver_trash_aws_s3-1.1.2/src/heaserver_trash_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/test_all.py` & `heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_trash_aws_s3-1.1.1/tests/heaserver/trashawss3test/testcase.py` & `heaserver_trash_aws_s3-1.1.2/tests/heaserver/trashawss3test/testcase.py`

 * *Files identical despite different names*

