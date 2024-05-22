# Comparing `tmp/klein_mongo-2.0.7.tar.gz` & `tmp/klein_mongo-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/klein_mongo-2.0.7.tar", last modified: Mon May 30 07:45:58 2022, max compression
+gzip compressed data, was "klein_mongo-3.0.0.tar", last modified: Wed May 22 13:39:35 2024, max compression
```

## Comparing `klein_mongo-2.0.7.tar` & `klein_mongo-3.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     9135 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/LICENSE.txt
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       17 2022-05-23 09:20:55.000000 klein_mongo-2.0.7/MANIFEST.in
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1197 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/PKG-INFO
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)      867 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/README.md
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       38 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/setup.cfg
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1535 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/setup.py
-drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/
-drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo/
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       62 2022-05-23 09:20:55.000000 klein_mongo-2.0.7/src/klein_mongo/__init__.py
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     3216 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/src/klein_mongo/connect.py
-drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     1197 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/PKG-INFO
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)      346 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/SOURCES.txt
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        1 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/dependency_links.txt
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       37 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/requires.txt
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)       12 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/top_level.txt
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        1 2022-05-30 07:45:15.000000 klein_mongo-2.0.7/src/klein_mongo.egg-info/zip-safe
-drwxr-xr-x   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)        0 2022-05-30 07:45:58.000000 klein_mongo-2.0.7/test/
--rw-r--r--   0 nick.etherington (1957169981) MEDCAT\Domain Users (1293359979)     2766 2022-05-30 07:36:35.000000 klein_mongo-2.0.7/test/test_connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:39:35.789599 klein_mongo-3.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     9135 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-22 13:39:35.789599 klein_mongo-3.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      868 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 13:39:35.789599 klein_mongo-3.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:39:35.786599 klein_mongo-3.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:39:35.787599 klein_mongo-3.0.0/src/klein_mongo/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/src/klein_mongo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3567 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/src/klein_mongo/connect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:39:35.788599 klein_mongo-3.0.0/src/klein_mongo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      361 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 13:39:35.000000 klein_mongo-3.0.0/src/klein_mongo.egg-info/zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/src/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:39:35.788599 klein_mongo-3.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2024-05-22 13:39:23.000000 klein_mongo-3.0.0/test/test_connect.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `klein_mongo-2.0.7/LICENSE.txt` & `klein_mongo-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `klein_mongo-2.0.7/PKG-INFO` & `klein_mongo-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: klein_mongo
-Version: 2.0.7
+Version: 3.0.0
 Summary: MongoDB integration
 Home-page: https://github.com/mdcatapult/py-mongo
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: klein_config>=3.0.0
+Requires-Dist: pymongo[srv]>=4.4.1
 
 # Klein Mongo
 
 Module to allow simple instantiation of MongoDB from configuration
 
 See the [config.example.yml](./config.example.yml) for example configuration.
 
@@ -27,15 +28,15 @@
 ```
 
 ## Development
 We use `virtualenv` for local development environments: `pip install virtualenv`.
 
 Once installed, run:
 ```
-virtualenv -p python3.7 venv
+virtualenv -p python3.11 venv
 source venv/bin/activate
 pip install -r requirements.txt
 ```
 Then configure your IDE to use the python interpreter located at `venv/bin/python`.
 ### Testing
 ```bash
 python -m pytest
@@ -43,9 +44,7 @@
 For test coverage you can run:
 ```bash
 pytest --cov-report term:skip-covered --cov src/ test/
 ```
 
 ### License
 This project is licensed under the terms of the Apache 2 license, which can be found in the repository as `LICENSE.txt`
-
-
```

### Comparing `klein_mongo-2.0.7/README.md` & `klein_mongo-3.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ```
 
 ## Development
 We use `virtualenv` for local development environments: `pip install virtualenv`.
 
 Once installed, run:
 ```
-virtualenv -p python3.7 venv
+virtualenv -p python3.11 venv
 source venv/bin/activate
 pip install -r requirements.txt
 ```
 Then configure your IDE to use the python interpreter located at `venv/bin/python`.
 ### Testing
 ```bash
 python -m pytest
```

### Comparing `klein_mongo-2.0.7/setup.py` & `klein_mongo-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,12 @@
       url='https://github.com/mdcatapult/py-mongo',
       author='Medicines Discovery Catapult',
       author_email='SoftwareEngineering@md.catapult.org.uk',
       license='Apache V2',
       packages=find_packages('src'),
       package_dir={'':'src'},
       install_requires=[
-          'klein_config~=3.0',
-          'pymongo[srv]~=3.11',
+          'klein_config>=3.0.0',
+          'pymongo[srv]>=4.4.1',
       ],
-      zip_safe=True)
+      zip_safe=True,
+      include_package_data=True)
```

### Comparing `klein_mongo-2.0.7/src/klein_mongo/connect.py` & `klein_mongo-3.0.0/src/klein_mongo/connect.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,14 +76,19 @@
         self.params["readPreference"] = config.get('mongo.readPreference', 'secondaryPreferred')
 
         # Use cross language compatible UUID encoding as default. Can be overridden with
         # 'pythonLegacy', 'javaLegacy' or 'csharpLegacy' if required.
         # ref: https://api.mongodb.com/python/current/api/pymongo/mongo_client.html?
         self.params['uuidRepresentation'] = config.get('mongo.uuidRepresentation', 'standard')
 
+        # There are some data with strings that cannot be handled by unicode
+        # This may cause an error during query
+        # Default this to ignore as there is no known good way to handle this other than ignoring corrupted data
+        self.params['unicode_decode_error_handler'] = config.get('mongo.unicode_decode_error_handler', 'ignore')
+
     @lazy_property
     def client(self):
         c = _MongoClient(*self.host, replicaset=self.replicaSet, **self.params)
         return c
 
 
 def get_client(config):
```

### Comparing `klein_mongo-2.0.7/src/klein_mongo.egg-info/PKG-INFO` & `klein_mongo-3.0.0/src/klein_mongo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
-Name: klein-mongo
-Version: 2.0.7
+Name: klein_mongo
+Version: 3.0.0
 Summary: MongoDB integration
 Home-page: https://github.com/mdcatapult/py-mongo
 Author: Medicines Discovery Catapult
 Author-email: SoftwareEngineering@md.catapult.org.uk
 License: Apache V2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: klein_config>=3.0.0
+Requires-Dist: pymongo[srv]>=4.4.1
 
 # Klein Mongo
 
 Module to allow simple instantiation of MongoDB from configuration
 
 See the [config.example.yml](./config.example.yml) for example configuration.
 
@@ -27,15 +28,15 @@
 ```
 
 ## Development
 We use `virtualenv` for local development environments: `pip install virtualenv`.
 
 Once installed, run:
 ```
-virtualenv -p python3.7 venv
+virtualenv -p python3.11 venv
 source venv/bin/activate
 pip install -r requirements.txt
 ```
 Then configure your IDE to use the python interpreter located at `venv/bin/python`.
 ### Testing
 ```bash
 python -m pytest
@@ -43,9 +44,7 @@
 For test coverage you can run:
 ```bash
 pytest --cov-report term:skip-covered --cov src/ test/
 ```
 
 ### License
 This project is licensed under the terms of the Apache 2 license, which can be found in the repository as `LICENSE.txt`
-
-
```

### Comparing `klein_mongo-2.0.7/test/test_connect.py` & `klein_mongo-3.0.0/test/test_connect.py`

 * *Files identical despite different names*

