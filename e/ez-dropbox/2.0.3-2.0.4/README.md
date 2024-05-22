# Comparing `tmp/ez-dropbox-2.0.3.tar.gz` & `tmp/ez-dropbox-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-dropbox-2.0.3.tar", last modified: Tue May 21 19:45:31 2024, max compression
+gzip compressed data, was "ez-dropbox-2.0.4.tar", last modified: Tue May 21 21:27:57 2024, max compression
```

## Comparing `ez-dropbox-2.0.3.tar` & `ez-dropbox-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:31.001172 ez-dropbox-2.0.3/
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:45:31.000877 ez-dropbox-2.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:30.998294 ez-dropbox-2.0.3/ez_dropbox.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 19:45:30.000000 ez-dropbox-2.0.3/ez_dropbox.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 19:45:30.999749 ez-dropbox-2.0.3/ezdbx/
--rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.3/ezdbx/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20426 2024-05-21 19:44:39.000000 ez-dropbox-2.0.3/ezdbx/main.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 19:45:31.001367 ez-dropbox-2.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 19:44:49.000000 ez-dropbox-2.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:27:57.644619 ez-dropbox-2.0.4/
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-12 12:48:02.000000 ez-dropbox-2.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 21:27:57.644322 ez-dropbox-2.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-05-21 19:09:21.000000 ez-dropbox-2.0.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:27:57.641677 ez-dropbox-2.0.4/ez_dropbox.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5000 2024-05-21 21:27:57.000000 ez-dropbox-2.0.4/ez_dropbox.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-21 21:27:57.000000 ez-dropbox-2.0.4/ez_dropbox.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 21:27:57.000000 ez-dropbox-2.0.4/ez_dropbox.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-21 21:27:57.000000 ez-dropbox-2.0.4/ez_dropbox.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-21 21:27:57.000000 ez-dropbox-2.0.4/ez_dropbox.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 21:27:57.643269 ez-dropbox-2.0.4/ezdbx/
+-rw-r--r--   0 root         (0) root         (0)      117 2024-05-12 12:48:02.000000 ez-dropbox-2.0.4/ezdbx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21673 2024-05-21 21:26:41.000000 ez-dropbox-2.0.4/ezdbx/main.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 21:27:57.644876 ez-dropbox-2.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-21 21:27:26.000000 ez-dropbox-2.0.4/setup.py
```

### Comparing `ez-dropbox-2.0.3/LICENSE` & `ez-dropbox-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.3/PKG-INFO` & `ez-dropbox-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.3
+Version: 2.0.4
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.3/README.md` & `ez-dropbox-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ez-dropbox-2.0.3/ez_dropbox.egg-info/PKG-INFO` & `ez-dropbox-2.0.4/ez_dropbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-dropbox
-Version: 2.0.3
+Version: 2.0.4
 Summary: You can easily operate Dropbox!
 Home-page: https://github.com/TorDataScientist/ez-dropbox
 Author: TorDataScientist
 License: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ez-dropbox-2.0.3/ezdbx/main.py` & `ez-dropbox-2.0.4/ezdbx/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,15 +202,17 @@
             try:
                 local_mod_time = datetime.fromtimestamp(os.path.getmtime(local_file))
             except OSError:
                 local_mod_time = None
 
             if dropbox_path in dropbox_files:
                 dropbox_mod_time = dropbox_files[dropbox_path]
-                if local_mod_time > dropbox_mod_time:
+                if abs((local_mod_time - dropbox_mod_time).total_seconds()) < 2:
+                    print(f'Local file and Dropbox file are identical: {local_file}')
+                elif local_mod_time > dropbox_mod_time:
                     self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
             else:
                 if local_mod_time is None:
                     self._handle_unsupported_file(local_file, dropbox_path)
                 else:
                     self.upload(local_file, os.path.dirname(dropbox_path), overwrite=True)
 
@@ -234,14 +236,37 @@
             if not os.path.exists(local_path):
                 self.download_file(dropbox_path, local_path)
             else:
                 local_mod_time = datetime.fromtimestamp(os.path.getmtime(local_path))
                 if local_mod_time < dropbox_mod_time:
                     self.download_file(dropbox_path, local_path)
 
+    def cleanup_local_files(self, local_folder, dropbox_folder):
+        """
+        保存に成功したファイルをローカルから削除します。
+        """
+        # ローカルファイルリストの取得
+        local_files = self._list_local_files(local_folder)
+        
+        # Dropbox内のファイルリストの取得
+        dropbox_files, _ = self._list_dropbox_files_and_folders(dropbox_folder, 'file')
+
+        # ローカルファイルリストとDropboxファイルリストの差分を取得
+        for local_file in local_files:
+            relative_path = os.path.relpath(local_file, local_folder)
+            dropbox_path = os.path.join(dropbox_folder, relative_path)
+            dropbox_path = os.path.normpath(dropbox_path)
+            
+            if dropbox_path in dropbox_files:
+                try:
+                    os.remove(local_file)
+                    print(f'{local_file} was successfully deleted from local storage.')
+                except Exception as e:
+                    print(f'Error deleting {local_file}: {e}')
+
     def check_exists(self, file_path):
         """
         指定したファイルまたはフォルダが存在するかを確認します。
         :param file_path: ファイルまたはフォルダのパス
         :return: 存在する場合はTrue、存在しない場合はFalse
         """
         return self._check_file_exists(file_path)
```

### Comparing `ez-dropbox-2.0.3/setup.py` & `ez-dropbox-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 packages = [
     'ezdbx'
 ]
 
 setup(
     name='ez-dropbox',
-    version='2.0.3',
+    version='2.0.4',
     license="MIT License",
     description="You can easily operate Dropbox!",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='TorDataScientist',
     url='https://github.com/TorDataScientist/ez-dropbox',
     packages=packages,
```

