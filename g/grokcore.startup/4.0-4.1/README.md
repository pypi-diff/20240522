# Comparing `tmp/grokcore.startup-4.0.tar.gz` & `tmp/grokcore.startup-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grokcore.startup-4.0.tar", last modified: Fri Jul 14 06:14:17 2023, max compression
+gzip compressed data, was "grokcore.startup-4.1.tar", last modified: Wed May 22 15:41:34 2024, max compression
```

## Comparing `grokcore.startup-4.0.tar` & `grokcore.startup-4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187892 grokcore.startup-4.0/
--rw-r--r--   0 m.howitz   (502) staff       (20)     2806 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)       32 2023-07-14 06:14:16.000000 grokcore.startup-4.0/COPYRIGHT.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      145 2023-07-14 06:14:16.000000 grokcore.startup-4.0/CREDITS.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2023-07-14 06:14:16.000000 grokcore.startup-4.0/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      224 2023-07-14 06:14:16.000000 grokcore.startup-4.0/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    16878 2023-07-14 06:14:17.187973 grokcore.startup-4.0/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      515 2023-07-14 06:14:16.000000 grokcore.startup-4.0/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      478 2023-07-14 06:14:17.188246 grokcore.startup-4.0/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     2270 2023-07-14 06:14:16.000000 grokcore.startup-4.0/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.183980 grokcore.startup-4.0/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.185682 grokcore.startup-4.0/src/grokcore/
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187472 grokcore.startup-4.0/src/grokcore/startup/
--rw-r--r--   0 m.howitz   (502) staff       (20)    12454 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      823 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5906 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/debug.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     2912 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/startup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.187756 grokcore.startup-4.0/src/grokcore/startup/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)       23 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)      421 2023-07-14 06:14:16.000000 grokcore.startup-4.0/src/grokcore/startup/tests/test_grokcorestartup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-07-14 06:14:17.186882 grokcore.startup-4.0/src/grokcore.startup.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    16878 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      719 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      115 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/entry_points.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)      222 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        9 2023-07-14 06:14:17.000000 grokcore.startup-4.0/src/grokcore.startup.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1434 2023-07-14 06:14:16.000000 grokcore.startup-4.0/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.728849 grokcore.startup-4.1/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2922 2024-05-22 15:41:34.000000 grokcore.startup-4.1/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      804 2024-05-22 15:41:34.000000 grokcore.startup-4.1/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)       32 2024-05-22 15:41:34.000000 grokcore.startup-4.1/COPYRIGHT.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      145 2024-05-22 15:41:34.000000 grokcore.startup-4.1/CREDITS.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2070 2024-05-22 15:41:34.000000 grokcore.startup-4.1/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      224 2024-05-22 15:41:34.000000 grokcore.startup-4.1/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17600 2024-05-22 15:41:34.728622 grokcore.startup-4.1/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      515 2024-05-22 15:41:34.000000 grokcore.startup-4.1/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      449 2024-05-22 15:41:34.729092 grokcore.startup-4.1/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2314 2024-05-22 15:41:34.000000 grokcore.startup-4.1/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.723246 grokcore.startup-4.1/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.725336 grokcore.startup-4.1/src/grokcore/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       56 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/__init__.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.727522 grokcore.startup-4.1/src/grokcore/startup/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    12454 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      823 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5906 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/debug.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     2912 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/startup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.727826 grokcore.startup-4.1/src/grokcore/startup/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       23 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)      421 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore/startup/tests/test_grokcorestartup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-05-22 15:41:34.728073 grokcore.startup-4.1/src/grokcore.startup.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    17600 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      719 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      115 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/entry_points.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/namespace_packages.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)      225 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        9 2024-05-22 15:41:34.000000 grokcore.startup-4.1/src/grokcore.startup.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1844 2024-05-22 15:41:34.000000 grokcore.startup-4.1/tox.ini
```

### Comparing `grokcore.startup-4.0/CHANGES.rst` & `grokcore.startup-4.1/CHANGES.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Changes
 *******
 
-4.0 (2023-07-14)
+4.1 (2024-05-22)
 ================
 
-- Add support for Python 3.10, 3.11.
+- Add support for Python 3.12.
+
+- Update ``debug.py`` to run with ``IPython >= 8``. Also requiring at least
+  that version of IPython.
+
 
-- Drop support for Python 2.7, 3.5, 3.6.
+4.0 (2023-07-14)
+================
 
-- Add support for Python 3.7, 3.8 and 3.9.
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
-- Drop support for Python 3.4.
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
 
 
 3.0.1 (2018-01-12)
 ==================
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
```

### Comparing `grokcore.startup-4.0/CONTRIBUTING.md` & `grokcore.startup-4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/LICENSE.txt` & `grokcore.startup-4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/PKG-INFO` & `grokcore.startup-4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grokcore.startup
-Version: 4.0
+Version: 4.1
 Summary: Paster support for Grok projects.
 Home-page: https://github.com/zopefoundation/grokcore.startup
 Author: Grok Team
 Author-email: zope-dev@zope.dev
 License: ZPL
 Keywords: zope zope3 grok grokproject WSGI Paste paster
 Classifier: Environment :: Web Environment
@@ -14,21 +14,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.app.debug
+Requires-Dist: zope.app.wsgi
+Requires-Dist: zope.component
+Requires-Dist: zope.dottedname
+Requires-Dist: zope.publisher
 Provides-Extra: test
+Requires-Dist: zope.app.appsetup; extra == "test"
+Requires-Dist: zope.component; extra == "test"
+Requires-Dist: zope.interface; extra == "test"
+Requires-Dist: zope.security; extra == "test"
+Requires-Dist: zope.securitypolicy; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: debug
-License-File: LICENSE.txt
+Requires-Dist: IPython>=8; extra == "debug"
 
 grokcore.startup
 ****************
 
 This package provides elements for starting a `Grok`_ project with
 `paster`_ and `WSGI`_.
 
@@ -431,24 +446,29 @@
 .. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
 .. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
 .. _ipython: http://ipython.org/
 
 Changes
 *******
 
-4.0 (2023-07-14)
+4.1 (2024-05-22)
 ================
 
-- Add support for Python 3.10, 3.11.
+- Add support for Python 3.12.
+
+- Update ``debug.py`` to run with ``IPython >= 8``. Also requiring at least
+  that version of IPython.
 
-- Drop support for Python 2.7, 3.5, 3.6.
 
-- Add support for Python 3.7, 3.8 and 3.9.
+4.0 (2023-07-14)
+================
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
-- Drop support for Python 3.4.
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
 
 
 3.0.1 (2018-01-12)
 ==================
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
```

### Comparing `grokcore.startup-4.0/README.rst` & `grokcore.startup-4.1/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/setup.py` & `grokcore.startup-4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,40 +5,35 @@
 
 
 def read(*rnames):
     return open(os.path.join(os.path.dirname(__file__), *rnames)).read()
 
 
 long_description = (
-    read('README.rst')
-    + '\n' +
-    read(os.path.join('src', 'grokcore', 'startup', 'README.rst'))
-    + '\n' +
-    read('CHANGES.rst')
-)
-
+    read('README.rst') + '\n' +
+    read(os.path.join('src', 'grokcore', 'startup', 'README.rst')) + '\n' +
+    read('CHANGES.rst'))
 
 tests_require = [
     'zope.app.appsetup',
     'zope.component',
     'zope.interface',
     'zope.security',
     'zope.securitypolicy',
     'zope.testing',
     'zope.testrunner',
 ]
 
-
 debug_requires = [
-    'IPython',
+    'IPython >= 8',
 ]
 
 setup(
     name='grokcore.startup',
-    version='4.0',
+    version='4.1',
     author='Grok Team',
     author_email='zope-dev@zope.dev',
     url='https://github.com/zopefoundation/grokcore.startup',
     description='Paster support for Grok projects.',
     long_description=long_description,
     license='ZPL',
     keywords='zope zope3 grok grokproject WSGI Paste paster',
@@ -50,14 +45,15 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
     packages=find_packages('src'),
     package_dir={'': 'src'},
     namespace_packages=['grokcore'],
```

### Comparing `grokcore.startup-4.0/src/grokcore/startup/README.rst` & `grokcore.startup-4.1/src/grokcore/startup/README.rst`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/src/grokcore/startup/__init__.py` & `grokcore.startup-4.1/src/grokcore/startup/__init__.py`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/src/grokcore/startup/debug.py` & `grokcore.startup-4.1/src/grokcore/startup/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,22 @@
 import os.path
 import textwrap
 from pprint import pprint
 
 import transaction
 import zope.app.debug
 import zope.app.wsgi
-from IPython.frontend.terminal.embed import InteractiveShellEmbed
+from IPython.terminal.embed import InteractiveShellEmbed
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.securitypolicy.zopepolicy import settingsForObject
 
 
 shell = InteractiveShellEmbed()
 
-
 PATH_SEP = '/'
 
 
 class GrokDebug:
 
     def __init__(self, debugger):
         debugger = debugger
@@ -68,16 +67,17 @@
                     pby=self.providedBy,
                     commit=transaction.commit)
 
     def update_ns(self):
         shell.user_ns.update(self.ns())
 
     def get_security_settings(self, path):
-        pprint(settingsForObject(get_context_by_path(
-                    self.get_start_context(path), path)))
+        pprint(
+            settingsForObject(
+                get_context_by_path(self.get_start_context(path), path)))
 
     def sync(self):
         self.root._p_jar.sync()
 
     def ls(self, path=None):
         """List objects.
 
@@ -173,22 +173,23 @@
         return [relpath + obj.__name__ for obj in context.values()]
 
     head, tail = os.path.split(relpath)
     if head and not head.endswith(PATH_SEP):
         head += PATH_SEP
     context = get_context_by_path(context, head)
 
-    return [head + obj.__name__ for obj in context.values()
-            if obj.__name__.startswith(tail)]
+    return [
+        head + obj.__name__ for obj in context.values()
+        if obj.__name__.startswith(tail)
+    ]
 
 
 def ipython_debug_prompt(debugger):
     grokd = GrokDebug(debugger)
-    banner = textwrap.dedent(
-        """\
+    banner = textwrap.dedent("""\
         IPython shell for Grok.
 
         Bound object names:
         -------------------
           root
           ctx
```

### Comparing `grokcore.startup-4.0/src/grokcore/startup/startup.py` & `grokcore.startup-4.1/src/grokcore/startup/startup.py`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/src/grokcore.startup.egg-info/PKG-INFO` & `grokcore.startup-4.1/src/grokcore.startup.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grokcore.startup
-Version: 4.0
+Version: 4.1
 Summary: Paster support for Grok projects.
 Home-page: https://github.com/zopefoundation/grokcore.startup
 Author: Grok Team
 Author-email: zope-dev@zope.dev
 License: ZPL
 Keywords: zope zope3 grok grokproject WSGI Paste paster
 Classifier: Environment :: Web Environment
@@ -14,21 +14,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+License-File: LICENSE.txt
+Requires-Dist: setuptools
+Requires-Dist: zope.app.debug
+Requires-Dist: zope.app.wsgi
+Requires-Dist: zope.component
+Requires-Dist: zope.dottedname
+Requires-Dist: zope.publisher
 Provides-Extra: test
+Requires-Dist: zope.app.appsetup; extra == "test"
+Requires-Dist: zope.component; extra == "test"
+Requires-Dist: zope.interface; extra == "test"
+Requires-Dist: zope.security; extra == "test"
+Requires-Dist: zope.securitypolicy; extra == "test"
+Requires-Dist: zope.testing; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 Provides-Extra: debug
-License-File: LICENSE.txt
+Requires-Dist: IPython>=8; extra == "debug"
 
 grokcore.startup
 ****************
 
 This package provides elements for starting a `Grok`_ project with
 `paster`_ and `WSGI`_.
 
@@ -431,24 +446,29 @@
 .. _WSGIPublisherApplication: http://apidoc.zope.org/++apidoc++/Code/zope/app/wsgi/WSGIPublisherApplication/index.html
 .. _zc.buildout: http://pypi.python.org/pypi/zc.buildout
 .. _ipython: http://ipython.org/
 
 Changes
 *******
 
-4.0 (2023-07-14)
+4.1 (2024-05-22)
 ================
 
-- Add support for Python 3.10, 3.11.
+- Add support for Python 3.12.
+
+- Update ``debug.py`` to run with ``IPython >= 8``. Also requiring at least
+  that version of IPython.
 
-- Drop support for Python 2.7, 3.5, 3.6.
 
-- Add support for Python 3.7, 3.8 and 3.9.
+4.0 (2023-07-14)
+================
+
+- Drop support for Python 2.7, 3.4, 3.5, 3.6.
 
-- Drop support for Python 3.4.
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
 
 
 3.0.1 (2018-01-12)
 ==================
 
 - Rearrange tests such that Travis CI can pick up all functional tests too.
```

### Comparing `grokcore.startup-4.0/src/grokcore.startup.egg-info/SOURCES.txt` & `grokcore.startup-4.1/src/grokcore.startup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grokcore.startup-4.0/tox.ini` & `grokcore.startup-4.1/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,61 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/pure-python
 [tox]
 minversion = 3.18
 envlist =
+    release-check
     lint
     py37
     py38
     py39
     py310
     py311
+    py312
     pypy3
     coverage
 
 [testenv]
 usedevelop = true
 package = wheel
 wheel_build_env = .pkg
 deps =
+setenv =
+    py312: VIRTUALENV_PIP=23.1.2
+    py312: PIP_REQUIRE_VIRTUALENV=0
 commands =
     zope-testrunner --test-path=src {posargs:-vc}
 extras =
     test
+[testenv:release-check]
+description = ensure that the distribution is ready to release
+basepython = python3
+skip_install = true
+deps =
+    twine
+    build
+    check-manifest
+    check-python-versions >= 0.20.0
+    wheel
+commands_pre =
+commands =
+    check-manifest
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
+    python -m build --sdist --no-isolation
+    twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
+deps =
+    isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
     flake8 src setup.py
-    check-manifest
-    check-python-versions
-deps =
-    check-manifest
-    check-python-versions >= 0.19.1
-    wheel
-    flake8
-    isort
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
@@ -52,22 +68,23 @@
     mkdir
 deps =
     coverage
 commands =
     mkdir -p {toxinidir}/parts/htmlcov
     coverage run -m zope.testrunner --test-path=src {posargs:-vc}
     coverage html --ignore-errors
-    coverage report --ignore-errors --show-missing --fail-under=31
+    coverage report --show-missing --fail-under=31
 
 [coverage:run]
 branch = True
 source = grokcore.startup
 
 [coverage:report]
 precision = 2
+ignore_errors = True
 exclude_lines =
     pragma: no cover
     pragma: nocover
     except ImportError:
     raise NotImplementedError
     if __name__ == '__main__':
     self.fail
```

