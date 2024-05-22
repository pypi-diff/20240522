# Comparing `tmp/alibabacloud_cbn20170912-1.1.1.tar.gz` & `tmp/alibabacloud_cbn20170912-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_cbn20170912-1.1.1.tar", last modified: Fri May 17 17:24:18 2024, max compression
+gzip compressed data, was "dist/alibabacloud_cbn20170912-1.1.2.tar", last modified: Wed May 22 17:11:33 2024, max compression
```

## Comparing `alibabacloud_cbn20170912-1.1.1.tar` & `alibabacloud_cbn20170912-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     6779 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2422 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1281666 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/client.py
--rw-r--r--   0 root         (0) root         (0)  1468039 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2422 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2632 2024-05-17 17:24:18.000000 alibabacloud_cbn20170912-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     7022 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1281666 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/client.py
+-rw-r--r--   0 root         (0) root         (0)  1468963 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2422 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2632 2024-05-22 17:11:33.000000 alibabacloud_cbn20170912-1.1.2/setup.py
```

### Comparing `alibabacloud_cbn20170912-1.1.1/ChangeLog.md` & `alibabacloud_cbn20170912-1.1.2/ChangeLog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+2024-05-17 Version: 1.1.1
+- Update API DescribeCenInterRegionBandwidthLimits: update response param.
+- Update API ListTransitRouterVpcAttachments: update response param.
+- Update API SetCenInterRegionBandwidthLimit: add param BandwidthType.
+
+
 2024-03-25 Version: 1.1.0
 - Support API CreateTransitRouterEcrAttachment.
 - Support API DeleteTransitRouterEcrAttachment.
 - Support API ListTransitRouterEcrAttachments.
 - Support API UpdateTransitRouterEcrAttachmentAttribute.
 - Update API DeleteTransitRouterVbrAttachment: update response param.
```

### Comparing `alibabacloud_cbn20170912-1.1.1/LICENSE` & `alibabacloud_cbn20170912-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.1.1/PKG-INFO` & `alibabacloud_cbn20170912-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_cbn20170912
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912-1.1.1/README-CN.md` & `alibabacloud_cbn20170912-1.1.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.1.1/README.md` & `alibabacloud_cbn20170912-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/client.py` & `alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912/models.py` & `alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16855,36 +16855,41 @@
     def __init__(
         self,
         cen_id: str = None,
         creation_time: str = None,
         description: str = None,
         flow_log_id: str = None,
         flow_log_name: str = None,
+        flow_log_version: str = None,
         interval: int = None,
+        log_format_string: str = None,
         log_store_name: str = None,
         project_name: str = None,
         region_id: str = None,
         status: str = None,
         tags: DescribeFlowlogsResponseBodyFlowLogsFlowLogTags = None,
         transit_router_attachment_id: str = None,
+        transit_router_id: str = None,
     ):
         # The ID of the CEN instance.
         self.cen_id = cen_id
         # The time when the flow log was created.
         # 
         # The time follows the ISO 8601 standard in the YYYY-MM-DDThh:mm:ssZ format. The time is displayed in UTC.
         self.creation_time = creation_time
         # The description of the flow log.
         self.description = description
         # The ID of the flow log.
         self.flow_log_id = flow_log_id
         # The name of the flow log.
         self.flow_log_name = flow_log_name
+        self.flow_log_version = flow_log_version
         # The time window for collecting log data. Unit: seconds. Valid values: **60** and **600**. Default value: **600**.
         self.interval = interval
+        self.log_format_string = log_format_string
         # The name of the Logstore where the flow log is stored.
         self.log_store_name = log_store_name
         # The name of the project where the flow log is stored.
         self.project_name = project_name
         # The ID of the region where the flow log is deployed.
         self.region_id = region_id
         # The status of the flow log. Valid values:
@@ -16892,14 +16897,15 @@
         # *   **Active**: The flow log is enabled.
         # *   **Inactive**: The flow log is disabled.
         self.status = status
         # A list of tags.
         self.tags = tags
         # The ID of the network instance connection.
         self.transit_router_attachment_id = transit_router_attachment_id
+        self.transit_router_id = transit_router_id
 
     def validate(self):
         if self.tags:
             self.tags.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -16913,57 +16919,69 @@
             result['CreationTime'] = self.creation_time
         if self.description is not None:
             result['Description'] = self.description
         if self.flow_log_id is not None:
             result['FlowLogId'] = self.flow_log_id
         if self.flow_log_name is not None:
             result['FlowLogName'] = self.flow_log_name
+        if self.flow_log_version is not None:
+            result['FlowLogVersion'] = self.flow_log_version
         if self.interval is not None:
             result['Interval'] = self.interval
+        if self.log_format_string is not None:
+            result['LogFormatString'] = self.log_format_string
         if self.log_store_name is not None:
             result['LogStoreName'] = self.log_store_name
         if self.project_name is not None:
             result['ProjectName'] = self.project_name
         if self.region_id is not None:
             result['RegionId'] = self.region_id
         if self.status is not None:
             result['Status'] = self.status
         if self.tags is not None:
             result['Tags'] = self.tags.to_map()
         if self.transit_router_attachment_id is not None:
             result['TransitRouterAttachmentId'] = self.transit_router_attachment_id
+        if self.transit_router_id is not None:
+            result['TransitRouterId'] = self.transit_router_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CenId') is not None:
             self.cen_id = m.get('CenId')
         if m.get('CreationTime') is not None:
             self.creation_time = m.get('CreationTime')
         if m.get('Description') is not None:
             self.description = m.get('Description')
         if m.get('FlowLogId') is not None:
             self.flow_log_id = m.get('FlowLogId')
         if m.get('FlowLogName') is not None:
             self.flow_log_name = m.get('FlowLogName')
+        if m.get('FlowLogVersion') is not None:
+            self.flow_log_version = m.get('FlowLogVersion')
         if m.get('Interval') is not None:
             self.interval = m.get('Interval')
+        if m.get('LogFormatString') is not None:
+            self.log_format_string = m.get('LogFormatString')
         if m.get('LogStoreName') is not None:
             self.log_store_name = m.get('LogStoreName')
         if m.get('ProjectName') is not None:
             self.project_name = m.get('ProjectName')
         if m.get('RegionId') is not None:
             self.region_id = m.get('RegionId')
         if m.get('Status') is not None:
             self.status = m.get('Status')
         if m.get('Tags') is not None:
             temp_model = DescribeFlowlogsResponseBodyFlowLogsFlowLogTags()
             self.tags = temp_model.from_map(m['Tags'])
         if m.get('TransitRouterAttachmentId') is not None:
             self.transit_router_attachment_id = m.get('TransitRouterAttachmentId')
+        if m.get('TransitRouterId') is not None:
+            self.transit_router_id = m.get('TransitRouterId')
         return self
 
 
 class DescribeFlowlogsResponseBodyFlowLogs(TeaModel):
     def __init__(
         self,
         flow_log: List[DescribeFlowlogsResponseBodyFlowLogsFlowLog] = None,
```

### Comparing `alibabacloud_cbn20170912-1.1.1/alibabacloud_cbn20170912.egg-info/PKG-INFO` & `alibabacloud_cbn20170912-1.1.2/alibabacloud_cbn20170912.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-cbn20170912
-Version: 1.1.1
+Version: 1.1.2
 Summary: Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_cbn20170912-1.1.1/setup.py` & `alibabacloud_cbn20170912-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_cbn20170912.
 
-Created on 17/05/2024
+Created on 22/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_cbn20170912"
 NAME = "alibabacloud_cbn20170912" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Cloud Enterprise Network (20170912) SDK Library for Python"
```

