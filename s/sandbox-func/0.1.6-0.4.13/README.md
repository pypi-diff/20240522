# Comparing `tmp/sandbox_func-0.1.6.tar.gz` & `tmp/sandbox_func-0.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sandbox_func-0.1.6.tar", last modified: Mon Oct 23 07:39:17 2023, max compression
+gzip compressed data, was "sandbox_func-0.4.13.tar", last modified: Wed May 22 02:27:33 2024, max compression
```

## Comparing `sandbox_func-0.1.6.tar` & `sandbox_func-0.4.13.tar`

### file list

```diff
@@ -1,87 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.831222 sandbox_func-0.1.6/
--rw-rw-rw-   0        0        0       83 2023-10-23 07:39:17.830211 sandbox_func-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-09-08 03:36:49.000000 sandbox_func-0.1.6/README.md
--rw-rw-rw-   0        0        0      894 2023-10-23 07:39:10.000000 sandbox_func-0.1.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.207057 sandbox_func-0.1.6/sandbox_func/
--rw-rw-rw-   0        0        0      234 2023-09-28 03:01:36.000000 sandbox_func-0.1.6/sandbox_func/__init__.py
--rw-rw-rw-   0        0        0      421 2023-09-25 10:08:35.000000 sandbox_func-0.1.6/sandbox_func/__main__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.244564 sandbox_func-0.1.6/sandbox_func/common/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.305812 sandbox_func-0.1.6/sandbox_func/common/config/
--rw-rw-rw-   0        0        0      641 2023-10-19 10:01:08.000000 sandbox_func-0.1.6/sandbox_func/common/config/BaseURLConfig.py
--rw-rw-rw-   0        0        0      441 2023-09-19 08:30:36.000000 sandbox_func-0.1.6/sandbox_func/common/config/BusinessURLConfig.py
--rw-rw-rw-   0        0        0      236 2023-09-14 08:52:32.000000 sandbox_func-0.1.6/sandbox_func/common/config/ConfigModel.py
--rw-rw-rw-   0        0        0      208 2023-10-19 09:54:07.000000 sandbox_func-0.1.6/sandbox_func/common/config/LogConfig.py
--rw-rw-rw-   0        0        0     3276 2023-09-21 05:56:15.000000 sandbox_func-0.1.6/sandbox_func/common/config/LoginConfig.py
--rw-rw-rw-   0        0        0       41 2023-10-16 12:22:24.000000 sandbox_func-0.1.6/sandbox_func/common/config/TencentConfig.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/config/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.328977 sandbox_func-0.1.6/sandbox_func/common/file/
--rw-rw-rw-   0        0        0     5009 2023-09-19 08:34:17.000000 sandbox_func-0.1.6/sandbox_func/common/file/CosFileManager.py
--rw-rw-rw-   0        0        0        0 2023-09-14 09:08:59.000000 sandbox_func-0.1.6/sandbox_func/common/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.400644 sandbox_func-0.1.6/sandbox_func/common/lang/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/lang/__init__.py
--rw-rw-rw-   0        0        0     3300 2023-09-22 07:14:06.000000 sandbox_func-0.1.6/sandbox_func/common/lang/async_requests.py
--rw-rw-rw-   0        0        0     2706 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/common/lang/dictclass.py
--rw-rw-rw-   0        0        0      232 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/lang/logger_setting.py
--rw-rw-rw-   0        0        0      339 2023-10-16 11:56:50.000000 sandbox_func-0.1.6/sandbox_func/common/lang/moduleutil.py
--rw-rw-rw-   0        0        0     1466 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/common/lang/singleton.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.426217 sandbox_func-0.1.6/sandbox_func/common/local/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/local/__init__.py
--rw-rw-rw-   0        0        0      763 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/local/clientinfo.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.456426 sandbox_func-0.1.6/sandbox_func/common/log/
--rw-rw-rw-   0        0        0     2565 2023-10-19 10:01:48.000000 sandbox_func-0.1.6/sandbox_func/common/log/AwLogger.py
--rw-rw-rw-   0        0        0      439 2023-10-16 12:15:03.000000 sandbox_func-0.1.6/sandbox_func/common/log/LogManager.py
--rw-rw-rw-   0        0        0        0 2023-09-14 08:49:17.000000 sandbox_func-0.1.6/sandbox_func/common/log/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.491717 sandbox_func-0.1.6/sandbox_func/common/request/
--rw-rw-rw-   0        0        0     1432 2023-09-22 07:54:08.000000 sandbox_func-0.1.6/sandbox_func/common/request/CybotronClient.py
--rw-rw-rw-   0        0        0      682 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/common/request/CybotronSyncClient.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/common/request/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.553647 sandbox_func-0.1.6/sandbox_func/model/
--rw-rw-rw-   0        0        0      304 2023-09-14 03:07:22.000000 sandbox_func-0.1.6/sandbox_func/model/SandboxApp.py
--rw-rw-rw-   0        0        0      273 2023-09-22 05:31:59.000000 sandbox_func-0.1.6/sandbox_func/model/SandboxFunc.py
--rw-rw-rw-   0        0        0     2137 2023-09-27 10:38:53.000000 sandbox_func-0.1.6/sandbox_func/model/SandboxFuncManager.py
--rw-rw-rw-   0        0        0      963 2023-10-19 09:46:28.000000 sandbox_func-0.1.6/sandbox_func/model/SandboxProjManager.py
--rw-rw-rw-   0        0        0      206 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/model/SandboxRepo.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.554657 sandbox_func-0.1.6/sandbox_func/repository/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 sandbox_func-0.1.6/sandbox_func/repository/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.556657 sandbox_func-0.1.6/sandbox_func/repository/cybotron/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.584888 sandbox_func-0.1.6/sandbox_func/repository/cybotron/model/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/model/__init__.py
--rw-rw-rw-   0        0        0     2717 2023-09-19 08:34:17.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/model/metadataobj.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.646225 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/
--rw-rw-rw-   0        0        0        0 2023-09-13 06:06:11.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/__init__.py
--rw-rw-rw-   0        0        0     3106 2023-09-19 08:34:17.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/common_access.py
--rw-rw-rw-   0        0        0     1299 2023-09-19 08:34:17.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/data_accessor.py
--rw-rw-rw-   0        0        0     1326 2023-09-19 08:34:17.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/metadata_accessor.py
--rw-rw-rw-   0        0        0     1904 2023-10-16 12:09:57.000000 sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/sandbox_accessor.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.714339 sandbox_func-0.1.6/sandbox_func/request/
--rw-rw-rw-   0        0        0      113 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/request/SFCallback.py
--rw-rw-rw-   0        0        0      165 2023-09-21 10:54:33.000000 sandbox_func-0.1.6/sandbox_func/request/SFEventRequest.py
--rw-rw-rw-   0        0        0      214 2023-09-21 10:54:18.000000 sandbox_func-0.1.6/sandbox_func/request/SFExtRequest.py
--rw-rw-rw-   0        0        0      169 2023-09-22 08:17:31.000000 sandbox_func-0.1.6/sandbox_func/request/SFRequest.py
--rw-rw-rw-   0        0        0      250 2023-09-22 03:32:34.000000 sandbox_func-0.1.6/sandbox_func/request/SFResponse.py
--rw-rw-rw-   0        0        0      650 2023-09-27 02:57:51.000000 sandbox_func-0.1.6/sandbox_func/request/SFResponseJob.py
--rw-rw-rw-   0        0        0      218 2023-10-16 12:11:51.000000 sandbox_func-0.1.6/sandbox_func/request/SFWebRequest.py
--rw-rw-rw-   0        0        0      166 2023-09-13 07:02:10.000000 sandbox_func-0.1.6/sandbox_func/request/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.775099 sandbox_func-0.1.6/sandbox_func/service/
--rw-rw-rw-   0        0        0     1284 2023-09-28 03:15:15.000000 sandbox_func-0.1.6/sandbox_func/service/SandboxCallbackService.py
--rw-rw-rw-   0        0        0     1161 2023-10-17 06:37:05.000000 sandbox_func-0.1.6/sandbox_func/service/SandboxFuncService.py
--rw-rw-rw-   0        0        0     2611 2023-10-16 12:18:17.000000 sandbox_func-0.1.6/sandbox_func/service/SandboxFuncServiceForTencent.py
--rw-rw-rw-   0        0        0        0 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/service/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.792679 sandbox_func-0.1.6/sandbox_func/service/cybotron/
--rw-rw-rw-   0        0        0        0 2023-09-14 08:54:30.000000 sandbox_func-0.1.6/sandbox_func/service/cybotron/__init__.py
--rw-rw-rw-   0        0        0     1221 2023-10-19 10:01:40.000000 sandbox_func-0.1.6/sandbox_func/service/cybotron/log_accessor.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.827732 sandbox_func-0.1.6/sandbox_func/web/
--rw-rw-rw-   0        0        0      381 2023-09-21 01:33:45.000000 sandbox_func-0.1.6/sandbox_func/web/SandboxFuncServer.py
--rw-rw-rw-   0        0        0       66 2023-09-13 06:52:03.000000 sandbox_func-0.1.6/sandbox_func/web/__init__.py
--rw-rw-rw-   0        0        0     4072 2023-10-19 09:48:47.000000 sandbox_func-0.1.6/sandbox_func/web/sandbox_app.py
-drwxrwxrwx   0        0        0        0 2023-10-23 07:39:17.242442 sandbox_func-0.1.6/sandbox_func.egg-info/
--rw-rw-rw-   0        0        0       83 2023-10-23 07:39:17.000000 sandbox_func-0.1.6/sandbox_func.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-10-23 07:39:17.000000 sandbox_func-0.1.6/sandbox_func.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-23 07:39:17.000000 sandbox_func-0.1.6/sandbox_func.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-10-23 07:39:17.000000 sandbox_func-0.1.6/sandbox_func.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-10-23 07:39:17.000000 sandbox_func-0.1.6/sandbox_func.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-10-23 07:39:17.831222 sandbox_func-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      201 2023-10-23 07:39:04.000000 sandbox_func-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/PKG-INFO
+-rw-rw----   0 root         (0) root         (0)       26 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/README.md
+-rw-rw----   0 root         (0) root         (0)     1130 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.607938 sandbox_func-0.4.13/sandbox_func/
+-rw-rw----   0 root         (0) root         (0)      294 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/__init__.py
+-rw-rw----   0 root         (0) root         (0)      164 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.607938 sandbox_func-0.4.13/sandbox_func/common/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.607938 sandbox_func-0.4.13/sandbox_func/common/config/
+-rw-rw----   0 root         (0) root         (0)     1522 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/BaseURLConfig.py
+-rw-rw----   0 root         (0) root         (0)      724 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/BusinessURLConfig.py
+-rw-rw----   0 root         (0) root         (0)      257 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/ConfigModel.py
+-rw-rw----   0 root         (0) root         (0)      104 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/LogConfig.py
+-rw-rw----   0 root         (0) root         (0)     4492 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/LoginConfig.py
+-rw-rw----   0 root         (0) root         (0)       76 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/PubilcConfig.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.607938 sandbox_func-0.4.13/sandbox_func/common/file/
+-rw-rw----   0 root         (0) root         (0)     1933 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/file/LTFileManager.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/file/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.611938 sandbox_func-0.4.13/sandbox_func/common/lang/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/__init__.py
+-rw-rw----   0 root         (0) root         (0)     3207 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/async_requests.py
+-rw-rw----   0 root         (0) root         (0)     2599 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/dictclass.py
+-rw-rw----   0 root         (0) root         (0)      230 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/logger_setting.py
+-rw-rw----   0 root         (0) root         (0)      459 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/moduleutil.py
+-rw-rw----   0 root         (0) root         (0)     1430 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/singleton.py
+-rw-rw----   0 root         (0) root         (0)      694 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/lang/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.611938 sandbox_func-0.4.13/sandbox_func/common/local/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/local/__init__.py
+-rw-rw----   0 root         (0) root         (0)      733 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/local/clientinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.611938 sandbox_func-0.4.13/sandbox_func/common/log/
+-rw-rw----   0 root         (0) root         (0)     2479 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/log/AwLogger.py
+-rw-rw----   0 root         (0) root         (0)      421 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/log/LogManager.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/log/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.611938 sandbox_func-0.4.13/sandbox_func/common/request/
+-rw-rw----   0 root         (0) root         (0)     2463 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/request/CybotronClient.py
+-rw-rw----   0 root         (0) root         (0)      835 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/request/CybotronSyncClient.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.615938 sandbox_func-0.4.13/sandbox_func/common/util/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/util/__init__.py
+-rw-rw----   0 root         (0) root         (0)      218 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/util/data_transfer_util.py
+-rw-rw----   0 root         (0) root         (0)     9782 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/util/dateutil.py
+-rw-rw----   0 root         (0) root         (0)      732 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/common/util/pathutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.615938 sandbox_func-0.4.13/sandbox_func/model/
+-rw-rw----   0 root         (0) root         (0)      291 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/SandboxApp.py
+-rw-rw----   0 root         (0) root         (0)      181 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/SandboxFunc.py
+-rw-rw----   0 root         (0) root         (0)      718 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/SandboxFuncManager.py
+-rw-rw----   0 root         (0) root         (0)     1575 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/SandboxProjManager.py
+-rw-rw----   0 root         (0) root         (0)      199 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/SandboxRepo.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.615938 sandbox_func-0.4.13/sandbox_func/repository/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.615938 sandbox_func-0.4.13/sandbox_func/repository/cybotron/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.615938 sandbox_func-0.4.13/sandbox_func/repository/cybotron/model/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/model/__init__.py
+-rw-rw----   0 root         (0) root         (0)      136 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/model/flowobj.py
+-rw-rw----   0 root         (0) root         (0)     2629 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/model/metadataobj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.619938 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/__init__.py
+-rw-rw----   0 root         (0) root         (0)     2609 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/common_access.py
+-rw-rw----   0 root         (0) root         (0)     1001 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/data_accessor.py
+-rw-rw----   0 root         (0) root         (0)     1027 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/metadata_accessor.py
+-rw-rw----   0 root         (0) root         (0)     4414 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/sandbox_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.619938 sandbox_func-0.4.13/sandbox_func/repository/lively_data/
+-rw-rw----   0 root         (0) root         (0)       24 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/lively_data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.619938 sandbox_func-0.4.13/sandbox_func/repository/lively_data/model/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/lively_data/model/__init__.py
+-rw-rw----   0 root         (0) root         (0)     2336 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/lively_data/model/metadataobj.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.619938 sandbox_func-0.4.13/sandbox_func/repository/lively_data/service/
+-rw-rw----   0 root         (0) root         (0)       24 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/lively_data/service/__init__.py
+-rw-rw----   0 root         (0) root         (0)     3203 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/repository/lively_data/service/livelytable_access.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.619938 sandbox_func-0.4.13/sandbox_func/request/
+-rw-rw----   0 root         (0) root         (0)      107 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFCallback.py
+-rw-rw----   0 root         (0) root         (0)      158 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFEventRequest.py
+-rw-rw----   0 root         (0) root         (0)      204 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFExtRequest.py
+-rw-rw----   0 root         (0) root         (0)      238 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFRequest.py
+-rw-rw----   0 root         (0) root         (0)      299 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFResponse.py
+-rw-rw----   0 root         (0) root         (0)     1306 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFResponseJob.py
+-rw-rw----   0 root         (0) root         (0)      208 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/SFWebRequest.py
+-rw-rw----   0 root         (0) root         (0)      163 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/sandbox_func/service/
+-rw-rw----   0 root         (0) root         (0)     1566 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/SandboxCallbackService.py
+-rw-rw----   0 root         (0) root         (0)     2066 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/SandboxFuncService.py
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/sandbox_func/service/cybotron/
+-rw-rw----   0 root         (0) root         (0)        0 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/cybotron/__init__.py
+-rw-rw----   0 root         (0) root         (0)      763 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/cybotron/log_accessor.py
+-rw-rw----   0 root         (0) root         (0)     1302 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/service/cybotron/service_call.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/sandbox_func/web/
+-rw-rw----   0 root         (0) root         (0)      403 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/web/SandboxFuncServer.py
+-rw-rw----   0 root         (0) root         (0)       65 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/web/__init__.py
+-rw-rw----   0 root         (0) root         (0)     4314 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/sandbox_func/web/sandbox_app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:27:33.607938 sandbox_func-0.4.13/sandbox_func.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      118 2024-05-22 02:27:33.000000 sandbox_func-0.4.13/sandbox_func.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3091 2024-05-22 02:27:33.000000 sandbox_func-0.4.13/sandbox_func.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 02:27:33.000000 sandbox_func-0.4.13/sandbox_func.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-22 02:27:33.000000 sandbox_func-0.4.13/sandbox_func.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 02:27:33.000000 sandbox_func-0.4.13/sandbox_func.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 02:27:33.623938 sandbox_func-0.4.13/setup.cfg
+-rw-rw----   0 root         (0) root         (0)      242 2024-05-22 02:25:03.000000 sandbox_func-0.4.13/setup.py
```

### Comparing `sandbox_func-0.1.6/sandbox_func/common/lang/async_requests.py` & `sandbox_func-0.4.13/sandbox_func/common/lang/async_requests.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,66 @@
-import logging
-import typing
-from asyncio import Timeout
-
-import httpx
-from httpx import Response, Request
-from httpx._client import UseClientDefault, USE_CLIENT_DEFAULT
-from httpx._types import URLTypes, RequestContent, RequestData, RequestFiles, QueryParamTypes, HeaderTypes, CookieTypes, \
-    TimeoutTypes, RequestExtensions, ProxiesTypes, VerifyTypes
-
-logger = logging.getLogger(__name__)
-logging.getLogger("httpx").setLevel(logging.WARNING)
-
-
-class AsyncRequests:
-    def __init__(self, base_url=None, proxies: typing.Optional[ProxiesTypes] = None, verify: VerifyTypes = False):
-        self.base_url = base_url
-        self.proxies = proxies
-        self.verify = verify
-
-    async def send(self, request: Request, retry=1) -> Response:
-        for retry_count in range(retry):
-            try:
-                async with httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies,
-                                             verify=self.verify) as client:
-                    return await client.send(request)
-            except Exception as e:
-                logger.error(f'{str(request.url)}请求接口失败，尝试第{retry_count + 1}次')
-                logger.error(f"请求参数：{str(request.json)}")
-                if retry_count == retry - 1:
-                    raise e
-                else:
-                    logger.error(e)
-
-    async def request(self, url, data, retry=1) -> Response:
-        for retry_count in range(retry):
-            try:
-                async with httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies,
-                                             verify=self.verify, timeout=None) as client:
-                    return await client.request('POST', url, data=data)
-            except Exception as e:
-                logger.error(e)
-                logger.error(f'{url}请求接口失败，尝试第{retry_count + 1}次')
-                logger.error(f"请求参数：{str(data)}")
-                if retry_count == retry - 1:
-                    raise e
-                else:
-                    logger.error(e)
-
-    def build_request(self,
-                      method: str,
-                      url: URLTypes,
-                      *,
-                      content: typing.Optional[RequestContent] = None,
-                      data: typing.Optional[RequestData] = None,
-                      files: typing.Optional[RequestFiles] = None,
-                      json: typing.Optional[typing.Any] = None,
-                      params: typing.Optional[QueryParamTypes] = None,
-                      headers: typing.Optional[HeaderTypes] = None,
-                      cookies: typing.Optional[CookieTypes] = None,
-                      timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
-                      extensions: typing.Optional[RequestExtensions] = None):
-        timeout = float(timeout) if isinstance(timeout, int) else timeout
-        return httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies, verify=self.verify).build_request(
-            method, url, content=content, data=data, files=files, json=json, params=params, headers=headers,
-            cookies=cookies,
-            timeout=timeout, extensions=extensions)
+import logging
+import typing
+
+import httpx
+from httpx import Response, Request
+from httpx._client import UseClientDefault, USE_CLIENT_DEFAULT
+from httpx._types import URLTypes, RequestContent, RequestData, RequestFiles, QueryParamTypes, HeaderTypes, CookieTypes, \
+    TimeoutTypes, RequestExtensions, ProxiesTypes, VerifyTypes
+
+logger = logging.getLogger(__name__)
+logging.getLogger("httpx").setLevel(logging.WARNING)
+
+
+class AsyncRequests:
+    def __init__(self, base_url=None, proxies: typing.Optional[ProxiesTypes] = None, verify: VerifyTypes = False):
+        self.base_url = base_url
+        self.proxies = proxies
+        self.verify = verify
+
+    async def send(self, request: Request, retry=1) -> Response:
+        for retry_count in range(retry):
+            try:
+                async with httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies,
+                                             verify=self.verify) as client:
+                    return await client.send(request)
+            except Exception as e:
+                logger.error(f'{str(request.url)}请求接口失败，尝试第{retry_count + 1}次')
+                # logger.error(f"请求参数：{str(request.json)}")
+                if retry_count == retry - 1:
+                    raise e
+                else:
+                    logger.error(e)
+
+    async def request(self, url, data, retry=1) -> Response:
+        for retry_count in range(retry):
+            try:
+                async with httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies,
+                                             verify=self.verify, timeout=None) as client:
+                    return await client.request('POST', url, data=data)
+            except Exception as e:
+                logger.error(e)
+                logger.error(f'{url}请求接口失败，尝试第{retry_count + 1}次')
+                logger.error(f"请求参数：{str(data)}")
+                if retry_count == retry - 1:
+                    raise e
+                else:
+                    logger.error(e)
+
+    def build_request(self,
+                      method: str,
+                      url: URLTypes,
+                      *,
+                      content: typing.Optional[RequestContent] = None,
+                      data: typing.Optional[RequestData] = None,
+                      files: typing.Optional[RequestFiles] = None,
+                      json: typing.Optional[typing.Any] = None,
+                      params: typing.Optional[QueryParamTypes] = None,
+                      headers: typing.Optional[HeaderTypes] = None,
+                      cookies: typing.Optional[CookieTypes] = None,
+                      timeout: typing.Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
+                      extensions: typing.Optional[RequestExtensions] = None):
+        timeout = float(timeout) if isinstance(timeout, int) else timeout
+        return httpx.AsyncClient(base_url=self.base_url, proxies=self.proxies, verify=self.verify).build_request(
+            method, url, content=content, data=data, files=files, json=json, params=params, headers=headers,
+            cookies=cookies,
+            timeout=timeout, extensions=extensions)
```

### Comparing `sandbox_func-0.1.6/sandbox_func/common/lang/singleton.py` & `sandbox_func-0.4.13/sandbox_func/common/lang/singleton.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from threading import Lock
-
-
-class SingletonMeta(type):
-    """
-    This is a thread-safe implementation of Singleton.
-    """
-
-    _instances = {}
-
-    _lock: Lock = Lock()
-    """
-    We now have a lock object that will be used to synchronize threads during
-    first access to the Singleton.
-    """
-
-    def __call__(cls, *args, **kwargs):
-        """
-        Possible changes to the value of the `__init__` argument do not affect
-        the returned instance.
-        """
-        # Now, imagine that the program has just been launched. Since there's no
-        # Singleton instance yet, multiple threads can simultaneously pass the
-        # previous conditional and reach this point almost at the same time. The
-        # first of them will acquire lock and will proceed further, while the
-        # rest will wait here.
-        with cls._lock:
-            # The first thread to acquire the lock, reaches this conditional,
-            # goes inside and creates the Singleton instance. Once it leaves the
-            # lock block, a thread that might have been waiting for the lock
-            # release may then enter this section. But since the Singleton field
-            # is already initialized, the thread won't create a new object.
-            if cls not in cls._instances:
-                instance = super().__call__(*args, **kwargs)
-                cls._instances[cls] = instance
-        return cls._instances[cls]
+from threading import Lock
+
+
+class SingletonMeta(type):
+    """
+    This is a thread-safe implementation of Singleton.
+    """
+
+    _instances = {}
+
+    _lock: Lock = Lock()
+    """
+    We now have a lock object that will be used to synchronize threads during
+    first access to the Singleton.
+    """
+
+    def __call__(cls, *args, **kwargs):
+        """
+        Possible changes to the value of the `__init__` argument do not affect
+        the returned instance.
+        """
+        # Now, imagine that the program has just been launched. Since there's no
+        # Singleton instance yet, multiple threads can simultaneously pass the
+        # previous conditional and reach this point almost at the same time. The
+        # first of them will acquire lock and will proceed further, while the
+        # rest will wait here.
+        with cls._lock:
+            # The first thread to acquire the lock, reaches this conditional,
+            # goes inside and creates the Singleton instance. Once it leaves the
+            # lock block, a thread that might have been waiting for the lock
+            # release may then enter this section. But since the Singleton field
+            # is already initialized, the thread won't create a new object.
+            if cls not in cls._instances:
+                instance = super().__call__(*args, **kwargs)
+                cls._instances[cls] = instance
+        return cls._instances[cls]
```

### Comparing `sandbox_func-0.1.6/sandbox_func/common/log/AwLogger.py` & `sandbox_func-0.4.13/sandbox_func/common/log/AwLogger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,85 +1,88 @@
-import logging
-from collections import UserDict
-from enum import Enum
-from pathlib import Path
-
-from sandbox_func.common.config.LogConfig import DEFAULT_LOG_FILE
-from sandbox_func.common.config.LoginConfig import DefaultLoginConfig
-from sandbox_func.service.cybotron.log_accessor import LogAccessor
-
-
-class LogLevel(Enum):
-    DEBUG = 'DEBUG'
-    INFO = 'INFO'
-    WARNING = 'WARNING'
-    ERROR = 'ERROR'
-    CRITICAL = 'CRITICAL'
-
-
-class Log(UserDict):
-    trace_id: str
-    app_id: str
-    app_version_id: str
-    func_id: str
-    creator: str
-    level: str
-    message: str
-
-
-class AwLogger:
-    """autowork log warapper"""
-
-    cybotron_access_info: dict = {}
-
-    @classmethod
-    def getLogger(cls, filename: str, level: LogLevel = LogLevel.INFO):
-        logger = logging.getLogger(filename)
-        if level is None:
-            logger.setLevel('INFO')
-        else:
-            logger.setLevel(level.value)
-
-        logfile = Path().home().joinpath(DEFAULT_LOG_FILE)
-        logdir = logfile.parent
-        if not logdir.exists():
-            logdir.mkdir(parents=True, exist_ok=True)
-
-        formatter = logging.Formatter(
-            fmt="%(asctime)s.%(msecs)03d [%(levelname)s] %(filename)s:%(lineno)s - %(""message)s",
-            datefmt='%Y-%m-%d %H:%M:%S')
-        file_handler = logging.FileHandler(logfile)
-        file_handler.setFormatter(formatter)
-        logger.addHandler(file_handler)
-
-        # 如果是debug模式，信息入库metabase.mb_sandbox_debug_log
-        if DefaultLoginConfig.get_debug():
-            db_handler = DBLogHandler()
-            db_handler.setFormatter(formatter)
-            logger.addHandler(db_handler)
-
-        return logger
-
-
-class DBLogHandler(logging.Handler):
-    def __init__(self):
-        super().__init__()
-
-    def emit(self, record: logging.LogRecord):
-        msg = record.getMessage()
-        trace_id = msg.split('-')[0]
-        real_msg = msg.split('-')[1]
-        cybotron_access_info = AwLogger.cybotron_access_info[trace_id]
-        log = Log(
-            trace_id=cybotron_access_info['trace_id'],
-            app_id=cybotron_access_info['app_id'],
-            app_version_id=cybotron_access_info['app_version_id'],
-            func_id=cybotron_access_info['func_id'],
-            creator=cybotron_access_info['creator'],
-            level=record.levelno,
-            message=real_msg
-        )
-
-        try:
-            LogAccessor.send_log(log.data)
-        except Exception as e:
-            print(e)
+import logging
+import os
+from collections import UserDict
+from enum import Enum
+
+from sandbox_func.common.util.pathutil import get_log_file_path
+from sandbox_func.common.config.LoginConfig import DefaultLoginConfig
+from sandbox_func.service.cybotron.log_accessor import LogAccessor
+
+
+class LogLevel(Enum):
+    DEBUG = 'DEBUG'
+    INFO = 'INFO'
+    WARNING = 'WARNING'
+    ERROR = 'ERROR'
+    CRITICAL = 'CRITICAL'
+
+
+class Log(UserDict):
+    trace_id: str
+    app_id: str
+    app_version_id: str
+    func_id: str
+    creator: str
+    level: str
+    message: str
+
+
+class LogRecord(UserDict):
+    trace_id: str
+
+
+class AwLogger:
+    """autowork log warapper"""
+
+    cybotron_access_info: dict = {}
+
+    @classmethod
+    def getLogger(cls, filename: str, level: LogLevel = LogLevel.INFO):
+        logger = logging.getLogger(filename)
+        if level is None:
+            logger.setLevel('INFO')
+        else:
+            logger.setLevel(level.value)
+
+        logfile = get_log_file_path()
+        os.makedirs(os.path.dirname(logfile), exist_ok=True)
+        formatter = logging.Formatter(
+            fmt="%(asctime)s.%(msecs)03d [%(levelname)s] %(filename)s:%(lineno)s - %(""message)s",
+            datefmt='%Y-%m-%d %H:%M:%S')
+        file_handler = logging.FileHandler(logfile)
+        file_handler.setFormatter(formatter)
+        logger.addHandler(file_handler)
+
+        # 如果是debug模式，信息入库metabase.mb_sandbox_debug_log
+        if DefaultLoginConfig.get_debug():
+            db_handler = DBLogHandler()
+            db_handler.setFormatter(formatter)
+            logger.addHandler(db_handler)
+
+        return logger
+
+    # @staticmethod
+    # def init_logger(trace_id: str, info: dict):
+    #     AwLogger.cybotron_access_info[trace_id] = Log(trace_id=trace_id, **info)
+    #     return LogRecord(trace_id=trace_id)
+
+
+class DBLogHandler(logging.Handler):
+    def __init__(self):
+        super().__init__()
+
+    def emit(self, record: logging.LogRecord):
+        msg = record.getMessage()
+        trace_id = record.args.get("trace_id")
+        cybotron_access_info = AwLogger.cybotron_access_info[trace_id]
+        log = Log(
+            trace_id=cybotron_access_info['trace_id'],
+            app_id=cybotron_access_info['app_id'],
+            func_id=cybotron_access_info['func_id'],
+            level=record.levelno,
+            message=msg
+        )
+
+        try:
+            LogAccessor.send_log(log.data)
+        except Exception as e:
+            print(e)
```

### Comparing `sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/common_access.py` & `sandbox_func-0.4.13/sandbox_func/repository/cybotron/service/common_access.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,86 +1,77 @@
-# -*- coding: utf-8 -*-
-import logging
-from typing import Dict
-
-from sandbox_func.common.lang.async_requests import AsyncRequests
-from sandbox_func.repository.cybotron.model.metadataobj import *
-
-logger = logging.getLogger(__name__)
-
-
-class CommonAccess:
-
-    def __init__(self):
-        self.URL = None
-        self.X_API_KEY = None
-        self.client = AsyncRequests("")
-
-    async def create(self, req: CreateRequest) -> CreateResponse:
-        """
-        单条创建接口
-        """
-        result = await self.get_response(req, "create")
-        return CreateResponse(lastId=result["lastId"])
-
-    async def update(self, req: UpdateRequest) -> UpdateResponse:
-        """
-        单条修改接口
-        """
-        result = await self.get_response(req, "update")
-        return UpdateResponse(count=result["count"], lastId=result["lastId"])
-
-    async def delete(self, req: DeleteRequest) -> DeleteResponse:
-        """
-        单条删除接口
-        """
-        result = await self.get_response(req, "delete")
-        return DeleteResponse(count=result["count"])
-
-    async def bulkCreate(self, req: BulkCreateRequest) -> BulkCreateResponse:
-        """
-        批量创建接口
-        """
-        result = await self.get_response(req, "bulkCreate")
-        return BulkCreateResponse(count=result["count"])
-
-    async def bulkUpdate(self, req: BulkUpdateRequest) -> BulkUpdateResponse:
-        """
-        批量修改接口
-        """
-        result = await self.get_response(req, "bulkUpdate")
-        return BulkUpdateResponse(count=result["count"])
-
-    async def bulkDelete(self, req: BulkDeleteRequest) -> BulkDeleteResponse:
-        """
-        批量删除接口
-        """
-        result = await self.get_response(req=req, method="bulkDelete")
-        return BulkDeleteResponse(count=result["count"])
-
-    async def get_response(self, req, method: str = "", re_method: str = "post") -> Dict:
-        """
-        请求数据
-        """
-        headers = {
-            'Content-Type': 'application/json',
-            'X-API-KEY': self.X_API_KEY
-        }
-        app_code = req.appCode
-        table_code = req.tableCode
-        url = f"{self.URL}/{app_code}/{table_code}/{method}"
-        logger.info(f"url:{url}, headers：{headers}, json:{req.dict()}")
-        request = self.client.build_request(method=re_method, url=url, timeout=15, json=req.dict(), headers=headers)
-        response = await self.client.send(request)
-        response = response.json()
-        if not response.get("success"):
-            raise Exception(response.get("message"))
-        return response["result"]
-
-    async def get_response_json(self, url: str = "", json: str = "", method: str = "", headers: Dict = None) -> str:
-        """
-        请求数据, 抽取公共使用
-        """
-        request = self.client.build_request(method=method, url=url, timeout=15, json=json, headers=headers)
-        response = await self.client.send(request)
-        response = response.json()
-        return response
+# -*- coding: utf-8 -*-
+import logging
+from typing import Dict
+
+from sandbox_func.common.request.CybotronSyncClient import CybotronClient
+from sandbox_func.repository.cybotron.model.metadataobj import *
+
+logger = logging.getLogger(__name__)
+
+
+class CommonAccess:
+
+    def __init__(self):
+        self.URL = None
+        self.client = CybotronClient()
+
+    async def create(self, req: CreateRequest) -> CreateResponse:
+        """
+        单条创建接口
+        """
+        result = await self.get_response(req, "create")
+        return CreateResponse(lastId=result["lastId"])
+
+    async def update(self, req: UpdateRequest) -> UpdateResponse:
+        """
+        单条修改接口
+        """
+        result = await self.get_response(req, "update")
+        return UpdateResponse(count=result["count"], lastId=result.get("lastId"))
+
+    async def delete(self, req: DeleteRequest) -> DeleteResponse:
+        """
+        单条删除接口
+        """
+        result = await self.get_response(req, "delete")
+        return DeleteResponse(count=result["count"])
+
+    async def bulk_create(self, req: BulkCreateRequest) -> BulkCreateResponse:
+        """
+        批量创建接口
+        """
+        result = await self.get_response(req, "bulkCreate")
+        return BulkCreateResponse(count=result["count"])
+
+    async def bulk_update(self, req: BulkUpdateRequest) -> BulkUpdateResponse:
+        """
+        批量修改接口
+        """
+        result = await self.get_response(req, "bulkUpdate")
+        return BulkUpdateResponse(count=result["count"])
+
+    async def bulk_delete(self, req: BulkDeleteRequest) -> BulkDeleteResponse:
+        """
+        批量删除接口
+        """
+        result = await self.get_response(req=req, method="bulkDelete")
+        return BulkDeleteResponse(count=result["count"])
+
+    async def get_response(self, req, method: str = "", re_method: str = "post") -> Dict:
+        """
+        请求数据
+        """
+        app_code = req.appCode
+        table_code = req.tableCode
+        url = f"{self.URL}/{app_code}/{table_code}/{method}"
+        logger.info(f"url:{url}, json:{req.dict()}")
+        response = await self.client.send(url, re_method, json=req.dict())
+        if not response.get("success"):
+            raise Exception(response.get("message"))
+        return response["result"]
+
+    async def get_response_json(self, url: str = "", json: str = "", method: str = "", headers: Dict = None) -> str:
+        """
+        请求数据, 抽取公共使用
+        """
+        response = await self.client.send(url, method, json=json)
+        return response
```

### Comparing `sandbox_func-0.1.6/sandbox_func/repository/cybotron/service/sandbox_accessor.py` & `sandbox_func-0.4.13/sandbox_func/service/SandboxFuncService.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import asyncio
-import json
-
-from sandbox_func.common.config.BaseURLConfig import BaseURLConfig
-from sandbox_func.common.config.BusinessURLConfig import BusinessURLConfig, DataTypeEnum
-from sandbox_func.common.config.LoginConfig import DefaultLoginConfig
-from sandbox_func.common.request.CybotronSyncClient import CybotronSyncClient
-from sandbox_func.repository.cybotron.model.metadataobj import GetRequest
-from sandbox_func.repository.cybotron.service.data_accessor import DataAccessor
-from sandbox_func.request import SFResponse, SFRequest
-
-
-class SandboxAccessor:
-
-    def __init__(self):
-        self.URL = BaseURLConfig.get_api_base_url(DefaultLoginConfig.get_env()) + BusinessURLConfig.get_url(
-            DataTypeEnum.SANDBOX)
-
-    def dispatchRequest(self, request: SFRequest) -> SFResponse:
-        client = CybotronSyncClient()
-        url = f"{self.URL}/{request.app_id}/{request.func_id}"
-        response = SFResponse()
-        try:
-            res = client.send(url, 'POST', json=request.input)
-            response.result = res['result']
-            result_json = json.loads(res['result'])
-            response.request_id = result_json["requestId"]
-            return response
-        except Exception as e:
-            response.error = e
-            return response
-
-    def confirmAysncRequest(self, request: SFRequest) -> SFResponse:
-        data_accessor = DataAccessor()
-        get_req = GetRequest(
-            appCode="metabase",
-            tableCode="mb_async_job",
-            id=request.request_id
-        )
-        response = SFResponse()
-        try:
-            get_res = asyncio.run(data_accessor.get(get_req))
-            response.request_id = request.request_id
-            response.result = get_res.data
-            return response
-        except Exception as e:
-            response.error = e
-            return response
+import logging
+
+from sandbox_func.common.lang.singleton import SingletonMeta
+from sandbox_func.model.SandboxFuncManager import SandboxFuncManager
+
+from sandbox_func.repository.cybotron.service.sandbox_accessor import SandboxAccessor
+from sandbox_func.request.SFRequest import SFRequest
+from sandbox_func.request.SFResponse import SFResponse
+from sandbox_func.request.SFResponseJob import SFResponseJob
+
+logger = logging.getLogger(__name__)
+
+
+class SandboxFuncService(metaclass=SingletonMeta):
+    def __init__(self):
+        pass
+
+    @staticmethod
+    async def create_async_job(app_id, request_id, status, progress) -> str:
+        return await SandboxAccessor.create_async_job(app_id, request_id, status, progress)
+
+    @staticmethod
+    async def update_async_job(request_id, status, progress, loading_message=None, success_message=None,
+                               error_code=None, error_message=None):
+        return await SandboxAccessor.update_async_job(request_id, status, progress, loading_message,
+                                                      success_message, error_code, error_message)
+
+    @staticmethod
+    async def call(request: SFRequest) -> SFResponse:
+        response = SFResponse()
+        job = SFResponseJob()
+        job.set_request_id(request.request_id)
+        job.set_job_id(request.job_id)
+        response.request_id = request.request_id
+        response.job = job
+        try:
+            func = SandboxFuncManager.get_func(request.class_file, request.method_name)
+            if not func or not func.run:
+                logger.error(f'沙盒函数缓存里找不到class_file={request.class_file}, method_name={request.method_name}')
+                raise Exception(f"class_file={request.class_file}, method_name={request.method_name} not found")
+            result = await func.run(request, response)
+            if result:
+                response.result = result
+            return response
+        except Exception as e:
+            logger.exception(e)
+            response.error = str(e)
+            return response
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sandbox_func-0.1.6/sandbox_func/service/SandboxCallbackService.py` & `sandbox_func-0.4.13/sandbox_func/service/SandboxCallbackService.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-import json
-
-import httpx
-
-from sandbox_func.request import SFResponse, SFRequest
-from sandbox_func.common.log.AwLogger import AwLogger
-
-logger = AwLogger.getLogger(__name__)
-
-
-class SandboxCallbackService:
-    """异步任务回调处理，如果request里包含hook信息，则进行回调"""
-
-    def __init__(self, request: SFRequest, response: SFResponse):
-        self.req = request
-        self.res = response
-
-    @staticmethod
-    def callback(req: SFRequest, res: SFResponse):
-        hook = req.input.get('hook')
-        if hook is not None:
-            callback_url = dict(hook).get('url')
-            data = {"result": res.result, "input": req.input, "progress": res.job.job_progress,
-                    "success": res.job.job_success, "error": res.job.job_error}
-            logger.info(f'异步请求回调， 回调地址：{callback_url}， 回调参数：{data}')
-            client = httpx.Client()
-            try:
-                client.post(callback_url,
-                            json=json.dumps(data, ensure_ascii=False, default=lambda dictclass: dictclass.data))
-            except Exception as e:
-                logger.error(f"回调处理报错，回调地址：{callback_url}, 回到参数：{data}, 报错信息：{e}")
+import logging
+
+from sandbox_func.request import SFResponse, SFRequest
+from sandbox_func.common.lang.async_requests import AsyncRequests
+
+# logger = AwLogger.getLogger(__name__)
+logger = logging.getLogger(__name__)
+
+
+class SandboxCallbackService:
+    """异步任务回调处理，如果request里包含hook信息，则进行回调"""
+
+    def __init__(self, request: SFRequest, response: SFResponse):
+        self.req = request
+        self.res = response
+
+    @staticmethod
+    async def callback(req: SFRequest, res: SFResponse):
+        logger.info(f"req:{req}")
+        hook = req.get('hook')
+        if hook:
+            client = AsyncRequests()
+            callback_url = hook.get('url')  # type:str
+            params = hook['params'].dict() if hook.get('params') else hook.get('params')  # 透传参数
+            req_input = req['input'].dict() if req.get('input') else req.get('input')
+            data = {"result": res.result, "input": req_input, "params": params,
+                    "progress": res.job.job_progress, "success": res.job.job_success, "error": res.job.job_error}
+            logger.info(f'异步请求回调， 回调地址：{callback_url}， 回调js参数：{data}')
+            try:
+                req = client.build_request('post', url=callback_url, json=data)
+                res = await client.send(req)
+                logger.info(f"回调成功，返回值:{res}")
+            except Exception as e:
+                logger.error(f"回调处理报错，回调地址：{callback_url}, 回调参数：{data}, 报错信息：{e}")
```

### Comparing `sandbox_func-0.1.6/sandbox_func.egg-info/SOURCES.txt` & `sandbox_func-0.4.13/sandbox_func.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,57 +10,68 @@
 sandbox_func.egg-info/top_level.txt
 sandbox_func/common/__init__.py
 sandbox_func/common/config/BaseURLConfig.py
 sandbox_func/common/config/BusinessURLConfig.py
 sandbox_func/common/config/ConfigModel.py
 sandbox_func/common/config/LogConfig.py
 sandbox_func/common/config/LoginConfig.py
-sandbox_func/common/config/TencentConfig.py
+sandbox_func/common/config/PubilcConfig.py
 sandbox_func/common/config/__init__.py
-sandbox_func/common/file/CosFileManager.py
+sandbox_func/common/file/LTFileManager.py
 sandbox_func/common/file/__init__.py
 sandbox_func/common/lang/__init__.py
 sandbox_func/common/lang/async_requests.py
 sandbox_func/common/lang/dictclass.py
 sandbox_func/common/lang/logger_setting.py
 sandbox_func/common/lang/moduleutil.py
 sandbox_func/common/lang/singleton.py
+sandbox_func/common/lang/sync.py
 sandbox_func/common/local/__init__.py
 sandbox_func/common/local/clientinfo.py
 sandbox_func/common/log/AwLogger.py
 sandbox_func/common/log/LogManager.py
 sandbox_func/common/log/__init__.py
 sandbox_func/common/request/CybotronClient.py
 sandbox_func/common/request/CybotronSyncClient.py
 sandbox_func/common/request/__init__.py
+sandbox_func/common/util/__init__.py
+sandbox_func/common/util/data_transfer_util.py
+sandbox_func/common/util/dateutil.py
+sandbox_func/common/util/pathutil.py
 sandbox_func/model/SandboxApp.py
 sandbox_func/model/SandboxFunc.py
 sandbox_func/model/SandboxFuncManager.py
 sandbox_func/model/SandboxProjManager.py
 sandbox_func/model/SandboxRepo.py
 sandbox_func/model/__init__.py
 sandbox_func/repository/__init__.py
 sandbox_func/repository/cybotron/__init__.py
 sandbox_func/repository/cybotron/model/__init__.py
+sandbox_func/repository/cybotron/model/flowobj.py
 sandbox_func/repository/cybotron/model/metadataobj.py
 sandbox_func/repository/cybotron/service/__init__.py
 sandbox_func/repository/cybotron/service/common_access.py
 sandbox_func/repository/cybotron/service/data_accessor.py
 sandbox_func/repository/cybotron/service/metadata_accessor.py
 sandbox_func/repository/cybotron/service/sandbox_accessor.py
+sandbox_func/repository/lively_data/__init__.py
+sandbox_func/repository/lively_data/model/__init__.py
+sandbox_func/repository/lively_data/model/metadataobj.py
+sandbox_func/repository/lively_data/service/__init__.py
+sandbox_func/repository/lively_data/service/livelytable_access.py
 sandbox_func/request/SFCallback.py
 sandbox_func/request/SFEventRequest.py
 sandbox_func/request/SFExtRequest.py
 sandbox_func/request/SFRequest.py
 sandbox_func/request/SFResponse.py
 sandbox_func/request/SFResponseJob.py
 sandbox_func/request/SFWebRequest.py
 sandbox_func/request/__init__.py
 sandbox_func/service/SandboxCallbackService.py
 sandbox_func/service/SandboxFuncService.py
-sandbox_func/service/SandboxFuncServiceForTencent.py
 sandbox_func/service/__init__.py
 sandbox_func/service/cybotron/__init__.py
 sandbox_func/service/cybotron/log_accessor.py
+sandbox_func/service/cybotron/service_call.py
 sandbox_func/web/SandboxFuncServer.py
 sandbox_func/web/__init__.py
 sandbox_func/web/sandbox_app.py
```

