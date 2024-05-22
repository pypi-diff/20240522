# Comparing `tmp/fps_yjs-0.5.4.tar.gz` & `tmp/fps_yjs-0.6.0.tar.gz`

## Comparing `fps_yjs-0.5.4.tar` & `fps_yjs-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/py.typed
--rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/routes.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/utils.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/ybasedoc.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/yblob.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/yfile.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/ynotebook.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ydocs/yunicode.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/awareness.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/django_channels_consumer.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket_provider.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket_server.py
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/yroom.py
--rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/ystore.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywebsocket/yutils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywidgets/__init__.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/fps_yjs/ywidgets/widgets.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/README.md
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fps_yjs-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/routes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/utils.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/ybasedoc.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/yblob.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/yfile.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/ynotebook.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ydocs/yunicode.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/awareness.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/django_channels_consumer.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket_provider.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket_server.py
+-rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/yroom.py
+-rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/ystore.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywebsocket/yutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywidgets/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/fps_yjs/ywidgets/widgets.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 fps_yjs-0.6.0/PKG-INFO
```

### Comparing `fps_yjs-0.5.4/fps_yjs/main.py` & `fps_yjs-0.6.0/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/routes.py` & `fps_yjs-0.6.0/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ydocs/utils.py` & `fps_yjs-0.6.0/fps_yjs/ydocs/utils.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ydocs/ybasedoc.py` & `fps_yjs-0.6.0/fps_yjs/ydocs/ybasedoc.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ydocs/yblob.py` & `fps_yjs-0.6.0/fps_yjs/ydocs/yblob.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ydocs/ynotebook.py` & `fps_yjs-0.6.0/fps_yjs/ydocs/ynotebook.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ydocs/yunicode.py` & `fps_yjs-0.6.0/fps_yjs/ydocs/yunicode.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/asgi_server.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/awareness.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/awareness.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/django_channels_consumer.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket_provider.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/websocket_server.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/yroom.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/yroom.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/ystore.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/ystore.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywebsocket/yutils.py` & `fps_yjs-0.6.0/fps_yjs/ywebsocket/yutils.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/fps_yjs/ywidgets/widgets.py` & `fps_yjs-0.6.0/fps_yjs/ywidgets/widgets.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/.gitignore` & `fps_yjs-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/COPYING.md` & `fps_yjs-0.6.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/pyproject.toml` & `fps_yjs-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.5.4/PKG-INFO` & `fps_yjs-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_yjs
-Version: 0.5.4
+Version: 0.6.0
 Summary: An FPS plugin for the Yjs API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

