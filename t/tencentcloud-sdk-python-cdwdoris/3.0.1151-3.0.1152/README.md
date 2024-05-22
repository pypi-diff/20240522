# Comparing `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1151.tar.gz` & `tmp/tencentcloud-sdk-python-cdwdoris-3.0.1152.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1151.tar", last modified: Mon May 20 20:25:21 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdwdoris-3.0.1152.tar", last modified: Tue May 21 20:28:10 2024, max compression
```

## Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151.tar` & `tencentcloud-sdk-python-cdwdoris-3.0.1152.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/
--rw-r--r--   0 root         (0) root         (0)    16479 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/__init__.py
--rw-r--r--   0 root         (0) root         (0)      703 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   132125 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      752 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/README.rst
--rw-r--r--   0 root         (0) root         (0)     1083 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1685 2024-05-20 20:25:21.000000 tencentcloud-sdk-python-cdwdoris-3.0.1151/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/
+-rw-r--r--   0 root         (0) root         (0)    16479 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      703 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   132125 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      752 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1083 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1685 2024-05-21 20:28:10.000000 tencentcloud-sdk-python-cdwdoris-3.0.1152/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1151'
+__version__ = '3.0.1152'
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/cdwdoris_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/errorcodes.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud/cdwdoris/v20211228/models.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud/cdwdoris/v20211228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/tencentcloud_sdk_python_cdwdoris.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1151
+Version: 3.0.1152
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/README.rst` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/setup.py` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-cdwdoris',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1151"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1152"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Cdwdoris SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-cdwdoris-3.0.1151/PKG-INFO` & `tencentcloud-sdk-python-cdwdoris-3.0.1152/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdwdoris
-Version: 3.0.1151
+Version: 3.0.1152
 Summary: Tencent Cloud Cdwdoris SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

