# Comparing `tmp/heaserver_organizations-1.3.0.tar.gz` & `tmp/heaserver_organizations-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_organizations-1.3.0.tar", last modified: Thu Apr 18 04:02:10 2024, max compression
+gzip compressed data, was "heaserver_organizations-1.4.0.tar", last modified: Tue May 21 23:52:33 2024, max compression
```

## Comparing `heaserver_organizations-1.3.0.tar` & `heaserver_organizations-1.4.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.685517 heaserver_organizations-1.3.0/
--rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/.gitignore
--rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5183 2024-04-18 04:02:10.683521 heaserver_organizations-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3793 2024-04-11 17:15:42.000000 heaserver_organizations-1.3.0/README.md
--rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/RELEASING.md
--rw-rw-rw-   0        0        0      404 2024-03-20 04:10:28.000000 heaserver_organizations-1.3.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.520206 heaserver_organizations-1.3.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.521205 heaserver_organizations-1.3.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.625476 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
--rw-rw-rw-   0        0        0    10758 2024-04-08 23:26:43.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      402 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    14802 2024-04-08 23:26:37.000000 heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/pytest.ini
--rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-18 04:02:10.685517 heaserver_organizations-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1911 2024-04-18 04:01:32.000000 heaserver_organizations-1.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.524212 heaserver_organizations-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.522207 heaserver_organizations-1.3.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.628473 heaserver_organizations-1.3.0/src/heaserver/organization/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/src/heaserver/organization/__init__.py
--rw-rw-rw-   0        0        0    28882 2024-04-05 18:49:42.000000 heaserver_organizations-1.3.0/src/heaserver/organization/service.py
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.630477 heaserver_organizations-1.3.0/src/heaserver/organization/wstl/
--rw-rw-rw-   0        0        0    23163 2024-04-11 17:16:54.000000 heaserver_organizations-1.3.0/src/heaserver/organization/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.682518 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/
--rw-rw-rw-   0        0        0     5183 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      997 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 04:02:10.000000 heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.525209 heaserver_organizations-1.3.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.526208 heaserver_organizations-1.3.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 04:02:10.677517 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/
--rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-12-18 21:21:27.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/test_all.py
--rw-rw-rw-   0        0        0     6894 2024-04-08 23:26:24.000000 heaserver_organizations-1.3.0/tests/heaserver/organizationtest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.630862 heaserver_organizations-1.4.0/
+-rw-rw-rw-   0        0        0      261 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/.gitignore
+-rw-rw-rw-   0        0        0     1663 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5446 2024-05-21 23:52:33.617088 heaserver_organizations-1.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4056 2024-05-21 23:50:49.000000 heaserver_organizations-1.4.0/README.md
+-rw-rw-rw-   0        0        0     1749 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/RELEASING.md
+-rw-rw-rw-   0        0        0      576 2024-05-17 22:08:10.000000 heaserver_organizations-1.4.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.395406 heaserver_organizations-1.4.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.395406 heaserver_organizations-1.4.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.530830 heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0    10980 2024-04-20 02:18:13.000000 heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      835 2024-05-21 22:02:46.000000 heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    15050 2024-05-17 22:32:58.000000 heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/pytest.ini
+-rw-rw-rw-   0        0        0      362 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6574 2023-12-18 21:21:27.000000 heaserver_organizations-1.4.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:52:33.631032 heaserver_organizations-1.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1911 2024-05-21 23:51:55.000000 heaserver_organizations-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.397702 heaserver_organizations-1.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.396861 heaserver_organizations-1.4.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.544993 heaserver_organizations-1.4.0/src/heaserver/organization/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.0/src/heaserver/organization/__init__.py
+-rw-rw-rw-   0        0        0    52574 2024-05-21 03:38:07.000000 heaserver_organizations-1.4.0/src/heaserver/organization/service.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.560557 heaserver_organizations-1.4.0/src/heaserver/organization/wstl/
+-rw-rw-rw-   0        0        0    24887 2024-05-21 20:03:34.000000 heaserver_organizations-1.4.0/src/heaserver/organization/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.617088 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/
+-rw-rw-rw-   0        0        0     5446 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 23:52:33.000000 heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.398744 heaserver_organizations-1.4.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.399258 heaserver_organizations-1.4.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:52:33.617088 heaserver_organizations-1.4.0/tests/heaserver/organizationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-14 19:48:11.000000 heaserver_organizations-1.4.0/tests/heaserver/organizationtest/__init__.py
+-rw-rw-rw-   0        0        0     2214 2024-05-19 21:02:26.000000 heaserver_organizations-1.4.0/tests/heaserver/organizationtest/test_all.py
+-rw-rw-rw-   0        0        0     7050 2024-05-21 21:15:05.000000 heaserver_organizations-1.4.0/tests/heaserver/organizationtest/testcase.py
```

### Comparing `heaserver_organizations-1.3.0/Dockerfile` & `heaserver_organizations-1.4.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.3.0/LICENSE` & `heaserver_organizations-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.3.0/PKG-INFO` & `heaserver_organizations-1.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.3.0
+Version: 1.4.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,24 +21,29 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.0
+* Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
+match.
+* The admin, manager, and member lists now omit system users.
+
 ## Version 1.3.0
-* Return the type_display_name attribute.
+* Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
```

### Comparing `heaserver_organizations-1.3.0/README.md` & `heaserver_organizations-1.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.0
+* Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
+match.
+* The admin, manager, and member lists now omit system users.
+
 ## Version 1.3.0
-* Return the type_display_name attribute.
+* Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
```

### Comparing `heaserver_organizations-1.3.0/RELEASING.md` & `heaserver_organizations-1.4.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py` & `heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/permissionstestcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,18 @@
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'version': None,
             'accounts': [],
-            'type_display_name': 'Organization'
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -57,15 +60,18 @@
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
             'version': None,
             'accounts': [],
-            'type_display_name': 'Organization'
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         }
     ],
     'filesystems': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver_organizations-1.3.0/integrationtests/heaserver/organizationintegrationtest/testcase.py` & `heaserver_organizations-1.4.0/integrationtests/heaserver/organizationintegrationtest/testcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,53 +23,57 @@
             "id": "666f6f2d6261722d71757578",
             "source": None,
             "source_detail": None,
             "name": "Bob",
             "display_name": "Bob",
             "description": "Description of Bob lab",
             "owner": NONE_USER,
-            "created": None,
-            "modified": None,
+            "created": '2022-05-17T00:00:00+00:00',
+            "modified": '2022-05-17T00:00:00+00:00',
             "invites": [],
             "shares": [],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": ['666f6f2d6261722d71757578'],
             "member_ids": ['0123456789ab0123456789ab'],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': [],
-            'type_display_name': 'Organization'
+            'account_ids': [],
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
             "description": "Description of Reximus",
             "owner": NONE_USER,
-            "created": None,
-            "modified": None,
+            "created": '2022-05-17T00:00:00+00:00',
+            "modified": '2022-05-17T00:00:00+00:00',
             "invites": [],
             "shares": [],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
             "admin_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': [],
-            'type_display_name': 'Organization'
+            'account_ids': [],
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         }
     ],
     CollectionKey(name='filesystems', db_manager_cls=MockDockerMongoManager): [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

### Comparing `heaserver_organizations-1.3.0/run-swaggerui.py` & `heaserver_organizations-1.4.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.3.0/setup.py` & `heaserver_organizations-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-organizations',
-    version='1.3.0',
+    version='1.4.0',
     description="a service for managing organization information for research laboratories and other research groups",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.organization'],
     package_data={'heaserver.organization': ['wstl/*.json']},
-    install_requires=['heaserver~=1.4.1'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_organizations-1.3.0/src/heaserver/organization/wstl/all.json` & `heaserver_organizations-1.4.0/src/heaserver/organization/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972865865688132%*

 * *Differences: {"'wstl'": "{'actions': {3: {'name': 'heaserver-organizations-account-get-actual', 'description': "*

 * *           "'View the actual account object', 'prompt': 'View actual'}, 7: {'inputs': {7: {'hea': "*

 * *           "{'optionsFromUrl': {'path': 'accounts/'}}, 'name': 'account_ids', 'prompt': "*

 * *           "'Accounts'}, 8: {'hea': {'optionsFromUrl': {'path': 'people/?excludesystem=yes'}}}, 9: "*

 * *           "{'hea': {'optionsFromUrl': {'path': 'people/?excludesystem=yes'}}}, 10: {'hea': "*

 * *           "{'optionsFromUr […]*

```diff
@@ -21,17 +21,17 @@
                 "name": "heaserver-organizations-organization-get-self",
                 "prompt": "View",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
-                "description": "View this account",
-                "name": "heaserver-organizations-awsaccount-get-self",
-                "prompt": "View",
+                "description": "View the actual account object",
+                "name": "heaserver-organizations-account-get-actual",
+                "prompt": "View actual",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
                 "description": "View this member",
                 "name": "heaserver-organizations-member-get-self",
@@ -109,67 +109,67 @@
                         "prompt": "MIME type",
                         "readOnly": true
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "optionsFromUrl": {
-                                "path": "awsaccounts/",
+                                "path": "accounts/",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
-                        "name": "aws_account_ids",
-                        "prompt": "AWS Accounts",
+                        "name": "account_ids",
+                        "prompt": "Accounts",
                         "readOnly": true,
                         "type": "select"
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
-                                "path": "people/",
+                                "path": "people/?excludesystem=yes",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
                         "name": "principal_investigator_id",
                         "prompt": "Principal Investigator",
                         "type": "select"
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "optionsFromUrl": {
-                                "path": "people/",
+                                "path": "people/?excludesystem=yes",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
                         "name": "admin_ids",
                         "prompt": "Admins",
                         "type": "select"
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "optionsFromUrl": {
-                                "path": "people/",
+                                "path": "people/?excludesystem=yes",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
                         "name": "manager_ids",
                         "prompt": "Managers",
                         "type": "select"
                     },
                     {
                         "hea": {
                             "cardinality": "multiple",
                             "optionsFromUrl": {
-                                "path": "people/",
+                                "path": "people/?excludesystem=yes",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
                         "name": "member_ids",
                         "prompt": "Members",
                         "type": "select"
@@ -274,14 +274,53 @@
                             "section": "shares"
                         },
                         "name": "type",
                         "prompt": "Type",
                         "readOnly": true,
                         "required": true,
                         "value": "heaobject.root.ShareImpl"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "admin_group_ids",
+                        "prompt": "Admin groups",
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "manager_group_ids",
+                        "prompt": "Manager groups",
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "member_group_ids",
+                        "prompt": "Member groups",
+                        "type": "select"
                     }
                 ],
                 "name": "heaserver-organizations-organization-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
```

### Comparing `heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/PKG-INFO` & `heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-organizations
-Version: 1.3.0
+Version: 1.4.0
 Summary: a service for managing organization information for research laboratories and other research groups
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-organizations,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,24 +21,29 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Organization
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Organization is a service for managing organization information for research laboratories and other research groups.
 
+## Version 1.4.0
+* Changing organization members, managers, admins, and PI now changes the users' volumes and credentials objects to
+match.
+* The admin, manager, and member lists now omit system users.
+
 ## Version 1.3.0
-* Return the type_display_name attribute.
+* Display type display name in properties card, and return the type display name from GET calls.
 
 ## Version 1.2.0
 * Improved performance accessing an organization's AWS accounts.
 * heaobject.organization.Organization objects now have an accounts attribute that mirrors the contents of the existing
 aws_account_ids attribute and will support other heaobject.account.Account subclasses in the future.
 
 ## Version 1.1.0
```

### Comparing `heaserver_organizations-1.3.0/src/heaserver_organizations.egg-info/SOURCES.txt` & `heaserver_organizations-1.4.0/src/heaserver_organizations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_organizations-1.3.0/tests/heaserver/organizationtest/test_all.py` & `heaserver_organizations-1.4.0/tests/heaserver/organizationtest/test_all.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .testcase import TestCase
 from heaserver.service.testcase.mixin import GetOneMixin, GetAllMixin, PostMixin, PutMixin, DeleteMixin
 from aiohttp import hdrs
 from heaserver.service.representor import cj
-
+from unittest.mock import patch
 
 class TestGet(TestCase, GetOneMixin):
     """Test case for GET requests specific to organizations."""
     async def test_get_status_opener_choices(self) -> None:
         """Checks if a GET request for the opener for an organization succeeds with status 300."""
         obj = await self.client.request('GET',
                                         (self._href / self._id() / 'opener').path,
@@ -32,14 +32,21 @@
     """Test case for GET all requests specific to organizations."""
     pass
 
 
 class TestPost(TestCase, PostMixin):
     pass
 
+async def _mock_update_group_membership(request, user, added_groups, deleted_groups, group_url_getter):
+    pass
+
+async def _mock_update_volumes_and_credentials(app, changed):
+    pass
 
+@patch('heaserver.organization.service._update_group_membership', _mock_update_group_membership)
+@patch('heaserver.organization.service._update_volumes_and_credentials', _mock_update_volumes_and_credentials)
 class TestPut(TestCase, PutMixin):
     pass
 
 
 class TestDelete(TestCase, DeleteMixin):
     pass
```

### Comparing `heaserver_organizations-1.3.0/tests/heaserver/organizationtest/testcase.py` & `heaserver_organizations-1.4.0/tests/heaserver/organizationtest/testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,25 @@
             "owner": NONE_USER,
             "created": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "modified": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "invites": [],
             "shares": [],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': [],
-            'type_display_name': 'Organization'
+            'account_ids': [],
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             'source_detail': None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -44,23 +46,25 @@
             "owner": NONE_USER,
             "created": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "modified": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "invites": [],
             "shares": [],
             "derived_by": None,
             "derived_from": [],
-            "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": ["11234867890b0123a56789ab"],
             "member_ids": [],
             "admin_ids": [],
             'type': 'heaobject.organization.Organization',
             'mime_type': 'application/x.organization',
-            'accounts': [],
-            'type_display_name': 'Organization'
+            'account_ids': [],
+            'type_display_name': 'Organization',
+            'member_group_ids': [],
+            'manager_group_ids': [],
+            'admin_group_ids': []
         }
     ],
     'people': [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
```

