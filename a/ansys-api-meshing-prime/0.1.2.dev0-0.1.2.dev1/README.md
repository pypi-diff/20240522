# Comparing `tmp/ansys-api-meshing-prime-0.1.2.dev0.tar.gz` & `tmp/ansys-api-meshing-prime-0.1.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-api-meshing-prime-0.1.2.dev0.tar", last modified: Tue Sep  5 19:31:00 2023, max compression
+gzip compressed data, was "ansys-api-meshing-prime-0.1.2.dev1.tar", last modified: Tue Sep 26 15:52:19 2023, max compression
```

## Comparing `ansys-api-meshing-prime-0.1.2.dev0.tar` & `ansys-api-meshing-prime-0.1.2.dev1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (999)     1089 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     1928 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1560 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (999)      179 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1676 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.503399 ansys-api-meshing-prime-0.1.2.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.503399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.503399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.503399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/
--rw-r--r--   0 runner    (1001) docker     (999)       10 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/VERSION
--rw-r--r--   0 runner    (1001) docker     (999)      259 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/v1/
--rw-r--r--   0 runner    (1001) docker     (999)     1350 2023-09-05 19:30:42.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/v1/prime.proto
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-05 19:31:00.507399 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1928 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      505 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       93 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)        6 2023-09-05 19:31:00.000000 ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.149260 ansys-api-meshing-prime-0.1.2.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.149260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.149260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.149260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2023-09-26 15:51:58.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/v1/prime.proto
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 15:52:19.153260 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 15:52:19.000000 ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/top_level.txt
```

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/LICENSE` & `ansys-api-meshing-prime-0.1.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/PKG-INFO` & `ansys-api-meshing-prime-0.1.2.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ansys-api-meshing-prime
-Version: 0.1.2.dev0
+Version: 0.1.2.dev1
 Summary: Autogenerated python gRPC interface package for ansys-api-meshing-prime
 Home-page: https://github.com/ansys/ansys-api-meshing-prime
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio~=1.46
+Requires-Dist: protobuf~=3.19
 
 # Ansys Prime Server gRPC Interface Package
 
 This Python package contains the auto-generated gRPC Python interface files for
 Ansys Prime Server.  Contributions for this API will not be accepted.  Please
 create an issue or discussion for questions or enhancements relating to this
 project.
@@ -36,16 +38,17 @@
 ```
 
 This will create both the source distribution containing just the protofiles
 along with the wheel containing the protofiles and build Python interface
 files.
 
 Note that the interface files are identical regardless of the version of Python
-used to generate them, but the last pre-built wheel was Python 3.7, so to
-improve your build time, use Python 3.7 when building the wheel.
+used to generate them, but the last pre-built wheel for `grpcio~=1.46` was
+Python 3.10, so to improve your build time, use Python 3.10 when building the
+wheel.
 
 ## Manual Deployment
 
 After building the packages, manually deploy them with:
 
 ```bash
 pip install twine
```

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/README.md` & `ansys-api-meshing-prime-0.1.2.dev1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 ```
 
 This will create both the source distribution containing just the protofiles
 along with the wheel containing the protofiles and build Python interface
 files.
 
 Note that the interface files are identical regardless of the version of Python
-used to generate them, but the last pre-built wheel was Python 3.7, so to
-improve your build time, use Python 3.7 when building the wheel.
+used to generate them, but the last pre-built wheel for `grpcio~=1.46` was
+Python 3.10, so to improve your build time, use Python 3.10 when building the
+wheel.
 
 ## Manual Deployment
 
 After building the packages, manually deploy them with:
 
 ```bash
 pip install twine
```

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/setup.py` & `ansys-api-meshing-prime-0.1.2.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         description=description,
         long_description=long_description,
         long_description_content_type='text/markdown',
         url=f'https://github.com/ansys/{package_name}',
         license='MIT',
         python_requires='>=3.8, <4',
         install_requires=[
-            'grpcio>=1.26.0',  
-            'protobuf>=3.12.2, <5',  # minimum required based on meta-package
+            'grpcio~=1.46',  
+            'protobuf~=3.19',  # minimum required based on meta-package
         ],
         packages=find_namespace_packages('src', include=('ansys.*',)),
         package_dir={'': 'src'},
         package_data={
             '': [ '*.proto', '*.pyi', 'py.typed', 'VERSION' ]
         },
         entry_points={
```

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/src/ansys/api/meshing/prime/v1/prime.proto` & `ansys-api-meshing-prime-0.1.2.dev1/src/ansys/api/meshing/prime/v1/prime.proto`

 * *Files identical despite different names*

### Comparing `ansys-api-meshing-prime-0.1.2.dev0/src/ansys_api_meshing_prime.egg-info/PKG-INFO` & `ansys-api-meshing-prime-0.1.2.dev1/src/ansys_api_meshing_prime.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: ansys-api-meshing-prime
-Version: 0.1.2.dev0
+Version: 0.1.2.dev1
 Summary: Autogenerated python gRPC interface package for ansys-api-meshing-prime
 Home-page: https://github.com/ansys/ansys-api-meshing-prime
 Author: ANSYS, Inc.
 Author-email: support@ansys.com
 License: MIT
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: grpcio~=1.46
+Requires-Dist: protobuf~=3.19
 
 # Ansys Prime Server gRPC Interface Package
 
 This Python package contains the auto-generated gRPC Python interface files for
 Ansys Prime Server.  Contributions for this API will not be accepted.  Please
 create an issue or discussion for questions or enhancements relating to this
 project.
@@ -36,16 +38,17 @@
 ```
 
 This will create both the source distribution containing just the protofiles
 along with the wheel containing the protofiles and build Python interface
 files.
 
 Note that the interface files are identical regardless of the version of Python
-used to generate them, but the last pre-built wheel was Python 3.7, so to
-improve your build time, use Python 3.7 when building the wheel.
+used to generate them, but the last pre-built wheel for `grpcio~=1.46` was
+Python 3.10, so to improve your build time, use Python 3.10 when building the
+wheel.
 
 ## Manual Deployment
 
 After building the packages, manually deploy them with:
 
 ```bash
 pip install twine
```

