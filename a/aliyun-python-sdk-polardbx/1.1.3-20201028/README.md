# Comparing `tmp/aliyun-python-sdk-polardbx-1.1.3.tar.gz` & `tmp/aliyun-python-sdk-polardbx-20201028.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-polardbx-1.1.3.tar", last modified: Wed May 22 03:33:22 2024, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-polardbx-20201028.tar", last modified: Wed Oct 28 02:53:59 2020, max compression
```

## Comparing `aliyun-python-sdk-polardbx-1.1.3.tar` & `aliyun-python-sdk-polardbx-20201028.tar`

### file list

```diff
@@ -1,91 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/
--rw-r--r--   0 root         (0) root         (0)      575 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5298 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3318 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/
--rw-r--r--   0 root         (0) root         (0)     2171 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AlignStoragePrimaryAzoneRequest.py
--rw-r--r--   0 root         (0) root         (0)     1516 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AllocateColdDataVolumeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2794 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AllocateInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1457 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CancelActiveOperationTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1928 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CheckCloudResourceAuthorizedRequest.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateBackupRequest.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     3351 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateDBRequest.py
--rw-r--r--   0 root         (0) root         (0)     2165 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateSuperAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     2209 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteAccountRequest.py
--rw-r--r--   0 root         (0) root         (0)     1504 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteDBRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeAccountListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1327 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationMaintainConfRequest.py
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationTaskCountRequest.py
--rw-r--r--   0 root         (0) root         (0)     3291 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeArchiveTableListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     2458 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeBackupSetListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1924 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeBackupSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     2449 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeBinaryLogListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeCharacterSetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1521 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeColdDataBasicInfoRequest.py
--rw-r--r--   0 root         (0) root         (0)     1747 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1711 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1512 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceHARequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceTopologyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1494 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceViaEndpointRequest.py
--rw-r--r--   0 root         (0) root         (0)     2596 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2614 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBNodePerformanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDbListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1693 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDistributeTableListRequest.py
--rw-r--r--   0 root         (0) root         (0)     2016 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeEventsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1703 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeParameterTemplatesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1687 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1287 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeScaleOutMigrateTaskListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1510 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeSecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeTagsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeUserEncryptionKeyListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1972 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DisableRightsSeparationRequest.py
--rw-r--r--   0 root         (0) root         (0)     3064 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/EnableRightsSeparationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2366 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1956 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyAccountDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2621 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyAccountPrivilegeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2315 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyActiveOperationMaintainConfRequest.py
--rw-r--r--   0 root         (0) root         (0)     1860 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyActiveOperationTasksRequest.py
--rw-r--r--   0 root         (0) root         (0)     3212 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceClassRequest.py
--rw-r--r--   0 root         (0) root         (0)     1904 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceConnectionStringRequest.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDatabaseDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2069 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     2097 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifySecurityIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1514 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ReleaseColdDataVolumeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2643 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ReleaseInstancePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2444 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ResetAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1506 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/RestartDBInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2422 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/SwitchDBInstanceHARequest.py
--rw-r--r--   0 root         (0) root         (0)     2173 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     6034 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UpdateBackupPolicyRequest.py
--rw-r--r--   0 root         (0) root         (0)     1912 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UpdateDBInstanceSSLRequest.py
--rw-r--r--   0 root         (0) root         (0)     2079 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UpdateDBInstanceTDERequest.py
--rw-r--r--   0 root         (0) root         (0)     2963 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UpdatePolarDBXInstanceNodeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1926 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/UpgradeDBInstanceKernelVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2024-05-22 03:33:22.000000 aliyun-python-sdk-polardbx-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2024-05-22 03:33:21.000000 aliyun-python-sdk-polardbx-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1565 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1565 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3521 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/
+-rw-r--r--   0 root         (0) root         (0)       24 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/
+-rw-r--r--   0 root         (0) root         (0)     2394 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/AllocateInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CheckHealthRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2160 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3494 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateDBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreatePolarxInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1814 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateSuperAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1382 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteAccountRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1210 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteDBRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeAccountListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1218 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeCharacterSetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1398 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1352 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDBInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDbListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDistributeTableListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1840 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeInstanceDbPerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeInstancePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeInstanceStoragePerformanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeModifyParameterLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeParameterTemplatesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1374 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1708 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribePolarxDbInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2012 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeScaleOutMigrateTaskListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeSecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeSqlAuditInfoRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeTableDetailRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2936 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeTasksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DisableSqlAuditRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/EnableSqlAuditRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1624 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyAccountDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1756 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyAccountPrivilegeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1636 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceClassRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1596 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceMaintainTimeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDatabaseDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifySecurityIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ReleaseInstancePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1598 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ResetAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ResetPolarxPgAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/RestartDBInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/UpgradeDBInstanceKernelVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-10-28 02:53:59.000000 aliyun-python-sdk-polardbx-20201028/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2020-10-28 02:53:58.000000 aliyun-python-sdk-polardbx-20201028/setup.py
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/PKG-INFO` & `aliyun-python-sdk-polardbx-20201028/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-polardbx
-Version: 1.1.3
+Version: 20201028
 Summary: The polardbx module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-polardbx
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/README.rst` & `aliyun-python-sdk-polardbx-20201028/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/PKG-INFO` & `aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-polardbx
-Version: 1.1.3
+Version: 20201028
 Summary: The polardbx module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-polardbx
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyun_python_sdk_polardbx.egg-info/SOURCES.txt` & `aliyun-python-sdk-polardbx-20201028/aliyun_python_sdk_polardbx.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,57 @@
-LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
 setup.py
 aliyun_python_sdk_polardbx.egg-info/PKG-INFO
 aliyun_python_sdk_polardbx.egg-info/SOURCES.txt
 aliyun_python_sdk_polardbx.egg-info/dependency_links.txt
 aliyun_python_sdk_polardbx.egg-info/requires.txt
 aliyun_python_sdk_polardbx.egg-info/top_level.txt
 aliyunsdkpolardbx/__init__.py
-aliyunsdkpolardbx/endpoint.py
 aliyunsdkpolardbx/request/__init__.py
-aliyunsdkpolardbx/request/v20200202/AlignStoragePrimaryAzoneRequest.py
-aliyunsdkpolardbx/request/v20200202/AllocateColdDataVolumeRequest.py
 aliyunsdkpolardbx/request/v20200202/AllocateInstancePublicConnectionRequest.py
-aliyunsdkpolardbx/request/v20200202/CancelActiveOperationTasksRequest.py
-aliyunsdkpolardbx/request/v20200202/ChangeResourceGroupRequest.py
-aliyunsdkpolardbx/request/v20200202/CheckCloudResourceAuthorizedRequest.py
+aliyunsdkpolardbx/request/v20200202/CheckHealthRequest.py
 aliyunsdkpolardbx/request/v20200202/CreateAccountRequest.py
-aliyunsdkpolardbx/request/v20200202/CreateBackupRequest.py
 aliyunsdkpolardbx/request/v20200202/CreateDBInstanceRequest.py
 aliyunsdkpolardbx/request/v20200202/CreateDBRequest.py
+aliyunsdkpolardbx/request/v20200202/CreatePolarxInstanceRequest.py
 aliyunsdkpolardbx/request/v20200202/CreateSuperAccountRequest.py
 aliyunsdkpolardbx/request/v20200202/DeleteAccountRequest.py
 aliyunsdkpolardbx/request/v20200202/DeleteDBInstanceRequest.py
 aliyunsdkpolardbx/request/v20200202/DeleteDBRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeAccountListRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationMaintainConfRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationTaskCountRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationTasksRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeArchiveTableListRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeBackupPolicyRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeBackupSetListRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeBackupSetRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeBinaryLogListRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeCharacterSetRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeColdDataBasicInfoRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceAttributeRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceConfigRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceHARequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceSSLRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceTDERequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceTopologyRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceViaEndpointRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeDBInstancesRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeDBNodePerformanceRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeDbListRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeDistributeTableListRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeEventsRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeInstanceDbPerformanceRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeInstancePerformanceRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeInstanceStoragePerformanceRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeModifyParameterLogRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeParameterTemplatesRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeParametersRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribePolarxDbInstancesRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeRegionsRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeScaleOutMigrateTaskListRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeSecurityIpsRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeTagsRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeSqlAuditInfoRequest.py
+aliyunsdkpolardbx/request/v20200202/DescribeTableDetailRequest.py
 aliyunsdkpolardbx/request/v20200202/DescribeTasksRequest.py
-aliyunsdkpolardbx/request/v20200202/DescribeUserEncryptionKeyListRequest.py
-aliyunsdkpolardbx/request/v20200202/DisableRightsSeparationRequest.py
-aliyunsdkpolardbx/request/v20200202/EnableRightsSeparationRequest.py
-aliyunsdkpolardbx/request/v20200202/ListTagResourcesRequest.py
+aliyunsdkpolardbx/request/v20200202/DisableSqlAuditRequest.py
+aliyunsdkpolardbx/request/v20200202/EnableSqlAuditRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyAccountDescriptionRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyAccountPrivilegeRequest.py
-aliyunsdkpolardbx/request/v20200202/ModifyActiveOperationMaintainConfRequest.py
-aliyunsdkpolardbx/request/v20200202/ModifyActiveOperationTasksRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceClassRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceConfigRequest.py
-aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceConnectionStringRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceDescriptionRequest.py
+aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceMaintainTimeRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyDatabaseDescriptionRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifyParameterRequest.py
 aliyunsdkpolardbx/request/v20200202/ModifySecurityIpsRequest.py
-aliyunsdkpolardbx/request/v20200202/ReleaseColdDataVolumeRequest.py
 aliyunsdkpolardbx/request/v20200202/ReleaseInstancePublicConnectionRequest.py
 aliyunsdkpolardbx/request/v20200202/ResetAccountPasswordRequest.py
+aliyunsdkpolardbx/request/v20200202/ResetPolarxPgAccountPasswordRequest.py
 aliyunsdkpolardbx/request/v20200202/RestartDBInstanceRequest.py
-aliyunsdkpolardbx/request/v20200202/SwitchDBInstanceHARequest.py
-aliyunsdkpolardbx/request/v20200202/TagResourcesRequest.py
-aliyunsdkpolardbx/request/v20200202/UntagResourcesRequest.py
-aliyunsdkpolardbx/request/v20200202/UpdateBackupPolicyRequest.py
-aliyunsdkpolardbx/request/v20200202/UpdateDBInstanceSSLRequest.py
-aliyunsdkpolardbx/request/v20200202/UpdateDBInstanceTDERequest.py
-aliyunsdkpolardbx/request/v20200202/UpdatePolarDBXInstanceNodeRequest.py
 aliyunsdkpolardbx/request/v20200202/UpgradeDBInstanceKernelVersionRequest.py
 aliyunsdkpolardbx/request/v20200202/__init__.py
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AlignStoragePrimaryAzoneRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeInstanceStoragePerformanceRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,40 +14,43 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class AlignStoragePrimaryAzoneRequest(RpcRequest):
+class DescribeInstanceStoragePerformanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'AlignStoragePrimaryAzone','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeInstanceStoragePerformance','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_SwitchTimeMode(self): # String
-		return self.get_query_params().get('SwitchTimeMode')
-
-	def set_SwitchTimeMode(self, SwitchTimeMode):  # String
-		self.add_query_param('SwitchTimeMode', SwitchTimeMode)
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
-
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
-	def get_StorageInstanceName(self): # String
-		return self.get_query_params().get('StorageInstanceName')
 
-	def set_StorageInstanceName(self, StorageInstanceName):  # String
-		self.add_query_param('StorageInstanceName', StorageInstanceName)
+	def get_DbInstanceName(self):
+		return self.get_query_params().get('DbInstanceName')
+
+	def set_DbInstanceName(self,DbInstanceName):
+		self.add_query_param('DbInstanceName',DbInstanceName)
+
+	def get_StorageInstanceId(self):
+		return self.get_query_params().get('StorageInstanceId')
+
+	def set_StorageInstanceId(self,StorageInstanceId):
+		self.add_query_param('StorageInstanceId',StorageInstanceId)
+
+	def get_Keys(self):
+		return self.get_query_params().get('Keys')
+
+	def set_Keys(self,Keys):
+		self.add_query_param('Keys',Keys)
+
+	def get_EndTime(self):
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self,EndTime):
+		self.add_query_param('EndTime',EndTime)
+
+	def get_StartTime(self):
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self,StartTime):
+		self.add_query_param('StartTime',StartTime)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AllocateColdDataVolumeRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/UpgradeDBInstanceKernelVersionRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,25 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class AllocateColdDataVolumeRequest(RpcRequest):
+class UpgradeDBInstanceKernelVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'AllocateColdDataVolume','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'UpgradeDBInstanceKernelVersion','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_SwitchTime(self):
+		return self.get_query_params().get('SwitchTime')
+
+	def set_SwitchTime(self,SwitchTime):
+		self.add_query_param('SwitchTime',SwitchTime)
+
+	def get_UpgradeTime(self):
+		return self.get_query_params().get('UpgradeTime')
+
+	def set_UpgradeTime(self,UpgradeTime):
+		self.add_query_param('UpgradeTime',UpgradeTime)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/AllocateInstancePublicConnectionRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ReleaseInstancePublicConnectionRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,55 +14,49 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class AllocateInstancePublicConnectionRequest(RpcRequest):
+class ReleaseInstancePublicConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'AllocateInstancePublicConnection','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ReleaseInstancePublicConnection','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_ResourceOwnerId(self): # Long
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
-		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ConnectionStringPrefix(self): # String
-		return self.get_query_params().get('ConnectionStringPrefix')
-
-	def set_ConnectionStringPrefix(self, ConnectionStringPrefix):  # String
-		self.add_query_param('ConnectionStringPrefix', ConnectionStringPrefix)
-	def get_ResourceOwnerAccount(self): # String
+	def set_ResourceOwnerId(self,ResourceOwnerId):
+		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
+
+	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
+	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
+		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
+
+	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
-	def get_OwnerId(self): # Long
+	def set_OwnerAccount(self,OwnerAccount):
+		self.add_query_param('OwnerAccount',OwnerAccount)
+
+	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
-	def get_Port(self): # String
-		return self.get_query_params().get('Port')
+	def set_OwnerId(self,OwnerId):
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_CurrentConnectionString(self):
+		return self.get_query_params().get('CurrentConnectionString')
 
-	def set_Port(self, Port):  # String
-		self.add_query_param('Port', Port)
+	def set_CurrentConnectionString(self,CurrentConnectionString):
+		self.add_query_param('CurrentConnectionString',CurrentConnectionString)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CancelActiveOperationTasksRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeSecurityIpsRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class CancelActiveOperationTasksRequest(RpcRequest):
+class DescribeSecurityIpsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'CancelActiveOperationTasks','polardbx')
-		self.set_method('GET')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeSecurityIps','polardbx')
+		self.set_method('POST')
 
-	def get_Ids(self): # String
-		return self.get_query_params().get('Ids')
+	def get_DBInstanceName(self):
+		return self.get_query_params().get('DBInstanceName')
 
-	def set_Ids(self, Ids):  # String
-		self.add_query_param('Ids', Ids)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CheckCloudResourceAuthorizedRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDBInstanceMaintainTimeRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,30 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class CheckCloudResourceAuthorizedRequest(RpcRequest):
+class ModifyDBInstanceMaintainTimeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'CheckCloudResourceAuthorized','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyDBInstanceMaintainTime','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_RoleArn(self): # String
-		return self.get_query_params().get('RoleArn')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
+	def get_MaintainTime(self):
+		return self.get_query_params().get('MaintainTime')
 
-	def set_RoleArn(self, RoleArn):  # String
-		self.add_query_param('RoleArn', RoleArn)
+	def set_MaintainTime(self,MaintainTime):
+		self.add_query_param('MaintainTime',MaintainTime)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/CreateSuperAccountRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateSuperAccountRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,40 +14,37 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
 class CreateSuperAccountRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'CreateSuperAccount','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_AccountDescription(self): # String
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_AccountDescription(self):
 		return self.get_query_params().get('AccountDescription')
 
-	def set_AccountDescription(self, AccountDescription):  # String
-		self.add_query_param('AccountDescription', AccountDescription)
-	def get_AccountPassword(self): # String
+	def set_AccountDescription(self,AccountDescription):
+		self.add_query_param('AccountDescription',AccountDescription)
+
+	def get_AccountPassword(self):
 		return self.get_query_params().get('AccountPassword')
 
-	def set_AccountPassword(self, AccountPassword):  # String
-		self.add_query_param('AccountPassword', AccountPassword)
-	def get_AccountName(self): # String
+	def set_AccountPassword(self,AccountPassword):
+		self.add_query_param('AccountPassword',AccountPassword)
+
+	def get_AccountName(self):
 		return self.get_query_params().get('AccountName')
 
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
+	def set_AccountName(self,AccountName):
+		self.add_query_param('AccountName',AccountName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteAccountRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyParameterRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,40 +14,37 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DeleteAccountRequest(RpcRequest):
+class ModifyParameterRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteAccount','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyParameter','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_SecurityAccountPassword(self): # String
-		return self.get_query_params().get('SecurityAccountPassword')
-
-	def set_SecurityAccountPassword(self, SecurityAccountPassword):  # String
-		self.add_query_param('SecurityAccountPassword', SecurityAccountPassword)
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
-
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
-	def get_SecurityAccountName(self): # String
-		return self.get_query_params().get('SecurityAccountName')
 
-	def set_SecurityAccountName(self, SecurityAccountName):  # String
-		self.add_query_param('SecurityAccountName', SecurityAccountName)
+	def get_ClientToken(self):
+		return self.get_query_params().get('ClientToken')
+
+	def set_ClientToken(self,ClientToken):
+		self.add_query_param('ClientToken',ClientToken)
+
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
+
+	def get_ParamLevel(self):
+		return self.get_query_params().get('ParamLevel')
+
+	def set_ParamLevel(self,ParamLevel):
+		self.add_query_param('ParamLevel',ParamLevel)
+
+	def get_Parameters(self):
+		return self.get_query_params().get('Parameters')
+
+	def set_Parameters(self,Parameters):
+		self.add_query_param('Parameters',Parameters)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteDBInstanceRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceAttributeRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DeleteDBInstanceRequest(RpcRequest):
+class DescribeDBInstanceAttributeRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteDBInstance','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDBInstanceAttribute','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DeleteDBRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/RestartDBInstanceRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DeleteDBRequest(RpcRequest):
+class RestartDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteDB','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'RestartDBInstance','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_DbName(self): # String
-		return self.get_query_params().get('DbName')
-
-	def set_DbName(self, DbName):  # String
-		self.add_query_param('DbName', DbName)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeActiveOperationMaintainConfRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeSqlAuditInfoRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,20 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeActiveOperationMaintainConfRequest(RpcRequest):
+class DescribeSqlAuditInfoRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeActiveOperationMaintainConf','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeSqlAuditInfo','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeArchiveTableListRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeModifyParameterLogRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,50 +14,49 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeArchiveTableListRequest(RpcRequest):
+class DescribeModifyParameterLogRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeArchiveTableList','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeModifyParameterLog','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_PageSize(self): # Long
+
+	def get_StartTime(self):
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self,StartTime):
+		self.add_query_param('StartTime',StartTime)
+
+	def get_PageNumber(self):
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self,PageNumber):
+		self.add_query_param('PageNumber',PageNumber)
+
+	def get_PageSize(self):
 		return self.get_query_params().get('PageSize')
 
-	def set_PageSize(self, PageSize):  # Long
-		self.add_query_param('PageSize', PageSize)
-	def get_PageIndex(self): # Long
-		return self.get_query_params().get('PageIndex')
-
-	def set_PageIndex(self, PageIndex):  # Long
-		self.add_query_param('PageIndex', PageIndex)
-	def get_TableName(self): # String
-		return self.get_query_params().get('TableName')
-
-	def set_TableName(self, TableName):  # String
-		self.add_query_param('TableName', TableName)
-	def get_SchemaName(self): # String
-		return self.get_query_params().get('SchemaName')
-
-	def set_SchemaName(self, SchemaName):  # String
-		self.add_query_param('SchemaName', SchemaName)
-	def get_Status(self): # String
-		return self.get_query_params().get('Status')
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
+
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
+
+	def get_ParamLevel(self):
+		return self.get_query_params().get('ParamLevel')
+
+	def set_ParamLevel(self,ParamLevel):
+		self.add_query_param('ParamLevel',ParamLevel)
+
+	def get_EndTime(self):
+		return self.get_query_params().get('EndTime')
 
-	def set_Status(self, Status):  # String
-		self.add_query_param('Status', Status)
+	def set_EndTime(self,EndTime):
+		self.add_query_param('EndTime',EndTime)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeBackupPolicyRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteDBInstanceRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeBackupPolicyRequest(RpcRequest):
+class DeleteDBInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeBackupPolicy','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteDBInstance','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceAttributeRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeCharacterSetRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,30 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeDBInstanceAttributeRequest(RpcRequest):
+class DescribeCharacterSetRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDBInstanceAttribute','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeCharacterSet','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_ResourceGroupId(self): # String
-		return self.get_query_params().get('ResourceGroupId')
-
-	def set_ResourceGroupId(self, ResourceGroupId):  # String
-		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceConfigRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeDbListRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,30 +14,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeDBInstanceConfigRequest(RpcRequest):
+class DescribeDbListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDBInstanceConfig','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDbList','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_ConfigName(self): # String
-		return self.get_query_params().get('ConfigName')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_DBName(self):
+		return self.get_query_params().get('DBName')
 
-	def set_ConfigName(self, ConfigName):  # String
-		self.add_query_param('ConfigName', ConfigName)
+	def set_DBName(self,DBName):
+		self.add_query_param('DBName',DBName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBInstanceViaEndpointRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DisableSqlAuditRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,25 +14,19 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeDBInstanceViaEndpointRequest(RpcRequest):
+class DisableSqlAuditRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDBInstanceViaEndpoint','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DisableSqlAudit','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Endpoint(self): # String
-		return self.get_query_params().get('Endpoint')
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
 
-	def set_Endpoint(self, Endpoint):  # String
-		self.add_query_param('Endpoint', Endpoint)
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDBNodePerformanceRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeTasksRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,55 +14,79 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeDBNodePerformanceRequest(RpcRequest):
+class DescribeTasksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDBNodePerformance','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeTasks','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_StartTime(self): # String
+	def get_ResourceOwnerId(self):
+		return self.get_query_params().get('ResourceOwnerId')
+
+	def set_ResourceOwnerId(self,ResourceOwnerId):
+		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
+
+	def get_StartTime(self):
 		return self.get_query_params().get('StartTime')
 
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_DBNodeRole(self): # String
-		return self.get_query_params().get('DBNodeRole')
-
-	def set_DBNodeRole(self, DBNodeRole):  # String
-		self.add_query_param('DBNodeRole', DBNodeRole)
-	def get_CharacterType(self): # String
-		return self.get_query_params().get('CharacterType')
-
-	def set_CharacterType(self, CharacterType):  # String
-		self.add_query_param('CharacterType', CharacterType)
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_DBNodeIds(self): # String
-		return self.get_query_params().get('DBNodeIds')
-
-	def set_DBNodeIds(self, DBNodeIds):  # String
-		self.add_query_param('DBNodeIds', DBNodeIds)
-	def get_Key(self): # String
-		return self.get_query_params().get('Key')
-
-	def set_Key(self, Key):  # String
-		self.add_query_param('Key', Key)
-	def get_EndTime(self): # String
+	def set_StartTime(self,StartTime):
+		self.add_query_param('StartTime',StartTime)
+
+	def get_PageNumber(self):
+		return self.get_query_params().get('PageNumber')
+
+	def set_PageNumber(self,PageNumber):
+		self.add_query_param('PageNumber',PageNumber)
+
+	def get_PageSize(self):
+		return self.get_query_params().get('PageSize')
+
+	def set_PageSize(self,PageSize):
+		self.add_query_param('PageSize',PageSize)
+
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
+
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
+
+	def get_ResourceOwnerAccount(self):
+		return self.get_query_params().get('ResourceOwnerAccount')
+
+	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
+		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
+
+	def get_OwnerAccount(self):
+		return self.get_query_params().get('OwnerAccount')
+
+	def set_OwnerAccount(self,OwnerAccount):
+		self.add_query_param('OwnerAccount',OwnerAccount)
+
+	def get_EndTime(self):
 		return self.get_query_params().get('EndTime')
 
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
+	def set_EndTime(self,EndTime):
+		self.add_query_param('EndTime',EndTime)
+
+	def get_OwnerId(self):
+		return self.get_query_params().get('OwnerId')
+
+	def set_OwnerId(self,OwnerId):
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_TaskAction(self):
+		return self.get_query_params().get('TaskAction')
+
+	def set_TaskAction(self,TaskAction):
+		self.add_query_param('TaskAction',TaskAction)
+
+	def get_Status(self):
+		return self.get_query_params().get('Status')
+
+	def set_Status(self,Status):
+		self.add_query_param('Status',Status)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeDbListRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteDBRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,30 +14,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeDbListRequest(RpcRequest):
+class DeleteDBRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeDbList','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteDB','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_DBName(self): # String
-		return self.get_query_params().get('DBName')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_DbName(self):
+		return self.get_query_params().get('DbName')
 
-	def set_DBName(self, DBName):  # String
-		self.add_query_param('DBName', DBName)
+	def set_DbName(self,DbName):
+		self.add_query_param('DbName',DbName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeParameterTemplatesRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeParameterTemplatesRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,30 +14,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
 class DescribeParameterTemplatesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeParameterTemplates','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceId(self): # String
+	def get_DBInstanceId(self):
 		return self.get_query_params().get('DBInstanceId')
 
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_ParamLevel(self): # String
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
+
+	def get_ParamLevel(self):
 		return self.get_query_params().get('ParamLevel')
 
-	def set_ParamLevel(self, ParamLevel):  # String
-		self.add_query_param('ParamLevel', ParamLevel)
+	def set_ParamLevel(self,ParamLevel):
+		self.add_query_param('ParamLevel',ParamLevel)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeParametersRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DeleteAccountRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeParametersRequest(RpcRequest):
+class DeleteAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeParameters','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DeleteAccount','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
+	def get_DBInstanceName(self):
+		return self.get_query_params().get('DBInstanceName')
+
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
 
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_ParamLevel(self): # String
-		return self.get_query_params().get('ParamLevel')
+	def get_AccountName(self):
+		return self.get_query_params().get('AccountName')
 
-	def set_ParamLevel(self, ParamLevel):  # String
-		self.add_query_param('ParamLevel', ParamLevel)
+	def set_AccountName(self,AccountName):
+		self.add_query_param('AccountName',AccountName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeRegionsRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CheckHealthRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,20 +14,13 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeRegionsRequest(RpcRequest):
+class CheckHealthRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeRegions','polardbx')
-		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'CheckHealth','polardbx')
+		self.set_method('POST')
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeScaleOutMigrateTaskListRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeScaleOutMigrateTaskListRequest.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,45 +14,43 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
 class DescribeScaleOutMigrateTaskListRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeScaleOutMigrateTaskList','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_ResourceOwnerId(self): # Long
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
-		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_ResourceOwnerAccount(self): # String
+	def set_ResourceOwnerId(self,ResourceOwnerId):
+		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
+
+	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
+	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
+		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
+
+	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
-	def get_OwnerId(self): # Long
+	def set_OwnerAccount(self,OwnerAccount):
+		self.add_query_param('OwnerAccount',OwnerAccount)
+
+	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
+	def set_OwnerId(self,OwnerId):
+		self.add_query_param('OwnerId',OwnerId)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DescribeTasksRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/AllocateInstancePublicConnectionRequest.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,65 +14,55 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DescribeTasksRequest(RpcRequest):
+class AllocateInstancePublicConnectionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeTasks','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'AllocateInstancePublicConnection','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ResourceOwnerId(self): # Long
+	def get_DBInstanceName(self):
+		return self.get_query_params().get('DBInstanceName')
+
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_ResourceOwnerId(self):
 		return self.get_query_params().get('ResourceOwnerId')
 
-	def set_ResourceOwnerId(self, ResourceOwnerId):  # Long
-		self.add_query_param('ResourceOwnerId', ResourceOwnerId)
-	def get_StartTime(self): # String
-		return self.get_query_params().get('StartTime')
-
-	def set_StartTime(self, StartTime):  # String
-		self.add_query_param('StartTime', StartTime)
-	def get_PageNumber(self): # Integer
-		return self.get_query_params().get('PageNumber')
-
-	def set_PageNumber(self, PageNumber):  # Integer
-		self.add_query_param('PageNumber', PageNumber)
-	def get_PageSize(self): # Integer
-		return self.get_query_params().get('PageSize')
-
-	def set_PageSize(self, PageSize):  # Integer
-		self.add_query_param('PageSize', PageSize)
-	def get_DBInstanceId(self): # String
-		return self.get_query_params().get('DBInstanceId')
-
-	def set_DBInstanceId(self, DBInstanceId):  # String
-		self.add_query_param('DBInstanceId', DBInstanceId)
-	def get_ResourceOwnerAccount(self): # String
+	def set_ResourceOwnerId(self,ResourceOwnerId):
+		self.add_query_param('ResourceOwnerId',ResourceOwnerId)
+
+	def get_ConnectionStringPrefix(self):
+		return self.get_query_params().get('ConnectionStringPrefix')
+
+	def set_ConnectionStringPrefix(self,ConnectionStringPrefix):
+		self.add_query_param('ConnectionStringPrefix',ConnectionStringPrefix)
+
+	def get_ResourceOwnerAccount(self):
 		return self.get_query_params().get('ResourceOwnerAccount')
 
-	def set_ResourceOwnerAccount(self, ResourceOwnerAccount):  # String
-		self.add_query_param('ResourceOwnerAccount', ResourceOwnerAccount)
-	def get_OwnerAccount(self): # String
+	def set_ResourceOwnerAccount(self,ResourceOwnerAccount):
+		self.add_query_param('ResourceOwnerAccount',ResourceOwnerAccount)
+
+	def get_OwnerAccount(self):
 		return self.get_query_params().get('OwnerAccount')
 
-	def set_OwnerAccount(self, OwnerAccount):  # String
-		self.add_query_param('OwnerAccount', OwnerAccount)
-	def get_EndTime(self): # String
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # String
-		self.add_query_param('EndTime', EndTime)
-	def get_OwnerId(self): # Long
+	def set_OwnerAccount(self,OwnerAccount):
+		self.add_query_param('OwnerAccount',OwnerAccount)
+
+	def get_OwnerId(self):
 		return self.get_query_params().get('OwnerId')
 
-	def set_OwnerId(self, OwnerId):  # Long
-		self.add_query_param('OwnerId', OwnerId)
+	def set_OwnerId(self,OwnerId):
+		self.add_query_param('OwnerId',OwnerId)
+
+	def get_Port(self):
+		return self.get_query_params().get('Port')
+
+	def set_Port(self,Port):
+		self.add_query_param('Port',Port)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/DisableRightsSeparationRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ResetPolarxPgAccountPasswordRequest.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,35 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class DisableRightsSeparationRequest(RpcRequest):
+class ResetPolarxPgAccountPasswordRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DisableRightsSeparation','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ResetPolarxPgAccountPassword','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_DbaAccountPassword(self): # String
-		return self.get_query_params().get('DbaAccountPassword')
-
-	def set_DbaAccountPassword(self, DbaAccountPassword):  # String
-		self.add_query_param('DbaAccountPassword', DbaAccountPassword)
-	def get_DbaAccountName(self): # String
-		return self.get_query_params().get('DbaAccountName')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_AccountPassword(self):
+		return self.get_query_params().get('AccountPassword')
+
+	def set_AccountPassword(self,AccountPassword):
+		self.add_query_param('AccountPassword',AccountPassword)
+
+	def get_AccountName(self):
+		return self.get_query_params().get('AccountName')
 
-	def set_DbaAccountName(self, DbaAccountName):  # String
-		self.add_query_param('DbaAccountName', DbaAccountName)
+	def set_AccountName(self,AccountName):
+		self.add_query_param('AccountName',AccountName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ListTagResourcesRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeTableDetailRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,45 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class ListTagResourcesRequest(RpcRequest):
+class DescribeTableDetailRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ListTagResources','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeTableDetail','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
-	def get_Tags(self): # RepeatList
-		return self.get_query_params().get('Tag')
-
-	def set_Tags(self, Tag):  # RepeatList
-		for depth1 in range(len(Tag)):
-			if Tag[depth1].get('Value') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
-			if Tag[depth1].get('Key') is not None:
-				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
-	def get_ResourceIds(self): # RepeatList
-		return self.get_query_params().get('ResourceId')
-
-	def set_ResourceIds(self, ResourceId):  # RepeatList
-		for depth1 in range(len(ResourceId)):
-			self.add_query_param('ResourceId.' + str(depth1 + 1), ResourceId[depth1])
-	def get_ResourceType(self): # String
-		return self.get_query_params().get('ResourceType')
 
-	def set_ResourceType(self, ResourceType):  # String
-		self.add_query_param('ResourceType', ResourceType)
+	def get_DBInstanceName(self):
+		return self.get_query_params().get('DBInstanceName')
+
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_DbName(self):
+		return self.get_query_params().get('DbName')
+
+	def set_DbName(self,DbName):
+		self.add_query_param('DbName',DbName)
+
+	def get_TableName(self):
+		return self.get_query_params().get('TableName')
+
+	def set_TableName(self,TableName):
+		self.add_query_param('TableName',TableName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyAccountDescriptionRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ModifyDatabaseDescriptionRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,35 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class ModifyAccountDescriptionRequest(RpcRequest):
+class ModifyDatabaseDescriptionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyAccountDescription','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyDatabaseDescription','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_AccountDescription(self): # String
-		return self.get_query_params().get('AccountDescription')
-
-	def set_AccountDescription(self, AccountDescription):  # String
-		self.add_query_param('AccountDescription', AccountDescription)
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_DbName(self):
+		return self.get_query_params().get('DbName')
+
+	def set_DbName(self,DbName):
+		self.add_query_param('DbName',DbName)
+
+	def get_DbDescription(self):
+		return self.get_query_params().get('DbDescription')
 
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
+	def set_DbDescription(self,DbDescription):
+		self.add_query_param('DbDescription',DbDescription)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyActiveOperationTasksRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeParametersRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,35 +14,25 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class ModifyActiveOperationTasksRequest(RpcRequest):
+class DescribeParametersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyActiveOperationTasks','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeParameters','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
+	def get_DBInstanceId(self):
+		return self.get_query_params().get('DBInstanceId')
 
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
-	def get_Ids(self): # String
-		return self.get_query_params().get('Ids')
+	def set_DBInstanceId(self,DBInstanceId):
+		self.add_query_param('DBInstanceId',DBInstanceId)
 
-	def set_Ids(self, Ids):  # String
-		self.add_query_param('Ids', Ids)
-	def get_ImmediateStart(self): # Long
-		return self.get_query_params().get('ImmediateStart')
+	def get_ParamLevel(self):
+		return self.get_query_params().get('ParamLevel')
 
-	def set_ImmediateStart(self, ImmediateStart):  # Long
-		self.add_query_param('ImmediateStart', ImmediateStart)
+	def set_ParamLevel(self,ParamLevel):
+		self.add_query_param('ParamLevel',ParamLevel)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ModifyDatabaseDescriptionRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeInstancePerformanceRequest.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,35 +14,43 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class ModifyDatabaseDescriptionRequest(RpcRequest):
+class DescribeInstancePerformanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ModifyDatabaseDescription','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeInstancePerformance','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_DbName(self): # String
-		return self.get_query_params().get('DbName')
-
-	def set_DbName(self, DbName):  # String
-		self.add_query_param('DbName', DbName)
-	def get_DbDescription(self): # String
-		return self.get_query_params().get('DbDescription')
 
-	def set_DbDescription(self, DbDescription):  # String
-		self.add_query_param('DbDescription', DbDescription)
+	def get_DbInstanceName(self):
+		return self.get_query_params().get('DbInstanceName')
+
+	def set_DbInstanceName(self,DbInstanceName):
+		self.add_query_param('DbInstanceName',DbInstanceName)
+
+	def get_Keys(self):
+		return self.get_query_params().get('Keys')
+
+	def set_Keys(self,Keys):
+		self.add_query_param('Keys',Keys)
+
+	def get_EndTime(self):
+		return self.get_query_params().get('EndTime')
+
+	def set_EndTime(self,EndTime):
+		self.add_query_param('EndTime',EndTime)
+
+	def get_StartTime(self):
+		return self.get_query_params().get('StartTime')
+
+	def set_StartTime(self,StartTime):
+		self.add_query_param('StartTime',StartTime)
+
+	def get_NodeId(self):
+		return self.get_query_params().get('NodeId')
+
+	def set_NodeId(self,NodeId):
+		self.add_query_param('NodeId',NodeId)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/ResetAccountPasswordRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/ResetAccountPasswordRequest.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,45 +14,31 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
 class ResetAccountPasswordRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'ResetAccountPassword','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_SecurityAccountPassword(self): # String
-		return self.get_query_params().get('SecurityAccountPassword')
-
-	def set_SecurityAccountPassword(self, SecurityAccountPassword):  # String
-		self.add_query_param('SecurityAccountPassword', SecurityAccountPassword)
-	def get_AccountPassword(self): # String
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_AccountPassword(self):
 		return self.get_query_params().get('AccountPassword')
 
-	def set_AccountPassword(self, AccountPassword):  # String
-		self.add_query_param('AccountPassword', AccountPassword)
-	def get_AccountName(self): # String
-		return self.get_query_params().get('AccountName')
+	def set_AccountPassword(self,AccountPassword):
+		self.add_query_param('AccountPassword',AccountPassword)
 
-	def set_AccountName(self, AccountName):  # String
-		self.add_query_param('AccountName', AccountName)
-	def get_SecurityAccountName(self): # String
-		return self.get_query_params().get('SecurityAccountName')
+	def get_AccountName(self):
+		return self.get_query_params().get('AccountName')
 
-	def set_SecurityAccountName(self, SecurityAccountName):  # String
-		self.add_query_param('SecurityAccountName', SecurityAccountName)
+	def set_AccountName(self,AccountName):
+		self.add_query_param('AccountName',AccountName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/RestartDBInstanceRequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/DescribeRegionsRequest.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,25 +14,13 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class RestartDBInstanceRequest(RpcRequest):
+class DescribeRegionsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'RestartDBInstance','polardbx')
-		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
-
-	def get_DBInstanceName(self): # String
-		return self.get_query_params().get('DBInstanceName')
-
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'DescribeRegions','polardbx')
+		self.set_method('POST')
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/aliyunsdkpolardbx/request/v20200202/SwitchDBInstanceHARequest.py` & `aliyun-python-sdk-polardbx-20201028/aliyunsdkpolardbx/request/v20200202/CreateAccountRequest.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,45 +14,49 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
-from aliyunsdkpolardbx.endpoint import endpoint_data
 
-class SwitchDBInstanceHARequest(RpcRequest):
+class CreateAccountRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'SwitchDBInstanceHA','polardbx')
+		RpcRequest.__init__(self, 'polardbx', '2020-02-02', 'CreateAccount','polardbx')
 		self.set_method('POST')
-
-		if hasattr(self, "endpoint_map"):
-			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
-		if hasattr(self, "endpoint_regional"):
-			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DBInstanceName(self): # String
+	def get_DBInstanceName(self):
 		return self.get_query_params().get('DBInstanceName')
 
-	def set_DBInstanceName(self, DBInstanceName):  # String
-		self.add_query_param('DBInstanceName', DBInstanceName)
-	def get_TargetPrimaryRegionId(self): # String
-		return self.get_query_params().get('TargetPrimaryRegionId')
-
-	def set_TargetPrimaryRegionId(self, TargetPrimaryRegionId):  # String
-		self.add_query_param('TargetPrimaryRegionId', TargetPrimaryRegionId)
-	def get_SwitchTimeMode(self): # String
-		return self.get_query_params().get('SwitchTimeMode')
-
-	def set_SwitchTimeMode(self, SwitchTimeMode):  # String
-		self.add_query_param('SwitchTimeMode', SwitchTimeMode)
-	def get_TargetPrimaryAzoneId(self): # String
-		return self.get_query_params().get('TargetPrimaryAzoneId')
-
-	def set_TargetPrimaryAzoneId(self, TargetPrimaryAzoneId):  # String
-		self.add_query_param('TargetPrimaryAzoneId', TargetPrimaryAzoneId)
-	def get_SwitchTime(self): # String
-		return self.get_query_params().get('SwitchTime')
+	def set_DBInstanceName(self,DBInstanceName):
+		self.add_query_param('DBInstanceName',DBInstanceName)
+
+	def get_AccountDescription(self):
+		return self.get_query_params().get('AccountDescription')
+
+	def set_AccountDescription(self,AccountDescription):
+		self.add_query_param('AccountDescription',AccountDescription)
+
+	def get_AccountPrivilege(self):
+		return self.get_query_params().get('AccountPrivilege')
+
+	def set_AccountPrivilege(self,AccountPrivilege):
+		self.add_query_param('AccountPrivilege',AccountPrivilege)
+
+	def get_AccountPassword(self):
+		return self.get_query_params().get('AccountPassword')
+
+	def set_AccountPassword(self,AccountPassword):
+		self.add_query_param('AccountPassword',AccountPassword)
+
+	def get_AccountName(self):
+		return self.get_query_params().get('AccountName')
+
+	def set_AccountName(self,AccountName):
+		self.add_query_param('AccountName',AccountName)
+
+	def get_DBName(self):
+		return self.get_query_params().get('DBName')
 
-	def set_SwitchTime(self, SwitchTime):  # String
-		self.add_query_param('SwitchTime', SwitchTime)
+	def set_DBName(self,DBName):
+		self.add_query_param('DBName',DBName)
```

### Comparing `aliyun-python-sdk-polardbx-1.1.3/setup.py` & `aliyun-python-sdk-polardbx-20201028/setup.py`

 * *Files identical despite different names*

