# Comparing `tmp/pipxu-1.8.tar.gz` & `tmp/pipxu-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipxu-1.8.tar", last modified: Sat Apr  6 04:32:47 2024, max compression
+gzip compressed data, was "pipxu-1.9.tar", last modified: Tue Apr  9 10:51:11 2024, max compression
```

## Comparing `pipxu-1.8.tar` & `pipxu-1.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/
--rw-r--r--   0 mark      (1000) mark      (1000)       74 2024-04-04 00:13:06.000000 pipxu-1.8/.flake8
--rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-04-04 00:13:06.000000 pipxu-1.8/.gitignore
--rw-r--r--   0 mark      (1000) mark      (1000)      472 2024-04-04 00:13:57.000000 pipxu-1.8/Makefile
--rw-r--r--   0 mark      (1000) mark      (1000)    16992 2024-04-06 04:32:47.460507 pipxu-1.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    16469 2024-04-05 03:58:58.000000 pipxu-1.8/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/doc/
--rw-r--r--   0 mark      (1000) mark      (1000)     2539 2024-04-04 00:13:06.000000 pipxu-1.8/doc/debug.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/__main__.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu/commands/
--rw-r--r--   0 mark      (1000) mark      (1000)     1729 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/debug.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1192 2024-04-06 00:46:58.000000 pipxu-1.8/pipxu/commands/inject.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4772 2024-04-06 03:52:55.000000 pipxu-1.8/pipxu/commands/install.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1442 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/list.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1515 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/reinstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2960 2024-04-06 00:46:43.000000 pipxu-1.8/pipxu/commands/reinstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      964 2024-04-06 00:46:12.000000 pipxu-1.8/pipxu/commands/runpip.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1182 2024-04-06 00:46:28.000000 pipxu-1.8/pipxu/commands/uninject.py
--rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/uninstall-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)      938 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/uninstall.py
--rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu/commands/upgrade-all.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1413 2024-04-06 00:47:39.000000 pipxu-1.8/pipxu/commands/upgrade.py
--rw-r--r--   0 mark      (1000) mark      (1000)     1607 2024-04-06 00:44:27.000000 pipxu-1.8/pipxu/commands/version.py
--rw-r--r--   0 mark      (1000) mark      (1000)     5800 2024-04-06 04:17:47.000000 pipxu-1.8/pipxu/pipxu.py
--rw-r--r--   0 mark      (1000) mark      (1000)      872 2024-04-06 03:24:54.000000 pipxu-1.8/pipxu/run.py
--rw-r--r--   0 mark      (1000) mark      (1000)    10394 2024-04-06 03:50:43.000000 pipxu-1.8/pipxu/utils.py
--rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-04 00:13:06.000000 pipxu-1.8/pipxu-bootstrap
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-06 04:32:47.460507 pipxu-1.8/pipxu.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    16992 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      688 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-06 04:32:47.000000 pipxu-1.8/pipxu.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-04 00:13:06.000000 pipxu-1.8/pyproject.toml
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-06 04:32:47.460507 pipxu-1.8/setup.cfg
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-09 10:51:11.498681 pipxu-1.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2024-04-04 00:13:06.000000 pipxu-1.9/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       60 2024-04-04 00:13:06.000000 pipxu-1.9/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      472 2024-04-04 00:13:57.000000 pipxu-1.9/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    17174 2024-04-09 10:51:11.498681 pipxu-1.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    16651 2024-04-09 10:49:35.000000 pipxu-1.9/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-09 10:51:11.495348 pipxu-1.9/doc/
+-rw-r--r--   0 mark      (1000) mark      (1000)     2539 2024-04-04 00:13:06.000000 pipxu-1.9/doc/debug.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-09 10:51:11.495348 pipxu-1.9/pipxu/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      126 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/__main__.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-09 10:51:11.498681 pipxu-1.9/pipxu/commands/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1728 2024-04-09 10:49:32.000000 pipxu-1.9/pipxu/commands/debug.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1330 2024-04-09 10:49:35.000000 pipxu-1.9/pipxu/commands/inject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5056 2024-04-09 10:49:35.000000 pipxu-1.9/pipxu/commands/install.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1442 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/commands/list.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1512 2024-04-09 10:49:32.000000 pipxu-1.9/pipxu/commands/reinstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3013 2024-04-09 10:49:35.000000 pipxu-1.9/pipxu/commands/reinstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      964 2024-04-09 10:49:32.000000 pipxu-1.9/pipxu/commands/runpip.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1182 2024-04-06 00:46:28.000000 pipxu-1.9/pipxu/commands/uninject.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      763 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/commands/uninstall-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      938 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/commands/uninstall.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      757 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu/commands/upgrade-all.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1471 2024-04-09 10:49:35.000000 pipxu-1.9/pipxu/commands/upgrade.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     1607 2024-04-06 00:44:27.000000 pipxu-1.9/pipxu/commands/version.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     5800 2024-04-06 04:17:47.000000 pipxu-1.9/pipxu/pipxu.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      872 2024-04-06 03:24:54.000000 pipxu-1.9/pipxu/run.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    10478 2024-04-09 10:49:35.000000 pipxu-1.9/pipxu/utils.py
+-rwxr-xr-x   0 mark      (1000) mark      (1000)      316 2024-04-04 00:13:06.000000 pipxu-1.9/pipxu-bootstrap
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2024-04-09 10:51:11.498681 pipxu-1.9/pipxu.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    17174 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      688 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       43 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       68 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        6 2024-04-09 10:51:11.000000 pipxu-1.9/pipxu.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1096 2024-04-04 00:13:06.000000 pipxu-1.9/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2024-04-09 10:51:11.498681 pipxu-1.9/setup.cfg
```

### Comparing `pipxu-1.8/PKG-INFO` & `pipxu-1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.8
+Version: 1.9
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -99,16 +99,16 @@
 
 Tries to work out your preferred debugger from the standard
 PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
 you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
-  args                  options and arguments to pass to application. should
-                        start with "--".
+  args                  options and arguments to pass to application, should
+                        start with "--"
 
 options:
   -h, --help            show this help message and exit
   -e EXECUTABLE, --executable EXECUTABLE
                         executable to run, default is same as "package" name
   -d DEBUGGER, --debugger DEBUGGER
                         explicit debugger package to use
@@ -130,34 +130,36 @@
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
-                           [--system-site-packages] [-v]
+                           [--system-site-packages] [-i INDEX_URL] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   --system-site-packages
                         allow venv access to system packages
+  -i INDEX_URL, --index-url INDEX_URL
+                        base URL of Python Package Index
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -184,21 +186,21 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
@@ -215,34 +217,34 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
 Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
   package     installed application name
-  args        arguments to pass to uv pip. should start with "--".
+  args        arguments to pass to uv pip, should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
@@ -368,19 +370,20 @@
 ```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
 ## Recovery
 
-The `pipxu` package also installs the `pipxu-bootstrap` shell script on
-your system so you can always recover easily from a broken `pipxu`
-installation by manually running that script. E.g. The following may be
-needed after a major or incompatible Python version upgrade where
-`pipxu` may have stopped working:
+The `pipxu` package also installs the aforementioned
+[`pipxu-bootstrap`](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
+shell script on your system so you can always recover easily from a
+broken `pipxu` installation by manually running that script. E.g. The
+following may be needed after a major or incompatible Python version
+upgrade where `pipxu` may have stopped working:
 
 ```sh
 $ pipxu-bootstrap
 $ pipxu reinstall-all --skip pipxu
 ```
 
 ## Comparison to pipx
```

### Comparing `pipxu-1.8/README.md` & `pipxu-1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,16 @@
 
 Tries to work out your preferred debugger from the standard
 PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
 you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
-  args                  options and arguments to pass to application. should
-                        start with "--".
+  args                  options and arguments to pass to application, should
+                        start with "--"
 
 options:
   -h, --help            show this help message and exit
   -e EXECUTABLE, --executable EXECUTABLE
                         executable to run, default is same as "package" name
   -d DEBUGGER, --debugger DEBUGGER
                         explicit debugger package to use
@@ -115,34 +115,36 @@
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
-                           [--system-site-packages] [-v]
+                           [--system-site-packages] [-i INDEX_URL] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   --system-site-packages
                         allow venv access to system packages
+  -i INDEX_URL, --index-url INDEX_URL
+                        base URL of Python Package Index
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -169,21 +171,21 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
@@ -200,34 +202,34 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
 Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
   package     installed application name
-  args        arguments to pass to uv pip. should start with "--".
+  args        arguments to pass to uv pip, should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
@@ -353,19 +355,20 @@
 ```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
 ## Recovery
 
-The `pipxu` package also installs the `pipxu-bootstrap` shell script on
-your system so you can always recover easily from a broken `pipxu`
-installation by manually running that script. E.g. The following may be
-needed after a major or incompatible Python version upgrade where
-`pipxu` may have stopped working:
+The `pipxu` package also installs the aforementioned
+[`pipxu-bootstrap`](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
+shell script on your system so you can always recover easily from a
+broken `pipxu` installation by manually running that script. E.g. The
+following may be needed after a major or incompatible Python version
+upgrade where `pipxu` may have stopped working:
 
 ```sh
 $ pipxu-bootstrap
 $ pipxu reinstall-all --skip pipxu
 ```
 
 ## Comparison to pipx
```

### Comparing `pipxu-1.8/doc/debug.md` & `pipxu-1.9/doc/debug.md`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/debug.py` & `pipxu-1.9/pipxu/commands/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
                         help='executable to run, '
                         'default is same as "package" name')
     parser.add_argument('-d', '--debugger',
                         help='explicit debugger package to use')
     parser.add_argument('package',
                         help='installed application name')
     parser.add_argument('args', nargs='*',
-                        help='options and arguments to pass to application. '
-                        'should start with "--".')
+                        help='options and arguments to pass to application, '
+                        'should start with "--"')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
```

### Comparing `pipxu-1.8/pipxu/commands/inject.py` & `pipxu-1.9/pipxu/commands/inject.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,13 +18,16 @@
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
 
-    pip_args = utils.make_args((args.verbose, '-v'))
+    data = utils.get_json(vdir, args) or {}
+    url = data.get('url')
+    pip_args = utils.make_args((args.verbose, '-v'), (url, f'-i "{url}"'))
     extras = ' '.join(f'"{a}"' for a in args.extras)
     if not utils.piprun(vdir, f'install{pip_args} --compile {extras}', args):
         return f'Error: failed to install "{extras}" to {pkgname}'
 
-    return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args, add=True)
+    return utils.add_or_remove_pkg(vdir, pkgname, args.extras, args,
+                                   data=data, add=True)
```

### Comparing `pipxu-1.8/pipxu/commands/install.py` & `pipxu-1.9/pipxu/commands/install.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,36 +26,40 @@
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     xgroup = parser.add_mutually_exclusive_group()
     xgroup.add_argument('-p', '--python',
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
-                        'i.e. from `pyenv versions`, e.g. "3.9".')
+                        'i.e. from `pyenv versions`, e.g. "3.9"')
     parser.add_argument('-f', '--force', action='store_true',
                         help='recreate any already installed venv')
     parser.add_argument('-e', '--editable', action='store_true',
                         help='install application[s] in editable mode')
     parser.add_argument('-d', '--include-deps', action='store_true',
                         help='include executables from dependencies')
     parser.add_argument('--system-site-packages', action='store_true',
                         help='allow venv access to system packages')
+    parser.add_argument('-i', '--index-url',
+                        help='base URL of Python Package Index')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to install')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
                                 (args.system_site_packages,
                                  '--system-site-packages'),
                                 (True, f'--python={pyexe}'))
-    pip_args = utils.make_args((args.verbose, '-v'), (args.editable, '-e'))
+    pip_args = utils.make_args((args.verbose, '-v'),
+                               (args.index_url, f'-i "{args.index_url}"'),
+                               (args.editable, '-e'))
 
     lockfile = user_runtime_path() / f'{args._prog}.lock'
     vdirbase = args._venvs_dir
     for pkg in args.package:
         # Use a lock file in case we are running multiple installs in parallel
         with FileLock(lockfile):
             vdir = get_next_vdir(vdirbase)
@@ -110,14 +114,17 @@
 
         if args.include_deps:
             data['deps'] = True
 
         if args.system_site_packages:
             data['sys'] = True
 
+        if args.index_url:
+            data['url'] = args.index_url
+
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
             pdir.unlink()
             utils.rm_vdir(vdir, args)
             return err
 
     return None
```

### Comparing `pipxu-1.8/pipxu/commands/list.py` & `pipxu-1.9/pipxu/commands/list.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/reinstall-all.py` & `pipxu-1.9/pipxu/commands/reinstall-all.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     xgroup = parser.add_mutually_exclusive_group()
     xgroup.add_argument('-p', '--python',
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
-                        'i.e. from `pyenv versions`, e.g. "3.9".')
+                        'i.e. from `pyenv versions`, e.g. "3.9"')
     parser.add_argument('--system-site-packages', action='store_true',
-                        help='allow venv access to system packages. '
-                        'Overrides the per-application setting.')
+                        help='allow venv access to system packages, '
+                        'overrides the per-application setting')
     parser.add_argument('--no-system-site-packages', action='store_true',
-                        help='remove venv access to system packages. '
-                        'Overrides the per-application setting.')
+                        help='remove venv access to system packages, '
+                        'overrides the per-application setting')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('-s', '--skip', nargs='*',
                         help='skip these applications, '
                         'e.g. "-s package1 package2"')
 
 def main(args: Namespace) -> Optional[str]:
```

### Comparing `pipxu-1.8/pipxu/commands/reinstall.py` & `pipxu-1.9/pipxu/commands/reinstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,39 +14,40 @@
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     xgroup = parser.add_mutually_exclusive_group()
     xgroup.add_argument('-p', '--python',
                         help='specify explicit python executable path')
     xgroup.add_argument('-P', '--pyenv',
                         help='pyenv python version to use, '
-                        'i.e. from `pyenv versions`, e.g. "3.9".')
+                        'i.e. from `pyenv versions`, e.g. "3.9"')
     parser.add_argument('--system-site-packages', action='store_true',
-                        help='allow venv access to system packages. '
-                        'Overrides the per-application setting.')
+                        help='allow venv access to system packages, '
+                        'overrides the per-application setting')
     parser.add_argument('--no-system-site-packages', action='store_true',
-                        help='remove venv access to system packages. '
-                        'Overrides the per-application setting.')
+                        help='remove venv access to system packages, '
+                        'overrides the per-application setting')
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to reinstall')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pyexe = utils.get_python(args)
     venv_args = utils.make_args((args.verbose, '-v'), (not args.verbose, '-q'),
                                 (True, f'--python={pyexe}'))
-    pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
         print(f'Reinstalling {pkgname} ..')
         data = utils.get_json(vdir, args) or {}
+        url = data.get('url')
+        pip_args = utils.make_args((args.verbose, '-v'), (url, f'-i "{url}"'))
 
         if args.system_site_packages or (
                 not args.no_system_site_packages and data.get('sys')):
             data['sys'] = True
         else:
             data.pop('sys', None)
```

### Comparing `pipxu-1.8/pipxu/commands/runpip.py` & `pipxu-1.9/pipxu/commands/runpip.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .. import utils
 
 def init(parser: ArgumentParser) -> None:
     'Called to add command arguments to parser at init'
     parser.add_argument('package',
                         help='installed application name')
     parser.add_argument('args', nargs='*',
-                        help='arguments to pass to uv pip. '
+                        help='arguments to pass to uv pip, '
                         'should start with "--".')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
     pkgname, vdir = utils.get_package_from_arg(args.package, args)
     if not vdir:
         return f'Application {pkgname} is not installed.'
```

### Comparing `pipxu-1.8/pipxu/commands/uninject.py` & `pipxu-1.9/pipxu/commands/uninject.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/uninstall-all.py` & `pipxu-1.9/pipxu/commands/uninstall-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/uninstall.py` & `pipxu-1.9/pipxu/commands/uninstall.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/upgrade-all.py` & `pipxu-1.9/pipxu/commands/upgrade-all.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/commands/upgrade.py` & `pipxu-1.9/pipxu/commands/upgrade.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,24 +12,25 @@
     parser.add_argument('-v', '--verbose', action='store_true',
                         help='give more output')
     parser.add_argument('package', nargs='+',
                         help='application[s] to upgrade')
 
 def main(args: Namespace) -> Optional[str]:
     'Called to action this command'
-    pip_args = utils.make_args((args.verbose, '-v'))
     for pkgname in args.package:
         pkgname, vdir = utils.get_package_from_arg(pkgname, args)
         if not vdir:
             return f'Application {pkgname} is not installed.'
 
         print(f'Upgrading {pkgname} ..')
         data = utils.get_json(vdir, args) or {}
         editpath = data.get('editpath')
-        pkg = f'-e {editpath}' if editpath else pkgname
+        pkg = f'-e "{editpath}"' if editpath else pkgname
+        url = data.get('url')
+        pip_args = utils.make_args((args.verbose, '-v'), (url, f'-i "{url}"'))
         extras = ' '.join(data.get('injected', []))
         if not utils.piprun(vdir, 'install --compile --reinstall -U'
                             f'{pip_args} {pkg} {extras}', args):
             return f'Error: failed to {args.name} {pkgname}'
 
         err = utils.make_links(vdir, pkgname, args, data)
         if err:
```

### Comparing `pipxu-1.8/pipxu/commands/version.py` & `pipxu-1.9/pipxu/commands/version.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/pipxu.py` & `pipxu-1.9/pipxu/pipxu.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/run.py` & `pipxu-1.9/pipxu/run.py`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pipxu/utils.py` & `pipxu-1.9/pipxu/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json
 import os
 import shutil
 import sys
 from argparse import Namespace
 from pathlib import Path
-from typing import Iterable, Optional
+from typing import Iterable, Optional, Any
 
 from .run import run
 
 def subenvars(path: str) -> Path:
     'Substitute environment variables in a path string'
     return Path(os.path.expandvars(path)).expanduser()
 
@@ -58,15 +58,15 @@
             if len(fields) == 2:
                 data[fields[0]] = fields[1], None
             else:
                 data[fields[0]] = fields[1], fields[2]
 
     return data
 
-def make_args(*args: tuple[bool, str]) -> str:
+def make_args(*args: tuple[Any, str]) -> str:
     'Build a string of args based on (bool, arg) pairs'
     argstr = ' '.join(v2 for v1, v2 in args if v1)
     return ' ' + argstr if argstr else ''
 
 def _load_record(rfile: Path) -> Iterable[str]:
     'Yield the executable names from a RECORD file'
     with rfile.open() as fp:
@@ -180,19 +180,21 @@
     if vdir.exists():
         if args.verbose:
             print(f'Removing {vdir}')
 
         shutil.rmtree(vdir)
 
 def add_or_remove_pkg(vdir: Path, pkgname: str, pkgs: list[str],
-                      args: Namespace, *, add: bool) -> Optional[str]:
+                      args: Namespace, *,
+                      add: bool, data: Optional[dict] = None) -> Optional[str]:
     'Record the addition/removal of a package into the virtual environment'
-    data = get_json(vdir, args)
     if not data:
-        return 'No JSON data found'
+        data = get_json(vdir, args)
+        if not data:
+            return 'No JSON data found'
 
     dataset = set(data.get('injected') or [])
     pkgset = set(pkgs)
     newset = (dataset | pkgset) if add else (dataset - pkgset)
 
     if newset:
         data['injected'] = sorted(list(newset))
```

### Comparing `pipxu-1.8/pipxu.egg-info/PKG-INFO` & `pipxu-1.9/pipxu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipxu
-Version: 1.8
+Version: 1.9
 Summary: Install and Run Python Applications in Isolated Environments using UV
 Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
 Project-URL: Homepage, https://github.com/bulletmark/pipxu
 Keywords: pipx,pip,uv,venv,virtualenv
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -99,16 +99,16 @@
 
 Tries to work out your preferred debugger from the standard
 PYTHONBREAKPOINT environment variable. If not set it defaults to pdb. Or
 you can set it explicitly with the -d/--debugger option.
 
 positional arguments:
   package               installed application name
-  args                  options and arguments to pass to application. should
-                        start with "--".
+  args                  options and arguments to pass to application, should
+                        start with "--"
 
 options:
   -h, --help            show this help message and exit
   -e EXECUTABLE, --executable EXECUTABLE
                         executable to run, default is same as "package" name
   -d DEBUGGER, --debugger DEBUGGER
                         explicit debugger package to use
@@ -130,34 +130,36 @@
   -v, --verbose  give more output
 ```
 
 ### Command `install`
 
 ```
 usage: pipxu install [-h] [-p PYTHON | -P PYENV] [-f] [-e] [-d]
-                           [--system-site-packages] [-v]
+                           [--system-site-packages] [-i INDEX_URL] [-v]
                            package [package ...]
 
 Install a Python application using an isolated virtual environment.
 
 positional arguments:
   package               application[s] to install
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   -f, --force           recreate any already installed venv
   -e, --editable        install application[s] in editable mode
   -d, --include-deps    include executables from dependencies
   --system-site-packages
                         allow venv access to system packages
+  -i INDEX_URL, --index-url INDEX_URL
+                        base URL of Python Package Index
   -v, --verbose         give more output
 ```
 
 ### Command `list`
 
 ```
 usage: pipxu list [-h] [--json] [package ...]
@@ -184,21 +186,21 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
   -s [SKIP ...], --skip [SKIP ...]
                         skip these applications, e.g. "-s package1 package2"
 ```
 
 ### Command `reinstall`
 
@@ -215,34 +217,34 @@
 
 options:
   -h, --help            show this help message and exit
   -p PYTHON, --python PYTHON
                         specify explicit python executable path
   -P PYENV, --pyenv PYENV
                         pyenv python version to use, i.e. from `pyenv
-                        versions`, e.g. "3.9".
+                        versions`, e.g. "3.9"
   --system-site-packages
-                        allow venv access to system packages. Overrides the
-                        per-application setting.
+                        allow venv access to system packages, overrides the
+                        per-application setting
   --no-system-site-packages
-                        remove venv access to system packages. Overrides the
-                        per-application setting.
+                        remove venv access to system packages, overrides the
+                        per-application setting
   -v, --verbose         give more output
 ```
 
 ### Command `runpip`
 
 ```
 usage: pipxu runpip [-h] package [args ...]
 
 Run pip with given arguments on virtual environment for the given application.
 
 positional arguments:
   package     installed application name
-  args        arguments to pass to uv pip. should start with "--".
+  args        arguments to pass to uv pip, should start with "--".
 
 options:
   -h, --help  show this help message and exit
 ```
 
 ### Command `uninject`
 
@@ -368,19 +370,20 @@
 ```sh
 $ pipxu uninstall-all --skip pipxu
 $ pipxu uninstall pipxu
 ```
 
 ## Recovery
 
-The `pipxu` package also installs the `pipxu-bootstrap` shell script on
-your system so you can always recover easily from a broken `pipxu`
-installation by manually running that script. E.g. The following may be
-needed after a major or incompatible Python version upgrade where
-`pipxu` may have stopped working:
+The `pipxu` package also installs the aforementioned
+[`pipxu-bootstrap`](https://github.com/bulletmark/pipxu/blob/main/pipxu-bootstrap)
+shell script on your system so you can always recover easily from a
+broken `pipxu` installation by manually running that script. E.g. The
+following may be needed after a major or incompatible Python version
+upgrade where `pipxu` may have stopped working:
 
 ```sh
 $ pipxu-bootstrap
 $ pipxu reinstall-all --skip pipxu
 ```
 
 ## Comparison to pipx
```

### Comparing `pipxu-1.8/pipxu.egg-info/SOURCES.txt` & `pipxu-1.9/pipxu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pipxu-1.8/pyproject.toml` & `pipxu-1.9/pyproject.toml`

 * *Files identical despite different names*

