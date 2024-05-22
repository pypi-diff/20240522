# Comparing `tmp/logikal-utils-1.0.1.tar.gz` & `tmp/logikal_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logikal-utils-1.0.1.tar", last modified: Fri Jan 26 20:20:31 2024, max compression
+gzip compressed data, was "logikal_utils-1.1.0.tar", last modified: Wed May 22 09:20:56 2024, max compression
```

## Comparing `logikal-utils-1.0.1.tar` & `logikal_utils-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/logikal_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/logikal_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/logikal_utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/logikal_utils/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/logikal_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/logikal_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-01-26 20:20:31.000000 logikal-utils-1.0.1/logikal_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-26 20:20:31.000000 logikal-utils-1.0.1/logikal_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 20:20:31.000000 logikal-utils-1.0.1/logikal_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-26 20:20:31.000000 logikal-utils-1.0.1/logikal_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-26 20:20:31.000000 logikal-utils-1.0.1/logikal_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-26 20:20:14.000000 logikal-utils-1.0.1/requirements/extras/docker.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 20:20:31.354927 logikal-utils-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/logikal_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/logikal_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/extras/docker.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/setup.cfg
```

### Comparing `logikal-utils-1.0.1/.copier-answers.yml` & `logikal_utils-1.1.0/.copier-answers.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is an answers file generated by Copier.
 ##
 ###################################################################################################
-_commit: v1.0.2
+_commit: v1.0.4
 _src_path: git@github.com:logikal-io/python-package-template.git
 audience: Developers
 classifiers:
 - 'Topic :: Software Development'
 cloud: false
 description: Common Python utilities used at Logikal
 extras:
@@ -17,8 +17,7 @@
 keywords:
 - python
 - utilities
 license: mit
 name: logikal-utils
 scripts: []
 title: logikal-utils
-
```

### Comparing `logikal-utils-1.0.1/LICENSE.txt` & `logikal_utils-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logikal-utils-1.0.1/PKG-INFO` & `logikal_utils-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logikal-utils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Common Python utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -36,14 +36,16 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: termcolor~=2.4
 Requires-Dist: tomli~=2.0
 Provides-Extra: docker
 Requires-Dist: docker~=7.0; extra == "docker"
+Requires-Dist: requests<2.32; extra == "docker"
+Requires-Dist: types-requests<2.32; extra == "docker"
 
 logikal-utils
 =============
 Common Python utilities used at Logikal.
 
 Getting Started
 ---------------
```

### Comparing `logikal-utils-1.0.1/logikal_utils/docker.py` & `logikal_utils-1.1.0/logikal_utils/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import subprocess
+from pathlib import Path
 from time import sleep, time
 from typing import Optional
 
 from docker import DockerClient, from_env as client_from_env
 from docker.models.containers import Container
 from termcolor import colored
 
@@ -18,15 +19,16 @@
         start_timeout_seconds: float = 30,
         ready_log_text: Optional[str] = None,
         log_poll_seconds: float = 3,
     ):
         """
         Manage a project's Docker Compose services.
 
-        .. note:: Automatically starts all services during initialization whenever necessary.
+        .. note:: Automatically starts all services during initialization whenever necessary based
+            on the ``compose.yml`` or ``compose/local.yml`` file.
         .. note:: Requires the :ref:`docker extra <index:Docker>`.
 
         Args:
             name: The name of the service to manage.
             project: The name of the project to use.
             start_timeout_seconds: The time to wait for services to start.
             ready_log_text: The log text that signals that the service is ready.
@@ -49,16 +51,23 @@
         return f'Docker Compose project "{self.project}" service "{self.name}"'
 
     def start_services(self) -> None:
         """
         Start all Docker Compose services in the given project.
         """
         print(colored('Starting Docker Compose services', 'yellow', attrs=['bold']))
+        for compose_file in [Path('compose.yml'), Path('compose/local.yml')]:
+            if compose_file.exists():
+                print(f'Using {compose_file}')
+                break
+        else:
+            raise RuntimeError('Compose file not found')
+
         command = [
-            'docker', 'compose', 'up', '--detach',
+            'docker', 'compose', '--file', str(compose_file), 'up', '--detach',
             *(['--quiet-pull'] if 'GITHUB_ACTIONS' in os.environ else []),
             '--wait', '--wait-timeout', str(self.start_timeout_seconds),
         ]
         subprocess.run(command, text=True, check=True)  # nosec: secure, not using untrusted input
         print()
 
     def _running_container(self, client: DockerClient, start_services: bool) -> Container:
```

### Comparing `logikal-utils-1.0.1/logikal_utils.egg-info/PKG-INFO` & `logikal_utils-1.1.0/logikal_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logikal-utils
-Version: 1.0.1
+Version: 1.1.0
 Summary: Common Python utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -36,14 +36,16 @@
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: termcolor~=2.4
 Requires-Dist: tomli~=2.0
 Provides-Extra: docker
 Requires-Dist: docker~=7.0; extra == "docker"
+Requires-Dist: requests<2.32; extra == "docker"
+Requires-Dist: types-requests<2.32; extra == "docker"
 
 logikal-utils
 =============
 Common Python utilities used at Logikal.
 
 Getting Started
 ---------------
```

### Comparing `logikal-utils-1.0.1/logikal_utils.egg-info/SOURCES.txt` & `logikal_utils-1.1.0/logikal_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logikal-utils-1.0.1/pyproject.toml` & `logikal_utils-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logikal-utils-1.0.1/requirements/build.txt.lock` & `logikal_utils-1.1.0/requirements/build.txt.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 5cb1a368e35962412e4230ef67a622b3ed950d02d59c40d132b27e3a685ef8f8
+##  Requirements hash: 8706de2163a25299dbe1d5d6f26df03b6aaaad435e67227452ee6c0b2b97aea0
 ##
 ###################################################################################################
-build==1.0.3
-certifi==2023.11.17
+backports.tarfile==1.1.1
+build==1.2.1
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
-cryptography==42.0.1
+cryptography==42.0.7
 docutils==0.20.1
-idna==3.6
-importlib-metadata==7.0.1
-importlib-resources==6.1.1
-jaraco.classes==3.3.0
+idna==3.7
+importlib_metadata==7.1.0
+importlib_resources==6.4.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-keyring==24.3.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
 more-itertools==10.2.0
-nh3==0.2.15
-packaging==23.2
-pip==23.3.2
-pkginfo==1.9.6
-pycparser==2.21
-Pygments==2.17.2
-pyproject_hooks==1.0.0
-readme-renderer==42.0
-requests==2.31.0
+nh3==0.2.17
+packaging==24.0
+pip==24.0
+pkginfo==1.10.0
+pycparser==2.22
+Pygments==2.18.0
+pyproject_hooks==1.1.0
+readme_renderer==43.0
+requests==2.32.2
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
+rich==13.7.1
 SecretStorage==3.3.3
-setuptools==69.0.3
+setuptools==70.0.0
 tomli==2.0.1
-twine==4.0.2
-typing_extensions==4.9.0
-urllib3==2.1.0
-wheel==0.42.0
-zipp==3.17.0
+twine==5.1.0
+typing_extensions==4.11.0
+urllib3==2.2.1
+wheel==0.43.0
+zipp==3.18.2
```

### Comparing `logikal-utils-1.0.1/requirements/dev.txt.lock` & `logikal_utils-1.1.0/requirements/dev.txt.lock`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,102 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 677b927d1157df20456fdf2eb36e33caa6b9370ded51fd5624f9699bdba961bc
+##  Requirements hash: f7da736a3e836f66831f6d8f08bc5e5e69f04ad41877fcb30b62bd52008a53ce
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
-astroid==3.0.2
+astroid==3.2.2
 attrs==23.2.0
-Babel==2.14.0
-bandit==1.7.7
-build==1.0.3
-certifi==2023.11.17
+Babel==2.15.0
+backports.tarfile==1.1.1
+bandit==1.7.8
+build==1.2.1
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 colorama==0.4.6
-coverage==7.4.0
-cryptography==42.0.1
-dill==0.3.7
+coverage==7.5.1
+cryptography==42.0.7
+dill==0.3.8
 docker==7.0.0
 docutils==0.20.1
-exceptiongroup==1.2.0
-execnet==2.0.2
-filelock==3.13.1
-idna==3.6
+exceptiongroup==1.2.1
+execnet==2.1.1
+filelock==3.14.0
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
-importlib-resources==6.1.1
+importlib_metadata==7.1.0
+importlib_resources==6.4.0
 iniconfig==2.0.0
 isort==5.13.2
-jaraco.classes==3.3.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-Jinja2==3.1.3
-keyring==24.3.0
+Jinja2==3.1.4
+keyring==25.2.1
 logikal-docs==1.1.4
 markdown-it-py==3.0.0
-MarkupSafe==2.1.4
+MarkupSafe==2.1.5
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==10.2.0
-mypy==1.8.0
+mypy==1.10.0
 mypy-extensions==1.0.0
-nh3==0.2.15
+nh3==0.2.17
 packaging==23.2
 pbr==6.0.0
-pillow==10.2.0
-pip==23.3.2
-pip-licenses==4.3.4
-pkginfo==1.9.6
-platformdirs==4.1.0
-pluggy==1.3.0
-prettytable==3.9.0
+pillow==10.3.0
+pip==24.0
+pip-licenses==4.4.0
+pkginfo==1.10.0
+platformdirs==4.2.2
+pluggy==1.5.0
+prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
-pycparser==2.21
+pycparser==2.22
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.0.3
+Pygments==2.18.0
+pylint==3.2.0
 pyorbs==2.1.0
-pyproject_hooks==1.0.0
-pytest==7.4.4
-pytest-cov==4.1.0
-pytest-logikal==2.0.1
-pytest-mock==3.12.0
+pyproject_hooks==1.1.0
+pytest==8.2.0
+pytest-cov==5.0.0
+pytest-logikal==3.0.0
+pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
-pytz==2023.3.post1
+pytest-xdist==3.6.1
+pytz==2024.1
 PyYAML==6.0.1
-readme-renderer==42.0
+readme_renderer==43.0
 requests==2.31.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
+rich==13.7.1
 SecretStorage==3.3.3
-setuptools==69.0.3
+setuptools==70.0.0
 snowballstemmer==2.2.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-stevedore==5.1.0
+stevedore==5.2.0
 termcolor==2.4.0
 tomli==2.0.1
-tomlkit==0.12.3
-twine==4.0.2
-typing_extensions==4.9.0
-urllib3==2.1.0
+tomlkit==0.12.5
+twine==5.1.0
+types-requests==2.31.0.20240406
+typing_extensions==4.11.0
+urllib3==2.2.1
 wcwidth==0.2.13
-wheel==0.42.0
-zipp==3.17.0
+wheel==0.43.0
+zipp==3.18.2
```

### Comparing `logikal-utils-1.0.1/requirements/docs.txt.lock` & `logikal_utils-1.1.0/requirements/docs.txt.lock`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 5383d4de9e386be60a001d6967c706d8076b5a292f2eb756591d4771f1fd747c
+##  Requirements hash: c6bcc16e1beca628be6ad4cccd1e490a8d027c814b421c05364e0e7fc7ef0ae4
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
-Babel==2.14.0
-certifi==2023.11.17
+Babel==2.15.0
+certifi==2024.2.2
 charset-normalizer==3.3.2
 docker==7.0.0
 docutils==0.20.1
-idna==3.6
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
-Jinja2==3.1.3
+importlib_metadata==7.1.0
+Jinja2==3.1.4
 logikal-docs==1.1.4
-MarkupSafe==2.1.4
+MarkupSafe==2.1.5
 packaging==23.2
-pip==23.3.2
-Pygments==2.17.2
-pytz==2023.3.post1
+pip==24.0
+Pygments==2.18.0
+pytz==2024.1
 requests==2.31.0
-setuptools==69.0.3
+setuptools==70.0.0
 snowballstemmer==2.2.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 termcolor==2.4.0
 tomli==2.0.1
-urllib3==2.1.0
-wheel==0.42.0
-zipp==3.17.0
+types-requests==2.31.0.20240406
+urllib3==2.2.1
+wheel==0.43.0
+zipp==3.18.2
```

