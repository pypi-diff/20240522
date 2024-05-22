# Comparing `tmp/saritasa_invocations-1.1.0.tar.gz` & `tmp/saritasa_invocations-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saritasa_invocations-1.1.0.tar", max compression
+gzip compressed data, was "saritasa_invocations-1.1.1.tar", max compression
```

## Comparing `saritasa_invocations-1.1.0.tar` & `saritasa_invocations-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1092 2023-07-13 03:53:10.395007 saritasa_invocations-1.1.0/LICENSE
--rw-r--r--   0        0        0    25714 2024-03-04 04:41:25.345285 saritasa_invocations-1.1.0/README.md
--rw-r--r--   0        0        0     4630 2024-03-04 04:44:56.588271 saritasa_invocations-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1604 2023-12-04 04:13:49.862456 saritasa_invocations-1.1.0/saritasa_invocations/__init__.py
--rw-r--r--   0        0        0    12146 2023-11-29 10:30:30.636258 saritasa_invocations-1.1.0/saritasa_invocations/_config.py
--rw-r--r--   0        0        0     8100 2023-11-09 06:17:01.288409 saritasa_invocations-1.1.0/saritasa_invocations/alembic.py
--rw-r--r--   0        0        0     1026 2023-11-09 08:01:13.807701 saritasa_invocations-1.1.0/saritasa_invocations/celery.py
--rw-r--r--   0        0        0     1884 2023-09-01 09:33:39.049709 saritasa_invocations-1.1.0/saritasa_invocations/cruft.py
--rw-r--r--   0        0        0     1736 2023-09-04 04:29:03.365894 saritasa_invocations-1.1.0/saritasa_invocations/db.py
--rw-r--r--   0        0        0     3266 2023-09-19 08:41:36.770357 saritasa_invocations-1.1.0/saritasa_invocations/db_k8s.py
--rw-r--r--   0        0        0     9804 2023-11-29 10:30:30.636258 saritasa_invocations-1.1.0/saritasa_invocations/django.py
--rw-r--r--   0        0        0     5479 2023-09-18 04:31:01.313542 saritasa_invocations-1.1.0/saritasa_invocations/docker.py
--rw-r--r--   0        0        0      748 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.0/saritasa_invocations/fastapi.py
--rw-r--r--   0        0        0    10133 2024-03-04 04:43:57.862329 saritasa_invocations-1.1.0/saritasa_invocations/git.py
--rw-r--r--   0        0        0      497 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.0/saritasa_invocations/github_actions.py
--rw-r--r--   0        0        0     8303 2023-11-09 06:11:49.930062 saritasa_invocations-1.1.0/saritasa_invocations/k8s.py
--rw-r--r--   0        0        0      386 2023-09-12 10:09:13.359744 saritasa_invocations-1.1.0/saritasa_invocations/mypy.py
--rw-r--r--   0        0        0      457 2023-07-25 09:59:23.448672 saritasa_invocations-1.1.0/saritasa_invocations/open_api.py
--rw-r--r--   0        0        0     1773 2024-03-04 04:41:25.345285 saritasa_invocations-1.1.0/saritasa_invocations/pip.py
--rw-r--r--   0        0        0     2037 2023-11-29 10:30:30.636258 saritasa_invocations-1.1.0/saritasa_invocations/poetry.py
--rw-r--r--   0        0        0      820 2023-11-27 04:05:58.043712 saritasa_invocations-1.1.0/saritasa_invocations/pre_commit.py
--rw-r--r--   0        0        0     1059 2023-08-29 05:21:38.726347 saritasa_invocations-1.1.0/saritasa_invocations/printing.py
--rw-r--r--   0        0        0        0 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.0/saritasa_invocations/py.typed
--rw-r--r--   0        0        0      388 2023-09-12 10:09:13.359744 saritasa_invocations-1.1.0/saritasa_invocations/pytest.py
--rw-r--r--   0        0        0     2696 2023-09-18 04:31:01.313542 saritasa_invocations-1.1.0/saritasa_invocations/python.py
--rw-r--r--   0        0        0     1375 2023-11-09 06:11:49.930062 saritasa_invocations-1.1.0/saritasa_invocations/secrets.py
--rw-r--r--   0        0        0     1701 2023-10-27 09:38:41.428085 saritasa_invocations-1.1.0/saritasa_invocations/system.py
--rw-r--r--   0        0        0    26908 1970-01-01 00:00:00.000000 saritasa_invocations-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-07-13 03:53:10.395007 saritasa_invocations-1.1.1/LICENSE
+-rw-r--r--   0        0        0    25714 2024-03-04 04:41:25.345285 saritasa_invocations-1.1.1/README.md
+-rw-r--r--   0        0        0     4632 2024-05-22 01:41:28.836160 saritasa_invocations-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1604 2023-12-04 04:13:49.862456 saritasa_invocations-1.1.1/saritasa_invocations/__init__.py
+-rw-r--r--   0        0        0    12147 2024-05-22 01:22:37.845527 saritasa_invocations-1.1.1/saritasa_invocations/_config.py
+-rw-r--r--   0        0        0     8100 2023-11-09 06:17:01.288409 saritasa_invocations-1.1.1/saritasa_invocations/alembic.py
+-rw-r--r--   0        0        0     1026 2023-11-09 08:01:13.807701 saritasa_invocations-1.1.1/saritasa_invocations/celery.py
+-rw-r--r--   0        0        0     1884 2023-09-01 09:33:39.049709 saritasa_invocations-1.1.1/saritasa_invocations/cruft.py
+-rw-r--r--   0        0        0     1736 2023-09-04 04:29:03.365894 saritasa_invocations-1.1.1/saritasa_invocations/db.py
+-rw-r--r--   0        0        0     3266 2023-09-19 08:41:36.770357 saritasa_invocations-1.1.1/saritasa_invocations/db_k8s.py
+-rw-r--r--   0        0        0     9804 2023-11-29 10:30:30.636258 saritasa_invocations-1.1.1/saritasa_invocations/django.py
+-rw-r--r--   0        0        0     5479 2023-09-18 04:31:01.313542 saritasa_invocations-1.1.1/saritasa_invocations/docker.py
+-rw-r--r--   0        0        0      748 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.1/saritasa_invocations/fastapi.py
+-rw-r--r--   0        0        0    10133 2024-03-04 04:43:57.862329 saritasa_invocations-1.1.1/saritasa_invocations/git.py
+-rw-r--r--   0        0        0      497 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.1/saritasa_invocations/github_actions.py
+-rw-r--r--   0        0        0     8303 2023-11-09 06:11:49.930062 saritasa_invocations-1.1.1/saritasa_invocations/k8s.py
+-rw-r--r--   0        0        0      386 2023-09-12 10:09:13.359744 saritasa_invocations-1.1.1/saritasa_invocations/mypy.py
+-rw-r--r--   0        0        0      457 2023-07-25 09:59:23.448672 saritasa_invocations-1.1.1/saritasa_invocations/open_api.py
+-rw-r--r--   0        0        0     1773 2024-03-04 04:41:25.345285 saritasa_invocations-1.1.1/saritasa_invocations/pip.py
+-rw-r--r--   0        0        0     2037 2023-11-29 10:30:30.636258 saritasa_invocations-1.1.1/saritasa_invocations/poetry.py
+-rw-r--r--   0        0        0      820 2023-11-27 04:05:58.043712 saritasa_invocations-1.1.1/saritasa_invocations/pre_commit.py
+-rw-r--r--   0        0        0     1059 2023-08-29 05:21:38.726347 saritasa_invocations-1.1.1/saritasa_invocations/printing.py
+-rw-r--r--   0        0        0        0 2023-08-28 06:35:31.518887 saritasa_invocations-1.1.1/saritasa_invocations/py.typed
+-rw-r--r--   0        0        0      388 2023-09-12 10:09:13.359744 saritasa_invocations-1.1.1/saritasa_invocations/pytest.py
+-rw-r--r--   0        0        0     2696 2023-09-18 04:31:01.313542 saritasa_invocations-1.1.1/saritasa_invocations/python.py
+-rw-r--r--   0        0        0     1375 2023-11-09 06:11:49.930062 saritasa_invocations-1.1.1/saritasa_invocations/secrets.py
+-rw-r--r--   0        0        0     1701 2023-10-27 09:38:41.428085 saritasa_invocations-1.1.1/saritasa_invocations/system.py
+-rw-r--r--   0        0        0    26908 1970-01-01 00:00:00.000000 saritasa_invocations-1.1.1/PKG-INFO
```

### Comparing `saritasa_invocations-1.1.0/LICENSE` & `saritasa_invocations-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/README.md` & `saritasa_invocations-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/pyproject.toml` & `saritasa_invocations-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saritasa-invocations"
-version = "1.1.0"
+version = "1.1.1"
 description = "Collection of invoke commands used by Saritasa"
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 maintainers = [
     "Stanislav Khlud <stanislav.khlud@saritasa.com>",
 ]
@@ -48,27 +48,27 @@
 
 [tool.poetry.extras]
 env_settings = ["python-decouple"]
 
 [tool.poetry.group.dev.dependencies]
 # Improved REPL
 ipdb = "^0.13.13"
-ipython = "^8.22.1"
+ipython = "^8.24.0"
 # A framework for managing and maintaining multi-language pre-commit hooks.
 # https://pre-commit.com/
-pre-commit = "^3.6.2"
+pre-commit = "^3.7.1"
 
 [tool.poetry.group.linters.dependencies]
 # Flake dependencies are added so that VSCode extension for flake8
 # would work properly
 # https://marketplace.visualstudio.com/items?itemName=ms-python.flake8&ssr=false#overview
 flake8 = "^7.0.0"
 # A plugin for Flake8 finding likely bugs and design problems in your program.
 # https://github.com/PyCQA/flake8-bugbear
-flake8-bugbear = "^24.2.6"
+flake8-bugbear = "^24.4.26"
 # A flake8 plugin that warn about backslashes usage.
 # https://github.com/wemake-services/flake8-broken-line
 flake8-broken-line = "^1.0.0"
 # A simple module that adds an extension for the fantastic pydocstyle tool to flake8.
 # https://github.com/PyCQA/flake8-docstrings
 flake8-docstrings = "^1.7.0"
 # A flake8 plugin loading the configuration from pyproject.toml
@@ -79,15 +79,15 @@
 flake8-modern-annotations = "^1.6.0"
 # McCabe complexity checker.
 # https://github.com/PyCQA/mccabe
 mccabe = "^0.7.0"
 
 # Mypy is a static type checker for Python.
 # https://mypy.readthedocs.io/en/stable/
-mypy = "^1.8.0"
+mypy = "^1.10.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/__init__.py` & `saritasa_invocations-1.1.1/saritasa_invocations/__init__.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/_config.py` & `saritasa_invocations-1.1.1/saritasa_invocations/_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
     component_selector: str = "app.kubernetes.io/component"
     get_pod_name_command: str = (
         "kubectl get pods "
         "--selector {component_selector}={component} "
         "--no-headers --output jsonpath='{{.items[0].metadata.name}}'"
     )
     default_component: str = "backend"
-    default_entry: str = "cnb/lifecycle/launcher bash"
+    default_entry: str = "/cnb/lifecycle/launcher bash"
     python_shell: str = "shell_plus"
     health_check: str = "health_check"
     secret_file_path_in_pod: str | None = None
     temp_secret_file_path: str = ".env.to_delete"
     env_color: str = "cyan"
```

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/alembic.py` & `saritasa_invocations-1.1.1/saritasa_invocations/alembic.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/celery.py` & `saritasa_invocations-1.1.1/saritasa_invocations/celery.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/cruft.py` & `saritasa_invocations-1.1.1/saritasa_invocations/cruft.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/db.py` & `saritasa_invocations-1.1.1/saritasa_invocations/db.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/db_k8s.py` & `saritasa_invocations-1.1.1/saritasa_invocations/db_k8s.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/django.py` & `saritasa_invocations-1.1.1/saritasa_invocations/django.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/docker.py` & `saritasa_invocations-1.1.1/saritasa_invocations/docker.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/fastapi.py` & `saritasa_invocations-1.1.1/saritasa_invocations/fastapi.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/git.py` & `saritasa_invocations-1.1.1/saritasa_invocations/git.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/k8s.py` & `saritasa_invocations-1.1.1/saritasa_invocations/k8s.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/pip.py` & `saritasa_invocations-1.1.1/saritasa_invocations/pip.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/poetry.py` & `saritasa_invocations-1.1.1/saritasa_invocations/poetry.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/pre_commit.py` & `saritasa_invocations-1.1.1/saritasa_invocations/pre_commit.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/printing.py` & `saritasa_invocations-1.1.1/saritasa_invocations/printing.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/python.py` & `saritasa_invocations-1.1.1/saritasa_invocations/python.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/secrets.py` & `saritasa_invocations-1.1.1/saritasa_invocations/secrets.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/saritasa_invocations/system.py` & `saritasa_invocations-1.1.1/saritasa_invocations/system.py`

 * *Files identical despite different names*

### Comparing `saritasa_invocations-1.1.0/PKG-INFO` & `saritasa_invocations-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saritasa-invocations
-Version: 1.1.0
+Version: 1.1.1
 Summary: Collection of invoke commands used by Saritasa
 Home-page: https://pypi.org/project/saritasa-invocations/
 License: MIT
 Keywords: python,invoke
 Author: Saritasa
 Author-email: pypi@saritasa.com
 Maintainer: Stanislav Khlud
```

