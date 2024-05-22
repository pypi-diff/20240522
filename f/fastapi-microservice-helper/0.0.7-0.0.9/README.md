# Comparing `tmp/fastapi_microservice_helper-0.0.7.tar.gz` & `tmp/fastapi_microservice_helper-0.0.9.tar.gz`

## Comparing `fastapi_microservice_helper-0.0.7.tar` & `fastapi_microservice_helper-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/build_and_publish.sh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/build_and_test.sh
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/requirements.txt
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/sdk.toml
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/tox.ini
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/sdk/.gitignore
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/sdk/sdk.toml
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/sdk/src/sdk_test_microservice/__init__.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/sdk/src/sdk_test_microservice/sdk.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/__init__.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/base_microservice_client.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/clone_generation.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/code_generation.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/decorator.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/helper.py
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/sdk_builder.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/sdk_template.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/models/generation_detail.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/models/method_detail.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/tests/clone_class_test.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/tests/dto.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/tests/sdk_builder_test.py
--rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/LICENSE
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/README.md
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0      161 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/build_and_publish.sh
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/build_and_test.sh
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/sdk.toml
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/tox.ini
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/sdk/.gitignore
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/sdk/pyproject.toml
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/sdk/src/sdk_test_microservice/__init__.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/sdk/src/sdk_test_microservice/sdk.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/__init__.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/base_microservice_client.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/clone_generation.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/code_generation.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/decorator.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/helper.py
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/sdk_builder.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/sdk_template.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/models/generation_detail.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/models/method_detail.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/tests/clone_class_test.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/tests/dto.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/tests/sdk_builder_test.py
+-rw-r--r--   0        0        0     3285 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/README.md
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 fastapi_microservice_helper-0.0.9/PKG-INFO
```

### Comparing `fastapi_microservice_helper-0.0.7/sdk.toml` & `fastapi_microservice_helper-0.0.9/sdk.toml`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/sdk/.gitignore` & `fastapi_microservice_helper-0.0.9/sdk/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/sdk/sdk.toml` & `fastapi_microservice_helper-0.0.9/sdk/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/sdk/src/sdk_test_microservice/sdk.py` & `fastapi_microservice_helper-0.0.9/sdk/src/sdk_test_microservice/sdk.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     type: TypeEnum=Field(default=TypeEnum.USER)
     
     
 
 from dataclasses import dataclass
 from inspect import isclass
 
-from fastapi import HTTPException
 import httpx
+from fastapi import HTTPException
 from pydantic import BaseModel
 
 
 @dataclass
 class MicroserviceOption:
     is_json: bool = True
     headers: dict = None
```

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/base_microservice_client.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/base_microservice_client.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/clone_generation.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/clone_generation.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/code_generation.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/code_generation.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/decorator.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/decorator.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/helper.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/helper.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/sdk_builder.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/sdk_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 from inspect import getsourcefile
-from shutil import copy, rmtree
+from shutil import copy, rmtree, copyfile
 from typing import Dict
 
 import toml
 from fastapi.routing import APIRoute
 from pydash import group_by
 from ssort import ssort
 from starlette.routing import BaseRoute
@@ -43,22 +43,26 @@
 
     def generate_init_file(self, source_path: str):
         content = 'from .sdk import *'
         with open(os.path.join(source_path, '__init__.py'), "w+") as file:
             file.write(content)
 
     def clone_static_files(self, root_path: str, sdk_path: str):
-        files = ['.gitignore', 'sdk.toml']
+        files = ['.gitignore']
         for file in files:
             file_path = os.path.join(root_path, file)
 
             if not os.path.exists(file_path):
                 raise Exception(f'{file} not exists in root folder.')
             copy(file_path, sdk_path)
 
+        if not os.path.exists(os.path.join(root_path, 'sdk.toml')):
+            raise Exception('sdk.toml not exists in root folder.')
+        copyfile(os.path.join(root_path, 'sdk.toml'), os.path.join(sdk_path, 'pyproject.toml'))
+
     def generate_code(self, name: str, source_path: str, routes: list[BaseRoute]):
         microservices = list()
         for route in routes:
             if isinstance(route, APIRoute):
                 if route.path.startswith('/microservices/'):
                     microservices.append(self.get_api_detail(route))
```

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/sdk_template.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/sdk_template.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/src/fastapi_microservice_helper/models/generation_detail.py` & `fastapi_microservice_helper-0.0.9/src/fastapi_microservice_helper/models/generation_detail.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/tests/dto.py` & `fastapi_microservice_helper-0.0.9/tests/dto.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/tests/sdk_builder_test.py` & `fastapi_microservice_helper-0.0.9/tests/sdk_builder_test.py`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/.gitignore` & `fastapi_microservice_helper-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/LICENSE` & `fastapi_microservice_helper-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/README.md` & `fastapi_microservice_helper-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_microservice_helper-0.0.7/pyproject.toml` & `fastapi_microservice_helper-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fastapi_microservice_helper"
-version = "0.0.7"
+version = "0.0.9"
 authors = [
   { name="Dzung Nguyen", email="dung@megatron-solutions.com" },
 ]
 description = "FastAPI Microservice Helper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fastapi_microservice_helper-0.0.7/PKG-INFO` & `fastapi_microservice_helper-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_microservice_helper
-Version: 0.0.7
+Version: 0.0.9
 Summary: FastAPI Microservice Helper
 Project-URL: Homepage, https://github.com/megatron-global/fastapi-microservice-helper
 Project-URL: Bug Tracker, https://github.com/megatron-global/fastapi-microservice-helper/issues
 Author-email: Dzung Nguyen <dung@megatron-solutions.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

