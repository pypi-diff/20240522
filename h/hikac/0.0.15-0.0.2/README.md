# Comparing `tmp/hikac-0.0.15.tar.gz` & `tmp/hikac-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hikac-0.0.15.tar", last modified: Wed May 22 16:33:16 2024, max compression
+gzip compressed data, was "hikac-0.0.2.tar", last modified: Wed May 22 16:03:54 2024, max compression
```

## Comparing `hikac-0.0.15.tar` & `hikac-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.684605 hikac-0.0.15/
--rw-r--r--   0 yusufjon   (501) staff       (20)     1073 2024-05-22 15:25:24.000000 hikac-0.0.15/LICENSE
--rw-r--r--   0 yusufjon   (501) staff       (20)     1489 2024-05-22 16:33:16.684469 hikac-0.0.15/PKG-INFO
--rw-r--r--   0 yusufjon   (501) staff       (20)      991 2024-05-22 16:28:57.000000 hikac-0.0.15/README.md
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.681559 hikac-0.0.15/app/
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.682443 hikac-0.0.15/app/hikac/
--rw-r--r--   0 yusufjon   (501) staff       (20)       46 2024-05-22 15:22:35.000000 hikac-0.0.15/app/hikac/__init__.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.683766 hikac-0.0.15/app/hikac/src/
--rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.15/app/hikac/src/__init__.py
--rw-r--r--   0 yusufjon   (501) staff       (20)     1743 2024-05-22 15:20:43.000000 hikac-0.0.15/app/hikac/src/hikac.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.684157 hikac-0.0.15/app/hikac/test/
--rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.15/app/hikac/test/__init__.py
--rw-r--r--   0 yusufjon   (501) staff       (20)      166 2024-05-22 15:22:26.000000 hikac-0.0.15/app/hikac/test/test_hikac.py
-drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:33:16.683459 hikac-0.0.15/app/hikac.egg-info/
--rw-r--r--   0 yusufjon   (501) staff       (20)     1489 2024-05-22 16:33:16.000000 hikac-0.0.15/app/hikac.egg-info/PKG-INFO
--rw-r--r--   0 yusufjon   (501) staff       (20)      317 2024-05-22 16:33:16.000000 hikac-0.0.15/app/hikac.egg-info/SOURCES.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)        1 2024-05-22 16:33:16.000000 hikac-0.0.15/app/hikac.egg-info/dependency_links.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)       42 2024-05-22 16:33:16.000000 hikac-0.0.15/app/hikac.egg-info/requires.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)        6 2024-05-22 16:33:16.000000 hikac-0.0.15/app/hikac.egg-info/top_level.txt
--rw-r--r--   0 yusufjon   (501) staff       (20)       38 2024-05-22 16:33:16.684660 hikac-0.0.15/setup.cfg
--rw-r--r--   0 yusufjon   (501) staff       (20)      838 2024-05-22 16:33:12.000000 hikac-0.0.15/setup.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.015025 hikac-0.0.2/
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1073 2024-05-22 15:25:24.000000 hikac-0.0.2/LICENSE
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1326 2024-05-22 16:03:54.014886 hikac-0.0.2/PKG-INFO
+-rw-r--r--   0 yusufjon   (501) staff       (20)      132 2024-05-22 15:11:40.000000 hikac-0.0.2/README.md
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.012545 hikac-0.0.2/app/
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.013198 hikac-0.0.2/app/hikac/
+-rw-r--r--   0 yusufjon   (501) staff       (20)       46 2024-05-22 15:22:35.000000 hikac-0.0.2/app/hikac/__init__.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.014208 hikac-0.0.2/app/hikac/src/
+-rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.2/app/hikac/src/__init__.py
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1743 2024-05-22 15:20:43.000000 hikac-0.0.2/app/hikac/src/hikac.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.014649 hikac-0.0.2/app/hikac/test/
+-rw-r--r--   0 yusufjon   (501) staff       (20)        0 2024-05-22 15:09:16.000000 hikac-0.0.2/app/hikac/test/__init__.py
+-rw-r--r--   0 yusufjon   (501) staff       (20)      166 2024-05-22 15:22:26.000000 hikac-0.0.2/app/hikac/test/test_hikac.py
+drwxr-xr-x   0 yusufjon   (501) staff       (20)        0 2024-05-22 16:03:54.013955 hikac-0.0.2/app/hikac.egg-info/
+-rw-r--r--   0 yusufjon   (501) staff       (20)     1326 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/PKG-INFO
+-rw-r--r--   0 yusufjon   (501) staff       (20)      317 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/SOURCES.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)        1 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/dependency_links.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)       42 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/requires.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)        6 2024-05-22 16:03:53.000000 hikac-0.0.2/app/hikac.egg-info/top_level.txt
+-rw-r--r--   0 yusufjon   (501) staff       (20)       38 2024-05-22 16:03:54.015087 hikac-0.0.2/setup.cfg
+-rw-r--r--   0 yusufjon   (501) staff       (20)      837 2024-05-22 16:03:50.000000 hikac-0.0.2/setup.py
```

### Comparing `hikac-0.0.15/LICENSE` & `hikac-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hikac-0.0.15/PKG-INFO` & `hikac-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,45 @@
 Metadata-Version: 2.1
 Name: hikac
-Version: 0.0.15
+Version: 0.0.2
 Summary: A hikvision access control request manager
 Home-page: https://github.com/yusufjonc07/hikac
 Author: YusufAxmad
 Author-email: studentyusufaxmad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# HIKAC
+# HIKVISION AC REQUEST MANAGER
+A package used to get needy data from Hikvision ac device request.
 
-This modest python package helps you to get events from HIKVISION AC terminals. 
-
-## Installation
-
-```sh
-pip install hikac
-
-```
-
-## Usage in FastAPI
-
-```sh
-
-from hikac import get_data_from_ac_event
-
-@attandance_router.post("/attandance/face-id", include_in_schema=False)
-async def listen_for_ac_event(
-    req: Request,
-    db: Session = ActiveSession,
-):
-    try:
-
-        # use the class to collect nececary items of dict
-        eventData = await get_data_from_ac_event(req)
-
-        if eventData.attendanceStatus:
-
-            #you can use these attributes
-            #eventData.deviceIpAddress
-            #eventData.attendanceStatus
-            #eventData.deviceName
-            #eventData.dateTime
-            #eventData.employeeId
-            #eventData.employeeName
-
-            # write  your logic here
-
-            return "success"
-    except Exception as e:
-        print(e.args)
-```
-
-## How to configure Hikvision device - Soon!
-![Http Litening](./hiklistening.jpg)
+## How to use
+_After installing the package use following import:_ <br>
 
+**from hikac import get_data_from_ac_event
 
+_In Your Api router, you can also use like that:_
+
+**@attandance_router.post("/attandance/face-id", include_in_schema=False)
+**async def get_attandance_users_list(
+**    req: Request,
+**    db: Session = ActiveSession,
+**):
+**    try:
+**        # use the class to collect nececary items of dict
+**        eventData = await get_data_from_ac_event(req)
+**
+**        if eventData.attendanceStatus:
+**            await makeDavomat(eventData.employeeId, eventData.attendanceStatus, eventData.dateTime, eventData.deviceName, db)
+**
+**            return "success"
+**    except Exception as e:
+**        print(e.args)
+**
```

### Comparing `hikac-0.0.15/app/hikac/src/hikac.py` & `hikac-0.0.2/app/hikac/src/hikac.py`

 * *Files identical despite different names*

### Comparing `hikac-0.0.15/app/hikac.egg-info/PKG-INFO` & `hikac-0.0.2/app/hikac.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,45 @@
 Metadata-Version: 2.1
 Name: hikac
-Version: 0.0.15
+Version: 0.0.2
 Summary: A hikvision access control request manager
 Home-page: https://github.com/yusufjonc07/hikac
 Author: YusufAxmad
 Author-email: studentyusufaxmad@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# HIKAC
+# HIKVISION AC REQUEST MANAGER
+A package used to get needy data from Hikvision ac device request.
 
-This modest python package helps you to get events from HIKVISION AC terminals. 
-
-## Installation
-
-```sh
-pip install hikac
-
-```
-
-## Usage in FastAPI
-
-```sh
-
-from hikac import get_data_from_ac_event
-
-@attandance_router.post("/attandance/face-id", include_in_schema=False)
-async def listen_for_ac_event(
-    req: Request,
-    db: Session = ActiveSession,
-):
-    try:
-
-        # use the class to collect nececary items of dict
-        eventData = await get_data_from_ac_event(req)
-
-        if eventData.attendanceStatus:
-
-            #you can use these attributes
-            #eventData.deviceIpAddress
-            #eventData.attendanceStatus
-            #eventData.deviceName
-            #eventData.dateTime
-            #eventData.employeeId
-            #eventData.employeeName
-
-            # write  your logic here
-
-            return "success"
-    except Exception as e:
-        print(e.args)
-```
-
-## How to configure Hikvision device - Soon!
-![Http Litening](./hiklistening.jpg)
+## How to use
+_After installing the package use following import:_ <br>
 
+**from hikac import get_data_from_ac_event
 
+_In Your Api router, you can also use like that:_
+
+**@attandance_router.post("/attandance/face-id", include_in_schema=False)
+**async def get_attandance_users_list(
+**    req: Request,
+**    db: Session = ActiveSession,
+**):
+**    try:
+**        # use the class to collect nececary items of dict
+**        eventData = await get_data_from_ac_event(req)
+**
+**        if eventData.attendanceStatus:
+**            await makeDavomat(eventData.employeeId, eventData.attendanceStatus, eventData.dateTime, eventData.deviceName, db)
+**
+**            return "success"
+**    except Exception as e:
+**        print(e.args)
+**
```

### Comparing `hikac-0.0.15/setup.py` & `hikac-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="hikac",
-    version="0.0.15",
+    version="0.0.2",
     description="A hikvision access control request manager",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/yusufjonc07/hikac",
     author="YusufAxmad",
```

