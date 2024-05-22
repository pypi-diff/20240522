# Comparing `tmp/heaserver_accounts-1.1.3.tar.gz` & `tmp/heaserver_accounts-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_accounts-1.1.3.tar", last modified: Sun May  5 19:43:17 2024, max compression
+gzip compressed data, was "heaserver_accounts-1.2.0.tar", last modified: Wed May 22 16:09:18 2024, max compression
```

## Comparing `heaserver_accounts-1.1.3.tar` & `heaserver_accounts-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.745172 heaserver_accounts-1.1.3/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/.gitignore
--rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6091 2024-05-05 19:43:17.744173 heaserver_accounts-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4783 2024-05-05 18:21:28.000000 heaserver_accounts-1.1.3/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/RELEASING.md
--rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.522235 heaserver_accounts-1.1.3/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.523238 heaserver_accounts-1.1.3/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.638413 heaserver_accounts-1.1.3/integrationtests/heaserver/accountintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/integrationtests/heaserver/accountintegrationtest/__init__.py
--rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/integrationtests/heaserver/accountintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7797 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.3/integrationtests/heaserver/accountintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/requirements_dev.txt
--rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-05 19:43:17.746175 heaserver_accounts-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1825 2024-05-05 19:42:28.000000 heaserver_accounts-1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.525235 heaserver_accounts-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.524237 heaserver_accounts-1.1.3/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.655517 heaserver_accounts-1.1.3/src/heaserver/account/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/src/heaserver/account/__init__.py
--rw-rw-rw-   0        0        0    47097 2024-05-03 22:13:10.000000 heaserver_accounts-1.1.3/src/heaserver/account/service.py
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.668516 heaserver_accounts-1.1.3/src/heaserver/account/wstl/
--rw-rw-rw-   0        0        0    11957 2024-05-03 03:06:58.000000 heaserver_accounts-1.1.3/src/heaserver/account/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.742175 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/
--rw-rw-rw-   0        0        0     6091 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-05 19:43:17.000000 heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.526235 heaserver_accounts-1.1.3/tests/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.526235 heaserver_accounts-1.1.3/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-05 19:43:17.740172 heaserver_accounts-1.1.3/tests/heaserver/accounttest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.1.3/tests/heaserver/accounttest/__init__.py
--rw-rw-rw-   0        0        0     7626 2024-04-09 21:25:34.000000 heaserver_accounts-1.1.3/tests/heaserver/accounttest/test_all.py
--rw-rw-rw-   0        0        0     5462 2024-05-03 22:13:10.000000 heaserver_accounts-1.1.3/tests/heaserver/accounttest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.145314 heaserver_accounts-1.2.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1624 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6189 2024-05-22 16:09:18.143292 heaserver_accounts-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4881 2024-05-22 16:07:31.000000 heaserver_accounts-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/RELEASING.md
+-rw-rw-rw-   0        0        0      441 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.054439 heaserver_accounts-1.2.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.055439 heaserver_accounts-1.2.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.098178 heaserver_accounts-1.2.0/integrationtests/heaserver/accountintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/integrationtests/heaserver/accountintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0      481 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/integrationtests/heaserver/accountintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     7962 2024-05-15 20:55:34.000000 heaserver_accounts-1.2.0/integrationtests/heaserver/accountintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4294 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:09:18.145314 heaserver_accounts-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1825 2024-05-22 16:08:34.000000 heaserver_accounts-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.057022 heaserver_accounts-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.056021 heaserver_accounts-1.2.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.103023 heaserver_accounts-1.2.0/src/heaserver/account/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/src/heaserver/account/__init__.py
+-rw-rw-rw-   0        0        0    48842 2024-05-17 17:57:56.000000 heaserver_accounts-1.2.0/src/heaserver/account/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.105071 heaserver_accounts-1.2.0/src/heaserver/account/wstl/
+-rw-rw-rw-   0        0        0    11957 2024-05-03 03:06:58.000000 heaserver_accounts-1.2.0/src/heaserver/account/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.142770 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/
+-rw-rw-rw-   0        0        0     6189 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 16:09:18.000000 heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.058073 heaserver_accounts-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.058073 heaserver_accounts-1.2.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:09:18.140945 heaserver_accounts-1.2.0/tests/heaserver/accounttest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:51:28.000000 heaserver_accounts-1.2.0/tests/heaserver/accounttest/__init__.py
+-rw-rw-rw-   0        0        0     8157 2024-05-15 20:57:39.000000 heaserver_accounts-1.2.0/tests/heaserver/accounttest/test_all.py
+-rw-rw-rw-   0        0        0     5519 2024-05-15 20:55:15.000000 heaserver_accounts-1.2.0/tests/heaserver/accounttest/testcase.py
```

### Comparing `heaserver_accounts-1.1.3/Dockerfile` & `heaserver_accounts-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/LICENSE` & `heaserver_accounts-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/PKG-INFO` & `heaserver_accounts-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.3
+Version: 1.2.0
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.2.0
+* New /accounts endpoint that returns heaobject.account.AccountView objects.
+
 ## Version 1.1.3
 * Another attempt at fixing the crash regression.
 
 ## Version 1.1.2
 * Fixed crash regression.
 
 ## Version 1.1.1
```

### Comparing `heaserver_accounts-1.1.3/README.md` & `heaserver_accounts-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.2.0
+* New /accounts endpoint that returns heaobject.account.AccountView objects.
+
 ## Version 1.1.3
 * Another attempt at fixing the crash regression.
 
 ## Version 1.1.2
 * Fixed crash regression.
 
 ## Version 1.1.1
```

### Comparing `heaserver_accounts-1.1.3/RELEASING.md` & `heaserver_accounts-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/integrationtests/heaserver/accountintegrationtest/testcase.py` & `heaserver_accounts-1.2.0/integrationtests/heaserver/accountintegrationtest/testcase.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,16 +43,15 @@
         'name': 'amazon_web_services',
         'owner': NONE_USER,
         'shares': [],
         'source': None,
         'type': 'heaobject.volume.Volume',
         'version': None,
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
-        'file_system_type': 'heaobject.volume.AWSFileSystem',
-        'credential_id': None  # Let boto3 try to find the user's credentials.
+        'file_system_type': 'heaobject.volume.AWSFileSystem'  # Let boto3 try to find the user's credentials.
     }],
     CollectionKey(name='awsaccounts', db_manager_cls=MockS3Manager): [
         {
             "alternate_contact_name": None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": None,
@@ -69,15 +68,18 @@
             "name": "master",
             "owner": AWS_USER,
             "phone_number": None,
             "shares": [],
             "source": AWS,
             "source_detail": AWS,
             "type": "heaobject.account.AWSAccount",
-            "type_display_name": "AWS Account"
+            "type_display_name": "AWS Account",
+            "file_system_type": "heaobject.volume.AWSFileSystem",
+            "file_system_name": "DEFAULT_FILE_SYSTEM",
+            "credential_type_name": "heaobject.keychain.AWSCredentials"
         }
     ]
 }
 
 
 HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
 HEASERVER_VOLUMES_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-volumes:1.0.0'
```

### Comparing `heaserver_accounts-1.1.3/run-swaggerui.py` & `heaserver_accounts-1.2.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/setup.py` & `heaserver_accounts-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-accounts',
-    version='1.1.3',
+    version='1.2.0',
     description="Manages account information",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.account'],
     package_data={'heaserver.account': ['wstl/*.json']},
     install_requires=[
-        'heaserver~=1.5.3'
+        'heaserver~=1.6.0'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
```

### Comparing `heaserver_accounts-1.1.3/src/heaserver/account/service.py` & `heaserver_accounts-1.2.0/src/heaserver/account/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import aws, awsservicelib
 from heaserver.service.wstl import builder_factory, action
 from heaserver.service import response, client
 from heaserver.service.appproperty import HEA_DB, HEA_CACHE
 from heaserver.service.heaobjectsupport import new_heaobject_from_type
-from heaobject.account import AWSAccount  #, AccountView
+from heaobject.account import AWSAccount, AccountView
 from heaobject.bucket import AWSBucket
 from heaobject.storage import AWSStorage
 from heaobject.root import DesktopObjectDict
 from heaobject.volume import AWSFileSystem
 from heaobject.user import NONE_USER
 from yarl import URL
 from aiohttp.web import Request, Response
@@ -32,48 +32,84 @@
     For testing whether the service is up.
 
     :param request: the HTTP request.
     :return: Always returns status code 200.
     """
     return response.status_ok(None)
 
+@routes.get('/accounts/{id}')
+async def get_account_id(request: web.Request) -> web.Response:
+    id_ = request.match_info['id']
+    async with DesktopObjectActionLifecycle(request=request,
+                                            code='hea-get',
+                                            description=f'Getting account {id_}',
+                                            activity_cb=publish_desktop_object) as activity:
+        sub = request.headers.get(SUB, NONE_USER)
+        try:
+            aws_account, volume_id = await _get_awsaccount_by_aws_account_id(request, id_.split('^')[1])
+        except IndexError:
+            raise response.status_bad_request(f'Invalid account id {id_}')
+        if aws_account is None:
+            raise response.status_not_found()
+        else:
+            av = AccountView()
+            av.actual_object_id = aws_account.id
+            av.actual_object_type_name = aws_account.type
+            av.actual_object_uri = f'awsaccounts/{aws_account.id}'
+            av.display_name = aws_account.display_name
+            av.owner = aws_account.owner
+            av.shares = aws_account.shares
+            av.created = aws_account.created
+            av.modified = aws_account.modified
+            av.name = aws_account.name
+            av.type_display_name = aws_account.type_display_name
+            av.file_system_type = aws_account.file_system_type
+            av.file_system_name = aws_account.file_system_name
+            activity.new_object_type_name = AccountView.get_type_name()
+            activity.new_object_id = id_
+            activity.new_object_uri = f'accounts/{id_}'
+            activity.new_volume_id = volume_id
+            return await response.get(request, av.to_dict(), permissions=av.get_permissions(sub))
 
-# @routes.get('/accounts')
-# @routes.get('/accounts/')
-# @action(name='heaserver-accounts-account-get-actual', rel='hea-actual', path='{+actual_object_uri}')
-# async def get_accounts(request: web.Request) -> web.Response:
-#     async with DesktopObjectActionLifecycle(request=request,
-#                                                 code='hea-get',
-#                                                 description=f'Getting all accounts',
-#                                                 activity_cb=publish_desktop_object) as activity:
-#         logger = logging.getLogger(__name__)
-#         sub = request.headers.get(SUB, NONE_USER)
-#         account_ids = request.query.getall('account_id', [])
-#         try:
-#             aws_accounts = await _aws_account_ids_to_aws_accounts(request, tuple(a.split('^')[1] for a in account_ids))
-#         except IndexError:
-#             return response.status_bad_request(f'Invalid account_id query parameter {", ".join(account_ids)}')
-#         activity.new_object_type_name = AWSAccount.get_type_name()
-#         activity.new_object_uri = 'accounts/'
-#         account_views: list[AccountView] = []
-#         for aws_account in aws_accounts:
-#             av = AccountView()
-#             av.actual_object_id = aws_account.id
-#             av.actual_object_type_name = aws_account.type
-#             av.actual_object_uri = f'awsaccounts/{aws_account.id}'
-#             av.display_name = aws_account.display_name
-#             av.owner = aws_account.owner
-#             av.shares = aws_account.shares
-#             av.created = aws_account.created
-#             av.modified = aws_account.modified
-#             av.name = aws_account.name
-#             av.type_display_name = aws_account.type_display_name
-#             account_views.append(av)
-#         return await response.get_all(request, [a.to_dict() for a in account_views],
-#                                       permissions=[a.get_permissions(sub) for a in account_views])
+@routes.get('/accounts')
+@routes.get('/accounts/')
+@action(name='heaserver-accounts-account-get-actual', rel='hea-actual', path='{+actual_object_uri}')
+async def get_accounts(request: web.Request) -> web.Response:
+    async with DesktopObjectActionLifecycle(request=request,
+                                                code='hea-get',
+                                                description=f'Getting all accounts',
+                                                activity_cb=publish_desktop_object) as activity:
+        logger = logging.getLogger(__name__)
+        sub = request.headers.get(SUB, NONE_USER)
+        account_ids = request.query.getall('account_id', [])
+        try:
+            aws_accounts = await _aws_account_ids_to_aws_accounts(request, tuple(a.split('^')[1] for a in account_ids))
+        except IndexError:
+            return response.status_bad_request(f'Invalid account_id query parameter {", ".join(account_ids)}')
+        activity.new_object_type_name = AccountView.get_type_name()
+        activity.new_object_uri = 'accounts/'
+        account_views: list[AccountView] = []
+        for aws_account in aws_accounts:
+            av = AccountView()
+            av.actual_object_id = aws_account.id
+            av.actual_object_type_name = aws_account.type
+            av.actual_object_uri = f'awsaccounts/{aws_account.id}'
+            av.display_name = aws_account.display_name
+            av.owner = aws_account.owner
+            av.shares = aws_account.shares
+            av.created = aws_account.created
+            av.modified = aws_account.modified
+            av.name = aws_account.name
+            av.type_display_name = aws_account.type_display_name
+            av.type_display_name = aws_account.type_display_name
+            av.file_system_type = aws_account.file_system_type
+            av.file_system_name = aws_account.file_system_name
+            account_views.append(av)
+        return await response.get_all(request, [a.to_dict() for a in account_views],
+                                      permissions=[a.get_permissions(sub) for a in account_views])
 
 @routes.options('/awsaccounts/{id}')
 async def get_awsaccount_options(request: web.Request) -> web.Response:
     """
     ---
     summary: Allowed HTTP methods.
     tags:
@@ -130,15 +166,15 @@
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account, volume_id = cached_value
         else:
-            account, volume_id = await _get_awsaccount_by_id(request)
+            account, volume_id = await _get_awsaccount_by_aws_account_id(request, id_)
             logger.debug('Got account %s and volume %s', account, volume_id)
             if account is None:
                 raise response.status_not_found()
             request.app[HEA_CACHE][cache_key] = (account, volume_id)
             request.app[HEA_CACHE][(sub, f'volume_id^{volume_id}')] = (account, volume_id)
         request.match_info['volume_id'] = volume_id
         activity.new_object_type_name = AWSAccount.get_type_name()
@@ -272,15 +308,15 @@
         volume_id = request.match_info['volume_id']
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'volume_id^{volume_id}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account, volume_id = cached_value
         else:
-            account = await _get_account(request, volume_id)
+            account = await _get_awsaccount_by_volume_id(request, volume_id)
             if account is None:
                 raise response.status_not_found()
             request.app[HEA_CACHE][cache_key] = (account, volume_id)
             request.app[HEA_CACHE][(sub, f'id^{account.id}')] = (account, volume_id)
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_volume_id = volume_id
         activity.new_object_uri = f'volumes/{account.id}'
@@ -374,15 +410,15 @@
                                                     description=f'Getting my AWS account',
                                                     activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, f'id^{id_}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account, volume_id = cached_value
         else:
-            account = await _get_account(request, volume_id)
+            account = await _get_awsaccount_by_volume_id(request, volume_id)
             if account is None:
                 raise response.status_not_found()
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = f'awsaccounts/{account.id}'
         activity.new_volume_id = volume_id
         activity.new_object_id = account.id
         return await response.get_multiple_choices(request)
@@ -547,15 +583,15 @@
                                                 activity_cb=publish_desktop_object) as activity:
             sub = request.headers.get(SUB, NONE_USER)
             cache_key = (sub, f'volume_id^{volume_id}')
             cached_value = request.app[HEA_CACHE].get(cache_key)
             if cached_value is not None:
                 account, _ = cached_value
             else:
-                account = await _get_account(request, volume_id)
+                account = await _get_awsaccount_by_volume_id(request, volume_id)
                 if account is None:
                     raise response.status_not_found()
             activity.new_object_type_name = AWSAccount.get_type_name()
             activity.new_object_uri = f'awsaccounts/{account.id}'
             activity.new_volume_id = volume_id
             activity.new_object_id = account.id
             return await response.get_multiple_choices(request)
@@ -600,15 +636,15 @@
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'volume_id^{volume_id}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account, _ = cached_value
             return await response.get(request, cached_value)
         else:
-            account = await _get_account(request, volume_id)
+            account = await _get_awsaccount_by_volume_id(request, volume_id)
             if account is None:
                 return response.status_not_found()
             request.app[HEA_CACHE][cache_key] = (account, volume_id)
             request.app[HEA_CACHE][(sub, f'id^{account.id}')] = (account, volume_id)
         activity.new_object_id = account.id
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_volume_id = volume_id
@@ -645,15 +681,15 @@
                                                 activity_cb=publish_desktop_object) as activity:
         sub = request.headers.get(SUB, NONE_USER)
         cache_key = (sub, f'id^{request.match_info["id"]}')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value is not None:
             account, volume_id = cached_value
         else:
-            account, volume_id = await _get_awsaccount_by_id(request)
+            account, volume_id = await _get_awsaccount_by_aws_account_id(request, id_)
             if account is None:
                 return response.status_not_found()
             request.app[HEA_CACHE][cache_key] = (account, volume_id)
         activity.new_object_id = id_
         activity.new_object_type_name = AWSAccount.get_type_name()
         activity.new_object_uri = f'awsaccounts/{id_}'
         activity.new_volume_id = volume_id
@@ -732,15 +768,15 @@
     """
     async with DesktopObjectActionLifecycle(request=request,
                                                 code='hea-create',
                                                 description=f'Creating a new bucket in my AWS account',
                                                 activity_cb=publish_desktop_object) as activity:
         logger = logging.getLogger(__name__)
         volume_id = request.match_info['volume_id']
-        bucket_url = await type_to_resource_url(request, AWSBucket, file_system_type_or_type_name=AWSFileSystem)
+        bucket_url = await type_to_resource_url(request, AWSBucket)
         if bucket_url is None:
             raise ValueError('No AWSBucket service registered')
         headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
         resource_base = str(URL(bucket_url) / volume_id / 'buckets')
         bucket = await new_heaobject_from_type(request, type_=AWSBucket)
         try:
             id_ = await client.post(request.app, resource_base, data=bucket, headers=headers)
@@ -834,15 +870,15 @@
                                                 description=f'Creating a new bucket in AWS account',
                                                 activity_cb=publish_desktop_object) as activity:
         logger = logging.getLogger(__name__)
         volume_id = await awsservicelib.get_volume_id_for_account_id(request)
         if volume_id is None:
             activity.status = Status.FAILED
             return response.status_bad_request(f'Invalid account id {request.match_info["id"]}')
-        bucket_url = await type_to_resource_url(request, AWSBucket, file_system_type_or_type_name=AWSFileSystem)
+        bucket_url = await type_to_resource_url(request, AWSBucket)
         if bucket_url is None:
             raise ValueError('No AWSBucket service registered')
         headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
         resource_base = str(URL(bucket_url) / volume_id / 'buckets')
         bucket = await new_heaobject_from_type(request, type_=AWSBucket)
         try:
             id_ = await client.post(request.app, resource_base, data=bucket, headers=headers)
@@ -868,15 +904,15 @@
 def main() -> None:
     config = init_cmd_line(description='Manages account information',
                            default_port=8080)
     start(package_name='heaserver-accounts', db=aws.S3Manager,
           wstl_builder_factory=builder_factory(__package__), config=config)
 
 
-async def _get_account(request: Request, volume_id: str) -> AWSAccount:
+async def _get_awsaccount_by_volume_id(request: Request, volume_id: str) -> AWSAccount:
     """
     Gets the AWS account associated with the provided volume id.
 
     Only get since you can't delete or put id information
     currently being accessed. If organizations get included, then the delete, put, and post will be added for name,
     phone, email, ,etc.
     NOTE: maybe get email from the login portion of the application?
@@ -885,25 +921,24 @@
     :param volume_id: the id string of the volume representing the user's AWS account.
     :return: an HTTP response with an AWSAccount object in the body.
     FIXME: a bad volume_id should result in a 400 status code; currently has status code 500.
     """
     return await request.app[HEA_DB].get_account(request, volume_id)
 
 
-async def _get_awsaccount_by_id(request: web.Request) -> tuple[AWSAccount | None, str | None]:
+async def _get_awsaccount_by_aws_account_id(request: web.Request, aws_account_id: str) -> tuple[AWSAccount | None, str | None]:
     """
     Gets an account by its id and the account's volume id. The id is expected to be the request object's match_info
     mapping, with key 'id'.
 
     :param request: an aiohttp Request object (required).
     :return: a two-tuple containing an AWSAccount dict and volume id, or None if no account was found.
     """
-    account_id = request.match_info['id']
     db = request.app[HEA_DB]
-    async for volume in db.get_volumes(request, AWSFileSystem, account_ids=[account_id], account_type_names=[AWSAccount.get_type_name()]):
+    async for volume in db.get_volumes(request, AWSFileSystem, account_ids=[f'{AWSAccount.get_type_name()}^{aws_account_id}']):
         volume_id = volume.id
         return await db.get_account(request, volume_id), volume_id
     return (None, None)
 
 
 
 async def _get_account_by_name(request: web.Request) -> tuple[AWSAccount | None, str | None]:
@@ -972,21 +1007,19 @@
     logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, NONE_USER)
     cache_key = (sub, None, aws_account_ids)
     accounts = request.app[HEA_CACHE].get(cache_key) if aws_account_ids is None else None
     if accounts is None:
         db = request.app[HEA_DB]
         accounts: list[AWSAccount] = []
-        volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem,
-                                                                   account_ids=aws_account_ids,
-                                                                   account_type_names=[AWSAccount.get_type_name()] * len(aws_account_ids) if aws_account_ids is not None else None)]
+        volume_ids = [volume.id async for volume in db.get_volumes(request, AWSFileSystem, account_ids=tuple(f'{AWSAccount.get_type_name()}^{a}' for a in aws_account_ids))]
         logger.debug('Checking volumes %s for accounts %s', volume_ids, aws_account_ids)
         account_id_to_account = {}
         async for aws_account, volume_id in db.get_accounts(request, volume_ids):
             if not aws_account_ids or aws_account.id in aws_account_ids:
                 account_id_to_account[aws_account.id] = aws_account
                 request.app[HEA_CACHE][(sub, f'id^{aws_account.id}')] = (aws_account, volume_id)
         accounts_ = list(account_id_to_account.values())
         if accounts is None:
-            request.app[HEA_CACHE][cache_key] = accounts_
+            request.app[HEA_CACHE][cache_key] = (accounts_, volume_id)
         accounts = accounts_
     return accounts
```

### Comparing `heaserver_accounts-1.1.3/src/heaserver/account/wstl/all.json` & `heaserver_accounts-1.2.0/src/heaserver/account/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/PKG-INFO` & `heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-accounts
-Version: 1.1.3
+Version: 1.2.0
 Summary: Manages account information
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-accounts,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server AWS Accounts Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server AWS Accounts Microservice is It manages the AWS account information details.
 
+## Version 1.2.0
+* New /accounts endpoint that returns heaobject.account.AccountView objects.
+
 ## Version 1.1.3
 * Another attempt at fixing the crash regression.
 
 ## Version 1.1.2
 * Fixed crash regression.
 
 ## Version 1.1.1
```

### Comparing `heaserver_accounts-1.1.3/src/heaserver_accounts.egg-info/SOURCES.txt` & `heaserver_accounts-1.2.0/src/heaserver_accounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_accounts-1.1.3/tests/heaserver/accounttest/test_all.py` & `heaserver_accounts-1.2.0/tests/heaserver/accounttest/test_all.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,18 @@
                                                         {'name': 'name', 'value': 'master', 'prompt': 'name', 'display': True},
                                                         {'name': 'owner', 'value': 'system|aws', 'prompt': 'owner', 'display': True},
                                                         {'name': 'phone_number', 'value': None, 'prompt': 'phone_number', 'display': True},
                                                         {'name': 'shares', 'value': [], 'prompt': 'shares', 'display': True},
                                                         {'name': 'source', 'value': 'Amazon Web Services', 'prompt': 'source', 'display': True},
                                                         {'name': 'source_detail', 'value': 'Amazon Web Services', 'prompt': 'source_detail', 'display': True},
                                                         {'name': 'type', 'value': 'heaobject.account.AWSAccount', 'prompt': 'type', 'display': True},
-                                                        {'name': 'type_display_name', 'value': 'AWS Account', 'prompt': 'type_display_name', 'display': True}],
+                                                        {'name': 'type_display_name', 'value': 'AWS Account', 'prompt': 'type_display_name', 'display': True},
+                                                        {'name': 'file_system_type', 'value': 'heaobject.volume.AWSFileSystem', 'prompt': 'file_system_type', 'display': True},
+                                                        {'name': 'file_system_name', 'value': 'DEFAULT_FILE_SYSTEM', 'prompt': 'file_system_name', 'display': True},
+                                                        {'name': 'credential_type_name', 'value': 'heaobject.keychain.AWSCredentials', 'prompt': 'credential_type_name', 'display': True}],
                                                'links': []}],
                                     'template': {'prompt': 'New Folder', 'rel': '',
                                                  'data': [{'name': 'display_name', 'value': None, 'prompt': 'Name', 'required': True, 'readOnly': False, 'pattern': None},
                                                           {'name': 'type', 'value': 'heaobject.bucket.AWSBucket', 'prompt': 'Type', 'required': True, 'readOnly': True, 'pattern': None, 'display': False},
                                                           {'name': 'region', 'value': None, 'prompt': 'Region', 'required': True, 'readOnly': False, 'pattern': None, 'type': 'select',
                                                            'options': [{'value': 'us-east-2', 'text': 'US East (Ohio)'}, {'value': 'us-east-1', 'text': 'US East (N. Virginia)'}, {'value': 'us-west-1', 'text': 'US West (N. California)'}, {'value': 'us-west-2', 'text': 'US West (Oregon)'}, {'value': 'af-south-1', 'text': 'Africa (Cape Town)'}, {'value': 'ap-east-1', 'text': 'Asia Pacific (Hong Kong)'}, {'value': 'ap-southeast-3', 'text': 'Asia Pacific (Jakarta)'}, {'value': 'ap-south-1', 'text': 'Asia Pacific (Mumbai)'}, {'value': 'ap-northeast-3', 'text': 'Asia Pacific (Osaka)'}, {'value': 'ap-northeast-2', 'text': 'Asia Pacific (Seoul)'}, {'value': 'ap-southeast-1', 'text': 'Asia Pacific (Singapore)'}, {'value': 'ap-southeast-2', 'text': 'Asia Pacific (Sydney)'}, {'value': 'ap-northeast-1', 'text': 'Asia Pacific (Tokyo)'}, {'value': 'ca-central-1', 'text': 'Canada (Central)'}, {'value': 'eu-central-1', 'text': 'Europe (Frankfurt)'}, {'value': 'eu-west-1', 'text': 'Europe (Ireland)'}, {'value': 'eu-west-2', 'text': 'Europe (London)'}, {'value': 'eu-south-1', 'text': 'Europe (Milan)'}, {'value': 'eu-west-3', 'text': 'Europe (Paris)'}, {'value': 'eu-north-1', 'text': 'Europe (Stockholm)'}, {'value': 'me-south-1', 'text': 'Middle East (Bahrain)'}, {'value': 'sa-east-1', 'text': 'South America (São Paulo)'}],
                                                            "value": "us-east-1"},
```

### Comparing `heaserver_accounts-1.1.3/tests/heaserver/accounttest/testcase.py` & `heaserver_accounts-1.2.0/tests/heaserver/accounttest/testcase.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,20 +40,15 @@
         'shares': [],
         'source': None,
         'type': 'heaobject.volume.Volume',
         'version': None,
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'credential_id': None,  # Let boto3 try to find the user's credentials.
-        'account': {
-            'type': AccountAssociation.get_type_name(),
-            'actual_object_type_name': AWSAccount.get_type_name(),
-            'actual_object_id': "123456789012"
-        }
-
+        'account_id': f'{AWSAccount.get_type_name()}^123456789012'
     }],
     'awsaccounts': [
         {
             "alternate_contact_name": None,
             "alternate_email_address": None,
             "alternate_phone_number": None,
             "created": None,
@@ -70,15 +65,18 @@
             "name": "master",
             "owner": "system|aws",
             "phone_number": None,
             "shares": [],
             "source": AWS,
             "source_detail": AWS,
             "type": AWSAccount.get_type_name(),
-            "type_display_name": "AWS Account"
+            "type_display_name": "AWS Account",
+            "file_system_type": "heaobject.volume.AWSFileSystem",
+            "file_system_name": "DEFAULT_FILE_SYSTEM",
+            "credential_type_name": "heaobject.keychain.AWSCredentials"
         }
     ]}
 
 AWSAccountTestCase = \
     microservicetestcase.get_test_case_cls_default(
         href='http://localhost:8080/awsaccounts',
         wstl_package=service.__package__,
```

