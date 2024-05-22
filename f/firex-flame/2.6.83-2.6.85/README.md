# Comparing `tmp/firex_flame-2.6.83.tar.gz` & `tmp/firex_flame-2.6.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firex_flame-2.6.83.tar", last modified: Wed Apr 24 13:55:28 2024, max compression
+gzip compressed data, was "firex_flame-2.6.85.tar", last modified: Wed May 22 14:54:05 2024, max compression
```

## Comparing `firex_flame-2.6.83.tar` & `firex_flame-2.6.85.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-04-24 13:55:04.000000 firex_flame-2.6.83/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-04-24 13:55:04.000000 firex_flame-2.6.83/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-04-24 13:55:28.766620 firex_flame-2.6.83/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-04-24 13:55:04.000000 firex_flame-2.6.83/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-04-24 13:55:04.000000 firex_flame-2.6.83/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.767620 firex_flame-2.6.83/firex_flame/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-04-24 13:55:28.767620 firex_flame-2.6.83/firex_flame/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    15302 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/api.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/controller.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/event_broker_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/event_file_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/flame_helper.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    43510 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/flame_task_graph.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/launcher.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/main_app.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/model_dumper.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/firex_flame/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/templates/index.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-04-24 13:55:04.000000 firex_flame-2.6.83/firex_flame/web_app.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-04-24 13:55:28.766620 firex_flame-2.6.83/firex_flame.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      286 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      137 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      172 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-04-24 13:55:28.000000 firex_flame-2.6.83/firex_flame.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-04-24 13:55:28.767620 firex_flame-2.6.83/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1675 2024-04-24 13:55:04.000000 firex_flame-2.6.83/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-04-24 13:55:04.000000 firex_flame-2.6.83/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-05-22 14:53:50.000000 firex_flame-2.6.85/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-05-22 14:53:50.000000 firex_flame-2.6.85/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      785 2024-05-22 14:54:05.717453 firex_flame-2.6.85/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-05-22 14:53:50.000000 firex_flame-2.6.85/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-05-22 14:53:50.000000 firex_flame-2.6.85/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.718453 firex_flame-2.6.85/firex_flame/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-05-22 14:54:05.718453 firex_flame-2.6.85/firex_flame/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15544 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/api.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/controller.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/event_broker_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/event_file_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/flame_helper.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    43510 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/flame_task_graph.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/launcher.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/main_app.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/model_dumper.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/firex_flame/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/templates/index.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/web_app.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/firex_flame.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      785 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      136 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      257 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-05-22 14:54:05.718453 firex_flame-2.6.85/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1928 2024-05-22 14:53:50.000000 firex_flame-2.6.85/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-05-22 14:53:50.000000 firex_flame-2.6.85/versioneer.py
```

### Comparing `firex_flame-2.6.83/LICENSE` & `firex_flame-2.6.85/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/README.md` & `firex_flame-2.6.85/README.md`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/fastentrypoints.py` & `firex_flame-2.6.85/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/__main__.py` & `firex_flame-2.6.85/firex_flame/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/api.py` & `firex_flame-2.6.85/firex_flame/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,18 +359,25 @@
 
     @web_app.route('/api/revoke/<uuid>', methods=['GET', 'POST'])
     def rest_revoke_task(uuid):
         return _rest_revoke_task(uuid)
 
     @web_app.route('/api/revoke', methods=['GET', 'POST'])
     def rest_revoke_root_task():
-        root_uuid = controller.graph.root_uuid
+        # a revoke run quickly after submission
+        # might be received before the root task is known,
+        # so wait a brief amount of time.
+        root_uuid = wait_until(
+            lambda: controller.graph.root_uuid,
+            timeout=5,
+            sleep_for=0.1,
+        )
+        logger.debug(f'Revoking entire run via root task UUID: {root_uuid}')
         if not root_uuid:
             return '', 500
-        logger.debug(f'Revoking entire run via root task UUID: {root_uuid}')
         return _rest_revoke_task(root_uuid)
 
     def _revoke_task(uuid, type, user, revoke_reason):
         msg = f"Received {type} request to revoke {uuid} from user {user}"
         if revoke_reason:
             msg += f' with reason: {revoke_reason}'
             revoke_reason = revoke_reason[:200] # trim since we'll store this.
```

### Comparing `firex_flame-2.6.83/firex_flame/controller.py` & `firex_flame-2.6.85/firex_flame/controller.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/event_broker_processor.py` & `firex_flame-2.6.85/firex_flame/event_broker_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/event_file_processor.py` & `firex_flame-2.6.85/firex_flame/event_file_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/flame_helper.py` & `firex_flame-2.6.85/firex_flame/flame_helper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/flame_task_graph.py` & `firex_flame-2.6.85/firex_flame/flame_task_graph.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/launcher.py` & `firex_flame-2.6.85/firex_flame/launcher.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/main_app.py` & `firex_flame-2.6.85/firex_flame/main_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/model_dumper.py` & `firex_flame-2.6.85/firex_flame/model_dumper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/templates/index.html` & `firex_flame-2.6.85/firex_flame/templates/index.html`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame/web_app.py` & `firex_flame-2.6.85/firex_flame/web_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/firex_flame.egg-info/SOURCES.txt` & `firex_flame-2.6.85/firex_flame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.83/setup.py` & `firex_flame-2.6.85/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,23 @@
             "requests",
             "beautifulsoup4",
             "paramiko",
             "gevent-websocket",
             "gevent",
             "importlib-resources",
             "jsonpath-ng",
+
+            # pin to debug seg fail in Open Source CI.
+            # "setuptools==69.5.1",
+
+            "zope.interface==6.3",
+            "zipp==3.18.1",
+            "bcrypt==4.1.2",
+            "cryptography==42.0.5",
+            "rapidfuzz==3.8.1",
       ],
       package_data={
         'firex_flame': ['templates/*.html'],
       },
       entry_points={
           'console_scripts': ['firex_flame = firex_flame.__main__:main'],
           'firex_tracking_service': ['flame_launcher = firex_flame.launcher:FlameLauncher', ],
```

### Comparing `firex_flame-2.6.83/versioneer.py` & `firex_flame-2.6.85/versioneer.py`

 * *Files identical despite different names*

