# Comparing `tmp/heaserver-activity-1.1.0.tar.gz` & `tmp/heaserver_activity-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-activity-1.1.0.tar", last modified: Wed Apr  3 23:39:34 2024, max compression
+gzip compressed data, was "heaserver_activity-1.1.1.tar", last modified: Wed May 22 00:22:00 2024, max compression
```

## Comparing `heaserver-activity-1.1.0.tar` & `heaserver_activity-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.818362 heaserver-activity-1.1.0/
--rw-rw-rw-   0        0        0    11625 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       39 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4982 2024-04-03 23:39:34.817003 heaserver-activity-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3663 2024-04-03 21:31:38.000000 heaserver-activity-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 23:39:34.818362 heaserver-activity-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1823 2024-04-03 23:38:58.000000 heaserver-activity-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.708037 heaserver-activity-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.707017 heaserver-activity-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.733002 heaserver-activity-1.1.0/src/heaserver/activity/
--rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/src/heaserver/activity/__init__.py
--rw-rw-rw-   0        0        0    15003 2024-04-03 21:16:46.000000 heaserver-activity-1.1.0/src/heaserver/activity/service.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.743002 heaserver-activity-1.1.0/src/heaserver/activity/wstl/
--rw-rw-rw-   0        0        0     7666 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/src/heaserver/activity/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.816002 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/
--rw-rw-rw-   0        0        0     4982 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      871 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 23:39:34.000000 heaserver-activity-1.1.0/src/heaserver_activity.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.709008 heaserver-activity-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.709008 heaserver-activity-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.804003 heaserver-activity-1.1.0/tests/heaserver/activitytest/
--rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 23:39:34.814005 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/
--rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088
--rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284
--rw-rw-rw-   0        0        0     2983 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/permissionstestcase.py
--rw-rw-rw-   0        0        0     2482 2024-04-03 16:54:29.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/test_all.py
--rw-rw-rw-   0        0        0      338 2023-12-18 19:13:06.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     8546 2024-04-03 17:54:33.000000 heaserver-activity-1.1.0/tests/heaserver/activitytest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.387751 heaserver_activity-1.1.1/
+-rw-rw-rw-   0        0        0    11625 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5275 2024-05-22 00:22:00.386706 heaserver_activity-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3956 2024-05-22 00:19:38.000000 heaserver_activity-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 00:22:00.387751 heaserver_activity-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1823 2024-05-22 00:20:05.000000 heaserver_activity-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.224961 heaserver_activity-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.223922 heaserver_activity-1.1.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.255714 heaserver_activity-1.1.1/src/heaserver/activity/
+-rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/src/heaserver/activity/__init__.py
+-rw-rw-rw-   0        0        0    14807 2024-05-17 21:32:09.000000 heaserver_activity-1.1.1/src/heaserver/activity/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.267441 heaserver_activity-1.1.1/src/heaserver/activity/wstl/
+-rw-rw-rw-   0        0        0     7666 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/src/heaserver/activity/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.385149 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/
+-rw-rw-rw-   0        0        0     5275 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      871 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 00:22:00.000000 heaserver_activity-1.1.1/src/heaserver_activity.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.225999 heaserver_activity-1.1.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.226525 heaserver_activity-1.1.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.369407 heaserver_activity-1.1.1/tests/heaserver/activitytest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:22:00.383584 heaserver_activity-1.1.1/tests/heaserver/activitytest/__pycache__/
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088
+-rw-rw-rw-   0        0        0     1279 2023-06-11 22:22:03.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284
+-rw-rw-rw-   0        0        0     2983 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     2545 2024-05-22 00:17:49.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/test_all.py
+-rw-rw-rw-   0        0        0      338 2023-12-18 19:13:06.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     8771 2024-05-22 00:17:00.000000 heaserver_activity-1.1.1/tests/heaserver/activitytest/testcase.py
```

### Comparing `heaserver-activity-1.1.0/LICENSE` & `heaserver_activity-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/PKG-INFO` & `heaserver_activity-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.1.0
+Version: 1.1.1
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.1
+* Returned DesktopObjectAction objects now have a type_display_name attribute.
+* Returned RecentlyAccessView objects now have a type_display_name attribute, and the default display_name is now
+Untitled Recently Accessed View (rather than Untitled RecentlyAccessedView).
+
 ## Version 1.1.0
 * Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
 
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
```

### Comparing `heaserver-activity-1.1.0/README.md` & `heaserver_activity-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.1
+* Returned DesktopObjectAction objects now have a type_display_name attribute.
+* Returned RecentlyAccessView objects now have a type_display_name attribute, and the default display_name is now
+Untitled Recently Accessed View (rather than Untitled RecentlyAccessedView).
+
 ## Version 1.1.0
 * Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
 
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
```

### Comparing `heaserver-activity-1.1.0/setup.py` & `heaserver_activity-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-activity',
-    version='1.1.0',
+    version='1.1.1',
     description="A service for tracking activity in hea",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.activity'],
     package_data={'heaserver.activity': ['wstl/*.json']},
-    install_requires=['heaserver~=1.1.3'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-activity-1.1.0/src/heaserver/activity/service.py` & `heaserver_activity-1.1.1/src/heaserver/activity/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,21 +260,17 @@
     logger = logging.getLogger(__name__)
     logger.debug('Saving desktop object action %s', desktop_object)
     saved_object = await app[appproperty.HEA_DB].get_admin(MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION, mongoattributes={
         'application_id': desktop_object.application_id
     })
     if saved_object is not None:
         desktop_object.id = saved_object['id']
-        if desktop_object.modified is None:
-            desktop_object.modified = datetime.now()
         if await app[appproperty.HEA_DB].update_admin(desktop_object, MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION) is None:
             raise ValueError(f'Failed to update desktop object action {desktop_object}')
     else:
-        if desktop_object.created is None:
-            desktop_object.created = datetime.now()
         if (result := await app[appproperty.HEA_DB].insert_admin(desktop_object, MONGODB_DESKTOP_OBJECT_ACTION_COLLECTION)) is None:
             raise ValueError(f'Failed to insert desktop object action {desktop_object}')
         desktop_object.id = result
     logger.debug('Desktop object saved: %s', desktop_object)
 
     desktop_object_dict = desktop_object.to_dict()
     if _wsresponses:
```

### Comparing `heaserver-activity-1.1.0/src/heaserver/activity/wstl/all.json` & `heaserver_activity-1.1.1/src/heaserver/activity/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/src/heaserver_activity.egg-info/PKG-INFO` & `heaserver_activity-1.1.1/src/heaserver_activity.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-activity
-Version: 1.1.0
+Version: 1.1.1
 Summary: A service for tracking activity in hea
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-activity,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,27 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.3
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Activity Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Activity Microservice is A service for tracking activity in hea.
 
+## Version 1.1.1
+* Returned DesktopObjectAction objects now have a type_display_name attribute.
+* Returned RecentlyAccessView objects now have a type_display_name attribute, and the default display_name is now
+Untitled Recently Accessed View (rather than Untitled RecentlyAccessedView).
+
 ## Version 1.1.0
 * Added query parameter for excluding desktop objects actions with certain codes from query results and the web socket.
 
 ## Version 1.0.3
 * Improved performance.
 
 ## Version 1.0.2
```

### Comparing `heaserver-activity-1.1.0/src/heaserver_activity.egg-info/SOURCES.txt` & `heaserver_activity-1.1.1/src/heaserver_activity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088` & `heaserver_activity-1.1.1/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.20088`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284` & `heaserver_activity-1.1.1/tests/heaserver/activitytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.38284`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/tests/heaserver/activitytest/permissionstestcase.py` & `heaserver_activity-1.1.1/tests/heaserver/activitytest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-activity-1.1.0/tests/heaserver/activitytest/test_all.py` & `heaserver_activity-1.1.1/tests/heaserver/activitytest/test_all.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,9 +50,10 @@
                 'ended': None,
                 'human_readable_duration': None,
                 'mime_type': 'application/x.desktopobjectaction',
                 'new_volume_id': None,
                 'old_volume_id': None,
                 'requested': '2022-05-17T00:00:00-06:00',
                 'status_updated': '2022-05-17T00:00:00-06:00',
-                'began': '2022-05-17T00:00:00-06:00'
+                'began': '2022-05-17T00:00:00-06:00',
+                'type_display_name': 'Desktop Object Action'
             }], await obj.json())
```

### Comparing `heaserver-activity-1.1.0/tests/heaserver/activitytest/testcase.py` & `heaserver_activity-1.1.1/tests/heaserver/activitytest/testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,16 @@
         'ended': None,
         'human_readable_duration': None,
         'mime_type': 'application/x.desktopobjectaction',
         'new_volume_id': None,
         'old_volume_id': None,
         'requested': '2022-05-17T00:00:00-06:00',
         'status_updated': '2022-05-17T00:00:00-06:00',
-        'began': '2022-05-17T00:00:00-06:00'
+        'began': '2022-05-17T00:00:00-06:00',
+        'type_display_name': 'Desktop Object Action'
     },
     {
         'id': '0123456789ab0123456789ab',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -77,54 +78,57 @@
         'human_readable_duration': None,
         'mime_type': 'application/x.desktopobjectaction',
         'new_volume_id': None,
         'old_volume_id': None,
         'requested': '2022-05-17T00:00:00-06:00',
         'status_updated': '2022-05-17T00:00:00-06:00',
         'began': '2022-05-17T00:00:00-06:00',
+        'type_display_name': 'Desktop Object Action'
     }],
     'recentlyaccessedviews': [{
         'id': '666f6f2d6261722d71757578',
         'accessed': '2022-05-17T00:00:00-06:00',
         'actual_object_id': '666f6f2d6261722d71757578',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_uri': 'awss3projects/666f6f2d6261722d71757578',
         'type': 'heaobject.activity.RecentlyAccessedView',
         'created': None,
         'modified': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'name': None,
-        'display_name': 'Untitled RecentlyAccessedView',
+        'display_name': 'Untitled Recently Accessed View',
         'invites': [],
         'owner': 'user-a',
         'shares': [],
         'source': None,
-        'source_detail': None
+        'source_detail': None,
+        'type_display_name': 'Recently Accessed View'
     },
     {
         'id': '0123456789ab0123456789ab',
         'accessed': '2022-05-17T00:00:00-06:00',
         'actual_object_id': '0123456789ab0123456789ab',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_uri': 'awss3projects/0123456789ab0123456789ab',
         'type': 'heaobject.activity.RecentlyAccessedView',
         'created': None,
         'modified': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'name': None,
-        'display_name': 'Untitled RecentlyAccessedView',
+        'display_name': 'Untitled Recently Accessed View',
         'invites': [],
         'owner': 'user-a',
         'shares': [],
         'source': None,
-        'source_detail': None
+        'source_detail': None,
+        'type_display_name': 'Recently Accessed View'
     }
     ]}
 
 
 RecentlyAccessedViewsByTypeTestCase = get_test_case_cls_default(coll='recentlyaccessedviews',
                                                          wstl_package=service.__package__,
                                                          href='http://localhost:8080/recentlyaccessedviews/bytype/heaobject.project.AWSS3Project',
```

