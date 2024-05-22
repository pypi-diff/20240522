# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1152.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1153.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1152.tar", last modified: Tue May 21 20:40:29 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1153.tar", last modified: Wed May 22 20:44:33 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1153.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2032 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49419 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)    10489 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/hunyuan_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      749 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/README.rst
--rw-r--r--   0 root         (0) root         (0)     1081 2024-05-21 20:40:28.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-21 20:40:29.000000 tencentcloud-sdk-python-hunyuan-3.0.1152/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49460 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)    10489 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      749 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-22 20:44:33.000000 tencentcloud-sdk-python-hunyuan-3.0.1153/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         :param _Temperature: 说明：
 1. 较高的数值会使输出更加随机，而较低的数值会使其更加集中和确定。
 2. 默认 1.0，取值区间为 [0.0, 2.0]。
 3. 非必要不建议使用，不合理的取值会影响效果。
         :type Temperature: float
         :param _EnableEnhancement: 功能增强（如搜索）开关。
 说明：
-1. 仅 hunyuan-pro 模型可用，其它版本不生效。
+1. hunyuan-lite 无功能增强（如搜索）能力，该参数对 hunyuan-lite 版本不生效。
 2. 未传值时默认打开开关。
 3. 关闭时将直接由主模型生成回复内容，可以降低响应时延（对于流式输出时的首字时延尤为明显）。但在少数场景里，回复效果可能会下降。
 4. 安全审核能力不属于功能增强范围，不受此字段影响。
         :type EnableEnhancement: bool
         """
         self._Model = None
         self._Messages = None
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1153/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1152
+Version: 3.0.1153
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1153/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1153/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1152"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1153"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1152/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1153/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1152
+Version: 3.0.1153
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

