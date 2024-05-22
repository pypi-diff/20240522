# Comparing `tmp/fps_terminals-0.5.4.tar.gz` & `tmp/fps_terminals-0.6.0.tar.gz`

## Comparing `fps_terminals-0.5.4.tar` & `fps_terminals-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/fps_terminals/main.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/fps_terminals/routes.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/fps_terminals/win_server.py
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/fps_terminals/main.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 fps_terminals-0.6.0/PKG-INFO
```

### Comparing `fps_terminals-0.5.4/fps_terminals/main.py` & `fps_terminals-0.6.0/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.4/fps_terminals/routes.py` & `fps_terminals-0.6.0/fps_terminals/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -41,26 +41,20 @@
         return terminal
 
     async def delete_terminal(
         self,
         name: str,
         user: User,
     ):
-        for websocket in TERMINALS[name]["server"].websockets:
-            TERMINALS[name]["server"].quit(websocket)
-        del TERMINALS[name]
+        await TERMINALS[name]["server"].exit(TERMINALS, name)
         return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
     async def terminal_websocket(
         self,
         name,
         websocket_permissions,
     ):
         if websocket_permissions is None:
             return
         websocket, permissions = websocket_permissions
         await websocket.accept()
-        await TERMINALS[name]["server"].serve(websocket, permissions)
-        if name in TERMINALS:
-            TERMINALS[name]["server"].quit(websocket)
-            if not TERMINALS[name]["server"].websockets:
-                del TERMINALS[name]
+        await TERMINALS[name]["server"].serve(websocket, permissions, TERMINALS, name)
```

### Comparing `fps_terminals-0.5.4/fps_terminals/win_server.py` & `fps_terminals-0.6.0/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.4/.gitignore` & `fps_terminals-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.4/COPYING.md` & `fps_terminals-0.6.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.4/pyproject.toml` & `fps_terminals-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_terminals-0.5.4/PKG-INFO` & `fps_terminals-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fps_terminals
-Version: 0.5.4
+Version: 0.6.0
 Summary: An FPS plugin for the terminals API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```

