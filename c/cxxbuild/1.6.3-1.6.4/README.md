# Comparing `tmp/cxxbuild-1.6.3.tar.gz` & `tmp/cxxbuild-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cxxbuild-1.6.3.tar", last modified: Tue May 21 14:54:31 2024, max compression
+gzip compressed data, was "cxxbuild-1.6.4.tar", last modified: Wed May 22 00:47:50 2024, max compression
```

## Comparing `cxxbuild-1.6.3.tar` & `cxxbuild-1.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/
--rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14991 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12930 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/README.md
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.129412 cxxbuild-1.6.3/cxxbuild/
--rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.3/cxxbuild/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54411 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/cxxbuild/cxxbuild.py
-drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-21 14:54:31.133412 cxxbuild-1.6.3/cxxbuild.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14991 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      277 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-21 14:54:31.000000 cxxbuild-1.6.3/cxxbuild.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      923 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 14:54:31.137412 cxxbuild-1.6.3/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      227 2024-05-21 14:54:06.000000 cxxbuild-1.6.3/setup.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-22 00:47:50.019753 cxxbuild-1.6.4/
+-rw-rw-r--   0 root         (0) root         (0)     1065 2023-11-07 22:41:49.000000 cxxbuild-1.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15190 2024-05-22 00:47:50.019753 cxxbuild-1.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13129 2024-05-22 00:47:25.000000 cxxbuild-1.6.4/README.md
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-22 00:47:50.015753 cxxbuild-1.6.4/cxxbuild/
+-rw-r--r--   0 root         (0) root         (0)       27 2023-12-31 14:16:19.000000 cxxbuild-1.6.4/cxxbuild/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54882 2024-05-22 00:47:25.000000 cxxbuild-1.6.4/cxxbuild/cxxbuild.py
+drwxr-sr-x   0 root         (0) root         (0)        0 2024-05-22 00:47:50.019753 cxxbuild-1.6.4/cxxbuild.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15190 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      277 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-22 00:47:50.000000 cxxbuild-1.6.4/cxxbuild.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      923 2024-05-22 00:47:25.000000 cxxbuild-1.6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 00:47:50.019753 cxxbuild-1.6.4/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      227 2024-05-22 00:47:25.000000 cxxbuild-1.6.4/setup.py
```

### Comparing `cxxbuild-1.6.3/LICENSE` & `cxxbuild-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cxxbuild-1.6.3/PKG-INFO` & `cxxbuild-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.3
+Version: 1.6.4
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.3`
+- Version: `cxxbuild version=1.6.4`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -199,14 +199,17 @@
 - take system `-lm` dependency
 - C++ standard `c++17` is used
 - build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
+The `local` can be specified for `cmake` or `bazel`, like `cmake+local` or `bazel+local`.
+On `cmake` it represents a `find_package`, while on `bazel` it is a `local_repository` (to implement, yet).
+
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
 Some ongoing extensions will allow managing dev dependencies, 
 such as build systems (cmake, bazel, etc) and C/C++ package managers (conan, etc), all automatically on `cxxdeps.txt` (or exclusively on `cxxdeps.dev.txt`):
 ```
 cmake == *          [ cmake ]       pip dev [ ninja ]
```

### Comparing `cxxbuild-1.6.3/README.md` & `cxxbuild-1.6.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.3`
+- Version: `cxxbuild version=1.6.4`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -155,14 +155,17 @@
 - take system `-lm` dependency
 - C++ standard `c++17` is used
 - build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
+The `local` can be specified for `cmake` or `bazel`, like `cmake+local` or `bazel+local`.
+On `cmake` it represents a `find_package`, while on `bazel` it is a `local_repository` (to implement, yet).
+
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
 Some ongoing extensions will allow managing dev dependencies, 
 such as build systems (cmake, bazel, etc) and C/C++ package managers (conan, etc), all automatically on `cxxdeps.txt` (or exclusively on `cxxdeps.dev.txt`):
 ```
 cmake == *          [ cmake ]       pip dev [ ninja ]
```

### Comparing `cxxbuild-1.6.3/cxxbuild/cxxbuild.py` & `cxxbuild-1.6.4/cxxbuild/cxxbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import platform
 import sys
 import json
 import subprocess
 
 def version():
-    v = "cxxbuild=1.6.3"
+    v = "cxxbuild=1.6.4"
     return v
 
 def usage():
     u=version()+"""
 Usage:
     cxxbuild [build] [ROOT_PATH] 
       builds with cxxbuild, examples: 
@@ -992,14 +992,16 @@
             # add extra source file
             build_options_args.append("!extrasrc "+str(sys.argv[i + 1]))
         if (sys.argv[i] == "--tests"):
             build_options_args.append("!tests \""+str(sys.argv[i + 1])+"\"")
         if (sys.argv[i] == "--include"):
             # force --include to appear
             build_options_args.append("!include \""+str(sys.argv[i + 1])+"\"")
+        if (sys.argv[i] == "--ignore"):
+            build_options_args.append("!ignore "+str(sys.argv[i + 1]))
         if (sys.argv[i] == "--define"):
             # force --define to appear
             build_options_args.append("!define "+str(sys.argv[i + 1]))
         if (sys.argv[i] == "--cmake"):
             build_options_args.append("!build cmake")
         if (sys.argv[i] == "--bazel"):
             build_options_args.append("!build bazel")
@@ -1041,14 +1043,17 @@
     #
     use_cmake=None
     use_bazel=None
     cppstd="17"
     INCLUDE_DIRS = []
     DEFINITIONS = []
     EXTRA_SOURCES = []
+    IGNORE = []
+    # ignore build/ folder by default
+    IGNORE.append("build/")
     for op in build_options:
         # import shlex
         # oplist = shlex.split(op)
         oplist = op.split()
         print(op.split())
         if oplist[0] == '!version':
             MIN_CXXBUILD_VERSION=oplist[1]
@@ -1060,14 +1065,16 @@
                 print("Insufficient CXXBUILD version! Please upgrade!")
                 print("Current version: "+current_version)
                 print("Required version (cxxdeps): "+MIN_CXXBUILD_VERSION)
                 print("Aborting...")
                 exit(1)
         if oplist[0] == '!include':
             INCLUDE_DIRS.append(oplist[1].strip("\""))
+        if oplist[0] == '!ignore':
+            IGNORE.append(op[len(oplist[0]):].strip())
         if oplist[0] == '!define':
             DEFINITIONS.append(op[len(oplist[0]):].strip())
         if oplist[0] == '!extrasrc':
             EXTRA_SOURCES.append(op[len(oplist[0]):].strip())
         if oplist[0] == '!src':
             search_src = oplist[1].strip("\"")
         if oplist[0] == '!tests':
@@ -1097,17 +1104,17 @@
         
     # build system defaults to cmake
     if use_cmake is None:
         use_cmake = True
         use_bazel = False
 
     #
-    return run_build(root_path, use_cmake, use_bazel, cppstd, search_src, search_tests, search_include, INCLUDE_DIRS, DEFINITIONS, EXTRA_SOURCES)
+    return run_build(root_path, use_cmake, use_bazel, cppstd, search_src, search_tests, search_include, INCLUDE_DIRS, DEFINITIONS, EXTRA_SOURCES, IGNORE)
 
-def run_build(root_path, use_cmake, use_bazel, cppstd, search_src, search_tests, search_include, INCLUDE_DIRS, DEFINITIONS, EXTRA_SOURCES):
+def run_build(root_path, use_cmake, use_bazel, cppstd, search_src, search_tests, search_include, INCLUDE_DIRS, DEFINITIONS, EXTRA_SOURCES, IGNORE):
     #
     print("begin build on root_path=",root_path)
     # find all source files,
     # find all files with an entry point,
     src_list = []
     src_main = {}
     # ENFORCING THIS PATH... MUST ADD MULTIPLE PATH OPTION!
@@ -1205,20 +1212,24 @@
         root = root.removeprefix(root_path).removeprefix("/")
         #print("root: ", root)
         #print("subdirs: ", subdirs)
         #print("files: ", files)
         if "include" in subdirs:
             incdir = root+"/"+search_include
             incdir = incdir.removeprefix(root_path).removeprefix("/")
-            # ignore 'build' stuff
-            if incdir[0:6] == 'build/':
-                print("WARNING: 'build/' prefixed folder ignored: ", incdir)
-                pass
-            else:
+            must_ignore=False
+            for ign in IGNORE:
+                # ignore 'build' stuff and others in IGNORE
+                if incdir.startswith(ign):
+                    print("WARNING: '"+ign+"' prefixed folder ignored: ", incdir)
+                    must_ignore=True
+                    break
+            if not must_ignore:
                 INCLUDE_DIRS.append(incdir)
+            # end-for
         # TODO: search in other places too... maybe inside src?
     # keep unique only!
     INCLUDE_DIRS = list(set(INCLUDE_DIRS))
 
     print("INCLUDE_DIRS=",INCLUDE_DIRS)
 
     if use_cmake == True:
```

### Comparing `cxxbuild-1.6.3/cxxbuild.egg-info/PKG-INFO` & `cxxbuild-1.6.4/cxxbuild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cxxbuild
-Version: 1.6.3
+Version: 1.6.4
 Summary: CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!
 Author-email: Igor Machado Coelho <igormcoelho@proton.me>
 License: MIT License
         
         Copyright (c) 2023 manydeps
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -48,15 +48,15 @@
 
 ![C++11](https://img.shields.io/badge/std-c%2B%2B11-blue) ![C++14](https://img.shields.io/badge/std-c%2B%2B14-blue) ![C++17](https://img.shields.io/badge/std-c%2B%2B17-blue) ![C++20](https://img.shields.io/badge/std-c%2B%2B20-blue) ![C++23](https://img.shields.io/badge/std-c%2B%2B23-blue)
 
 [![DOI](https://zenodo.org/badge/715821683.svg)](https://zenodo.org/doi/10.5281/zenodo.10447208)
 
 _**cxxbuild** (or "cplusplusbuild") is a python script to easily generate C/C++ build files for cmake and bazel._
 
-- Version: `cxxbuild version=1.6.3`
+- Version: `cxxbuild version=1.6.4`
 - Installation: `pip install cxxbuild` (or `pipx install cxxbuild` for newer distributions)
 
 For basic introduction, read the post: [Using cxxbuild to easily build C++ project with tests and dependencies](https://igormcoelho.medium.com/using-cxxbuild-to-easily-build-c-project-with-tests-and-dependencies-a3726b453f75)
 
 We know it is very hard to start a C++ project and learn basics of build systems such as CMake and Bazel, and package managers like conan and vcpkg... so just type "cxxbuild" and be happy!
 But you MUST follow the canonical organization below:
 
@@ -199,14 +199,17 @@
 - take system `-lm` dependency
 - C++ standard `c++17` is used
 - build system `cmake` is used
 
 The `git` part could be any package manager, such as conan and vcpkg, although not implemented yet!
 The `git` can be specified for `cmake` or `bazel`, like `cmake+git` or `bazel+git`.
 
+The `local` can be specified for `cmake` or `bazel`, like `cmake+local` or `bazel+local`.
+On `cmake` it represents a `find_package`, while on `bazel` it is a `local_repository` (to implement, yet).
+
 It can also be `bcr`, for the Bazel Central Registry, or more specifically: `bazel+bcr` (not supported for `cmake+bcr`)
 
 ### Ongoing extensions for cxxdeps
 Some ongoing extensions will allow managing dev dependencies, 
 such as build systems (cmake, bazel, etc) and C/C++ package managers (conan, etc), all automatically on `cxxdeps.txt` (or exclusively on `cxxdeps.dev.txt`):
 ```
 cmake == *          [ cmake ]       pip dev [ ninja ]
```

### Comparing `cxxbuild-1.6.3/pyproject.toml` & `cxxbuild-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires=["setuptools", "wheel"]
 build-backend="setuptools.build_meta"
 
 [project]
 name="cxxbuild"
-version="1.6.3"
+version="1.6.4"
 description="CxxBuild is a python script to easily build C++ programs: just invoke 'cxxbuild' and it works!"
 readme="README.md"
 authors=[{ name="Igor Machado Coelho", email="igormcoelho@proton.me" }]
 license={ file="LICENSE" }
 classifiers=[
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

