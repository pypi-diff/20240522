# Comparing `tmp/aliyun-python-sdk-swas-open-1.0.6.tar.gz` & `tmp/aliyun-python-sdk-swas-open-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-swas-open-1.0.6.tar", last modified: Wed Mar 13 12:11:46 2024, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-swas-open-1.0.7.tar", last modified: Wed May 22 09:36:31 2024, max compression
```

## Comparing `aliyun-python-sdk-swas-open-1.0.6.tar` & `aliyun-python-sdk-swas-open-1.0.7.tar`

### file list

```diff
@@ -1,97 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      575 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      539 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5688 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/
--rw-r--r--   0 root         (0) root         (0)     1472 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2738 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     2653 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1937 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2064 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1615 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py
--rw-r--r--   0 root         (0) root         (0)     2693 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2002 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1392 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1579 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py
--rw-r--r--   0 root         (0) root         (0)     1404 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1412 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1645 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantAttributesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1448 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2586 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCommandInvocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2483 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCommandsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1295 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2019 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1422 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py
--rw-r--r--   0 root         (0) root         (0)     1440 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py
--rw-r--r--   0 root         (0) root         (0)     1420 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1794 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2482 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1430 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1748 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1949 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1249 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py
--rw-r--r--   0 root         (0) root         (0)     1587 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py
--rw-r--r--   0 root         (0) root         (0)     1784 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InvokeCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     3043 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2342 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2221 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1372 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1006 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     1225 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2577 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2294 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2307 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1587 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1623 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1404 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1611 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1561 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1571 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2964 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1410 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1219 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartTerminalSessionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1400 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1595 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2101 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2079 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1929 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateCommandAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1557 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1589 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1573 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1800 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-03-13 12:11:46.000000 aliyun-python-sdk-swas-open-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2482 2024-03-13 12:11:45.000000 aliyun-python-sdk-swas-open-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5821 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2064 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2002 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteCustomImagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteFirewallRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantAttributesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2586 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCommandInvocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCommandsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InvokeCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1225 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2577 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1219 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartTerminalSessionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2101 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateCommandAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2482 2024-05-22 09:36:31.000000 aliyun-python-sdk-swas-open-1.0.7/setup.py
```

### Comparing `aliyun-python-sdk-swas-open-1.0.6/LICENSE` & `aliyun-python-sdk-swas-open-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/PKG-INFO` & `aliyun-python-sdk-swas-open-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-swas-open
-Version: 1.0.6
+Version: 1.0.7
 Summary: The swas-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-swas-open
```

### Comparing `aliyun-python-sdk-swas-open-1.0.6/README.rst` & `aliyun-python-sdk-swas-open-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/PKG-INFO` & `aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-swas-open
-Version: 1.0.6
+Version: 1.0.7
 Summary: The swas-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-swas-open
```

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt` & `aliyun-python-sdk-swas-open-1.0.7/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
 aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py
 aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py
 aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteCommandRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
+aliyunsdkswas_open/request/v20200601/DeleteCustomImagesRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
+aliyunsdkswas_open/request/v20200601/DeleteFirewallRulesRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantAttributesRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeCommandInvocationsRequest.py
```

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateCommandRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteCommandRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantAttributesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantAttributesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCommandInvocationsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCommandInvocationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeCommandsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeCommandsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/InvokeCommandRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/InvokeCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ListTagResourcesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ListTagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StartTerminalSessionRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StartTerminalSessionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/TagResourcesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/TagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UntagResourcesRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UntagResourcesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateCommandAttributeRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateCommandAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py` & `aliyun-python-sdk-swas-open-1.0.7/aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.6/setup.py` & `aliyun-python-sdk-swas-open-1.0.7/setup.py`

 * *Files identical despite different names*

