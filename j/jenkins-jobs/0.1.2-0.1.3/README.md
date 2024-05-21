# Comparing `tmp/jenkins_jobs-0.1.2.tar.gz` & `tmp/jenkins_jobs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkins_jobs-0.1.2.tar", last modified: Wed Apr 24 01:05:05 2024, max compression
+gzip compressed data, was "jenkins_jobs-0.1.3.tar", last modified: Tue May 21 23:25:56 2024, max compression
```

## Comparing `jenkins_jobs-0.1.2.tar` & `jenkins_jobs-0.1.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      183 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/AUTHORS.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3577 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       89 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/HISTORY.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/LICENSE
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      262 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/MANIFEST.in
--rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     5814 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.2/README.rst
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.026406 jenkins_jobs-0.1.2/docs/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      613 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/Makefile
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.026406 jenkins_jobs-0.1.2/docs/_build/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.026406 jenkins_jobs-0.1.2/docs/_build/html/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.026406 jenkins_jobs-0.1.2/docs/_build/html/_static/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      286 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/authors.rst
--rwxrwxr-x   0 alceu     (1000) alceu     (1000)     1228 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.2/docs/conf.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       33 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/contributing.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/history.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      311 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/index.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1166 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/installation.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      954 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.2/docs/jenkins_jobs.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      774 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/make.bat
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       73 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.2/docs/modules.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       27 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/readme.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       79 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/docs/usage.rst
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      413 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/setup.cfg
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1734 2024-04-24 01:03:57.000000 jenkins_jobs-0.1.2/setup.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.026406 jenkins_jobs-0.1.2/src/
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/src/jenkins_jobs/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      157 2024-04-24 01:03:57.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/__init__.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3017 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/exceptions.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1735 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/exporter.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     9855 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/jobs.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1336 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/reporter.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3212 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/src/jenkins_jobs/retrievers.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/
--rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1324 2024-04-24 01:05:05.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/SOURCES.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/dependency_links.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      106 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/entry_points.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/not-zip-safe
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       40 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/requires.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       13 2024-04-24 01:05:04.000000 jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/top_level.txt
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/tests/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       42 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/__init__.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      288 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/conftest.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-24 01:05:05.030406 jenkins_jobs-0.1.2/tests/raw_data/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4581 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/bogus-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2481 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2457 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-nodesc.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2596 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-trigger.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2477 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/freestyle-job.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2641 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/maven-job-plugin-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2637 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/maven-job-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1844 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin-bogus.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1840 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin-timer.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4587 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin.xml
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     6522 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/test_jobs.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1762 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.2/tests/test_retrievers.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.766839 jenkins_jobs-0.1.3/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      183 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/AUTHORS.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3577 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       89 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/HISTORY.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/LICENSE
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      262 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/MANIFEST.in
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-05-21 23:25:56.766839 jenkins_jobs-0.1.3/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     5814 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.3/README.rst
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.762839 jenkins_jobs-0.1.3/docs/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      613 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/Makefile
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.758839 jenkins_jobs-0.1.3/docs/_build/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.758839 jenkins_jobs-0.1.3/docs/_build/html/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.762839 jenkins_jobs-0.1.3/docs/_build/html/_static/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      286 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.3/docs/_build/html/_static/file.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.3/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       90 2024-04-07 20:26:45.000000 jenkins_jobs-0.1.3/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/authors.rst
+-rwxrwxr-x   0 alceu     (1000) alceu     (1000)     1228 2024-04-07 20:43:43.000000 jenkins_jobs-0.1.3/docs/conf.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       33 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/contributing.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       28 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/history.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      311 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/index.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1166 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/installation.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      954 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.3/docs/jenkins_jobs.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      774 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/make.bat
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       73 2024-04-07 20:39:49.000000 jenkins_jobs-0.1.3/docs/modules.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       27 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/readme.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       79 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/docs/usage.rst
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      413 2024-05-21 23:25:56.766839 jenkins_jobs-0.1.3/setup.cfg
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1734 2024-05-21 23:25:39.000000 jenkins_jobs-0.1.3/setup.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.758839 jenkins_jobs-0.1.3/src/
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.762839 jenkins_jobs-0.1.3/src/jenkins_jobs/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      157 2024-05-21 23:25:39.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/__init__.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3017 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/exceptions.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1735 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/exporter.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     9855 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/jobs.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1336 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/reporter.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3212 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/src/jenkins_jobs/retrievers.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.766839 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6839 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1324 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/SOURCES.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/dependency_links.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      106 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/entry_points.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/not-zip-safe
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       40 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/requires.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       13 2024-05-21 23:25:56.000000 jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/top_level.txt
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.762839 jenkins_jobs-0.1.3/tests/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       42 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/__init__.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      288 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/conftest.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:25:56.766839 jenkins_jobs-0.1.3/tests/raw_data/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4581 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/bogus-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2481 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2457 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-nodesc.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2596 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-trigger.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2477 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/freestyle-job.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2641 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/maven-job-plugin-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2637 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/maven-job-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1844 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin-bogus.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1840 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin-timer.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4587 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin.xml
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     6522 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/test_jobs.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1762 2024-04-07 20:01:27.000000 jenkins_jobs-0.1.3/tests/test_retrievers.py
```

### Comparing `jenkins_jobs-0.1.2/CONTRIBUTING.rst` & `jenkins_jobs-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/LICENSE` & `jenkins_jobs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/PKG-INFO` & `jenkins_jobs-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenkins_jobs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Listing all jobs on a Jenkins server with more information than jenkins-cli.jar
 Home-page: https://github.com/glasswalk3r/jenkins-jobs
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 License: GNU General Public License v3
 Keywords: jenkins jobs
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jenkins_jobs-0.1.2/README.rst` & `jenkins_jobs-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/docs/Makefile` & `jenkins_jobs-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/docs/conf.py` & `jenkins_jobs-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/docs/installation.rst` & `jenkins_jobs-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/docs/jenkins_jobs.rst` & `jenkins_jobs-0.1.3/docs/jenkins_jobs.rst`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/docs/make.bat` & `jenkins_jobs-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/setup.py` & `jenkins_jobs-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     name='jenkins_jobs',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/glasswalk3r/jenkins-jobs',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs/exceptions.py` & `jenkins_jobs-0.1.3/src/jenkins_jobs/exceptions.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs/exporter.py` & `jenkins_jobs-0.1.3/src/jenkins_jobs/exporter.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs/jobs.py` & `jenkins_jobs-0.1.3/src/jenkins_jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs/reporter.py` & `jenkins_jobs-0.1.3/src/jenkins_jobs/reporter.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs/retrievers.py` & `jenkins_jobs-0.1.3/src/jenkins_jobs/retrievers.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/PKG-INFO` & `jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenkins_jobs
-Version: 0.1.2
+Version: 0.1.3
 Summary: Listing all jobs on a Jenkins server with more information than jenkins-cli.jar
 Home-page: https://github.com/glasswalk3r/jenkins-jobs
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 License: GNU General Public License v3
 Keywords: jenkins jobs
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `jenkins_jobs-0.1.2/src/jenkins_jobs.egg-info/SOURCES.txt` & `jenkins_jobs-0.1.3/src/jenkins_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/bogus-plugin.xml` & `jenkins_jobs-0.1.3/tests/raw_data/bogus-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-bogus.xml` & `jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-nodesc.xml` & `jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-nodesc.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/freestyle-job-trigger.xml` & `jenkins_jobs-0.1.3/tests/raw_data/freestyle-job-trigger.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/freestyle-job.xml` & `jenkins_jobs-0.1.3/tests/raw_data/freestyle-job.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/maven-job-plugin-bogus.xml` & `jenkins_jobs-0.1.3/tests/raw_data/maven-job-plugin-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/maven-job-plugin.xml` & `jenkins_jobs-0.1.3/tests/raw_data/maven-job-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin-bogus.xml` & `jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin-bogus.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin-timer.xml` & `jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin-timer.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/raw_data/workflow-job-plugin.xml` & `jenkins_jobs-0.1.3/tests/raw_data/workflow-job-plugin.xml`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/test_jobs.py` & `jenkins_jobs-0.1.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `jenkins_jobs-0.1.2/tests/test_retrievers.py` & `jenkins_jobs-0.1.3/tests/test_retrievers.py`

 * *Files identical despite different names*

