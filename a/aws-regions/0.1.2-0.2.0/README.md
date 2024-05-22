# Comparing `tmp/aws-regions-0.1.2.tar.gz` & `tmp/aws_regions-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-regions-0.1.2.tar", last modified: Wed Feb 16 19:44:40 2022, max compression
+gzip compressed data, was "aws_regions-0.2.0.tar", last modified: Wed May 22 19:19:54 2024, max compression
```

## Comparing `aws-regions-0.1.2.tar` & `aws_regions-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.502168 aws-regions-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-02-16 19:44:31.000000 aws-regions-0.1.2/CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (121)     2049 2022-02-16 19:44:31.000000 aws-regions-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-02-16 19:44:31.000000 aws-regions-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-02-16 19:44:31.000000 aws-regions-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-02-16 19:44:40.502168 aws-regions-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1889 2022-02-16 19:44:31.000000 aws-regions-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.498168 aws-regions-0.1.2/aws_regions/
--rw-r--r--   0 runner    (1001) docker     (121)     1179 2022-02-16 19:44:31.000000 aws-regions-0.1.2/aws_regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-02-16 19:44:31.000000 aws-regions-0.1.2/aws_regions/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2410 2022-02-16 19:44:31.000000 aws-regions-0.1.2/aws_regions/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.498168 aws-regions-0.1.2/aws_regions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-16 19:44:40.000000 aws-regions-0.1.2/aws_regions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-02-16 19:44:40.502168 aws-regions-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2022-02-16 19:44:31.000000 aws-regions-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.498168 aws-regions-0.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.502168 aws-regions-0.1.2/tests/cassettes/
--rw-r--r--   0 runner    (1001) docker     (121)    20839 2022-02-16 19:44:31.000000 aws-regions-0.1.2/tests/cassettes/get_all_regions.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 19:44:40.502168 aws-regions-0.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-02-16 19:44:31.000000 aws-regions-0.1.2/tests/data/test.config
--rw-r--r--   0 runner    (1001) docker     (121)     2084 2022-02-16 19:44:31.000000 aws-regions-0.1.2/tests/test_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.589076 aws_regions-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-22 19:19:46.000000 aws_regions-0.2.0/CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-22 19:19:46.000000 aws_regions-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 19:19:46.000000 aws_regions-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 19:19:46.000000 aws_regions-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-22 19:19:54.585076 aws_regions-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-22 19:19:46.000000 aws_regions-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.581076 aws_regions-0.2.0/aws_regions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-22 19:19:46.000000 aws_regions-0.2.0/aws_regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-22 19:19:46.000000 aws_regions-0.2.0/aws_regions/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-22 19:19:46.000000 aws_regions-0.2.0/aws_regions/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.585076 aws_regions-0.2.0/aws_regions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:19:54.000000 aws_regions-0.2.0/aws_regions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-22 19:19:54.589076 aws_regions-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-05-22 19:19:46.000000 aws_regions-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.585076 aws_regions-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.585076 aws_regions-0.2.0/tests/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (127)  1062354 2024-05-22 19:19:46.000000 aws_regions-0.2.0/tests/cassettes/get_all_regions.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:19:54.585076 aws_regions-0.2.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 19:19:46.000000 aws_regions-0.2.0/tests/data/test.config
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-05-22 19:19:46.000000 aws_regions-0.2.0/tests/test_endpoints.py
```

### Comparing `aws-regions-0.1.2/CONTRIBUTING.md` & `aws_regions-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aws-regions-0.1.2/LICENSE` & `aws_regions-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-regions-0.1.2/PKG-INFO` & `aws_regions-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: aws-regions
-Version: 0.1.2
-Summary: Provides functions to get up-to-date AWS regions lists.
-Home-page: https://github.com/SUSE-Enceladus/aws-regions
-Author: SUSE
-Author-email: public-cloud-dev@susecloud.net
-License: MIT
-Keywords: aws-regions aws_regions
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: test
-License-File: LICENSE
-
 [![Continuous testing & Linting](https://github.com/SUSE-Enceladus/aws-regions/actions/workflows/ci.yml/badge.svg)](https://github.com/SUSE-Enceladus/aws-regions/actions/workflows/ci.yml)
 
 Overview
 ========
 
 This package provides a very simple API for retrieving the most up-to-date
 region list. The region info is pulled from the botocore Github project so
@@ -94,9 +67,7 @@
 =======
 
 Copyright (c) 2021 SUSE LLC.
 
 Distributed under the terms of MIT license, see
 [LICENSE](https://github.com/SUSE-Enceladus/aws-regions/blob/master/LICENSE)
 for details.
-
-
```

### Comparing `aws-regions-0.1.2/aws_regions/__init__.py` & `aws_regions-0.2.0/aws_regions/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 __author__ = """SUSE"""
 __email__ = 'public-cloud-dev@susecloud.net'
-__version__ = '0.1.2'
+__version__ = '0.2.0'
```

### Comparing `aws-regions-0.1.2/aws_regions/config.py` & `aws_regions-0.2.0/aws_regions/config.py`

 * *Files identical despite different names*

### Comparing `aws-regions-0.1.2/aws_regions/endpoints.py` & `aws_regions-0.2.0/aws_regions/endpoints.py`

 * *Files identical despite different names*

### Comparing `aws-regions-0.1.2/aws_regions.egg-info/PKG-INFO` & `aws_regions-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 Metadata-Version: 2.1
 Name: aws-regions
-Version: 0.1.2
+Version: 0.2.0
 Summary: Provides functions to get up-to-date AWS regions lists.
 Home-page: https://github.com/SUSE-Enceladus/aws-regions
 Author: SUSE
 Author-email: public-cloud-dev@susecloud.net
 License: MIT
 Keywords: aws-regions aws_regions
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: dataclasses~=0.8; python_version < "3.7"
 Provides-Extra: dev
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: vcrpy; extra == "dev"
+Requires-Dist: bumpversion; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: vcrpy; extra == "test"
 
 [![Continuous testing & Linting](https://github.com/SUSE-Enceladus/aws-regions/actions/workflows/ci.yml/badge.svg)](https://github.com/SUSE-Enceladus/aws-regions/actions/workflows/ci.yml)
 
 Overview
 ========
 
 This package provides a very simple API for retrieving the most up-to-date
@@ -94,9 +104,7 @@
 =======
 
 Copyright (c) 2021 SUSE LLC.
 
 Distributed under the terms of MIT license, see
 [LICENSE](https://github.com/SUSE-Enceladus/aws-regions/blob/master/LICENSE)
 for details.
-
-
```

### Comparing `aws-regions-0.1.2/setup.py` & `aws_regions-0.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,27 +36,27 @@
 
 with open('requirements-dev.txt') as req_file:
     dev_requirements = test_requirements + req_file.read().splitlines()[2:]
 
 
 setup(
     name='aws-regions',
-    version='0.1.2',
+    version='0.2.0',
     description='Provides functions to get up-to-date AWS regions lists.',
     long_description=readme,
     long_description_content_type="text/markdown",
     author="SUSE",
     author_email='public-cloud-dev@susecloud.net',
     url='https://github.com/SUSE-Enceladus/aws-regions',
     packages=find_packages(),
     package_dir={
         'aws_regions': 'aws_regions'
     },
     include_package_data=True,
-    python_requires='>=3.6',
+    python_requires='>=3.10',
     install_requires=requirements,
     extras_require={
         'dev': dev_requirements,
         'test': test_requirements
     },
     license='MIT',
     zip_safe=False,
@@ -64,14 +64,12 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

