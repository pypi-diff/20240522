# Comparing `tmp/cs.fs-20240422.tar.gz` & `tmp/cs.fs-20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fs-20240422.tar", last modified: Mon Apr 22 02:50:34 2024, max compression
+gzip compressed data, was "cs.fs-20240522.tar", last modified: Tue May 21 23:27:58 2024, max compression
```

## Comparing `cs.fs-20240422.tar` & `cs.fs-20240522.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.952857 cs.fs-20240422/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-04-22 02:50:19.000000 cs.fs-20240422/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)     8337 2024-04-22 02:50:34.952527 cs.fs-20240422/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)     7523 2024-04-22 02:50:24.000000 cs.fs-20240422/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.947802 cs.fs-20240422/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.948092 cs.fs-20240422/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.949849 cs.fs-20240422/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    14257 2024-04-22 02:50:00.000000 cs.fs-20240422/lib/python/cs/fs.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-04-22 02:50:34.952052 cs.fs-20240422/lib/python/cs.fs.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)     8337 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)       62 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-04-22 02:50:34.000000 cs.fs-20240422/lib/python/cs.fs.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)     8741 2024-04-22 02:50:33.000000 cs.fs-20240422/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-04-22 02:50:34.952961 cs.fs-20240422/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:27:58.628358 cs.fs-20240522/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-21 23:27:43.000000 cs.fs-20240522/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8829 2024-05-21 23:27:58.627957 cs.fs-20240522/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8015 2024-05-21 23:27:48.000000 cs.fs-20240522/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:27:58.623661 cs.fs-20240522/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:27:58.623966 cs.fs-20240522/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:27:58.625255 cs.fs-20240522/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    17426 2024-05-21 23:27:30.000000 cs.fs-20240522/lib/python/cs/fs.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:27:58.627468 cs.fs-20240522/lib/python/cs.fs.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)     8829 2024-05-21 23:27:58.000000 cs.fs-20240522/lib/python/cs.fs.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      255 2024-05-21 23:27:58.000000 cs.fs-20240522/lib/python/cs.fs.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-21 23:27:58.000000 cs.fs-20240522/lib/python/cs.fs.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)       52 2024-05-21 23:27:58.000000 cs.fs-20240522/lib/python/cs.fs.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-21 23:27:58.000000 cs.fs-20240522/lib/python/cs.fs.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)     9212 2024-05-21 23:27:56.000000 cs.fs-20240522/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-21 23:27:58.628467 cs.fs-20240522/setup.cfg
```

### Comparing `cs.fs-20240422/PKG-INFO` & `cs.fs-20240522/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20240422
+Version: 20240522
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240422*:
-New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+*Latest release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -150,24 +150,31 @@
 * `skip_suffixes`: if supplied, skip entries whose extension
   is in `skip_suffixes`
 * `sort_names`: option flag, default `False`; yield entires
   in lexical order if true
 * `follow_symlinks`: optional flag, default `False`; passed to `scandir`
 * `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
-## Function `shortpath(path, prefixes=None)`
+## Function `shortpath(fspath, prefixes=None, *, collapseuser=False, foldsymlinks=False)`
 
-Return `path` with the first matching leading prefix replaced.
+Return `fspath` with the first matching leading prefix replaced.
 
 Parameters:
-* `environ`: environment mapping if not os.environ
-* `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
-  each `prefix` is subject to environment variable
-  substitution before consideration
-  The default considers "$HOME/" for replacement by "~/".
+* `prefixes`: optional list of `(prefix,subst)` pairs
+* `collapseuser`: optional flag to enable detection of user
+  home directory paths; default `False`
+* `foldsymlinks`: optional flag to enable detection of
+  convenience symlinks which point deeper into the path;
+  default `False`
+
+The `prefixes` is an optional iterable of `(prefix,subst)`
+to consider for replacement.  Each `prefix` is subject to
+environment variable substitution before consideration.
+The default `prefixes` is from `SHORTPATH_PREFIXES_DEFAULT`:
+`(('$HOME/', '~/'),)`.
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -182,14 +189,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
+
 *Release 20240422*:
 New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
```

### Comparing `cs.fs-20240422/README.md` & `cs.fs-20240522/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240422*:
-New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+*Latest release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -132,24 +132,31 @@
 * `skip_suffixes`: if supplied, skip entries whose extension
   is in `skip_suffixes`
 * `sort_names`: option flag, default `False`; yield entires
   in lexical order if true
 * `follow_symlinks`: optional flag, default `False`; passed to `scandir`
 * `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
-## Function `shortpath(path, prefixes=None)`
+## Function `shortpath(fspath, prefixes=None, *, collapseuser=False, foldsymlinks=False)`
 
-Return `path` with the first matching leading prefix replaced.
+Return `fspath` with the first matching leading prefix replaced.
 
 Parameters:
-* `environ`: environment mapping if not os.environ
-* `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
-  each `prefix` is subject to environment variable
-  substitution before consideration
-  The default considers "$HOME/" for replacement by "~/".
+* `prefixes`: optional list of `(prefix,subst)` pairs
+* `collapseuser`: optional flag to enable detection of user
+  home directory paths; default `False`
+* `foldsymlinks`: optional flag to enable detection of
+  convenience symlinks which point deeper into the path;
+  default `False`
+
+The `prefixes` is an optional iterable of `(prefix,subst)`
+to consider for replacement.  Each `prefix` is subject to
+environment variable substitution before consideration.
+The default `prefixes` is from `SHORTPATH_PREFIXES_DEFAULT`:
+`(('$HOME/', '~/'),)`.
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -164,14 +171,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
+
 *Release 20240422*:
 New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
```

### Comparing `cs.fs-20240422/lib/python/cs/fs.py` & `cs.fs-20240522/lib/python/cs/fs.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,37 +18,36 @@
     isdir as isdirpath,
     join as joinpath,
     normpath,
     realpath,
     relpath,
     splitext,
 )
+from pathlib import Path
+from pwd import getpwuid
 from tempfile import TemporaryDirectory
 from threading import Lock
 from typing import Any, Callable, Optional, Union
 
-from icontract import require
-
-from cs.deco import decorator
+from cs.deco import decorator, fmtdoc
 from cs.obj import SingletonMixin
 from cs.pfx import pfx, pfx_call
 
-__version__ = '20240422'
+__version__ = '20240522'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
     'install_requires': [
         'cs.deco',
         'cs.obj',
         'cs.pfx',
-        'icontract',
     ],
 }
 
 pfx_listdir = partial(pfx_call, os.listdir)
 pfx_mkdir = partial(pfx_call, os.mkdir)
 pfx_makedirs = partial(pfx_call, os.makedirs)
 pfx_rename = partial(pfx_call, os.rename)
@@ -333,40 +332,139 @@
     fspath = self._resolve_fspath(fspath)
     HasFSPath.__init__(self, fspath)
     if lock is None:
       lock = Lock()
     self._lock = lock
     return True
 
-DEFAULT_SHORTEN_PREFIXES = (('$HOME/', '~/'),)
+SHORTPATH_PREFIXES_DEFAULT = (('$HOME/', '~/'),)
 
-def shortpath(path, prefixes=None):
-  ''' Return `path` with the first matching leading prefix replaced.
+@fmtdoc
+def shortpath(
+    fspath, prefixes=None, *, collapseuser=False, foldsymlinks=False
+):
+  ''' Return `fspath` with the first matching leading prefix replaced.
 
       Parameters:
-      * `environ`: environment mapping if not os.environ
-      * `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
-        each `prefix` is subject to environment variable
-        substitution before consideration
-        The default considers "$HOME/" for replacement by "~/".
+      * `prefixes`: optional list of `(prefix,subst)` pairs
+      * `collapseuser`: optional flag to enable detection of user
+        home directory paths; default `False`
+      * `foldsymlinks`: optional flag to enable detection of
+        convenience symlinks which point deeper into the path;
+        default `False`
+
+      The `prefixes` is an optional iterable of `(prefix,subst)`
+      to consider for replacement.  Each `prefix` is subject to
+      environment variable substitution before consideration.
+      The default `prefixes` is from `SHORTPATH_PREFIXES_DEFAULT`:
+      `{SHORTPATH_PREFIXES_DEFAULT!r}`.
   '''
   if prefixes is None:
-    prefixes = DEFAULT_SHORTEN_PREFIXES
+    prefixes = SHORTPATH_PREFIXES_DEFAULT
+  if collapseuser or foldsymlinks:
+    # our resolved path
+    leaf = Path(fspath).resolve()
+    assert leaf.is_absolute()
+    # Paths from leaf-parent to root
+    parents = list(leaf.parents)
+    paths = [leaf] + parents
+
+    def statkey(P):
+      ''' A 2-tuple of `(st_dev,st_info)` from `P.stat()`
+            or `None` if the `stat` fails.
+        '''
+      try:
+        S = P.stat()
+      except OSError:
+        return None
+      return S.st_dev, S.st_ino
+
+    base_s = None
+    if collapseuser:
+      # scan for the lowest homedir in the path
+      pws = {}
+      for i, path in enumerate(paths):
+        try:
+          st = path.stat()
+        except OSError:
+          continue
+        try:
+          pw = pws[st.st_uid]
+        except KeyError:
+          pw = pws[st.st_uid] = getpwuid(st.st_uid)
+        if path.samefile(pw.pw_dir):
+          base_s = '~' if pw.pw_uid == os.geteuid() else f'~{pw.pw_name}'
+          paths = paths[:i + 1]
+          break
+    # a list of (Path,display) from base to leaf
+    paths_as = [[path, None] for path in reversed(paths)]
+    # note the display for the base Path
+    paths_as[0][1] = base_s
+    if not foldsymlinks:
+      keep_as = paths_as
+    else:
+      # look for symlinks which point deeper into the path
+      # map path keys to (i,path)
+      pathindex_by_key = {
+          sk: i
+          for sk, i in
+          ((statkey(path_as[0]), i) for i, path_as in enumerate(paths_as))
+          if sk is not None
+      }
+      # scan from the base towards the leaf, excluding the leaf
+      i = 0
+      keep_as = []
+      while i < len(paths_as) - 1:
+        path_as = paths_as[i]
+        keep_as.append(path_as)
+        path = path_as[0]
+        skip_to_i = None
+        try:
+          for entry in os.scandir(path):
+            if not entry.name.isalpha():
+              continue
+            ep = Path(entry.path)
+            try:
+              if not ep.is_symlink():
+                continue
+            except OSError:
+              continue
+            # see the the symlink resolves to a path entry
+            try:
+              pathndx = pathindex_by_key[statkey(ep)]
+            except KeyError:
+              continue
+            if skip_to_i is None or pathndx > skip_to_i:
+              # we will advance to skip_to_i
+              skip_to_i = pathndx
+              # note the symlink name for this component
+              paths_as[skip_to_i][1] = ep.name
+          i = i + 1 if skip_to_i is None else skip_to_i
+        except OSError:
+          i += 1
+    parts = list(
+        (path_as[0].path if i == 0 else path_as[0].name
+         ) if path_as[1] is None else path_as[1]
+        for i, path_as in enumerate(keep_as)
+    )
+    parts.append(leaf.name)
+    fspath = os.sep.join(parts)
+  # replace leading prefix
   for prefix, subst in prefixes:
     prefix = expandvars(prefix)
-    if path.startswith(prefix):
-      return subst + path[len(prefix):]
-  return path
+    if fspath.startswith(prefix):
+      return subst + fspath[len(prefix):]
+  return fspath
 
 def longpath(path, prefixes=None):
   ''' Return `path` with prefixes and environment variables substituted.
       The converse of `shortpath()`.
   '''
   if prefixes is None:
-    prefixes = DEFAULT_SHORTEN_PREFIXES
+    prefixes = SHORTPATH_PREFIXES_DEFAULT
   for prefix, subst in prefixes:
     if path.startswith(subst):
       path = prefix + path[len(subst):]
       break
   path = expandvars(path)
   return path
```

### Comparing `cs.fs-20240422/lib/python/cs.fs.egg-info/PKG-INFO` & `cs.fs-20240522/lib/python/cs.fs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fs
-Version: 20240422
+Version: 20240522
 Summary: Assorted filesystem related utility functions, some of which have been bloating cs.fileutils for too long.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -15,16 +15,16 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240422*:
-New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+*Latest release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -150,24 +150,31 @@
 * `skip_suffixes`: if supplied, skip entries whose extension
   is in `skip_suffixes`
 * `sort_names`: option flag, default `False`; yield entires
   in lexical order if true
 * `follow_symlinks`: optional flag, default `False`; passed to `scandir`
 * `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
-## Function `shortpath(path, prefixes=None)`
+## Function `shortpath(fspath, prefixes=None, *, collapseuser=False, foldsymlinks=False)`
 
-Return `path` with the first matching leading prefix replaced.
+Return `fspath` with the first matching leading prefix replaced.
 
 Parameters:
-* `environ`: environment mapping if not os.environ
-* `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
-  each `prefix` is subject to environment variable
-  substitution before consideration
-  The default considers "$HOME/" for replacement by "~/".
+* `prefixes`: optional list of `(prefix,subst)` pairs
+* `collapseuser`: optional flag to enable detection of user
+  home directory paths; default `False`
+* `foldsymlinks`: optional flag to enable detection of
+  convenience symlinks which point deeper into the path;
+  default `False`
+
+The `prefixes` is an optional iterable of `(prefix,subst)`
+to consider for replacement.  Each `prefix` is subject to
+environment variable substitution before consideration.
+The default `prefixes` is from `SHORTPATH_PREFIXES_DEFAULT`:
+`(('$HOME/', '~/'),)`.
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -182,14 +189,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
+
 *Release 20240422*:
 New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
```

### Comparing `cs.fs-20240422/pyproject.toml` & `cs.fs-20240522/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,40 +8,39 @@
     "python2",
     "python3",
 ]
 dependencies = [
     "cs.deco>=20240412",
     "cs.obj>=20220918",
     "cs.pfx>=20240412",
-    "icontract",
 ]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20240422"
+version = "20240522"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 Assorted filesystem related utility functions,
 some of which have been bloating cs.fileutils for too long.
 
-*Latest release 20240422*:
-New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
+*Latest release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
 
 ## Function `atomic_directory(*da, **dkw)`
 
 Decorator for a function which fills in a directory
 which calls the function against a temporary directory
 then renames the temporary to the target name on completion.
 
@@ -167,24 +166,31 @@
 * `skip_suffixes`: if supplied, skip entries whose extension
   is in `skip_suffixes`
 * `sort_names`: option flag, default `False`; yield entires
   in lexical order if true
 * `follow_symlinks`: optional flag, default `False`; passed to `scandir`
 * `recurse`: optional flag, default `True`; if true, recurse into subdrectories
 
-## Function `shortpath(path, prefixes=None)`
+## Function `shortpath(fspath, prefixes=None, *, collapseuser=False, foldsymlinks=False)`
 
-Return `path` with the first matching leading prefix replaced.
+Return `fspath` with the first matching leading prefix replaced.
 
 Parameters:
-* `environ`: environment mapping if not os.environ
-* `prefixes`: optional iterable of `(prefix,subst)` to consider for replacement;
-  each `prefix` is subject to environment variable
-  substitution before consideration
-  The default considers \"$HOME/\" for replacement by \"~/\".
+* `prefixes`: optional list of `(prefix,subst)` pairs
+* `collapseuser`: optional flag to enable detection of user
+  home directory paths; default `False`
+* `foldsymlinks`: optional flag to enable detection of
+  convenience symlinks which point deeper into the path;
+  default `False`
+
+The `prefixes` is an optional iterable of `(prefix,subst)`
+to consider for replacement.  Each `prefix` is subject to
+environment variable substitution before consideration.
+The default `prefixes` is from `SHORTPATH_PREFIXES_DEFAULT`:
+`(('$HOME/', '~/'),)`.
 
 ## Function `validate_rpath(rpath: str)`
 
 Test that `rpath` is a clean relative path with no funny business;
 raise `ValueError` if the test fails.
 
 Tests:
@@ -199,14 +205,17 @@
     False
     >>> validate_rpath('.')
 
 # Release Log
 
 
 
+*Release 20240522*:
+shortpath: new collapseuser=False, foldsymlinks=False parameters, rename DEFAULT_SHORTEN_PREFIXES to SHORTPATH_PREFIXES_DEFAULT.
+
 *Release 20240422*:
 New scandirtree scandir based version of os.walk, yielding (is_dir,fspath). New shim scandirpaths.
 
 *Release 20240412*:
 HasFSPath: explain that the __init__ is optional in the docstring.
 
 *Release 20240316*:
```

