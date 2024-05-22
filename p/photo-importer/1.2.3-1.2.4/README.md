# Comparing `tmp/photo-importer-1.2.3.tar.gz` & `tmp/photo-importer-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "photo-importer-1.2.3.tar", last modified: Tue Apr 23 22:01:53 2024, max compression
+gzip compressed data, was "photo-importer-1.2.4.tar", last modified: Wed May 22 21:26:16 2024, max compression
```

## Comparing `photo-importer-1.2.3.tar` & `photo-importer-1.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:01:53.447000 photo-importer-1.2.3/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    35147 2018-05-05 16:37:35.000000 photo-importer-1.2.3/LICENSE
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     5040 2024-04-23 22:01:53.447000 photo-importer-1.2.3/PKG-INFO
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     3923 2024-04-23 21:48:31.000000 photo-importer-1.2.3/README.md
--rwxr-xr-x   0 sashacmc  (1000) sashacmc  (1000)       74 2019-11-27 19:11:35.000000 photo-importer-1.2.3/photo-importer
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)       80 2023-05-25 18:31:39.000000 photo-importer-1.2.3/photo-importer-server
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1496 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo-importer.cfg
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      255 2023-05-25 18:31:39.000000 photo-importer-1.2.3/photo-importer.service
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:01:53.443000 photo-importer-1.2.3/photo_importer/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        0 2020-05-29 10:50:44.000000 photo-importer-1.2.3/photo_importer/__init__.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2273 2024-04-23 21:32:32.000000 photo-importer-1.2.3/photo_importer/config.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     6833 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/fileprop.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5641 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/fileprop_test.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3228 2024-04-23 21:32:32.000000 photo-importer-1.2.3/photo_importer/importer.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1932 2023-05-25 19:12:11.000000 photo-importer-1.2.3/photo_importer/importer_test.py
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1493 2023-05-25 18:31:39.000000 photo-importer-1.2.3/photo_importer/log.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4651 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/mover.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4740 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/rotator.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2694 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/run.py
--rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15047 2023-05-12 15:44:26.000000 photo-importer-1.2.3/photo_importer/server.py
--rwxr-xr-x   0 sashacmc  (1000) sashacmc  (1000)      525 2020-05-29 10:50:44.000000 photo-importer-1.2.3/photo_importer/test.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:01:53.447000 photo-importer-1.2.3/photo_importer.egg-info/
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)     5040 2024-04-23 22:01:53.000000 photo-importer-1.2.3/photo_importer.egg-info/PKG-INFO
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)      670 2024-04-23 22:01:53.000000 photo-importer-1.2.3/photo_importer.egg-info/SOURCES.txt
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-04-23 22:01:53.000000 photo-importer-1.2.3/photo_importer.egg-info/dependency_links.txt
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        1 2019-11-27 19:12:43.000000 photo-importer-1.2.3/photo_importer.egg-info/not-zip-safe
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)       30 2024-04-23 22:01:53.000000 photo-importer-1.2.3/photo_importer.egg-info/requires.txt
--rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-04-23 22:01:53.000000 photo-importer-1.2.3/photo_importer.egg-info/top_level.txt
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-04-23 22:01:53.447000 photo-importer-1.2.3/setup.cfg
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1856 2024-04-23 21:32:32.000000 photo-importer-1.2.3/setup.py
-drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-04-23 22:01:53.447000 photo-importer-1.2.3/web/
--rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     7665 2023-05-12 15:44:26.000000 photo-importer-1.2.3/web/index.html
--r--r--r--   0 sashacmc  (1000) sashacmc  (1000)     1107 2019-01-27 00:13:21.000000 photo-importer-1.2.3/web/log.png
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-22 21:26:16.367552 photo-importer-1.2.4/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)    35147 2018-05-05 16:37:35.000000 photo-importer-1.2.4/LICENSE
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     5040 2024-05-22 21:26:16.363552 photo-importer-1.2.4/PKG-INFO
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     3923 2024-04-23 21:48:31.000000 photo-importer-1.2.4/README.md
+-rwxr-xr-x   0 sashacmc  (1000) sashacmc  (1000)       74 2019-11-27 19:11:35.000000 photo-importer-1.2.4/photo-importer
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)       80 2023-05-25 18:31:39.000000 photo-importer-1.2.4/photo-importer-server
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1666 2024-05-22 17:41:04.000000 photo-importer-1.2.4/photo-importer.cfg
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)      255 2023-05-25 18:31:39.000000 photo-importer-1.2.4/photo-importer.service
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-22 21:26:16.363552 photo-importer-1.2.4/photo_importer/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        0 2020-05-29 10:50:44.000000 photo-importer-1.2.4/photo_importer/__init__.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2302 2024-05-22 17:41:16.000000 photo-importer-1.2.4/photo_importer/config.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     7006 2024-05-22 17:41:47.000000 photo-importer-1.2.4/photo_importer/fileprop.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     5641 2023-05-12 15:44:26.000000 photo-importer-1.2.4/photo_importer/fileprop_test.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     3228 2024-04-23 21:32:32.000000 photo-importer-1.2.4/photo_importer/importer.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     1932 2023-05-25 19:12:11.000000 photo-importer-1.2.4/photo_importer/importer_test.py
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1493 2023-05-25 18:31:39.000000 photo-importer-1.2.4/photo_importer/log.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4651 2023-05-12 15:44:26.000000 photo-importer-1.2.4/photo_importer/mover.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     4740 2023-05-12 15:44:26.000000 photo-importer-1.2.4/photo_importer/rotator.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)     2694 2023-05-12 15:44:26.000000 photo-importer-1.2.4/photo_importer/run.py
+-rwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)    15047 2023-05-12 15:44:26.000000 photo-importer-1.2.4/photo_importer/server.py
+-rwxr-xr-x   0 sashacmc  (1000) sashacmc  (1000)      525 2020-05-29 10:50:44.000000 photo-importer-1.2.4/photo_importer/test.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-22 21:26:16.363552 photo-importer-1.2.4/photo_importer.egg-info/
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)     5040 2024-05-22 21:26:15.000000 photo-importer-1.2.4/photo_importer.egg-info/PKG-INFO
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)      670 2024-05-22 21:26:16.000000 photo-importer-1.2.4/photo_importer.egg-info/SOURCES.txt
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        1 2024-05-22 21:26:15.000000 photo-importer-1.2.4/photo_importer.egg-info/dependency_links.txt
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)        1 2019-11-27 19:12:43.000000 photo-importer-1.2.4/photo_importer.egg-info/not-zip-safe
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)       30 2024-05-22 21:26:15.000000 photo-importer-1.2.4/photo_importer.egg-info/requires.txt
+-rw-r--r--   0 sashacmc  (1000) sashacmc  (1000)       15 2024-05-22 21:26:15.000000 photo-importer-1.2.4/photo_importer.egg-info/top_level.txt
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)       38 2024-05-22 21:26:16.367552 photo-importer-1.2.4/setup.cfg
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     1842 2024-05-22 17:43:31.000000 photo-importer-1.2.4/setup.py
+drwxrwxr-x   0 sashacmc  (1000) sashacmc  (1000)        0 2024-05-22 21:26:16.363552 photo-importer-1.2.4/web/
+-rw-rw-r--   0 sashacmc  (1000) sashacmc  (1000)     7665 2023-05-12 15:44:26.000000 photo-importer-1.2.4/web/index.html
+-r--r--r--   0 sashacmc  (1000) sashacmc  (1000)     1107 2019-01-27 00:13:21.000000 photo-importer-1.2.4/web/log.png
```

### Comparing `photo-importer-1.2.3/LICENSE` & `photo-importer-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/PKG-INFO` & `photo-importer-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-importer
-Version: 1.2.3
+Version: 1.2.4
 Summary: Photo importer tool
 Home-page: https://github.com/sashacmc/photo-importer
 Author: Alexander Bushnev
 Author-email: Alexander@Bushnev.pro
 License: GNU General Public License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `photo-importer-1.2.3/README.md` & `photo-importer-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo-importer.cfg` & `photo-importer-1.2.4/photo-importer.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,19 @@
 # Use shutil libarary in place of system calls (bool, 0/1)
 # slower but provide more cross platform compatibility
 use_shutil = 0
 
 # Add original filename, if it does not contain a timestamp (bool, 0/1)
 # (Useful if filename contains some notable information)
 add_orig_name = 0
-            
+
+# This time shift (in seconds) will be added to the original timestamp during renaming
+# (useful if original file have a wrong timestamp, timestamp will no affected)
+time_shift = 0
+
 [server]            
 # Server port
 port = 8080
 
 # Path to html files
 web_path = /usr/share/photo-importer/web/
```

### Comparing `photo-importer-1.2.3/photo_importer/config.py` & `photo-importer-1.2.4/photo_importer/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             'remove_empty_dirs': 1,
             'move_mode': 1,
             'threads_count': 2,
             'umask': '0o000',
             'use_jpegtran': 0,
             'use_shutil': 0,
             'add_orig_name': 0,
+            'time_shift': 0,
         },
         'server': {
             'port': 8080,
             'web_path': 'web',
             'out_path': '/mnt/multimedia/NEW/',
             'in_path': '',
             'log_file': 'photo-importer-server.log',
```

### Comparing `photo-importer-1.2.3/photo_importer/fileprop.py` & `photo-importer-1.2.4/photo_importer/fileprop.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 ext = '.' + ext.lower()
                 if ext in self.EXT_TO_TYPE:
                     logging.fatal('Double ext: ' + ext)
                 self.EXT_TO_TYPE[ext] = tp
 
     def __type_by_ext(self, ext):
         try:
-            return self.EXT_TO_TYPE[ext.lower()]
+            return self.EXT_TO_TYPE[ext]
         except KeyError:
             logging.warning('Unknown ext: ' + ext)
             return IGNORE
 
     def __time(self, fullname, name, tp):
         if tp not in (IMAGE, VIDEO, AUDIO):
             return None
@@ -178,18 +178,22 @@
         self.__out_list.add(res)
 
         return res
 
     def get(self, fullname):
         path, fname_ext = os.path.split(fullname)
         fname, ext = os.path.splitext(fname_ext)
+        ext = ext.lower()
 
         tp = self.__type_by_ext(ext)
 
         ftime = self.__time(fullname, fname, tp)
+        time_shift = self.__config['main']['time_shift']
+        if ftime and time_shift:
+            ftime += datetime.timedelta(seconds=int(time_shift))
 
         if ftime:
             out_name = ftime.strftime(
                 self.__config['main']['out_time_format']
             ) + self.__calc_orig_name(fname)
         else:
             out_name = None
```

### Comparing `photo-importer-1.2.3/photo_importer/fileprop_test.py` & `photo-importer-1.2.4/photo_importer/fileprop_test.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/importer.py` & `photo-importer-1.2.4/photo_importer/importer.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/importer_test.py` & `photo-importer-1.2.4/photo_importer/importer_test.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/log.py` & `photo-importer-1.2.4/photo_importer/log.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/mover.py` & `photo-importer-1.2.4/photo_importer/mover.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/rotator.py` & `photo-importer-1.2.4/photo_importer/rotator.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/run.py` & `photo-importer-1.2.4/photo_importer/run.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/server.py` & `photo-importer-1.2.4/photo_importer/server.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer/test.py` & `photo-importer-1.2.4/photo_importer/test.py`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/photo_importer.egg-info/PKG-INFO` & `photo-importer-1.2.4/photo_importer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photo-importer
-Version: 1.2.3
+Version: 1.2.4
 Summary: Photo importer tool
 Home-page: https://github.com/sashacmc/photo-importer
 Author: Alexander Bushnev
 Author-email: Alexander@Bushnev.pro
 License: GNU General Public License v3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `photo-importer-1.2.3/photo_importer.egg-info/SOURCES.txt` & `photo-importer-1.2.4/photo_importer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/setup.py` & `photo-importer-1.2.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup
 import os
 
 
 def get_long_description():
     this_directory = os.path.abspath(os.path.dirname(__file__))
-    with open(
-        os.path.join(this_directory, 'README.md'), encoding='utf-8'
-    ) as f:
+    with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
         long_description = f.read()
 
     return long_description
 
 
 setup(
     name='photo-importer',
-    version='1.2.3',
+    version='1.2.4',
     description='Photo importer tool',
     author='Alexander Bushnev',
     author_email='Alexander@Bushnev.pro',
     license='GNU General Public License v3.0',
     packages=['photo_importer'],
     data_files=[
         ('/etc/', ['photo-importer.cfg']),
```

### Comparing `photo-importer-1.2.3/web/index.html` & `photo-importer-1.2.4/web/index.html`

 * *Files identical despite different names*

### Comparing `photo-importer-1.2.3/web/log.png` & `photo-importer-1.2.4/web/log.png`

 * *Files identical despite different names*

