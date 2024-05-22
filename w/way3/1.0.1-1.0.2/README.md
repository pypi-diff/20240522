# Comparing `tmp/way3-1.0.1.tar.gz` & `tmp/way3-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way3-1.0.1.tar", last modified: Sun May 19 02:39:46 2024, max compression
+gzip compressed data, was "way3-1.0.2.tar", last modified: Wed May 22 11:53:31 2024, max compression
```

## Comparing `way3-1.0.1.tar` & `way3-1.0.2.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-19 02:39:40.000000 way3-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-19 02:39:46.898268 way3-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-19 02:39:40.000000 way3-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 02:39:46.898268 way3-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-19 02:39:40.000000 way3-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.894268 way3-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:40.000000 way3-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-19 02:39:40.000000 way3-1.0.1/tests/test_file_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-19 02:39:40.000000 way3-1.0.1/tests/test_file_op.py
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-19 02:39:40.000000 way3-1.0.1/tests/test_folder_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.894268 way3-1.0.1/way3/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-19 02:39:40.000000 way3-1.0.1/way3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/way3/file_find/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_find/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_find/current_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_find/traverse_files_from_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/way3/file_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_op/create_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_op/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-19 02:39:40.000000 way3-1.0.1/way3/file_op/read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/way3/folder_op/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:40.000000 way3-1.0.1/way3/folder_op/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-19 02:39:40.000000 way3-1.0.1/way3/folder_op/create_folder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/way3/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:40.000000 way3-1.0.1/way3/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-19 02:39:40.000000 way3-1.0.1/way3/utils/ignore_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 02:39:46.898268 way3-1.0.1/way3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-19 02:39:46.000000 way3-1.0.1/way3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-19 02:39:46.000000 way3-1.0.1/way3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 02:39:46.000000 way3-1.0.1/way3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 02:39:46.000000 way3-1.0.1/way3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.982205 way3-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-22 11:53:25.000000 way3-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-22 11:53:31.982205 way3-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-22 11:53:25.000000 way3-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:53:31.982205 way3-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 11:53:25.000000 way3-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:25.000000 way3-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-22 11:53:25.000000 way3-1.0.2/tests/test_file_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-22 11:53:25.000000 way3-1.0.2/tests/test_file_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-05-22 11:53:25.000000 way3-1.0.2/tests/test_folder_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-22 11:53:25.000000 way3-1.0.2/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/way3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-22 11:53:25.000000 way3-1.0.2/way3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/way3/file_find/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_find/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_find/current_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_find/find_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_find/find_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_find/get_files_from_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/way3/file_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_op/create_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4450 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_op/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 11:53:25.000000 way3-1.0.2/way3/file_op/read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/way3/folder_op/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:25.000000 way3-1.0.2/way3/folder_op/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-22 11:53:25.000000 way3-1.0.2/way3/folder_op/create_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.978204 way3-1.0.2/way3/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:25.000000 way3-1.0.2/way3/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-22 11:53:25.000000 way3-1.0.2/way3/utils/ignore_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-22 11:53:25.000000 way3-1.0.2/way3/utils/os_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:53:31.982205 way3-1.0.2/way3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-22 11:53:31.000000 way3-1.0.2/way3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-22 11:53:31.000000 way3-1.0.2/way3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:53:31.000000 way3-1.0.2/way3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:53:31.000000 way3-1.0.2/way3.egg-info/top_level.txt
```

### Comparing `way3-1.0.1/LICENSE` & `way3-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/PKG-INFO` & `way3-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `way3-1.0.1/README.md` & `way3-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/setup.py` & `way3-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="way3",
-    version="1.0.1",
+    version="1.0.2",
     author="aboutmydreams",
     author_email="aboutmydreams@163.com",
     description="Simplified file path management for Python developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aboutmydreams/way3",
     packages=setuptools.find_packages(),
```

### Comparing `way3-1.0.1/tests/test_file_find.py` & `way3-1.0.2/tests/test_file_find.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/tests/test_file_op.py` & `way3-1.0.2/tests/test_file_op.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/tests/test_folder_op.py` & `way3-1.0.2/tests/test_folder_op.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3/__init__.py` & `way3-1.0.2/way3/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,30 +9,35 @@
 from .file_op.edit import delete_line as delete_line  # noqa: E402
 from .file_op.edit import replace_string_in_line as replace_string_in_line  # noqa: E402
 from .file_op.edit import replace_string_in_file as replace_string_in_file  # noqa: E402
 
 
 # File Find
 from .file_find.current_dir import get_current_dir as get_current_dir  # noqa: E402
-from .file_find.traverse_files_from_folder import parse_gitignore as parse_gitignore  # noqa: E402
-from .file_find.traverse_files_from_folder import is_gitignored as is_gitignored  # noqa: E402
-from .file_find.traverse_files_from_folder import (  # noqa: E402
+from .file_find.get_files_from_folder import parse_gitignore as parse_gitignore  # noqa: E402
+from .file_find.get_files_from_folder import is_gitignored as is_gitignored  # noqa: E402
+from .file_find.get_files_from_folder import (  # noqa: E402
     get_files_in_directory as get_files_in_directory,
 )
-from .file_find.traverse_files_from_folder import (  # noqa: E402
+from .file_find.get_files_from_folder import (  # noqa: E402
     get_directory_structure as get_directory_structure,
 )
-from .file_find.traverse_files_from_folder import (  # noqa: E402
+from .file_find.get_files_from_folder import (  # noqa: E402
     get_directory_folder_list as get_directory_folder_list,
 )
-from .file_find.traverse_files_from_folder import (  # noqa: E402
+from .file_find.get_files_from_folder import (  # noqa: E402
     get_directory_file_list as get_directory_file_list,
 )
+from .file_find.find_files import find_files_by_name as find_files_by_name  # noqa: E402)
+from .file_find.find_folders import find_folders_by_name as find_folders_by_name  # noqa: E402)
 
 # Folder OP
 from .folder_op.create_folder import create_directory as create_directory  # noqa: E402
 from .folder_op.create_folder import rename_directory as rename_directory  # noqa: E402
 from .folder_op.create_folder import delete_directory as delete_directory  # noqa: E402
 
 ## read file
 from .file_op.read import read_file as read_file  # noqa: E402
 from .file_op.read import read_line as read_line  # noqa: E402
+
+# utils
+from .utils.os_tree import tree as tree  # noqa: E402
```

### Comparing `way3-1.0.1/way3/file_find/traverse_files_from_folder.py` & `way3-1.0.2/way3/file_find/get_files_from_folder.py`

 * *Files 17% similar despite different names*

```diff
@@ -45,25 +45,25 @@
     for root, dirs, files in os.walk(path):
         directory_structure[root] = {"dirs": dirs, "files": files}
     return directory_structure
 
 
 def get_directory_folder_list(path) -> List[str]:
     """
-    获取指定路径下的目录结构
+    获取指定路径下的文件夹列表
     :param path: 路径
-    :return: 目录结构
+    :return: 文件夹绝对路径列表
     """
     directory_structure = get_directory_structure(path)
     absolute_path = list(directory_structure.keys())[0]
     return directory_structure[absolute_path]["dirs"]
 
 
 def get_directory_file_list(path) -> List[str]:
     """
-    获取指定路径下的目录结构
+    获取指定路径下的文件列表
     :param path: 路径
-    :return: 目录结构
+    :return: 文件绝对路径列表
     """
     directory_structure = get_directory_structure(path)
     absolute_path = list(directory_structure.keys())[0]
     return directory_structure[absolute_path]["files"]
```

### Comparing `way3-1.0.1/way3/file_op/create_file.py` & `way3-1.0.2/way3/file_op/create_file.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3/file_op/edit.py` & `way3-1.0.2/way3/file_op/edit.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3/file_op/read.py` & `way3-1.0.2/way3/file_op/read.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3/folder_op/create_folder.py` & `way3-1.0.2/way3/folder_op/create_folder.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3/utils/ignore_rule.py` & `way3-1.0.2/way3/utils/ignore_rule.py`

 * *Files identical despite different names*

### Comparing `way3-1.0.1/way3.egg-info/PKG-INFO` & `way3-1.0.2/way3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: way3
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simplified file path management for Python developers
 Home-page: https://github.com/aboutmydreams/way3
 Author: aboutmydreams
 Author-email: aboutmydreams@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `way3-1.0.1/way3.egg-info/SOURCES.txt` & `way3-1.0.2/way3.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 LICENSE
 README.md
 setup.py
 tests/__init__.py
 tests/test_file_find.py
 tests/test_file_op.py
 tests/test_folder_op.py
+tests/test_tree.py
 way3/__init__.py
 way3.egg-info/PKG-INFO
 way3.egg-info/SOURCES.txt
 way3.egg-info/dependency_links.txt
 way3.egg-info/top_level.txt
 way3/file_find/__init__.py
 way3/file_find/current_dir.py
-way3/file_find/traverse_files_from_folder.py
+way3/file_find/find_files.py
+way3/file_find/find_folders.py
+way3/file_find/get_files_from_folder.py
 way3/file_op/__init__.py
 way3/file_op/create_file.py
 way3/file_op/edit.py
 way3/file_op/read.py
 way3/folder_op/__init__.py
 way3/folder_op/create_folder.py
 way3/utils/__init__.py
-way3/utils/ignore_rule.py
+way3/utils/ignore_rule.py
+way3/utils/os_tree.py
```

