# Comparing `tmp/antchain_yuqing-1.2.3.tar.gz` & `tmp/antchain_yuqing-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_yuqing-1.2.3.tar", last modified: Mon Apr 17 08:00:56 2023, max compression
+gzip compressed data, was "dist/antchain_yuqing-1.2.9.tar", last modified: Mon Aug 14 16:58:23 2023, max compression
```

## Comparing `antchain_yuqing-1.2.3.tar` & `antchain_yuqing-1.2.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/
--rw-r--r--   0 root         (0) root         (0)      600 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2180 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      813 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      999 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47795 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/client.py
--rw-r--r--   0 root         (0) root         (0)   152781 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_sdk_yuqing/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2180 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      347 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/antchain_yuqing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2503 2023-04-17 08:00:56.000000 antchain_yuqing-1.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 16:58:23.000000 antchain_yuqing-1.2.9/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-08-14 16:58:23.000000 antchain_yuqing-1.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      813 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      999 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 16:58:23.000000 antchain_yuqing-1.2.9/antchain_sdk_yuqing/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_sdk_yuqing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54103 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_sdk_yuqing/client.py
+-rw-r--r--   0 root         (0) root         (0)   166768 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_sdk_yuqing/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-14 16:58:23.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/antchain_yuqing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-14 16:58:23.000000 antchain_yuqing-1.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-08-14 16:58:22.000000 antchain_yuqing-1.2.9/setup.py
```

### Comparing `antchain_yuqing-1.2.3/LICENSE` & `antchain_yuqing-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_yuqing-1.2.3/PKG-INFO` & `antchain_yuqing-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_yuqing
-Version: 1.2.3
+Version: 1.2.9
 Summary: Ant Chain YUQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yuqing-1.2.3/README-CN.md` & `antchain_yuqing-1.2.9/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_yuqing-1.2.3/README.md` & `antchain_yuqing-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `antchain_yuqing-1.2.3/antchain_sdk_yuqing/client.py` & `antchain_yuqing-1.2.9/antchain_sdk_yuqing/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.3',
+                    'sdk_version': '1.2.9',
                     '_prod_code': 'YUQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.3',
+                    'sdk_version': '1.2.9',
                     '_prod_code': 'YUQING',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -1222,7 +1222,175 @@
         Summary: 获取历史與情消息
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             yuqing_models.GetMessagesHistoryResponse(),
             await self.do_request_async('1.0', 'universalsaas.yuqing.messages.history.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
+
+    def submit_hotspot_task(
+        self,
+        request: yuqing_models.SubmitHotspotTaskRequest,
+    ) -> yuqing_models.SubmitHotspotTaskResponse:
+        """
+        Description: 提交实时热搜任务
+        Summary: 提交实时热搜任务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.submit_hotspot_task_ex(request, headers, runtime)
+
+    async def submit_hotspot_task_async(
+        self,
+        request: yuqing_models.SubmitHotspotTaskRequest,
+    ) -> yuqing_models.SubmitHotspotTaskResponse:
+        """
+        Description: 提交实时热搜任务
+        Summary: 提交实时热搜任务
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.submit_hotspot_task_ex_async(request, headers, runtime)
+
+    def submit_hotspot_task_ex(
+        self,
+        request: yuqing_models.SubmitHotspotTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.SubmitHotspotTaskResponse:
+        """
+        Description: 提交实时热搜任务
+        Summary: 提交实时热搜任务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.SubmitHotspotTaskResponse(),
+            self.do_request('1.0', 'universalsaas.yuqing.hotspot.task.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def submit_hotspot_task_ex_async(
+        self,
+        request: yuqing_models.SubmitHotspotTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.SubmitHotspotTaskResponse:
+        """
+        Description: 提交实时热搜任务
+        Summary: 提交实时热搜任务
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.SubmitHotspotTaskResponse(),
+            await self.do_request_async('1.0', 'universalsaas.yuqing.hotspot.task.submit', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_hotspot_task(
+        self,
+        request: yuqing_models.GetHotspotTaskRequest,
+    ) -> yuqing_models.GetHotspotTaskResponse:
+        """
+        Description: 获取实时热搜任务结果
+        Summary: 获取实时热搜任务结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_hotspot_task_ex(request, headers, runtime)
+
+    async def get_hotspot_task_async(
+        self,
+        request: yuqing_models.GetHotspotTaskRequest,
+    ) -> yuqing_models.GetHotspotTaskResponse:
+        """
+        Description: 获取实时热搜任务结果
+        Summary: 获取实时热搜任务结果
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_hotspot_task_ex_async(request, headers, runtime)
+
+    def get_hotspot_task_ex(
+        self,
+        request: yuqing_models.GetHotspotTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.GetHotspotTaskResponse:
+        """
+        Description: 获取实时热搜任务结果
+        Summary: 获取实时热搜任务结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.GetHotspotTaskResponse(),
+            self.do_request('1.0', 'universalsaas.yuqing.hotspot.task.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_hotspot_task_ex_async(
+        self,
+        request: yuqing_models.GetHotspotTaskRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.GetHotspotTaskResponse:
+        """
+        Description: 获取实时热搜任务结果
+        Summary: 获取实时热搜任务结果
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.GetHotspotTaskResponse(),
+            await self.do_request_async('1.0', 'universalsaas.yuqing.hotspot.task.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def get_sts_token(
+        self,
+        request: yuqing_models.GetStsTokenRequest,
+    ) -> yuqing_models.GetStsTokenResponse:
+        """
+        Description: 获取stsToken，作用于通用SAAS业务
+        Summary: 获取stsToken
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sts_token_ex(request, headers, runtime)
+
+    async def get_sts_token_async(
+        self,
+        request: yuqing_models.GetStsTokenRequest,
+    ) -> yuqing_models.GetStsTokenResponse:
+        """
+        Description: 获取stsToken，作用于通用SAAS业务
+        Summary: 获取stsToken
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_sts_token_ex_async(request, headers, runtime)
+
+    def get_sts_token_ex(
+        self,
+        request: yuqing_models.GetStsTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.GetStsTokenResponse:
+        """
+        Description: 获取stsToken，作用于通用SAAS业务
+        Summary: 获取stsToken
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.GetStsTokenResponse(),
+            self.do_request('1.0', 'universalsaas.yuqing.sts.token.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def get_sts_token_ex_async(
+        self,
+        request: yuqing_models.GetStsTokenRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> yuqing_models.GetStsTokenResponse:
+        """
+        Description: 获取stsToken，作用于通用SAAS业务
+        Summary: 获取stsToken
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            yuqing_models.GetStsTokenResponse(),
+            await self.do_request_async('1.0', 'universalsaas.yuqing.sts.token.get', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
```

### Comparing `antchain_yuqing-1.2.3/antchain_sdk_yuqing/models.py` & `antchain_yuqing-1.2.9/antchain_sdk_yuqing/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,337 @@
         if m.get('key') is not None:
             self.key = m.get('key')
         if m.get('value') is not None:
             self.value = m.get('value')
         return self
 
 
+class HotspotMessage(TeaModel):
+    def __init__(
+        self,
+        user_id: str = None,
+        total_exist_timestamp: int = None,
+        last_exist_date_format: str = None,
+        crawler_time_fmt: str = None,
+        first_exist_date_format: str = None,
+        max_rank_total_timestamp: int = None,
+        followers_count: int = None,
+        max_rank: int = None,
+        reads_count: int = None,
+        comments_count: int = None,
+        doc_title: str = None,
+        first_rank: int = None,
+        original_count: int = None,
+        presenter_name: str = None,
+        rank: int = None,
+        media_type: str = None,
+        doc_id: str = None,
+        type: str = None,
+        hot_value: int = None,
+        doc_content: str = None,
+        screen_name: str = None,
+        media_sub_type: str = None,
+        discusses_count: int = None,
+        category: str = None,
+        video_count: int = None,
+        max_rank_total_time_format: str = None,
+        province: str = None,
+        total_exist_time_format: str = None,
+        first_top_exist_timestamp: int = None,
+        doc_url: str = None,
+        max_hot_value: int = None,
+        city: str = None,
+        last_exist_timestamp: int = None,
+        first_top_exist_date_format: str = None,
+        last_rank: int = None,
+        first_hot_value: int = None,
+        hotspot_type: str = None,
+        first_xxist_timestamp: int = None,
+    ):
+        # 热搜/热榜/话题 对应用户id (可能为空)
+        self.user_id = user_id
+        # 在榜总时间
+        self.total_exist_timestamp = total_exist_timestamp
+        # 下榜时间
+        self.last_exist_date_format = last_exist_date_format
+        # 爬虫爬取的时间
+        self.crawler_time_fmt = crawler_time_fmt
+        # 第一次上榜的格式化时间
+        self.first_exist_date_format = first_exist_date_format
+        # 最高排名的总时长
+        self.max_rank_total_timestamp = max_rank_total_timestamp
+        # 跟随量
+        self.followers_count = followers_count
+        # 在榜单中的最高排名
+        self.max_rank = max_rank
+        # 阅读量
+        self.reads_count = reads_count
+        # 评论数
+        self.comments_count = comments_count
+        # 标题，例如话题的标题就是话题本身
+        self.doc_title = doc_title
+        # 首次上榜排名
+        self.first_rank = first_rank
+        # 原创人数
+        self.original_count = original_count
+        # 主持人
+        self.presenter_name = presenter_name
+        # 热搜在热搜榜的位置
+        self.rank = rank
+        # 热点媒体类型
+        self.media_type = media_type
+        # 文档id
+        self.doc_id = doc_id
+        # 类型
+        self.type = type
+        # 热度值
+        self.hot_value = hot_value
+        # 内容，热榜数据中存在着文章，热文就是有内容的
+        self.doc_content = doc_content
+        # 热搜/热榜/话题 对应用户名称 (可能为空)
+        self.screen_name = screen_name
+        # 热点媒体子类型
+        self.media_sub_type = media_sub_type
+        # 讨论量
+        self.discusses_count = discusses_count
+        # 分类
+        self.category = category
+        # 视频量
+        self.video_count = video_count
+        # 最高排名的格式化总时长
+        self.max_rank_total_time_format = max_rank_total_time_format
+        # 省
+        self.province = province
+        # 在榜格式化的总时间
+        self.total_exist_time_format = total_exist_time_format
+        # 第一次上最高排名的时间
+        self.first_top_exist_timestamp = first_top_exist_timestamp
+        # 链接地址
+        self.doc_url = doc_url
+        # 最大的热度值
+        self.max_hot_value = max_hot_value
+        # 市
+        self.city = city
+        # 最后一次上榜的时间
+        self.last_exist_timestamp = last_exist_timestamp
+        # 第一次上最高排名的时间
+        self.first_top_exist_date_format = first_top_exist_date_format
+        # 下榜排名
+        self.last_rank = last_rank
+        # 首次上榜热度
+        self.first_hot_value = first_hot_value
+        # 热搜类型
+        self.hotspot_type = hotspot_type
+        # 第一次上榜的时间
+        self.first_xxist_timestamp = first_xxist_timestamp
+
+    def validate(self):
+        self.validate_required(self.user_id, 'user_id')
+        self.validate_required(self.total_exist_timestamp, 'total_exist_timestamp')
+        self.validate_required(self.last_exist_date_format, 'last_exist_date_format')
+        self.validate_required(self.crawler_time_fmt, 'crawler_time_fmt')
+        self.validate_required(self.first_exist_date_format, 'first_exist_date_format')
+        self.validate_required(self.max_rank_total_timestamp, 'max_rank_total_timestamp')
+        self.validate_required(self.followers_count, 'followers_count')
+        self.validate_required(self.max_rank, 'max_rank')
+        self.validate_required(self.reads_count, 'reads_count')
+        self.validate_required(self.comments_count, 'comments_count')
+        self.validate_required(self.doc_title, 'doc_title')
+        self.validate_required(self.first_rank, 'first_rank')
+        self.validate_required(self.original_count, 'original_count')
+        self.validate_required(self.presenter_name, 'presenter_name')
+        self.validate_required(self.rank, 'rank')
+        self.validate_required(self.media_type, 'media_type')
+        self.validate_required(self.doc_id, 'doc_id')
+        self.validate_required(self.type, 'type')
+        self.validate_required(self.hot_value, 'hot_value')
+        self.validate_required(self.doc_content, 'doc_content')
+        self.validate_required(self.screen_name, 'screen_name')
+        self.validate_required(self.media_sub_type, 'media_sub_type')
+        self.validate_required(self.discusses_count, 'discusses_count')
+        self.validate_required(self.category, 'category')
+        self.validate_required(self.video_count, 'video_count')
+        self.validate_required(self.max_rank_total_time_format, 'max_rank_total_time_format')
+        self.validate_required(self.province, 'province')
+        self.validate_required(self.total_exist_time_format, 'total_exist_time_format')
+        self.validate_required(self.first_top_exist_timestamp, 'first_top_exist_timestamp')
+        self.validate_required(self.max_hot_value, 'max_hot_value')
+        self.validate_required(self.city, 'city')
+        self.validate_required(self.last_exist_timestamp, 'last_exist_timestamp')
+        self.validate_required(self.first_top_exist_date_format, 'first_top_exist_date_format')
+        self.validate_required(self.last_rank, 'last_rank')
+        self.validate_required(self.first_hot_value, 'first_hot_value')
+        self.validate_required(self.hotspot_type, 'hotspot_type')
+        self.validate_required(self.first_xxist_timestamp, 'first_xxist_timestamp')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.user_id is not None:
+            result['user_id'] = self.user_id
+        if self.total_exist_timestamp is not None:
+            result['total_exist_timestamp'] = self.total_exist_timestamp
+        if self.last_exist_date_format is not None:
+            result['last_exist_date_format'] = self.last_exist_date_format
+        if self.crawler_time_fmt is not None:
+            result['crawler_time_fmt'] = self.crawler_time_fmt
+        if self.first_exist_date_format is not None:
+            result['first_exist_date_format'] = self.first_exist_date_format
+        if self.max_rank_total_timestamp is not None:
+            result['max_rank_total_timestamp'] = self.max_rank_total_timestamp
+        if self.followers_count is not None:
+            result['followers_count'] = self.followers_count
+        if self.max_rank is not None:
+            result['max_rank'] = self.max_rank
+        if self.reads_count is not None:
+            result['reads_count'] = self.reads_count
+        if self.comments_count is not None:
+            result['comments_count'] = self.comments_count
+        if self.doc_title is not None:
+            result['doc_title'] = self.doc_title
+        if self.first_rank is not None:
+            result['first_rank'] = self.first_rank
+        if self.original_count is not None:
+            result['original_count'] = self.original_count
+        if self.presenter_name is not None:
+            result['presenter_name'] = self.presenter_name
+        if self.rank is not None:
+            result['rank'] = self.rank
+        if self.media_type is not None:
+            result['media_type'] = self.media_type
+        if self.doc_id is not None:
+            result['doc_id'] = self.doc_id
+        if self.type is not None:
+            result['type'] = self.type
+        if self.hot_value is not None:
+            result['hot_value'] = self.hot_value
+        if self.doc_content is not None:
+            result['doc_content'] = self.doc_content
+        if self.screen_name is not None:
+            result['screen_name'] = self.screen_name
+        if self.media_sub_type is not None:
+            result['media_sub_type'] = self.media_sub_type
+        if self.discusses_count is not None:
+            result['discusses_count'] = self.discusses_count
+        if self.category is not None:
+            result['category'] = self.category
+        if self.video_count is not None:
+            result['video_count'] = self.video_count
+        if self.max_rank_total_time_format is not None:
+            result['max_rank_total_time_format'] = self.max_rank_total_time_format
+        if self.province is not None:
+            result['province'] = self.province
+        if self.total_exist_time_format is not None:
+            result['total_exist_time_format'] = self.total_exist_time_format
+        if self.first_top_exist_timestamp is not None:
+            result['first_top_exist_timestamp'] = self.first_top_exist_timestamp
+        if self.doc_url is not None:
+            result['doc_url'] = self.doc_url
+        if self.max_hot_value is not None:
+            result['max_hot_value'] = self.max_hot_value
+        if self.city is not None:
+            result['city'] = self.city
+        if self.last_exist_timestamp is not None:
+            result['last_exist_timestamp'] = self.last_exist_timestamp
+        if self.first_top_exist_date_format is not None:
+            result['first_top_exist_date_format'] = self.first_top_exist_date_format
+        if self.last_rank is not None:
+            result['last_rank'] = self.last_rank
+        if self.first_hot_value is not None:
+            result['first_hot_value'] = self.first_hot_value
+        if self.hotspot_type is not None:
+            result['hotspot_type'] = self.hotspot_type
+        if self.first_xxist_timestamp is not None:
+            result['first_xxist_timestamp'] = self.first_xxist_timestamp
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('user_id') is not None:
+            self.user_id = m.get('user_id')
+        if m.get('total_exist_timestamp') is not None:
+            self.total_exist_timestamp = m.get('total_exist_timestamp')
+        if m.get('last_exist_date_format') is not None:
+            self.last_exist_date_format = m.get('last_exist_date_format')
+        if m.get('crawler_time_fmt') is not None:
+            self.crawler_time_fmt = m.get('crawler_time_fmt')
+        if m.get('first_exist_date_format') is not None:
+            self.first_exist_date_format = m.get('first_exist_date_format')
+        if m.get('max_rank_total_timestamp') is not None:
+            self.max_rank_total_timestamp = m.get('max_rank_total_timestamp')
+        if m.get('followers_count') is not None:
+            self.followers_count = m.get('followers_count')
+        if m.get('max_rank') is not None:
+            self.max_rank = m.get('max_rank')
+        if m.get('reads_count') is not None:
+            self.reads_count = m.get('reads_count')
+        if m.get('comments_count') is not None:
+            self.comments_count = m.get('comments_count')
+        if m.get('doc_title') is not None:
+            self.doc_title = m.get('doc_title')
+        if m.get('first_rank') is not None:
+            self.first_rank = m.get('first_rank')
+        if m.get('original_count') is not None:
+            self.original_count = m.get('original_count')
+        if m.get('presenter_name') is not None:
+            self.presenter_name = m.get('presenter_name')
+        if m.get('rank') is not None:
+            self.rank = m.get('rank')
+        if m.get('media_type') is not None:
+            self.media_type = m.get('media_type')
+        if m.get('doc_id') is not None:
+            self.doc_id = m.get('doc_id')
+        if m.get('type') is not None:
+            self.type = m.get('type')
+        if m.get('hot_value') is not None:
+            self.hot_value = m.get('hot_value')
+        if m.get('doc_content') is not None:
+            self.doc_content = m.get('doc_content')
+        if m.get('screen_name') is not None:
+            self.screen_name = m.get('screen_name')
+        if m.get('media_sub_type') is not None:
+            self.media_sub_type = m.get('media_sub_type')
+        if m.get('discusses_count') is not None:
+            self.discusses_count = m.get('discusses_count')
+        if m.get('category') is not None:
+            self.category = m.get('category')
+        if m.get('video_count') is not None:
+            self.video_count = m.get('video_count')
+        if m.get('max_rank_total_time_format') is not None:
+            self.max_rank_total_time_format = m.get('max_rank_total_time_format')
+        if m.get('province') is not None:
+            self.province = m.get('province')
+        if m.get('total_exist_time_format') is not None:
+            self.total_exist_time_format = m.get('total_exist_time_format')
+        if m.get('first_top_exist_timestamp') is not None:
+            self.first_top_exist_timestamp = m.get('first_top_exist_timestamp')
+        if m.get('doc_url') is not None:
+            self.doc_url = m.get('doc_url')
+        if m.get('max_hot_value') is not None:
+            self.max_hot_value = m.get('max_hot_value')
+        if m.get('city') is not None:
+            self.city = m.get('city')
+        if m.get('last_exist_timestamp') is not None:
+            self.last_exist_timestamp = m.get('last_exist_timestamp')
+        if m.get('first_top_exist_date_format') is not None:
+            self.first_top_exist_date_format = m.get('first_top_exist_date_format')
+        if m.get('last_rank') is not None:
+            self.last_rank = m.get('last_rank')
+        if m.get('first_hot_value') is not None:
+            self.first_hot_value = m.get('first_hot_value')
+        if m.get('hotspot_type') is not None:
+            self.hotspot_type = m.get('hotspot_type')
+        if m.get('first_xxist_timestamp') is not None:
+            self.first_xxist_timestamp = m.get('first_xxist_timestamp')
+        return self
+
+
 class Markdown(TeaModel):
     def __init__(
         self,
         title: str = None,
         text: str = None,
     ):
         # 标题
@@ -371,18 +694,19 @@
         doc_url: str = None,
         emotion_type: int = None,
         highlight_keywords: List[str] = None,
         media_type: str = None,
         message_type: str = None,
         parent_doc_id: str = None,
         publish_time: int = None,
-        relevance_score: int = None,
+        relevance_score: str = None,
         similar_number: int = None,
         weibo_comment_id: str = None,
         weibo_mid: str = None,
+        propagation_score: str = None,
     ):
         # 作者头像地址
         self.author_avatar_url = author_avatar_url
         # 粉丝数
         self.author_followers_count = author_followers_count
         # 好友数
         self.author_friends_count = author_friends_count
@@ -426,14 +750,16 @@
         self.relevance_score = relevance_score
         # 相似文章数
         self.similar_number = similar_number
         # 微博评论id
         self.weibo_comment_id = weibo_comment_id
         # 微博消息id
         self.weibo_mid = weibo_mid
+        # 传播得分，0-10
+        self.propagation_score = propagation_score
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -486,14 +812,16 @@
             result['relevance_score'] = self.relevance_score
         if self.similar_number is not None:
             result['similar_number'] = self.similar_number
         if self.weibo_comment_id is not None:
             result['weibo_comment_id'] = self.weibo_comment_id
         if self.weibo_mid is not None:
             result['weibo_mid'] = self.weibo_mid
+        if self.propagation_score is not None:
+            result['propagation_score'] = self.propagation_score
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('author_avatar_url') is not None:
             self.author_avatar_url = m.get('author_avatar_url')
         if m.get('author_followers_count') is not None:
@@ -540,14 +868,16 @@
             self.relevance_score = m.get('relevance_score')
         if m.get('similar_number') is not None:
             self.similar_number = m.get('similar_number')
         if m.get('weibo_comment_id') is not None:
             self.weibo_comment_id = m.get('weibo_comment_id')
         if m.get('weibo_mid') is not None:
             self.weibo_mid = m.get('weibo_mid')
+        if m.get('propagation_score') is not None:
+            self.propagation_score = m.get('propagation_score')
         return self
 
 
 class ActionCard(TeaModel):
     def __init__(
         self,
         title: str = None,
@@ -772,337 +1102,14 @@
             self.feed_card = temp_model.from_map(m['feed_card'])
         if m.get('at') is not None:
             temp_model = At()
             self.at = temp_model.from_map(m['at'])
         return self
 
 
-class HotspotMessage(TeaModel):
-    def __init__(
-        self,
-        user_id: str = None,
-        total_exist_timestamp: int = None,
-        last_exist_date_format: str = None,
-        crawler_time_fmt: str = None,
-        first_exist_date_format: str = None,
-        max_rank_total_timestamp: int = None,
-        followers_count: int = None,
-        max_rank: int = None,
-        reads_count: int = None,
-        comments_count: int = None,
-        doc_title: str = None,
-        first_rank: int = None,
-        original_count: int = None,
-        presenter_name: str = None,
-        rank: int = None,
-        media_type: str = None,
-        doc_id: str = None,
-        type: str = None,
-        hot_value: int = None,
-        doc_content: str = None,
-        screen_name: str = None,
-        media_sub_type: str = None,
-        discusses_count: int = None,
-        category: str = None,
-        video_count: int = None,
-        max_rank_total_time_format: str = None,
-        province: str = None,
-        total_exist_time_format: str = None,
-        first_top_exist_timestamp: int = None,
-        doc_url: str = None,
-        max_hot_value: int = None,
-        city: str = None,
-        last_exist_timestamp: int = None,
-        first_top_exist_date_format: str = None,
-        last_rank: int = None,
-        first_hot_value: int = None,
-        hotspot_type: str = None,
-        first_xxist_timestamp: int = None,
-    ):
-        # 热搜/热榜/话题 对应用户id (可能为空)
-        self.user_id = user_id
-        # 在榜总时间
-        self.total_exist_timestamp = total_exist_timestamp
-        # 下榜时间
-        self.last_exist_date_format = last_exist_date_format
-        # 爬虫爬取的时间
-        self.crawler_time_fmt = crawler_time_fmt
-        # 第一次上榜的格式化时间
-        self.first_exist_date_format = first_exist_date_format
-        # 最高排名的总时长
-        self.max_rank_total_timestamp = max_rank_total_timestamp
-        # 跟随量
-        self.followers_count = followers_count
-        # 在榜单中的最高排名
-        self.max_rank = max_rank
-        # 阅读量
-        self.reads_count = reads_count
-        # 评论数
-        self.comments_count = comments_count
-        # 标题，例如话题的标题就是话题本身
-        self.doc_title = doc_title
-        # 首次上榜排名
-        self.first_rank = first_rank
-        # 原创人数
-        self.original_count = original_count
-        # 主持人
-        self.presenter_name = presenter_name
-        # 热搜在热搜榜的位置
-        self.rank = rank
-        # 热点媒体类型
-        self.media_type = media_type
-        # 文档id
-        self.doc_id = doc_id
-        # 类型
-        self.type = type
-        # 热度值
-        self.hot_value = hot_value
-        # 内容，热榜数据中存在着文章，热文就是有内容的
-        self.doc_content = doc_content
-        # 热搜/热榜/话题 对应用户名称 (可能为空)
-        self.screen_name = screen_name
-        # 热点媒体子类型
-        self.media_sub_type = media_sub_type
-        # 讨论量
-        self.discusses_count = discusses_count
-        # 分类
-        self.category = category
-        # 视频量
-        self.video_count = video_count
-        # 最高排名的格式化总时长
-        self.max_rank_total_time_format = max_rank_total_time_format
-        # 省
-        self.province = province
-        # 在榜格式化的总时间
-        self.total_exist_time_format = total_exist_time_format
-        # 第一次上最高排名的时间
-        self.first_top_exist_timestamp = first_top_exist_timestamp
-        # 链接地址
-        self.doc_url = doc_url
-        # 最大的热度值
-        self.max_hot_value = max_hot_value
-        # 市
-        self.city = city
-        # 最后一次上榜的时间
-        self.last_exist_timestamp = last_exist_timestamp
-        # 第一次上最高排名的时间
-        self.first_top_exist_date_format = first_top_exist_date_format
-        # 下榜排名
-        self.last_rank = last_rank
-        # 首次上榜热度
-        self.first_hot_value = first_hot_value
-        # 热搜类型
-        self.hotspot_type = hotspot_type
-        # 第一次上榜的时间
-        self.first_xxist_timestamp = first_xxist_timestamp
-
-    def validate(self):
-        self.validate_required(self.user_id, 'user_id')
-        self.validate_required(self.total_exist_timestamp, 'total_exist_timestamp')
-        self.validate_required(self.last_exist_date_format, 'last_exist_date_format')
-        self.validate_required(self.crawler_time_fmt, 'crawler_time_fmt')
-        self.validate_required(self.first_exist_date_format, 'first_exist_date_format')
-        self.validate_required(self.max_rank_total_timestamp, 'max_rank_total_timestamp')
-        self.validate_required(self.followers_count, 'followers_count')
-        self.validate_required(self.max_rank, 'max_rank')
-        self.validate_required(self.reads_count, 'reads_count')
-        self.validate_required(self.comments_count, 'comments_count')
-        self.validate_required(self.doc_title, 'doc_title')
-        self.validate_required(self.first_rank, 'first_rank')
-        self.validate_required(self.original_count, 'original_count')
-        self.validate_required(self.presenter_name, 'presenter_name')
-        self.validate_required(self.rank, 'rank')
-        self.validate_required(self.media_type, 'media_type')
-        self.validate_required(self.doc_id, 'doc_id')
-        self.validate_required(self.type, 'type')
-        self.validate_required(self.hot_value, 'hot_value')
-        self.validate_required(self.doc_content, 'doc_content')
-        self.validate_required(self.screen_name, 'screen_name')
-        self.validate_required(self.media_sub_type, 'media_sub_type')
-        self.validate_required(self.discusses_count, 'discusses_count')
-        self.validate_required(self.category, 'category')
-        self.validate_required(self.video_count, 'video_count')
-        self.validate_required(self.max_rank_total_time_format, 'max_rank_total_time_format')
-        self.validate_required(self.province, 'province')
-        self.validate_required(self.total_exist_time_format, 'total_exist_time_format')
-        self.validate_required(self.first_top_exist_timestamp, 'first_top_exist_timestamp')
-        self.validate_required(self.max_hot_value, 'max_hot_value')
-        self.validate_required(self.city, 'city')
-        self.validate_required(self.last_exist_timestamp, 'last_exist_timestamp')
-        self.validate_required(self.first_top_exist_date_format, 'first_top_exist_date_format')
-        self.validate_required(self.last_rank, 'last_rank')
-        self.validate_required(self.first_hot_value, 'first_hot_value')
-        self.validate_required(self.hotspot_type, 'hotspot_type')
-        self.validate_required(self.first_xxist_timestamp, 'first_xxist_timestamp')
-
-    def to_map(self):
-        _map = super().to_map()
-        if _map is not None:
-            return _map
-
-        result = dict()
-        if self.user_id is not None:
-            result['user_id'] = self.user_id
-        if self.total_exist_timestamp is not None:
-            result['total_exist_timestamp'] = self.total_exist_timestamp
-        if self.last_exist_date_format is not None:
-            result['last_exist_date_format'] = self.last_exist_date_format
-        if self.crawler_time_fmt is not None:
-            result['crawler_time_fmt'] = self.crawler_time_fmt
-        if self.first_exist_date_format is not None:
-            result['first_exist_date_format'] = self.first_exist_date_format
-        if self.max_rank_total_timestamp is not None:
-            result['max_rank_total_timestamp'] = self.max_rank_total_timestamp
-        if self.followers_count is not None:
-            result['followers_count'] = self.followers_count
-        if self.max_rank is not None:
-            result['max_rank'] = self.max_rank
-        if self.reads_count is not None:
-            result['reads_count'] = self.reads_count
-        if self.comments_count is not None:
-            result['comments_count'] = self.comments_count
-        if self.doc_title is not None:
-            result['doc_title'] = self.doc_title
-        if self.first_rank is not None:
-            result['first_rank'] = self.first_rank
-        if self.original_count is not None:
-            result['original_count'] = self.original_count
-        if self.presenter_name is not None:
-            result['presenter_name'] = self.presenter_name
-        if self.rank is not None:
-            result['rank'] = self.rank
-        if self.media_type is not None:
-            result['media_type'] = self.media_type
-        if self.doc_id is not None:
-            result['doc_id'] = self.doc_id
-        if self.type is not None:
-            result['type'] = self.type
-        if self.hot_value is not None:
-            result['hot_value'] = self.hot_value
-        if self.doc_content is not None:
-            result['doc_content'] = self.doc_content
-        if self.screen_name is not None:
-            result['screen_name'] = self.screen_name
-        if self.media_sub_type is not None:
-            result['media_sub_type'] = self.media_sub_type
-        if self.discusses_count is not None:
-            result['discusses_count'] = self.discusses_count
-        if self.category is not None:
-            result['category'] = self.category
-        if self.video_count is not None:
-            result['video_count'] = self.video_count
-        if self.max_rank_total_time_format is not None:
-            result['max_rank_total_time_format'] = self.max_rank_total_time_format
-        if self.province is not None:
-            result['province'] = self.province
-        if self.total_exist_time_format is not None:
-            result['total_exist_time_format'] = self.total_exist_time_format
-        if self.first_top_exist_timestamp is not None:
-            result['first_top_exist_timestamp'] = self.first_top_exist_timestamp
-        if self.doc_url is not None:
-            result['doc_url'] = self.doc_url
-        if self.max_hot_value is not None:
-            result['max_hot_value'] = self.max_hot_value
-        if self.city is not None:
-            result['city'] = self.city
-        if self.last_exist_timestamp is not None:
-            result['last_exist_timestamp'] = self.last_exist_timestamp
-        if self.first_top_exist_date_format is not None:
-            result['first_top_exist_date_format'] = self.first_top_exist_date_format
-        if self.last_rank is not None:
-            result['last_rank'] = self.last_rank
-        if self.first_hot_value is not None:
-            result['first_hot_value'] = self.first_hot_value
-        if self.hotspot_type is not None:
-            result['hotspot_type'] = self.hotspot_type
-        if self.first_xxist_timestamp is not None:
-            result['first_xxist_timestamp'] = self.first_xxist_timestamp
-        return result
-
-    def from_map(self, m: dict = None):
-        m = m or dict()
-        if m.get('user_id') is not None:
-            self.user_id = m.get('user_id')
-        if m.get('total_exist_timestamp') is not None:
-            self.total_exist_timestamp = m.get('total_exist_timestamp')
-        if m.get('last_exist_date_format') is not None:
-            self.last_exist_date_format = m.get('last_exist_date_format')
-        if m.get('crawler_time_fmt') is not None:
-            self.crawler_time_fmt = m.get('crawler_time_fmt')
-        if m.get('first_exist_date_format') is not None:
-            self.first_exist_date_format = m.get('first_exist_date_format')
-        if m.get('max_rank_total_timestamp') is not None:
-            self.max_rank_total_timestamp = m.get('max_rank_total_timestamp')
-        if m.get('followers_count') is not None:
-            self.followers_count = m.get('followers_count')
-        if m.get('max_rank') is not None:
-            self.max_rank = m.get('max_rank')
-        if m.get('reads_count') is not None:
-            self.reads_count = m.get('reads_count')
-        if m.get('comments_count') is not None:
-            self.comments_count = m.get('comments_count')
-        if m.get('doc_title') is not None:
-            self.doc_title = m.get('doc_title')
-        if m.get('first_rank') is not None:
-            self.first_rank = m.get('first_rank')
-        if m.get('original_count') is not None:
-            self.original_count = m.get('original_count')
-        if m.get('presenter_name') is not None:
-            self.presenter_name = m.get('presenter_name')
-        if m.get('rank') is not None:
-            self.rank = m.get('rank')
-        if m.get('media_type') is not None:
-            self.media_type = m.get('media_type')
-        if m.get('doc_id') is not None:
-            self.doc_id = m.get('doc_id')
-        if m.get('type') is not None:
-            self.type = m.get('type')
-        if m.get('hot_value') is not None:
-            self.hot_value = m.get('hot_value')
-        if m.get('doc_content') is not None:
-            self.doc_content = m.get('doc_content')
-        if m.get('screen_name') is not None:
-            self.screen_name = m.get('screen_name')
-        if m.get('media_sub_type') is not None:
-            self.media_sub_type = m.get('media_sub_type')
-        if m.get('discusses_count') is not None:
-            self.discusses_count = m.get('discusses_count')
-        if m.get('category') is not None:
-            self.category = m.get('category')
-        if m.get('video_count') is not None:
-            self.video_count = m.get('video_count')
-        if m.get('max_rank_total_time_format') is not None:
-            self.max_rank_total_time_format = m.get('max_rank_total_time_format')
-        if m.get('province') is not None:
-            self.province = m.get('province')
-        if m.get('total_exist_time_format') is not None:
-            self.total_exist_time_format = m.get('total_exist_time_format')
-        if m.get('first_top_exist_timestamp') is not None:
-            self.first_top_exist_timestamp = m.get('first_top_exist_timestamp')
-        if m.get('doc_url') is not None:
-            self.doc_url = m.get('doc_url')
-        if m.get('max_hot_value') is not None:
-            self.max_hot_value = m.get('max_hot_value')
-        if m.get('city') is not None:
-            self.city = m.get('city')
-        if m.get('last_exist_timestamp') is not None:
-            self.last_exist_timestamp = m.get('last_exist_timestamp')
-        if m.get('first_top_exist_date_format') is not None:
-            self.first_top_exist_date_format = m.get('first_top_exist_date_format')
-        if m.get('last_rank') is not None:
-            self.last_rank = m.get('last_rank')
-        if m.get('first_hot_value') is not None:
-            self.first_hot_value = m.get('first_hot_value')
-        if m.get('hotspot_type') is not None:
-            self.hotspot_type = m.get('hotspot_type')
-        if m.get('first_xxist_timestamp') is not None:
-            self.first_xxist_timestamp = m.get('first_xxist_timestamp')
-        return self
-
-
 class Alarm(TeaModel):
     def __init__(
         self,
         tags: List[str] = None,
         content: str = None,
         alarm_timestamp: int = None,
         project_id: int = None,
@@ -1279,14 +1286,83 @@
         if m.get('publish_time_end') is not None:
             self.publish_time_end = m.get('publish_time_end')
         if m.get('url_list') is not None:
             self.url_list = m.get('url_list')
         return self
 
 
+class HotspotTask(TeaModel):
+    def __init__(
+        self,
+        task_id: str = None,
+        count: int = None,
+        page_now: int = None,
+        page_size: int = None,
+        pages: List[HotspotMessage] = None,
+    ):
+        # 任务ID
+        self.task_id = task_id
+        # 数量
+        self.count = count
+        # 当前页
+        self.page_now = page_now
+        # 每页数量
+        self.page_size = page_size
+        # 数据
+        self.pages = pages
+
+    def validate(self):
+        self.validate_required(self.task_id, 'task_id')
+        self.validate_required(self.count, 'count')
+        self.validate_required(self.page_now, 'page_now')
+        self.validate_required(self.page_size, 'page_size')
+        self.validate_required(self.pages, 'pages')
+        if self.pages:
+            for k in self.pages:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.task_id is not None:
+            result['task_id'] = self.task_id
+        if self.count is not None:
+            result['count'] = self.count
+        if self.page_now is not None:
+            result['page_now'] = self.page_now
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        result['pages'] = []
+        if self.pages is not None:
+            for k in self.pages:
+                result['pages'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('task_id') is not None:
+            self.task_id = m.get('task_id')
+        if m.get('count') is not None:
+            self.count = m.get('count')
+        if m.get('page_now') is not None:
+            self.page_now = m.get('page_now')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        self.pages = []
+        if m.get('pages') is not None:
+            for k in m.get('pages'):
+                temp_model = HotspotMessage()
+                self.pages.append(temp_model.from_map(k))
+        return self
+
+
 class SearchCondition(TeaModel):
     def __init__(
         self,
         ass_keyword_list: List[str] = None,
         at_author_name_list: List[str] = None,
         author_name_list: List[str] = None,
         comments_level: int = None,
@@ -4130,7 +4206,335 @@
         if m.get('yuqing_messages') is not None:
             for k in m.get('yuqing_messages'):
                 temp_model = YuqingMessage()
                 self.yuqing_messages.append(temp_model.from_map(k))
         return self
 
 
+class SubmitHotspotTaskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        media_sub_types: List[str] = None,
+        expired_time: int = None,
+        sort_by_direction: str = None,
+        sort_by: str = None,
+        crawler_time_start_filter: int = None,
+        crawler_time_end_filter: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 媒体类型
+        self.media_sub_types = media_sub_types
+        # 任务过期时间,单位秒
+        self.expired_time = expired_time
+        # 排序方式： 正序(+)、倒序(-)
+        self.sort_by_direction = sort_by_direction
+        # 排序字段
+        self.sort_by = sort_by
+        # 爬取开始时间过滤
+        self.crawler_time_start_filter = crawler_time_start_filter
+        # 爬取结束时间过滤
+        self.crawler_time_end_filter = crawler_time_end_filter
+
+    def validate(self):
+        self.validate_required(self.media_sub_types, 'media_sub_types')
+        self.validate_required(self.expired_time, 'expired_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.media_sub_types is not None:
+            result['media_sub_types'] = self.media_sub_types
+        if self.expired_time is not None:
+            result['expired_time'] = self.expired_time
+        if self.sort_by_direction is not None:
+            result['sort_by_direction'] = self.sort_by_direction
+        if self.sort_by is not None:
+            result['sort_by'] = self.sort_by
+        if self.crawler_time_start_filter is not None:
+            result['crawler_time_start_filter'] = self.crawler_time_start_filter
+        if self.crawler_time_end_filter is not None:
+            result['crawler_time_end_filter'] = self.crawler_time_end_filter
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('media_sub_types') is not None:
+            self.media_sub_types = m.get('media_sub_types')
+        if m.get('expired_time') is not None:
+            self.expired_time = m.get('expired_time')
+        if m.get('sort_by_direction') is not None:
+            self.sort_by_direction = m.get('sort_by_direction')
+        if m.get('sort_by') is not None:
+            self.sort_by = m.get('sort_by')
+        if m.get('crawler_time_start_filter') is not None:
+            self.crawler_time_start_filter = m.get('crawler_time_start_filter')
+        if m.get('crawler_time_end_filter') is not None:
+            self.crawler_time_end_filter = m.get('crawler_time_end_filter')
+        return self
+
+
+class SubmitHotspotTaskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        task_ids: List[str] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 任务ID
+        self.task_ids = task_ids
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.task_ids is not None:
+            result['task_ids'] = self.task_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('task_ids') is not None:
+            self.task_ids = m.get('task_ids')
+        return self
+
+
+class GetHotspotTaskRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        task_ids: List[str] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 任务ID
+        self.task_ids = task_ids
+
+    def validate(self):
+        self.validate_required(self.task_ids, 'task_ids')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.task_ids is not None:
+            result['task_ids'] = self.task_ids
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('task_ids') is not None:
+            self.task_ids = m.get('task_ids')
+        return self
+
+
+class GetHotspotTaskResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        hotspot_tasks: List[HotspotTask] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 任务的结果
+        self.hotspot_tasks = hotspot_tasks
+
+    def validate(self):
+        if self.hotspot_tasks:
+            for k in self.hotspot_tasks:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        result['hotspot_tasks'] = []
+        if self.hotspot_tasks is not None:
+            for k in self.hotspot_tasks:
+                result['hotspot_tasks'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        self.hotspot_tasks = []
+        if m.get('hotspot_tasks') is not None:
+            for k in m.get('hotspot_tasks'):
+                temp_model = HotspotTask()
+                self.hotspot_tasks.append(temp_model.from_map(k))
+        return self
+
+
+class GetStsTokenRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_type: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 业务类型
+        self.biz_type = biz_type
+
+    def validate(self):
+        self.validate_required(self.biz_type, 'biz_type')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_type is not None:
+            result['biz_type'] = self.biz_type
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_type') is not None:
+            self.biz_type = m.get('biz_type')
+        return self
+
+
+class GetStsTokenResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        access_key_id: str = None,
+        access_key_secret: str = None,
+        security_token: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # AK
+        self.access_key_id = access_key_id
+        # SK
+        self.access_key_secret = access_key_secret
+        # stsToken
+        self.security_token = security_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.access_key_id is not None:
+            result['access_key_id'] = self.access_key_id
+        if self.access_key_secret is not None:
+            result['access_key_secret'] = self.access_key_secret
+        if self.security_token is not None:
+            result['security_token'] = self.security_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('access_key_id') is not None:
+            self.access_key_id = m.get('access_key_id')
+        if m.get('access_key_secret') is not None:
+            self.access_key_secret = m.get('access_key_secret')
+        if m.get('security_token') is not None:
+            self.security_token = m.get('security_token')
+        return self
+
+
```

### Comparing `antchain_yuqing-1.2.3/antchain_yuqing.egg-info/PKG-INFO` & `antchain_yuqing-1.2.9/antchain_yuqing.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-yuqing
-Version: 1.2.3
+Version: 1.2.9
 Summary: Ant Chain YUQING SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_yuqing-1.2.3/setup.py` & `antchain_yuqing-1.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_yuqing.
 
-Created on 17/04/2023
+Created on 14/08/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_yuqing"
 NAME = "antchain_yuqing" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain YUQING SDK Library for Python"
 AUTHOR = "Ant Chain SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/alipay/antchain-openapi-prod-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
     "antchain_alipay_util>=1.0.1, <2.0.0",
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_rpc_util>=0.0.4, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

