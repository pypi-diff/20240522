# Comparing `tmp/deps-manager-1.0.8.tar.gz` & `tmp/deps-manager-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deps-manager-1.0.8.tar", last modified: Mon May 20 04:51:04 2024, max compression
+gzip compressed data, was "deps-manager-1.0.9.tar", last modified: Mon May 20 04:55:30 2024, max compression
```

## Comparing `deps-manager-1.0.8.tar` & `deps-manager-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:51:04.811638 deps-manager-1.0.8/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:51:04.811359 deps-manager-1.0.8/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.8/README.md
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:51:04.809004 deps-manager-1.0.8/deps_manager/
--rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.8/deps_manager/__init__.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     8059 2024-05-20 04:50:16.000000 deps-manager-1.0.8/deps_manager/dependencies.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)     3947 2024-05-20 04:50:53.000000 deps-manager-1.0.8/deps_manager/main.py
--rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.8/deps_manager/utils.py
-drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:51:04.810650 deps-manager-1.0.8/deps_manager.egg-info/
--rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/PKG-INFO
--rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/SOURCES.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/dependency_links.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/entry_points.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/requires.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 04:51:04.000000 deps-manager-1.0.8/deps_manager.egg-info/top_level.txt
--rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 04:51:04.811693 deps-manager-1.0.8/setup.cfg
--rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 04:51:03.000000 deps-manager-1.0.8/setup.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:55:30.995218 deps-manager-1.0.9/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:55:30.994997 deps-manager-1.0.9/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     2347 2024-04-06 05:24:23.000000 deps-manager-1.0.9/README.md
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:55:30.993132 deps-manager-1.0.9/deps_manager/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        0 2024-04-06 02:20:53.000000 deps-manager-1.0.9/deps_manager/__init__.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     8059 2024-05-20 04:50:16.000000 deps-manager-1.0.9/deps_manager/dependencies.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)     4139 2024-05-20 04:54:57.000000 deps-manager-1.0.9/deps_manager/main.py
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      405 2024-04-06 02:20:53.000000 deps-manager-1.0.9/deps_manager/utils.py
+drwxr-xr-x   0 harshadatupe   (501) staff       (20)        0 2024-05-20 04:55:30.994680 deps-manager-1.0.9/deps_manager.egg-info/
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      320 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/PKG-INFO
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      333 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)        1 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       55 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/entry_points.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       20 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/requires.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       13 2024-05-20 04:55:30.000000 deps-manager-1.0.9/deps_manager.egg-info/top_level.txt
+-rw-r--r--   0 harshadatupe   (501) staff       (20)       38 2024-05-20 04:55:30.995264 deps-manager-1.0.9/setup.cfg
+-rw-r--r--   0 harshadatupe   (501) staff       (20)      570 2024-05-20 04:55:29.000000 deps-manager-1.0.9/setup.py
```

### Comparing `deps-manager-1.0.8/README.md` & `deps-manager-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.8/deps_manager/dependencies.py` & `deps-manager-1.0.9/deps_manager/dependencies.py`

 * *Files identical despite different names*

### Comparing `deps-manager-1.0.8/deps_manager/main.py` & `deps-manager-1.0.9/deps_manager/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,17 +90,20 @@
 def remove_unused(venv_path, source_code_full_path):
     """Remove unused dependencies.
     - Currently this feature is supported for python projects only.
     """
     remove_unused_dependencies(venv_path, source_code_full_path)
 
 @cli.command()
-@requirements_option
+@click.option('-r', '--requirements_file',
+              prompt="Enter the relative path to the requirements.txt file",
+              required=True,
+              help="Path to requirements file")
 @click.option('-td', '--tests_dir', required=True,
-              prompt="Enter the tests directory name of the project",
+              prompt="Enter the relative path to the tests directory of the project",
               help="Name of the directory containing the project's tests")
 def containerize_and_test(requirements_file, tests_dir):
     """
     Containerize and run the tests.
 
     Before running, ensure the following requirements are met:
     - Only applicable to Python projects.
```

### Comparing `deps-manager-1.0.8/setup.py` & `deps-manager-1.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='deps-manager',
-    version='1.0.8',
+    version='1.0.9',
     author="Harshada Tupe",
     author_email="harshadatupe8@gmail.com",
     license="MIT",
     packages=find_packages(),
     classifiers=["Programming Language :: Python :: 3 :: Only",
                  "Operating System :: OS Independent"],
     python_requires='>=3.8',
```

