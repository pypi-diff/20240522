# Comparing `tmp/heaserver_folders_aws_s3-1.1.5.tar.gz` & `tmp/heaserver_folders_aws_s3-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_folders_aws_s3-1.1.5.tar", last modified: Thu May  9 16:26:17 2024, max compression
+gzip compressed data, was "heaserver_folders_aws_s3-1.1.6.tar", last modified: Wed May 22 20:16:39 2024, max compression
```

## Comparing `heaserver_folders_aws_s3-1.1.5.tar` & `heaserver_folders_aws_s3-1.1.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.219562 heaserver_folders_aws_s3-1.1.5/
--rw-rw-rw-   0        0        0      261 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/.gitignore
--rw-rw-rw-   0        0        0     1664 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.5/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/LICENSE
--rw-rw-rw-   0        0        0      272 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6721 2024-05-09 16:26:17.218563 heaserver_folders_aws_s3-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5479 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/README.md
--rw-rw-rw-   0        0        0     1777 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/RELEASING.md
--rw-rw-rw-   0        0        0      658 2024-05-07 21:12:58.000000 heaserver_folders_aws_s3-1.1.5/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.053485 heaserver_folders_aws_s3-1.1.5/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.053485 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.128491 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    38201 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0    40185 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
--rw-rw-rw-   0        0        0    30533 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/test_all.py
--rw-rw-rw-   0        0        0      111 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/pytest.ini
--rw-rw-rw-   0        0        0      261 2023-11-06 17:01:54.000000 heaserver_folders_aws_s3-1.1.5/requirements_dev.txt
--rw-rw-rw-   0        0        0    14460 2024-03-11 17:23:33.000000 heaserver_folders_aws_s3-1.1.5/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-09 16:26:17.219562 heaserver_folders_aws_s3-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     2473 2024-05-09 16:17:34.000000 heaserver_folders_aws_s3-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.054485 heaserver_folders_aws_s3-1.1.5/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.158487 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0   154476 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/projectservice.py
--rw-rw-rw-   0        0        0   157027 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/service.py
--rw-rw-rw-   0        0        0     8385 2024-02-08 15:54:03.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/util.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.164492 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    33202 2024-05-08 14:18:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.217562 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     6721 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-09 16:26:17.000000 heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/tests/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.055485 heaserver_folders_aws_s3-1.1.5/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.209568 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2023-06-12 15:33:15.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    37459 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0    38816 2024-05-07 21:13:04.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/projectawss3testcase.py
--rw-rw-rw-   0        0        0     2608 2023-12-12 15:20:12.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2024-05-09 16:26:17.216562 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2023-06-12 16:27:45.000000 heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.273726 heaserver_folders_aws_s3-1.1.6/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.6/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/.gitignore
+-rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.6/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6958 2024-05-22 20:16:39.272725 heaserver_folders_aws_s3-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5716 2024-05-22 19:36:49.000000 heaserver_folders_aws_s3-1.1.6/README.md
+-rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/RELEASING.md
+-rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.208105 heaserver_folders_aws_s3-1.1.6/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.208105 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.239107 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    38201 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    40185 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
+-rw-rw-rw-   0        0        0    30533 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/test_all.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/pytest.ini
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/requirements_dev.txt
+-rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver_folders_aws_s3-1.1.6/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:16:39.273726 heaserver_folders_aws_s3-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2473 2024-05-22 20:15:59.000000 heaserver_folders_aws_s3-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.210106 heaserver_folders_aws_s3-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.209108 heaserver_folders_aws_s3-1.1.6/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.249108 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0   154476 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/projectservice.py
+-rw-rw-rw-   0        0        0   157027 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/service.py
+-rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/util.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.250106 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    33202 2024-05-22 19:25:52.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.271725 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     6958 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 20:16:39.000000 heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.211106 heaserver_folders_aws_s3-1.1.6/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.212106 heaserver_folders_aws_s3-1.1.6/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.267725 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    37459 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    38816 2024-04-09 21:50:01.000000 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/projectawss3testcase.py
+-rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:16:39.269724 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver_folders_aws_s3-1.1.5/Dockerfile` & `heaserver_folders_aws_s3-1.1.6/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/LICENSE` & `heaserver_folders_aws_s3-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/PKG-INFO` & `heaserver_folders_aws_s3-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.5
+Version: 1.1.6
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.6
+* Minor bug fixes.
+
+## Version 1.1.5
+* Made a project's unarchive restore duration required in the unarchive card.
+
+## Version 1.1.4
+* Made a folder's unarchive restore duration required in the unarchive card.
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_folders_aws_s3-1.1.5/README.md` & `heaserver_folders_aws_s3-1.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.6
+* Minor bug fixes.
+
+## Version 1.1.5
+* Made a project's unarchive restore duration required in the unarchive card.
+
+## Version 1.1.4
+* Made a folder's unarchive restore duration required in the unarchive card.
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_folders_aws_s3-1.1.5/RELEASING.md` & `heaserver_folders_aws_s3-1.1.6/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/docker-entrypoint.sh` & `heaserver_folders_aws_s3-1.1.6/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/integrationtests/heaserver/folderawss3integrationtest/test_all.py` & `heaserver_folders_aws_s3-1.1.6/integrationtests/heaserver/folderawss3integrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/run-swaggerui.py` & `heaserver_folders_aws_s3-1.1.6/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/setup.py` & `heaserver_folders_aws_s3-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.1.5',
+                 version='1.1.6',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.folderawss3'],
                  package_data={'heaserver.folderawss3': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.5.3'
+                     'heaserver~=1.6.0'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/projectservice.py` & `heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/projectservice.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/service.py` & `heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/util.py` & `heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/util.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver/folderawss3/wstl/all.json` & `heaserver_folders_aws_s3-1.1.6/src/heaserver/folderawss3/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.1.5
+Version: 1.1.6
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.6
+* Minor bug fixes.
+
+## Version 1.1.5
+* Made a project's unarchive restore duration required in the unarchive card.
+
+## Version 1.1.4
+* Made a folder's unarchive restore duration required in the unarchive card.
+
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
 
 ## Version 1.1.2
 * Fixed new folder form submission.
 
 ## Version 1.1.1
```

### Comparing `heaserver_folders_aws_s3-1.1.5/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver_folders_aws_s3-1.1.6/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/projectawss3testcase.py` & `heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/projectawss3testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/test_all.py` & `heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_folders_aws_s3-1.1.5/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver_folders_aws_s3-1.1.6/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*

