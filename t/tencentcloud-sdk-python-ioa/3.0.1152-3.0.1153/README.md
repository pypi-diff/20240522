# Comparing `tmp/tencentcloud-sdk-python-ioa-3.0.1152.tar.gz` & `tmp/tencentcloud-sdk-python-ioa-3.0.1153.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ioa-3.0.1152.tar", last modified: Tue May 21 20:41:46 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ioa-3.0.1153.tar", last modified: Wed May 22 20:47:41 2024, max compression
```

## Comparing `tencentcloud-sdk-python-ioa-3.0.1152.tar` & `tencentcloud-sdk-python-ioa-3.0.1153.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/
--rw-r--r--   0 root         (0) root         (0)     1938 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/ioa_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1272 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    35668 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/models.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-21 20:41:46.000000 tencentcloud-sdk-python-ioa-3.0.1152/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/ioa_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    35668 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/models.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-22 20:47:41.000000 tencentcloud-sdk-python-ioa-3.0.1153/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1152'
+__version__ = '3.0.1153'
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/ioa_client.py` & `tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/ioa_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/errorcodes.py` & `tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud/ioa/v20220601/models.py` & `tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud/ioa/v20220601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/README.rst` & `tencentcloud-sdk-python-ioa-3.0.1153/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/setup.py` & `tencentcloud-sdk-python-ioa-3.0.1153/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-ioa',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1152"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1153"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Ioa SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ioa-3.0.1153/tencentcloud_sdk_python_ioa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ioa
-Version: 3.0.1152
+Version: 3.0.1153
 Summary: Tencent Cloud Ioa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ioa-3.0.1152/PKG-INFO` & `tencentcloud-sdk-python-ioa-3.0.1153/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ioa
-Version: 3.0.1152
+Version: 3.0.1153
 Summary: Tencent Cloud Ioa SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

