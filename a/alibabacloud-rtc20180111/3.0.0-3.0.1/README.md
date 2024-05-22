# Comparing `tmp/alibabacloud_rtc20180111-3.0.0.tar.gz` & `tmp/alibabacloud_rtc20180111-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rtc20180111-3.0.0.tar", last modified: Thu Mar 21 02:25:19 2024, max compression
+gzip compressed data, was "dist/alibabacloud_rtc20180111-3.0.1.tar", last modified: Wed May 22 17:15:05 2024, max compression
```

## Comparing `alibabacloud_rtc20180111-3.0.0.tar` & `alibabacloud_rtc20180111-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     1947 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2421 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   276366 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/client.py
--rw-r--r--   0 root         (0) root         (0)   552033 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2421 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2631 2024-03-21 02:25:19.000000 alibabacloud_rtc20180111-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   334856 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/client.py
+-rw-r--r--   0 root         (0) root         (0)   561396 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2421 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-22 17:15:05.000000 alibabacloud_rtc20180111-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2631 2024-05-22 17:15:04.000000 alibabacloud_rtc20180111-3.0.1/setup.py
```

### Comparing `alibabacloud_rtc20180111-3.0.0/ChangeLog.md` & `alibabacloud_rtc20180111-3.0.1/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+2024-03-21 Version: 3.0.0
+- Support API DescribeChannel.
+- Support API DescribeChannelAllUsers.
+- Support API DescribeChannelUser.
+- Support API RemoveUsers.
+- Support API StartCloudRecord.
+- Support API StartStreamingOut.
+- Support API StopChannel.
+- Support API StopCloudRecord.
+- Support API StopStreamingOut.
+- Update API CreateAppStreamingOutTemplate: update param StreamingOutTemplate.
+- Update API DescribeAppKey: update response param.
+- Update API DescribeAppStreamingOutTemplates: update response param.
+- Update API ModifyAppStreamingOutTemplate: update param StreamingOutTemplate.
+
+
 2024-03-08 Version: 2.0.0
 - Support API DescribeChannel.
 - Support API DescribeChannelAllUsers.
 - Support API DescribeChannelUser.
 - Support API RemoveUsers.
 - Support API StartCloudRecord.
 - Support API StartStreamingOut.
```

### Comparing `alibabacloud_rtc20180111-3.0.0/LICENSE` & `alibabacloud_rtc20180111-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rtc20180111-3.0.0/PKG-INFO` & `alibabacloud_rtc20180111-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rtc20180111
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud Real-Time Communication (20180111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rtc20180111-3.0.0/README-CN.md` & `alibabacloud_rtc20180111-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rtc20180111-3.0.0/README.md` & `alibabacloud_rtc20180111-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/client.py` & `alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,14 +42,19 @@
         return EndpointUtilClient.get_endpoint_rules(product_id, region_id, endpoint_rule, network, suffix)
 
     def add_record_template_with_options(
         self,
         request: rtc_20180111_models.AddRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.AddRecordTemplateResponse:
+        """
+        @param request: AddRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -106,14 +111,19 @@
         )
 
     async def add_record_template_with_options_async(
         self,
         request: rtc_20180111_models.AddRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.AddRecordTemplateResponse:
+        """
+        @param request: AddRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: AddRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -169,29 +179,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def add_record_template(
         self,
         request: rtc_20180111_models.AddRecordTemplateRequest,
     ) -> rtc_20180111_models.AddRecordTemplateResponse:
+        """
+        @param request: AddRecordTemplateRequest
+        @return: AddRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.add_record_template_with_options(request, runtime)
 
     async def add_record_template_async(
         self,
         request: rtc_20180111_models.AddRecordTemplateRequest,
     ) -> rtc_20180111_models.AddRecordTemplateResponse:
+        """
+        @param request: AddRecordTemplateRequest
+        @return: AddRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.add_record_template_with_options_async(request, runtime)
 
     def create_app_streaming_out_template_with_options(
         self,
         tmp_req: rtc_20180111_models.CreateAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateAppStreamingOutTemplateResponse:
+        """
+        @summary 创建应用推流模版
+        
+        @param tmp_req: CreateAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.CreateAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -218,14 +243,21 @@
         )
 
     async def create_app_streaming_out_template_with_options_async(
         self,
         tmp_req: rtc_20180111_models.CreateAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateAppStreamingOutTemplateResponse:
+        """
+        @summary 创建应用推流模版
+        
+        @param tmp_req: CreateAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.CreateAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -251,29 +283,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_app_streaming_out_template(
         self,
         request: rtc_20180111_models.CreateAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.CreateAppStreamingOutTemplateResponse:
+        """
+        @summary 创建应用推流模版
+        
+        @param request: CreateAppStreamingOutTemplateRequest
+        @return: CreateAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_app_streaming_out_template_with_options(request, runtime)
 
     async def create_app_streaming_out_template_async(
         self,
         request: rtc_20180111_models.CreateAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.CreateAppStreamingOutTemplateResponse:
+        """
+        @summary 创建应用推流模版
+        
+        @param request: CreateAppStreamingOutTemplateRequest
+        @return: CreateAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_app_streaming_out_template_with_options_async(request, runtime)
 
     def create_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.CreateAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateAutoLiveStreamRuleResponse:
+        """
+        @param request: CreateAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_back):
             query['CallBack'] = request.call_back
         if not UtilClient.is_unset(request.channel_id_prefixes):
@@ -308,14 +357,19 @@
         )
 
     async def create_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.CreateAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateAutoLiveStreamRuleResponse:
+        """
+        @param request: CreateAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_back):
             query['CallBack'] = request.call_back
         if not UtilClient.is_unset(request.channel_id_prefixes):
@@ -349,29 +403,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.CreateAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.CreateAutoLiveStreamRuleResponse:
+        """
+        @param request: CreateAutoLiveStreamRuleRequest
+        @return: CreateAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_auto_live_stream_rule_with_options(request, runtime)
 
     async def create_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.CreateAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.CreateAutoLiveStreamRuleResponse:
+        """
+        @param request: CreateAutoLiveStreamRuleRequest
+        @return: CreateAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_auto_live_stream_rule_with_options_async(request, runtime)
 
     def create_event_subscribe_with_options(
         self,
         request: rtc_20180111_models.CreateEventSubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateEventSubscribeResponse:
+        """
+        @param request: CreateEventSubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateEventSubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.callback_url):
             query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.channel_id):
@@ -408,14 +475,19 @@
         )
 
     async def create_event_subscribe_with_options_async(
         self,
         request: rtc_20180111_models.CreateEventSubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateEventSubscribeResponse:
+        """
+        @param request: CreateEventSubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateEventSubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.callback_url):
             query['CallbackUrl'] = request.callback_url
         if not UtilClient.is_unset(request.channel_id):
@@ -451,29 +523,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_event_subscribe(
         self,
         request: rtc_20180111_models.CreateEventSubscribeRequest,
     ) -> rtc_20180111_models.CreateEventSubscribeResponse:
+        """
+        @param request: CreateEventSubscribeRequest
+        @return: CreateEventSubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_event_subscribe_with_options(request, runtime)
 
     async def create_event_subscribe_async(
         self,
         request: rtc_20180111_models.CreateEventSubscribeRequest,
     ) -> rtc_20180111_models.CreateEventSubscribeResponse:
+        """
+        @param request: CreateEventSubscribeRequest
+        @return: CreateEventSubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_event_subscribe_with_options_async(request, runtime)
 
     def create_mpulayout_with_options(
         self,
         request: rtc_20180111_models.CreateMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateMPULayoutResponse:
+        """
+        @param request: CreateMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.audio_mix_count):
             query['AudioMixCount'] = request.audio_mix_count
         if not UtilClient.is_unset(request.name):
@@ -502,14 +587,19 @@
         )
 
     async def create_mpulayout_with_options_async(
         self,
         request: rtc_20180111_models.CreateMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.CreateMPULayoutResponse:
+        """
+        @param request: CreateMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.audio_mix_count):
             query['AudioMixCount'] = request.audio_mix_count
         if not UtilClient.is_unset(request.name):
@@ -537,29 +627,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_mpulayout(
         self,
         request: rtc_20180111_models.CreateMPULayoutRequest,
     ) -> rtc_20180111_models.CreateMPULayoutResponse:
+        """
+        @param request: CreateMPULayoutRequest
+        @return: CreateMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_mpulayout_with_options(request, runtime)
 
     async def create_mpulayout_async(
         self,
         request: rtc_20180111_models.CreateMPULayoutRequest,
     ) -> rtc_20180111_models.CreateMPULayoutResponse:
+        """
+        @param request: CreateMPULayoutRequest
+        @return: CreateMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_mpulayout_with_options_async(request, runtime)
 
     def delete_app_streaming_out_template_with_options(
         self,
         tmp_req: rtc_20180111_models.DeleteAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteAppStreamingOutTemplateResponse:
+        """
+        @summary 删除应用推流模版
+        
+        @param tmp_req: DeleteAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.DeleteAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -586,14 +691,21 @@
         )
 
     async def delete_app_streaming_out_template_with_options_async(
         self,
         tmp_req: rtc_20180111_models.DeleteAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteAppStreamingOutTemplateResponse:
+        """
+        @summary 删除应用推流模版
+        
+        @param tmp_req: DeleteAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.DeleteAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -619,29 +731,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_app_streaming_out_template(
         self,
         request: rtc_20180111_models.DeleteAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.DeleteAppStreamingOutTemplateResponse:
+        """
+        @summary 删除应用推流模版
+        
+        @param request: DeleteAppStreamingOutTemplateRequest
+        @return: DeleteAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_app_streaming_out_template_with_options(request, runtime)
 
     async def delete_app_streaming_out_template_async(
         self,
         request: rtc_20180111_models.DeleteAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.DeleteAppStreamingOutTemplateResponse:
+        """
+        @summary 删除应用推流模版
+        
+        @param request: DeleteAppStreamingOutTemplateRequest
+        @return: DeleteAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_app_streaming_out_template_with_options_async(request, runtime)
 
     def delete_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.DeleteAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteAutoLiveStreamRuleResponse:
+        """
+        @param request: DeleteAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -666,14 +795,19 @@
         )
 
     async def delete_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.DeleteAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteAutoLiveStreamRuleResponse:
+        """
+        @param request: DeleteAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -697,29 +831,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.DeleteAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DeleteAutoLiveStreamRuleResponse:
+        """
+        @param request: DeleteAutoLiveStreamRuleRequest
+        @return: DeleteAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_auto_live_stream_rule_with_options(request, runtime)
 
     async def delete_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.DeleteAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DeleteAutoLiveStreamRuleResponse:
+        """
+        @param request: DeleteAutoLiveStreamRuleRequest
+        @return: DeleteAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_auto_live_stream_rule_with_options_async(request, runtime)
 
     def delete_channel_with_options(
         self,
         request: rtc_20180111_models.DeleteChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteChannelResponse:
+        """
+        @param request: DeleteChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -744,14 +891,19 @@
         )
 
     async def delete_channel_with_options_async(
         self,
         request: rtc_20180111_models.DeleteChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteChannelResponse:
+        """
+        @param request: DeleteChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -775,29 +927,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_channel(
         self,
         request: rtc_20180111_models.DeleteChannelRequest,
     ) -> rtc_20180111_models.DeleteChannelResponse:
+        """
+        @param request: DeleteChannelRequest
+        @return: DeleteChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_channel_with_options(request, runtime)
 
     async def delete_channel_async(
         self,
         request: rtc_20180111_models.DeleteChannelRequest,
     ) -> rtc_20180111_models.DeleteChannelResponse:
+        """
+        @param request: DeleteChannelRequest
+        @return: DeleteChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_channel_with_options_async(request, runtime)
 
     def delete_event_subscribe_with_options(
         self,
         request: rtc_20180111_models.DeleteEventSubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteEventSubscribeResponse:
+        """
+        @param request: DeleteEventSubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteEventSubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.subscribe_id):
@@ -822,14 +987,19 @@
         )
 
     async def delete_event_subscribe_with_options_async(
         self,
         request: rtc_20180111_models.DeleteEventSubscribeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteEventSubscribeResponse:
+        """
+        @param request: DeleteEventSubscribeRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteEventSubscribeResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.subscribe_id):
@@ -853,29 +1023,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_event_subscribe(
         self,
         request: rtc_20180111_models.DeleteEventSubscribeRequest,
     ) -> rtc_20180111_models.DeleteEventSubscribeResponse:
+        """
+        @param request: DeleteEventSubscribeRequest
+        @return: DeleteEventSubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_event_subscribe_with_options(request, runtime)
 
     async def delete_event_subscribe_async(
         self,
         request: rtc_20180111_models.DeleteEventSubscribeRequest,
     ) -> rtc_20180111_models.DeleteEventSubscribeResponse:
+        """
+        @param request: DeleteEventSubscribeRequest
+        @return: DeleteEventSubscribeResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_event_subscribe_with_options_async(request, runtime)
 
     def delete_mpulayout_with_options(
         self,
         request: rtc_20180111_models.DeleteMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteMPULayoutResponse:
+        """
+        @param request: DeleteMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.layout_id):
             query['LayoutId'] = request.layout_id
         if not UtilClient.is_unset(request.owner_id):
@@ -900,14 +1083,19 @@
         )
 
     async def delete_mpulayout_with_options_async(
         self,
         request: rtc_20180111_models.DeleteMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteMPULayoutResponse:
+        """
+        @param request: DeleteMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.layout_id):
             query['LayoutId'] = request.layout_id
         if not UtilClient.is_unset(request.owner_id):
@@ -931,29 +1119,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_mpulayout(
         self,
         request: rtc_20180111_models.DeleteMPULayoutRequest,
     ) -> rtc_20180111_models.DeleteMPULayoutResponse:
+        """
+        @param request: DeleteMPULayoutRequest
+        @return: DeleteMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_mpulayout_with_options(request, runtime)
 
     async def delete_mpulayout_async(
         self,
         request: rtc_20180111_models.DeleteMPULayoutRequest,
     ) -> rtc_20180111_models.DeleteMPULayoutResponse:
+        """
+        @param request: DeleteMPULayoutRequest
+        @return: DeleteMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_mpulayout_with_options_async(request, runtime)
 
     def delete_record_template_with_options(
         self,
         request: rtc_20180111_models.DeleteRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteRecordTemplateResponse:
+        """
+        @param request: DeleteRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.template_id):
@@ -978,14 +1179,19 @@
         )
 
     async def delete_record_template_with_options_async(
         self,
         request: rtc_20180111_models.DeleteRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DeleteRecordTemplateResponse:
+        """
+        @param request: DeleteRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.template_id):
@@ -1009,29 +1215,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_record_template(
         self,
         request: rtc_20180111_models.DeleteRecordTemplateRequest,
     ) -> rtc_20180111_models.DeleteRecordTemplateResponse:
+        """
+        @param request: DeleteRecordTemplateRequest
+        @return: DeleteRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_record_template_with_options(request, runtime)
 
     async def delete_record_template_async(
         self,
         request: rtc_20180111_models.DeleteRecordTemplateRequest,
     ) -> rtc_20180111_models.DeleteRecordTemplateResponse:
+        """
+        @param request: DeleteRecordTemplateRequest
+        @return: DeleteRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_record_template_with_options_async(request, runtime)
 
     def describe_app_key_with_options(
         self,
         request: rtc_20180111_models.DescribeAppKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppKeyResponse:
+        """
+        @summary 查看AppKey
+        
+        @param request: DescribeAppKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppKeyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         req = open_api_models.OpenApiRequest(
@@ -1054,14 +1275,21 @@
         )
 
     async def describe_app_key_with_options_async(
         self,
         request: rtc_20180111_models.DescribeAppKeyRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppKeyResponse:
+        """
+        @summary 查看AppKey
+        
+        @param request: DescribeAppKeyRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppKeyResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         req = open_api_models.OpenApiRequest(
@@ -1083,29 +1311,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_app_key(
         self,
         request: rtc_20180111_models.DescribeAppKeyRequest,
     ) -> rtc_20180111_models.DescribeAppKeyResponse:
+        """
+        @summary 查看AppKey
+        
+        @param request: DescribeAppKeyRequest
+        @return: DescribeAppKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_app_key_with_options(request, runtime)
 
     async def describe_app_key_async(
         self,
         request: rtc_20180111_models.DescribeAppKeyRequest,
     ) -> rtc_20180111_models.DescribeAppKeyResponse:
+        """
+        @summary 查看AppKey
+        
+        @param request: DescribeAppKeyRequest
+        @return: DescribeAppKeyResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_app_key_with_options_async(request, runtime)
 
     def describe_app_streaming_out_templates_with_options(
         self,
         tmp_req: rtc_20180111_models.DescribeAppStreamingOutTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppStreamingOutTemplatesResponse:
+        """
+        @summary 应用推流模版列表
+        
+        @param tmp_req: DescribeAppStreamingOutTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppStreamingOutTemplatesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.DescribeAppStreamingOutTemplatesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.condition):
             request.condition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.condition, 'Condition', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -1136,14 +1383,21 @@
         )
 
     async def describe_app_streaming_out_templates_with_options_async(
         self,
         tmp_req: rtc_20180111_models.DescribeAppStreamingOutTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppStreamingOutTemplatesResponse:
+        """
+        @summary 应用推流模版列表
+        
+        @param tmp_req: DescribeAppStreamingOutTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppStreamingOutTemplatesResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.DescribeAppStreamingOutTemplatesShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.condition):
             request.condition_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.condition, 'Condition', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -1173,33 +1427,54 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_app_streaming_out_templates(
         self,
         request: rtc_20180111_models.DescribeAppStreamingOutTemplatesRequest,
     ) -> rtc_20180111_models.DescribeAppStreamingOutTemplatesResponse:
+        """
+        @summary 应用推流模版列表
+        
+        @param request: DescribeAppStreamingOutTemplatesRequest
+        @return: DescribeAppStreamingOutTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_app_streaming_out_templates_with_options(request, runtime)
 
     async def describe_app_streaming_out_templates_async(
         self,
         request: rtc_20180111_models.DescribeAppStreamingOutTemplatesRequest,
     ) -> rtc_20180111_models.DescribeAppStreamingOutTemplatesResponse:
+        """
+        @summary 应用推流模版列表
+        
+        @param request: DescribeAppStreamingOutTemplatesRequest
+        @return: DescribeAppStreamingOutTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_app_streaming_out_templates_with_options_async(request, runtime)
 
     def describe_apps_with_options(
         self,
         request: rtc_20180111_models.DescribeAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppsResponse:
+        """
+        @summary App列表
+        
+        @param request: DescribeAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.app_version):
+            query['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -1226,18 +1501,27 @@
         )
 
     async def describe_apps_with_options_async(
         self,
         request: rtc_20180111_models.DescribeAppsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAppsResponse:
+        """
+        @summary App列表
+        
+        @param request: DescribeAppsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAppsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
+        if not UtilClient.is_unset(request.app_version):
+            query['AppVersion'] = request.app_version
         if not UtilClient.is_unset(request.order):
             query['Order'] = request.order
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
             query['PageNum'] = request.page_num
         if not UtilClient.is_unset(request.page_size):
@@ -1263,29 +1547,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_apps(
         self,
         request: rtc_20180111_models.DescribeAppsRequest,
     ) -> rtc_20180111_models.DescribeAppsResponse:
+        """
+        @summary App列表
+        
+        @param request: DescribeAppsRequest
+        @return: DescribeAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_apps_with_options(request, runtime)
 
     async def describe_apps_async(
         self,
         request: rtc_20180111_models.DescribeAppsRequest,
     ) -> rtc_20180111_models.DescribeAppsResponse:
+        """
+        @summary App列表
+        
+        @param request: DescribeAppsRequest
+        @return: DescribeAppsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_apps_with_options_async(request, runtime)
 
     def describe_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.DescribeAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAutoLiveStreamRuleResponse:
+        """
+        @param request: DescribeAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         req = open_api_models.OpenApiRequest(
@@ -1308,14 +1609,19 @@
         )
 
     async def describe_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.DescribeAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeAutoLiveStreamRuleResponse:
+        """
+        @param request: DescribeAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         req = open_api_models.OpenApiRequest(
@@ -1337,29 +1643,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.DescribeAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DescribeAutoLiveStreamRuleResponse:
+        """
+        @param request: DescribeAutoLiveStreamRuleRequest
+        @return: DescribeAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_auto_live_stream_rule_with_options(request, runtime)
 
     async def describe_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.DescribeAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DescribeAutoLiveStreamRuleResponse:
+        """
+        @param request: DescribeAutoLiveStreamRuleRequest
+        @return: DescribeAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_auto_live_stream_rule_with_options_async(request, runtime)
 
     def describe_call_with_options(
         self,
         request: rtc_20180111_models.DescribeCallRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeCallResponse:
+        """
+        @summary 调用DescribeCall获取单次通信详情。
+        
+        @param request: DescribeCallRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCallResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1390,14 +1711,21 @@
         )
 
     async def describe_call_with_options_async(
         self,
         request: rtc_20180111_models.DescribeCallRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeCallResponse:
+        """
+        @summary 调用DescribeCall获取单次通信详情。
+        
+        @param request: DescribeCallRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCallResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1427,29 +1755,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_call(
         self,
         request: rtc_20180111_models.DescribeCallRequest,
     ) -> rtc_20180111_models.DescribeCallResponse:
+        """
+        @summary 调用DescribeCall获取单次通信详情。
+        
+        @param request: DescribeCallRequest
+        @return: DescribeCallResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_call_with_options(request, runtime)
 
     async def describe_call_async(
         self,
         request: rtc_20180111_models.DescribeCallRequest,
     ) -> rtc_20180111_models.DescribeCallResponse:
+        """
+        @summary 调用DescribeCall获取单次通信详情。
+        
+        @param request: DescribeCallRequest
+        @return: DescribeCallResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_call_with_options_async(request, runtime)
 
     def describe_call_list_with_options(
         self,
         request: rtc_20180111_models.DescribeCallListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeCallListResponse:
+        """
+        @summary 调用DescribeCallList分页查询时间范围内创建的通信信息。
+        
+        @param request: DescribeCallListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCallListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_status):
             query['CallStatus'] = request.call_status
         if not UtilClient.is_unset(request.channel_id):
@@ -1488,14 +1835,21 @@
         )
 
     async def describe_call_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeCallListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeCallListResponse:
+        """
+        @summary 调用DescribeCallList分页查询时间范围内创建的通信信息。
+        
+        @param request: DescribeCallListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCallListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_status):
             query['CallStatus'] = request.call_status
         if not UtilClient.is_unset(request.channel_id):
@@ -1533,29 +1887,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_call_list(
         self,
         request: rtc_20180111_models.DescribeCallListRequest,
     ) -> rtc_20180111_models.DescribeCallListResponse:
+        """
+        @summary 调用DescribeCallList分页查询时间范围内创建的通信信息。
+        
+        @param request: DescribeCallListRequest
+        @return: DescribeCallListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_call_list_with_options(request, runtime)
 
     async def describe_call_list_async(
         self,
         request: rtc_20180111_models.DescribeCallListRequest,
     ) -> rtc_20180111_models.DescribeCallListResponse:
+        """
+        @summary 调用DescribeCallList分页查询时间范围内创建的通信信息。
+        
+        @param request: DescribeCallListRequest
+        @return: DescribeCallListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_call_list_with_options_async(request, runtime)
 
     def describe_channel_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelResponse:
+        """
+        @summary DescribeChannel
+        
+        @param request: DescribeChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -1578,14 +1951,21 @@
         )
 
     async def describe_channel_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelResponse:
+        """
+        @summary DescribeChannel
+        
+        @param request: DescribeChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -1607,29 +1987,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel(
         self,
         request: rtc_20180111_models.DescribeChannelRequest,
     ) -> rtc_20180111_models.DescribeChannelResponse:
+        """
+        @summary DescribeChannel
+        
+        @param request: DescribeChannelRequest
+        @return: DescribeChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_with_options(request, runtime)
 
     async def describe_channel_async(
         self,
         request: rtc_20180111_models.DescribeChannelRequest,
     ) -> rtc_20180111_models.DescribeChannelResponse:
+        """
+        @summary DescribeChannel
+        
+        @param request: DescribeChannelRequest
+        @return: DescribeChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_with_options_async(request, runtime)
 
     def describe_channel_all_users_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelAllUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelAllUsersResponse:
+        """
+        @summary 查询频道的所有参会者
+        
+        @param request: DescribeChannelAllUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAllUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -1652,14 +2051,21 @@
         )
 
     async def describe_channel_all_users_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelAllUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelAllUsersResponse:
+        """
+        @summary 查询频道的所有参会者
+        
+        @param request: DescribeChannelAllUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAllUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -1681,29 +2087,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_all_users(
         self,
         request: rtc_20180111_models.DescribeChannelAllUsersRequest,
     ) -> rtc_20180111_models.DescribeChannelAllUsersResponse:
+        """
+        @summary 查询频道的所有参会者
+        
+        @param request: DescribeChannelAllUsersRequest
+        @return: DescribeChannelAllUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_all_users_with_options(request, runtime)
 
     async def describe_channel_all_users_async(
         self,
         request: rtc_20180111_models.DescribeChannelAllUsersRequest,
     ) -> rtc_20180111_models.DescribeChannelAllUsersResponse:
+        """
+        @summary 查询频道的所有参会者
+        
+        @param request: DescribeChannelAllUsersRequest
+        @return: DescribeChannelAllUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_all_users_with_options_async(request, runtime)
 
     def describe_channel_area_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelAreaDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelAreaDistributionStatData获取频道地区分布统计数据。
+        
+        @param request: DescribeChannelAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1732,14 +2157,21 @@
         )
 
     async def describe_channel_area_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelAreaDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelAreaDistributionStatData获取频道地区分布统计数据。
+        
+        @param request: DescribeChannelAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1767,29 +2199,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_area_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeChannelAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeChannelAreaDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelAreaDistributionStatData获取频道地区分布统计数据。
+        
+        @param request: DescribeChannelAreaDistributionStatDataRequest
+        @return: DescribeChannelAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_area_distribution_stat_data_with_options(request, runtime)
 
     async def describe_channel_area_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeChannelAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeChannelAreaDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelAreaDistributionStatData获取频道地区分布统计数据。
+        
+        @param request: DescribeChannelAreaDistributionStatDataRequest
+        @return: DescribeChannelAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_area_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_channel_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelDistributionStatData获取频道分布统计数据。
+        
+        @param request: DescribeChannelDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1818,14 +2269,21 @@
         )
 
     async def describe_channel_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelDistributionStatData获取频道分布统计数据。
+        
+        @param request: DescribeChannelDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1853,29 +2311,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeChannelDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeChannelDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelDistributionStatData获取频道分布统计数据。
+        
+        @param request: DescribeChannelDistributionStatDataRequest
+        @return: DescribeChannelDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_distribution_stat_data_with_options(request, runtime)
 
     async def describe_channel_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeChannelDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeChannelDistributionStatDataResponse:
+        """
+        @summary 调用DescribeChannelDistributionStatData获取频道分布统计数据。
+        
+        @param request: DescribeChannelDistributionStatDataRequest
+        @return: DescribeChannelDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_channel_overall_data_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelOverallDataResponse:
+        """
+        @summary 调用DescribeChannelOverallData查询频道概览数据。
+        
+        @param request: DescribeChannelOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1902,14 +2379,21 @@
         )
 
     async def describe_channel_overall_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelOverallDataResponse:
+        """
+        @summary 调用DescribeChannelOverallData查询频道概览数据。
+        
+        @param request: DescribeChannelOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -1935,29 +2419,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_overall_data(
         self,
         request: rtc_20180111_models.DescribeChannelOverallDataRequest,
     ) -> rtc_20180111_models.DescribeChannelOverallDataResponse:
+        """
+        @summary 调用DescribeChannelOverallData查询频道概览数据。
+        
+        @param request: DescribeChannelOverallDataRequest
+        @return: DescribeChannelOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_overall_data_with_options(request, runtime)
 
     async def describe_channel_overall_data_async(
         self,
         request: rtc_20180111_models.DescribeChannelOverallDataRequest,
     ) -> rtc_20180111_models.DescribeChannelOverallDataResponse:
+        """
+        @summary 调用DescribeChannelOverallData查询频道概览数据。
+        
+        @param request: DescribeChannelOverallDataRequest
+        @return: DescribeChannelOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_overall_data_with_options_async(request, runtime)
 
     def describe_channel_participants_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelParticipantsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelParticipantsResponse:
+        """
+        @param request: DescribeChannelParticipantsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelParticipantsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.order):
@@ -1988,14 +2489,19 @@
         )
 
     async def describe_channel_participants_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelParticipantsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelParticipantsResponse:
+        """
+        @param request: DescribeChannelParticipantsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelParticipantsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.order):
@@ -2025,29 +2531,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_participants(
         self,
         request: rtc_20180111_models.DescribeChannelParticipantsRequest,
     ) -> rtc_20180111_models.DescribeChannelParticipantsResponse:
+        """
+        @param request: DescribeChannelParticipantsRequest
+        @return: DescribeChannelParticipantsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_participants_with_options(request, runtime)
 
     async def describe_channel_participants_async(
         self,
         request: rtc_20180111_models.DescribeChannelParticipantsRequest,
     ) -> rtc_20180111_models.DescribeChannelParticipantsResponse:
+        """
+        @param request: DescribeChannelParticipantsRequest
+        @return: DescribeChannelParticipantsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_participants_with_options_async(request, runtime)
 
     def describe_channel_top_pub_user_list_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelTopPubUserListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelTopPubUserListResponse:
+        """
+        @summary 调用DescribeChannelTopPubUserList获取频道内发布端的用户列表（按用户在线时长降序）。
+        
+        @param request: DescribeChannelTopPubUserListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelTopPubUserListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2074,14 +2595,21 @@
         )
 
     async def describe_channel_top_pub_user_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelTopPubUserListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelTopPubUserListResponse:
+        """
+        @summary 调用DescribeChannelTopPubUserList获取频道内发布端的用户列表（按用户在线时长降序）。
+        
+        @param request: DescribeChannelTopPubUserListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelTopPubUserListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2107,29 +2635,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_top_pub_user_list(
         self,
         request: rtc_20180111_models.DescribeChannelTopPubUserListRequest,
     ) -> rtc_20180111_models.DescribeChannelTopPubUserListResponse:
+        """
+        @summary 调用DescribeChannelTopPubUserList获取频道内发布端的用户列表（按用户在线时长降序）。
+        
+        @param request: DescribeChannelTopPubUserListRequest
+        @return: DescribeChannelTopPubUserListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_top_pub_user_list_with_options(request, runtime)
 
     async def describe_channel_top_pub_user_list_async(
         self,
         request: rtc_20180111_models.DescribeChannelTopPubUserListRequest,
     ) -> rtc_20180111_models.DescribeChannelTopPubUserListResponse:
+        """
+        @summary 调用DescribeChannelTopPubUserList获取频道内发布端的用户列表（按用户在线时长降序）。
+        
+        @param request: DescribeChannelTopPubUserListRequest
+        @return: DescribeChannelTopPubUserListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_top_pub_user_list_with_options_async(request, runtime)
 
     def describe_channel_user_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUserResponse:
+        """
+        @summary DescribeChannelUser
+        
+        @param request: DescribeChannelUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.user_id):
@@ -2154,14 +2701,21 @@
         )
 
     async def describe_channel_user_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUserResponse:
+        """
+        @summary DescribeChannelUser
+        
+        @param request: DescribeChannelUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.user_id):
@@ -2185,29 +2739,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_user(
         self,
         request: rtc_20180111_models.DescribeChannelUserRequest,
     ) -> rtc_20180111_models.DescribeChannelUserResponse:
+        """
+        @summary DescribeChannelUser
+        
+        @param request: DescribeChannelUserRequest
+        @return: DescribeChannelUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_user_with_options(request, runtime)
 
     async def describe_channel_user_async(
         self,
         request: rtc_20180111_models.DescribeChannelUserRequest,
     ) -> rtc_20180111_models.DescribeChannelUserResponse:
+        """
+        @summary DescribeChannelUser
+        
+        @param request: DescribeChannelUserRequest
+        @return: DescribeChannelUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_user_with_options_async(request, runtime)
 
     def describe_channel_user_metrics_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelUserMetricsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUserMetricsResponse:
+        """
+        @summary 调用DescribeChannelUserMetrics查询频道总览中的用户数据。
+        
+        @param request: DescribeChannelUserMetricsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUserMetricsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2234,14 +2807,21 @@
         )
 
     async def describe_channel_user_metrics_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelUserMetricsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUserMetricsResponse:
+        """
+        @summary 调用DescribeChannelUserMetrics查询频道总览中的用户数据。
+        
+        @param request: DescribeChannelUserMetricsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUserMetricsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2267,29 +2847,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_user_metrics(
         self,
         request: rtc_20180111_models.DescribeChannelUserMetricsRequest,
     ) -> rtc_20180111_models.DescribeChannelUserMetricsResponse:
+        """
+        @summary 调用DescribeChannelUserMetrics查询频道总览中的用户数据。
+        
+        @param request: DescribeChannelUserMetricsRequest
+        @return: DescribeChannelUserMetricsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_user_metrics_with_options(request, runtime)
 
     async def describe_channel_user_metrics_async(
         self,
         request: rtc_20180111_models.DescribeChannelUserMetricsRequest,
     ) -> rtc_20180111_models.DescribeChannelUserMetricsResponse:
+        """
+        @summary 调用DescribeChannelUserMetrics查询频道总览中的用户数据。
+        
+        @param request: DescribeChannelUserMetricsRequest
+        @return: DescribeChannelUserMetricsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_user_metrics_with_options_async(request, runtime)
 
     def describe_channel_users_with_options(
         self,
         request: rtc_20180111_models.DescribeChannelUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUsersResponse:
+        """
+        @param request: DescribeChannelUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -2314,14 +2911,19 @@
         )
 
     async def describe_channel_users_with_options_async(
         self,
         request: rtc_20180111_models.DescribeChannelUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeChannelUsersResponse:
+        """
+        @param request: DescribeChannelUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -2345,29 +2947,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_users(
         self,
         request: rtc_20180111_models.DescribeChannelUsersRequest,
     ) -> rtc_20180111_models.DescribeChannelUsersResponse:
+        """
+        @param request: DescribeChannelUsersRequest
+        @return: DescribeChannelUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_users_with_options(request, runtime)
 
     async def describe_channel_users_async(
         self,
         request: rtc_20180111_models.DescribeChannelUsersRequest,
     ) -> rtc_20180111_models.DescribeChannelUsersResponse:
+        """
+        @param request: DescribeChannelUsersRequest
+        @return: DescribeChannelUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_users_with_options_async(request, runtime)
 
     def describe_end_point_event_list_with_options(
         self,
         request: rtc_20180111_models.DescribeEndPointEventListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeEndPointEventListResponse:
+        """
+        @summary 调用DescribeEndPointEventList获取端对端用户事件列表。
+        
+        @param request: DescribeEndPointEventListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEndPointEventListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2396,14 +3013,21 @@
         )
 
     async def describe_end_point_event_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeEndPointEventListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeEndPointEventListResponse:
+        """
+        @summary 调用DescribeEndPointEventList获取端对端用户事件列表。
+        
+        @param request: DescribeEndPointEventListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEndPointEventListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2431,29 +3055,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_end_point_event_list(
         self,
         request: rtc_20180111_models.DescribeEndPointEventListRequest,
     ) -> rtc_20180111_models.DescribeEndPointEventListResponse:
+        """
+        @summary 调用DescribeEndPointEventList获取端对端用户事件列表。
+        
+        @param request: DescribeEndPointEventListRequest
+        @return: DescribeEndPointEventListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_end_point_event_list_with_options(request, runtime)
 
     async def describe_end_point_event_list_async(
         self,
         request: rtc_20180111_models.DescribeEndPointEventListRequest,
     ) -> rtc_20180111_models.DescribeEndPointEventListResponse:
+        """
+        @summary 调用DescribeEndPointEventList获取端对端用户事件列表。
+        
+        @param request: DescribeEndPointEventListRequest
+        @return: DescribeEndPointEventListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_end_point_event_list_with_options_async(request, runtime)
 
     def describe_end_point_metric_data_with_options(
         self,
         request: rtc_20180111_models.DescribeEndPointMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeEndPointMetricDataResponse:
+        """
+        @summary 调用DescribeEndPointMetricData获取端对端指标数据。
+        
+        @param request: DescribeEndPointMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEndPointMetricDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2488,14 +3131,21 @@
         )
 
     async def describe_end_point_metric_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeEndPointMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeEndPointMetricDataResponse:
+        """
+        @summary 调用DescribeEndPointMetricData获取端对端指标数据。
+        
+        @param request: DescribeEndPointMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEndPointMetricDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2529,29 +3179,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_end_point_metric_data(
         self,
         request: rtc_20180111_models.DescribeEndPointMetricDataRequest,
     ) -> rtc_20180111_models.DescribeEndPointMetricDataResponse:
+        """
+        @summary 调用DescribeEndPointMetricData获取端对端指标数据。
+        
+        @param request: DescribeEndPointMetricDataRequest
+        @return: DescribeEndPointMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_end_point_metric_data_with_options(request, runtime)
 
     async def describe_end_point_metric_data_async(
         self,
         request: rtc_20180111_models.DescribeEndPointMetricDataRequest,
     ) -> rtc_20180111_models.DescribeEndPointMetricDataResponse:
+        """
+        @summary 调用DescribeEndPointMetricData获取端对端指标数据。
+        
+        @param request: DescribeEndPointMetricDataRequest
+        @return: DescribeEndPointMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_end_point_metric_data_with_options_async(request, runtime)
 
     def describe_fault_diagnosis_factor_distribution_stat_with_options(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatResponse:
+        """
+        @summary 获取异常诊断影响因素分布
+        
+        @param request: DescribeFaultDiagnosisFactorDistributionStatRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisFactorDistributionStatResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_ts):
             query['EndTs'] = request.end_ts
         if not UtilClient.is_unset(request.start_ts):
@@ -2576,14 +3245,21 @@
         )
 
     async def describe_fault_diagnosis_factor_distribution_stat_with_options_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatResponse:
+        """
+        @summary 获取异常诊断影响因素分布
+        
+        @param request: DescribeFaultDiagnosisFactorDistributionStatRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisFactorDistributionStatResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_ts):
             query['EndTs'] = request.end_ts
         if not UtilClient.is_unset(request.start_ts):
@@ -2607,29 +3283,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_fault_diagnosis_factor_distribution_stat(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatResponse:
+        """
+        @summary 获取异常诊断影响因素分布
+        
+        @param request: DescribeFaultDiagnosisFactorDistributionStatRequest
+        @return: DescribeFaultDiagnosisFactorDistributionStatResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_fault_diagnosis_factor_distribution_stat_with_options(request, runtime)
 
     async def describe_fault_diagnosis_factor_distribution_stat_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisFactorDistributionStatResponse:
+        """
+        @summary 获取异常诊断影响因素分布
+        
+        @param request: DescribeFaultDiagnosisFactorDistributionStatRequest
+        @return: DescribeFaultDiagnosisFactorDistributionStatResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_fault_diagnosis_factor_distribution_stat_with_options_async(request, runtime)
 
     def describe_fault_diagnosis_overall_data_with_options(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisOverallDataResponse:
+        """
+        @summary 获取异常诊断总览数据
+        
+        @param request: DescribeFaultDiagnosisOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_ts):
             query['EndTs'] = request.end_ts
         if not UtilClient.is_unset(request.start_ts):
@@ -2656,14 +3351,21 @@
         )
 
     async def describe_fault_diagnosis_overall_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisOverallDataResponse:
+        """
+        @summary 获取异常诊断总览数据
+        
+        @param request: DescribeFaultDiagnosisOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_ts):
             query['EndTs'] = request.end_ts
         if not UtilClient.is_unset(request.start_ts):
@@ -2689,29 +3391,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_fault_diagnosis_overall_data(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisOverallDataRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisOverallDataResponse:
+        """
+        @summary 获取异常诊断总览数据
+        
+        @param request: DescribeFaultDiagnosisOverallDataRequest
+        @return: DescribeFaultDiagnosisOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_fault_diagnosis_overall_data_with_options(request, runtime)
 
     async def describe_fault_diagnosis_overall_data_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisOverallDataRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisOverallDataResponse:
+        """
+        @summary 获取异常诊断总览数据
+        
+        @param request: DescribeFaultDiagnosisOverallDataRequest
+        @return: DescribeFaultDiagnosisOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_fault_diagnosis_overall_data_with_options_async(request, runtime)
 
     def describe_fault_diagnosis_user_detail_with_options(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserDetailResponse:
+        """
+        @summary 获取异常诊断用户详情
+        
+        @param request: DescribeFaultDiagnosisUserDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisUserDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2742,14 +3463,21 @@
         )
 
     async def describe_fault_diagnosis_user_detail_with_options_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserDetailResponse:
+        """
+        @summary 获取异常诊断用户详情
+        
+        @param request: DescribeFaultDiagnosisUserDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisUserDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -2779,29 +3507,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_fault_diagnosis_user_detail(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserDetailRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserDetailResponse:
+        """
+        @summary 获取异常诊断用户详情
+        
+        @param request: DescribeFaultDiagnosisUserDetailRequest
+        @return: DescribeFaultDiagnosisUserDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_fault_diagnosis_user_detail_with_options(request, runtime)
 
     async def describe_fault_diagnosis_user_detail_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserDetailRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserDetailResponse:
+        """
+        @summary 获取异常诊断用户详情
+        
+        @param request: DescribeFaultDiagnosisUserDetailRequest
+        @return: DescribeFaultDiagnosisUserDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_fault_diagnosis_user_detail_with_options_async(request, runtime)
 
     def describe_fault_diagnosis_user_list_with_options(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserListResponse:
+        """
+        @summary 获取异常诊断用户明细列表
+        
+        @param request: DescribeFaultDiagnosisUserListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisUserListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.end_ts):
@@ -2836,14 +3583,21 @@
         )
 
     async def describe_fault_diagnosis_user_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserListResponse:
+        """
+        @summary 获取异常诊断用户明细列表
+        
+        @param request: DescribeFaultDiagnosisUserListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeFaultDiagnosisUserListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.end_ts):
@@ -2877,29 +3631,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_fault_diagnosis_user_list(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserListRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserListResponse:
+        """
+        @summary 获取异常诊断用户明细列表
+        
+        @param request: DescribeFaultDiagnosisUserListRequest
+        @return: DescribeFaultDiagnosisUserListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_fault_diagnosis_user_list_with_options(request, runtime)
 
     async def describe_fault_diagnosis_user_list_async(
         self,
         request: rtc_20180111_models.DescribeFaultDiagnosisUserListRequest,
     ) -> rtc_20180111_models.DescribeFaultDiagnosisUserListResponse:
+        """
+        @summary 获取异常诊断用户明细列表
+        
+        @param request: DescribeFaultDiagnosisUserListRequest
+        @return: DescribeFaultDiagnosisUserListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_fault_diagnosis_user_list_with_options_async(request, runtime)
 
     def describe_mpulayout_info_list_with_options(
         self,
         request: rtc_20180111_models.DescribeMPULayoutInfoListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeMPULayoutInfoListResponse:
+        """
+        @param request: DescribeMPULayoutInfoListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMPULayoutInfoListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.layout_id):
             query['LayoutId'] = request.layout_id
         if not UtilClient.is_unset(request.name):
@@ -2930,14 +3701,19 @@
         )
 
     async def describe_mpulayout_info_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeMPULayoutInfoListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeMPULayoutInfoListResponse:
+        """
+        @param request: DescribeMPULayoutInfoListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMPULayoutInfoListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.layout_id):
             query['LayoutId'] = request.layout_id
         if not UtilClient.is_unset(request.name):
@@ -2967,29 +3743,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_mpulayout_info_list(
         self,
         request: rtc_20180111_models.DescribeMPULayoutInfoListRequest,
     ) -> rtc_20180111_models.DescribeMPULayoutInfoListResponse:
+        """
+        @param request: DescribeMPULayoutInfoListRequest
+        @return: DescribeMPULayoutInfoListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_mpulayout_info_list_with_options(request, runtime)
 
     async def describe_mpulayout_info_list_async(
         self,
         request: rtc_20180111_models.DescribeMPULayoutInfoListRequest,
     ) -> rtc_20180111_models.DescribeMPULayoutInfoListResponse:
+        """
+        @param request: DescribeMPULayoutInfoListRequest
+        @return: DescribeMPULayoutInfoListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_mpulayout_info_list_with_options_async(request, runtime)
 
     def describe_pub_user_list_by_sub_user_with_options(
         self,
         request: rtc_20180111_models.DescribePubUserListBySubUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribePubUserListBySubUserResponse:
+        """
+        @summary 调用DescribePubUserListBySubUser根据订阅端获取通信中发布端用户列表。
+        
+        @param request: DescribePubUserListBySubUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePubUserListBySubUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -3018,14 +3809,21 @@
         )
 
     async def describe_pub_user_list_by_sub_user_with_options_async(
         self,
         request: rtc_20180111_models.DescribePubUserListBySubUserRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribePubUserListBySubUserResponse:
+        """
+        @summary 调用DescribePubUserListBySubUser根据订阅端获取通信中发布端用户列表。
+        
+        @param request: DescribePubUserListBySubUserRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePubUserListBySubUserResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -3053,29 +3851,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_pub_user_list_by_sub_user(
         self,
         request: rtc_20180111_models.DescribePubUserListBySubUserRequest,
     ) -> rtc_20180111_models.DescribePubUserListBySubUserResponse:
+        """
+        @summary 调用DescribePubUserListBySubUser根据订阅端获取通信中发布端用户列表。
+        
+        @param request: DescribePubUserListBySubUserRequest
+        @return: DescribePubUserListBySubUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_pub_user_list_by_sub_user_with_options(request, runtime)
 
     async def describe_pub_user_list_by_sub_user_async(
         self,
         request: rtc_20180111_models.DescribePubUserListBySubUserRequest,
     ) -> rtc_20180111_models.DescribePubUserListBySubUserResponse:
+        """
+        @summary 调用DescribePubUserListBySubUser根据订阅端获取通信中发布端用户列表。
+        
+        @param request: DescribePubUserListBySubUserRequest
+        @return: DescribePubUserListBySubUserResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_pub_user_list_by_sub_user_with_options_async(request, runtime)
 
     def describe_qoe_metric_data_with_options(
         self,
         request: rtc_20180111_models.DescribeQoeMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQoeMetricDataResponse:
+        """
+        @summary 调用DescribeQoeMetricData获取单次通信中用户的下行体验质量指标。
+        
+        @param request: DescribeQoeMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQoeMetricDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -3104,14 +3921,21 @@
         )
 
     async def describe_qoe_metric_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeQoeMetricDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQoeMetricDataResponse:
+        """
+        @summary 调用DescribeQoeMetricData获取单次通信中用户的下行体验质量指标。
+        
+        @param request: DescribeQoeMetricDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQoeMetricDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.created_ts):
@@ -3139,29 +3963,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_qoe_metric_data(
         self,
         request: rtc_20180111_models.DescribeQoeMetricDataRequest,
     ) -> rtc_20180111_models.DescribeQoeMetricDataResponse:
+        """
+        @summary 调用DescribeQoeMetricData获取单次通信中用户的下行体验质量指标。
+        
+        @param request: DescribeQoeMetricDataRequest
+        @return: DescribeQoeMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_qoe_metric_data_with_options(request, runtime)
 
     async def describe_qoe_metric_data_async(
         self,
         request: rtc_20180111_models.DescribeQoeMetricDataRequest,
     ) -> rtc_20180111_models.DescribeQoeMetricDataResponse:
+        """
+        @summary 调用DescribeQoeMetricData获取单次通信中用户的下行体验质量指标。
+        
+        @param request: DescribeQoeMetricDataRequest
+        @return: DescribeQoeMetricDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_qoe_metric_data_with_options_async(request, runtime)
 
     def describe_quality_area_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeQualityAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityAreaDistributionStatDataResponse:
+        """
+        @summary 获取质量统计区域分布统计数据
+        
+        @param request: DescribeQualityAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.parent_area):
@@ -3188,14 +4031,21 @@
         )
 
     async def describe_quality_area_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeQualityAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityAreaDistributionStatDataResponse:
+        """
+        @summary 获取质量统计区域分布统计数据
+        
+        @param request: DescribeQualityAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.parent_area):
@@ -3221,29 +4071,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_quality_area_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeQualityAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityAreaDistributionStatDataResponse:
+        """
+        @summary 获取质量统计区域分布统计数据
+        
+        @param request: DescribeQualityAreaDistributionStatDataRequest
+        @return: DescribeQualityAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_quality_area_distribution_stat_data_with_options(request, runtime)
 
     async def describe_quality_area_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeQualityAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityAreaDistributionStatDataResponse:
+        """
+        @summary 获取质量统计区域分布统计数据
+        
+        @param request: DescribeQualityAreaDistributionStatDataRequest
+        @return: DescribeQualityAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_quality_area_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_quality_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeQualityDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityDistributionStatDataResponse:
+        """
+        @summary 获取质量统计分布数据
+        
+        @param request: DescribeQualityDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3270,14 +4139,21 @@
         )
 
     async def describe_quality_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeQualityDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityDistributionStatDataResponse:
+        """
+        @summary 获取质量统计分布数据
+        
+        @param request: DescribeQualityDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3303,29 +4179,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_quality_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeQualityDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityDistributionStatDataResponse:
+        """
+        @summary 获取质量统计分布数据
+        
+        @param request: DescribeQualityDistributionStatDataRequest
+        @return: DescribeQualityDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_quality_distribution_stat_data_with_options(request, runtime)
 
     async def describe_quality_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeQualityDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityDistributionStatDataResponse:
+        """
+        @summary 获取质量统计分布数据
+        
+        @param request: DescribeQualityDistributionStatDataRequest
+        @return: DescribeQualityDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_quality_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_quality_os_sdk_version_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取质量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeQualityOsSdkVersionDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityOsSdkVersionDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3350,14 +4245,21 @@
         )
 
     async def describe_quality_os_sdk_version_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取质量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeQualityOsSdkVersionDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityOsSdkVersionDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3381,29 +4283,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_quality_os_sdk_version_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取质量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeQualityOsSdkVersionDistributionStatDataRequest
+        @return: DescribeQualityOsSdkVersionDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_quality_os_sdk_version_distribution_stat_data_with_options(request, runtime)
 
     async def describe_quality_os_sdk_version_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeQualityOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取质量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeQualityOsSdkVersionDistributionStatDataRequest
+        @return: DescribeQualityOsSdkVersionDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_quality_os_sdk_version_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_quality_overall_data_with_options(
         self,
         request: rtc_20180111_models.DescribeQualityOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityOverallDataResponse:
+        """
+        @summary 获取质量统计概览数据
+        
+        @param request: DescribeQualityOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3430,14 +4351,21 @@
         )
 
     async def describe_quality_overall_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeQualityOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeQualityOverallDataResponse:
+        """
+        @summary 获取质量统计概览数据
+        
+        @param request: DescribeQualityOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeQualityOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -3463,29 +4391,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_quality_overall_data(
         self,
         request: rtc_20180111_models.DescribeQualityOverallDataRequest,
     ) -> rtc_20180111_models.DescribeQualityOverallDataResponse:
+        """
+        @summary 获取质量统计概览数据
+        
+        @param request: DescribeQualityOverallDataRequest
+        @return: DescribeQualityOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_quality_overall_data_with_options(request, runtime)
 
     async def describe_quality_overall_data_async(
         self,
         request: rtc_20180111_models.DescribeQualityOverallDataRequest,
     ) -> rtc_20180111_models.DescribeQualityOverallDataResponse:
+        """
+        @summary 获取质量统计概览数据
+        
+        @param request: DescribeQualityOverallDataRequest
+        @return: DescribeQualityOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_quality_overall_data_with_options_async(request, runtime)
 
     def describe_record_files_with_options(
         self,
         request: rtc_20180111_models.DescribeRecordFilesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRecordFilesResponse:
+        """
+        @param request: DescribeRecordFilesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRecordFilesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.end_time):
@@ -3520,14 +4465,19 @@
         )
 
     async def describe_record_files_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRecordFilesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRecordFilesResponse:
+        """
+        @param request: DescribeRecordFilesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRecordFilesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.end_time):
@@ -3561,29 +4511,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_record_files(
         self,
         request: rtc_20180111_models.DescribeRecordFilesRequest,
     ) -> rtc_20180111_models.DescribeRecordFilesResponse:
+        """
+        @param request: DescribeRecordFilesRequest
+        @return: DescribeRecordFilesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_record_files_with_options(request, runtime)
 
     async def describe_record_files_async(
         self,
         request: rtc_20180111_models.DescribeRecordFilesRequest,
     ) -> rtc_20180111_models.DescribeRecordFilesResponse:
+        """
+        @param request: DescribeRecordFilesRequest
+        @return: DescribeRecordFilesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_record_files_with_options_async(request, runtime)
 
     def describe_record_templates_with_options(
         self,
         request: rtc_20180111_models.DescribeRecordTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRecordTemplatesResponse:
+        """
+        @param request: DescribeRecordTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRecordTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -3612,14 +4575,19 @@
         )
 
     async def describe_record_templates_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRecordTemplatesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRecordTemplatesResponse:
+        """
+        @param request: DescribeRecordTemplatesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRecordTemplatesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -3647,29 +4615,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_record_templates(
         self,
         request: rtc_20180111_models.DescribeRecordTemplatesRequest,
     ) -> rtc_20180111_models.DescribeRecordTemplatesResponse:
+        """
+        @param request: DescribeRecordTemplatesRequest
+        @return: DescribeRecordTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_record_templates_with_options(request, runtime)
 
     async def describe_record_templates_async(
         self,
         request: rtc_20180111_models.DescribeRecordTemplatesRequest,
     ) -> rtc_20180111_models.DescribeRecordTemplatesResponse:
+        """
+        @param request: DescribeRecordTemplatesRequest
+        @return: DescribeRecordTemplatesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_record_templates_with_options_async(request, runtime)
 
     def describe_rtc_channel_list_with_options(
         self,
         request: rtc_20180111_models.DescribeRtcChannelListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcChannelListResponse:
+        """
+        @param request: DescribeRtcChannelListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcChannelListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3706,14 +4687,19 @@
         )
 
     async def describe_rtc_channel_list_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRtcChannelListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcChannelListResponse:
+        """
+        @param request: DescribeRtcChannelListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcChannelListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3749,29 +4735,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_rtc_channel_list(
         self,
         request: rtc_20180111_models.DescribeRtcChannelListRequest,
     ) -> rtc_20180111_models.DescribeRtcChannelListResponse:
+        """
+        @param request: DescribeRtcChannelListRequest
+        @return: DescribeRtcChannelListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_rtc_channel_list_with_options(request, runtime)
 
     async def describe_rtc_channel_list_async(
         self,
         request: rtc_20180111_models.DescribeRtcChannelListRequest,
     ) -> rtc_20180111_models.DescribeRtcChannelListResponse:
+        """
+        @param request: DescribeRtcChannelListRequest
+        @return: DescribeRtcChannelListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_rtc_channel_list_with_options_async(request, runtime)
 
     def describe_rtc_channel_metric_with_options(
         self,
         request: rtc_20180111_models.DescribeRtcChannelMetricRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcChannelMetricResponse:
+        """
+        @param request: DescribeRtcChannelMetricRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcChannelMetricResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3798,14 +4797,19 @@
         )
 
     async def describe_rtc_channel_metric_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRtcChannelMetricRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcChannelMetricResponse:
+        """
+        @param request: DescribeRtcChannelMetricRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcChannelMetricResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3831,29 +4835,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_rtc_channel_metric(
         self,
         request: rtc_20180111_models.DescribeRtcChannelMetricRequest,
     ) -> rtc_20180111_models.DescribeRtcChannelMetricResponse:
+        """
+        @param request: DescribeRtcChannelMetricRequest
+        @return: DescribeRtcChannelMetricResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_rtc_channel_metric_with_options(request, runtime)
 
     async def describe_rtc_channel_metric_async(
         self,
         request: rtc_20180111_models.DescribeRtcChannelMetricRequest,
     ) -> rtc_20180111_models.DescribeRtcChannelMetricResponse:
+        """
+        @param request: DescribeRtcChannelMetricRequest
+        @return: DescribeRtcChannelMetricResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_rtc_channel_metric_with_options_async(request, runtime)
 
     def describe_rtc_duration_data_with_options(
         self,
         request: rtc_20180111_models.DescribeRtcDurationDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcDurationDataResponse:
+        """
+        @param request: DescribeRtcDurationDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcDurationDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -3884,14 +4901,19 @@
         )
 
     async def describe_rtc_duration_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRtcDurationDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcDurationDataResponse:
+        """
+        @param request: DescribeRtcDurationDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcDurationDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -3921,29 +4943,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_rtc_duration_data(
         self,
         request: rtc_20180111_models.DescribeRtcDurationDataRequest,
     ) -> rtc_20180111_models.DescribeRtcDurationDataResponse:
+        """
+        @param request: DescribeRtcDurationDataRequest
+        @return: DescribeRtcDurationDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_rtc_duration_data_with_options(request, runtime)
 
     async def describe_rtc_duration_data_async(
         self,
         request: rtc_20180111_models.DescribeRtcDurationDataRequest,
     ) -> rtc_20180111_models.DescribeRtcDurationDataResponse:
+        """
+        @param request: DescribeRtcDurationDataRequest
+        @return: DescribeRtcDurationDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_rtc_duration_data_with_options_async(request, runtime)
 
     def describe_rtc_peak_channel_cnt_data_with_options(
         self,
         request: rtc_20180111_models.DescribeRtcPeakChannelCntDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcPeakChannelCntDataResponse:
+        """
+        @param request: DescribeRtcPeakChannelCntDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcPeakChannelCntDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -3974,14 +5009,19 @@
         )
 
     async def describe_rtc_peak_channel_cnt_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRtcPeakChannelCntDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcPeakChannelCntDataResponse:
+        """
+        @param request: DescribeRtcPeakChannelCntDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcPeakChannelCntDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -4011,29 +5051,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_rtc_peak_channel_cnt_data(
         self,
         request: rtc_20180111_models.DescribeRtcPeakChannelCntDataRequest,
     ) -> rtc_20180111_models.DescribeRtcPeakChannelCntDataResponse:
+        """
+        @param request: DescribeRtcPeakChannelCntDataRequest
+        @return: DescribeRtcPeakChannelCntDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_rtc_peak_channel_cnt_data_with_options(request, runtime)
 
     async def describe_rtc_peak_channel_cnt_data_async(
         self,
         request: rtc_20180111_models.DescribeRtcPeakChannelCntDataRequest,
     ) -> rtc_20180111_models.DescribeRtcPeakChannelCntDataResponse:
+        """
+        @param request: DescribeRtcPeakChannelCntDataRequest
+        @return: DescribeRtcPeakChannelCntDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_rtc_peak_channel_cnt_data_with_options_async(request, runtime)
 
     def describe_rtc_user_cnt_data_with_options(
         self,
         request: rtc_20180111_models.DescribeRtcUserCntDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcUserCntDataResponse:
+        """
+        @param request: DescribeRtcUserCntDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcUserCntDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -4064,14 +5117,19 @@
         )
 
     async def describe_rtc_user_cnt_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeRtcUserCntDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeRtcUserCntDataResponse:
+        """
+        @param request: DescribeRtcUserCntDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeRtcUserCntDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.interval):
@@ -4101,29 +5159,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_rtc_user_cnt_data(
         self,
         request: rtc_20180111_models.DescribeRtcUserCntDataRequest,
     ) -> rtc_20180111_models.DescribeRtcUserCntDataResponse:
+        """
+        @param request: DescribeRtcUserCntDataRequest
+        @return: DescribeRtcUserCntDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_rtc_user_cnt_data_with_options(request, runtime)
 
     async def describe_rtc_user_cnt_data_async(
         self,
         request: rtc_20180111_models.DescribeRtcUserCntDataRequest,
     ) -> rtc_20180111_models.DescribeRtcUserCntDataResponse:
+        """
+        @param request: DescribeRtcUserCntDataRequest
+        @return: DescribeRtcUserCntDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_rtc_user_cnt_data_with_options_async(request, runtime)
 
     def describe_usage_area_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeUsageAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageAreaDistributionStatDataResponse:
+        """
+        @summary 获取用量统计地域分布数据
+        
+        @param request: DescribeUsageAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.parent_area):
@@ -4150,14 +5223,21 @@
         )
 
     async def describe_usage_area_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeUsageAreaDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageAreaDistributionStatDataResponse:
+        """
+        @summary 获取用量统计地域分布数据
+        
+        @param request: DescribeUsageAreaDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageAreaDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.parent_area):
@@ -4183,29 +5263,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_usage_area_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeUsageAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageAreaDistributionStatDataResponse:
+        """
+        @summary 获取用量统计地域分布数据
+        
+        @param request: DescribeUsageAreaDistributionStatDataRequest
+        @return: DescribeUsageAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_usage_area_distribution_stat_data_with_options(request, runtime)
 
     async def describe_usage_area_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeUsageAreaDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageAreaDistributionStatDataResponse:
+        """
+        @summary 获取用量统计地域分布数据
+        
+        @param request: DescribeUsageAreaDistributionStatDataRequest
+        @return: DescribeUsageAreaDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_usage_area_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_usage_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeUsageDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageDistributionStatDataResponse:
+        """
+        @summary 获取用量统计分布数据
+        
+        @param request: DescribeUsageDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4232,14 +5331,21 @@
         )
 
     async def describe_usage_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeUsageDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageDistributionStatDataResponse:
+        """
+        @summary 获取用量统计分布数据
+        
+        @param request: DescribeUsageDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4265,29 +5371,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_usage_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeUsageDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageDistributionStatDataResponse:
+        """
+        @summary 获取用量统计分布数据
+        
+        @param request: DescribeUsageDistributionStatDataRequest
+        @return: DescribeUsageDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_usage_distribution_stat_data_with_options(request, runtime)
 
     async def describe_usage_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeUsageDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageDistributionStatDataResponse:
+        """
+        @summary 获取用量统计分布数据
+        
+        @param request: DescribeUsageDistributionStatDataRequest
+        @return: DescribeUsageDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_usage_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_usage_os_sdk_version_distribution_stat_data_with_options(
         self,
         request: rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取用量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeUsageOsSdkVersionDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageOsSdkVersionDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4312,14 +5437,21 @@
         )
 
     async def describe_usage_os_sdk_version_distribution_stat_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取用量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeUsageOsSdkVersionDistributionStatDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageOsSdkVersionDistributionStatDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4343,29 +5475,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_usage_os_sdk_version_distribution_stat_data(
         self,
         request: rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取用量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeUsageOsSdkVersionDistributionStatDataRequest
+        @return: DescribeUsageOsSdkVersionDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_usage_os_sdk_version_distribution_stat_data_with_options(request, runtime)
 
     async def describe_usage_os_sdk_version_distribution_stat_data_async(
         self,
         request: rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataRequest,
     ) -> rtc_20180111_models.DescribeUsageOsSdkVersionDistributionStatDataResponse:
+        """
+        @summary 获取用量统计各操作系统下SDK版本分布数据
+        
+        @param request: DescribeUsageOsSdkVersionDistributionStatDataRequest
+        @return: DescribeUsageOsSdkVersionDistributionStatDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_usage_os_sdk_version_distribution_stat_data_with_options_async(request, runtime)
 
     def describe_usage_overall_data_with_options(
         self,
         request: rtc_20180111_models.DescribeUsageOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageOverallDataResponse:
+        """
+        @summary 获取用量统计概览数据
+        
+        @param request: DescribeUsageOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4392,14 +5543,21 @@
         )
 
     async def describe_usage_overall_data_with_options_async(
         self,
         request: rtc_20180111_models.DescribeUsageOverallDataRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUsageOverallDataResponse:
+        """
+        @summary 获取用量统计概览数据
+        
+        @param request: DescribeUsageOverallDataRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUsageOverallDataResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.end_date):
             query['EndDate'] = request.end_date
         if not UtilClient.is_unset(request.start_date):
@@ -4425,29 +5583,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_usage_overall_data(
         self,
         request: rtc_20180111_models.DescribeUsageOverallDataRequest,
     ) -> rtc_20180111_models.DescribeUsageOverallDataResponse:
+        """
+        @summary 获取用量统计概览数据
+        
+        @param request: DescribeUsageOverallDataRequest
+        @return: DescribeUsageOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_usage_overall_data_with_options(request, runtime)
 
     async def describe_usage_overall_data_async(
         self,
         request: rtc_20180111_models.DescribeUsageOverallDataRequest,
     ) -> rtc_20180111_models.DescribeUsageOverallDataResponse:
+        """
+        @summary 获取用量统计概览数据
+        
+        @param request: DescribeUsageOverallDataRequest
+        @return: DescribeUsageOverallDataResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_usage_overall_data_with_options_async(request, runtime)
 
     def describe_user_info_in_channel_with_options(
         self,
         request: rtc_20180111_models.DescribeUserInfoInChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUserInfoInChannelResponse:
+        """
+        @param request: DescribeUserInfoInChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUserInfoInChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -4474,14 +5649,19 @@
         )
 
     async def describe_user_info_in_channel_with_options_async(
         self,
         request: rtc_20180111_models.DescribeUserInfoInChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DescribeUserInfoInChannelResponse:
+        """
+        @param request: DescribeUserInfoInChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeUserInfoInChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -4507,29 +5687,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_user_info_in_channel(
         self,
         request: rtc_20180111_models.DescribeUserInfoInChannelRequest,
     ) -> rtc_20180111_models.DescribeUserInfoInChannelResponse:
+        """
+        @param request: DescribeUserInfoInChannelRequest
+        @return: DescribeUserInfoInChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_user_info_in_channel_with_options(request, runtime)
 
     async def describe_user_info_in_channel_async(
         self,
         request: rtc_20180111_models.DescribeUserInfoInChannelRequest,
     ) -> rtc_20180111_models.DescribeUserInfoInChannelResponse:
+        """
+        @param request: DescribeUserInfoInChannelRequest
+        @return: DescribeUserInfoInChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_user_info_in_channel_with_options_async(request, runtime)
 
     def disable_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.DisableAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DisableAutoLiveStreamRuleResponse:
+        """
+        @param request: DisableAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -4554,14 +5747,19 @@
         )
 
     async def disable_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.DisableAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.DisableAutoLiveStreamRuleResponse:
+        """
+        @param request: DisableAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DisableAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -4585,29 +5783,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def disable_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.DisableAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DisableAutoLiveStreamRuleResponse:
+        """
+        @param request: DisableAutoLiveStreamRuleRequest
+        @return: DisableAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.disable_auto_live_stream_rule_with_options(request, runtime)
 
     async def disable_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.DisableAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.DisableAutoLiveStreamRuleResponse:
+        """
+        @param request: DisableAutoLiveStreamRuleRequest
+        @return: DisableAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.disable_auto_live_stream_rule_with_options_async(request, runtime)
 
     def enable_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.EnableAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.EnableAutoLiveStreamRuleResponse:
+        """
+        @param request: EnableAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -4632,14 +5843,19 @@
         )
 
     async def enable_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.EnableAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.EnableAutoLiveStreamRuleResponse:
+        """
+        @param request: EnableAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: EnableAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.rule_id):
@@ -4663,29 +5879,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def enable_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.EnableAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.EnableAutoLiveStreamRuleResponse:
+        """
+        @param request: EnableAutoLiveStreamRuleRequest
+        @return: EnableAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.enable_auto_live_stream_rule_with_options(request, runtime)
 
     async def enable_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.EnableAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.EnableAutoLiveStreamRuleResponse:
+        """
+        @param request: EnableAutoLiveStreamRuleRequest
+        @return: EnableAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.enable_auto_live_stream_rule_with_options_async(request, runtime)
 
     def get_mputask_status_with_options(
         self,
         request: rtc_20180111_models.GetMPUTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.GetMPUTaskStatusResponse:
+        """
+        @param request: GetMPUTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMPUTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -4710,14 +5939,19 @@
         )
 
     async def get_mputask_status_with_options_async(
         self,
         request: rtc_20180111_models.GetMPUTaskStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.GetMPUTaskStatusResponse:
+        """
+        @param request: GetMPUTaskStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMPUTaskStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -4741,29 +5975,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_mputask_status(
         self,
         request: rtc_20180111_models.GetMPUTaskStatusRequest,
     ) -> rtc_20180111_models.GetMPUTaskStatusResponse:
+        """
+        @param request: GetMPUTaskStatusRequest
+        @return: GetMPUTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.get_mputask_status_with_options(request, runtime)
 
     async def get_mputask_status_async(
         self,
         request: rtc_20180111_models.GetMPUTaskStatusRequest,
     ) -> rtc_20180111_models.GetMPUTaskStatusResponse:
+        """
+        @param request: GetMPUTaskStatusRequest
+        @return: GetMPUTaskStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.get_mputask_status_with_options_async(request, runtime)
 
     def modify_app_with_options(
         self,
         request: rtc_20180111_models.ModifyAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyAppResponse:
+        """
+        @summary 修改App信息
+        
+        @param request: ModifyAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAppResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.owner_id):
@@ -4788,14 +6037,21 @@
         )
 
     async def modify_app_with_options_async(
         self,
         request: rtc_20180111_models.ModifyAppRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyAppResponse:
+        """
+        @summary 修改App信息
+        
+        @param request: ModifyAppRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAppResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.app_name):
             query['AppName'] = request.app_name
         if not UtilClient.is_unset(request.owner_id):
@@ -4819,29 +6075,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_app(
         self,
         request: rtc_20180111_models.ModifyAppRequest,
     ) -> rtc_20180111_models.ModifyAppResponse:
+        """
+        @summary 修改App信息
+        
+        @param request: ModifyAppRequest
+        @return: ModifyAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_app_with_options(request, runtime)
 
     async def modify_app_async(
         self,
         request: rtc_20180111_models.ModifyAppRequest,
     ) -> rtc_20180111_models.ModifyAppResponse:
+        """
+        @summary 修改App信息
+        
+        @param request: ModifyAppRequest
+        @return: ModifyAppResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_app_with_options_async(request, runtime)
 
     def modify_app_streaming_out_template_with_options(
         self,
         tmp_req: rtc_20180111_models.ModifyAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyAppStreamingOutTemplateResponse:
+        """
+        @summary 更新应用推流模版
+        
+        @param tmp_req: ModifyAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.ModifyAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -4868,14 +6143,21 @@
         )
 
     async def modify_app_streaming_out_template_with_options_async(
         self,
         tmp_req: rtc_20180111_models.ModifyAppStreamingOutTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyAppStreamingOutTemplateResponse:
+        """
+        @summary 更新应用推流模版
+        
+        @param tmp_req: ModifyAppStreamingOutTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyAppStreamingOutTemplateResponse
+        """
         UtilClient.validate_model(tmp_req)
         request = rtc_20180111_models.ModifyAppStreamingOutTemplateShrinkRequest()
         OpenApiUtilClient.convert(tmp_req, request)
         if not UtilClient.is_unset(tmp_req.streaming_out_template):
             request.streaming_out_template_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.streaming_out_template, 'StreamingOutTemplate', 'json')
         query = {}
         if not UtilClient.is_unset(request.app_id):
@@ -4901,29 +6183,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_app_streaming_out_template(
         self,
         request: rtc_20180111_models.ModifyAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.ModifyAppStreamingOutTemplateResponse:
+        """
+        @summary 更新应用推流模版
+        
+        @param request: ModifyAppStreamingOutTemplateRequest
+        @return: ModifyAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_app_streaming_out_template_with_options(request, runtime)
 
     async def modify_app_streaming_out_template_async(
         self,
         request: rtc_20180111_models.ModifyAppStreamingOutTemplateRequest,
     ) -> rtc_20180111_models.ModifyAppStreamingOutTemplateResponse:
+        """
+        @summary 更新应用推流模版
+        
+        @param request: ModifyAppStreamingOutTemplateRequest
+        @return: ModifyAppStreamingOutTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_app_streaming_out_template_with_options_async(request, runtime)
 
     def modify_mpulayout_with_options(
         self,
         request: rtc_20180111_models.ModifyMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyMPULayoutResponse:
+        """
+        @param request: ModifyMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.audio_mix_count):
             query['AudioMixCount'] = request.audio_mix_count
         if not UtilClient.is_unset(request.layout_id):
@@ -4954,14 +6253,19 @@
         )
 
     async def modify_mpulayout_with_options_async(
         self,
         request: rtc_20180111_models.ModifyMPULayoutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.ModifyMPULayoutResponse:
+        """
+        @param request: ModifyMPULayoutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyMPULayoutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.audio_mix_count):
             query['AudioMixCount'] = request.audio_mix_count
         if not UtilClient.is_unset(request.layout_id):
@@ -4991,29 +6295,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_mpulayout(
         self,
         request: rtc_20180111_models.ModifyMPULayoutRequest,
     ) -> rtc_20180111_models.ModifyMPULayoutResponse:
+        """
+        @param request: ModifyMPULayoutRequest
+        @return: ModifyMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_mpulayout_with_options(request, runtime)
 
     async def modify_mpulayout_async(
         self,
         request: rtc_20180111_models.ModifyMPULayoutRequest,
     ) -> rtc_20180111_models.ModifyMPULayoutResponse:
+        """
+        @param request: ModifyMPULayoutRequest
+        @return: ModifyMPULayoutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_mpulayout_with_options_async(request, runtime)
 
     def remove_terminals_with_options(
         self,
         request: rtc_20180111_models.RemoveTerminalsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.RemoveTerminalsResponse:
+        """
+        @param request: RemoveTerminalsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveTerminalsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -5040,14 +6357,19 @@
         )
 
     async def remove_terminals_with_options_async(
         self,
         request: rtc_20180111_models.RemoveTerminalsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.RemoveTerminalsResponse:
+        """
+        @param request: RemoveTerminalsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveTerminalsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.owner_id):
@@ -5073,29 +6395,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_terminals(
         self,
         request: rtc_20180111_models.RemoveTerminalsRequest,
     ) -> rtc_20180111_models.RemoveTerminalsResponse:
+        """
+        @param request: RemoveTerminalsRequest
+        @return: RemoveTerminalsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_terminals_with_options(request, runtime)
 
     async def remove_terminals_async(
         self,
         request: rtc_20180111_models.RemoveTerminalsRequest,
     ) -> rtc_20180111_models.RemoveTerminalsResponse:
+        """
+        @param request: RemoveTerminalsRequest
+        @return: RemoveTerminalsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_terminals_with_options_async(request, runtime)
 
     def remove_users_with_options(
         self,
         request: rtc_20180111_models.RemoveUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.RemoveUsersResponse:
+        """
+        @summary RemoveUsers
+        
+        @param request: RemoveUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.users):
@@ -5120,14 +6457,21 @@
         )
 
     async def remove_users_with_options_async(
         self,
         request: rtc_20180111_models.RemoveUsersRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.RemoveUsersResponse:
+        """
+        @summary RemoveUsers
+        
+        @param request: RemoveUsersRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RemoveUsersResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.users):
@@ -5151,29 +6495,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def remove_users(
         self,
         request: rtc_20180111_models.RemoveUsersRequest,
     ) -> rtc_20180111_models.RemoveUsersResponse:
+        """
+        @summary RemoveUsers
+        
+        @param request: RemoveUsersRequest
+        @return: RemoveUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.remove_users_with_options(request, runtime)
 
     async def remove_users_async(
         self,
         request: rtc_20180111_models.RemoveUsersRequest,
     ) -> rtc_20180111_models.RemoveUsersResponse:
+        """
+        @summary RemoveUsers
+        
+        @param request: RemoveUsersRequest
+        @return: RemoveUsersResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.remove_users_with_options_async(request, runtime)
 
     def start_cloud_record_with_options(
         self,
         request: rtc_20180111_models.StartCloudRecordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartCloudRecordResponse:
+        """
+        @summary StartCloudRecord
+        
+        @param request: StartCloudRecordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartCloudRecordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.panes):
@@ -5204,14 +6567,21 @@
         )
 
     async def start_cloud_record_with_options_async(
         self,
         request: rtc_20180111_models.StartCloudRecordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartCloudRecordResponse:
+        """
+        @summary StartCloudRecord
+        
+        @param request: StartCloudRecordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartCloudRecordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.panes):
@@ -5241,29 +6611,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_cloud_record(
         self,
         request: rtc_20180111_models.StartCloudRecordRequest,
     ) -> rtc_20180111_models.StartCloudRecordResponse:
+        """
+        @summary StartCloudRecord
+        
+        @param request: StartCloudRecordRequest
+        @return: StartCloudRecordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_cloud_record_with_options(request, runtime)
 
     async def start_cloud_record_async(
         self,
         request: rtc_20180111_models.StartCloudRecordRequest,
     ) -> rtc_20180111_models.StartCloudRecordResponse:
+        """
+        @summary StartCloudRecord
+        
+        @param request: StartCloudRecordRequest
+        @return: StartCloudRecordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_cloud_record_with_options_async(request, runtime)
 
     def start_mputask_with_options(
         self,
         request: rtc_20180111_models.StartMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartMPUTaskResponse:
+        """
+        @param request: StartMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -5347,14 +6734,19 @@
         )
 
     async def start_mputask_with_options_async(
         self,
         request: rtc_20180111_models.StartMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartMPUTaskResponse:
+        """
+        @param request: StartMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -5437,29 +6829,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_mputask(
         self,
         request: rtc_20180111_models.StartMPUTaskRequest,
     ) -> rtc_20180111_models.StartMPUTaskResponse:
+        """
+        @param request: StartMPUTaskRequest
+        @return: StartMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_mputask_with_options(request, runtime)
 
     async def start_mputask_async(
         self,
         request: rtc_20180111_models.StartMPUTaskRequest,
     ) -> rtc_20180111_models.StartMPUTaskResponse:
+        """
+        @param request: StartMPUTaskRequest
+        @return: StartMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_mputask_with_options_async(request, runtime)
 
     def start_record_task_with_options(
         self,
         request: rtc_20180111_models.StartRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartRecordTaskResponse:
+        """
+        @param request: StartRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.crop_mode):
@@ -5518,14 +6923,19 @@
         )
 
     async def start_record_task_with_options_async(
         self,
         request: rtc_20180111_models.StartRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartRecordTaskResponse:
+        """
+        @param request: StartRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.crop_mode):
@@ -5583,29 +6993,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_record_task(
         self,
         request: rtc_20180111_models.StartRecordTaskRequest,
     ) -> rtc_20180111_models.StartRecordTaskResponse:
+        """
+        @param request: StartRecordTaskRequest
+        @return: StartRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_record_task_with_options(request, runtime)
 
     async def start_record_task_async(
         self,
         request: rtc_20180111_models.StartRecordTaskRequest,
     ) -> rtc_20180111_models.StartRecordTaskResponse:
+        """
+        @param request: StartRecordTaskRequest
+        @return: StartRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_record_task_with_options_async(request, runtime)
 
     def start_streaming_out_with_options(
         self,
         request: rtc_20180111_models.StartStreamingOutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartStreamingOutResponse:
+        """
+        @summary StartStreamingOut
+        
+        @param request: StartStreamingOutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartStreamingOutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.panes):
@@ -5636,14 +7061,21 @@
         )
 
     async def start_streaming_out_with_options_async(
         self,
         request: rtc_20180111_models.StartStreamingOutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StartStreamingOutResponse:
+        """
+        @summary StartStreamingOut
+        
+        @param request: StartStreamingOutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartStreamingOutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.panes):
@@ -5673,29 +7105,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_streaming_out(
         self,
         request: rtc_20180111_models.StartStreamingOutRequest,
     ) -> rtc_20180111_models.StartStreamingOutResponse:
+        """
+        @summary StartStreamingOut
+        
+        @param request: StartStreamingOutRequest
+        @return: StartStreamingOutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_streaming_out_with_options(request, runtime)
 
     async def start_streaming_out_async(
         self,
         request: rtc_20180111_models.StartStreamingOutRequest,
     ) -> rtc_20180111_models.StartStreamingOutResponse:
+        """
+        @summary StartStreamingOut
+        
+        @param request: StartStreamingOutRequest
+        @return: StartStreamingOutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_streaming_out_with_options_async(request, runtime)
 
     def stop_channel_with_options(
         self,
         request: rtc_20180111_models.StopChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopChannelResponse:
+        """
+        @summary 删除频道
+        
+        @param request: StopChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -5718,14 +7169,21 @@
         )
 
     async def stop_channel_with_options_async(
         self,
         request: rtc_20180111_models.StopChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopChannelResponse:
+        """
+        @summary 删除频道
+        
+        @param request: StopChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         req = open_api_models.OpenApiRequest(
@@ -5747,29 +7205,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_channel(
         self,
         request: rtc_20180111_models.StopChannelRequest,
     ) -> rtc_20180111_models.StopChannelResponse:
+        """
+        @summary 删除频道
+        
+        @param request: StopChannelRequest
+        @return: StopChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_channel_with_options(request, runtime)
 
     async def stop_channel_async(
         self,
         request: rtc_20180111_models.StopChannelRequest,
     ) -> rtc_20180111_models.StopChannelResponse:
+        """
+        @summary 删除频道
+        
+        @param request: StopChannelRequest
+        @return: StopChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_channel_with_options_async(request, runtime)
 
     def stop_cloud_record_with_options(
         self,
         request: rtc_20180111_models.StopCloudRecordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopCloudRecordResponse:
+        """
+        @summary StopCloudRecord
+        
+        @param request: StopCloudRecordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopCloudRecordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.task_id):
@@ -5794,14 +7271,21 @@
         )
 
     async def stop_cloud_record_with_options_async(
         self,
         request: rtc_20180111_models.StopCloudRecordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopCloudRecordResponse:
+        """
+        @summary StopCloudRecord
+        
+        @param request: StopCloudRecordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopCloudRecordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.task_id):
@@ -5825,29 +7309,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_cloud_record(
         self,
         request: rtc_20180111_models.StopCloudRecordRequest,
     ) -> rtc_20180111_models.StopCloudRecordResponse:
+        """
+        @summary StopCloudRecord
+        
+        @param request: StopCloudRecordRequest
+        @return: StopCloudRecordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_cloud_record_with_options(request, runtime)
 
     async def stop_cloud_record_async(
         self,
         request: rtc_20180111_models.StopCloudRecordRequest,
     ) -> rtc_20180111_models.StopCloudRecordResponse:
+        """
+        @summary StopCloudRecord
+        
+        @param request: StopCloudRecordRequest
+        @return: StopCloudRecordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_cloud_record_with_options_async(request, runtime)
 
     def stop_mputask_with_options(
         self,
         request: rtc_20180111_models.StopMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopMPUTaskResponse:
+        """
+        @param request: StopMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -5872,14 +7373,19 @@
         )
 
     async def stop_mputask_with_options_async(
         self,
         request: rtc_20180111_models.StopMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopMPUTaskResponse:
+        """
+        @param request: StopMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -5903,29 +7409,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_mputask(
         self,
         request: rtc_20180111_models.StopMPUTaskRequest,
     ) -> rtc_20180111_models.StopMPUTaskResponse:
+        """
+        @param request: StopMPUTaskRequest
+        @return: StopMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_mputask_with_options(request, runtime)
 
     async def stop_mputask_async(
         self,
         request: rtc_20180111_models.StopMPUTaskRequest,
     ) -> rtc_20180111_models.StopMPUTaskResponse:
+        """
+        @param request: StopMPUTaskRequest
+        @return: StopMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_mputask_with_options_async(request, runtime)
 
     def stop_record_task_with_options(
         self,
         request: rtc_20180111_models.StopRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopRecordTaskResponse:
+        """
+        @param request: StopRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -5950,14 +7469,19 @@
         )
 
     async def stop_record_task_with_options_async(
         self,
         request: rtc_20180111_models.StopRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopRecordTaskResponse:
+        """
+        @param request: StopRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.task_id):
@@ -5981,29 +7505,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_record_task(
         self,
         request: rtc_20180111_models.StopRecordTaskRequest,
     ) -> rtc_20180111_models.StopRecordTaskResponse:
+        """
+        @param request: StopRecordTaskRequest
+        @return: StopRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_record_task_with_options(request, runtime)
 
     async def stop_record_task_async(
         self,
         request: rtc_20180111_models.StopRecordTaskRequest,
     ) -> rtc_20180111_models.StopRecordTaskResponse:
+        """
+        @param request: StopRecordTaskRequest
+        @return: StopRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_record_task_with_options_async(request, runtime)
 
     def stop_streaming_out_with_options(
         self,
         request: rtc_20180111_models.StopStreamingOutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopStreamingOutResponse:
+        """
+        @summary StopStreamingOut
+        
+        @param request: StopStreamingOutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopStreamingOutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.task_id):
@@ -6028,14 +7567,21 @@
         )
 
     async def stop_streaming_out_with_options_async(
         self,
         request: rtc_20180111_models.StopStreamingOutRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.StopStreamingOutResponse:
+        """
+        @summary StopStreamingOut
+        
+        @param request: StopStreamingOutRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopStreamingOutResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.task_id):
@@ -6059,29 +7605,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_streaming_out(
         self,
         request: rtc_20180111_models.StopStreamingOutRequest,
     ) -> rtc_20180111_models.StopStreamingOutResponse:
+        """
+        @summary StopStreamingOut
+        
+        @param request: StopStreamingOutRequest
+        @return: StopStreamingOutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_streaming_out_with_options(request, runtime)
 
     async def stop_streaming_out_async(
         self,
         request: rtc_20180111_models.StopStreamingOutRequest,
     ) -> rtc_20180111_models.StopStreamingOutResponse:
+        """
+        @summary StopStreamingOut
+        
+        @param request: StopStreamingOutRequest
+        @return: StopStreamingOutResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_streaming_out_with_options_async(request, runtime)
 
     def update_auto_live_stream_rule_with_options(
         self,
         request: rtc_20180111_models.UpdateAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateAutoLiveStreamRuleResponse:
+        """
+        @param request: UpdateAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_back):
             query['CallBack'] = request.call_back
         if not UtilClient.is_unset(request.channel_id_prefixes):
@@ -6118,14 +7681,19 @@
         )
 
     async def update_auto_live_stream_rule_with_options_async(
         self,
         request: rtc_20180111_models.UpdateAutoLiveStreamRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateAutoLiveStreamRuleResponse:
+        """
+        @param request: UpdateAutoLiveStreamRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAutoLiveStreamRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.call_back):
             query['CallBack'] = request.call_back
         if not UtilClient.is_unset(request.channel_id_prefixes):
@@ -6161,29 +7729,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_auto_live_stream_rule(
         self,
         request: rtc_20180111_models.UpdateAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.UpdateAutoLiveStreamRuleResponse:
+        """
+        @param request: UpdateAutoLiveStreamRuleRequest
+        @return: UpdateAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_auto_live_stream_rule_with_options(request, runtime)
 
     async def update_auto_live_stream_rule_async(
         self,
         request: rtc_20180111_models.UpdateAutoLiveStreamRuleRequest,
     ) -> rtc_20180111_models.UpdateAutoLiveStreamRuleResponse:
+        """
+        @param request: UpdateAutoLiveStreamRuleRequest
+        @return: UpdateAutoLiveStreamRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_auto_live_stream_rule_with_options_async(request, runtime)
 
     def update_mputask_with_options(
         self,
         request: rtc_20180111_models.UpdateMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateMPUTaskResponse:
+        """
+        @param request: UpdateMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -6244,14 +7825,19 @@
         )
 
     async def update_mputask_with_options_async(
         self,
         request: rtc_20180111_models.UpdateMPUTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateMPUTaskResponse:
+        """
+        @param request: UpdateMPUTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateMPUTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -6311,29 +7897,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_mputask(
         self,
         request: rtc_20180111_models.UpdateMPUTaskRequest,
     ) -> rtc_20180111_models.UpdateMPUTaskResponse:
+        """
+        @param request: UpdateMPUTaskRequest
+        @return: UpdateMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_mputask_with_options(request, runtime)
 
     async def update_mputask_async(
         self,
         request: rtc_20180111_models.UpdateMPUTaskRequest,
     ) -> rtc_20180111_models.UpdateMPUTaskResponse:
+        """
+        @param request: UpdateMPUTaskRequest
+        @return: UpdateMPUTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_mputask_with_options_async(request, runtime)
 
     def update_record_task_with_options(
         self,
         request: rtc_20180111_models.UpdateRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateRecordTaskResponse:
+        """
+        @param request: UpdateRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.crop_mode):
@@ -6386,14 +7985,19 @@
         )
 
     async def update_record_task_with_options_async(
         self,
         request: rtc_20180111_models.UpdateRecordTaskRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateRecordTaskResponse:
+        """
+        @param request: UpdateRecordTaskRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRecordTaskResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.channel_id):
             query['ChannelId'] = request.channel_id
         if not UtilClient.is_unset(request.crop_mode):
@@ -6445,29 +8049,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_record_task(
         self,
         request: rtc_20180111_models.UpdateRecordTaskRequest,
     ) -> rtc_20180111_models.UpdateRecordTaskResponse:
+        """
+        @param request: UpdateRecordTaskRequest
+        @return: UpdateRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_record_task_with_options(request, runtime)
 
     async def update_record_task_async(
         self,
         request: rtc_20180111_models.UpdateRecordTaskRequest,
     ) -> rtc_20180111_models.UpdateRecordTaskResponse:
+        """
+        @param request: UpdateRecordTaskRequest
+        @return: UpdateRecordTaskResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_record_task_with_options_async(request, runtime)
 
     def update_record_template_with_options(
         self,
         request: rtc_20180111_models.UpdateRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateRecordTemplateResponse:
+        """
+        @param request: UpdateRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -6526,14 +8143,19 @@
         )
 
     async def update_record_template_with_options_async(
         self,
         request: rtc_20180111_models.UpdateRecordTemplateRequest,
         runtime: util_models.RuntimeOptions,
     ) -> rtc_20180111_models.UpdateRecordTemplateResponse:
+        """
+        @param request: UpdateRecordTemplateRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateRecordTemplateResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_id):
             query['AppId'] = request.app_id
         if not UtilClient.is_unset(request.background_color):
             query['BackgroundColor'] = request.background_color
         if not UtilClient.is_unset(request.backgrounds):
@@ -6591,16 +8213,24 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_record_template(
         self,
         request: rtc_20180111_models.UpdateRecordTemplateRequest,
     ) -> rtc_20180111_models.UpdateRecordTemplateResponse:
+        """
+        @param request: UpdateRecordTemplateRequest
+        @return: UpdateRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.update_record_template_with_options(request, runtime)
 
     async def update_record_template_async(
         self,
         request: rtc_20180111_models.UpdateRecordTemplateRequest,
     ) -> rtc_20180111_models.UpdateRecordTemplateResponse:
+        """
+        @param request: UpdateRecordTemplateRequest
+        @return: UpdateRecordTemplateResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.update_record_template_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111/models.py` & `alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,31 +212,40 @@
         oss_bucket: str = None,
         oss_endpoint: str = None,
         oss_file_prefix: str = None,
         owner_id: int = None,
         task_profile: str = None,
         watermarks: List[AddRecordTemplateRequestWatermarks] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.background_color = background_color
         self.backgrounds = backgrounds
         self.clock_widgets = clock_widgets
         self.delay_stop_time = delay_stop_time
         self.enable_m3u_8date_time = enable_m3u_8date_time
+        # This parameter is required.
         self.file_split_interval = file_split_interval
+        # This parameter is required.
         self.formats = formats
         self.http_callback_url = http_callback_url
+        # This parameter is required.
         self.layout_ids = layout_ids
+        # This parameter is required.
         self.media_encode = media_encode
         self.mns_queue = mns_queue
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.oss_bucket = oss_bucket
         self.oss_endpoint = oss_endpoint
+        # This parameter is required.
         self.oss_file_prefix = oss_file_prefix
         self.owner_id = owner_id
+        # This parameter is required.
         self.task_profile = task_profile
         self.watermarks = watermarks
 
     def validate(self):
         if self.backgrounds:
             for k in self.backgrounds:
                 if k:
@@ -431,16 +440,19 @@
 class CreateAppStreamingOutTemplateRequestStreamingOutTemplate(TeaModel):
     def __init__(
         self,
         layout_ids: List[str] = None,
         media_encode: int = None,
         name: str = None,
     ):
+        # This parameter is required.
         self.layout_ids = layout_ids
+        # This parameter is required.
         self.media_encode = media_encode
+        # This parameter is required.
         self.name = name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -469,15 +481,17 @@
 
 class CreateAppStreamingOutTemplateRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template: CreateAppStreamingOutTemplateRequestStreamingOutTemplate = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template = streaming_out_template
 
     def validate(self):
         if self.streaming_out_template:
             self.streaming_out_template.validate()
 
     def to_map(self):
@@ -504,15 +518,17 @@
 
 class CreateAppStreamingOutTemplateShrinkRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template_shrink: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template_shrink = streaming_out_template_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -618,20 +634,22 @@
         channel_id_prefixes: List[str] = None,
         channel_ids: List[str] = None,
         media_encode: int = None,
         owner_id: int = None,
         play_domain: str = None,
         rule_name: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.call_back = call_back
         self.channel_id_prefixes = channel_id_prefixes
         self.channel_ids = channel_ids
         self.media_encode = media_encode
         self.owner_id = owner_id
+        # This parameter is required.
         self.play_domain = play_domain
         self.rule_name = rule_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -762,18 +780,22 @@
         client_token: str = None,
         events: List[str] = None,
         need_callback_auth: bool = None,
         owner_id: int = None,
         role: int = None,
         users: List[str] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.callback_url = callback_url
         self.channel_id = channel_id
+        # This parameter is required.
         self.client_token = client_token
+        # This parameter is required.
         self.events = events
         self.need_callback_auth = need_callback_auth
         self.owner_id = owner_id
         self.role = role
         self.users = users
 
     def validate(self):
@@ -970,18 +992,21 @@
         self,
         app_id: str = None,
         audio_mix_count: int = None,
         name: str = None,
         owner_id: int = None,
         panes: List[CreateMPULayoutRequestPanes] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.audio_mix_count = audio_mix_count
         self.name = name
         self.owner_id = owner_id
+        # This parameter is required.
         self.panes = panes
 
     def validate(self):
         if self.panes:
             for k in self.panes:
                 if k:
                     k.validate()
@@ -1099,14 +1124,15 @@
 
 
 class DeleteAppStreamingOutTemplateRequestStreamingOutTemplate(TeaModel):
     def __init__(
         self,
         template_id: str = None,
     ):
+        # This parameter is required.
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1127,15 +1153,17 @@
 
 class DeleteAppStreamingOutTemplateRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template: DeleteAppStreamingOutTemplateRequestStreamingOutTemplate = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template = streaming_out_template
 
     def validate(self):
         if self.streaming_out_template:
             self.streaming_out_template.validate()
 
     def to_map(self):
@@ -1162,15 +1190,17 @@
 
 class DeleteAppStreamingOutTemplateShrinkRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template_shrink: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template_shrink = streaming_out_template_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1265,16 +1295,18 @@
 class DeleteAutoLiveStreamRuleRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1372,15 +1404,17 @@
 class DeleteChannelRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1479,16 +1513,18 @@
 class DeleteEventSubscribeRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         subscribe_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.subscribe_id = subscribe_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1586,15 +1622,17 @@
 class DeleteMPULayoutRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         layout_id: int = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.layout_id = layout_id
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1693,17 +1731,19 @@
 class DeleteRecordTemplateRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         template_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         # 1
         self.owner_id = owner_id
+        # This parameter is required.
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1800,14 +1840,15 @@
 
 class DescribeAppKeyRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1943,14 +1984,15 @@
     def __init__(
         self,
         app_id: str = None,
         condition: DescribeAppStreamingOutTemplatesRequestCondition = None,
         page_num: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.condition = condition
         self.page_num = page_num
         self.page_size = page_size
 
     def validate(self):
         if self.condition:
@@ -1990,14 +2032,15 @@
     def __init__(
         self,
         app_id: str = None,
         condition_shrink: str = None,
         page_num: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.condition_shrink = condition_shrink
         self.page_num = page_num
         self.page_size = page_size
 
     def validate(self):
         pass
@@ -2177,21 +2220,23 @@
         return self
 
 
 class DescribeAppsRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
+        app_version: str = None,
         order: str = None,
         owner_id: int = None,
         page_num: int = None,
         page_size: int = None,
         status: str = None,
     ):
         self.app_id = app_id
+        self.app_version = app_version
         self.order = order
         self.owner_id = owner_id
         self.page_num = page_num
         self.page_size = page_size
         self.status = status
 
     def validate(self):
@@ -2201,14 +2246,16 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.app_id is not None:
             result['AppId'] = self.app_id
+        if self.app_version is not None:
+            result['AppVersion'] = self.app_version
         if self.order is not None:
             result['Order'] = self.order
         if self.owner_id is not None:
             result['OwnerId'] = self.owner_id
         if self.page_num is not None:
             result['PageNum'] = self.page_num
         if self.page_size is not None:
@@ -2217,14 +2264,16 @@
             result['Status'] = self.status
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppId') is not None:
             self.app_id = m.get('AppId')
+        if m.get('AppVersion') is not None:
+            self.app_version = m.get('AppVersion')
         if m.get('Order') is not None:
             self.order = m.get('Order')
         if m.get('OwnerId') is not None:
             self.owner_id = m.get('OwnerId')
         if m.get('PageNum') is not None:
             self.page_num = m.get('PageNum')
         if m.get('PageSize') is not None:
@@ -2457,14 +2506,15 @@
 
 class DescribeAutoLiveStreamRuleRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -2652,16 +2702,20 @@
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         ext_data_type: str = None,
         query_exp_info: bool = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
         self.ext_data_type = ext_data_type
         self.query_exp_info = query_exp_info
 
     def validate(self):
         pass
@@ -3105,22 +3159,28 @@
         page_no: int = None,
         page_size: int = None,
         query_mode: str = None,
         start_ts: int = None,
         user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
         self.call_status = call_status
         self.channel_id = channel_id
+        # This parameter is required.
         self.end_ts = end_ts
         self.order_by = order_by
+        # This parameter is required.
         self.page_no = page_no
+        # This parameter is required.
         self.page_size = page_size
         self.query_mode = query_mode
+        # This parameter is required.
         self.start_ts = start_ts
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -3348,15 +3408,17 @@
 
 class DescribeChannelRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3497,15 +3559,17 @@
 
 class DescribeChannelAllUsersRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3649,16 +3713,20 @@
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         parent_area: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
         self.parent_area = parent_area
 
     def validate(self):
         pass
 
@@ -3834,18 +3902,23 @@
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         stat_dim: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
+        # This parameter is required.
         self.stat_dim = stat_dim
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4006,16 +4079,20 @@
         self,
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4341,15 +4418,17 @@
         app_id: str = None,
         channel_id: str = None,
         order: str = None,
         owner_id: int = None,
         page_num: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.order = order
         self.owner_id = owner_id
         self.page_num = page_num
         self.page_size = page_size
 
     def validate(self):
@@ -4518,16 +4597,20 @@
         self,
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4748,16 +4831,19 @@
 class DescribeChannelUserRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         user_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4922,16 +5008,20 @@
         self,
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5188,15 +5278,17 @@
 class DescribeChannelUsersRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -5352,18 +5444,23 @@
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         user_id_list: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
+        # This parameter is required.
         self.user_id_list = user_id_list
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5616,18 +5713,23 @@
         destroyed_ts: int = None,
         metrics: str = None,
         pub_call_id_list: str = None,
         pub_user_id: str = None,
         sub_user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
+        # This parameter is required.
         self.metrics = metrics
         self.pub_call_id_list = pub_call_id_list
         self.pub_user_id = pub_user_id
         self.sub_user_id = sub_user_id
 
     def validate(self):
         pass
@@ -5950,16 +6052,20 @@
     def __init__(
         self,
         app_id: str = None,
         end_ts: int = None,
         start_ts: int = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_ts = end_ts
+        # This parameter is required.
         self.start_ts = start_ts
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6112,17 +6218,22 @@
         self,
         app_id: str = None,
         end_ts: int = None,
         start_ts: int = None,
         stat_dim: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_ts = end_ts
+        # This parameter is required.
         self.start_ts = start_ts
+        # This parameter is required.
         self.stat_dim = stat_dim
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6358,19 +6469,25 @@
         channel_id: str = None,
         created_ts: int = None,
         fault_type: str = None,
         query_call_user_info: bool = None,
         user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
+        # This parameter is required.
         self.fault_type = fault_type
         self.query_call_user_info = query_call_user_info
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7062,20 +7179,26 @@
         fault_types: str = None,
         page_no: int = None,
         page_size: int = None,
         start_ts: int = None,
         user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
+        # This parameter is required.
         self.end_ts = end_ts
         self.fault_types = fault_types
+        # This parameter is required.
         self.page_no = page_no
+        # This parameter is required.
         self.page_size = page_size
+        # This parameter is required.
         self.start_ts = start_ts
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -7321,14 +7444,15 @@
         app_id: str = None,
         layout_id: int = None,
         name: str = None,
         owner_id: int = None,
         page_num: int = None,
         page_size: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.layout_id = layout_id
         self.name = name
         self.owner_id = owner_id
         self.page_num = page_num
         self.page_size = page_size
 
@@ -7646,18 +7770,23 @@
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         sub_user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
+        # This parameter is required.
         self.sub_user_id = sub_user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8117,18 +8246,23 @@
         app_id: str = None,
         channel_id: str = None,
         created_ts: int = None,
         destroyed_ts: int = None,
         user_id: str = None,
     ):
         # APP ID。
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.created_ts = created_ts
         self.destroyed_ts = destroyed_ts
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8425,17 +8559,21 @@
         self,
         app_id: str = None,
         end_date: int = None,
         parent_area: str = None,
         start_date: int = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
         self.parent_area = parent_area
+        # This parameter is required.
         self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8640,17 +8778,22 @@
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
         stat_dim: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.stat_dim = stat_dim
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8854,16 +8997,20 @@
     def __init__(
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9070,17 +9217,22 @@
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
         types: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.types = types
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9281,14 +9433,15 @@
         end_time: str = None,
         owner_id: int = None,
         page_num: int = None,
         page_size: int = None,
         start_time: str = None,
         task_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.channel_id = channel_id
         self.end_time = end_time
         self.owner_id = owner_id
         self.page_num = page_num
         self.page_size = page_size
         self.start_time = start_time
@@ -9510,14 +9663,15 @@
         self,
         app_id: str = None,
         owner_id: int = None,
         page_num: int = None,
         page_size: int = None,
         template_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         # 1
         self.owner_id = owner_id
         self.page_num = page_num
         self.page_size = page_size
         self.template_ids = template_ids
 
@@ -10007,18 +10161,21 @@
         sort_type: str = None,
         time_point: str = None,
         user_id: str = None,
     ):
         self.app_id = app_id
         self.channel_id = channel_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.page_no = page_no
+        # This parameter is required.
         self.page_size = page_size
         self.service_area = service_area
         self.sort_type = sort_type
+        # This parameter is required.
         self.time_point = time_point
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -10283,17 +10440,20 @@
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         owner_id: int = None,
         time_point: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.time_point = time_point
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11279,17 +11439,21 @@
         self,
         app_id: str = None,
         end_date: str = None,
         parent_area: str = None,
         start_date: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
         self.parent_area = parent_area
+        # This parameter is required.
         self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11452,17 +11616,22 @@
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
         stat_dim: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.stat_dim = stat_dim
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11630,16 +11799,20 @@
     def __init__(
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11810,17 +11983,22 @@
         self,
         app_id: str = None,
         end_date: int = None,
         start_date: int = None,
         types: str = None,
     ):
         # APP ID
+        # 
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.types = types
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12011,17 +12189,20 @@
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         owner_id: int = None,
         user_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12194,16 +12375,18 @@
 class DisableAutoLiveStreamRuleRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12301,16 +12484,18 @@
 class EnableAutoLiveStreamRuleRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         rule_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.rule_id = rule_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12408,16 +12593,18 @@
 class GetMPUTaskStatusRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12521,15 +12708,17 @@
 class ModifyAppRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         app_name: str = None,
         owner_id: int = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.app_name = app_name
         self.owner_id = owner_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -12629,17 +12818,21 @@
     def __init__(
         self,
         layout_ids: List[str] = None,
         media_encode: int = None,
         name: str = None,
         template_id: str = None,
     ):
+        # This parameter is required.
         self.layout_ids = layout_ids
+        # This parameter is required.
         self.media_encode = media_encode
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.template_id = template_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12672,15 +12865,17 @@
 
 class ModifyAppStreamingOutTemplateRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template: ModifyAppStreamingOutTemplateRequestStreamingOutTemplate = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template = streaming_out_template
 
     def validate(self):
         if self.streaming_out_template:
             self.streaming_out_template.validate()
 
     def to_map(self):
@@ -12707,15 +12902,17 @@
 
 class ModifyAppStreamingOutTemplateShrinkRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         streaming_out_template_shrink: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.streaming_out_template_shrink = streaming_out_template_shrink
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12882,16 +13079,18 @@
         app_id: str = None,
         audio_mix_count: int = None,
         layout_id: int = None,
         name: str = None,
         owner_id: int = None,
         panes: List[ModifyMPULayoutRequestPanes] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.audio_mix_count = audio_mix_count
+        # This parameter is required.
         self.layout_id = layout_id
         self.name = name
         self.owner_id = owner_id
         self.panes = panes
 
     def validate(self):
         if self.panes:
@@ -13013,17 +13212,20 @@
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         owner_id: int = None,
         terminal_ids: List[str] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.terminal_ids = terminal_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13205,14 +13407,15 @@
 
 
 class RemoveUsersRequestUsers(TeaModel):
     def __init__(
         self,
         user_id: str = None,
     ):
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13234,16 +13437,19 @@
 class RemoveUsersRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         users: List[RemoveUsersRequestUsers] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.users = users
 
     def validate(self):
         if self.users:
             for k in self.users:
                 if k:
                     k.validate()
@@ -13402,14 +13608,16 @@
 class StartCloudRecordRequestPanes(TeaModel):
     def __init__(
         self,
         pane_id: int = None,
         source_type: str = None,
     ):
         # paneId
+        # 
+        # This parameter is required.
         self.pane_id = pane_id
         # sourceType
         self.source_type = source_type
 
     def validate(self):
         pass
 
@@ -13440,22 +13648,32 @@
         access_key: str = None,
         bucket: str = None,
         region: int = None,
         secret_key: str = None,
         vendor: int = None,
     ):
         # accessKey
+        # 
+        # This parameter is required.
         self.access_key = access_key
         # bucket
+        # 
+        # This parameter is required.
         self.bucket = bucket
         # region
+        # 
+        # This parameter is required.
         self.region = region
         # secretKey
+        # 
+        # This parameter is required.
         self.secret_key = secret_key
         # vendor
+        # 
+        # This parameter is required.
         self.vendor = vendor
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13497,24 +13715,32 @@
         channel_id: str = None,
         panes: List[StartCloudRecordRequestPanes] = None,
         storage_config: StartCloudRecordRequestStorageConfig = None,
         task_id: str = None,
         template_id: str = None,
     ):
         # appId
+        # 
+        # This parameter is required.
         self.app_id = app_id
         # channelName
+        # 
+        # This parameter is required.
         self.channel_id = channel_id
         # panes
         self.panes = panes
         # storageConfig
+        # 
+        # This parameter is required.
         self.storage_config = storage_config
         # taskId
         self.task_id = task_id
         # templateId
+        # 
+        # This parameter is required.
         self.template_id = template_id
 
     def validate(self):
         if self.panes:
             for k in self.panes:
                 if k:
                     k.validate()
@@ -14158,17 +14384,19 @@
         unsub_spec_audio_users: List[str] = None,
         unsub_spec_camera_users: List[str] = None,
         unsub_spec_share_screen_users: List[str] = None,
         user_panes: List[StartMPUTaskRequestUserPanes] = None,
         vad_interval: int = None,
         watermarks: List[StartMPUTaskRequestWatermarks] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.background_color = background_color
         self.backgrounds = backgrounds
+        # This parameter is required.
         self.channel_id = channel_id
         self.clock_widgets = clock_widgets
         self.crop_mode = crop_mode
         self.enhanced_param = enhanced_param
         self.layout_ids = layout_ids
         self.media_encode = media_encode
         self.mix_mode = mix_mode
@@ -14179,14 +14407,15 @@
         self.source_type = source_type
         self.stream_type = stream_type
         self.stream_url = stream_url
         self.sub_spec_audio_users = sub_spec_audio_users
         self.sub_spec_camera_users = sub_spec_camera_users
         self.sub_spec_share_screen_users = sub_spec_share_screen_users
         self.sub_spec_users = sub_spec_users
+        # This parameter is required.
         self.task_id = task_id
         self.task_type = task_type
         self.time_stamp_ref = time_stamp_ref
         self.unsub_spec_audio_users = unsub_spec_audio_users
         self.unsub_spec_camera_users = unsub_spec_camera_users
         self.unsub_spec_share_screen_users = unsub_spec_share_screen_users
         self.user_panes = user_panes
@@ -14649,29 +14878,33 @@
         task_profile: str = None,
         template_id: str = None,
         unsub_spec_audio_users: List[str] = None,
         unsub_spec_camera_users: List[str] = None,
         unsub_spec_share_screen_users: List[str] = None,
         user_panes: List[StartRecordTaskRequestUserPanes] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.crop_mode = crop_mode
         self.layout_ids = layout_ids
         self.media_encode = media_encode
         self.mix_mode = mix_mode
         self.owner_id = owner_id
         self.source_type = source_type
         self.stream_type = stream_type
         self.sub_spec_audio_users = sub_spec_audio_users
         self.sub_spec_camera_users = sub_spec_camera_users
         self.sub_spec_share_screen_users = sub_spec_share_screen_users
         self.sub_spec_users = sub_spec_users
+        # This parameter is required.
         self.task_id = task_id
         self.task_profile = task_profile
+        # This parameter is required.
         self.template_id = template_id
         self.unsub_spec_audio_users = unsub_spec_audio_users
         self.unsub_spec_camera_users = unsub_spec_camera_users
         self.unsub_spec_share_screen_users = unsub_spec_share_screen_users
         self.user_panes = user_panes
 
     def validate(self):
@@ -14848,14 +15081,15 @@
 
 class StartStreamingOutRequestPanes(TeaModel):
     def __init__(
         self,
         pane_id: str = None,
         source_type: str = None,
     ):
+        # This parameter is required.
         self.pane_id = pane_id
         self.source_type = source_type
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -14885,19 +15119,23 @@
         app_id: str = None,
         channel_id: str = None,
         panes: List[StartStreamingOutRequestPanes] = None,
         task_id: str = None,
         template_id: str = None,
         url: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.panes = panes
         self.task_id = task_id
+        # This parameter is required.
         self.template_id = template_id
+        # This parameter is required.
         self.url = url
 
     def validate(self):
         if self.panes:
             for k in self.panes:
                 if k:
                     k.validate()
@@ -15020,15 +15258,17 @@
 
 class StopChannelRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15122,16 +15362,19 @@
 class StopCloudRecordRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15235,16 +15478,18 @@
 class StopMPUTaskRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15342,16 +15587,18 @@
 class StopRecordTaskRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         owner_id: int = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.owner_id = owner_id
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15449,16 +15696,19 @@
 class StopStreamingOutRequest(TeaModel):
     def __init__(
         self,
         app_id: str = None,
         channel_id: str = None,
         task_id: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15568,21 +15818,24 @@
         channel_ids: List[str] = None,
         media_encode: int = None,
         owner_id: int = None,
         play_domain: str = None,
         rule_id: int = None,
         rule_name: str = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.call_back = call_back
         self.channel_id_prefixes = channel_id_prefixes
         self.channel_ids = channel_ids
         self.media_encode = media_encode
         self.owner_id = owner_id
+        # This parameter is required.
         self.play_domain = play_domain
+        # This parameter is required.
         self.rule_id = rule_id
         self.rule_name = rule_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -16184,14 +16437,15 @@
         task_id: str = None,
         unsub_spec_audio_users: List[str] = None,
         unsub_spec_camera_users: List[str] = None,
         unsub_spec_share_screen_users: List[str] = None,
         user_panes: List[UpdateMPUTaskRequestUserPanes] = None,
         watermarks: List[UpdateMPUTaskRequestWatermarks] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.background_color = background_color
         self.backgrounds = backgrounds
         self.clock_widgets = clock_widgets
         self.crop_mode = crop_mode
         self.layout_ids = layout_ids
         self.media_encode = media_encode
@@ -16199,14 +16453,15 @@
         self.owner_id = owner_id
         self.source_type = source_type
         self.stream_type = stream_type
         self.sub_spec_audio_users = sub_spec_audio_users
         self.sub_spec_camera_users = sub_spec_camera_users
         self.sub_spec_share_screen_users = sub_spec_share_screen_users
         self.sub_spec_users = sub_spec_users
+        # This parameter is required.
         self.task_id = task_id
         self.unsub_spec_audio_users = unsub_spec_audio_users
         self.unsub_spec_camera_users = unsub_spec_camera_users
         self.unsub_spec_share_screen_users = unsub_spec_share_screen_users
         self.user_panes = user_panes
         self.watermarks = watermarks
 
@@ -16624,26 +16879,30 @@
         task_profile: str = None,
         template_id: str = None,
         unsub_spec_audio_users: List[str] = None,
         unsub_spec_camera_users: List[str] = None,
         unsub_spec_share_screen_users: List[str] = None,
         user_panes: List[UpdateRecordTaskRequestUserPanes] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
+        # This parameter is required.
         self.channel_id = channel_id
         self.crop_mode = crop_mode
         self.layout_ids = layout_ids
         self.media_encode = media_encode
         self.owner_id = owner_id
         self.sub_spec_audio_users = sub_spec_audio_users
         self.sub_spec_camera_users = sub_spec_camera_users
         self.sub_spec_share_screen_users = sub_spec_share_screen_users
         self.sub_spec_users = sub_spec_users
+        # This parameter is required.
         self.task_id = task_id
         self.task_profile = task_profile
+        # This parameter is required.
         self.template_id = template_id
         self.unsub_spec_audio_users = unsub_spec_audio_users
         self.unsub_spec_camera_users = unsub_spec_camera_users
         self.unsub_spec_share_screen_users = unsub_spec_share_screen_users
         self.user_panes = user_panes
 
     def validate(self):
@@ -17015,32 +17274,42 @@
         oss_endpoint: str = None,
         oss_file_prefix: str = None,
         owner_id: int = None,
         task_profile: str = None,
         template_id: str = None,
         watermarks: List[UpdateRecordTemplateRequestWatermarks] = None,
     ):
+        # This parameter is required.
         self.app_id = app_id
         self.background_color = background_color
         self.backgrounds = backgrounds
         self.clock_widgets = clock_widgets
         self.delay_stop_time = delay_stop_time
         self.enable_m3u_8date_time = enable_m3u_8date_time
+        # This parameter is required.
         self.file_split_interval = file_split_interval
+        # This parameter is required.
         self.formats = formats
         self.http_callback_url = http_callback_url
+        # This parameter is required.
         self.layout_ids = layout_ids
+        # This parameter is required.
         self.media_encode = media_encode
         self.mns_queue = mns_queue
+        # This parameter is required.
         self.name = name
+        # This parameter is required.
         self.oss_bucket = oss_bucket
         self.oss_endpoint = oss_endpoint
+        # This parameter is required.
         self.oss_file_prefix = oss_file_prefix
         self.owner_id = owner_id
+        # This parameter is required.
         self.task_profile = task_profile
+        # This parameter is required.
         self.template_id = template_id
         self.watermarks = watermarks
 
     def validate(self):
         if self.backgrounds:
             for k in self.backgrounds:
                 if k:
```

### Comparing `alibabacloud_rtc20180111-3.0.0/alibabacloud_rtc20180111.egg-info/PKG-INFO` & `alibabacloud_rtc20180111-3.0.1/alibabacloud_rtc20180111.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rtc20180111
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud Real-Time Communication (20180111) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rtc20180111-3.0.0/setup.py` & `alibabacloud_rtc20180111-3.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rtc20180111.
 
-Created on 21/03/2024
+Created on 22/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rtc20180111"
 NAME = "alibabacloud_rtc20180111" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Real-Time Communication (20180111) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

