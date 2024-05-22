# Comparing `tmp/flask_app_install-0.1.2.tar.gz` & `tmp/flask_app_install-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_app_install-0.1.2.tar", last modified: Mon May 20 13:12:35 2024, max compression
+gzip compressed data, was "flask_app_install-0.1.3.tar", last modified: Wed May 22 03:32:06 2024, max compression
```

## Comparing `flask_app_install-0.1.2.tar` & `flask_app_install-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 13:12:35.785273 flask_app_install-0.1.2/
-drwxrwxrwx   0        0        0        0 2024-05-20 13:12:35.783274 flask_app_install-0.1.2/Flask_App_Install.egg-info/
--rw-rw-rw-   0        0        0      867 2024-05-20 13:12:35.000000 flask_app_install-0.1.2/Flask_App_Install.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2024-05-20 13:12:35.000000 flask_app_install-0.1.2/Flask_App_Install.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 13:12:35.000000 flask_app_install-0.1.2/Flask_App_Install.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-20 13:12:35.000000 flask_app_install-0.1.2/Flask_App_Install.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-20 13:12:35.000000 flask_app_install-0.1.2/Flask_App_Install.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.1.2/LICENCE
--rw-rw-rw-   0        0        0      867 2024-05-20 13:12:35.784276 flask_app_install-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       88 2024-05-20 07:39:14.000000 flask_app_install-0.1.2/README.md
--rw-rw-rw-   0        0        0      360 2024-05-20 13:06:13.000000 flask_app_install-0.1.2/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-20 13:12:35.785273 flask_app_install-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1313 2024-05-20 13:11:12.000000 flask_app_install-0.1.2/setup.py
--rw-rw-rw-   0        0        0      209 2024-05-20 12:43:39.000000 flask_app_install-0.1.2/setup.sh
-drwxrwxrwx   0        0        0        0 2024-05-20 13:12:35.780935 flask_app_install-0.1.2/src/
--rw-rw-rw-   0        0        0      106 2024-05-20 07:36:38.000000 flask_app_install-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     1836 2024-05-20 08:21:17.000000 flask_app_install-0.1.2/src/app.py
--rw-rw-rw-   0        0        0      372 2024-05-20 07:38:30.000000 flask_app_install-0.1.2/src/writefile_app.py
+drwxrwxrwx   0        0        0        0 2024-05-22 03:32:06.124428 flask_app_install-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-22 03:32:06.118432 flask_app_install-0.1.3/Flask_App_Install.egg-info/
+-rw-rw-rw-   0        0        0      951 2024-05-22 03:32:05.000000 flask_app_install-0.1.3/Flask_App_Install.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2024-05-22 03:32:05.000000 flask_app_install-0.1.3/Flask_App_Install.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 03:32:05.000000 flask_app_install-0.1.3/Flask_App_Install.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-22 03:32:05.000000 flask_app_install-0.1.3/Flask_App_Install.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 03:32:05.000000 flask_app_install-0.1.3/Flask_App_Install.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 flask_app_install-0.1.3/LICENCE
+-rw-rw-rw-   0        0        0      951 2024-05-22 03:32:06.121426 flask_app_install-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2024-05-22 03:28:51.000000 flask_app_install-0.1.3/README.md
+-rw-rw-rw-   0        0        0      360 2024-05-20 13:06:13.000000 flask_app_install-0.1.3/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-22 03:32:06.125427 flask_app_install-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2024-05-22 03:31:25.000000 flask_app_install-0.1.3/setup.py
+-rw-rw-rw-   0        0        0      209 2024-05-20 12:43:39.000000 flask_app_install-0.1.3/setup.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 03:32:06.112348 flask_app_install-0.1.3/src/
+-rw-rw-rw-   0        0        0      106 2024-05-20 07:36:38.000000 flask_app_install-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0     2029 2024-05-22 03:11:11.000000 flask_app_install-0.1.3/src/app.py
+-rw-rw-rw-   0        0        0      372 2024-05-20 07:38:30.000000 flask_app_install-0.1.3/src/writefile_app.py
```

### Comparing `flask_app_install-0.1.2/LICENCE` & `flask_app_install-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `flask_app_install-0.1.2/setup.py` & `flask_app_install-0.1.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Sets up a basic Flask App with Javascipt Functionality'
 LONG_DESCRIPTION = 'A package that sets up a basic Flask App Boilerplate with Javascript Functionality.'
 
 # Setting up
 setup(
     name="Flask_App_Install",
     version=VERSION,
     author="kunaalg",
     author_email="<kunaal@runcode.in>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
-    data_files=[('src/app.py', ['src/app.py'])],
+    include_package_data=True,
+    data_files=[('src/writefile_app.py', ['src/writefile_app.py'])],
     packages=find_packages(),
     scripts=['run.sh','setup.sh'],
     install_requires=['datetime', 'pandas', 'requests', 'numpy', 'flask', 'virtualenv', 'pipreqs', 'pip-tools'],
     keywords=['python', 'Flask', 'App', 'Javascript', 'Function', 'math'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `flask_app_install-0.1.2/src/app.py` & `flask_app_install-0.1.3/src/app.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,17 @@
         <script src="{{ url_for('static', filename='js/script.js') }}"></script>
     </head>
     <body>
         <!-- rest of your HTML code -->
     </body>
     </html>
     """
-
+    new_directory = 'templates'
+    if not os.path.exists(new_directory):
+        os.makedirs(new_directory)
     with open(os.path.join('templates', 'index.html'), 'w') as f:
         f.write(html_content)
 
 def create_script_js():
     js_content = """
     $(document).ready(function(){
         $('#myForm').on('submit', function(e){
@@ -36,16 +38,18 @@
                 success : function(response){
                     $('#result').html(response.result);
                 }
             });
         });
     });
     """
-
-    with open(os.path.join('static', 'js', 'script.js'), 'w') as f:
+    new_dir = 'static'
+    if not os.path.exists(new_dir):
+        os.makedirs(new_dir)
+    with open(os.path.join('static', 'script.js'), 'w') as f:
         f.write(js_content)
 
 def create_app():
     app = Flask(__name__)
 
     @app.route('/')
     def index():
```

