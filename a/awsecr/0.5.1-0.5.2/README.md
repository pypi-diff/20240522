# Comparing `tmp/awsecr-0.5.1.tar.gz` & `tmp/awsecr-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsecr-0.5.1.tar", last modified: Sat Apr  6 23:57:30 2024, max compression
+gzip compressed data, was "awsecr-0.5.2.tar", last modified: Tue May 21 23:37:25 2024, max compression
```

## Comparing `awsecr-0.5.1.tar` & `awsecr-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-06 23:57:30.908139 awsecr-0.5.1/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2024-03-27 22:47:31.000000 awsecr-0.5.1/LICENSE
--rw-r--r--   0 alceu     (1000) alceu     (1000)     6296 2024-04-06 23:57:30.908139 awsecr-0.5.1/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     5469 2024-04-02 00:50:48.000000 awsecr-0.5.1/README.md
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-06 23:57:30.908139 awsecr-0.5.1/awsecr/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      145 2024-04-06 23:56:17.000000 awsecr-0.5.1/awsecr/__init__.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     3201 2024-04-02 00:50:48.000000 awsecr-0.5.1/awsecr/awsecr.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4686 2024-03-27 22:47:31.000000 awsecr-0.5.1/awsecr/cli.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      857 2024-03-27 22:47:31.000000 awsecr-0.5.1/awsecr/exception.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4462 2024-04-02 00:50:48.000000 awsecr-0.5.1/awsecr/image.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     2942 2024-03-27 22:47:31.000000 awsecr-0.5.1/awsecr/repository.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-06 23:57:30.908139 awsecr-0.5.1/awsecr.egg-info/
--rw-r--r--   0 alceu     (1000) alceu     (1000)     6296 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/PKG-INFO
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      462 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/SOURCES.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/dependency_links.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       43 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/entry_points.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/not-zip-safe
--rw-rw-r--   0 alceu     (1000) alceu     (1000)       98 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/requires.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)        7 2024-04-06 23:57:30.000000 awsecr-0.5.1/awsecr.egg-info/top_level.txt
--rw-rw-r--   0 alceu     (1000) alceu     (1000)      423 2024-04-06 23:57:30.912139 awsecr-0.5.1/setup.cfg
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1460 2024-04-06 23:56:17.000000 awsecr-0.5.1/setup.py
-drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-04-06 23:57:30.908139 awsecr-0.5.1/tests/
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4051 2024-03-27 22:47:31.000000 awsecr-0.5.1/tests/test_aws_ecr.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)    10169 2024-03-27 22:47:31.000000 awsecr-0.5.1/tests/test_aws_ecr_image.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     4187 2024-03-27 22:47:31.000000 awsecr-0.5.1/tests/test_aws_ecr_repository.py
--rw-rw-r--   0 alceu     (1000) alceu     (1000)     1524 2024-03-27 22:47:31.000000 awsecr-0.5.1/tests/test_exceptions.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:37:25.775384 awsecr-0.5.2/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)    35149 2024-03-27 22:47:31.000000 awsecr-0.5.2/LICENSE
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6298 2024-05-21 23:37:25.775384 awsecr-0.5.2/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     5469 2024-04-02 00:50:48.000000 awsecr-0.5.2/README.md
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:37:25.771384 awsecr-0.5.2/awsecr/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      145 2024-05-21 23:37:07.000000 awsecr-0.5.2/awsecr/__init__.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     3201 2024-04-02 00:50:48.000000 awsecr-0.5.2/awsecr/awsecr.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4686 2024-03-27 22:47:31.000000 awsecr-0.5.2/awsecr/cli.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      857 2024-03-27 22:47:31.000000 awsecr-0.5.2/awsecr/exception.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4462 2024-04-02 00:50:48.000000 awsecr-0.5.2/awsecr/image.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     2942 2024-03-27 22:47:31.000000 awsecr-0.5.2/awsecr/repository.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:37:25.775384 awsecr-0.5.2/awsecr.egg-info/
+-rw-r--r--   0 alceu     (1000) alceu     (1000)     6298 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/PKG-INFO
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      462 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/SOURCES.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/dependency_links.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)       43 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/entry_points.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        1 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/not-zip-safe
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      100 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/requires.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)        7 2024-05-21 23:37:25.000000 awsecr-0.5.2/awsecr.egg-info/top_level.txt
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)      423 2024-05-21 23:37:25.775384 awsecr-0.5.2/setup.cfg
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1462 2024-05-21 23:37:07.000000 awsecr-0.5.2/setup.py
+drwxrwxr-x   0 alceu     (1000) alceu     (1000)        0 2024-05-21 23:37:25.771384 awsecr-0.5.2/tests/
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4051 2024-03-27 22:47:31.000000 awsecr-0.5.2/tests/test_aws_ecr.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)    10169 2024-03-27 22:47:31.000000 awsecr-0.5.2/tests/test_aws_ecr_image.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     4187 2024-03-27 22:47:31.000000 awsecr-0.5.2/tests/test_aws_ecr_repository.py
+-rw-rw-r--   0 alceu     (1000) alceu     (1000)     1524 2024-03-27 22:47:31.000000 awsecr-0.5.2/tests/test_exceptions.py
```

### Comparing `awsecr-0.5.1/LICENSE` & `awsecr-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/PKG-INFO` & `awsecr-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsecr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easy interaction with AWS ECR from a CLI
 Home-page: https://github.com/glasswalk3r/awsecr
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 Keywords: awsecr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3==1.34.77
+Requires-Dist: boto3==1.34.109
 Requires-Dist: docker==7.0.0
 Requires-Dist: terminaltables==3.1.10
 Requires-Dist: colorama==0.4.6
-Requires-Dist: boto3-stubs[ecr,sts]==1.34.77
+Requires-Dist: boto3-stubs[ecr,sts]==1.34.110
 
 # awsecr
 
 [![Python application](https://github.com/glasswalk3r/awsecr/actions/workflows/python-app.yml/badge.svg)](https://github.com/glasswalk3r/awsecr/actions/workflows/python-app.yml)
 
 CLI to interact with AWS ECR service.
```

### Comparing `awsecr-0.5.1/README.md` & `awsecr-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr/awsecr.py` & `awsecr-0.5.2/awsecr/awsecr.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr/cli.py` & `awsecr-0.5.2/awsecr/cli.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr/exception.py` & `awsecr-0.5.2/awsecr/exception.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr/image.py` & `awsecr-0.5.2/awsecr/image.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr/repository.py` & `awsecr-0.5.2/awsecr/repository.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/awsecr.egg-info/PKG-INFO` & `awsecr-0.5.2/awsecr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsecr
-Version: 0.5.1
+Version: 0.5.2
 Summary: Easy interaction with AWS ECR from a CLI
 Home-page: https://github.com/glasswalk3r/awsecr
 Author: Alceu Rodrigues de Freitas Junior
 Author-email: arfreitas@cpan.org
 Keywords: awsecr
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: boto3==1.34.77
+Requires-Dist: boto3==1.34.109
 Requires-Dist: docker==7.0.0
 Requires-Dist: terminaltables==3.1.10
 Requires-Dist: colorama==0.4.6
-Requires-Dist: boto3-stubs[ecr,sts]==1.34.77
+Requires-Dist: boto3-stubs[ecr,sts]==1.34.110
 
 # awsecr
 
 [![Python application](https://github.com/glasswalk3r/awsecr/actions/workflows/python-app.yml/badge.svg)](https://github.com/glasswalk3r/awsecr/actions/workflows/python-app.yml)
 
 CLI to interact with AWS ECR service.
```

### Comparing `awsecr-0.5.1/setup.py` & `awsecr-0.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
-requirements = ['boto3==1.34.77', 'docker==7.0.0', 'terminaltables==3.1.10',
-                'colorama==0.4.6', 'boto3-stubs[ecr,sts]==1.34.77']
+requirements = ['boto3==1.34.109', 'docker==7.0.0', 'terminaltables==3.1.10',
+                'colorama==0.4.6', 'boto3-stubs[ecr,sts]==1.34.110']
 setup_requirements = ['pytest-runner', ]
 test_requirements = ['pytest>=3', ]
 
 setup(
     author="Alceu Rodrigues de Freitas Junior",
     author_email='arfreitas@cpan.org',
     python_requires='>=3.8',
@@ -38,10 +38,10 @@
     keywords='awsecr',
     name='awsecr',
     packages=find_packages(include=['awsecr', 'awsecr.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/glasswalk3r/awsecr',
-    version='0.5.1',
+    version='0.5.2',
     zip_safe=False,
 )
```

### Comparing `awsecr-0.5.1/tests/test_aws_ecr.py` & `awsecr-0.5.2/tests/test_aws_ecr.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/tests/test_aws_ecr_image.py` & `awsecr-0.5.2/tests/test_aws_ecr_image.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/tests/test_aws_ecr_repository.py` & `awsecr-0.5.2/tests/test_aws_ecr_repository.py`

 * *Files identical despite different names*

### Comparing `awsecr-0.5.1/tests/test_exceptions.py` & `awsecr-0.5.2/tests/test_exceptions.py`

 * *Files identical despite different names*

