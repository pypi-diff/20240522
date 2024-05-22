# Comparing `tmp/alibabacloud_emr-serverless-spark20230808-1.1.0.tar.gz` & `tmp/alibabacloud_emr-serverless-spark20230808-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.1.0.tar", last modified: Mon May 20 17:14:59 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.2.0.tar", last modified: Tue May 21 17:11:27 2024, max compression
```

## Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0.tar` & `alibabacloud_emr-serverless-spark20230808-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      415 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1163 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1248 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37330 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/client.py
--rw-r--r--   0 root         (0) root         (0)   116185 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2700 2024-05-20 17:14:59.000000 alibabacloud_emr-serverless-spark20230808-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      543 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42336 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/client.py
+-rw-r--r--   0 root         (0) root         (0)   130230 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-21 17:11:27.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2700 2024-05-21 17:11:26.000000 alibabacloud_emr-serverless-spark20230808-1.2.0/setup.py
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/LICENSE` & `alibabacloud_emr-serverless-spark20230808-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr-serverless-spark20230808
-Version: 1.1.0
+Version: 1.2.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/README-CN.md` & `alibabacloud_emr-serverless-spark20230808-1.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/README.md` & `alibabacloud_emr-serverless-spark20230808-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/client.py` & `alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -545,14 +545,138 @@
         @param request: ListReleaseVersionsRequest
         @return: ListReleaseVersionsResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.list_release_versions_with_options_async(request, headers, runtime)
 
+    def list_session_clusters_with_options(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListSessionClustersRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListSessionClustersResponse:
+        """
+        @summary 查询run列表
+        
+        @param request: ListSessionClustersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSessionClustersResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.queue_name):
+            query['queueName'] = request.queue_name
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.session_cluster_id):
+            query['sessionClusterId'] = request.session_cluster_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListSessionClusters',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/sessionClusters',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListSessionClustersResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_session_clusters_with_options_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListSessionClustersRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.ListSessionClustersResponse:
+        """
+        @summary 查询run列表
+        
+        @param request: ListSessionClustersRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListSessionClustersResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        if not UtilClient.is_unset(request.queue_name):
+            query['queueName'] = request.queue_name
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        if not UtilClient.is_unset(request.session_cluster_id):
+            query['sessionClusterId'] = request.session_cluster_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListSessionClusters',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/v1/workspaces/{OpenApiUtilClient.get_encode_param(workspace_id)}/sessionClusters',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.ListSessionClustersResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_session_clusters(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListSessionClustersRequest,
+    ) -> emr_serverless_spark_20230808_models.ListSessionClustersResponse:
+        """
+        @summary 查询run列表
+        
+        @param request: ListSessionClustersRequest
+        @return: ListSessionClustersResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_session_clusters_with_options(workspace_id, request, headers, runtime)
+
+    async def list_session_clusters_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.ListSessionClustersRequest,
+    ) -> emr_serverless_spark_20230808_models.ListSessionClustersResponse:
+        """
+        @summary 查询run列表
+        
+        @param request: ListSessionClustersRequest
+        @return: ListSessionClustersResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_session_clusters_with_options_async(workspace_id, request, headers, runtime)
+
     def list_workspace_queues_with_options(
         self,
         workspace_id: str,
         request: emr_serverless_spark_20230808_models.ListWorkspaceQueuesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> emr_serverless_spark_20230808_models.ListWorkspaceQueuesResponse:
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808/models.py` & `alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -2541,14 +2541,413 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ListReleaseVersionsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListSessionClustersRequest(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        queue_name: str = None,
+        region_id: str = None,
+        session_cluster_id: str = None,
+    ):
+        # 一次获取的最大记录数。
+        self.max_results = max_results
+        # 标记当前开始读取的位置，置空表示从头开始。
+        self.next_token = next_token
+        self.queue_name = queue_name
+        self.region_id = region_id
+        # 作业名称。
+        self.session_cluster_id = session_cluster_id
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
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.queue_name is not None:
+            result['queueName'] = self.queue_name
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        if self.session_cluster_id is not None:
+            result['sessionClusterId'] = self.session_cluster_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('queueName') is not None:
+            self.queue_name = m.get('queueName')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        if m.get('sessionClusterId') is not None:
+            self.session_cluster_id = m.get('sessionClusterId')
+        return self
+
+
+class ListSessionClustersResponseBodySessionClustersApplicationConfigs(TeaModel):
+    def __init__(
+        self,
+        config_file_name: str = None,
+        config_item_key: str = None,
+        config_item_value: str = None,
+    ):
+        self.config_file_name = config_file_name
+        self.config_item_key = config_item_key
+        self.config_item_value = config_item_value
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
+        if self.config_file_name is not None:
+            result['configFileName'] = self.config_file_name
+        if self.config_item_key is not None:
+            result['configItemKey'] = self.config_item_key
+        if self.config_item_value is not None:
+            result['configItemValue'] = self.config_item_value
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('configFileName') is not None:
+            self.config_file_name = m.get('configFileName')
+        if m.get('configItemKey') is not None:
+            self.config_item_key = m.get('configItemKey')
+        if m.get('configItemValue') is not None:
+            self.config_item_value = m.get('configItemValue')
+        return self
+
+
+class ListSessionClustersResponseBodySessionClustersAutoStartConfiguration(TeaModel):
+    def __init__(
+        self,
+        enable: bool = None,
+    ):
+        self.enable = enable
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
+        if self.enable is not None:
+            result['enable'] = self.enable
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enable') is not None:
+            self.enable = m.get('enable')
+        return self
+
+
+class ListSessionClustersResponseBodySessionClustersAutoStopConfiguration(TeaModel):
+    def __init__(
+        self,
+        enable: bool = None,
+        idle_timeout_minutes: int = None,
+    ):
+        self.enable = enable
+        self.idle_timeout_minutes = idle_timeout_minutes
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
+        if self.enable is not None:
+            result['enable'] = self.enable
+        if self.idle_timeout_minutes is not None:
+            result['idleTimeoutMinutes'] = self.idle_timeout_minutes
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('enable') is not None:
+            self.enable = m.get('enable')
+        if m.get('idleTimeoutMinutes') is not None:
+            self.idle_timeout_minutes = m.get('idleTimeoutMinutes')
+        return self
+
+
+class ListSessionClustersResponseBodySessionClustersStateChangeReason(TeaModel):
+    def __init__(
+        self,
+        code: str = None,
+        message: str = None,
+    ):
+        self.code = code
+        self.message = message
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
+        if self.code is not None:
+            result['code'] = self.code
+        if self.message is not None:
+            result['message'] = self.message
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('code') is not None:
+            self.code = m.get('code')
+        if m.get('message') is not None:
+            self.message = m.get('message')
+        return self
+
+
+class ListSessionClustersResponseBodySessionClusters(TeaModel):
+    def __init__(
+        self,
+        application_configs: List[ListSessionClustersResponseBodySessionClustersApplicationConfigs] = None,
+        auto_start_configuration: ListSessionClustersResponseBodySessionClustersAutoStartConfiguration = None,
+        auto_stop_configuration: ListSessionClustersResponseBodySessionClustersAutoStopConfiguration = None,
+        name: str = None,
+        queue_name: str = None,
+        session_cluster_id: str = None,
+        state: str = None,
+        state_change_reason: ListSessionClustersResponseBodySessionClustersStateChangeReason = None,
+        user_id: str = None,
+        user_name: str = None,
+        workspace_id: str = None,
+    ):
+        self.application_configs = application_configs
+        self.auto_start_configuration = auto_start_configuration
+        self.auto_stop_configuration = auto_stop_configuration
+        self.name = name
+        # 作业实例名称。
+        self.queue_name = queue_name
+        # SQL Compute id
+        self.session_cluster_id = session_cluster_id
+        # 作业状态。
+        self.state = state
+        self.state_change_reason = state_change_reason
+        # 任务实例ID。
+        self.user_id = user_id
+        self.user_name = user_name
+        # 工作空间id。
+        self.workspace_id = workspace_id
+
+    def validate(self):
+        if self.application_configs:
+            for k in self.application_configs:
+                if k:
+                    k.validate()
+        if self.auto_start_configuration:
+            self.auto_start_configuration.validate()
+        if self.auto_stop_configuration:
+            self.auto_stop_configuration.validate()
+        if self.state_change_reason:
+            self.state_change_reason.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['applicationConfigs'] = []
+        if self.application_configs is not None:
+            for k in self.application_configs:
+                result['applicationConfigs'].append(k.to_map() if k else None)
+        if self.auto_start_configuration is not None:
+            result['autoStartConfiguration'] = self.auto_start_configuration.to_map()
+        if self.auto_stop_configuration is not None:
+            result['autoStopConfiguration'] = self.auto_stop_configuration.to_map()
+        if self.name is not None:
+            result['name'] = self.name
+        if self.queue_name is not None:
+            result['queueName'] = self.queue_name
+        if self.session_cluster_id is not None:
+            result['sessionClusterId'] = self.session_cluster_id
+        if self.state is not None:
+            result['state'] = self.state
+        if self.state_change_reason is not None:
+            result['stateChangeReason'] = self.state_change_reason.to_map()
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        if self.user_name is not None:
+            result['userName'] = self.user_name
+        if self.workspace_id is not None:
+            result['workspaceId'] = self.workspace_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.application_configs = []
+        if m.get('applicationConfigs') is not None:
+            for k in m.get('applicationConfigs'):
+                temp_model = ListSessionClustersResponseBodySessionClustersApplicationConfigs()
+                self.application_configs.append(temp_model.from_map(k))
+        if m.get('autoStartConfiguration') is not None:
+            temp_model = ListSessionClustersResponseBodySessionClustersAutoStartConfiguration()
+            self.auto_start_configuration = temp_model.from_map(m['autoStartConfiguration'])
+        if m.get('autoStopConfiguration') is not None:
+            temp_model = ListSessionClustersResponseBodySessionClustersAutoStopConfiguration()
+            self.auto_stop_configuration = temp_model.from_map(m['autoStopConfiguration'])
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('queueName') is not None:
+            self.queue_name = m.get('queueName')
+        if m.get('sessionClusterId') is not None:
+            self.session_cluster_id = m.get('sessionClusterId')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('stateChangeReason') is not None:
+            temp_model = ListSessionClustersResponseBodySessionClustersStateChangeReason()
+            self.state_change_reason = temp_model.from_map(m['stateChangeReason'])
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        if m.get('userName') is not None:
+            self.user_name = m.get('userName')
+        if m.get('workspaceId') is not None:
+            self.workspace_id = m.get('workspaceId')
+        return self
+
+
+class ListSessionClustersResponseBody(TeaModel):
+    def __init__(
+        self,
+        max_results: int = None,
+        next_token: str = None,
+        request_id: str = None,
+        session_clusters: List[ListSessionClustersResponseBodySessionClusters] = None,
+        total_count: int = None,
+    ):
+        # 本次请求所返回的最大记录条数。
+        self.max_results = max_results
+        # 返回读取到的数据位置，空代表数据已经读取完毕。
+        self.next_token = next_token
+        # 请求ID。
+        self.request_id = request_id
+        self.session_clusters = session_clusters
+        # 本次请求条件下的数据总量。
+        self.total_count = total_count
+
+    def validate(self):
+        if self.session_clusters:
+            for k in self.session_clusters:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        result['sessionClusters'] = []
+        if self.session_clusters is not None:
+            for k in self.session_clusters:
+                result['sessionClusters'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        self.session_clusters = []
+        if m.get('sessionClusters') is not None:
+            for k in m.get('sessionClusters'):
+                temp_model = ListSessionClustersResponseBodySessionClusters()
+                self.session_clusters.append(temp_model.from_map(k))
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class ListSessionClustersResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: ListSessionClustersResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = ListSessionClustersResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class ListWorkspaceQueuesRequest(TeaModel):
     def __init__(
         self,
         environment: str = None,
         region_id: str = None,
     ):
         self.environment = environment
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr-serverless-spark20230808
-Version: 1.1.0
+Version: 1.2.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt` & `alibabacloud_emr-serverless-spark20230808-1.2.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.1.0/setup.py` & `alibabacloud_emr-serverless-spark20230808-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr-serverless-spark20230808.
 
-Created on 20/05/2024
+Created on 21/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr_serverless_spark20230808"
 NAME = "alibabacloud_emr-serverless-spark20230808" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python"
```

