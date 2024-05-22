# Comparing `tmp/ryry_cli-1.2.tar.gz` & `tmp/ryry_cli-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryry_cli-1.2.tar", last modified: Wed May 22 13:46:21 2024, max compression
+gzip compressed data, was "ryry_cli-1.3.tar", last modified: Wed May 22 14:20:16 2024, max compression
```

## Comparing `ryry_cli-1.2.tar` & `ryry_cli-1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:46:21.700380 ryry_cli-1.2/
--rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.2/LICENSE
--rw-rw-rw-   0        0        0     2071 2024-05-22 13:46:21.699379 ryry_cli-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 13:46:21.691280 ryry_cli-1.2/ryry/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.2/ryry/__init__.py
--rw-rw-rw-   0        0        0      150 2024-05-22 13:46:20.000000 ryry_cli-1.2/ryry/constant.py
--rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.2/ryry/main.py
--rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.2/ryry/ryry_server_socket.py
--rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.2/ryry/ryry_service.py
--rw-rw-rw-   0        0        0     8105 2024-05-21 10:48:41.000000 ryry_cli-1.2/ryry/ryry_webapi.py
--rw-rw-rw-   0        0        0    14641 2024-05-22 13:45:39.000000 ryry_cli-1.2/ryry/ryry_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:46:21.693379 ryry_cli-1.2/ryry/script_template/
--rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.2/ryry/script_template/__init__.py
--rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.2/ryry/script_template/main.py
--rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.2/ryry/script_template/run.py
--rw-rw-rw-   0        0        0     2447 2024-05-21 10:23:27.000000 ryry_cli-1.2/ryry/server_func.py
--rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.2/ryry/store.py
--rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.2/ryry/task.py
--rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.2/ryry/taskUtils.py
--rw-rw-rw-   0        0        0     3934 2024-05-22 13:45:26.000000 ryry_cli-1.2/ryry/upload.py
--rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.2/ryry/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:46:21.698380 ryry_cli-1.2/ryry_cli.egg-info/
--rw-rw-rw-   0        0        0     2071 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      539 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      167 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-22 13:46:21.000000 ryry_cli-1.2/ryry_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 13:46:21.701380 ryry_cli-1.2/setup.cfg
--rw-rw-rw-   0        0        0     2296 2024-05-22 13:45:39.000000 ryry_cli-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:20:16.465402 ryry_cli-1.3/
+-rw-rw-rw-   0        0        0     1077 2024-05-21 11:01:18.000000 ryry_cli-1.3/LICENSE
+-rw-rw-rw-   0        0        0     2071 2024-05-22 14:20:16.465402 ryry_cli-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2024-05-21 10:59:20.000000 ryry_cli-1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 14:20:16.456889 ryry_cli-1.3/ryry/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.3/ryry/__init__.py
+-rw-rw-rw-   0        0        0      150 2024-05-22 14:20:15.000000 ryry_cli-1.3/ryry/constant.py
+-rw-rw-rw-   0        0        0    10438 2024-05-21 11:07:52.000000 ryry_cli-1.3/ryry/main.py
+-rw-rw-rw-   0        0        0     5895 2024-05-21 11:10:49.000000 ryry_cli-1.3/ryry/ryry_server_socket.py
+-rw-rw-rw-   0        0        0     9198 2024-05-21 08:19:13.000000 ryry_cli-1.3/ryry/ryry_service.py
+-rw-rw-rw-   0        0        0     8082 2024-05-22 14:20:00.000000 ryry_cli-1.3/ryry/ryry_webapi.py
+-rw-rw-rw-   0        0        0    14641 2024-05-22 14:20:10.000000 ryry_cli-1.3/ryry/ryry_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:20:16.458886 ryry_cli-1.3/ryry/script_template/
+-rw-rw-rw-   0        0        0        0 2023-10-11 09:27:31.000000 ryry_cli-1.3/ryry/script_template/__init__.py
+-rw-rw-rw-   0        0        0      893 2024-03-11 07:11:36.000000 ryry_cli-1.3/ryry/script_template/main.py
+-rw-rw-rw-   0        0        0      495 2024-03-11 07:12:45.000000 ryry_cli-1.3/ryry/script_template/run.py
+-rw-rw-rw-   0        0        0     2447 2024-05-21 10:23:27.000000 ryry_cli-1.3/ryry/server_func.py
+-rw-rw-rw-   0        0        0     4375 2024-05-20 06:06:46.000000 ryry_cli-1.3/ryry/store.py
+-rw-rw-rw-   0        0        0     8723 2024-05-21 10:52:24.000000 ryry_cli-1.3/ryry/task.py
+-rw-rw-rw-   0        0        0    10277 2024-05-21 09:54:41.000000 ryry_cli-1.3/ryry/taskUtils.py
+-rw-rw-rw-   0        0        0     3984 2024-05-22 14:01:11.000000 ryry_cli-1.3/ryry/upload.py
+-rw-rw-rw-   0        0        0    13198 2024-05-21 08:18:59.000000 ryry_cli-1.3/ryry/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:20:16.464398 ryry_cli-1.3/ryry_cli.egg-info/
+-rw-rw-rw-   0        0        0     2071 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      539 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      167 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-22 14:20:16.000000 ryry_cli-1.3/ryry_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:20:16.466402 ryry_cli-1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2296 2024-05-22 14:20:10.000000 ryry_cli-1.3/setup.py
```

### Comparing `ryry_cli-1.2/LICENSE` & `ryry_cli-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/PKG-INFO` & `ryry_cli-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.2
+Version: 1.3
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.2/README.md` & `ryry_cli-1.3/README.md`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/main.py` & `ryry_cli-1.3/ryry/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/ryry_server_socket.py` & `ryry_cli-1.3/ryry/ryry_server_socket.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/ryry_service.py` & `ryry_cli-1.3/ryry/ryry_service.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/ryry_webapi.py` & `ryry_cli-1.3/ryry/ryry_webapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     try:
         requests.adapters.DEFAULT_RETRIES = 2
         s.keep_alive = False
         s.headers.update({'Connection':'close'})
         s.headers.update({'Usertoken':"0cce7cfe3629e16ee9b3ea8563305d3a15c524804da1861db07c2c867d79da63"})
         if len(files) <= 0:
             s.headers.update({'Content-Type':'application/json'})
-        res = s.post(url=f"https://api.dalipen.com/{func}", json=params, files=files, timeout=timeout, verify=False)
+        res = s.post(url=f"https://api.dalipen.com/{func}", data=params, files=files, timeout=timeout, verify=False)
         if res.status_code == 200:
             result_data = json.loads(res.content)
             res.close()
             if result_data["code"] == 0:
                 return 0, "", result_data["data"]
             else:
                 return result_data["code"], result_data["msg"], ""
@@ -162,15 +162,14 @@
     if r1 != 0:
         if failSaveNotify:
             #tasks may have failed due to network problems, so collect and resend
             saveTaskNotifyData(taskUUID, status, msg, dataStr)
         return False
     return r3
   
-retryLastTaskNotify()
 def TaskUpdateProgress(taskUUID, progress, dataStr):
     # req = aigc_ext_pb2.TaskUpdateReq()
     # req.taskUUID = taskUUID
     # req.progress = progress
     # req.data = dataStr
     
     # rsp = aigc_ext_pb2.TaskUpdateRes()
```

### Comparing `ryry_cli-1.2/ryry/ryry_widget.py` & `ryry_cli-1.3/ryry/ryry_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         replaceIfNeed(dstDir, filename, ".png")
         replaceIfNeed(dstDir, filename, ".html")
 
 def setWidgetData(root, widgetid):
     data = GetWidgetConfig(root)
     data["widget_id"] = widgetid
     data["name"] = "Demo"
-    data["version"] = "1.2"
+    data["version"] = "1.3"
     data["device_keys"] = [
         utils.generate_unique_id()
     ]
     data["cmd"] = os.path.join(root, "main.py")
     with open(os.path.join(root, "config.json"), 'w') as f:
         json.dump(data, f)
```

### Comparing `ryry_cli-1.2/ryry/script_template/main.py` & `ryry_cli-1.3/ryry/script_template/main.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/server_func.py` & `ryry_cli-1.3/ryry/server_func.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/store.py` & `ryry_cli-1.3/ryry/store.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/task.py` & `ryry_cli-1.3/ryry/task.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/taskUtils.py` & `ryry_cli-1.3/ryry/taskUtils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry/upload.py` & `ryry_cli-1.3/ryry/upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,8 +95,10 @@
     needDeleteSrc, newSrc = transcode(src)
     addtionExif(newSrc, taskUUID)
     file_name = Path(newSrc).name
     ossurl = ryry_webapi.upload(newSrc, os.path.splitext(file_name)[-1][1:])
     ossurl = additionalUrl(newSrc, ossurl)
     if needDeleteSrc:
         os.remove(newSrc)
-    return ossurl
+    return ossurl
+
+upload("C:\\Users\\123\\Desktop\\1.png", None)
```

### Comparing `ryry_cli-1.2/ryry/utils.py` & `ryry_cli-1.3/ryry/utils.py`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/ryry_cli.egg-info/PKG-INFO` & `ryry_cli-1.3/ryry_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryry-cli
-Version: 1.2
+Version: 1.3
 Summary: ryry tools
 Home-page: https://github.com/dalipenMedia
 Author: dalipen
 Author-email: dalipen01@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ryry_cli-1.2/ryry_cli.egg-info/SOURCES.txt` & `ryry_cli-1.3/ryry_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryry_cli-1.2/setup.py` & `ryry_cli-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 import os
 import subprocess
 import datetime
 
-ryry_version = "1.2"
+ryry_version = "1.3"
 ryry_build_number = int(ryry_version.replace(".",""))
 cur_dir = os.path.dirname(os.path.abspath(__file__))
 constanspy = os.path.join(cur_dir, "ryry", "constant.py")
 try:
     # result = subprocess.run("git config user.email", stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True)
     build_user = "Noh"
     # if result.returncode == 0:
@@ -20,15 +20,15 @@
 app_bulld_number={ryry_build_number}
 app_bulld_anchor="{build_user}_{build_pts}"
 app_name="ryry-cli"
 ''')
 except:
     with open(constanspy, 'w') as f:
         f.write(f'''#!!!!! do not change this file !!!!!
-app_version="1.2"
+app_version="1.3"
 app_bulld_number=1
 app_bulld_anchor=""
 app_name="ryry-cli"
 ''')
 
 with open("README.md", "r", encoding='UTF-8') as fh:
     long_description = fh.read()
```

