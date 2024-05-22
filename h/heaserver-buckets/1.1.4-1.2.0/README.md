# Comparing `tmp/heaserver_buckets-1.1.4.tar.gz` & `tmp/heaserver_buckets-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_buckets-1.1.4.tar", last modified: Tue May  7 20:34:21 2024, max compression
+gzip compressed data, was "heaserver_buckets-1.2.0.tar", last modified: Wed May 22 18:41:16 2024, max compression
```

## Comparing `heaserver_buckets-1.1.4.tar` & `heaserver_buckets-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.447635 heaserver_buckets-1.1.4/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/.gitignore
--rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     5486 2024-05-07 20:34:21.446243 heaserver_buckets-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4112 2024-05-07 20:27:59.000000 heaserver_buckets-1.1.4/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/RELEASING.md
--rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.304543 heaserver_buckets-1.1.4/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.304543 heaserver_buckets-1.1.4/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.387578 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    10949 2024-05-07 18:50:12.000000 heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/requirements_dev.txt
--rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-07 20:34:21.447635 heaserver_buckets-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1858 2024-05-07 20:33:25.000000 heaserver_buckets-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.306542 heaserver_buckets-1.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.305544 heaserver_buckets-1.1.4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.392028 heaserver_buckets-1.1.4/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    73812 2024-05-07 18:19:20.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.393598 heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0    14793 2024-04-09 21:37:15.000000 heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.444697 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     5486 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 20:34:21.000000 heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.307542 heaserver_buckets-1.1.4/tests/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.307542 heaserver_buckets-1.1.4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-07 20:34:21.443073 heaserver_buckets-1.1.4/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     9195 2024-05-07 18:49:58.000000 heaserver_buckets-1.1.4/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.199686 heaserver_buckets-1.2.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5712 2024-05-22 18:41:16.197688 heaserver_buckets-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4371 2024-05-22 18:39:02.000000 heaserver_buckets-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/RELEASING.md
+-rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.034895 heaserver_buckets-1.2.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.035411 heaserver_buckets-1.2.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.120621 heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    10949 2024-05-07 20:36:00.000000 heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:41:16.199686 heaserver_buckets-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2024-05-22 18:39:19.000000 heaserver_buckets-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.037472 heaserver_buckets-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.036444 heaserver_buckets-1.2.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.135148 heaserver_buckets-1.2.0/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    74684 2024-05-22 18:33:17.000000 heaserver_buckets-1.2.0/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.138245 heaserver_buckets-1.2.0/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0    14793 2024-04-09 21:37:15.000000 heaserver_buckets-1.2.0/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.193572 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     5712 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 18:41:16.000000 heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.038499 heaserver_buckets-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.038797 heaserver_buckets-1.2.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:41:16.193572 heaserver_buckets-1.2.0/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver_buckets-1.2.0/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     9195 2024-05-07 20:36:00.000000 heaserver_buckets-1.2.0/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver_buckets-1.1.4/Dockerfile` & `heaserver_buckets-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/LICENSE` & `heaserver_buckets-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/PKG-INFO` & `heaserver_buckets-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.4
+Version: 1.2.0
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,23 +21,27 @@
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
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.2.0
+* Added deletecontents query parameter the bucket delete endpoint. If true/yes/y, requesting a bucket delete will
+delete the bucket's contents first. If false/no/n or omitted, the bucket delete will succeed only if the bucket is
+empty.
+
 ## Version 1.1.4
 * Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
 users without permissions to delete buckets).
 
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
```

### Comparing `heaserver_buckets-1.1.4/README.md` & `heaserver_buckets-1.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.2.0
+* Added deletecontents query parameter the bucket delete endpoint. If true/yes/y, requesting a bucket delete will
+delete the bucket's contents first. If false/no/n or omitted, the bucket delete will succeed only if the bucket is
+empty.
+
 ## Version 1.1.4
 * Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
 users without permissions to delete buckets).
 
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
```

### Comparing `heaserver_buckets-1.1.4/RELEASING.md` & `heaserver_buckets-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/test_all.py` & `heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver_buckets-1.2.0/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/run-swaggerui.py` & `heaserver_buckets-1.2.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/setup.py` & `heaserver_buckets-1.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.1.4',
+    version='1.2.0',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.bucket'],
     package_data={'heaserver.bucket': ['wstl/*.json']},
-    install_requires=['heaserver~=1.5.3', 'heaobject~=1.5.1'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_buckets-1.1.4/src/heaserver/bucket/service.py` & `heaserver_buckets-1.2.0/src/heaserver/bucket/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from heaobject.project import AWSS3Project
 from heaobject.volume import AWSFileSystem
 from heaobject.bucket import AWSBucket
 from heaobject.error import DeserializeException
 from heaobject.root import Tag, ShareImpl, Permission
 from heaobject.activity import Status
 from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
+from heaobject.util import parse_bool
 from heaserver.service.appproperty import HEA_CACHE
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.heaobjectsupport import new_heaobject_from_type, type_to_resource_url
 from heaserver.service.sources import AWS_S3
 from heaserver.service.messagebroker import publish_desktop_object, publisher_cleanup_context_factory
 from heaserver.service.activity import DesktopObjectActionLifecycle
 from botocore.exceptions import ClientError as BotoClientError
@@ -377,15 +378,15 @@
       '400':
         $ref: '#/components/responses/400'
       '404':
         $ref: '#/components/responses/404'
     """
     volume_id = request.match_info['volume_id']
     bucket_id = request.match_info['bucket_id']
-    folder_url = await type_to_resource_url(request, AWSS3Folder, file_system_type_or_type_name=AWSFileSystem)
+    folder_url = await type_to_resource_url(request, AWSS3Folder)
     if folder_url is None:
         raise ValueError('No AWSS3Folder service registered')
     headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
     resource_base = str(URL(folder_url) / volume_id / 'buckets' / bucket_id / 'awss3folders' / 'root' / 'newfolder')
     folder = await new_heaobject_from_type(request, type_=AWSS3Folder)
     try:
         id_ = await client.post(request.app, resource_base, data=folder, headers=headers)
@@ -468,15 +469,15 @@
       '400':
         $ref: '#/components/responses/400'
       '404':
         $ref: '#/components/responses/404'
     """
     volume_id = request.match_info['volume_id']
     bucket_id = request.match_info['bucket_id']
-    project_url = await type_to_resource_url(request, AWSS3Project, file_system_type_or_type_name=AWSFileSystem)
+    project_url = await type_to_resource_url(request, AWSS3Project)
     if project_url is None:
         raise ValueError('No AWSS3Project service registered')
     headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
     resource_base = str(URL(project_url) / volume_id / 'buckets' / bucket_id / 'awss3projects')
     project = await new_heaobject_from_type(request, type_=AWSS3Project)
     try:
         id_ = await client.post(request.app, resource_base, data=project, headers=headers)
@@ -559,15 +560,15 @@
         $ref: '#/components/responses/400'
       '404':
         $ref: '#/components/responses/404'
     """
     volume_id = request.match_info['volume_id']
     bucket_id = request.match_info['id']
 
-    folder_url = await type_to_resource_url(request, AWSS3Folder, file_system_type_or_type_name=AWSFileSystem)
+    folder_url = await type_to_resource_url(request, AWSS3Folder)
     if folder_url is None:
         raise ValueError('No AWSS3Folder service registered')
     headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
 
     resource_base = str(URL(folder_url) / volume_id / 'buckets' / bucket_id / 'awss3folders' / 'root' / 'uploader')
     logging.info(f"This is the url to reach the folder service from the bucket\n{resource_base}")
     # posting to root of bucket with file template
@@ -1239,15 +1240,18 @@
 
 
 
 
 @routes.delete('/volumes/{volume_id}/buckets/{id}')
 async def delete_bucket(request: web.Request) -> web.Response:
     """
-    Deletes the bucket with the specified id.
+    Deletes the bucket with the specified id. The bucket must be empty. If the bucket is versioned, then there can be
+    no objects with delete markers in the bucket either. Setting the deletecontents query parameter to y, yes, or true
+    will delete the bucket's contents, including any deleted versions, and then delete the bucket.
+
     :param request: the HTTP request.
     :return: No Content or Not Found.
     ---
     summary: A specific bucket.
     tags:
         - heaserver-buckets
     parameters:
@@ -1263,14 +1267,23 @@
           description: The id of the user's AWS volume.
           schema:
             type: string
           examples:
             example:
               summary: A volume id
               value: 666f6f2d6261722d71757578
+        - name: deletecontents
+          in: query
+          description: flag whether to delete the bucket's contents before deleting the bucket.
+          schema:
+            type: boolean
+          examples:
+            example:
+              summary: The default value
+              value: false
     responses:
       '200':
         description: Expected response to a valid request.
         content:
             application/json:
                 schema:
                     type: array
@@ -1288,14 +1301,15 @@
                         type: object
       '404':
         $ref: '#/components/responses/404'
     """
     sub = request.headers.get(SUB, NONE_USER)
     volume_id = request.match_info.get("volume_id", None)
     bucket_id = request.match_info.get("id", None)
+    delete_contents = parse_bool(request.query.get('deletecontents'))
     if not volume_id:
         return web.HTTPBadRequest(body="volume_id is required")
     if not bucket_id:
         return web.HTTPBadRequest(body="bucket_id is required")
     loop = asyncio.get_running_loop()
     async with DesktopObjectActionLifecycle(request=request,
                                                 code='hea-delete',
@@ -1303,15 +1317,16 @@
                                                 activity_cb=publish_desktop_object) as activity:
         activity.old_object_id = bucket_id
         activity.old_object_uri = f'volumes/{volume_id}/buckets/{bucket_id}'
         activity.old_object_type_name = AWSBucket.get_type_name()
         activity.old_volume_id = volume_id
         async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
             try:
-                await _delete_bucket_objects(s3_client, bucket_id)
+                if delete_contents:
+                    await _delete_bucket_objects(s3_client, bucket_id, delete_versions=True)
                 await loop.run_in_executor(None, partial(s3_client.delete_bucket, Bucket=bucket_id))
                 request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, 'head'), None)
                 request.app[HEA_CACHE].pop((sub, volume_id, None, 'items'), None)
                 request.app[HEA_CACHE].pop((sub, volume_id, None, 'actual'), None)
                 request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, 'actual'), None)
                 return web.HTTPNoContent()
             except BotoClientError as e:
@@ -1324,23 +1339,25 @@
                            default_port=8080)
     start(package_name='heaserver-buckets', db=aws.S3Manager,
           wstl_builder_factory=builder_factory(__package__),
           cleanup_ctx=[publisher_cleanup_context_factory(config)],
           config=config)
 
 
-async def _delete_bucket_objects(s3_client: S3Client, bucket_name: str,
-                                 delete_versions: bool = False) -> None:
+async def _delete_bucket_objects(s3_client: S3Client, bucket_name: str, delete_versions=False, fail_if_not_empty=False) -> None:
     """
-    Deletes all objects inside a bucket. Assumes the bucket exists.
+    Deletes all objects inside a bucket, assuming the bucket exists.
 
     :param request: the aiohttp Request (required).
     :param volume_id: the id string of the volume representing the user's AWS account.
     :param bucket_name: Bucket to delete
-    :param delete_versions: Boolean indicating if the versioning should be deleted as well, defaults to False
+    :param delete_versions: Boolean indicating if the versioning should be deleted as well, defaults to False. For
+    versioned buckets, this flag must be set to True or subsequently attempting to delete the bucket will fail.
+    :raises BotoClientError: if the bucket does not exist, or another error occurred while deleting the bucket's
+    contents.
     """
     loop = asyncio.get_running_loop()
     if delete_versions:
         bucket_versioning = await loop.run_in_executor(None, partial(s3_client.get_bucket_versioning, Bucket=bucket_name))
         if bucket_versioning['Status'] == 'Enabled':
             object_response_paginator = await loop.run_in_executor(None, s3_client.get_paginator, 'list_object_versions')
```

### Comparing `heaserver_buckets-1.1.4/src/heaserver/bucket/wstl/all.json` & `heaserver_buckets-1.2.0/src/heaserver/bucket/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.1.4
+Version: 1.2.0
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,23 +21,27 @@
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
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.2.0
+* Added deletecontents query parameter the bucket delete endpoint. If true/yes/y, requesting a bucket delete will
+delete the bucket's contents first. If false/no/n or omitted, the bucket delete will succeed only if the bucket is
+empty.
+
 ## Version 1.1.4
 * Grant all users DELETER privileges to buckets so that the webclient permits deletion (the backend will still deny
 users without permissions to delete buckets).
 
 ## Version 1.1.3
 * Fixed potential issue preventing the service from updating temporary credentials.
```

### Comparing `heaserver_buckets-1.1.4/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver_buckets-1.2.0/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/tests/heaserver/buckettest/test_all.py` & `heaserver_buckets-1.2.0/tests/heaserver/buckettest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_buckets-1.1.4/tests/heaserver/buckettest/testcase.py` & `heaserver_buckets-1.2.0/tests/heaserver/buckettest/testcase.py`

 * *Files identical despite different names*

