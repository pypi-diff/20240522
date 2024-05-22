# Comparing `tmp/fast_multi_regex-0.8.tar.gz` & `tmp/fast_multi_regex-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_multi_regex-0.8.tar", last modified: Sun May 19 16:43:07 2024, max compression
+gzip compressed data, was "fast_multi_regex-0.9.tar", last modified: Mon May 20 05:02:58 2024, max compression
```

## Comparing `fast_multi_regex-0.8.tar` & `fast_multi_regex-0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.562597 fast_multi_regex-0.8/
--rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.8/LICENSE
--rwxrwxrwx   0     1024 users      (100)     2320 2024-05-19 16:43:07.561597 fast_multi_regex-0.8/PKG-INFO
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.542597 fast_multi_regex-0.8/fast_multi_regex/
--rwxrwxrwx   0     1024 users      (100)      541 2024-05-19 11:29:13.000000 fast_multi_regex-0.8/fast_multi_regex/__init__.py
--rwxrwxrwx   0     1024 users      (100)     6358 2024-05-19 16:41:29.000000 fast_multi_regex-0.8/fast_multi_regex/api.py
--rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.8/fast_multi_regex/api_types.py
--rwxrwxrwx   0     1024 users      (100)    39019 2024-05-19 16:27:18.000000 fast_multi_regex-0.8/fast_multi_regex/matcher.py
--rwxrwxrwx   0     1024 users      (100)     3194 2024-05-19 11:28:53.000000 fast_multi_regex-0.8/fast_multi_regex/server.py
--rwxrwxrwx   0     1024 users      (100)    11603 2024-05-19 14:35:20.000000 fast_multi_regex-0.8/fast_multi_regex/utils.py
-drwxrwxrwx   0     1024 users      (100)        0 2024-05-19 16:43:07.558597 fast_multi_regex-0.8/fast_multi_regex.egg-info/
--rwxrwxrwx   0     1024 users      (100)     2320 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/PKG-INFO
--rwxrwxrwx   0     1024 users      (100)      422 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/SOURCES.txt
--rwxrwxrwx   0     1024 users      (100)        1 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/dependency_links.txt
--rwxrwxrwx   0     1024 users      (100)       79 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/entry_points.txt
--rwxrwxrwx   0     1024 users      (100)       76 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/requires.txt
--rwxrwxrwx   0     1024 users      (100)       17 2024-05-19 16:43:07.000000 fast_multi_regex-0.8/fast_multi_regex.egg-info/top_level.txt
--rwxrwxrwx   0     1024 users      (100)       38 2024-05-19 16:43:07.563597 fast_multi_regex-0.8/setup.cfg
--rwxrwxrwx   0     1024 users      (100)     1300 2024-05-19 16:42:33.000000 fast_multi_regex-0.8/setup.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-20 05:02:58.313359 fast_multi_regex-0.9/
+-rwxrwxrwx   0     1024 users      (100)    35149 2024-05-17 08:41:36.000000 fast_multi_regex-0.9/LICENSE
+-rwxrwxrwx   0     1024 users      (100)     2618 2024-05-20 05:02:58.312358 fast_multi_regex-0.9/PKG-INFO
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-20 05:02:58.294358 fast_multi_regex-0.9/fast_multi_regex/
+-rwxrwxrwx   0     1024 users      (100)      581 2024-05-20 04:44:42.000000 fast_multi_regex-0.9/fast_multi_regex/__init__.py
+-rwxrwxrwx   0     1024 users      (100)     6358 2024-05-19 16:41:29.000000 fast_multi_regex-0.9/fast_multi_regex/api.py
+-rwxrwxrwx   0     1024 users      (100)     3166 2024-05-19 11:43:21.000000 fast_multi_regex-0.9/fast_multi_regex/api_types.py
+-rwxrwxrwx   0     1024 users      (100)    39059 2024-05-20 05:00:59.000000 fast_multi_regex-0.9/fast_multi_regex/matcher.py
+-rwxrwxrwx   0     1024 users      (100)     3194 2024-05-20 05:01:24.000000 fast_multi_regex-0.9/fast_multi_regex/server.py
+-rwxrwxrwx   0     1024 users      (100)    13491 2024-05-20 04:59:01.000000 fast_multi_regex-0.9/fast_multi_regex/utils.py
+drwxrwxrwx   0     1024 users      (100)        0 2024-05-20 05:02:58.309358 fast_multi_regex-0.9/fast_multi_regex.egg-info/
+-rwxrwxrwx   0     1024 users      (100)     2618 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/PKG-INFO
+-rwxrwxrwx   0     1024 users      (100)      422 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1024 users      (100)        1 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1024 users      (100)       79 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/entry_points.txt
+-rwxrwxrwx   0     1024 users      (100)       76 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/requires.txt
+-rwxrwxrwx   0     1024 users      (100)       17 2024-05-20 05:02:58.000000 fast_multi_regex-0.9/fast_multi_regex.egg-info/top_level.txt
+-rwxrwxrwx   0     1024 users      (100)       38 2024-05-20 05:02:58.313359 fast_multi_regex-0.9/setup.cfg
+-rwxrwxrwx   0     1024 users      (100)     1300 2024-05-20 04:59:51.000000 fast_multi_regex-0.9/setup.py
```

### Comparing `fast_multi_regex-0.8/LICENSE` & `fast_multi_regex-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.8/PKG-INFO` & `fast_multi_regex-0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_multi_regex
-Version: 0.8
+Version: 0.9
 Summary: Fast multi-regex, multi-pattern, boolean expression matching
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,26 +22,33 @@
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
 
-构建正则库，matchers_config_folder 内 json 文件例子（参考 OneTarget 格式和 file_processor_matchers_update 方法解析）：
+构建正则库，即增删改 matchers_config_folder 中的 json 文件（允许子文件夹嵌套），例子（参考 matcher_config_example）：
 ```json
 {
     "cache_size": 128,
     "literal": false,
     "targets": [
         {
-            "mark": "test",
+            "mark": "example",
             "regexs": [
                 {
-                    "expression": "test",
+                    "expression": "例子",
                     "flag": 40,
+                    "flag_ext": {
+                        "min_offset": null,
+                        "max_offset": null,
+                        "min_length": null,
+                        "edit_distance": null,
+                        "hamming_distance": null
+                    },
                     "min_match_count": 1,
                     "max_match_count": 0
                 }
             ],
             "min_regex_count": 1,
             "max_regex_count": 0,
             "bool_expr": "",
```

### Comparing `fast_multi_regex-0.8/fast_multi_regex/__init__.py` & `fast_multi_regex-0.9/fast_multi_regex/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 from .utils import (
     load_matchers,
     DelayedFilesHandler,
     file_processor_matchers_update,
     update_matchers_folder,
     async_request,
     sync_request,
+    matcher_config_example,
 )
 from .api_types import (
     OneMatch,
     OneMatchMark,
     OneQuery,
     BodyMatch,
     RespMatch,
     RespInfo,
     BodyTargets,
     RespTargets,
     BodyFindExpression,
     RespFindExpression,
 )
 from .api import app
-from .server import app_server
+from .server import app_server, log_config
```

### Comparing `fast_multi_regex-0.8/fast_multi_regex/api.py` & `fast_multi_regex-0.9/fast_multi_regex/api.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.8/fast_multi_regex/api_types.py` & `fast_multi_regex-0.9/fast_multi_regex/api_types.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.8/fast_multi_regex/matcher.py` & `fast_multi_regex-0.9/fast_multi_regex/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,19 +162,19 @@
         self._db = hyperscan.loadb(state['_db'], hyperscan.HS_MODE_BLOCK)
         self._db.scratch = hyperscan.Scratch(self._db)
         self._mark_bool_info = mark_bool_info
         for k, v in state['serializable_var'].items():
             setattr(self, k, v)
         self.reset_cache()
     
-    def reset_cache(self, cache_size: int = None) -> bool:
+    def reset_cache(self, cache_size: Optional[int] = None) -> bool:
         """重置缓存
 
         Args:
-            cache_size (int, optional): 修改后的缓存大小. 为 None、小于等于0不使用缓存
+            cache_size (int, optional): 修改后的缓存大小. 为 None/小于0 不修改原始缓存大小，等于0不使用缓存
 
         Returns:
             bool: 是否修改成功
         """
         reset_success = False
         if cache_size is not None and cache_size >= 0:
             self._info.cache_size = cache_size
```

### Comparing `fast_multi_regex-0.8/fast_multi_regex/server.py` & `fast_multi_regex-0.9/fast_multi_regex/server.py`

 * *Files identical despite different names*

### Comparing `fast_multi_regex-0.8/fast_multi_regex/utils.py` & `fast_multi_regex-0.9/fast_multi_regex/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,29 @@
 from pydantic import BaseModel
 import aiohttp
 import logging
 import asyncio
 import requests
 import time
 import json
-from .matcher import MultiRegexMatcher
+from .matcher import MultiRegexMatcher, FlagExt, OneRegex, OneTarget
+
+
+def model_to_dict(model: Optional[Union[BaseModel, dict]], **kwargs) -> dict:
+    """
+    Convert a Pydantic model to a dictionary, compatible with both Pydantic 1.x and 2.x.
+    """
+    if isinstance(model, (dict, type(None))):
+        return model
+    try:
+        # Try using Pydantic 2.x method
+        return model.model_dump(**kwargs)
+    except AttributeError:
+        # Fallback to Pydantic 1.x method
+        return model.dict(**kwargs)
 
 
 def load_matchers(folder: str) -> dict[str, MultiRegexMatcher]:
     """递归加载文件夹中的所有 MultiRegexMatcher pkl 文件
 
     Args:
         folder (str): 主文件夹路径
@@ -135,61 +149,99 @@
     pkl_path = os.path.join(matchers_folder, f'{name}.pkl')
     success = False
     if opt == 'modified' or opt == 'created':
         with open(path, 'r', encoding='utf-8') as f:
             config: dict = json.load(f)
         if not config.get('targets'):
             return None
-        cache_size = config.get('cache_size', 128)
+        cache_size = config.get('cache_size')
         literal = config.get('literal', False)
         if name in matchers:
             success |= matchers[name].compile(config['targets'], literal=literal)
-            if cache_size != matchers[name].info.cache_size:
+            if cache_size is not None and cache_size != matchers[name].info.cache_size:
                 matchers[name].reset_cache(cache_size)
                 success = True
         else:
-            matchers[name] = MultiRegexMatcher(cache_size)
+            matchers[name] = MultiRegexMatcher()
             matchers[name].compile(config['targets'], literal=literal)
+            matchers[name].reset_cache(cache_size)
             success = True
         if success:
             os.makedirs(os.path.dirname(pkl_path), exist_ok=True)
             with open(pkl_path, 'wb') as f:
                 pickle.dump(matchers[name], f)
     elif opt == 'deleted':
         matchers.pop(name, None)
         if os.path.exists(pkl_path):
             os.remove(pkl_path)
             success = True
     if success:
         return f'file_processor_matchers_update: "{name}" {opt}'
 
 
+matcher_config_example = {
+    "cache_size": 128,  # 缓存大小
+    "literal": False,  # 是否使用字面量匹配（正则当作普通字符匹配）
+    "targets": [
+        model_to_dict(OneTarget(
+            mark="example",  # 正则组名称，不能重复
+            regexs=[OneRegex(
+                expression='例子',  # 正则
+                flag_ext=FlagExt(),
+            )],
+        )),
+    ]
+}
+
+
 def update_matchers_folder(
     matchers_folder: str,
     matchers_config_folder: str,
     delay: int = 30,
     create_folder: bool = True,
     blocking: bool = False,
+    default_matcher_config: dict = matcher_config_example,
 ) -> dict[str, MultiRegexMatcher]:
     """初始化 matchers 文件夹，创建 DelayedFilesHandler 监控配置文件夹, 根据配置变动实时更新 matchers 文件夹
 
     Args:
         matchers_folder (str): 匹配器保存的文件夹
         matchers_config_folder (str): 匹配器配置文件夹，将自动把配置文件转换为匹配器
         delay (int, optional): 配置文件这么多秒后不再修改才会更新到匹配器文件夹
         create_folder (bool, optional): 是否自动创建文件夹
         blocking (bool, optional): 是否阻塞
+        default_matcher_config (dict, optional): 默认配置, 当没有匹配器时且有这个变量会自动写入这个 default.json
 
     Returns:
         dict[str, MultiRegexMatcher]: 加载的 matchers
     """
     if create_folder:
         os.makedirs(matchers_folder, exist_ok=True)
         os.makedirs(matchers_config_folder, exist_ok=True)
     matchers = load_matchers(matchers_folder)
+    
+    # 写入默认配置
+    default_json = os.path.join(matchers_config_folder, 'default.json')
+    if (
+        not matchers and 
+        default_matcher_config and 
+        default_matcher_config.get('targets')
+    ):
+        matchers['default'] = MultiRegexMatcher()
+        matchers['default'].compile(
+            default_matcher_config['targets'],
+            literal=default_matcher_config.get('literal', False),
+        )
+        matchers['default'].reset_cache(default_matcher_config.get('cache_size'))
+        with open(default_json, 'w', encoding='utf-8') as f:
+            json.dump(default_matcher_config, f, ensure_ascii=False, indent=4)
+        with open(os.path.join(matchers_folder, 'default.pkl'), 'wb') as f:
+            pickle.dump(matchers['default'], f)
+    
+    # 监控配置文件夹
     print('file_processor_matchers_update: init matchers:', list(matchers))
     obj = DelayedFilesHandler(
         matchers_config_folder, 
         file_handler=file_processor_matchers_update,
         context={
             'matchers_folder': matchers_folder,
             'matchers_config_folder': matchers_config_folder,
@@ -227,15 +279,15 @@
         kwargs (dict): 其他 session 支持的参数
 
     Returns:
         dict: 请求结果
             message (str): 返回信息
             status (int): 状态码
     """
-    body = body if isinstance(body, (dict, type(None))) else dict(body)
+    body = model_to_dict(body)
     if token:
         if not headers:
             headers = {'Content-Type': 'application/json'}
         headers['Authorization'] = f'Bearer {token}'
     for i in range(try_times):
         try:
             async with aiohttp.ClientSession() as session:
@@ -281,15 +333,15 @@
         kwargs (dict): 其他 session 支持的参数，例如 timeout
 
     Returns:
         dict: 请求结果
             message (str): 返回信息
             status (int): 状态码
     """
-    body = body if isinstance(body, (dict, type(None))) else dict(body)
+    body = model_to_dict(body)
     if token:
         if not headers:
             headers = {'Content-Type': 'application/json'}
         headers['Authorization'] = f'Bearer {token}'
     for i in range(try_times):
         try:
             if method == 'get':
```

### Comparing `fast_multi_regex-0.8/fast_multi_regex.egg-info/PKG-INFO` & `fast_multi_regex-0.9/fast_multi_regex.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-multi-regex
-Version: 0.8
+Version: 0.9
 Summary: Fast multi-regex, multi-pattern, boolean expression matching
 Home-page: https://github.com/aitsc/fast_multi_regex
 Author: tanshicheng
 License: GPLv3
 Keywords: tools
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -22,26 +22,33 @@
 ## 使用
 ```shell
 pip install fast-multi-regex
 fast_multi_regex_server --help
 fast_multi_regex_server
 ```
 
-构建正则库，matchers_config_folder 内 json 文件例子（参考 OneTarget 格式和 file_processor_matchers_update 方法解析）：
+构建正则库，即增删改 matchers_config_folder 中的 json 文件（允许子文件夹嵌套），例子（参考 matcher_config_example）：
 ```json
 {
     "cache_size": 128,
     "literal": false,
     "targets": [
         {
-            "mark": "test",
+            "mark": "example",
             "regexs": [
                 {
-                    "expression": "test",
+                    "expression": "例子",
                     "flag": 40,
+                    "flag_ext": {
+                        "min_offset": null,
+                        "max_offset": null,
+                        "min_length": null,
+                        "edit_distance": null,
+                        "hamming_distance": null
+                    },
                     "min_match_count": 1,
                     "max_match_count": 0
                 }
             ],
             "min_regex_count": 1,
             "max_regex_count": 0,
             "bool_expr": "",
```

### Comparing `fast_multi_regex-0.8/setup.py` & `fast_multi_regex-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 if os.path.exists('readme.md'):
     long_description = open('readme.md', 'r', encoding='utf8').read()
 else:
     long_description = 'https://github.com/aitsc/fast_multi_regex'
 
 setup(
     name='fast_multi_regex',
-    version='0.8',
+    version='0.9',
     description="Fast multi-regex, multi-pattern, boolean expression matching",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='tanshicheng',
     license='GPLv3',
     url='https://github.com/aitsc/fast_multi_regex',
     keywords='tools',
```

