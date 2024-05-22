# Comparing `tmp/dash-flask-keycloak-1.2.1.tar.gz` & `tmp/dash_flask_keycloak-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-flask-keycloak-1.2.1.tar", last modified: Tue Mar 26 10:17:35 2024, max compression
+gzip compressed data, was "dash_flask_keycloak-1.3.1.tar", last modified: Wed May 22 10:39:23 2024, max compression
```

## Comparing `dash-flask-keycloak-1.2.1.tar` & `dash_flask_keycloak-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/
--rw-r--r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1596 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/PKG-INFO
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1014 2024-03-24 10:55:28.000000 dash-flask-keycloak-1.2.1/README.md
-drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/dash_flask_keycloak/
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       32 2023-12-21 10:20:32.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak/__init__.py
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)    19513 2024-03-26 10:10:59.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak/core.py
-drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2023-12-21 10:20:32.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/__init__.py
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1501 2024-03-26 10:13:29.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/dash_example.py
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1057 2024-03-24 10:36:05.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/flask_example.py
-drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/
--rw-r--r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1596 2024-03-26 10:17:35.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/PKG-INFO
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)      434 2024-03-26 10:17:35.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/SOURCES.txt
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        1 2024-03-26 10:17:35.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/dependency_links.txt
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       57 2024-03-26 10:17:35.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/requires.txt
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       20 2024-03-26 10:17:35.000000 dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/top_level.txt
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       79 2024-03-26 10:17:35.569291 dash-flask-keycloak-1.2.1/setup.cfg
--rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)      941 2024-03-26 10:17:27.000000 dash-flask-keycloak-1.2.1/setup.py
+drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/
+-rw-r--r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1596 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/PKG-INFO
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1014 2024-03-24 10:55:28.000000 dash_flask_keycloak-1.3.1/README.md
+drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/dash_flask_keycloak/
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       32 2023-12-21 10:20:32.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak/__init__.py
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)    19857 2024-05-22 10:23:01.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak/core.py
+drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2023-12-21 10:20:32.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/__init__.py
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1501 2024-03-26 10:13:29.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/dash_example.py
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1057 2024-03-24 10:36:05.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/flask_example.py
+drwxrwxr-x   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        0 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/
+-rw-r--r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)     1596 2024-05-22 10:39:23.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/PKG-INFO
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)      434 2024-05-22 10:39:23.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)        1 2024-05-22 10:39:23.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       57 2024-05-22 10:39:23.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/requires.txt
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       20 2024-05-22 10:39:23.000000 dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/top_level.txt
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)       79 2024-05-22 10:39:23.600573 dash_flask_keycloak-1.3.1/setup.cfg
+-rw-rw-r--   0 ilnurfayzrakhmanov  (1000) ilnurfayzrakhmanov  (1000)      941 2024-05-22 10:36:44.000000 dash_flask_keycloak-1.3.1/setup.py
```

### Comparing `dash-flask-keycloak-1.2.1/PKG-INFO` & `dash_flask_keycloak-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-flask-keycloak
-Version: 1.2.1
+Version: 1.3.1
 Summary: Extension providing Keycloak integration via the python-keycloak package to the Dash/Flask app
 Home-page: https://github.com/Ilnur786/dash-flask-keycloak
 Author: Ilnur Faizrakhmanov, Emil Haldrup Eriksen
 Author-email: ilnurfrwork@gmail.com
 License: MIT
 Keywords: python,dash,flask,keycloak,pyjwt
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dash-flask-keycloak-1.2.1/README.md` & `dash_flask_keycloak-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dash-flask-keycloak-1.2.1/dash_flask_keycloak/core.py` & `dash_flask_keycloak-1.3.1/dash_flask_keycloak/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,24 +134,25 @@
             pass
         session.clear()
         return response
 
 
 class AuthMiddleWare:
     def __init__(self, app, auth_handler, redirect_uri=None, uri_whitelist=None,
-                 prefix_callback_path=None, abort_on_unauthorized=None, before_login=None):
+                 url_prefix=None, keycloak_callback_prefix=None, abort_on_unauthorized=None, before_login=None):
         self.app = app
         self.auth_handler = auth_handler
         self._redirect_uri = redirect_uri
         self.uri_whitelist = uri_whitelist
         # Setup uris.
         self.before_login = before_login
         # Optionally, prefix callback path with current path.
-        self.prefix = prefix_callback_path.rstrip('/')
-        self.callback_path = self.prefix + "/keycloak/callback"
+        self.prefix = url_prefix.rstrip('/')
+        self.callback_path = self.prefix + keycloak_callback_prefix if keycloak_callback_prefix is not None \
+            else self.prefix + "/keycloak/callback"
         self.abort_on_unauthorized = abort_on_unauthorized
 
     def get_auth_uri(self, state, environ):
         return self.auth_handler.auth_url(state, self.get_callback_uri(environ))
 
     def get_callback_uri(self, environ):
         parse_result = urllib.parse.urlparse(self.get_redirect_uri(environ))
@@ -228,17 +229,17 @@
         # Request is authorized, just proceed.
         return self.app(environ, start_response)
 
 
 class FlaskKeycloak:
     def __init__(self, app, keycloak_openid, redirect_uri=None, uri_whitelist=None, logout_path=None,
                  heartbeat_path=None,
-                 login_path=None, prefix_callback_path=None,
+                 login_path=None, url_prefix=None,
                  abort_on_unauthorized=None, before_login=None, ssl_context=None, state_control=True,
-                 session_lifetime=None):
+                 session_lifetime=None, keycloak_callback_prefix=None):
         server = app if isinstance(app, Flask) else app.server
         logout_path = '/logout' if logout_path is None else logout_path
         uri_whitelist = [] if uri_whitelist is None else uri_whitelist
         # uri_whitelist = uri_whitelist + [logout_path]
         if heartbeat_path is not None:
             uri_whitelist = uri_whitelist + [heartbeat_path]
         if login_path is not None:
@@ -260,15 +261,15 @@
             except AttributeError:
                 app.layout.children = [app.layout.children, dcc.Location(id='url', refresh=True)]
         # Add middleware.
         auth_handler = AuthHandler(server.wsgi_app, server.config, server.session_interface, keycloak_openid,
                                    ssl_context,
                                    state_control, session_lifetime)
         auth_middleware = AuthMiddleWare(server.wsgi_app, auth_handler, redirect_uri, uri_whitelist,
-                                         prefix_callback_path, abort_on_unauthorized, before_login)
+                                         url_prefix, keycloak_callback_prefix, abort_on_unauthorized, before_login)
 
         def _save_external_url():
             g.external_url = auth_middleware.get_redirect_uri(request.environ)
 
         server.before_request(_save_external_url)
         server.wsgi_app = auth_middleware
 
@@ -308,37 +309,38 @@
                 return "Chuck Norris can kill two stones with one bird."
 
     @staticmethod
     def build(app: Union[Dash, Flask], redirect_uri: str = None, config_path: Union[str, os.PathLike] = None,
               config_data: Union[str, dict] = None,
               logout_path: str = None, heartbeat_path: str = None,
               authorization_settings_path: str = None, uri_whitelist: List[str] = None, login_path: str = None,
-              prefix_callback_path: str = '', abort_on_unauthorized: List[str] = None, debug_user=None,
+              url_prefix: str = '', abort_on_unauthorized: List[str] = None, debug_user=None,
               debug_roles: str = None, ssl_context: ssl.SSLContext = None, state_control: bool = True,
-              session_lifetime: Union[int, timedelta] = None):
+              session_lifetime: Union[int, timedelta] = None, keycloak_callback_prefix: str = None):
         """
         Build FlaskKeycloak class instance
 
         :param app: if your app is Dash one - put it here. Otherwise, put Flask app.
         :param redirect_uri: target url of the app
         :param config_path: path to the keycloak.json file
         :param config_data: keycloak parameters for KeycloakOpenID
         :param logout_path: logout path
         :param heartbeat_path: heartbeat_path
         :param authorization_settings_path: keycloak authorization settings
         :param uri_whitelist: uri which will proceed upon authorization
         :param login_path: if given, this route will proceed upon authorization and credentials can be given as json via post request
-        :param prefix_callback_path: prefix callback path
+        :param url_prefix: additional url path
         :param abort_on_unauthorized: list of url which will abort anyway and redirect to login page
         :param debug_user: username for debug
         :param debug_roles: user roles for debug
         :param ssl_context: custom ssl context for PyJWK client
         :param state_control: if True, will control state parameter in keycloak redirect uri and in session's cookie
         :param session_lifetime: if isn't None, session will include lifespan.
             Should be a datetime.timedelta object or count of seconds (int).
+        :param keycloak_callback_prefix: keycloak callback prefix, as a default: https://<url_to_app>/keycloak/callback/
         :return: FlaskKeycloak class instance
         """
         try:
             # The oidc json is either read from a file with 'config_path' or is directly passed as 'config_data'
             if not config_data:
                 # Read config, assumed to be in Keycloak OIDC JSON format.
                 config_path = "keycloak.json" if config_path is None else config_path
@@ -355,18 +357,19 @@
             # If there is not debug user and no keycloak, raise the exception.
             if before_login is None:
                 raise ex
             # Create dummy object, we are bypassing keycloak anyway.
             keycloak_openid = KeycloakOpenID("url", "name", "client_id", "client_secret_key")
         return FlaskKeycloak(app, keycloak_openid, redirect_uri, logout_path=logout_path,
                              heartbeat_path=heartbeat_path, uri_whitelist=uri_whitelist, login_path=login_path,
-                             prefix_callback_path=prefix_callback_path,
+                             url_prefix=url_prefix,
                              abort_on_unauthorized=abort_on_unauthorized,
                              before_login=_setup_debug_session(debug_user, debug_roles), ssl_context=ssl_context,
-                             state_control=state_control, session_lifetime=session_lifetime)
+                             state_control=state_control, session_lifetime=session_lifetime,
+                             keycloak_callback_prefix=keycloak_callback_prefix)
 
     @staticmethod
     def try_build(app, **kwargs):
         success = True
         try:
             FlaskKeycloak.build(app, **kwargs)
         except FileNotFoundError:
```

### Comparing `dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/dash_example.py` & `dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/dash_example.py`

 * *Files identical despite different names*

### Comparing `dash-flask-keycloak-1.2.1/dash_flask_keycloak/examples/flask_example.py` & `dash_flask_keycloak-1.3.1/dash_flask_keycloak/examples/flask_example.py`

 * *Files identical despite different names*

### Comparing `dash-flask-keycloak-1.2.1/dash_flask_keycloak.egg-info/PKG-INFO` & `dash_flask_keycloak-1.3.1/dash_flask_keycloak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-flask-keycloak
-Version: 1.2.1
+Version: 1.3.1
 Summary: Extension providing Keycloak integration via the python-keycloak package to the Dash/Flask app
 Home-page: https://github.com/Ilnur786/dash-flask-keycloak
 Author: Ilnur Faizrakhmanov, Emil Haldrup Eriksen
 Author-email: ilnurfrwork@gmail.com
 License: MIT
 Keywords: python,dash,flask,keycloak,pyjwt
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dash-flask-keycloak-1.2.1/setup.py` & `dash_flask_keycloak-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="dash-flask-keycloak",
-    version="1.2.1",
+    version="1.3.1",
     description="Extension providing Keycloak integration via the python-keycloak package to the Dash/Flask app",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Ilnur786/dash-flask-keycloak",
     author="Ilnur Faizrakhmanov, Emil Haldrup Eriksen",
     author_email="ilnurfrwork@gmail.com",
     license="MIT",
```

