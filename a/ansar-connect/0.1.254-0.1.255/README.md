# Comparing `tmp/ansar_connect-0.1.254.tar.gz` & `tmp/ansar_connect-0.1.255.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansar_connect-0.1.254.tar", last modified: Tue May 21 14:08:44 2024, max compression
+gzip compressed data, was "ansar_connect-0.1.255.tar", last modified: Tue May 21 21:33:48 2024, max compression
```

## Comparing `ansar_connect-0.1.254.tar` & `ansar_connect-0.1.255.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.481551 ansar_connect-0.1.254/
--rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.254/LICENSE
--rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-21 14:08:44.481551 ansar_connect-0.1.254/PKG-INFO
--rwxr-xr-x   0 scott     (1000) scott     (1000)      538 2024-05-21 07:49:27.000000 ansar_connect-0.1.254/README.md
--rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-21 14:08:22.000000 ansar_connect-0.1.254/pyproject.toml
--rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-21 14:08:44.481551 ansar_connect-0.1.254/setup.cfg
--rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-21 14:08:13.000000 ansar_connect-0.1.254/setup.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.477551 ansar_connect-0.1.254/src/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.477551 ansar_connect-0.1.254/src/ansar/
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.477551 ansar_connect-0.1.254/src/ansar/command/
--rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.254/src/ansar/command/ansar_command.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.254/src/ansar/command/ansar_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.254/src/ansar/command/ansar_group.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.254/src/ansar/command/shared_directory.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.481551 ansar_connect-0.1.254/src/ansar/connect/
--rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-21 14:08:41.000000 ansar_connect-0.1.254/src/ansar/connect/__init__.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.254/src/ansar/connect/connect_directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.254/src/ansar/connect/directory.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.254/src/ansar/connect/directory_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.254/src/ansar/connect/foh_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.254/src/ansar/connect/group_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.254/src/ansar/connect/grouping.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.254/src/ansar/connect/moving.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.254/src/ansar/connect/networking.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.254/src/ansar/connect/networking_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     9680 2024-05-18 21:34:58.000000 ansar_connect-0.1.254/src/ansar/connect/node.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.254/src/ansar/connect/plumbing.py
--rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.254/src/ansar/connect/procedure.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.254/src/ansar/connect/product.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.254/src/ansar/connect/socketry.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.254/src/ansar/connect/standard.py
--rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.254/src/ansar/connect/transporting.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.254/src/ansar/connect/transporting_if.py
--rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.254/src/ansar/connect/wan.py
-drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 14:08:44.481551 ansar_connect-0.1.254/src/ansar_connect.egg-info/
--rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/PKG-INFO
--rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/SOURCES.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/dependency_links.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/entry_points.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/requires.txt
--rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-21 14:08:44.000000 ansar_connect-0.1.254/src/ansar_connect.egg-info/top_level.txt
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1124 2023-06-30 14:19:32.000000 ansar_connect-0.1.255/LICENSE
+-rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/PKG-INFO
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      538 2024-05-21 07:49:27.000000 ansar_connect-0.1.255/README.md
+-rwxr-xr-x   0 scott     (1000) scott     (1000)      764 2024-05-21 14:08:22.000000 ansar_connect-0.1.255/pyproject.toml
+-rw-rw-r--   0 scott     (1000) scott     (1000)       38 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/setup.cfg
+-rwxr-xr-x   0 scott     (1000) scott     (1000)     2251 2024-05-21 14:08:13.000000 ansar_connect-0.1.255/setup.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.092358 ansar_connect-0.1.255/src/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.092358 ansar_connect-0.1.255/src/ansar/
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/src/ansar/command/
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14549 2024-04-18 02:21:13.000000 ansar_connect-0.1.255/src/ansar/command/ansar_command.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     3497 2024-05-18 00:58:30.000000 ansar_connect-0.1.255/src/ansar/command/ansar_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9940 2024-04-13 00:34:27.000000 ansar_connect-0.1.255/src/ansar/command/ansar_group.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9088 2024-05-18 00:58:30.000000 ansar_connect-0.1.255/src/ansar/command/shared_directory.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/src/ansar/connect/
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     3012 2024-05-21 21:33:44.000000 ansar_connect-0.1.255/src/ansar/connect/__init__.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    14072 2024-04-18 00:04:05.000000 ansar_connect-0.1.255/src/ansar/connect/connect_directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    88788 2024-05-18 21:19:19.000000 ansar_connect-0.1.255/src/ansar/connect/directory.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    12616 2024-05-18 21:27:31.000000 ansar_connect-0.1.255/src/ansar/connect/directory_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    10503 2024-05-19 15:01:15.000000 ansar_connect-0.1.255/src/ansar/connect/foh_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2192 2024-04-18 00:04:05.000000 ansar_connect-0.1.255/src/ansar/connect/group_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    15853 2024-05-20 01:19:54.000000 ansar_connect-0.1.255/src/ansar/connect/grouping.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2221 2024-04-02 20:33:16.000000 ansar_connect-0.1.255/src/ansar/connect/moving.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    23051 2024-05-19 00:29:25.000000 ansar_connect-0.1.255/src/ansar/connect/networking.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1558 2024-03-01 02:40:39.000000 ansar_connect-0.1.255/src/ansar/connect/networking_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     9679 2024-05-21 15:14:21.000000 ansar_connect-0.1.255/src/ansar/connect/node.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2091 2024-03-05 13:29:47.000000 ansar_connect-0.1.255/src/ansar/connect/plumbing.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)    34158 2024-05-20 23:55:13.000000 ansar_connect-0.1.255/src/ansar/connect/procedure.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2397 2024-04-17 22:27:55.000000 ansar_connect-0.1.255/src/ansar/connect/product.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)    42334 2024-05-19 21:19:26.000000 ansar_connect-0.1.255/src/ansar/connect/socketry.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     2159 2024-03-25 00:38:01.000000 ansar_connect-0.1.255/src/ansar/connect/standard.py
+-rwxrwxr-x   0 scott     (1000) scott     (1000)     2804 2024-05-18 21:19:19.000000 ansar_connect-0.1.255/src/ansar/connect/transporting.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1289 2024-04-17 04:02:16.000000 ansar_connect-0.1.255/src/ansar/connect/transporting_if.py
+-rw-rw-r--   0 scott     (1000) scott     (1000)     6602 2024-05-07 01:18:28.000000 ansar_connect-0.1.255/src/ansar/connect/wan.py
+drwxrwxr-x   0 scott     (1000) scott     (1000)        0 2024-05-21 21:33:48.096358 ansar_connect-0.1.255/src/ansar_connect.egg-info/
+-rw-r--r--   0 scott     (1000) scott     (1000)     1303 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/PKG-INFO
+-rw-rw-r--   0 scott     (1000) scott     (1000)     1021 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/SOURCES.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        1 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/dependency_links.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)      212 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/entry_points.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)       48 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/requires.txt
+-rw-rw-r--   0 scott     (1000) scott     (1000)        6 2024-05-21 21:33:48.000000 ansar_connect-0.1.255/src/ansar_connect.egg-info/top_level.txt
```

### Comparing `ansar_connect-0.1.254/LICENSE` & `ansar_connect-0.1.255/LICENSE`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/PKG-INFO` & `ansar_connect-0.1.255/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.254
+Version: 0.1.255
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.254/README.md` & `ansar_connect-0.1.255/README.md`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/pyproject.toml` & `ansar_connect-0.1.255/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/setup.py` & `ansar_connect-0.1.255/setup.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/command/ansar_command.py` & `ansar_connect-0.1.255/src/ansar/command/ansar_command.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/command/ansar_directory.py` & `ansar_connect-0.1.255/src/ansar/command/ansar_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/command/ansar_group.py` & `ansar_connect-0.1.255/src/ansar/command/ansar_group.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/command/shared_directory.py` & `ansar_connect-0.1.255/src/ansar/command/shared_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/__init__.py` & `ansar_connect-0.1.255/src/ansar/connect/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Tools and runtime for asynchronous programming.
 
 Repo: git@github.com:mr-ansar/ansar-connect.git
 Branch: main
-Commit: 471685add068557160d58da74b3483fa6216e184
-Version: 0.1.253 (2024-05-22@02:08:41+NZST)
+Commit: 0189614a9658658a9f2368a4e8fc35e868d53d07
+Version: 0.1.254 (2024-05-22@09:33:44+NZST)
 """
 
 from ansar.create import *
 
 #bind = bind_any
 #create = create_object
```

### Comparing `ansar_connect-0.1.254/src/ansar/connect/connect_directory.py` & `ansar_connect-0.1.255/src/ansar/connect/connect_directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/directory.py` & `ansar_connect-0.1.255/src/ansar/connect/directory.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/directory_if.py` & `ansar_connect-0.1.255/src/ansar/connect/directory_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/foh_if.py` & `ansar_connect-0.1.255/src/ansar/connect/foh_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/group_if.py` & `ansar_connect-0.1.255/src/ansar/connect/group_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/grouping.py` & `ansar_connect-0.1.255/src/ansar/connect/grouping.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/moving.py` & `ansar_connect-0.1.255/src/ansar/connect/moving.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/networking.py` & `ansar_connect-0.1.255/src/ansar/connect/networking.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/networking_if.py` & `ansar_connect-0.1.255/src/ansar/connect/networking_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/node.py` & `ansar_connect-0.1.255/src/ansar/connect/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
 	:type factory_settings: instance of a registered class
 	:param factory_input: per-invocation values
 	:type factory_input: instance of a registered class
 	:param factory_variables: host environment values
 	:type factory_variables: instance of a registered class
 	:param parameter_passing: method for parsing sys.argv[]
 	:type parameter_passing: a function
-	:param parameter_table: table of sub-commands and their association functions
+	:param parameter_table: table of sub-commands and their associated functions
 	:type parameter_table: dict
 	:param upgrade: function that accepts old versions of settings/input and produces the current version
 	:type upgrade: function
 	:param logs: a callable object expecting to receive log objects
 	:type logs: function or class with __call__ method
 	:param scope: level of the internal directory object
 	:type scope: enumeration
```

### Comparing `ansar_connect-0.1.254/src/ansar/connect/plumbing.py` & `ansar_connect-0.1.255/src/ansar/connect/plumbing.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/procedure.py` & `ansar_connect-0.1.255/src/ansar/connect/procedure.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/product.py` & `ansar_connect-0.1.255/src/ansar/connect/product.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/socketry.py` & `ansar_connect-0.1.255/src/ansar/connect/socketry.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/standard.py` & `ansar_connect-0.1.255/src/ansar/connect/standard.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/transporting.py` & `ansar_connect-0.1.255/src/ansar/connect/transporting.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/transporting_if.py` & `ansar_connect-0.1.255/src/ansar/connect/transporting_if.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar/connect/wan.py` & `ansar_connect-0.1.255/src/ansar/connect/wan.py`

 * *Files identical despite different names*

### Comparing `ansar_connect-0.1.254/src/ansar_connect.egg-info/PKG-INFO` & `ansar_connect-0.1.255/src/ansar_connect.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansar-connect
-Version: 0.1.254
+Version: 0.1.255
 Summary: Tools and runtime for asynchronous programming
 Author: Scott Woods
 Author-email: Scott Woods <scott.18.ansar@gmail.com.com>
 Project-URL: Documentation, https://ansar-connect-manual.s3.ap-southeast-2.amazonaws.com/0.1.1/index.html
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ansar_connect-0.1.254/src/ansar_connect.egg-info/SOURCES.txt` & `ansar_connect-0.1.255/src/ansar_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

