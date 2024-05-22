# Comparing `tmp/slapos.rebootstrap-4.6.tar.gz` & `tmp/slapos.rebootstrap-4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slapos.rebootstrap-4.6.tar", last modified: Wed Mar 27 10:32:34 2024, max compression
+gzip compressed data, was "slapos.rebootstrap-4.7.tar", last modified: Wed May 22 13:14:27 2024, max compression
```

## Comparing `slapos.rebootstrap-4.6.tar` & `slapos.rebootstrap-4.7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-03-27 10:32:34.626668 slapos.rebootstrap-4.6/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2829 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/CHANGELOG.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)       74 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/MANIFEST.in
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7027 2024-03-27 10:32:34.626668 slapos.rebootstrap-4.6/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2001 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/README.rst
--rw-r--r--   0 tomo      (1000) tomo      (1000)       38 2024-03-27 10:32:34.626668 slapos.rebootstrap-4.6/setup.cfg
--rw-r--r--   0 tomo      (1000) tomo      (1000)     1385 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/setup.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-03-27 10:32:34.622668 slapos.rebootstrap-4.6/slapos/
--rw-r--r--   0 tomo      (1000) tomo      (1000)      245 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/__init__.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-03-27 10:32:34.626668 slapos.rebootstrap-4.6/slapos/rebootstrap/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4621 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/__init__.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2299 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/bootstrap.py
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2635 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/different_version.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)     2432 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/same_version.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)      811 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/same_version_already_installed.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)     4102 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.6/slapos/rebootstrap/tests.py
-drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-03-27 10:32:34.622668 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/
--rw-r--r--   0 tomo      (1000) tomo      (1000)     7027 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/PKG-INFO
--rw-r--r--   0 tomo      (1000) tomo      (1000)      628 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/SOURCES.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/dependency_links.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       66 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/entry_points.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/namespace_packages.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)       51 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/requires.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/top_level.txt
--rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2024-03-27 10:32:34.000000 slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/zip-safe
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2982 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/CHANGELOG.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       74 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.7/MANIFEST.in
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7236 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2001 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.7/README.rst
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       38 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/setup.cfg
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     1385 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/setup.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/slapos/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      245 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.7/slapos/__init__.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/slapos/rebootstrap/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4090 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/slapos/rebootstrap/__init__.py
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2901 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/slapos/rebootstrap/different_version.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     2757 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/slapos/rebootstrap/same_version.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      811 2024-03-27 10:32:12.000000 slapos.rebootstrap-4.7/slapos/rebootstrap/same_version_already_installed.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     4326 2024-05-22 13:14:11.000000 slapos.rebootstrap-4.7/slapos/rebootstrap/tests.py
+drwxr-xr-x   0 tomo      (1000) tomo      (1000)        0 2024-05-22 13:14:27.251719 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/
+-rw-r--r--   0 tomo      (1000) tomo      (1000)     7236 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/PKG-INFO
+-rw-r--r--   0 tomo      (1000) tomo      (1000)      596 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/SOURCES.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/dependency_links.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       66 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/entry_points.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/namespace_packages.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)       51 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/requires.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        7 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/top_level.txt
+-rw-r--r--   0 tomo      (1000) tomo      (1000)        1 2024-05-22 13:14:27.000000 slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/zip-safe
```

### Comparing `slapos.rebootstrap-4.6/CHANGELOG.rst` & `slapos.rebootstrap-4.7/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changes
 =======
 
+4.7 (2024-05-22)
+----------------
+
+- Stop using deprecated setuptools.easy_install
+- Check zc.buildout version on import
+- Unify rebootstrap mechanisms
+
 4.6 (2024-03-26)
 ----------------
 
 - Add support for slapos.buildout >= 3.0.1+slapos001
 - Support installing setuptools from tar.gz
 - Remove invalid zc.buildout>=2.7.1+slapos001 requirement
 - Remove useless monkey-patch of zc.buildout
```

### Comparing `slapos.rebootstrap-4.6/PKG-INFO` & `slapos.rebootstrap-4.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slapos.rebootstrap
-Version: 4.6
+Version: 4.7
 Summary: A zc.buildout extension to solve chicken-and-egg problem of using python which is built by itself
 Home-page: https://lab.nexedi.com/nexedi/slapos.rebootstrap
 Maintainer: Kazuhiko Shiozaki
 Maintainer-email: kazuhiko@nexedi.com
 License: ZPL 2.1
 Description: Rerun buildout with a python provided by buildout
         =================================================
@@ -69,14 +69,21 @@
         Please keep in mind that clean python environment is required -- the best one is
         provided by buildout or virtualenv *WITHOUT* site packages.
         
         
         Changes
         =======
         
+        4.7 (2024-05-22)
+        ----------------
+        
+        - Stop using deprecated setuptools.easy_install
+        - Check zc.buildout version on import
+        - Unify rebootstrap mechanisms
+        
         4.6 (2024-03-26)
         ----------------
         
         - Add support for slapos.buildout >= 3.0.1+slapos001
         - Support installing setuptools from tar.gz
         - Remove invalid zc.buildout>=2.7.1+slapos001 requirement
         - Remove useless monkey-patch of zc.buildout
```

### Comparing `slapos.rebootstrap-4.6/README.rst` & `slapos.rebootstrap-4.7/README.rst`

 * *Files identical despite different names*

### Comparing `slapos.rebootstrap-4.6/setup.py` & `slapos.rebootstrap-4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup, find_packages
-version = '4.6'
+version = '4.7'
 name = "slapos.rebootstrap"
 
 long_description = open("README.rst").read() + '\n\n'
 long_description += open("CHANGELOG.rst").read()
 
 extras_require = {
     'test': [
```

### Comparing `slapos.rebootstrap-4.6/slapos/rebootstrap/__init__.py` & `slapos.rebootstrap-4.7/slapos/rebootstrap/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,16 +8,39 @@
 # THIS SOFTWARE IS PROVIDED "AS IS" AND ANY AND ALL EXPRESS OR IMPLIED
 # WARRANTIES ARE DISCLAIMED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
 # WARRANTIES OF TITLE, MERCHANTABILITY, AGAINST INFRINGEMENT, AND FITNESS
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 
-import errno, logging, os, shutil, subprocess, sys, tempfile
-from zc.buildout import easy_install, UserError
+import errno, logging, os, shutil, subprocess, sys
+import pkg_resources
+from zc.buildout import UserError
+
+
+buildout_dist = pkg_resources.get_distribution('zc.buildout')
+if 'slapos' not in str(buildout_dist.version):
+  raise UserError(
+    "Incompatible version %s\n"
+    "Consider installing e.g. zc.buildout==3.0.1+slapos001"
+    % buildout_dist)
+
+
+def get_paths():
+  # zc.buildout and dependencies
+  dists = pkg_resources.require('zc.buildout')
+  # propagate slapos.libnetworkcache availability
+  try:
+    import slapos.libnetworkcache
+    dists.append(pkg_resources.get_distribution('slapos.libnetworkcache'))
+  except ImportError:
+    pass
+  # keep same order as in sys.path
+  paths = {d.location for d in dists}
+  return [p for p in sys.path if p in paths]
 
 
 class extension(object):
 
   def __init__(self, buildout):
     self.environ = os.environ.copy()
     self.buildout = buildout
@@ -65,59 +88,26 @@
     try:
       with open(new_bin) as x:
         x = x.readline().rstrip()
     except IOError as e:
       if e.errno != errno.ENOENT:
         raise
       x = None
-    if x != '#!' + self.wanted_python:
-      from .bootstrap import get_distributions, setup_script
-      if subprocess.call((self.wanted_python, '-c',
-          'import sys; sys.exit(sys.version_info[:2] == %r)'
-          % (sys.version_info[:2],))):
-        setup_script(new_bin, self.wanted_python)
-      else:
-        # With a different version of Python,
-        # we must reinstall required eggs from source.
-        from pkg_resources import resource_string
-        with Cache(buildout['buildout']) as cache:
-          subprocess.check_call([self.wanted_python, '-c',
-            resource_string(__name__, 'bootstrap.py'),
-            new_bin, cache._dest, cache.tmp,
-            ] + list(map(cache, get_distributions())))
-
-    shutil.copy(new_bin, installed)
+    if x == '#!' + self.wanted_python:
+      shutil.copy(new_bin, installed)
+    else:
+      old = installed + '-old'
+      shutil.move(installed, old)
+      try:
+        paths = get_paths()
+        args = [arg for arg in sys.argv if arg.startswith('buildout:')]
+        subprocess.check_call(
+          [self.wanted_python, '-c',
+          "import sys ; sys.path[0:0]=%r ; "
+          "import zc.buildout.buildout ; "
+          "sys.argv[1:1]=%r ; "
+          "zc.buildout.buildout.main()" % (paths, args + ['bootstrap'])])
+      except subprocess.CalledProcessError:
+        shutil.move(old, installed)
+        raise
+      shutil.copy(installed, new_bin)
     os.execve(self.wanted_python, [self.wanted_python] + sys.argv, self.environ)
-
-
-class Cache(easy_install.Installer):
-
-  def __init__(self, buildout):
-    easy_install.Installer.__init__(self,
-      buildout['eggs-directory'],
-      buildout.get('find-links', '').split())
-
-  def __enter__(self):
-    self.tmp = self._download_cache or tempfile.mkdtemp('get_dist')
-    return self
-
-  def __exit__(self, t, v, tb):
-    if self.tmp is not self._download_cache:
-      shutil.rmtree(self.tmp)
-    del self.tmp
-
-  def __call__(self, dist):
-    req = dist.as_requirement()
-    cache = self._download_cache
-    if cache:
-      from pkg_resources import SOURCE_DIST
-      for avail in self._index[dist.project_name]:
-        if (avail.version == dist.version and
-            avail.precedence == SOURCE_DIST and
-            cache == os.path.dirname(avail.location)):
-          return str(req)
-    avail = self._obtain(req, True)
-    if avail is None:
-      raise UserError("Couldn't find a distribution for %r" % str(req))
-    if self._fetch(avail, self.tmp, cache) is None:
-      raise UserError("Couldn't download distribution %s." % avail)
-    return str(req)
```

### Comparing `slapos.rebootstrap-4.6/slapos/rebootstrap/different_version.txt` & `slapos.rebootstrap-4.7/slapos/rebootstrap/different_version.txt`

 * *Files 18% similar despite different names*

```diff
@@ -58,24 +58,34 @@
 ... [installpython]
 ... recipe = recipes:pyinstall
 ...
 ... [realrun]
 ... recipe = recipes:pyshow
 ... """ % dict(syspython=sys.executable))
 
+>>> cat(buildout) # doctest: +ELLIPSIS
+#!/system_python
+...
+
 >>> print(system(buildout, env={'PYTHONWARNINGS':'ignore'})) # doctest: +ELLIPSIS
 slapos.rebootstrap: Make sure that the section 'installpython' won't be reinstalled after rebootstrap.
 Develop: '/sample-buildout/recipes'
 Installing installpython.
 slapos.rebootstrap: 
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
 bin/buildout is being reinstalled right now, as new python:
   /sample_buildout/parts/installpython/bin/python
 is available, and buildout is using another python:
   /system_python
 Buildout will be restarted automatically to have this change applied.
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
 <BLANKLINE>
-While:
-  Installing.
-Error: Couldn't find a distribution for 'setuptools==...'
+Generated script '/sample-buildout/bin/buildout'.
+Develop: '/sample-buildout/recipes'
+Updating installpython.
+Installing realrun.
+Running with: /sample_buildout/parts/installpython/bin/python
 <BLANKLINE>
+
+>>> cat(buildout) # doctest: +ELLIPSIS
+/sample-buildout/parts/installpython/bin/python
+...
```

### Comparing `slapos.rebootstrap-4.6/slapos/rebootstrap/same_version.txt` & `slapos.rebootstrap-4.7/slapos/rebootstrap/same_version.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,41 +18,53 @@
 ... [installpython]
 ... recipe = recipes:pyinstall
 ...
 ... [realrun]
 ... recipe = recipes:pyshow
 ... """ % dict(syspython=sys.executable))
 
+>>> cat(buildout) # doctest: +ELLIPSIS
+#!/system_python
+...
+
 >>> print(system(buildout, env={'PYTHONWARNINGS':'ignore'}))
 slapos.rebootstrap: Make sure that the section 'installpython' won't be reinstalled after rebootstrap.
 Develop: '/sample-buildout/recipes'
 Installing installpython.
 slapos.rebootstrap: 
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
 bin/buildout is being reinstalled right now, as new python:
   /sample_buildout/parts/installpython/bin/python
 is available, and buildout is using another python:
   /system_python
 Buildout will be restarted automatically to have this change applied.
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
 <BLANKLINE>
-Generated script '/sample-buildout/bin/buildout-rebootstrap'.
+Generated script '/sample-buildout/bin/buildout'.
 Develop: '/sample-buildout/recipes'
 Updating installpython.
 Installing realrun.
 Running with: /sample_buildout/parts/installpython/bin/python
 <BLANKLINE>
 
+>>> cat(buildout) # doctest: +ELLIPSIS
+/sample-buildout/parts/installpython/bin/python
+...
+
 >>> print(system(buildout, env={'PYTHONWARNINGS':'ignore'}))
 Develop: '/sample-buildout/recipes'
 Updating installpython.
 Updating realrun.
 Running with: /sample_buildout/parts/installpython/bin/python
 <BLANKLINE>
 
+>>> cat(buildout) # doctest: +ELLIPSIS
+/sample-buildout/parts/installpython/bin/python
+...
+
 >>> cp(buildout + '-orig', buildout)
 >>> print(system(buildout, env={'PYTHONWARNINGS':'ignore'}))
 slapos.rebootstrap: Make sure that the section 'installpython' won't be reinstalled after rebootstrap.
 Develop: '/sample-buildout/recipes'
 Updating installpython.
 slapos.rebootstrap: 
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
@@ -64,7 +76,11 @@
 ************ REBOOTSTRAP: IMPORTANT NOTICE ************
 <BLANKLINE>
 Develop: '/sample-buildout/recipes'
 Updating installpython.
 Updating realrun.
 Running with: /sample_buildout/parts/installpython/bin/python
 <BLANKLINE>
+
+>>> cat(buildout) # doctest: +ELLIPSIS
+/sample-buildout/parts/installpython/bin/python
+...
```

### Comparing `slapos.rebootstrap-4.6/slapos/rebootstrap/same_version_already_installed.txt` & `slapos.rebootstrap-4.7/slapos/rebootstrap/same_version_already_installed.txt`

 * *Files identical despite different names*

### Comparing `slapos.rebootstrap-4.6/slapos/rebootstrap/tests.py` & `slapos.rebootstrap-4.7/slapos/rebootstrap/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,23 +46,27 @@
   write(sample_buildout, 'recipes', 'pyinstall.py', """
 import os, zc.buildout, shutil, sys
 
 class Pyinstall:
 
   def __init__(self, buildout, name, options):
     self.options = options
-    options['executable'] = os.path.join(buildout['buildout'][
-      'parts-directory'], name, 'bin', 'python')
+    self.part_dir = os.path.join(buildout['buildout']['parts-directory'], name)
+    options['executable'] = os.path.join(self.part_dir, 'bin', 'python')
 
   def install(self):
     python = self.options['executable']
     if not os.path.exists(python):
-      d = os.path.dirname(python)
-      os.path.exists(d) or os.makedirs(d)
-      shutil.copy(sys.executable, python)
+      try:
+        from venv import create
+        create(self.part_dir, clear=True)
+      except ImportError:
+        d = os.path.dirname(python)
+        os.path.exists(d) or os.makedirs(d)
+        shutil.copy(sys.executable, python)
     return []
 
   update = install
 """)
   write(sample_buildout, 'recipes', 'pyalreadyinstalled.py', """
 from __future__ import print_function
 import os, zc.buildout, shutil, sys
@@ -120,14 +124,15 @@
                          ' /sample_buildout'),
                         (re.compile(sys.executable),
                          '/system_python'),
                         (re.compile('.*CryptographyDeprecationWarning: Python 2 is no longer supported.*\n.*\n'),
                          ''),
                         zc.buildout.testing.normalize_path,
                         zc.buildout.testing.not_found,
+                        zc.buildout.testing.root_logger_messages,
                         ]),
     )
   test_list = []
   for text in pkg_resources.resource_listdir(__name__, '.'):
     if text.endswith('.txt'):
       test_list.append(doctest.DocFileSuite(text, **kwargs))
   suite = unittest.TestSuite(test_list)
```

### Comparing `slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/PKG-INFO` & `slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slapos.rebootstrap
-Version: 4.6
+Version: 4.7
 Summary: A zc.buildout extension to solve chicken-and-egg problem of using python which is built by itself
 Home-page: https://lab.nexedi.com/nexedi/slapos.rebootstrap
 Maintainer: Kazuhiko Shiozaki
 Maintainer-email: kazuhiko@nexedi.com
 License: ZPL 2.1
 Description: Rerun buildout with a python provided by buildout
         =================================================
@@ -69,14 +69,21 @@
         Please keep in mind that clean python environment is required -- the best one is
         provided by buildout or virtualenv *WITHOUT* site packages.
         
         
         Changes
         =======
         
+        4.7 (2024-05-22)
+        ----------------
+        
+        - Stop using deprecated setuptools.easy_install
+        - Check zc.buildout version on import
+        - Unify rebootstrap mechanisms
+        
         4.6 (2024-03-26)
         ----------------
         
         - Add support for slapos.buildout >= 3.0.1+slapos001
         - Support installing setuptools from tar.gz
         - Remove invalid zc.buildout>=2.7.1+slapos001 requirement
         - Remove useless monkey-patch of zc.buildout
```

### Comparing `slapos.rebootstrap-4.6/slapos.rebootstrap.egg-info/SOURCES.txt` & `slapos.rebootstrap-4.7/slapos.rebootstrap.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,12 +8,11 @@
 slapos.rebootstrap.egg-info/dependency_links.txt
 slapos.rebootstrap.egg-info/entry_points.txt
 slapos.rebootstrap.egg-info/namespace_packages.txt
 slapos.rebootstrap.egg-info/requires.txt
 slapos.rebootstrap.egg-info/top_level.txt
 slapos.rebootstrap.egg-info/zip-safe
 slapos/rebootstrap/__init__.py
-slapos/rebootstrap/bootstrap.py
 slapos/rebootstrap/different_version.txt
 slapos/rebootstrap/same_version.txt
 slapos/rebootstrap/same_version_already_installed.txt
 slapos/rebootstrap/tests.py
```

