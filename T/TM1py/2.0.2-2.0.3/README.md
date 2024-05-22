# Comparing `tmp/tm1py-2.0.2.tar.gz` & `tmp/tm1py-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TM1py-2.0.2.tar", last modified: Mon Feb 19 15:06:53 2024, max compression
+gzip compressed data, was "TM1py-2.0.3.tar", last modified: Wed May 22 12:27:37 2024, max compression
```

## Comparing `tm1py-2.0.2.tar` & `tm1py-2.0.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.749865 TM1py-2.0.2/
--rw-rw-rw-   0        0        0     1103 2023-02-20 21:26:26.000000 TM1py-2.0.2/LICENSE
--rw-rw-rw-   0        0        0     4462 2024-02-19 15:06:53.749865 TM1py-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3522 2024-01-27 18:06:29.000000 TM1py-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.627842 TM1py-2.0.2/TM1py/
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.634841 TM1py-2.0.2/TM1py/Exceptions/
--rw-rw-rw-   0        0        0     3984 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Exceptions/Exceptions.py
--rw-rw-rw-   0        0        0      207 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Exceptions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.674534 TM1py-2.0.2/TM1py/Objects/
--rw-rw-rw-   0        0        0     5869 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Annotation.py
--rw-rw-rw-   0        0        0     6868 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Application.py
--rw-rw-rw-   0        0        0     3781 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Axis.py
--rw-rw-rw-   0        0        0     5094 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Objects/Chore.py
--rw-rw-rw-   0        0        0     2049 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/ChoreFrequency.py
--rw-rw-rw-   0        0        0     3385 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/ChoreStartTime.py
--rw-rw-rw-   0        0        0     2809 2024-01-11 12:56:37.000000 TM1py-2.0.2/TM1py/Objects/ChoreTask.py
--rw-rw-rw-   0        0        0     3494 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Cube.py
--rw-rw-rw-   0        0        0     4420 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Dimension.py
--rw-rw-rw-   0        0        0     2945 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Element.py
--rw-rw-rw-   0        0        0     2403 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/ElementAttribute.py
--rw-rw-rw-   0        0        0     2313 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Git.py
--rw-rw-rw-   0        0        0      685 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/GitCommit.py
--rw-rw-rw-   0        0        0     2905 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/GitPlan.py
--rw-rw-rw-   0        0        0    17697 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Objects/GitProject.py
--rw-rw-rw-   0        0        0      743 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/GitRemote.py
--rw-rw-rw-   0        0        0    13499 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Objects/Hierarchy.py
--rw-rw-rw-   0        0        0     2926 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/MDXView.py
--rw-rw-rw-   0        0        0    12608 2024-01-15 13:50:27.000000 TM1py-2.0.2/TM1py/Objects/NativeView.py
--rw-rw-rw-   0        0        0    19980 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Objects/Process.py
--rw-rw-rw-   0        0        0     7579 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/ProcessDebugBreakpoint.py
--rw-rw-rw-   0        0        0     2800 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Rules.py
--rw-rw-rw-   0        0        0     2644 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/Sandbox.py
--rw-rw-rw-   0        0        0     1434 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Objects/Server.py
--rw-rw-rw-   0        0        0    10274 2024-01-15 13:50:27.000000 TM1py-2.0.2/TM1py/Objects/Subset.py
--rw-rw-rw-   0        0        0      608 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/TM1Object.py
--rw-rw-rw-   0        0        0     5801 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Objects/User.py
--rw-rw-rw-   0        0        0      812 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/View.py
--rw-rw-rw-   0        0        0     1158 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Objects/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.729764 TM1py-2.0.2/TM1py/Services/
--rw-rw-rw-   0        0        0     3630 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/AnnotationService.py
--rw-rw-rw-   0        0        0    15000 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/ApplicationService.py
--rw-rw-rw-   0        0        0     4105 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/AuditLogService.py
--rw-rw-rw-   0        0        0   236089 2024-01-31 14:09:33.000000 TM1py-2.0.2/TM1py/Services/CellService.py
--rw-rw-rw-   0        0        0    11428 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/ChoreService.py
--rw-rw-rw-   0        0        0     2548 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/ConfigurationService.py
--rw-rw-rw-   0        0        0    15558 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Services/CubeService.py
--rw-rw-rw-   0        0        0     8758 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/DimensionService.py
--rw-rw-rw-   0        0        0    59374 2024-01-31 12:10:55.000000 TM1py-2.0.2/TM1py/Services/ElementService.py
--rw-rw-rw-   0        0        0     5607 2024-01-31 12:11:06.000000 TM1py-2.0.2/TM1py/Services/FileService.py
--rw-rw-rw-   0        0        0    10344 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/GitService.py
--rw-rw-rw-   0        0        0    31052 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Services/HierarchyService.py
--rw-rw-rw-   0        0        0     1661 2024-01-27 18:08:52.000000 TM1py-2.0.2/TM1py/Services/JobService.py
--rw-rw-rw-   0        0        0     3495 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/LoggerService.py
--rw-rw-rw-   0        0        0    10308 2024-01-27 18:09:49.000000 TM1py-2.0.2/TM1py/Services/ManageService.py
--rw-rw-rw-   0        0        0     7111 2024-02-15 16:02:02.000000 TM1py-2.0.2/TM1py/Services/MessageLogService.py
--rw-rw-rw-   0        0        0     3236 2024-01-27 18:09:49.000000 TM1py-2.0.2/TM1py/Services/MonitoringService.py
--rw-rw-rw-   0        0        0     2928 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Services/ObjectService.py
--rw-rw-rw-   0        0        0     3052 2023-04-21 17:21:23.000000 TM1py-2.0.2/TM1py/Services/PowerBiService.py
--rw-rw-rw-   0        0        0    31558 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Services/ProcessService.py
--rw-rw-rw-   0        0        0    47718 2024-02-19 15:00:29.000000 TM1py-2.0.2/TM1py/Services/RestService.py
--rw-rw-rw-   0        0        0     4848 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/SandboxService.py
--rw-rw-rw-   0        0        0     9480 2024-01-23 12:11:03.000000 TM1py-2.0.2/TM1py/Services/SecurityService.py
--rw-rw-rw-   0        0        0    11151 2024-02-15 16:02:02.000000 TM1py-2.0.2/TM1py/Services/ServerService.py
--rw-rw-rw-   0        0        0     2373 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/SessionService.py
--rw-rw-rw-   0        0        0     8550 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/SubsetService.py
--rw-rw-rw-   0        0        0     6480 2024-01-27 18:09:14.000000 TM1py-2.0.2/TM1py/Services/TM1Service.py
--rw-rw-rw-   0        0        0     2499 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/ThreadService.py
--rw-rw-rw-   0        0        0     4525 2024-01-27 17:50:50.000000 TM1py-2.0.2/TM1py/Services/TransactionLogService.py
--rw-rw-rw-   0        0        0     2465 2024-01-27 18:09:49.000000 TM1py-2.0.2/TM1py/Services/UserService.py
--rw-rw-rw-   0        0        0    13548 2024-01-17 17:54:05.000000 TM1py-2.0.2/TM1py/Services/ViewService.py
--rw-rw-rw-   0        0        0     1730 2024-01-27 18:09:49.000000 TM1py-2.0.2/TM1py/Services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.733765 TM1py-2.0.2/TM1py/Utils/
--rw-rw-rw-   0        0        0    10265 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Utils/MDXUtils.py
--rw-rw-rw-   0        0        0    52843 2024-02-01 20:32:06.000000 TM1py-2.0.2/TM1py/Utils/Utils.py
--rw-rw-rw-   0        0        0       69 2023-02-20 21:26:26.000000 TM1py-2.0.2/TM1py/Utils/__init__.py
--rw-rw-rw-   0        0        0     3559 2024-02-19 15:06:38.000000 TM1py-2.0.2/TM1py/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-19 15:06:53.631842 TM1py-2.0.2/TM1py.egg-info/
--rw-rw-rw-   0        0        0     4462 2024-02-19 15:06:53.000000 TM1py-2.0.2/TM1py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4083 2024-02-19 15:06:53.000000 TM1py-2.0.2/TM1py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-19 15:06:53.000000 TM1py-2.0.2/TM1py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-02-19 15:06:53.000000 TM1py-2.0.2/TM1py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       64 2024-02-19 15:06:53.000000 TM1py-2.0.2/TM1py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       91 2023-06-07 17:36:08.000000 TM1py-2.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-19 15:06:53.750796 TM1py-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1596 2024-02-19 15:06:38.000000 TM1py-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.958560 TM1py-2.0.3/
+-rw-rw-rw-   0        0        0     1103 2023-02-20 21:26:26.000000 TM1py-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4942 2024-05-22 12:27:37.957561 TM1py-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3981 2024-05-06 09:17:22.000000 TM1py-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.795505 TM1py-2.0.3/TM1py/
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.809032 TM1py-2.0.3/TM1py/Exceptions/
+-rw-rw-rw-   0        0        0     3984 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Exceptions/Exceptions.py
+-rw-rw-rw-   0        0        0      207 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Exceptions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.862140 TM1py-2.0.3/TM1py/Objects/
+-rw-rw-rw-   0        0        0     5869 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Annotation.py
+-rw-rw-rw-   0        0        0     6868 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Application.py
+-rw-rw-rw-   0        0        0     3781 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Axis.py
+-rw-rw-rw-   0        0        0     5094 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Objects/Chore.py
+-rw-rw-rw-   0        0        0     2049 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/ChoreFrequency.py
+-rw-rw-rw-   0        0        0     3385 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/ChoreStartTime.py
+-rw-rw-rw-   0        0        0     2809 2024-01-11 12:56:37.000000 TM1py-2.0.3/TM1py/Objects/ChoreTask.py
+-rw-rw-rw-   0        0        0     3494 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/Objects/Cube.py
+-rw-rw-rw-   0        0        0     4420 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Dimension.py
+-rw-rw-rw-   0        0        0     2945 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Element.py
+-rw-rw-rw-   0        0        0     2403 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/ElementAttribute.py
+-rw-rw-rw-   0        0        0     2313 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Git.py
+-rw-rw-rw-   0        0        0      685 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/GitCommit.py
+-rw-rw-rw-   0        0        0     2905 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/GitPlan.py
+-rw-rw-rw-   0        0        0    17697 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Objects/GitProject.py
+-rw-rw-rw-   0        0        0      743 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/GitRemote.py
+-rw-rw-rw-   0        0        0    13499 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Objects/Hierarchy.py
+-rw-rw-rw-   0        0        0     2926 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/MDXView.py
+-rw-rw-rw-   0        0        0    12608 2024-01-15 13:50:27.000000 TM1py-2.0.3/TM1py/Objects/NativeView.py
+-rw-rw-rw-   0        0        0    19994 2024-04-03 13:46:01.000000 TM1py-2.0.3/TM1py/Objects/Process.py
+-rw-rw-rw-   0        0        0     7579 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/ProcessDebugBreakpoint.py
+-rw-rw-rw-   0        0        0     3001 2024-05-22 12:12:40.000000 TM1py-2.0.3/TM1py/Objects/Rules.py
+-rw-rw-rw-   0        0        0     2644 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/Sandbox.py
+-rw-rw-rw-   0        0        0     1434 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Objects/Server.py
+-rw-rw-rw-   0        0        0    10274 2024-01-15 13:50:27.000000 TM1py-2.0.3/TM1py/Objects/Subset.py
+-rw-rw-rw-   0        0        0      608 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/TM1Object.py
+-rw-rw-rw-   0        0        0     5801 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Objects/User.py
+-rw-rw-rw-   0        0        0      812 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/View.py
+-rw-rw-rw-   0        0        0     1158 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Objects/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.925568 TM1py-2.0.3/TM1py/Services/
+-rw-rw-rw-   0        0        0     3630 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/AnnotationService.py
+-rw-rw-rw-   0        0        0    16461 2024-04-03 16:11:35.000000 TM1py-2.0.3/TM1py/Services/ApplicationService.py
+-rw-rw-rw-   0        0        0     4116 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/Services/AuditLogService.py
+-rw-rw-rw-   0        0        0   236827 2024-05-14 12:17:14.000000 TM1py-2.0.3/TM1py/Services/CellService.py
+-rw-rw-rw-   0        0        0    11428 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/ChoreService.py
+-rw-rw-rw-   0        0        0     2548 2024-01-27 17:50:50.000000 TM1py-2.0.3/TM1py/Services/ConfigurationService.py
+-rw-rw-rw-   0        0        0    17415 2024-05-22 12:12:40.000000 TM1py-2.0.3/TM1py/Services/CubeService.py
+-rw-rw-rw-   0        0        0     8758 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/DimensionService.py
+-rw-rw-rw-   0        0        0    60308 2024-05-06 10:22:05.000000 TM1py-2.0.3/TM1py/Services/ElementService.py
+-rw-rw-rw-   0        0        0     8514 2024-05-14 12:17:11.000000 TM1py-2.0.3/TM1py/Services/FileService.py
+-rw-rw-rw-   0        0        0    10344 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/GitService.py
+-rw-rw-rw-   0        0        0    31052 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Services/HierarchyService.py
+-rw-rw-rw-   0        0        0     1661 2024-01-27 18:08:52.000000 TM1py-2.0.3/TM1py/Services/JobService.py
+-rw-rw-rw-   0        0        0     3495 2024-01-27 17:50:50.000000 TM1py-2.0.3/TM1py/Services/LoggerService.py
+-rw-rw-rw-   0        0        0    10308 2024-01-27 18:09:49.000000 TM1py-2.0.3/TM1py/Services/ManageService.py
+-rw-rw-rw-   0        0        0     6915 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/Services/MessageLogService.py
+-rw-rw-rw-   0        0        0     3236 2024-01-27 18:09:49.000000 TM1py-2.0.3/TM1py/Services/MonitoringService.py
+-rw-rw-rw-   0        0        0     2928 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Services/ObjectService.py
+-rw-rw-rw-   0        0        0     3052 2023-04-21 17:21:23.000000 TM1py-2.0.3/TM1py/Services/PowerBiService.py
+-rw-rw-rw-   0        0        0    31558 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Services/ProcessService.py
+-rw-rw-rw-   0        0        0    47625 2024-05-14 12:17:11.000000 TM1py-2.0.3/TM1py/Services/RestService.py
+-rw-rw-rw-   0        0        0     4848 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/SandboxService.py
+-rw-rw-rw-   0        0        0     9480 2024-01-23 12:11:03.000000 TM1py-2.0.3/TM1py/Services/SecurityService.py
+-rw-rw-rw-   0        0        0    11151 2024-02-15 16:02:02.000000 TM1py-2.0.3/TM1py/Services/ServerService.py
+-rw-rw-rw-   0        0        0     2373 2024-01-27 17:50:50.000000 TM1py-2.0.3/TM1py/Services/SessionService.py
+-rw-rw-rw-   0        0        0     8550 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/SubsetService.py
+-rw-rw-rw-   0        0        0     6379 2024-04-03 16:11:35.000000 TM1py-2.0.3/TM1py/Services/TM1Service.py
+-rw-rw-rw-   0        0        0     2586 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/Services/ThreadService.py
+-rw-rw-rw-   0        0        0     4325 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/Services/TransactionLogService.py
+-rw-rw-rw-   0        0        0     2465 2024-01-27 18:09:49.000000 TM1py-2.0.3/TM1py/Services/UserService.py
+-rw-rw-rw-   0        0        0    13548 2024-01-17 17:54:05.000000 TM1py-2.0.3/TM1py/Services/ViewService.py
+-rw-rw-rw-   0        0        0     1730 2024-01-27 18:09:49.000000 TM1py-2.0.3/TM1py/Services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.931567 TM1py-2.0.3/TM1py/Utils/
+-rw-rw-rw-   0        0        0    10265 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Utils/MDXUtils.py
+-rw-rw-rw-   0        0        0    53177 2024-05-14 12:16:55.000000 TM1py-2.0.3/TM1py/Utils/Utils.py
+-rw-rw-rw-   0        0        0       69 2023-02-20 21:26:26.000000 TM1py-2.0.3/TM1py/Utils/__init__.py
+-rw-rw-rw-   0        0        0     3609 2024-05-06 09:17:22.000000 TM1py-2.0.3/TM1py/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:27:37.805041 TM1py-2.0.3/TM1py.egg-info/
+-rw-rw-rw-   0        0        0     4942 2024-05-22 12:27:37.000000 TM1py-2.0.3/TM1py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4083 2024-05-22 12:27:37.000000 TM1py-2.0.3/TM1py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:27:37.000000 TM1py-2.0.3/TM1py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      143 2024-05-22 12:27:37.000000 TM1py-2.0.3/TM1py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       64 2024-05-22 12:27:37.000000 TM1py-2.0.3/TM1py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-06-07 17:36:08.000000 TM1py-2.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:27:37.958560 TM1py-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2024-05-14 12:17:14.000000 TM1py-2.0.3/setup.py
```

### Comparing `TM1py-2.0.2/LICENSE` & `TM1py-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/PKG-INFO` & `TM1py-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TM1py
-Version: 2.0.2
+Version: 2.0.3
 Summary: A python module for TM1.
 Home-page: https://github.com/cubewise-code/tm1py
-Download-URL: https://github.com/Cubewise-code/TM1py/tarball/2.0.2
+Download-URL: https://github.com/Cubewise-code/TM1py/tarball/2.0.3
 Author: Marius Wirtz
 Author-email: MWirtz@cubewise.com
 License: MIT
 Keywords: TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
+Provides-Extra: dev
 License-File: LICENSE
 
 
 <img src="https://s3-ap-southeast-2.amazonaws.com/downloads.cubewise.com/web_assets/CubewiseLogos/TM1py-logo.png" style="width: 70%; height: 70%;text-align: center"/>
 
 
 TM1py is the python package for IBM Planning Analytics (TM1).
@@ -50,15 +51,16 @@
 
 Requirements
 =======================
 
 - python (3.7 or higher)
 - requests
 - requests_negotiate_sspi
-- TM1 11 
+- TM1 11, TM1 12
+- keyring
 
 
 Optional Requirements
 =======================
 
 - pandas
 
@@ -69,52 +71,74 @@
 
     pip install tm1py
     
 > with pandas
 
     pip install "tm1py[pandas]"
     
-    
+> keyring
+
+    pip install keyring
+
 Usage
 =======================
 
 > TM1 11 on-premise
 
 ``` python
 from TM1py.Services import TM1Service
 
 with TM1Service(address='localhost', port=8001, user='admin', password='apple', ssl=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 > TM1 11 on IBM cloud
 
 ``` python
 with TM1Service(
         base_url='https://mycompany.planning-analytics.ibmcloud.com/tm1/api/tm1/',
         user="non_interactive_user",
         namespace="LDAP",
         password="U3lSn5QLwoQZY2",
         ssl=True,
         verify=True,
         async_requests_mode=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
+```
+
+
+> TM1 12 MCSP
+
+``` python
+from TM1py import TM1Service
+
+params = {
+    "base_url": "https://us-east-1.planninganalytics.saas.ibm.com/api/<TenantId>/v0/tm1/<DatabaseName>/",
+    "user": "apikey",
+    "password": "<TheActualApiKey>",
+    "async_requests_mode": True,
+    "ssl": True,
+    "verify": True
+}
+
+with TM1Service(**params) as tm1:
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 PAaaS
 
 ``` python
 with TM1Service(
         address="us-east-2.aws.planninganalytics.ibm.com",
         api_key="AB4VfG7T8wPM-912uFKeYG5PGh0XbS80MVBAt7SEG6xn",
         iam_url="https://iam.cloud.ibm.com/identity/token",
         tenant="YA9A2T8BS2ZU",
         database="Database") as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 on-premise & Cloud Pak For Data
 
 ``` python
 with TM1Service(
@@ -122,15 +146,15 @@
         instance="your instance name",
         database="your database name",
         application_client_id="client id",
         application_client_secret="client secret",
         user="admin",
         ssl=True) as tm1:
 
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 
 
 Documentation
 =======================
```

### Comparing `TM1py-2.0.2/README.md` & `TM1py-2.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 Requirements
 =======================
 
 - python (3.7 or higher)
 - requests
 - requests_negotiate_sspi
-- TM1 11 
+- TM1 11, TM1 12
+- keyring
 
 
 Optional Requirements
 =======================
 
 - pandas
 
@@ -44,52 +45,74 @@
 
     pip install tm1py
     
 > with pandas
 
     pip install "tm1py[pandas]"
     
-    
+> keyring
+
+    pip install keyring
+
 Usage
 =======================
 
 > TM1 11 on-premise
 
 ``` python
 from TM1py.Services import TM1Service
 
 with TM1Service(address='localhost', port=8001, user='admin', password='apple', ssl=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 > TM1 11 on IBM cloud
 
 ``` python
 with TM1Service(
         base_url='https://mycompany.planning-analytics.ibmcloud.com/tm1/api/tm1/',
         user="non_interactive_user",
         namespace="LDAP",
         password="U3lSn5QLwoQZY2",
         ssl=True,
         verify=True,
         async_requests_mode=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
+```
+
+
+> TM1 12 MCSP
+
+``` python
+from TM1py import TM1Service
+
+params = {
+    "base_url": "https://us-east-1.planninganalytics.saas.ibm.com/api/<TenantId>/v0/tm1/<DatabaseName>/",
+    "user": "apikey",
+    "password": "<TheActualApiKey>",
+    "async_requests_mode": True,
+    "ssl": True,
+    "verify": True
+}
+
+with TM1Service(**params) as tm1:
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 PAaaS
 
 ``` python
 with TM1Service(
         address="us-east-2.aws.planninganalytics.ibm.com",
         api_key="AB4VfG7T8wPM-912uFKeYG5PGh0XbS80MVBAt7SEG6xn",
         iam_url="https://iam.cloud.ibm.com/identity/token",
         tenant="YA9A2T8BS2ZU",
         database="Database") as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 on-premise & Cloud Pak For Data
 
 ``` python
 with TM1Service(
@@ -97,15 +120,15 @@
         instance="your instance name",
         database="your database name",
         application_client_id="client id",
         application_client_secret="client secret",
         user="admin",
         ssl=True) as tm1:
 
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 
 
 Documentation
 =======================
```

### Comparing `TM1py-2.0.2/TM1py/Exceptions/Exceptions.py` & `TM1py-2.0.3/TM1py/Exceptions/Exceptions.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Annotation.py` & `TM1py-2.0.3/TM1py/Objects/Annotation.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Application.py` & `TM1py-2.0.3/TM1py/Objects/Application.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Axis.py` & `TM1py-2.0.3/TM1py/Objects/Axis.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Chore.py` & `TM1py-2.0.3/TM1py/Objects/Chore.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/ChoreFrequency.py` & `TM1py-2.0.3/TM1py/Objects/ChoreFrequency.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/ChoreStartTime.py` & `TM1py-2.0.3/TM1py/Objects/ChoreStartTime.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/ChoreTask.py` & `TM1py-2.0.3/TM1py/Objects/ChoreTask.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Cube.py` & `TM1py-2.0.3/TM1py/Objects/Cube.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Dimension.py` & `TM1py-2.0.3/TM1py/Objects/Dimension.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Element.py` & `TM1py-2.0.3/TM1py/Objects/Element.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/ElementAttribute.py` & `TM1py-2.0.3/TM1py/Objects/ElementAttribute.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Git.py` & `TM1py-2.0.3/TM1py/Objects/Git.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/GitCommit.py` & `TM1py-2.0.3/TM1py/Objects/GitCommit.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/GitPlan.py` & `TM1py-2.0.3/TM1py/Objects/GitPlan.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/GitProject.py` & `TM1py-2.0.3/TM1py/Objects/GitProject.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/GitRemote.py` & `TM1py-2.0.3/TM1py/Objects/GitRemote.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Hierarchy.py` & `TM1py-2.0.3/TM1py/Objects/Hierarchy.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/MDXView.py` & `TM1py-2.0.3/TM1py/Objects/MDXView.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/NativeView.py` & `TM1py-2.0.3/TM1py/Objects/NativeView.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Process.py` & `TM1py-2.0.3/TM1py/Objects/Process.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,18 +133,18 @@
     def from_dict(cls, process_as_dict: Dict) -> 'Process':
         """
         :param process_as_dict: Dictionary, process as dictionary
         :return: an instance of this class
         """
         return cls(name=process_as_dict['Name'],
                    has_security_access=process_as_dict['HasSecurityAccess'],
-                   ui_data=process_as_dict['UIData'],
+                   ui_data=process_as_dict.get('UIData',''),
                    parameters=process_as_dict['Parameters'],
                    variables=process_as_dict['Variables'],
-                   variables_ui_data=process_as_dict['VariablesUIData'],
+                   variables_ui_data=process_as_dict.get('VariablesUIData',''),
                    prolog_procedure=process_as_dict['PrologProcedure'],
                    metadata_procedure=process_as_dict['MetadataProcedure'],
                    data_procedure=process_as_dict['DataProcedure'],
                    epilog_procedure=process_as_dict['EpilogProcedure'],
                    datasource_type=process_as_dict['DataSource'].get('Type', ''),
                    datasource_ascii_decimal_separator=process_as_dict['DataSource'].get('asciiDecimalSeparator', ''),
                    datasource_ascii_delimiter_char=process_as_dict['DataSource'].get('asciiDelimiterChar', ''),
```

### Comparing `TM1py-2.0.2/TM1py/Objects/ProcessDebugBreakpoint.py` & `TM1py-2.0.3/TM1py/Objects/ProcessDebugBreakpoint.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Rules.py` & `TM1py-2.0.3/TM1py/Objects/Rules.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
-from typing import List
+import json
+from typing import List, Dict
 
 from TM1py.Objects.TM1Object import TM1Object
 
 
 class Rules(TM1Object):
     """
         Abstraction of Rules on a cube.
@@ -76,14 +77,22 @@
         if 'FEEDERS' in self._rules_analytics:
             # has feeders declaration
             feeders = self.rules_analytics[self._rules_analytics.index('FEEDERS'):]
             # has at least one actual feeder statements
             return len(feeders) > 1
         return False
 
+    @property
+    def body(self) -> str:
+        return json.dumps(self.body_as_dict)
+
+    @property
+    def body_as_dict(self) -> Dict:
+        return {'Rules': self.text}
+
     def __len__(self):
         return len(self.rules_analytics)
 
     # iterate through actual rule statments without linebreaks. Ignore comments.
     def __iter__(self):
         return iter(self.rules_analytics)
```

### Comparing `TM1py-2.0.2/TM1py/Objects/Sandbox.py` & `TM1py-2.0.3/TM1py/Objects/Sandbox.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Server.py` & `TM1py-2.0.3/TM1py/Objects/Server.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/Subset.py` & `TM1py-2.0.3/TM1py/Objects/Subset.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/TM1Object.py` & `TM1py-2.0.3/TM1py/Objects/TM1Object.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/User.py` & `TM1py-2.0.3/TM1py/Objects/User.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/View.py` & `TM1py-2.0.3/TM1py/Objects/View.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Objects/__init__.py` & `TM1py-2.0.3/TM1py/Objects/__init__.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/AnnotationService.py` & `TM1py-2.0.3/TM1py/Services/AnnotationService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ApplicationService.py` & `TM1py-2.0.3/TM1py/Services/ApplicationService.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,32 @@
     def get_all_private_root_names(self, **kwargs):
 
         url = "/Contents('Applications')/PrivateContents"
         response = self._rest.GET(url, **kwargs)
         applications = list(application['Name'] for application in response.json()['value'])
         return applications
 
+    def get_names(self, path: str, private: bool = False, **kwargs):
+        """ Retrieve Planning Analytics Application names in given path
 
+        :param path: path with forward slashes
+        :param private: boolean
+        :return: list of application names
+        """
+        contents = 'PrivateContents' if private else 'Contents'
+        mid = ""
+        if path.strip() != '':
+            mid = "".join([format_url("/Contents('{}')", element) for element in path.split('/')])
+        base_url = "/api/v1/Contents('Applications')" + mid + "/" + contents
+
+        response = self._rest.GET(url=base_url, **kwargs)
+        applications = list(application['Name'] for application in response.json()['value'])
+        
+        return applications
+    
     def get(self, path: str, application_type: Union[str, ApplicationTypes], name: str, private: bool = False,
             **kwargs) -> Application:
         """ Retrieve Planning Analytics Application
 
         :param path: path with forward slashes
         :param application_type: str or ApplicationType from Enum
         :param name:
@@ -248,14 +265,27 @@
                 **kwargs)
         else:
             url = "/Contents('Applications')" + mid + "/" + contents
             response = self._rest.POST(url, application.body, **kwargs)
 
         return response
 
+    def update_or_create(self, application: Union[Application, DocumentApplication], private: bool = False, **kwargs) -> Response:
+        """ Update or create Planning Analytics application
+
+        :param application: instance of Application
+        :param private: boolean
+        :return: Response
+        """
+        if self.exists(path=application.path, application_type=application.application_type, name=application.name, private=private,**kwargs):
+            response = self.update(application=application, private=private, **kwargs)
+        else:
+            response = self.create(application=application, private=private, **kwargs)
+        return response
+    
     def update_or_create_document_from_file(self, path: str, name: str,
                                             path_to_file: str, private: bool = False, **kwargs) -> Response:
         """Update or create application from file
 
         :param path: application path on server, i.e. 'Finance/Reports'
         :param name: name of the application on server, i.e. 'Flash.xlsx'
         :param path_to_file: full local file path of file, i.e. 'C:\\Users\\User\\Flash.xslx'
```

### Comparing `TM1py-2.0.2/TM1py/Services/AuditLogService.py` & `TM1py-2.0.3/TM1py/Services/AuditLogService.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 
 
 from TM1py.Services.ObjectService import ObjectService
 from TM1py.Services.RestService import RestService
 from TM1py.Utils import verify_version, deprecated_in_version, odata_track_changes_header, require_data_admin, \
     format_url, \
-    require_version, require_ops_admin
+    require_version, require_ops_admin, utc_localize_time
 from TM1py.Services.ConfigurationService import ConfigurationService
 
 
 class AuditLogService(ObjectService):
 
     def __init__(self, rest: RestService):
         super().__init__(rest)
@@ -70,27 +70,27 @@
                     "ObjectType eq '{}'", object_type))
             if object_name:
                 log_filters.append(format_url(
                     "ObjectName eq '{}'", object_name))
             if since:
                 # If since doesn't have tz information, UTC is assumed
                 if not since.tzinfo:
-                    since = self.utc_localize_time(since)
+                    since = utc_localize_time(since)
                 log_filters.append(format_url(
                     "TimeStamp ge {}", since.strftime("%Y-%m-%dT%H:%M:%SZ")))
             if until:
                 # If until doesn't have tz information, UTC is assumed
                 if not until.tzinfo:
-                    until = self.utc_localize_time(until)
+                    until = utc_localize_time(until)
                 log_filters.append(format_url(
                     "TimeStamp le {}", until.strftime("%Y-%m-%dT%H:%M:%SZ")))
             url += "&$filter={}".format(" and ".join(log_filters))
         # top limit
         if top:
             url += '&$top={}'.format(top)
         response = self._rest.GET(url, **kwargs)
         return response.json()['value']
 
     @require_ops_admin
     def activate(self):
         config = {'Administration': {'AuditLog': {'Enable': True}}}
-        self.configuration.update_static(config)
+        self.configuration.update_static(config)
```

### Comparing `TM1py-2.0.2/TM1py/Services/CellService.py` & `TM1py-2.0.3/TM1py/Services/CellService.py`

 * *Files 0% similar despite different names*

```diff
@@ -1415,18 +1415,20 @@
         ViewExtractSkipCalcsSet('{cube}', '{view_name}', {'1' if skip_consolidated_cells else '0'});
         ViewExtractSkipRuleValuesSet('{cube}', '{view_name}', {'1' if skip_rule_derived_cells else '0'});
         ViewExtractSkipZeroesSet('{cube}', '{view_name}', {'1' if skip_zeros else '0'});
         DatasourceAsciiDelimiter='{value_separator}';
         DatasourceAsciiQuoteCharacter='{quote_character}';
         nRecord=0;
         """
+
         process.prolog_procedure = prolog_procedure
 
         # ignore some variable in file and output variables ordered by their ordinal e.g. v2,v4,v5,v11
-        comma_sep_variables = ",".join(sorted(set(variables) - set(skip_variables), key=lambda v: int(v[1:])))
+        output_variables = sorted(set(variables) - set(skip_variables), key=lambda v: int(v[1:]))
+        comma_sep_variables = ",".join(output_variables)
         data_procedure_pre = f"""
         IF (nRecord = 0);
           SetOutputCharacterSet('{file_name}','TM1CS_UTF8');
         ENDIF;
         nRecord = nRecord + 1;
         """
         if header_line:
@@ -1454,14 +1456,31 @@
         if verify_version(required_version="12", version=self.version):
             data_procedure_pre += f"""
             IF (ISUNDEFINEDCELLVALUE(NVALUE,'{cube}') = 1);
               SVALUE ='0';
             ENDIF;
             """
 
+        for variable in output_variables + ["SVALUE"]:
+            data_procedure_pre += f"""
+            sTextToEscape = {variable};
+            sEscapeChar = '"';
+            IF (SCAN(sEscapeChar, sTextToEscape) > 0);
+                nPos = LONG ( sTextToEscape );
+                WHILE ( nPos > 0);
+                    sChar = Subst(sTextToEscape, nPos, 1);
+                    IF ( sChar @= sEscapeChar );
+                      sTextToEscape = INSRT(sEscapeChar, sTextToEscape, nPos);
+                    ENDIF;  
+                    nPos = nPos - 1;
+                END;
+                {variable} = sTextToEscape;
+            ENDIF;
+            """
+
         data_procedure = f"""
         TextOutput('{file_name}',{comma_sep_variables},SVALUE);
         """
         process.data_procedure = data_procedure_pre + data_procedure
 
         return process
 
@@ -1751,15 +1770,15 @@
 
         changeset = kwargs.get("changeset")
 
         cellset_id = self.create_cellset(mdx=mdx, sandbox_name=sandbox_name, **kwargs)
         if increment:
             current_values = self.extract_cellset_values(cellset_id, use_compact_json=True, delete_cellset=False,
                                                          **kwargs)
-            values = (x + (y or None) for x, y in zip(values, current_values))
+            values = (float(x) + float(y or 0) for x, y in zip(values, current_values))
 
         self.update_cellset(cellset_id=cellset_id, values=values, sandbox_name=sandbox_name, **kwargs)
         return changeset
 
     @tidy_cellset
     def update_cellset(self, cellset_id: str, values: Iterable, sandbox_name: str = None, changeset: str = None,
                        **kwargs) -> Response:
@@ -2956,15 +2975,15 @@
                                         member_properties=list(set(member_properties or []) | {"Name"}),
                                         top=top,
                                         skip=skip,
                                         delete_cellset=True,
                                         sandbox_name=sandbox_name,
                                         use_compact_json=use_compact_json,
                                         **kwargs)
-        return Utils.build_ui_arrays_from_cellset(raw_cellset_as_dict=data, value_precision=value_precision)
+        return Utils.build_ui_arrays_from_cellset(raw_cellset_as_dict=data, value_precision=value_precision, top=top)
 
     def execute_view_ui_array(
             self,
             cube_name: str,
             view_name: str,
             private: bool = False,
             elem_properties: Iterable[str] = None,
```

### Comparing `TM1py-2.0.2/TM1py/Services/ChoreService.py` & `TM1py-2.0.3/TM1py/Services/ChoreService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ConfigurationService.py` & `TM1py-2.0.3/TM1py/Services/ConfigurationService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/CubeService.py` & `TM1py-2.0.3/TM1py/Services/CubeService.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 import json
 import random
-from typing import List, Iterable, Dict
+from typing import List, Iterable, Dict, Union
 
 from requests import Response
 
 from TM1py.Objects.Cube import Cube
+from TM1py.Objects.Rules import Rules
 from TM1py.Services.CellService import CellService
 from TM1py.Services.ObjectService import ObjectService
 from TM1py.Services.RestService import RestService
 from TM1py.Services.ViewService import ViewService
 from TM1py.Utils import format_url, require_version, require_data_admin, case_and_space_insensitive_equals
 
 
@@ -131,14 +132,32 @@
         """
         url = format_url("/Cubes('{}')/tm1.CheckRules", cube_name)
 
         response = self._rest.POST(url, **kwargs)
         errors = response.json()["value"]
         return errors
 
+    def update_or_create_rules(self, cube_name: str, rules: Union[str, Rules], **kwargs) -> Response:
+        """ Update if exists, else create rules from a TM1 Server cube
+
+        :param cube_name: name of a cube
+        :param rules: rules content
+        :return: response
+        """
+        if isinstance(rules, str):
+            rules = Rules(rules=rules)
+        if isinstance(rules, Rules):
+            pass
+        else:
+            raise ValueError('rules must be type str or Rules')
+
+        url = format_url("/Cubes('{}')", cube_name)
+        response = self._rest.PATCH(url=url, data=rules.body, **kwargs)
+        return response
+
     @require_data_admin
     def delete(self, cube_name: str, **kwargs) -> Response:
         """ Delete a cube in TM1
 
         :param cube_name:
         :return: response
         """
@@ -374,7 +393,35 @@
         for dimension in dimensions:
             hierarchy = dimension_service.get(dimension).default_hierarchy
             element = random.choice(list((hierarchy.elements.keys())))
             if unique_names:
                 element = '[{}].[{}]'.format(dimension, element)
             elements.append(element)
         return elements
+
+    @require_data_admin
+    @require_version(version="11.8.20")
+    def get_vmm(self, cube_name: str):
+        url = format_url("/Cubes('{}')?$select=ViewStorageMaxMemory", cube_name)
+        response = self._rest.GET(url)
+        return response.json()["ViewStorageMaxMemory"]
+
+    @require_data_admin
+    @require_version(version="11.8.20")
+    def set_vmm(self, cube_name: str, vmm: int):
+        url = format_url("/Cubes('{}')", cube_name)
+        payload = {"ViewStorageMaxMemory": vmm}
+        response = self._rest.PATCH(url=url, data=json.dumps(payload))
+
+    @require_data_admin
+    @require_version(version="11.8.20")
+    def get_vmt(self, cube_name: str):
+        url = format_url("/Cubes('{}')?$select=ViewStorageMinTime", cube_name)
+        response = self._rest.GET(url)
+        return response.json()["ViewStorageMinTime"]
+
+    @require_data_admin
+    @require_version(version="11.8.20")
+    def set_vmt(self, cube_name: str, vmt: int):
+        url = format_url("/Cubes('{}')", cube_name)
+        payload = {"ViewStorageMinTime": vmt}
+        response = self._rest.PATCH(url=url, data=json.dumps(payload))
```

### Comparing `TM1py-2.0.2/TM1py/Services/DimensionService.py` & `TM1py-2.0.3/TM1py/Services/DimensionService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ElementService.py` & `TM1py-2.0.3/TM1py/Services/ElementService.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 import json
 from enum import Enum
 from io import StringIO
 from typing import List, Union, Iterable, Optional, Dict, Tuple
 
-import numpy as np
 
 from TM1py import Subset, Process
 
 try:
     import pandas as pd
+    import numpy as np
 
     _has_pandas = True
 except ImportError:
     _has_pandas = False
 
 from mdxpy import MdxHierarchySet, Member, MdxLevelExpression
 from requests import Response
@@ -162,14 +162,15 @@
     @require_pandas
     def get_elements_dataframe(self, dimension_name: str = None, hierarchy_name: str = None,
                                elements: Union[str, Iterable[str]] = None,
                                skip_consolidations: bool = True, attributes: Iterable[str] = None,
                                attribute_column_prefix: str = "", skip_parents: bool = False,
                                level_names: List[str] = None, parent_attribute: str = None,
                                skip_weights: bool = False, use_blob: bool = False, allow_empty_alias: bool = True,
+                               attribute_suffix: bool = False, element_type_column: str = 'Type',
                                **kwargs) -> 'pd.DataFrame':
         """
 
         :param dimension_name: Name of the dimension. Can be derived from elements MDX
         :param hierarchy_name: Name of the hierarchy in the dimension.Can be derived from elements MDX
         :param elements: Selection of members. Iterable or valid MDX string
         :param skip_consolidations: Boolean flag to skip consolidations
@@ -177,14 +178,16 @@
         :param attribute_column_prefix: string to prefix attribute colums to avoid name conflicts
         :param level_names: List of labels for parent columns. If None use level names from TM1.
         :param skip_parents: Boolean Flag to skip parent columns.
         :param parent_attribute: Attribute to be displayed in parent columns. If None, parent name is used.
         :param skip_weights: include weight columns
         :param use_blob: Up to 40% better performance and lower memory footprint in any case. Requires admin permissions
         :param allow_empty_alias: False if empty alias values should be substituted with element names instead
+        :param attribute_suffix: True if attribute columns should have ':a', ':s' or ':n' suffix
+        :param element_type_column: The column name in the df which specifies which element is which type.
         :return: pandas DataFrame
         """
 
         if isinstance(elements, str) and not all([dimension_name, hierarchy_name]):
             record = self.execute_set_mdx(
                 mdx=elements,
                 top_records=1,
@@ -226,15 +229,15 @@
 
         df = pd.DataFrame(
             data=[(member["Name"], element_types[member["Name"]])
                   for member
                   in members
                   if member["Name"] in element_types],
             dtype=str,
-            columns=[dimension_name, 'Type'])
+            columns=[dimension_name, element_type_column])
 
         calculated_members_definition = list()
         calculated_members_selection = list()
         levels_dict = {}
         if not skip_parents:
             levels = self.get_levels_count(dimension_name, hierarchy_name)
 
@@ -343,15 +346,16 @@
                 skip_zeros=False,
                 skip_consolidated_cells=False,
                 skip_rule_derived_cells=False,
                 line_separator="\r\n",
                 value_separator="~",
                 use_blob=True,
                 **kwargs)
-            df_data = pd.read_csv(StringIO(raw_csv), sep='~')
+
+            df_data = pd.read_csv(StringIO(raw_csv), sep='~', na_filter=False, dtype={0: str})
 
             # Use _group to avoid aggregation of multiple members into one df record
             # example: element A is part of multiple consolidations resulting df must have multiple records for A
             unique_values_count = df_data['}ElementAttributes_' + dimension_name].nunique()
             df_data['_group'] = (df_data.index // unique_values_count) + 1
 
             # pivot the dataframe
@@ -365,30 +369,57 @@
             # Drop the group key
             df_data = df_data.fillna("").drop(columns='_group')
 
         else:
             df_data = cell_service.execute_mdx_dataframe_shaped(mdx, **kwargs)
 
         if levels_dict:
-            # rename level names to conform sto strandard levels "1" -> "level0001"
+            # rename level names to conform sto standard levels "1" -> "level001"
             df_data.rename(columns=levels_dict, inplace=True)
 
         # format weights
         # Find columns with certain names
         cols_to_format = [col for col in df_data.columns if '_Weight' in col]
 
         # format the columns
         df_data[cols_to_format] = df_data[cols_to_format].apply(pd.to_numeric)
         df_data[cols_to_format] = df_data[cols_to_format].applymap(lambda x: '{:.6f}'.format(x))
 
-        # override columns. hierarchy name with dimension and prefix attributes
+        # override colum types
+        element_attributes = self.get_element_attributes(dimension_name, hierarchy_name)
+        attribute_column_types = {
+            ea.name: 'float' if ea.attribute_type == 'Numeric' else 'str'
+            for ea
+            in element_attributes
+            if ea.name in df_data.columns}
+        df_data = df_data.astype(attribute_column_types)
+
+        # substitute empty strings with element name if empty alias is not allowed
+        if not allow_empty_alias:
+            alias_attributes = [
+                ea.name
+                for ea in element_attributes
+                if ea.attribute_type == 'Alias' and ea.name in df_data.columns]
+
+            for col in alias_attributes:
+                df_data[col] = np.where(df_data[col] == '', df_data[dimension_name], df_data[col])
+
+        # override column names. hierarchy name with dimension and prefix attributes
         column_renaming = dict()
-        if attributes and attribute_column_prefix:
-            column_renaming = {attribute: str(attribute_column_prefix) + attribute for attribute in attributes}
+        if attribute_column_prefix or attribute_suffix:
+            column_renaming = {
+                ea.name: f"{attribute_column_prefix}{ea.name}" + (
+                    f":{ea.attribute_type.lower()[0]}"
+                    if attribute_suffix
+                    else "")
+                for ea
+                in element_attributes}
+
         column_renaming[hierarchy_name] = dimension_name
+
         df_data.rename(columns=column_renaming, inplace=True)
 
         # shift levels to right hand side
         if not skip_parents:
             # skip max level (= leaves)
             level_columns = level_names[1:]
 
@@ -412,22 +443,14 @@
             df_data.iloc[:, -len(level_columns):] = df_data.iloc[:, -len(level_columns):].fillna('')
             if not skip_weights:
                 df_data.iloc[:, -len(level_columns) * 2:-len(level_names)] = df_data.iloc[
                                                                              :,
                                                                              -len(level_columns) * 2:
                                                                              -len(level_names)].fillna(0)
 
-        if not allow_empty_alias:
-            # substitute empty strings with element name if empty alias is not allowed
-            alias_attributes = self.get_alias_element_attributes(dimension_name, hierarchy_name)
-            alias_attributes = list(set(alias_attributes).intersection(df_data.columns))
-
-            for col in alias_attributes:
-                df_data[col] = np.where(df_data[col] == '', df_data[dimension_name], df_data[col])
-
         return pd.merge(df, df_data, on=dimension_name).drop_duplicates()
 
     def get_edges(self, dimension_name: str, hierarchy_name: str, **kwargs) -> Dict[Tuple[str, str], int]:
         url = format_url(
             "/Dimensions('{}')/Hierarchies('{}')/Edges?select=ParentName,ComponentName,Weight",
             dimension_name,
             hierarchy_name)
```

### Comparing `TM1py-2.0.2/TM1py/Services/GitService.py` & `TM1py-2.0.3/TM1py/Services/GitService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/HierarchyService.py` & `TM1py-2.0.3/TM1py/Services/HierarchyService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/JobService.py` & `TM1py-2.0.3/TM1py/Services/JobService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/LoggerService.py` & `TM1py-2.0.3/TM1py/Services/LoggerService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ManageService.py` & `TM1py-2.0.3/TM1py/Services/ManageService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/MessageLogService.py` & `TM1py-2.0.3/TM1py/Services/MessageLogService.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import pytz
 from warnings import warn
 
 from datetime import datetime
 from typing import Dict, Iterable, Optional
 
 from TM1py.Objects.Process import Process
 from TM1py.Services.ObjectService import ObjectService
 from TM1py.Services.RestService import RestService
 from TM1py.Utils import verify_version, deprecated_in_version, odata_track_changes_header, require_ops_admin, require_data_admin, \
-    format_url, CaseAndSpaceInsensitiveDict, CaseAndSpaceInsensitiveSet
+    format_url, CaseAndSpaceInsensitiveDict, CaseAndSpaceInsensitiveSet, utc_localize_time
 
 
 class MessageLogService(ObjectService):
 
     def __init__(self, rest: RestService):
         super().__init__(rest)
         if verify_version(required_version="12.0.0", version=rest.version):
@@ -70,22 +69,22 @@
 
         if since or until or logger or level or msg_contains:
             log_filters = []
 
             if since:
                 # If since doesn't have tz information, UTC is assumed
                 if not since.tzinfo:
-                    since = self.utc_localize_time(since)
+                    since = utc_localize_time(since)
                 log_filters.append(format_url(
                     "TimeStamp ge {}", since.strftime("%Y-%m-%dT%H:%M:%SZ")))
 
             if until:
                 # If until doesn't have tz information, UTC is assumed
                 if not until.tzinfo:
-                    until = self.utc_localize_time(until)
+                    until = utc_localize_time(until)
                 log_filters.append(format_url(
                     "TimeStamp le {}", until.strftime("%Y-%m-%dT%H:%M:%SZ")))
 
             if logger:
                 log_filters.append(format_url("Logger eq '{}'", logger))
 
             if level:
@@ -150,12 +149,7 @@
             process_name)
         response = self._rest.GET(url=url, **kwargs)
         response_as_list = response.json()['value']
         if len(response_as_list) > 0:
             message_log_entry = response_as_list[0]
             return message_log_entry['Message']
         
-    @staticmethod
-    def utc_localize_time(timestamp):
-        timestamp = pytz.utc.localize(timestamp)
-        timestamp_utc = timestamp.astimezone(pytz.utc)
-        return timestamp_utc
```

### Comparing `TM1py-2.0.2/TM1py/Services/MonitoringService.py` & `TM1py-2.0.3/TM1py/Services/MonitoringService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ObjectService.py` & `TM1py-2.0.3/TM1py/Services/ObjectService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/PowerBiService.py` & `TM1py-2.0.3/TM1py/Services/PowerBiService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ProcessService.py` & `TM1py-2.0.3/TM1py/Services/ProcessService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/RestService.py` & `TM1py-2.0.3/TM1py/Services/RestService.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from base64 import b64encode, b64decode
 from enum import Enum
 from http.client import HTTPResponse
 from http.cookies import SimpleCookie
 from io import BytesIO
 from json import JSONDecodeError
 from typing import Union, Dict, Tuple, Optional
+from ast import literal_eval
 
 import requests
 import urllib3
 from requests import Timeout, Response, ConnectionError, Session
 from requests.adapters import HTTPAdapter
 from requests.auth import HTTPBasicAuth
 from urllib3._collections import HTTPHeaderDict
@@ -36,14 +37,15 @@
 class AuthenticationMode(Enum):
     BASIC = 1
     WIA = 2
     CAM = 3
     CAM_SSO = 4
     IBM_CLOUD_API_KEY = 5
     SERVICE_TO_SERVICE = 6
+    PA_PROXY = 7
 
     @property
     def use_v12_auth(self):
         if self.value < 5:
             return False
         return True
 
@@ -70,24 +72,14 @@
         'Content-Type': 'application/json; odata.streaming=true; charset=utf-8',
         'Accept': 'application/json;odata.metadata=none,text/plain',
         'TM1-SessionContext': 'TM1py'
     }
 
     DEFAULT_CONNECTION_POOL_SIZE = 10
 
-    # You can reset the following TCP socket options based on your own use cases when tcp_keepalive is enabled
-    # TCP_KEEPIDLE: Time in seconds until the first keepalive is sent
-    # TCP_KEEPINTVL: How often should the keepalive packet be sent
-    # TCP_KEEPCNT: The max number of keepalive packets to send
-    TCP_SOCKET_OPTIONS = {
-        'TCP_KEEPIDLE': 30,
-        'TCP_KEEPINTVL': 15,
-        'TCP_KEEPCNT': 60
-    }
-
     def __init__(self, **kwargs):
         """ Create an instance of RESTService
         :param address: String - address of the TM1 instance
         :param port: Int - HTTPPortNumber as specified in the tm1s.cfg
         :param ssl: boolean -  as specified in the tm1s.cfg
         :param instance: string -  planing analytics engine (v12) instance name
         :param database: string -  planing analytics engine (v12) database name
@@ -100,24 +92,23 @@
         :param cam_passport: String - the cam passport
         :param session_id: String - TM1SessionId e.g. q7O6e1w49AixeuLVxJ1GZg
         :param application_client_id - planning analytics engine (v12) named application client ID created via manage service
         :param application_client_secret - planning analytics engine (v12) named application secret created via manage service
         :param api_key: String - planing analytics engine (v12) API Key from https://cloud.ibm.com/iam/apikeys
         :param iam_url: String - planing analytics engine (v12) IBM Cloud IAM URL. Default: "https://iam.cloud.ibm.com"
         :param pa_url: String - planing analytics engine (v12) PA URL e.g., "https://us-east-2.aws.planninganalytics.ibm.com"
+        :param cpd_url: String - cloud pack for data url (aka ZEN) CPD URL e.g., "https://cpd-zen.apps.cp4dpa-test11.cp.fyre.ibm.com"
         :param tenant: String - planing analytics engine (v12) Tenant e.g., YC4B2M1AG2Y6
         :param session_context: String - Name of the Application. Controls "Context" column in Arc / TM1top.
                 If None, use default: TM1py
         :param verify: path to .cer file or 'True' / True / 'False' / False (if no ssl verification is required)
         :param logging: boolean - switch on/off verbose http logging into sys.stdout
         :param timeout: Float - Number of seconds that the client will wait to receive the first byte.
         :param cancel_at_timeout: Abort operation in TM1 when timeout is reached
         :param async_requests_mode: changes internal REST execution mode to avoid 60s timeout on IBM cloud
-        :param tcp_keepalive: maintain the TCP connection all the time, users should choose either async_requests_mode or tcp_keepalive to run a long-run request
-                If both are True, use async_requests_mode by default
         :param connection_pool_size - In a multi threaded environment, you should set this value to a
                 higher number, such as the number of threads
         :param integrated_login: True for IntegratedSecurityMode3
         :param integrated_login_domain: NT Domain name.
                 Default: '.' for local account.
         :param integrated_login_service: Kerberos Service type for remote Service Principal Name.
                 Default: 'HTTP'
@@ -140,46 +131,42 @@
         self._base_url = kwargs.get('base_url', None)
         self._auth_url = kwargs.get('auth_url', None)
         self._instance = kwargs.get('instance', None)
         self._database = kwargs.get('database', None)
         self._api_key = kwargs.get('api_key', None)
         self._iam_url = kwargs.get('iam_url', None)
         self._pa_url = kwargs.get('pa_url', None)
+        self._cpd_url = kwargs.get('cpd_url', None)
         self._tenant = kwargs.get('tenant', None)
+        self._user = kwargs.get('user', None)
 
         # other arguments
         self._auth_mode = self._determine_auth_mode()
         self._timeout = None if kwargs.get('timeout', None) is None else float(kwargs.get('timeout'))
         self._cancel_at_timeout = kwargs.get('cancel_at_timeout', False)
         self._async_requests_mode = self.translate_to_boolean(kwargs.get('async_requests_mode', False))
-        # Set tcp_keepalive to False explicitly to turn it off when async_requests_mode is enabled
-        self._tcp_keepalive = self._determine_tcp_keepalive(kwargs.get('tcp_keepalive', False))
         self._connection_pool_size = kwargs.get('connection_pool_size', self.DEFAULT_CONNECTION_POOL_SIZE)
         self._re_connect_on_session_timeout = kwargs.get('re_connect_on_session_timeout', True)
         # is retrieved on demand and then cached
         self._sandboxing_disabled = None
         # optional verbose logging to stdout
         self.handle_logging(kwargs.get('logging', False))
 
         self._proxies = self._handle_proxies(kwargs.get('proxies', None))
+        self._is_admin = None
+        self._is_data_admin = None
+        self._is_security_admin = None
+        self._is_ops_admin = None
 
         # populated later on the fly for users with the name different from 'Admin'
-        self._is_admin = self._determine_is_admin(kwargs.get('user', None))
-
-        # populated on the fly
-        if kwargs.get('user'):
-            self._is_admin = True if case_and_space_insensitive_equals(kwargs.get('user'), 'ADMIN') else None
-            self._is_data_admin = True if case_and_space_insensitive_equals(kwargs.get('user'), 'ADMIN') else None
-            self._is_security_admin = True if case_and_space_insensitive_equals(kwargs.get('user'), 'ADMIN') else None
-            self._is_ops_admin = True if case_and_space_insensitive_equals(kwargs.get('user'), 'ADMIN') else None
-        else:
-            self._is_admin = None
-            self._is_data_admin = None
-            self._is_security_admin = None
-            self._is_ops_admin = None
+        if self._user and case_and_space_insensitive_equals(self._user, 'ADMIN'):
+            self._is_admin = True
+            self._is_data_admin = True
+            self._is_security_admin = True
+            self._is_ops_admin = True
 
         self._verify = self._determine_verify(kwargs.get('verify', None))
 
         self._base_url, self._auth_url = self._construct_service_and_auth_root()
 
         self._version = None
         self._headers = self.HEADERS.copy()
@@ -195,23 +182,14 @@
         # First contact with TM1
         self.connect()
         if not self._version:
             self.set_version()
 
         self._manage_http_adapter()
 
-    def _determine_is_admin(self, user: [None, str]) -> [None, bool]:
-        if user is None:
-            return None
-
-        return True if case_and_space_insensitive_equals(user, 'ADMIN') else None
-
-    def _determine_tcp_keepalive(self, tcp_keepalive: bool):
-        return self.translate_to_boolean(tcp_keepalive) if self._async_requests_mode is not True else False
-
     def _determine_verify(self, verify: [bool, str] = None) -> [bool, str]:
         if verify is None:
             # Default SSL verification in v12 is True
             if self._auth_mode in [AuthenticationMode.IBM_CLOUD_API_KEY, AuthenticationMode.SERVICE_TO_SERVICE]:
                 return True
             else:
                 return False
@@ -278,20 +256,21 @@
                                            **kwargs)
                 if self._re_connect_on_session_timeout and response.status_code == 401:
                     self.connect()
                     response = self._s.request(method=method, url=url, data=data, verify=self._verify, timeout=timeout,
                                                **kwargs)
 
             else:
-                additional_header = {'Prefer': 'respond-async'}
+                additional_header = {'Prefer': f'respond-async'}
                 http_headers = kwargs.get('headers', dict())
                 http_headers.update(additional_header)
                 kwargs['headers'] = http_headers
                 response = self._s.request(method=method, url=url, data=data, verify=self._verify, timeout=timeout,
                                            **kwargs)
+
                 # reconnect in case of session timeout
                 if self._re_connect_on_session_timeout and response.status_code == 401:
                     self.connect()
                     response = self._s.request(method=method, url=url, data=data, verify=self._verify, timeout=timeout,
                                                **kwargs)
                 self.verify_response(response=response)
 
@@ -371,14 +350,29 @@
             raise ValueError("'ssl' must be True to connect to TM1 > v12 in IBM Cloud")
 
         base_url = f"https://{self._address}/api/{self._tenant}/v0/tm1/{self._database}"
         auth_url = f"{base_url}/Configuration/ProductVersion/$value"
 
         return base_url, auth_url
 
+    def _construct_pa_proxy_service_and_auth_root(self) -> Tuple[str, str]:
+        if not all([self._address, self._database]):
+            raise ValueError("'address' and 'database' must be provided to connect to TM1 > v12 using PA Proxy")
+
+        base_url = "http{}://{}/tm1/{}/api/v1".format(
+            's' if self._ssl else '',
+            self._address,
+            self._database)
+
+        auth_url = "http{}://{}/login".format(
+            's' if self._ssl else '',
+            self._address)
+
+        return base_url, auth_url
+
     def _construct_s2s_service_and_auth_root(self) -> Tuple[str, str]:
         if not all([self._instance, self._database]):
             raise ValueError("'Instance' and 'Database' arguments are required for v12 authentication with 'address'")
 
         # URL Format: http{ssl}://{address}:{port}/{instance}/api/v1/Databases('{database}')
         base_url = "http{}://{}{}/{}/api/v1/Databases('{}')".format(
             's' if self._ssl else '',
@@ -436,47 +430,36 @@
             else:
                 # if the base URL is provided when the REST service is created
                 return self._construct_all_version_service_and_auth_root_from_base_url()
 
         if self._auth_mode is AuthenticationMode.IBM_CLOUD_API_KEY:
             return self._construct_ibm_cloud_service_and_auth_root()
 
+        if self._auth_mode is AuthenticationMode.PA_PROXY:
+            return self._construct_pa_proxy_service_and_auth_root()
+
         # If an address and database and instances are specified then we create a CP4D connection
         elif self._auth_mode is AuthenticationMode.SERVICE_TO_SERVICE:
             return self._construct_s2s_service_and_auth_root()
 
     def _manage_http_adapter(self):
-        if self._tcp_keepalive:
-            # SO_KEEPALIVE: set 1 to enable TCP keepalive
-            socket_options = urllib3.connection.HTTPConnection.default_socket_options + [
-                (socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1),
-                (socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, self.TCP_SOCKET_OPTIONS['TCP_KEEPIDLE']),
-                (socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, self.TCP_SOCKET_OPTIONS['TCP_KEEPINTVL']),
-                (socket.IPPROTO_TCP, socket.TCP_KEEPCNT, self.TCP_SOCKET_OPTIONS['TCP_KEEPCNT'])]
-
-            if self._connection_pool_size is not None:
-                adapter = HTTPAdapterWithSocketOptions(
-                    pool_connections=int(self._connection_pool_size),
-                    pool_maxsize=int(self._connection_pool_size),
-                    socket_options=socket_options)
-            else:
-                adapter = HTTPAdapterWithSocketOptions(socket_options=socket_options)
-
-        else:
-            adapter = HTTPAdapterWithSocketOptions(
-                pool_connections=int(self._connection_pool_size or self.DEFAULT_CONNECTION_POOL_SIZE),
-                pool_maxsize=int(self._connection_pool_size))
+        adapter = HTTPAdapterWithSocketOptions(
+            pool_connections=int(self._connection_pool_size or self.DEFAULT_CONNECTION_POOL_SIZE),
+            pool_maxsize=int(self._connection_pool_size))
 
         self._s.mount(self._base_url, adapter)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
-        self.logout()
+        try:
+            self.logout()
+        except Exception as e:
+            warnings.warn(f"Logout Failed due to Exception: {e}")
 
     def GET(
             self,
             url: str,
             data: Union[str, bytes] = '',
             headers: Dict = None,
             async_requests_mode: bool = None,
@@ -650,22 +633,18 @@
             cancel_at_timeout=cancel_at_timeout,
             encoding=encoding
         )
 
     def logout(self, timeout: float = None, **kwargs):
         """ End TM1 Session and HTTP session
         """
-        # Easier to ask for forgiveness than permission
+
         try:
-            # ProductVersion >= TM1 10.2.2 FP 6
             self.POST('/ActiveSession/tm1.Close', '', headers={"Connection": "close"}, timeout=timeout,
                       async_requests_mode=False, **kwargs)
-        except TM1pyRestException:
-            # ProductVersion < TM1 10.2.2 FP 6
-            self.POST('/api/logout', '', headers={"Connection": "close"}, timeout=timeout, **kwargs)
         finally:
             self._s.close()
 
     @staticmethod
     def _extract_tm1_session_id_from_set_cookie_header(auth_response_headers: object) -> str:
         if auth_response_headers["set-cookie"]:
             cookie = SimpleCookie()
@@ -692,14 +671,19 @@
                 host=integrated_login_host,
                 delegate=integrated_login_delegate)
 
         elif self._auth_mode == AuthenticationMode.SERVICE_TO_SERVICE:
             application_auth = HTTPBasicAuth(application_client_id, application_client_secret)
             self._s.auth = application_auth
 
+        #Get the JWT token from the CPD URL
+        elif self._auth_mode == AuthenticationMode.PA_PROXY:
+            credentials = {"username": user, "password": password}
+            jwt = self._generate_cpd_access_token(credentials)
+
         elif self._auth_mode == AuthenticationMode.IBM_CLOUD_API_KEY:
             access_token = self._generate_ibm_iam_cloud_access_token()
             self.add_http_header('Authorization', "Bearer " + access_token)
 
         # v11 authorization (Basic, CAM) through Headers
         else:
             token = self._build_authorization_token(
@@ -738,15 +722,26 @@
                             "TM1SessionId",
                             self._extract_tm1_session_id_from_set_cookie_header(auth_response_headers=response.headers))
                         warnings.warn(
                             f"TM1SessionId has failed to be automatically added to the session cookies, future requests "
                             "using this TM1Service will use the session id extracted from the first response "
                             "Check the tm1-gateway domain settings are correct"
                             "in the container orchestrator ")
-
+                elif self._auth_mode == AuthenticationMode.PA_PROXY:
+                    header = {'Content-Type': 'application/x-www-form-urlencoded'}
+                    payload = f"jwt={jwt}"
+                    response = self._s.post(
+                                        url=self._auth_url,
+                                        headers=header,
+                                        verify=self._verify,
+                                        timeout=self._timeout,
+                                        data=payload)
+                    self.verify_response(response)
+                    csrf_cookie = response.cookies.get_dict(self._address, '/')['ba-sso-csrf']
+                    self.add_http_header('ba-sso-authenticity', csrf_cookie)
                 else:
                     response = self._s.get(
                         url=self._auth_url,
                         headers=self._headers,
                         verify=self._verify,
                         timeout=self._timeout)
                     self.verify_response(response)
@@ -1042,31 +1037,47 @@
             self._database,
             self._api_key,
             self._iam_url,
             self._pa_url,
             self._tenant
         ]):
             # v11
-            if not any([self._kwargs.get('namespace', None), self._kwargs.get('gateway', None)]):
+            if not any([
+                self._kwargs.get('namespace', None),
+                self._kwargs.get('gateway', None),
+                self._kwargs.get('integrated_login', None)
+            ]):
                 return AuthenticationMode.BASIC
 
             if self._kwargs.get('gateway', None):
                 return AuthenticationMode.CAM_SSO
 
             if self._kwargs.get("integrated_login", False):
                 return AuthenticationMode.WIA
 
             return AuthenticationMode.CAM
 
         # v12
         if self._iam_url:
             return AuthenticationMode.IBM_CLOUD_API_KEY
 
+        if self._address and self._user and not self._instance:
+            return AuthenticationMode.PA_PROXY
+
         return AuthenticationMode.SERVICE_TO_SERVICE
 
+    def _generate_cpd_access_token(self, credentials) -> str:
+        if not all([self._cpd_url]):
+            raise ValueError('cpd_url must be provided to authenticate via PA Proxy')
+        url = f"{self._cpd_url}/v1/preauth/signin"
+        headers = {'Content-Type': 'application/json;charset=UTF-8'}
+        response = requests.request("POST", url, headers=headers, json=credentials, verify=self._verify)
+        jwt = literal_eval(response.content.decode('utf8'))
+        return jwt['token']
+
     def _generate_ibm_iam_cloud_access_token(self) -> str:
         if not all([self._iam_url, self._api_key]):
             raise ValueError("'iam_url' and 'api_key' must be provided to generate access token from IBM Cloud")
 
         payload = f'grant_type=urn%3Aibm%3Aparams%3Aoauth%3Agrant-type%3Aapikey&apikey={self._api_key}'
         headers = {
             'Accept': 'application/json',
```

### Comparing `TM1py-2.0.2/TM1py/Services/SandboxService.py` & `TM1py-2.0.3/TM1py/Services/SandboxService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/SecurityService.py` & `TM1py-2.0.3/TM1py/Services/SecurityService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ServerService.py` & `TM1py-2.0.3/TM1py/Services/ServerService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/SessionService.py` & `TM1py-2.0.3/TM1py/Services/SessionService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/SubsetService.py` & `TM1py-2.0.3/TM1py/Services/SubsetService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/TM1Service.py` & `TM1py-2.0.3/TM1py/Services/TM1Service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pickle
-
+import warnings
 
 from TM1py.Services import HierarchyService, SecurityService, ApplicationService, SubsetService, \
      ProcessService, AnnotationService, ViewService, RestService, CellService, \
      ChoreService, DimensionService, CubeService, ElementService, SandboxService, GitService
 from TM1py.Services.FileService import FileService
 from TM1py.Services.JobService import JobService
 from TM1py.Services.UserService import UserService
@@ -41,16 +41,14 @@
         :param session_context: String - Name of the Application. Controls "Context" column in Arc / TM1top.
                 If None, use default: TM1py
         :param verify: path to .cer file or 'True' / True / 'False' / False (if no ssl verification is required)
         :param logging: boolean - switch on/off verbose http logging into sys.stdout
         :param timeout: Float - Number of seconds that the client will wait to receive the first byte.
         :param cancel_at_timeout: Abort operation in TM1 when timeout is reached
         :param async_requests_mode: changes internal REST execution mode to avoid 60s timeout on IBM cloud
-        :param tcp_keepalive: maintain the TCP connection all the time, users should choose either async_requests_mode or tcp_keepalive to run a long-run request
-                If both are True, use async_requests_mode by default
         :param connection_pool_size - In a multi threaded environment, you should set this value to a
                 higher number, such as the number of threads
         :param integrated_login: True for IntegratedSecurityMode3
         :param integrated_login_domain: NT Domain name.
                 Default: '.' for local account.
         :param integrated_login_service: Kerberos Service type for remote Service Principal Name.
                 Default: 'HTTP'
@@ -97,15 +95,18 @@
     def logout(self, **kwargs):
         self._tm1_rest.logout(**kwargs)
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
-        self.logout()
+        try:
+            self.logout()
+        except Exception as e:
+            warnings.warn(f"Logout Failed due to Exception: {e}")
 
     @property
     def whoami(self):
         return self.security.get_current_user()
 
     @property
     def metadata(self):
```

### Comparing `TM1py-2.0.2/TM1py/Services/ThreadService.py` & `TM1py-2.0.3/TM1py/Services/ThreadService.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,10 +62,12 @@
                 continue
             if thread["Type"] == "System":
                 continue
             if thread["Name"] == "Pseudo":
                 continue
             if thread["Function"] == "GET /Threads":
                 continue
+            if thread["Function"] == "GET /api/v1/Threads":
+                continue
             self.cancel(thread["ID"], **kwargs)
             canceled_threads.append(thread)
         return canceled_threads
```

### Comparing `TM1py-2.0.2/TM1py/Services/TransactionLogService.py` & `TM1py-2.0.3/TM1py/Services/TransactionLogService.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-import pytz
 from warnings import warn
 
 from datetime import datetime
 from typing import Dict
 
 from TM1py.Services.ObjectService import ObjectService
 from TM1py.Services.RestService import RestService
-from TM1py.Utils import verify_version, deprecated_in_version, odata_track_changes_header, require_data_admin, format_url
+from TM1py.Utils import verify_version, deprecated_in_version, odata_track_changes_header, require_data_admin, format_url, utc_localize_time
 
 
 class TransactionLogService(ObjectService):
 
     def __init__(self, rest: RestService):
         super().__init__(rest)
         if verify_version(required_version="12.0.0", version=rest.version):
             # warn only due to use in Monitoring Service
             warn("Transaction Logs are not available in this version of TM1, removed as of 12.0.0", DeprecationWarning,
                  2)
         self.last_delta_request = None
 
-    @staticmethod
-    def utc_localize_time(timestamp):
-        timestamp = pytz.utc.localize(timestamp)
-        timestamp_utc = timestamp.astimezone(pytz.utc)
-        return timestamp_utc
-
     @deprecated_in_version(version="12.0.0")
     @odata_track_changes_header
     def initialize_delta_requests(self, filter=None, **kwargs):
         url = "/TailTransactionLog()"
         if filter:
             url += "?$filter={}".format(filter)
         response = self._rest.GET(url=url, **kwargs)
@@ -78,21 +71,21 @@
                 log_filters.append(format_url("Cube eq '{}'", cube))
             if element_tuple_filter:
                 log_filters.append(format_url(
                     "Tuple/any(e: {})".format(" or ".join([f"e {v} '{k}'" for k, v in element_tuple_filter.items()]))))
             if since:
                 # If since doesn't have tz information, UTC is assumed
                 if not since.tzinfo:
-                    since = self.utc_localize_time(since)
+                    since = utc_localize_time(since)
                 log_filters.append(format_url(
                     "TimeStamp ge {}", since.strftime("%Y-%m-%dT%H:%M:%SZ")))
             if until:
                 # If until doesn't have tz information, UTC is assumed
                 if not until.tzinfo:
-                    until = self.utc_localize_time(until)
+                    until = utc_localize_time(until)
                 log_filters.append(format_url(
                     "TimeStamp le {}", until.strftime("%Y-%m-%dT%H:%M:%SZ")))
             url += "&$filter={}".format(" and ".join(log_filters))
         # top limit
         if top:
             url += '&$top={}'.format(top)
         response = self._rest.GET(url, **kwargs)
```

### Comparing `TM1py-2.0.2/TM1py/Services/UserService.py` & `TM1py-2.0.3/TM1py/Services/UserService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/ViewService.py` & `TM1py-2.0.3/TM1py/Services/ViewService.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Services/__init__.py` & `TM1py-2.0.3/TM1py/Services/__init__.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Utils/MDXUtils.py` & `TM1py-2.0.3/TM1py/Utils/MDXUtils.py`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/TM1py/Utils/Utils.py` & `TM1py-2.0.3/TM1py/Utils/Utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections
 import csv
 import functools
 import http.client as http_client
 import json
 import math
+import pytz
 import re
 import ssl
 import urllib.parse as urlparse
 from contextlib import suppress
 from enum import Enum, unique
 from io import StringIO
 from typing import Any, Dict, List, Tuple, Iterable, Optional, Generator, Union, Callable
@@ -606,15 +607,15 @@
             attribute_values = list(member['Attributes'].values())
             for attribute_value in attribute_values:
                 line_items.append(str(attribute_value) if attribute_value else '')
 
         return line_items
 
 
-def build_ui_arrays_from_cellset(raw_cellset_as_dict: Dict, value_precision: int):
+def build_ui_arrays_from_cellset(raw_cellset_as_dict: Dict, value_precision: int, top: int = None):
     """ Transform raw 1,2 or 3-dimension cellset data into concise dictionary
     * Useful for grids or charting libraries that want an array of cell values per row
     * Returns 3-dimensional cell structure for tabbed grids or multiple charts
     * Rows and pages are dicts, addressable by their name. Proper order of rows can be obtained in headers[1]
     * Example 'cells' return format:
         'cells': {
             '10100': {
@@ -634,14 +635,15 @@
                 'Revenue': [ 13888143.710000003,
                              14300216.43,
                              14502421.63,
                              14321501.940000001]}
         },
     :param raw_cellset_as_dict: raw data from TM1
     :param value_precision: Integer (optional) specifying number of decimal places to return
+    :param top: Int, number of cells to return (counting from top)
     :return: dict : { titles: [], headers: [axis][], cells: { Page0: { Row0: { [row values], Row1: [], ...}, ...}, ...} }
     """
     header_map = build_headers_from_cellset(raw_cellset_as_dict, force_header_dimensionality=3)
     titles = header_map['titles']
     headers = header_map['headers']
     cardinality = header_map['cardinality']
     value_format_string = ""
@@ -654,14 +656,16 @@
     for z in range(cardinality[2]):
         z_header = headers[2][z]['name']
         pages = {}
         for y in range(cardinality[1]):
             y_header = headers[1][y]['name']
             row = []
             for x in range(cardinality[0]):
+                if top and top <= ordinal_cells:
+                    break
                 raw_value = raw_cellset_as_dict['Cells'][ordinal_cells]['Value'] or 0
                 if value_precision:
                     row.append(float(value_format_string.format(raw_value)))
                 else:
                     row.append(raw_value)
                 ordinal_cells += 1
             pages[y_header] = row
@@ -1357,14 +1361,18 @@
 def read_object_name_from_url(url: str, pattern: str) -> str:
     match = re.match(pattern, url)
     if not match:
         return None
 
     return unquote(match.group(1))
 
+def utc_localize_time(timestamp):
+    timestamp = pytz.utc.localize(timestamp)
+    timestamp_utc = timestamp.astimezone(pytz.utc)
+    return timestamp_utc
 
 class HTTPAdapterWithSocketOptions(HTTPAdapter):
     def __init__(self, *args, **kwargs):
         self.socket_options = kwargs.pop("socket_options", None)
         super(HTTPAdapterWithSocketOptions, self).__init__(*args, **kwargs)
 
     def init_poolmanager(self, *args, **kwargs):
```

### Comparing `TM1py-2.0.2/TM1py/__init__.py` & `TM1py-2.0.3/TM1py/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,9 +69,10 @@
 from TM1py.Services.AuditLogService import AuditLogService
 
 from TM1py.Services.ServerService import ServerService
 from TM1py.Services.PowerBiService import PowerBiService
 from TM1py.Services.MonitoringService import MonitoringService
 
 from TM1py.Utils import Utils
+from TM1py.Services.JobService import JobService
 
-__version__ = "2.0.2"
+__version__ = "2.0.3"
```

### Comparing `TM1py-2.0.2/TM1py.egg-info/PKG-INFO` & `TM1py-2.0.3/TM1py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TM1py
-Version: 2.0.2
+Version: 2.0.3
 Summary: A python module for TM1.
 Home-page: https://github.com/cubewise-code/tm1py
-Download-URL: https://github.com/Cubewise-code/TM1py/tarball/2.0.2
+Download-URL: https://github.com/Cubewise-code/TM1py/tarball/2.0.3
 Author: Marius Wirtz
 Author-email: MWirtz@cubewise.com
 License: MIT
 Keywords: TM1,IBM Cognos TM1,Planning Analytics,PA,Cognos
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
+Provides-Extra: dev
 License-File: LICENSE
 
 
 <img src="https://s3-ap-southeast-2.amazonaws.com/downloads.cubewise.com/web_assets/CubewiseLogos/TM1py-logo.png" style="width: 70%; height: 70%;text-align: center"/>
 
 
 TM1py is the python package for IBM Planning Analytics (TM1).
@@ -50,15 +51,16 @@
 
 Requirements
 =======================
 
 - python (3.7 or higher)
 - requests
 - requests_negotiate_sspi
-- TM1 11 
+- TM1 11, TM1 12
+- keyring
 
 
 Optional Requirements
 =======================
 
 - pandas
 
@@ -69,52 +71,74 @@
 
     pip install tm1py
     
 > with pandas
 
     pip install "tm1py[pandas]"
     
-    
+> keyring
+
+    pip install keyring
+
 Usage
 =======================
 
 > TM1 11 on-premise
 
 ``` python
 from TM1py.Services import TM1Service
 
 with TM1Service(address='localhost', port=8001, user='admin', password='apple', ssl=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 > TM1 11 on IBM cloud
 
 ``` python
 with TM1Service(
         base_url='https://mycompany.planning-analytics.ibmcloud.com/tm1/api/tm1/',
         user="non_interactive_user",
         namespace="LDAP",
         password="U3lSn5QLwoQZY2",
         ssl=True,
         verify=True,
         async_requests_mode=True) as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
+```
+
+
+> TM1 12 MCSP
+
+``` python
+from TM1py import TM1Service
+
+params = {
+    "base_url": "https://us-east-1.planninganalytics.saas.ibm.com/api/<TenantId>/v0/tm1/<DatabaseName>/",
+    "user": "apikey",
+    "password": "<TheActualApiKey>",
+    "async_requests_mode": True,
+    "ssl": True,
+    "verify": True
+}
+
+with TM1Service(**params) as tm1:
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 PAaaS
 
 ``` python
 with TM1Service(
         address="us-east-2.aws.planninganalytics.ibm.com",
         api_key="AB4VfG7T8wPM-912uFKeYG5PGh0XbS80MVBAt7SEG6xn",
         iam_url="https://iam.cloud.ibm.com/identity/token",
         tenant="YA9A2T8BS2ZU",
         database="Database") as tm1:
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 > TM1 12 on-premise & Cloud Pak For Data
 
 ``` python
 with TM1Service(
@@ -122,15 +146,15 @@
         instance="your instance name",
         database="your database name",
         application_client_id="client id",
         application_client_secret="client secret",
         user="admin",
         ssl=True) as tm1:
 
-    print(tm1.server.get_product_Version())
+    print(tm1.server.get_product_version())
 ```
 
 
 
 
 Documentation
 =======================
```

### Comparing `TM1py-2.0.2/TM1py.egg-info/SOURCES.txt` & `TM1py-2.0.3/TM1py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TM1py-2.0.2/setup.py` & `TM1py-2.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-SCHEDULE_VERSION = '2.0.2'
+SCHEDULE_VERSION = '2.0.3'
 SCHEDULE_DOWNLOAD_URL = (
         'https://github.com/Cubewise-code/TM1py/tarball/' + SCHEDULE_VERSION
 )
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
@@ -39,11 +39,15 @@
         'ijson',
         'requests',
         'pytz',
         'requests_negotiate_sspi;platform_system=="Windows"',
         'mdxpy>=1.3.1',
         'networkx'],
     extras_require={
-        "pandas": ["pandas"]
+        "pandas": ["pandas"],
+        "dev": [
+            "pytest",
+            "pytest-xdist"
+        ]
     },
     python_requires='>=3.6',
 )
```

