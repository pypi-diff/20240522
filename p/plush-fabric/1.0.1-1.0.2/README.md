# Comparing `tmp/plush_fabric-1.0.1.tar.gz` & `tmp/plush_fabric-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plush_fabric-1.0.1.tar", last modified: Fri May 10 21:44:05 2024, max compression
+gzip compressed data, was "plush_fabric-1.0.2.tar", last modified: Tue May 21 22:19:02 2024, max compression
```

## Comparing `plush_fabric-1.0.1.tar` & `plush_fabric-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:05.617978 plush_fabric-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/LICENSE.TXT
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-10 21:44:05.617978 plush_fabric-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:05.613978 plush_fabric-1.0.1/plush/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:05.613978 plush_fabric-1.0.1/plush/fabric_commands/
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/fabric_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/fabric_commands/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/fabric_commands/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/fabric_commands/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/oauth_flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:05.613978 plush_fabric-1.0.1/plush/patchwork/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/patchwork/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/patchwork/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/patchwork/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/plush/repo_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 21:44:05.617978 plush_fabric-1.0.1/plush_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-10 21:44:05.000000 plush_fabric-1.0.1/plush_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-10 21:44:05.617978 plush_fabric-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-10 21:44:02.000000 plush_fabric-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/LICENSE.TXT
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/plush/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/plush/fabric_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/fabric_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/fabric_commands/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/fabric_commands/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/fabric_commands/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/oauth_flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/plush/patchwork/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/patchwork/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/patchwork/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/patchwork/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/plush/repo_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:19:02.644431 plush_fabric-1.0.2/plush_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 22:19:02.000000 plush_fabric-1.0.2/plush_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-21 22:19:02.648431 plush_fabric-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 22:18:59.000000 plush_fabric-1.0.2/setup.py
```

### Comparing `plush_fabric-1.0.1/LICENSE.TXT` & `plush_fabric-1.0.2/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/PKG-INFO` & `plush_fabric-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plush-fabric
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
 Home-page: https://github.com/kbarnes3/Plush
 Author: Kevin Barnes
 Author-email: kbarnes3@gmail.com
 Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
 Keywords: Fabric,GitHub,deployment
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 Requires-Dist: oauth2client>=4.1.3
 Requires-Dist: PyGithub>=2.3.0
-Requires-Dist: keyring>=25.2.0
+Requires-Dist: keyring>=25.2.1
 Requires-Dist: fabric>=3.2.2
 Requires-Dist: colorama>=0.4.6
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Provides-Extra: publish
 Requires-Dist: build; extra == "publish"
 Requires-Dist: twine; extra == "publish"
```

### Comparing `plush_fabric-1.0.1/README.md` & `plush_fabric-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/console.py` & `plush_fabric-1.0.2/plush/console.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/fabric_commands/__init__.py` & `plush_fabric-1.0.2/plush/fabric_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/fabric_commands/git.py` & `plush_fabric-1.0.2/plush/fabric_commands/git.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/fabric_commands/permissions.py` & `plush_fabric-1.0.2/plush/fabric_commands/permissions.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/fabric_commands/ssh_key.py` & `plush_fabric-1.0.2/plush/fabric_commands/ssh_key.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/oauth_flow.py` & `plush_fabric-1.0.2/plush/oauth_flow.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/patchwork/files.py` & `plush_fabric-1.0.2/plush/patchwork/files.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/patchwork/util.py` & `plush_fabric-1.0.2/plush/patchwork/util.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush/repo_keys.py` & `plush_fabric-1.0.2/plush/repo_keys.py`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/plush_fabric.egg-info/PKG-INFO` & `plush_fabric-1.0.2/plush_fabric.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plush-fabric
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
 Home-page: https://github.com/kbarnes3/Plush
 Author: Kevin Barnes
 Author-email: kbarnes3@gmail.com
 Project-URL: Bug Tracker, https://github.com/kbarnes3/Plush/issues
 Keywords: Fabric,GitHub,deployment
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 Requires-Dist: oauth2client>=4.1.3
 Requires-Dist: PyGithub>=2.3.0
-Requires-Dist: keyring>=25.2.0
+Requires-Dist: keyring>=25.2.1
 Requires-Dist: fabric>=3.2.2
 Requires-Dist: colorama>=0.4.6
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Provides-Extra: publish
 Requires-Dist: build; extra == "publish"
 Requires-Dist: twine; extra == "publish"
```

### Comparing `plush_fabric-1.0.1/plush_fabric.egg-info/SOURCES.txt` & `plush_fabric-1.0.2/plush_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plush_fabric-1.0.1/setup.cfg` & `plush_fabric-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plush-fabric
-version = 1.0.1
+version = 1.0.2
 author = Kevin Barnes
 author_email = kbarnes3@gmail.com
 description = Helper library for Fabric to simplify creating and managing GitHub deploy keys when deploying GitHub-hosted repositories
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kbarnes3/Plush
 project_urls = 
@@ -24,15 +24,15 @@
 	plush
 	plush.fabric_commands
 	plush.patchwork
 python_requires = >=3.12
 install_requires = 
 	oauth2client>=4.1.3
 	PyGithub>=2.3.0
-	keyring>=25.2.0
+	keyring>=25.2.1
 	fabric>=3.2.2
 	colorama>=0.4.6
 
 [options.entry_points]
 console_scripts = 
 	auth = plush.console:auth_entry
 	listkeys = plush.console:list_keys_entry
```

