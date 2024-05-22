# Comparing `tmp/mypy-boto3-wafv2-1.34.52.tar.gz` & `tmp/mypy-boto3-wafv2-1.34.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-wafv2-1.34.52.tar", last modified: Wed Feb 28 20:23:14 2024, max compression
+gzip compressed data, was "mypy-boto3-wafv2-1.34.58.tar", last modified: Thu Mar  7 20:22:54 2024, max compression
```

## Comparing `mypy-boto3-wafv2-1.34.52.tar` & `mypy-boto3-wafv2-1.34.58.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:23:14.491658 mypy-boto3-wafv2-1.34.52/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-02-28 20:23:14.491658 mypy-boto3-wafv2-1.34.52/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:23:14.487658 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37407 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    59867 2024-02-28 20:23:02.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    59867 2024-02-28 20:23:02.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:23:14.487658 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-28 20:23:14.000000 mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 20:23:14.491658 mypy-boto3-wafv2-1.34.52/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-28 20:23:00.000000 mypy-boto3-wafv2-1.34.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:54.134015 mypy-boto3-wafv2-1.34.58/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-03-07 20:22:54.134015 mypy-boto3-wafv2-1.34.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:54.134015 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37410 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37407 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-07 20:22:37.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    59793 2024-03-07 20:22:38.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59793 2024-03-07 20:22:37.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:54.134015 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-07 20:22:54.000000 mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 20:22:54.134015 mypy-boto3-wafv2-1.34.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-07 20:22:36.000000 mypy-boto3-wafv2-1.34.58/setup.py
```

### Comparing `mypy-boto3-wafv2-1.34.52/LICENSE` & `mypy-boto3-wafv2-1.34.58/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.34.52/PKG-INFO` & `mypy-boto3-wafv2-1.34.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.34.52
-Summary: Type annotations for boto3.WAFV2 1.34.52 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.58
+Summary: Type annotations for boto3.WAFV2 1.34.58 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.34.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.34.52/README.md` & `mypy-boto3-wafv2-1.34.58/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.34.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/__main__.py` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.WAFV2 1.34.52\n"
-        "Version:         1.34.52\n"
+        "Type annotations for boto3.WAFV2 1.34.58\n"
+        "Version:         1.34.58\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.52")
+    print("1.34.58")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/client.py` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/client.pyi` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/literals.py` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     "WAFV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ActionValueType = Literal["ALLOW", "BLOCK", "CAPTCHA", "CHALLENGE", "COUNT", "EXCLUDED_AS_COUNT"]
-AssociatedResourceTypeType = Literal["CLOUDFRONT"]
+AssociatedResourceTypeType = Literal[
+    "API_GATEWAY",
+    "APP_RUNNER_SERVICE",
+    "CLOUDFRONT",
+    "COGNITO_USER_POOL",
+    "VERIFIED_ACCESS_INSTANCE",
+]
 BodyParsingFallbackBehaviorType = Literal["EVALUATE_AS_STRING", "MATCH", "NO_MATCH"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 CountryCodeType = Literal[
     "AD",
     "AE",
     "AF",
     "AG",
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/literals.pyi` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,21 @@
     "WAFV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
 ActionValueType = Literal["ALLOW", "BLOCK", "CAPTCHA", "CHALLENGE", "COUNT", "EXCLUDED_AS_COUNT"]
-AssociatedResourceTypeType = Literal["CLOUDFRONT"]
+AssociatedResourceTypeType = Literal[
+    "API_GATEWAY",
+    "APP_RUNNER_SERVICE",
+    "CLOUDFRONT",
+    "COGNITO_USER_POOL",
+    "VERIFIED_ACCESS_INSTANCE",
+]
 BodyParsingFallbackBehaviorType = Literal["EVALUATE_AS_STRING", "MATCH", "NO_MATCH"]
 ComparisonOperatorType = Literal["EQ", "GE", "GT", "LE", "LT", "NE"]
 CountryCodeType = Literal[
     "AD",
     "AE",
     "AF",
     "AG",
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/type_defs.py` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ActionValueType,
+    AssociatedResourceTypeType,
     BodyParsingFallbackBehaviorType,
     ComparisonOperatorType,
     CountryCodeType,
     FailureReasonType,
     FallbackBehaviorType,
     FilterBehaviorType,
     FilterRequirementType,
@@ -43,18 +44,14 @@
     ScopeType,
     SensitivityLevelType,
     SizeInspectionLimitType,
     TextTransformationTypeType,
 )
 
 if sys.version_info >= (3, 12):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -1009,15 +1006,15 @@
         "Description": NotRequired[str],
     },
 )
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
         "RequestBody": NotRequired[
-            Mapping[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef]
+            Mapping[AssociatedResourceTypeType, RequestBodyAssociatedResourceTypeConfigTypeDef]
         ],
     },
 )
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2/type_defs.pyi` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     ActionValueType,
+    AssociatedResourceTypeType,
     BodyParsingFallbackBehaviorType,
     ComparisonOperatorType,
     CountryCodeType,
     FailureReasonType,
     FallbackBehaviorType,
     FilterBehaviorType,
     FilterRequirementType,
@@ -43,18 +44,14 @@
     ScopeType,
     SensitivityLevelType,
     SizeInspectionLimitType,
     TextTransformationTypeType,
 )
 
 if sys.version_info >= (3, 12):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-if sys.version_info >= (3, 12):
     from typing import NotRequired
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
@@ -1009,15 +1006,15 @@
         "Description": NotRequired[str],
     },
 )
 AssociationConfigTypeDef = TypedDict(
     "AssociationConfigTypeDef",
     {
         "RequestBody": NotRequired[
-            Mapping[Literal["CLOUDFRONT"], RequestBodyAssociatedResourceTypeConfigTypeDef]
+            Mapping[AssociatedResourceTypeType, RequestBodyAssociatedResourceTypeConfigTypeDef]
         ],
     },
 )
 RateLimitCookieTypeDef = TypedDict(
     "RateLimitCookieTypeDef",
     {
         "Name": str,
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/PKG-INFO` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-wafv2
-Version: 1.34.52
-Summary: Type annotations for boto3.WAFV2 1.34.52 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.58
+Summary: Type annotations for boto3.WAFV2 1.34.58 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-wafv2.svg?color=blue)](https://pypi.org/project/mypy-boto3-wafv2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_wafv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-wafv2)](https://pepy.tech/project/mypy-boto3-wafv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.WAFV2 1.34.52](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
+[boto3.WAFV2 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#WAFV2)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-wafv2-1.34.52/mypy_boto3_wafv2.egg-info/SOURCES.txt` & `mypy-boto3-wafv2-1.34.58/mypy_boto3_wafv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-wafv2-1.34.52/setup.py` & `mypy-boto3-wafv2-1.34.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-wafv2",
-    version="1.34.52",
+    version="1.34.58",
     packages=["mypy_boto3_wafv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.WAFV2 1.34.52 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.WAFV2 1.34.58 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

