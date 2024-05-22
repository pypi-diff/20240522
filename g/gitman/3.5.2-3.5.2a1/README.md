# Comparing `tmp/gitman-3.5.2.tar.gz` & `tmp/gitman-3.5.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitman-3.5.2.tar", max compression
+gzip compressed data, was "gitman-3.5.2a1.tar", max compression
```

## Comparing `gitman-3.5.2.tar` & `gitman-3.5.2a1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1088 2018-09-08 18:50:46.000000 gitman-3.5.2/LICENSE.md
--rw-r--r--   0        0        0     4117 2024-05-19 19:32:17.931935 gitman-3.5.2/README.md
--rw-r--r--   0        0        0      330 2024-04-27 19:05:29.618729 gitman-3.5.2/gitman/__init__.py
--rw-r--r--   0        0        0      589 2022-01-13 13:52:14.257310 gitman-3.5.2/gitman/__main__.py
--rw-r--r--   0        0        0    10748 2024-04-27 03:29:24.221458 gitman-3.5.2/gitman/cli.py
--rw-r--r--   0        0        0    11841 2024-05-22 11:05:57.613357 gitman-3.5.2/gitman/commands.py
--rw-r--r--   0        0        0     5395 2024-04-27 19:01:17.581121 gitman-3.5.2/gitman/common.py
--rw-r--r--   0        0        0      256 2021-02-12 02:33:38.716395 gitman-3.5.2/gitman/decorators.py
--rw-r--r--   0        0        0      726 2022-01-13 13:52:14.274203 gitman-3.5.2/gitman/exceptions.py
--rw-r--r--   0        0        0     8552 2024-04-27 19:52:07.997387 gitman-3.5.2/gitman/git.py
--rw-r--r--   0        0        0      241 2022-01-13 13:52:14.262983 gitman-3.5.2/gitman/hook-gitman.py
--rw-r--r--   0        0        0      127 2022-03-12 20:29:22.054396 gitman-3.5.2/gitman/models/__init__.py
--rw-r--r--   0        0        0    14926 2024-05-22 11:05:57.614107 gitman-3.5.2/gitman/models/config.py
--rw-r--r--   0        0        0      521 2020-11-18 21:15:23.000000 gitman-3.5.2/gitman/models/group.py
--rw-r--r--   0        0        0    11031 2024-04-27 19:07:19.093956 gitman-3.5.2/gitman/models/source.py
--rw-r--r--   0        0        0     3709 2024-04-27 03:29:24.222262 gitman-3.5.2/gitman/plugin.py
--rw-r--r--   0        0        0      740 2022-03-13 19:05:54.837062 gitman-3.5.2/gitman/settings.py
--rw-r--r--   0        0        0     4440 2024-04-27 19:52:07.998164 gitman-3.5.2/gitman/shell.py
--rw-r--r--   0        0        0       34 2017-01-09 13:05:30.000000 gitman-3.5.2/gitman/tests/__init__.py
--rw-r--r--   0        0        0      847 2024-04-27 22:35:16.562474 gitman-3.5.2/gitman/tests/conftest.py
--rw-r--r--   0        0        0      318 2021-06-02 20:53:11.405192 gitman-3.5.2/gitman/tests/files/gdm-custom.yml
--rw-r--r--   0        0        0      158 2018-11-20 14:52:53.000000 gitman-3.5.2/gitman/tests/files/gdm-default.yml
--rw-r--r--   0        0        0      755 2023-10-21 20:53:53.685344 gitman-3.5.2/gitman/tests/files/gitman.yml
--rw-r--r--   0        0        0      765 2023-01-25 17:38:54.328440 gitman-3.5.2/gitman/tests/files/subdir/gitman.yml
--rw-r--r--   0        0        0      778 2023-01-25 17:38:54.328826 gitman-3.5.2/gitman/tests/files/subdir/subsubdir/gitman.yml
--rw-r--r--   0        0        0      808 2023-01-25 17:38:54.329319 gitman-3.5.2/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml
--rw-r--r--   0        0        0    14500 2024-04-27 19:52:07.998606 gitman-3.5.2/gitman/tests/test_cli.py
--rw-r--r--   0        0        0     1118 2019-01-21 21:57:40.000000 gitman-3.5.2/gitman/tests/test_commands.py
--rw-r--r--   0        0        0     3047 2022-01-13 13:52:14.645994 gitman-3.5.2/gitman/tests/test_common.py
--rw-r--r--   0        0        0     9196 2024-04-27 19:52:07.998979 gitman-3.5.2/gitman/tests/test_git.py
--rw-r--r--   0        0        0     4807 2024-05-22 11:05:57.614993 gitman-3.5.2/gitman/tests/test_models_config.py
--rw-r--r--   0        0        0      263 2022-01-13 13:52:14.610271 gitman-3.5.2/gitman/tests/test_models_group.py
--rw-r--r--   0        0        0     5377 2024-04-27 19:52:07.999609 gitman-3.5.2/gitman/tests/test_models_source.py
--rw-r--r--   0        0        0     4329 2024-04-27 19:52:07.999994 gitman-3.5.2/gitman/tests/test_plugin.py
--rw-r--r--   0        0        0     3558 2024-04-27 19:52:08.000586 gitman-3.5.2/gitman/tests/test_shell.py
--rw-r--r--   0        0        0      344 2022-01-13 13:52:14.734256 gitman-3.5.2/gitman/tests/utils.py
--rw-r--r--   0        0        0     2542 2024-05-22 11:06:08.379184 gitman-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     5562 1970-01-01 00:00:00.000000 gitman-3.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-27 20:49:06.030198 gitman-3.5.2a1/LICENSE.md
+-rw-r--r--   0        0        0     4117 2024-05-19 22:26:57.861570 gitman-3.5.2a1/README.md
+-rw-r--r--   0        0        0      330 2024-04-27 20:49:06.036438 gitman-3.5.2a1/gitman/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-27 20:49:06.036505 gitman-3.5.2a1/gitman/__main__.py
+-rw-r--r--   0        0        0    10748 2024-04-27 20:49:06.036582 gitman-3.5.2a1/gitman/cli.py
+-rw-r--r--   0        0        0    11841 2024-05-20 22:57:47.526009 gitman-3.5.2a1/gitman/commands.py
+-rw-r--r--   0        0        0     5395 2024-04-27 20:49:06.036784 gitman-3.5.2a1/gitman/common.py
+-rw-r--r--   0        0        0      256 2024-04-27 20:49:06.036843 gitman-3.5.2a1/gitman/decorators.py
+-rw-r--r--   0        0        0      726 2024-04-27 20:49:06.036901 gitman-3.5.2a1/gitman/exceptions.py
+-rw-r--r--   0        0        0     8552 2024-04-27 20:49:06.036989 gitman-3.5.2a1/gitman/git.py
+-rw-r--r--   0        0        0      241 2024-04-27 20:49:06.037071 gitman-3.5.2a1/gitman/hook-gitman.py
+-rw-r--r--   0        0        0      127 2024-04-27 20:49:06.037159 gitman-3.5.2a1/gitman/models/__init__.py
+-rw-r--r--   0        0        0    14926 2024-05-20 22:57:47.526389 gitman-3.5.2a1/gitman/models/config.py
+-rw-r--r--   0        0        0      521 2024-04-27 20:49:06.037368 gitman-3.5.2a1/gitman/models/group.py
+-rw-r--r--   0        0        0    11031 2024-04-27 20:49:06.037440 gitman-3.5.2a1/gitman/models/source.py
+-rw-r--r--   0        0        0     3709 2024-04-27 20:49:06.037501 gitman-3.5.2a1/gitman/plugin.py
+-rw-r--r--   0        0        0      740 2024-04-27 20:49:06.037566 gitman-3.5.2a1/gitman/settings.py
+-rw-r--r--   0        0        0     4440 2024-04-27 20:49:06.037656 gitman-3.5.2a1/gitman/shell.py
+-rw-r--r--   0        0        0       34 2024-04-27 20:49:06.037747 gitman-3.5.2a1/gitman/tests/__init__.py
+-rw-r--r--   0        0        0      847 2024-04-28 21:36:16.641915 gitman-3.5.2a1/gitman/tests/conftest.py
+-rw-r--r--   0        0        0      318 2024-04-27 20:49:06.037910 gitman-3.5.2a1/gitman/tests/files/gdm-custom.yml
+-rw-r--r--   0        0        0      158 2024-04-27 20:49:06.037972 gitman-3.5.2a1/gitman/tests/files/gdm-default.yml
+-rw-r--r--   0        0        0      755 2024-04-27 20:49:06.038041 gitman-3.5.2a1/gitman/tests/files/gitman.yml
+-rw-r--r--   0        0        0      765 2024-04-27 20:49:06.038135 gitman-3.5.2a1/gitman/tests/files/subdir/gitman.yml
+-rw-r--r--   0        0        0      778 2024-04-27 20:49:06.038238 gitman-3.5.2a1/gitman/tests/files/subdir/subsubdir/gitman.yml
+-rw-r--r--   0        0        0      808 2024-04-27 20:49:06.038359 gitman-3.5.2a1/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml
+-rw-r--r--   0        0        0    14500 2024-04-27 20:49:06.038476 gitman-3.5.2a1/gitman/tests/test_cli.py
+-rw-r--r--   0        0        0     1118 2024-04-27 20:49:06.038551 gitman-3.5.2a1/gitman/tests/test_commands.py
+-rw-r--r--   0        0        0     3047 2024-04-27 20:49:06.038612 gitman-3.5.2a1/gitman/tests/test_common.py
+-rw-r--r--   0        0        0     9196 2024-04-27 20:49:06.038699 gitman-3.5.2a1/gitman/tests/test_git.py
+-rw-r--r--   0        0        0     4807 2024-05-20 22:57:47.526791 gitman-3.5.2a1/gitman/tests/test_models_config.py
+-rw-r--r--   0        0        0      263 2024-04-27 20:49:06.038854 gitman-3.5.2a1/gitman/tests/test_models_group.py
+-rw-r--r--   0        0        0     5377 2024-04-27 20:49:06.038951 gitman-3.5.2a1/gitman/tests/test_models_source.py
+-rw-r--r--   0        0        0     4329 2024-04-27 20:49:06.039031 gitman-3.5.2a1/gitman/tests/test_plugin.py
+-rw-r--r--   0        0        0     3558 2024-04-27 20:49:06.039093 gitman-3.5.2a1/gitman/tests/test_shell.py
+-rw-r--r--   0        0        0      344 2024-04-27 20:49:06.039150 gitman-3.5.2a1/gitman/tests/utils.py
+-rw-r--r--   0        0        0     2544 2024-05-20 22:58:43.973656 gitman-3.5.2a1/pyproject.toml
+-rw-r--r--   0        0        0     5564 1970-01-01 00:00:00.000000 gitman-3.5.2a1/PKG-INFO
```

### Comparing `gitman-3.5.2/LICENSE.md` & `gitman-3.5.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/README.md` & `gitman-3.5.2a1/README.md`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/__main__.py` & `gitman-3.5.2a1/gitman/__main__.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/cli.py` & `gitman-3.5.2a1/gitman/cli.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/commands.py` & `gitman-3.5.2a1/gitman/commands.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/common.py` & `gitman-3.5.2a1/gitman/common.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/exceptions.py` & `gitman-3.5.2a1/gitman/exceptions.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/git.py` & `gitman-3.5.2a1/gitman/git.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/models/config.py` & `gitman-3.5.2a1/gitman/models/config.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/models/group.py` & `gitman-3.5.2a1/gitman/models/group.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/models/source.py` & `gitman-3.5.2a1/gitman/models/source.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/plugin.py` & `gitman-3.5.2a1/gitman/plugin.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/settings.py` & `gitman-3.5.2a1/gitman/settings.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/shell.py` & `gitman-3.5.2a1/gitman/shell.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/conftest.py` & `gitman-3.5.2a1/gitman/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/files/gitman.yml` & `gitman-3.5.2a1/gitman/tests/files/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/files/subdir/gitman.yml` & `gitman-3.5.2a1/gitman/tests/files/subdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/files/subdir/subsubdir/gitman.yml` & `gitman-3.5.2a1/gitman/tests/files/subdir/subsubdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml` & `gitman-3.5.2a1/gitman/tests/files/subdir/subsubdir/skip/subsubsubsubdir/gitman.yml`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_cli.py` & `gitman-3.5.2a1/gitman/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_commands.py` & `gitman-3.5.2a1/gitman/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_common.py` & `gitman-3.5.2a1/gitman/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_git.py` & `gitman-3.5.2a1/gitman/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_models_config.py` & `gitman-3.5.2a1/gitman/tests/test_models_config.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_models_source.py` & `gitman-3.5.2a1/gitman/tests/test_models_source.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_plugin.py` & `gitman-3.5.2a1/gitman/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/gitman/tests/test_shell.py` & `gitman-3.5.2a1/gitman/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `gitman-3.5.2/pyproject.toml` & `gitman-3.5.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "gitman"
-version = "3.5.2"
+version = "3.5.2a1"
 description = "A language-agnostic dependency manager using Git."
 
 license = "MIT"
 
 authors = ["Jace Browning <jacebrowning@gmail.com>"]
 
 readme = "README.md"
```

### Comparing `gitman-3.5.2/PKG-INFO` & `gitman-3.5.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitman
-Version: 3.5.2
+Version: 3.5.2a1
 Summary: A language-agnostic dependency manager using Git.
 Home-page: https://pypi.org/project/gitman
 License: MIT
 Keywords: git,version control,build systems,dependency management,submodules
 Author: Jace Browning
 Author-email: jacebrowning@gmail.com
 Requires-Python: >=3.8,<4.0
```

