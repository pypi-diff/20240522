# Comparing `tmp/mypy-boto3-cloudformation-1.34.77.tar.gz` & `tmp/mypy_boto3_cloudformation-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudformation-1.34.77.tar", last modified: Wed Apr  3 19:32:38 2024, max compression
+gzip compressed data, was "mypy_boto3_cloudformation-1.34.84.tar", last modified: Fri Apr 12 19:32:35 2024, max compression
```

## Comparing `mypy-boto3-cloudformation-1.34.77.tar` & `mypy_boto3_cloudformation-1.34.84.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77001 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    76998 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21168 2024-04-03 19:32:01.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    21168 2024-04-03 19:32:01.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22366 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    22347 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-04-03 19:32:03.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    97867 2024-04-03 19:32:02.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-03 19:32:00.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 19:32:38.000000 mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:38.504162 mypy-boto3-cloudformation-1.34.77/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 19:31:59.000000 mypy-boto3-cloudformation-1.34.77/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.213306 mypy_boto3_cloudformation-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-12 19:32:35.213306 mypy_boto3_cloudformation-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18391 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.209306 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77077 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77074 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21282 2024-04-12 19:31:49.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21282 2024-04-12 19:31:49.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22409 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22390 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    23315 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    98321 2024-04-12 19:31:51.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98321 2024-04-12 19:31:50.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8824 2024-04-12 19:31:48.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:35.213306 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19974 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 19:32:35.000000 mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:35.213306 mypy_boto3_cloudformation-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-12 19:31:47.000000 mypy_boto3_cloudformation-1.34.84/setup.py
```

### Comparing `mypy-boto3-cloudformation-1.34.77/LICENSE` & `mypy_boto3_cloudformation-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/PKG-INFO` & `mypy_boto3_cloudformation-1.34.84/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.34.77
-Summary: Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.CloudFormation 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.77/README.md` & `mypy_boto3_cloudformation-1.34.84/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__init__.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/__main__.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudFormation 1.34.77\n"
-        "Version:         1.34.77\n"
+        "Type annotations for boto3.CloudFormation 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.77")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,20 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_account_limits)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#describe_account_limits)
         """
 
     def describe_change_set(
-        self, *, ChangeSetName: str, StackName: str = ..., NextToken: str = ...
+        self,
+        *,
+        ChangeSetName: str,
+        StackName: str = ...,
+        NextToken: str = ...,
+        IncludePropertyValues: bool = ...,
     ) -> DescribeChangeSetOutputTypeDef:
         """
         Returns the inputs for the change set and a list of changes that CloudFormation
         will make if you execute the change
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_change_set)
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/client.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -537,15 +537,20 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_account_limits)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/client/#describe_account_limits)
         """
 
     def describe_change_set(
-        self, *, ChangeSetName: str, StackName: str = ..., NextToken: str = ...
+        self,
+        *,
+        ChangeSetName: str,
+        StackName: str = ...,
+        NextToken: str = ...,
+        IncludePropertyValues: bool = ...,
     ) -> DescribeChangeSetOutputTypeDef:
         """
         Returns the inputs for the change set and a list of changes that CloudFormation
         will make if you execute the change
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Client.describe_change_set)
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccountFilterTypeType",
     "AccountGateStatusType",
+    "AttributeChangeTypeType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
     "ChangeSetCreateCompleteWaiterName",
     "ChangeSetHooksStatusType",
     "ChangeSetStatusType",
@@ -117,14 +118,15 @@
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
+AttributeChangeTypeType = Literal["Add", "Modify", "Remove"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
 ChangeSetHooksStatusType = Literal["PLANNED", "PLANNING", "UNAVAILABLE"]
 ChangeSetStatusType = Literal[
@@ -428,14 +430,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/literals.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccountFilterTypeType",
     "AccountGateStatusType",
+    "AttributeChangeTypeType",
     "CallAsType",
     "CapabilityType",
     "CategoryType",
     "ChangeActionType",
     "ChangeSetCreateCompleteWaiterName",
     "ChangeSetHooksStatusType",
     "ChangeSetStatusType",
@@ -117,14 +118,15 @@
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
 AccountFilterTypeType = Literal["DIFFERENCE", "INTERSECTION", "NONE", "UNION"]
 AccountGateStatusType = Literal["FAILED", "SKIPPED", "SUCCEEDED"]
+AttributeChangeTypeType = Literal["Add", "Modify", "Remove"]
 CallAsType = Literal["DELEGATED_ADMIN", "SELF"]
 CapabilityType = Literal["CAPABILITY_AUTO_EXPAND", "CAPABILITY_IAM", "CAPABILITY_NAMED_IAM"]
 CategoryType = Literal["ACTIVATED", "AWS_TYPES", "REGISTERED", "THIRD_PARTY"]
 ChangeActionType = Literal["Add", "Dynamic", "Import", "Modify", "Remove"]
 ChangeSetCreateCompleteWaiterName = Literal["change_set_create_complete"]
 ChangeSetHooksStatusType = Literal["PLANNED", "PLANNING", "UNAVAILABLE"]
 ChangeSetStatusType = Literal[
@@ -428,14 +430,15 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
+    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
+        IncludePropertyValues: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeChangeSetOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/paginator.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
+        IncludePropertyValues: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeChangeSetOutputPaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Paginator.DescribeChangeSet.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/paginators/#describechangesetpaginator)
         """
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/service_resource.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/service_resource.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/service_resource.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
+    AttributeChangeTypeType,
     CallAsType,
     CapabilityType,
     CategoryType,
     ChangeActionType,
     ChangeSetHooksStatusType,
     ChangeSetStatusType,
     ChangeSetTypeType,
@@ -621,14 +622,15 @@
 )
 DescribeChangeSetInputRequestTypeDef = TypedDict(
     "DescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
         "NextToken": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
     },
 )
 DescribeGeneratedTemplateInputRequestTypeDef = TypedDict(
     "DescribeGeneratedTemplateInputRequestTypeDef",
     {
         "GeneratedTemplateName": str,
     },
@@ -1138,14 +1140,18 @@
 )
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": NotRequired[ResourceAttributeType],
         "Name": NotRequired[str],
         "RequiresRecreation": NotRequired[RequiresRecreationType],
+        "Path": NotRequired[str],
+        "BeforeValue": NotRequired[str],
+        "AfterValue": NotRequired[str],
+        "AttributeChangeType": NotRequired[AttributeChangeTypeType],
     },
 )
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
@@ -1837,14 +1843,15 @@
     },
 )
 DescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
     "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
     "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     {
         "StackName": NotRequired[str],
@@ -1933,14 +1940,15 @@
 )
 DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
         "NextToken": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
 DescribeStacksInputStackCreateCompleteWaitTypeDef = TypedDict(
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     {
         "StackName": NotRequired[str],
@@ -2534,14 +2542,16 @@
         "PhysicalResourceId": NotRequired[str],
         "ResourceType": NotRequired[str],
         "Replacement": NotRequired[ReplacementType],
         "Scope": NotRequired[List[ResourceAttributeType]],
         "Details": NotRequired[List[ResourceChangeDetailTypeDef]],
         "ChangeSetId": NotRequired[str],
         "ModuleInfo": NotRequired[ModuleInfoTypeDef],
+        "BeforeContext": NotRequired[str],
+        "AfterContext": NotRequired[str],
     },
 )
 StackPaginatorTypeDef = TypedDict(
     "StackPaginatorTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/type_defs.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AccountFilterTypeType,
     AccountGateStatusType,
+    AttributeChangeTypeType,
     CallAsType,
     CapabilityType,
     CategoryType,
     ChangeActionType,
     ChangeSetHooksStatusType,
     ChangeSetStatusType,
     ChangeSetTypeType,
@@ -621,14 +622,15 @@
 )
 DescribeChangeSetInputRequestTypeDef = TypedDict(
     "DescribeChangeSetInputRequestTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
         "NextToken": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
     },
 )
 DescribeGeneratedTemplateInputRequestTypeDef = TypedDict(
     "DescribeGeneratedTemplateInputRequestTypeDef",
     {
         "GeneratedTemplateName": str,
     },
@@ -1138,14 +1140,18 @@
 )
 ResourceTargetDefinitionTypeDef = TypedDict(
     "ResourceTargetDefinitionTypeDef",
     {
         "Attribute": NotRequired[ResourceAttributeType],
         "Name": NotRequired[str],
         "RequiresRecreation": NotRequired[RequiresRecreationType],
+        "Path": NotRequired[str],
+        "BeforeValue": NotRequired[str],
+        "AfterValue": NotRequired[str],
+        "AttributeChangeType": NotRequired[AttributeChangeTypeType],
     },
 )
 RollbackTriggerTypeDef = TypedDict(
     "RollbackTriggerTypeDef",
     {
         "Arn": str,
         "Type": str,
@@ -1837,14 +1843,15 @@
     },
 )
 DescribeChangeSetInputDescribeChangeSetPaginateTypeDef = TypedDict(
     "DescribeChangeSetInputDescribeChangeSetPaginateTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 DescribeStackEventsInputDescribeStackEventsPaginateTypeDef = TypedDict(
     "DescribeStackEventsInputDescribeStackEventsPaginateTypeDef",
     {
         "StackName": NotRequired[str],
@@ -1933,14 +1940,15 @@
 )
 DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef = TypedDict(
     "DescribeChangeSetInputChangeSetCreateCompleteWaitTypeDef",
     {
         "ChangeSetName": str,
         "StackName": NotRequired[str],
         "NextToken": NotRequired[str],
+        "IncludePropertyValues": NotRequired[bool],
         "WaiterConfig": NotRequired[WaiterConfigTypeDef],
     },
 )
 DescribeStacksInputStackCreateCompleteWaitTypeDef = TypedDict(
     "DescribeStacksInputStackCreateCompleteWaitTypeDef",
     {
         "StackName": NotRequired[str],
@@ -2534,14 +2542,16 @@
         "PhysicalResourceId": NotRequired[str],
         "ResourceType": NotRequired[str],
         "Replacement": NotRequired[ReplacementType],
         "Scope": NotRequired[List[ResourceAttributeType]],
         "Details": NotRequired[List[ResourceChangeDetailTypeDef]],
         "ChangeSetId": NotRequired[str],
         "ModuleInfo": NotRequired[ModuleInfoTypeDef],
+        "BeforeContext": NotRequired[str],
+        "AfterContext": NotRequired[str],
     },
 )
 StackPaginatorTypeDef = TypedDict(
     "StackPaginatorTypeDef",
     {
         "StackName": str,
         "CreationTime": datetime,
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.py` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
     def wait(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
+        IncludePropertyValues: bool = ...,
         WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Waiter.ChangeSetCreateComplete.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/waiters/#changesetcreatecompletewaiter)
         """
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation/waiter.pyi` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     def wait(
         self,
         *,
         ChangeSetName: str,
         StackName: str = ...,
         NextToken: str = ...,
+        IncludePropertyValues: bool = ...,
         WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation.Waiter.ChangeSetCreateComplete.wait)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/waiters/#changesetcreatecompletewaiter)
         """
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/PKG-INFO` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudformation
-Version: 1.34.77
-Summary: Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.CloudFormation 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudformation.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudformation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudformation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudformation)](https://pepy.tech/project/mypy-boto3-cloudformation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudFormation 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
+[boto3.CloudFormation 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#CloudFormation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-cloudformation-1.34.77/mypy_boto3_cloudformation.egg-info/SOURCES.txt` & `mypy_boto3_cloudformation-1.34.84/mypy_boto3_cloudformation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudformation-1.34.77/setup.py` & `mypy_boto3_cloudformation-1.34.84/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudformation",
-    version="1.34.77",
+    version="1.34.84",
     packages=["mypy_boto3_cloudformation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.CloudFormation 1.34.77 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.CloudFormation 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

