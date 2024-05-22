# Comparing `tmp/dyff_storage-0.7.4.tar.gz` & `tmp/dyff_storage-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff_storage-0.7.4.tar", last modified: Fri May 10 23:19:02 2024, max compression
+gzip compressed data, was "dyff_storage-0.7.5.tar", last modified: Wed May 22 19:18:50 2024, max compression
```

## Comparing `dyff_storage-0.7.4.tar` & `dyff_storage-0.7.5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.465409 dyff_storage-0.7.4/
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1706 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/.secrets.baseline
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 23:19:02.464409 dyff_storage-0.7.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.452409 dyff_storage-0.7.4/dyff/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.458409 dyff_storage-0.7.4/dyff/storage/
--rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.458409 dyff_storage-0.7.4/dyff/storage/backend/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.459409 dyff_storage-0.7.4/dyff/storage/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.460409 dyff_storage-0.7.4/dyff/storage/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.460409 dyff_storage-0.7.4/dyff/storage/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.461409 dyff_storage-0.7.4/dyff/storage/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.462409 dyff_storage-0.7.4/dyff/storage/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.462409 dyff_storage-0.7.4/dyff/storage/backend/s3/
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15072 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/backend/s3/storage.py
--rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/config.py
--rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/dynamic_import.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/dyff/storage/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.464409 dyff_storage-0.7.4/dyff_storage.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3477 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-05-10 23:19:02.000000 dyff_storage-0.7.4/dyff_storage.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/makefile
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-10 23:19:02.465409 dyff_storage-0.7.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-10 23:19:02.463409 dyff_storage-0.7.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-10 23:18:56.000000 dyff_storage-0.7.4/tests/test_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.651763 dyff_storage-0.7.5/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      520 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        7 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/.secrets.baseline
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       51 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-22 19:18:50.651763 dyff_storage-0.7.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.638763 dyff_storage-0.7.5/dyff/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.644763 dyff_storage-0.7.5/dyff/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     2937 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.645763 dyff_storage-0.7.5/dyff/storage/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.646763 dyff_storage-0.7.5/dyff/storage/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3220 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     6196 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)    13398 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.646763 dyff_storage-0.7.5/dyff/storage/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6656 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.647763 dyff_storage-0.7.5/dyff/storage/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9209 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.647763 dyff_storage-0.7.5/dyff/storage/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.648763 dyff_storage-0.7.5/dyff/storage/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    23188 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.649763 dyff_storage-0.7.5/dyff/storage/backend/s3/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15737 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/backend/s3/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)    10386 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      485 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/dynamic_import.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/dyff/storage/typing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.650763 dyff_storage-0.7.5/dyff_storage.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3477 2024-05-22 19:18:50.000000 dyff_storage-0.7.5/dyff_storage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-05-22 19:18:50.000000 dyff_storage-0.7.5/dyff_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 19:18:50.000000 dyff_storage-0.7.5/dyff_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2024-05-22 19:18:50.000000 dyff_storage-0.7.5/dyff_storage.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-05-22 19:18:50.000000 dyff_storage-0.7.5/dyff_storage.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 19:18:50.651763 dyff_storage-0.7.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 19:18:50.650763 dyff_storage-0.7.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1194 2024-05-22 19:18:44.000000 dyff_storage-0.7.5/tests/test_import.py
```

### Comparing `dyff_storage-0.7.4/.gitignore` & `dyff_storage-0.7.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/.gitlab-ci.yml` & `dyff_storage-0.7.5/.gitlab-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     file:
       - detect-secrets.yml
   - project: buildgarden/pipelines/prettier
     ref: 0.3.2
     file:
       - prettier.yml
   - project: buildgarden/pipelines/python
-    ref: 0.9.1
+    ref: 0.12.0
     file:
       - python-autoflake.yml
       - python-isort.yml
       - python-black.yml
       - python-pytest.yml
       - python-pyroma.yml
       - python-build-sdist.yml
```

### Comparing `dyff_storage-0.7.4/.licenserc.yaml` & `dyff_storage-0.7.5/.licenserc.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/.pre-commit-config.yaml` & `dyff_storage-0.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/.secrets.baseline` & `dyff_storage-0.7.5/.secrets.baseline`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/CODE_OF_CONDUCT.md` & `dyff_storage-0.7.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/LICENSE` & `dyff_storage-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/PKG-INFO` & `dyff_storage-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.4/README.md` & `dyff_storage-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/__init__.py` & `dyff_storage-0.7.5/dyff/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/base/auth.py` & `dyff_storage-0.7.5/dyff/storage/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/base/command.py` & `dyff_storage-0.7.5/dyff/storage/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/base/query.py` & `dyff_storage-0.7.5/dyff/storage/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/base/storage.py` & `dyff_storage-0.7.5/dyff/storage/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/gcloud/storage.py` & `dyff_storage-0.7.5/dyff/storage/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/kafka/command.py` & `dyff_storage-0.7.5/dyff/storage/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/mock/command.py` & `dyff_storage-0.7.5/dyff/storage/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/mongodb/auth.py` & `dyff_storage-0.7.5/dyff/storage/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/mongodb/query.py` & `dyff_storage-0.7.5/dyff/storage/backend/mongodb/query.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/backend/s3/storage.py` & `dyff_storage-0.7.5/dyff/storage/backend/s3/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2024 UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 from __future__ import annotations
 
+import functools
 import hashlib
 import io
 
 # mypy: disable-error-code="import-untyped"
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import BinaryIO, Iterable, Optional, Tuple
@@ -162,33 +163,50 @@
         endpoint=parsed_endpoint.netloc,
         access_key=config.storage.s3.access_key,
         secret_key=config.storage.s3.secret_key.get_secret_value(),
         secure=secure,
     )
 
 
+def _translate_errors(fn):
+    @functools.wraps(fn)
+    def _impl(*args, **kwargs):
+        try:
+            fn(*args, **kwargs)
+        except Exception as ex:
+            if isinstance(ex, minio.S3Error):
+                if ex.code in ["NoSuchKey", "NoSuchBucket", "ResourceNotFound"]:
+                    raise KeyError(f"{ex._resource} ({ex.code})")
+            raise ex
+
+    return _impl
+
+
 class S3StorageBackend(StorageBackend):
+    @_translate_errors
     def storage_size(self, path: str) -> int:
         bucket, prefix = _split_bucket_path(path)
         client = _get_client()
         objects = client.list_objects(bucket, prefix, recursive=True)
         return sum(obj.size for obj in objects)
 
+    @_translate_errors
     def list_dir(self, path: str, *, recursive: bool = False) -> Iterable[str]:
         if not path.startswith("s3://"):
             raise ValueError("path must be an s3 object")
         if not path.endswith("/"):
             path += "/"
         client = _get_client()
         remote_path = path[len("s3://") :]
         bucket_name, *rest = remote_path.split("/")
         prefix = "/".join(rest)
         objects = client.list_objects(bucket_name, prefix, recursive=recursive)
         yield from (f"s3://{obj.bucket_name}/{obj.object_name}" for obj in objects)
 
+    @_translate_errors
     def download_recursive(self, source: str, destination: str) -> None:
         if not source.startswith("s3://"):
             raise ValueError("source must be an s3 object")
         if not source.endswith("/"):
             source += "/"
         client = _get_client()
         remote_path = source[len("s3://") :]
@@ -203,14 +221,15 @@
             remote_file = Path(obj.object_name).relative_to(prefix)
             remote_directory = Path(obj.object_name).parent.relative_to(prefix)
             local_directory = Path(destination) / remote_directory
             local_directory.mkdir(parents=True, exist_ok=True)
             local_file = Path(destination) / remote_file
             client.fget_object(obj.bucket_name, obj.object_name, str(local_file))
 
+    @_translate_errors
     def upload_recursive(self, source: str, destination: str) -> None:
         if not destination.startswith("s3://"):
             raise ValueError("destination must be an s3 object")
         if not destination.endswith("/"):
             destination += "/"
 
         source_path = Path(source)
@@ -230,40 +249,43 @@
             prefix = ""
 
         for file_path, upload_location in zip(source_paths, relative_paths):
             client.fput_object(
                 bucket_name, f"{prefix}{upload_location}", str(file_path)
             )
 
+    @_translate_errors
     def put_object(self, data: bytes | BinaryIO, destination: str) -> None:
         if not destination.startswith("s3://"):
             raise ValueError("destination must be an s3 object")
         bucket_name, bucket_path = _split_bucket_path(destination)
         if bucket_path.endswith("/"):
             raise ValueError("destination is a directory")
         if isinstance(data, bytes):
             data = io.BytesIO(data)
         _get_client().put_object(
             bucket_name, bucket_path, data, length=-1, part_size=10 * 1024 * 1024
         )
 
+    @_translate_errors
     def get_object(self, source: str) -> BinaryIO:
         if not source.startswith("s3://"):
             raise ValueError("source must be an s3 object")
         bucket_name, bucket_path = _split_bucket_path(source)
         if bucket_path.endswith("/"):
             raise ValueError("source is a directory")
 
         try:
             response = _get_client().get_object(bucket_name, bucket_path)
             return io.BytesIO(response.data)
         finally:
             response.close()
             response.release_conn()
 
+    @_translate_errors
     def signed_url_for_artifact_upload(
         self,
         artifact: Artifact,
         storage_path: str,
         *,
         size_limit_bytes: Optional[int] = None,
         _internal_client: bool = False,
@@ -296,14 +318,15 @@
         headers: dict[str, str] = {
             # TODO: Is there an s3 equivalent of this?
             # Google custom header limiting the size of the artifact
             # "x-goog-content-length-range": f"0,{size_limit_bytes}",
         }
         return StorageSignedURL(url=signed_url, method="PUT", headers=headers)
 
+    @_translate_errors
     def signed_url_for_dataset_upload(
         self,
         dataset_id: str,
         artifact: Artifact,
         *,
         size_limit_bytes: Optional[int] = None,
         storage_path: Optional[str] = None,
@@ -313,14 +336,15 @@
         return self.signed_url_for_artifact_upload(
             artifact,
             storage_path,
             size_limit_bytes=size_limit_bytes,
             _internal_client=_internal_client,
         )
 
+    @_translate_errors
     def artifact_downlinks(
         self, entity_kind: Entities, entity_id: str, *, _internal_client: bool = False
     ) -> Iterable[ArtifactURL]:
         storage_root = paths.entity_artifacts_root(entity_kind, entity_id)
         _root_bucket, root_path = _split_bucket_path(storage_root)
         artifact_paths = self.list_dir(storage_root, recursive=True)
         client = _get_client()
@@ -351,14 +375,15 @@
             yield ArtifactURL(
                 artifact=artifact,
                 signedURL=StorageSignedURL(
                     url=signed_url, method="GET", headers=headers
                 ),
             )
 
+    @_translate_errors
     def object_md5hash(self, storage_path: str) -> bytes:
         bucket_name, bucket_path = _split_bucket_path(storage_path)
         client = _get_client()
 
         response = None
         try:
             response = client.get_object(bucket_name, bucket_path)
@@ -373,14 +398,15 @@
             # https://aws.amazon.com/blogs/aws/new-additional-checksum-algorithms-for-amazon-s3/
             return hashlib.md5(response.read()).digest()
         finally:
             if response is not None:
                 response.close()
                 response.release_conn()
 
+    @_translate_errors
     def dataset_artifact_md5hash(
         self, dataset_id: str, artifact_path: str, *, storage_path: Optional[str] = None
     ) -> bytes:
         storage_path = storage_path or paths.dataset_root(dataset_id)
         return self.object_md5hash(f"{storage_path}/{dataset_id}/{artifact_path}")
```

### Comparing `dyff_storage-0.7.4/dyff/storage/config.py` & `dyff_storage-0.7.5/dyff/storage/config.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/paths.py` & `dyff_storage-0.7.5/dyff/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff/storage/timestamp.py` & `dyff_storage-0.7.5/dyff/storage/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/dyff_storage.egg-info/PKG-INFO` & `dyff_storage-0.7.5/dyff_storage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff-storage
-Version: 0.7.4
+Version: 0.7.5
 Summary: Python storage API for the Dyff AI auditing platform.
 Author-email: Digital Safety Research Institute <contact@dsri.org>
 License: Apache-2.0
 Project-URL: Home, https://gitlab.com/dyff/packages/dyff-storage
 Project-URL: Issues, https://gitlab.com/dyff/packages/dyff-storage/-/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dyff_storage-0.7.4/dyff_storage.egg-info/SOURCES.txt` & `dyff_storage-0.7.5/dyff_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/makefile` & `dyff_storage-0.7.5/makefile`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/pyproject.toml` & `dyff_storage-0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dyff_storage-0.7.4/tests/test_import.py` & `dyff_storage-0.7.5/tests/test_import.py`

 * *Files identical despite different names*

