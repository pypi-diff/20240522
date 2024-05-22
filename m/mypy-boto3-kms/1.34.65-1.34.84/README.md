# Comparing `tmp/mypy-boto3-kms-1.34.65.tar.gz` & `tmp/mypy_boto3_kms-1.34.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kms-1.34.65.tar", last modified: Mon Mar 18 20:47:30 2024, max compression
+gzip compressed data, was "mypy_boto3_kms-1.34.84.tar", last modified: Fri Apr 12 19:32:36 2024, max compression
```

## Comparing `mypy-boto3-kms-1.34.65.tar` & `mypy_boto3_kms-1.34.84.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.186615 mypy-boto3-kms-1.34.65/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-03-18 20:47:30.186615 mypy-boto3-kms-1.34.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11666 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.186615 mypy-boto3-kms-1.34.65/mypy_boto3_kms/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40973 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40970 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-03-18 20:46:57.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13627 2024-03-18 20:46:57.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8004 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 20:46:56.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34413 2024-03-18 20:46:57.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34413 2024-03-18 20:46:57.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:47:30.186615 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 20:47:30.000000 mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 20:47:30.186615 mypy-boto3-kms-1.34.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-18 20:46:55.000000 mypy-boto3-kms-1.34.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.961304 mypy_boto3_kms-1.34.84/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13337 2024-04-12 19:32:36.961304 mypy_boto3_kms-1.34.84/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11798 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.961304 mypy_boto3_kms-1.34.84/mypy_boto3_kms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42810 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42807 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13890 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9030 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    36125 2024-04-12 19:32:09.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36125 2024-04-12 19:32:09.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 19:32:36.961304 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13337 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 19:32:36.000000 mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 19:32:36.961304 mypy_boto3_kms-1.34.84/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-12 19:32:08.000000 mypy_boto3_kms-1.34.84/setup.py
```

### Comparing `mypy-boto3-kms-1.34.65/LICENSE` & `mypy_boto3_kms-1.34.84/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.34.65/PKG-INFO` & `mypy_boto3_kms-1.34.84/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.34.65
-Summary: Type annotations for boto3.KMS 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.KMS 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -283,14 +283,15 @@
 
 from mypy_boto3_kms import KMSClient
 from mypy_boto3_kms.paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 client: KMSClient = Session().client("kms")
 
@@ -298,14 +299,15 @@
 # Types should be correctly discovered by mypy and IDEs
 describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator(
     "describe_custom_key_stores"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
 list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
 list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
 list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
 list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator(
     "list_retirable_grants"
 )
 ```
```

### Comparing `mypy-boto3-kms-1.34.65/README.md` & `mypy_boto3_kms-1.34.84/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -250,14 +250,15 @@
 
 from mypy_boto3_kms import KMSClient
 from mypy_boto3_kms.paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 client: KMSClient = Session().client("kms")
 
@@ -265,14 +266,15 @@
 # Types should be correctly discovered by mypy and IDEs
 describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator(
     "describe_custom_key_stores"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
 list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
 list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
 list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
 list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator(
     "list_retirable_grants"
 )
 ```
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/__init__.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,53 @@
     from mypy_boto3_kms import (
         Client,
         DescribeCustomKeyStoresPaginator,
         KMSClient,
         ListAliasesPaginator,
         ListGrantsPaginator,
         ListKeyPoliciesPaginator,
+        ListKeyRotationsPaginator,
         ListKeysPaginator,
         ListResourceTagsPaginator,
         ListRetirableGrantsPaginator,
     )
 
     session = Session()
     client: KMSClient = session.client("kms")
 
     describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
     list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+    list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
     list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
     list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
     list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator("list_retirable_grants")
     ```
 """
 
 from .client import KMSClient
 from .paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 Client = KMSClient
 
 __all__ = (
     "Client",
     "DescribeCustomKeyStoresPaginator",
     "KMSClient",
     "ListAliasesPaginator",
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
+    "ListKeyRotationsPaginator",
     "ListKeysPaginator",
     "ListResourceTagsPaginator",
     "ListRetirableGrantsPaginator",
 )
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/__init__.pyi` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/__init__.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,53 @@
     from mypy_boto3_kms import (
         Client,
         DescribeCustomKeyStoresPaginator,
         KMSClient,
         ListAliasesPaginator,
         ListGrantsPaginator,
         ListKeyPoliciesPaginator,
+        ListKeyRotationsPaginator,
         ListKeysPaginator,
         ListResourceTagsPaginator,
         ListRetirableGrantsPaginator,
     )
 
     session = Session()
     client: KMSClient = session.client("kms")
 
     describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
     list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+    list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
     list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
     list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
     list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator("list_retirable_grants")
     ```
 """
 
 from .client import KMSClient
 from .paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 Client = KMSClient
 
 __all__ = (
     "Client",
     "DescribeCustomKeyStoresPaginator",
     "KMSClient",
     "ListAliasesPaginator",
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
+    "ListKeyRotationsPaginator",
     "ListKeysPaginator",
     "ListResourceTagsPaginator",
     "ListRetirableGrantsPaginator",
 )
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/__main__.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KMS 1.34.65\n"
-        "Version:         1.34.65\n"
+        "Type annotations for boto3.KMS 1.34.84\n"
+        "Version:         1.34.84\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.65")
+    print("1.34.84")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/client.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     XksProxyConnectivityTypeType,
 )
 from .paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
@@ -67,19 +68,21 @@
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
     GrantConstraintsTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
+    ListKeyRotationsResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
+    RotateKeyOnDemandResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
@@ -88,31 +91,30 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("KMSClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
     DryRunOperationException: Type[BotocoreClientError]
@@ -147,15 +149,14 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
-
 class KMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/)
     """
 
     meta: ClientMeta
@@ -389,18 +390,20 @@
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key)
         """
 
-    def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
+    def enable_key_rotation(
+        self, *, KeyId: str, RotationPeriodInDays: int = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
-        material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
+        material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html#rotating-keys-enable-disable)
         of the specified symmetric encryption KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
 
@@ -541,18 +544,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_policy)
         """
 
     def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
-        Gets a Boolean value that indicates whether [automatic rotation of the key
+        Provides detailed information about the rotation status for a KMS key,
+        including whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
-        is enabled for the specified KMS
-        key.
+        is enabled for the specified KMS key, the `rotation period
+        <https://docs.aws.amazon.com/kms/...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_rotation_status)
         """
 
     def get_parameters_for_import(
         self,
@@ -630,14 +634,26 @@
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_policies)
         """
 
+    def list_key_rotations(
+        self, *, KeyId: str, Limit: int = ..., Marker: str = ...
+    ) -> ListKeyRotationsResponseTypeDef:
+        """
+        Returns information about all completed key material rotations for the
+        specified KMS
+        key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_rotations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_rotations)
+        """
+
     def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_keys)
@@ -733,14 +749,24 @@
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#revoke_grant)
         """
 
+    def rotate_key_on_demand(self, *, KeyId: str) -> RotateKeyOnDemandResponseTypeDef:
+        """
+        Immediately initiates rotation of the key material of the specified symmetric
+        encryption KMS
+        key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.rotate_key_on_demand)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#rotate_key_on_demand)
+        """
+
     def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
@@ -901,14 +927,23 @@
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_key_rotations"]
+    ) -> ListKeyRotationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/client.pyi` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     XksProxyConnectivityTypeType,
 )
 from .paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 from .type_defs import (
     BlobTypeDef,
     CancelKeyDeletionResponseTypeDef,
@@ -67,19 +68,21 @@
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
     GrantConstraintsTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
+    ListKeyRotationsResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
     ReplicateKeyResponseTypeDef,
+    RotateKeyOnDemandResponseTypeDef,
     ScheduleKeyDeletionResponseTypeDef,
     SignResponseTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     VerifyMacResponseTypeDef,
     VerifyResponseTypeDef,
     XksProxyAuthenticationCredentialTypeTypeDef,
@@ -88,29 +91,32 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("KMSClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
+    ConflictException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
     DryRunOperationException: Type[BotocoreClientError]
@@ -145,14 +151,15 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
+
 class KMSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/)
     """
 
     meta: ClientMeta
@@ -386,18 +393,20 @@
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key)
         """
 
-    def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
+    def enable_key_rotation(
+        self, *, KeyId: str, RotationPeriodInDays: int = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
-        material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
+        material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html#rotating-keys-enable-disable)
         of the specified symmetric encryption KMS
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#enable_key_rotation)
         """
 
@@ -538,18 +547,19 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_policy)
         """
 
     def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
-        Gets a Boolean value that indicates whether [automatic rotation of the key
+        Provides detailed information about the rotation status for a KMS key,
+        including whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-keys.html)
-        is enabled for the specified KMS
-        key.
+        is enabled for the specified KMS key, the `rotation period
+        <https://docs.aws.amazon.com/kms/...`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_key_rotation_status)
         """
 
     def get_parameters_for_import(
         self,
@@ -627,14 +637,26 @@
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_policies)
         """
 
+    def list_key_rotations(
+        self, *, KeyId: str, Limit: int = ..., Marker: str = ...
+    ) -> ListKeyRotationsResponseTypeDef:
+        """
+        Returns information about all completed key material rotations for the
+        specified KMS
+        key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_rotations)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_key_rotations)
+        """
+
     def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#list_keys)
@@ -730,14 +752,24 @@
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#revoke_grant)
         """
 
+    def rotate_key_on_demand(self, *, KeyId: str) -> RotateKeyOnDemandResponseTypeDef:
+        """
+        Immediately initiates rotation of the key material of the specified symmetric
+        encryption KMS
+        key.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.rotate_key_on_demand)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#rotate_key_on_demand)
+        """
+
     def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
@@ -898,14 +930,23 @@
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_key_rotations"]
+    ) -> ListKeyRotationsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/literals.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     "KeyManagerTypeType",
     "KeySpecType",
     "KeyStateType",
     "KeyUsageTypeType",
     "ListAliasesPaginatorName",
     "ListGrantsPaginatorName",
     "ListKeyPoliciesPaginatorName",
+    "ListKeyRotationsPaginatorName",
     "ListKeysPaginatorName",
     "ListResourceTagsPaginatorName",
     "ListRetirableGrantsPaginatorName",
     "MacAlgorithmSpecType",
     "MessageTypeType",
     "MultiRegionKeyTypeType",
     "OriginTypeType",
+    "RotationTypeType",
     "SigningAlgorithmSpecType",
     "WrappingKeySpecType",
     "XksProxyConnectivityTypeType",
     "KMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
@@ -163,21 +165,23 @@
     "Unavailable",
     "Updating",
 ]
 KeyUsageTypeType = Literal["ENCRYPT_DECRYPT", "GENERATE_VERIFY_MAC", "SIGN_VERIFY"]
 ListAliasesPaginatorName = Literal["list_aliases"]
 ListGrantsPaginatorName = Literal["list_grants"]
 ListKeyPoliciesPaginatorName = Literal["list_key_policies"]
+ListKeyRotationsPaginatorName = Literal["list_key_rotations"]
 ListKeysPaginatorName = Literal["list_keys"]
 ListResourceTagsPaginatorName = Literal["list_resource_tags"]
 ListRetirableGrantsPaginatorName = Literal["list_retirable_grants"]
 MacAlgorithmSpecType = Literal["HMAC_SHA_224", "HMAC_SHA_256", "HMAC_SHA_384", "HMAC_SHA_512"]
 MessageTypeType = Literal["DIGEST", "RAW"]
 MultiRegionKeyTypeType = Literal["PRIMARY", "REPLICA"]
 OriginTypeType = Literal["AWS_CLOUDHSM", "AWS_KMS", "EXTERNAL", "EXTERNAL_KEY_STORE"]
+RotationTypeType = Literal["AUTOMATIC", "ON_DEMAND"]
 SigningAlgorithmSpecType = Literal[
     "ECDSA_SHA_256",
     "ECDSA_SHA_384",
     "ECDSA_SHA_512",
     "RSASSA_PKCS1_V1_5_SHA_256",
     "RSASSA_PKCS1_V1_5_SHA_384",
     "RSASSA_PKCS1_V1_5_SHA_512",
@@ -256,14 +260,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -276,24 +281,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -583,14 +590,15 @@
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_custom_key_stores",
     "list_aliases",
     "list_grants",
     "list_key_policies",
+    "list_key_rotations",
     "list_keys",
     "list_resource_tags",
     "list_retirable_grants",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/literals.pyi` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     "KeyManagerTypeType",
     "KeySpecType",
     "KeyStateType",
     "KeyUsageTypeType",
     "ListAliasesPaginatorName",
     "ListGrantsPaginatorName",
     "ListKeyPoliciesPaginatorName",
+    "ListKeyRotationsPaginatorName",
     "ListKeysPaginatorName",
     "ListResourceTagsPaginatorName",
     "ListRetirableGrantsPaginatorName",
     "MacAlgorithmSpecType",
     "MessageTypeType",
     "MultiRegionKeyTypeType",
     "OriginTypeType",
+    "RotationTypeType",
     "SigningAlgorithmSpecType",
     "WrappingKeySpecType",
     "XksProxyConnectivityTypeType",
     "KMSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
@@ -163,21 +165,23 @@
     "Unavailable",
     "Updating",
 ]
 KeyUsageTypeType = Literal["ENCRYPT_DECRYPT", "GENERATE_VERIFY_MAC", "SIGN_VERIFY"]
 ListAliasesPaginatorName = Literal["list_aliases"]
 ListGrantsPaginatorName = Literal["list_grants"]
 ListKeyPoliciesPaginatorName = Literal["list_key_policies"]
+ListKeyRotationsPaginatorName = Literal["list_key_rotations"]
 ListKeysPaginatorName = Literal["list_keys"]
 ListResourceTagsPaginatorName = Literal["list_resource_tags"]
 ListRetirableGrantsPaginatorName = Literal["list_retirable_grants"]
 MacAlgorithmSpecType = Literal["HMAC_SHA_224", "HMAC_SHA_256", "HMAC_SHA_384", "HMAC_SHA_512"]
 MessageTypeType = Literal["DIGEST", "RAW"]
 MultiRegionKeyTypeType = Literal["PRIMARY", "REPLICA"]
 OriginTypeType = Literal["AWS_CLOUDHSM", "AWS_KMS", "EXTERNAL", "EXTERNAL_KEY_STORE"]
+RotationTypeType = Literal["AUTOMATIC", "ON_DEMAND"]
 SigningAlgorithmSpecType = Literal[
     "ECDSA_SHA_256",
     "ECDSA_SHA_384",
     "ECDSA_SHA_512",
     "RSASSA_PKCS1_V1_5_SHA_256",
     "RSASSA_PKCS1_V1_5_SHA_384",
     "RSASSA_PKCS1_V1_5_SHA_512",
@@ -256,14 +260,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -276,24 +281,26 @@
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
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -583,14 +590,15 @@
     "sqs",
 ]
 PaginatorName = Literal[
     "describe_custom_key_stores",
     "list_aliases",
     "list_grants",
     "list_key_policies",
+    "list_key_rotations",
     "list_keys",
     "list_resource_tags",
     "list_retirable_grants",
 ]
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/paginator.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
     from mypy_boto3_kms.client import KMSClient
     from mypy_boto3_kms.paginator import (
         DescribeCustomKeyStoresPaginator,
         ListAliasesPaginator,
         ListGrantsPaginator,
         ListKeyPoliciesPaginator,
+        ListKeyRotationsPaginator,
         ListKeysPaginator,
         ListResourceTagsPaginator,
         ListRetirableGrantsPaginator,
     )
 
     session = Session()
     client: KMSClient = session.client("kms")
 
     describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
     list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+    list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
     list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
     list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
     list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator("list_retirable_grants")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
@@ -37,39 +39,39 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeCustomKeyStoresResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponsePaginatorTypeDef,
     ListKeyPoliciesResponseTypeDef,
+    ListKeyRotationsResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeCustomKeyStoresPaginator",
     "ListAliasesPaginator",
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
+    "ListKeyRotationsPaginator",
     "ListKeysPaginator",
     "ListResourceTagsPaginator",
     "ListRetirableGrantsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeCustomKeyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
     """
 
     def paginate(
@@ -80,30 +82,28 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
         """
 
-
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
         self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
         """
 
-
 class ListGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
     """
 
     def paginate(
@@ -115,29 +115,41 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGrantsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
         """
 
-
 class ListKeyPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
         self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
         """
 
+class ListKeyRotationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyRotations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyrotationspaginator)
+    """
+
+    def paginate(
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListKeyRotationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyRotations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyrotationspaginator)
+        """
 
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
     """
 
@@ -145,30 +157,28 @@
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
         """
 
-
 class ListResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
         self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
         """
 
-
 class ListRetirableGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/paginator.pyi` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/paginator.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
     from mypy_boto3_kms.client import KMSClient
     from mypy_boto3_kms.paginator import (
         DescribeCustomKeyStoresPaginator,
         ListAliasesPaginator,
         ListGrantsPaginator,
         ListKeyPoliciesPaginator,
+        ListKeyRotationsPaginator,
         ListKeysPaginator,
         ListResourceTagsPaginator,
         ListRetirableGrantsPaginator,
     )
 
     session = Session()
     client: KMSClient = session.client("kms")
 
     describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")
     list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
     list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
     list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+    list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
     list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
     list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
     list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator("list_retirable_grants")
     ```
 """
 
 from typing import Generic, Iterator, TypeVar
@@ -37,37 +39,41 @@
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     DescribeCustomKeyStoresResponseTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponsePaginatorTypeDef,
     ListKeyPoliciesResponseTypeDef,
+    ListKeyRotationsResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = (
     "DescribeCustomKeyStoresPaginator",
     "ListAliasesPaginator",
     "ListGrantsPaginator",
     "ListKeyPoliciesPaginator",
+    "ListKeyRotationsPaginator",
     "ListKeysPaginator",
     "ListResourceTagsPaginator",
     "ListRetirableGrantsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeCustomKeyStoresPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
     """
 
     def paginate(
@@ -78,28 +84,30 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[DescribeCustomKeyStoresResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.DescribeCustomKeyStores.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#describecustomkeystorespaginator)
         """
 
+
 class ListAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
     """
 
     def paginate(
         self, *, KeyId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listaliasespaginator)
         """
 
+
 class ListGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
     """
 
     def paginate(
@@ -111,56 +119,75 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListGrantsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListGrants.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listgrantspaginator)
         """
 
+
 class ListKeyPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
     """
 
     def paginate(
         self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeypoliciespaginator)
         """
 
+
+class ListKeyRotationsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyRotations)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyrotationspaginator)
+    """
+
+    def paginate(
+        self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
+    ) -> _PageIterator[ListKeyRotationsResponseTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeyRotations.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyrotationspaginator)
+        """
+
+
 class ListKeysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListKeys.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listkeyspaginator)
         """
 
+
 class ListResourceTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
     """
 
     def paginate(
         self, *, KeyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListResourceTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listresourcetagspaginator)
         """
 
+
 class ListRetirableGrantsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Paginator.ListRetirableGrants)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/paginators/#listretirablegrantspaginator)
     """
 
     def paginate(
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/type_defs.py` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     KeySpecType,
     KeyStateType,
     KeyUsageTypeType,
     MacAlgorithmSpecType,
     MessageTypeType,
     MultiRegionKeyTypeType,
     OriginTypeType,
+    RotationTypeType,
     SigningAlgorithmSpecType,
     WrappingKeySpecType,
     XksProxyConnectivityTypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -86,21 +87,24 @@
     "GrantConstraintsPaginatorTypeDef",
     "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
+    "ListKeyRotationsRequestRequestTypeDef",
+    "RotationsListEntryTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
+    "RotateKeyOnDemandRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
     "EncryptRequestRequestTypeDef",
     "GenerateMacRequestRequestTypeDef",
@@ -124,14 +128,15 @@
     "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportResponseTypeDef",
     "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
     "ListKeyPoliciesResponseTypeDef",
     "ReEncryptResponseTypeDef",
+    "RotateKeyOnDemandResponseTypeDef",
     "ScheduleKeyDeletionResponseTypeDef",
     "SignResponseTypeDef",
     "VerifyMacResponseTypeDef",
     "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
@@ -141,20 +146,22 @@
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeyRotationsRequestListKeyRotationsPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "GrantListEntryPaginatorTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
+    "ListKeyRotationsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
     "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
@@ -302,14 +309,15 @@
         "KeyId": str,
     },
 )
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
+        "RotationPeriodInDays": NotRequired[int],
     },
 )
 GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
@@ -400,14 +408,30 @@
     "ListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": NotRequired[int],
         "Marker": NotRequired[str],
     },
 )
+ListKeyRotationsRequestRequestTypeDef = TypedDict(
+    "ListKeyRotationsRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Limit": NotRequired[int],
+        "Marker": NotRequired[str],
+    },
+)
+RotationsListEntryTypeDef = TypedDict(
+    "RotationsListEntryTypeDef",
+    {
+        "KeyId": NotRequired[str],
+        "RotationDate": NotRequired[datetime],
+        "RotationType": NotRequired[RotationTypeType],
+    },
+)
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": NotRequired[int],
         "Marker": NotRequired[str],
     },
 )
@@ -456,14 +480,20 @@
     "RevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "DryRun": NotRequired[bool],
     },
 )
+RotateKeyOnDemandRequestRequestTypeDef = TypedDict(
+    "RotateKeyOnDemandRequestRequestTypeDef",
+    {
+        "KeyId": str,
+    },
+)
 ScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "ScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
         "PendingWindowInDays": NotRequired[int],
     },
 )
@@ -683,14 +713,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetKeyRotationStatusResponseTypeDef = TypedDict(
     "GetKeyRotationStatusResponseTypeDef",
     {
         "KeyRotationEnabled": bool,
+        "KeyId": str,
+        "RotationPeriodInDays": int,
+        "NextRotationDate": datetime,
+        "OnDemandRotationStartDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetParametersForImportResponseTypeDef = TypedDict(
     "GetParametersForImportResponseTypeDef",
     {
         "KeyId": str,
@@ -738,14 +772,21 @@
         "SourceKeyId": str,
         "KeyId": str,
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RotateKeyOnDemandResponseTypeDef = TypedDict(
+    "RotateKeyOnDemandResponseTypeDef",
+    {
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ScheduleKeyDeletionResponseTypeDef = TypedDict(
     "ScheduleKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
         "DeletionDate": datetime,
         "KeyState": KeyStateType,
         "PendingWindowInDays": int,
@@ -923,14 +964,21 @@
 ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "KeyId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListKeyRotationsRequestListKeyRotationsPaginateTypeDef = TypedDict(
+    "ListKeyRotationsRequestListKeyRotationsPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListKeysRequestListKeysPaginateTypeDef = TypedDict(
     "ListKeysRequestListKeysPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
@@ -976,14 +1024,23 @@
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListKeyRotationsResponseTypeDef = TypedDict(
+    "ListKeyRotationsResponseTypeDef",
+    {
+        "Rotations": List[RotationsListEntryTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": NotRequired[MultiRegionKeyTypeType],
         "PrimaryKey": NotRequired[MultiRegionKeyTypeDef],
         "ReplicaKeys": NotRequired[List[MultiRegionKeyTypeDef]],
     },
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms/type_defs.pyi` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     KeySpecType,
     KeyStateType,
     KeyUsageTypeType,
     MacAlgorithmSpecType,
     MessageTypeType,
     MultiRegionKeyTypeType,
     OriginTypeType,
+    RotationTypeType,
     SigningAlgorithmSpecType,
     WrappingKeySpecType,
     XksProxyConnectivityTypeType,
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
@@ -86,21 +87,24 @@
     "GrantConstraintsPaginatorTypeDef",
     "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
+    "ListKeyRotationsRequestRequestTypeDef",
+    "RotationsListEntryTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListResourceTagsRequestRequestTypeDef",
     "ListRetirableGrantsRequestRequestTypeDef",
     "MultiRegionKeyTypeDef",
     "PutKeyPolicyRequestRequestTypeDef",
     "RetireGrantRequestRequestTypeDef",
     "RevokeGrantRequestRequestTypeDef",
+    "RotateKeyOnDemandRequestRequestTypeDef",
     "ScheduleKeyDeletionRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "UpdateKeyDescriptionRequestRequestTypeDef",
     "UpdatePrimaryRegionRequestRequestTypeDef",
     "EncryptRequestRequestTypeDef",
     "GenerateMacRequestRequestTypeDef",
@@ -124,14 +128,15 @@
     "GetKeyPolicyResponseTypeDef",
     "GetKeyRotationStatusResponseTypeDef",
     "GetParametersForImportResponseTypeDef",
     "GetPublicKeyResponseTypeDef",
     "ListAliasesResponseTypeDef",
     "ListKeyPoliciesResponseTypeDef",
     "ReEncryptResponseTypeDef",
+    "RotateKeyOnDemandResponseTypeDef",
     "ScheduleKeyDeletionResponseTypeDef",
     "SignResponseTypeDef",
     "VerifyMacResponseTypeDef",
     "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
@@ -141,20 +146,22 @@
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
+    "ListKeyRotationsRequestListKeyRotationsPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
     "GrantListEntryPaginatorTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
+    "ListKeyRotationsResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
     "ListGrantsResponseTypeDef",
     "DescribeCustomKeyStoresResponseTypeDef",
@@ -302,14 +309,15 @@
         "KeyId": str,
     },
 )
 EnableKeyRotationRequestRequestTypeDef = TypedDict(
     "EnableKeyRotationRequestRequestTypeDef",
     {
         "KeyId": str,
+        "RotationPeriodInDays": NotRequired[int],
     },
 )
 GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "KeyId": str,
         "KeyPairSpec": DataKeyPairSpecType,
@@ -400,14 +408,30 @@
     "ListKeyPoliciesRequestRequestTypeDef",
     {
         "KeyId": str,
         "Limit": NotRequired[int],
         "Marker": NotRequired[str],
     },
 )
+ListKeyRotationsRequestRequestTypeDef = TypedDict(
+    "ListKeyRotationsRequestRequestTypeDef",
+    {
+        "KeyId": str,
+        "Limit": NotRequired[int],
+        "Marker": NotRequired[str],
+    },
+)
+RotationsListEntryTypeDef = TypedDict(
+    "RotationsListEntryTypeDef",
+    {
+        "KeyId": NotRequired[str],
+        "RotationDate": NotRequired[datetime],
+        "RotationType": NotRequired[RotationTypeType],
+    },
+)
 ListKeysRequestRequestTypeDef = TypedDict(
     "ListKeysRequestRequestTypeDef",
     {
         "Limit": NotRequired[int],
         "Marker": NotRequired[str],
     },
 )
@@ -456,14 +480,20 @@
     "RevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
         "DryRun": NotRequired[bool],
     },
 )
+RotateKeyOnDemandRequestRequestTypeDef = TypedDict(
+    "RotateKeyOnDemandRequestRequestTypeDef",
+    {
+        "KeyId": str,
+    },
+)
 ScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "ScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
         "PendingWindowInDays": NotRequired[int],
     },
 )
@@ -683,14 +713,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetKeyRotationStatusResponseTypeDef = TypedDict(
     "GetKeyRotationStatusResponseTypeDef",
     {
         "KeyRotationEnabled": bool,
+        "KeyId": str,
+        "RotationPeriodInDays": int,
+        "NextRotationDate": datetime,
+        "OnDemandRotationStartDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetParametersForImportResponseTypeDef = TypedDict(
     "GetParametersForImportResponseTypeDef",
     {
         "KeyId": str,
@@ -738,14 +772,21 @@
         "SourceKeyId": str,
         "KeyId": str,
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+RotateKeyOnDemandResponseTypeDef = TypedDict(
+    "RotateKeyOnDemandResponseTypeDef",
+    {
+        "KeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 ScheduleKeyDeletionResponseTypeDef = TypedDict(
     "ScheduleKeyDeletionResponseTypeDef",
     {
         "KeyId": str,
         "DeletionDate": datetime,
         "KeyState": KeyStateType,
         "PendingWindowInDays": int,
@@ -923,14 +964,21 @@
 ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef = TypedDict(
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     {
         "KeyId": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
+ListKeyRotationsRequestListKeyRotationsPaginateTypeDef = TypedDict(
+    "ListKeyRotationsRequestListKeyRotationsPaginateTypeDef",
+    {
+        "KeyId": str,
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
 ListKeysRequestListKeysPaginateTypeDef = TypedDict(
     "ListKeysRequestListKeysPaginateTypeDef",
     {
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListResourceTagsRequestListResourceTagsPaginateTypeDef = TypedDict(
@@ -976,14 +1024,23 @@
     {
         "Keys": List[KeyListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+ListKeyRotationsResponseTypeDef = TypedDict(
+    "ListKeyRotationsResponseTypeDef",
+    {
+        "Rotations": List[RotationsListEntryTypeDef],
+        "NextMarker": str,
+        "Truncated": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 MultiRegionConfigurationTypeDef = TypedDict(
     "MultiRegionConfigurationTypeDef",
     {
         "MultiRegionKeyType": NotRequired[MultiRegionKeyTypeType],
         "PrimaryKey": NotRequired[MultiRegionKeyTypeDef],
         "ReplicaKeys": NotRequired[List[MultiRegionKeyTypeDef]],
     },
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/PKG-INFO` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kms
-Version: 1.34.65
-Summary: Type annotations for boto3.KMS 1.34.65 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.84
+Summary: Type annotations for boto3.KMS 1.34.84 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kms.svg?color=blue)](https://pypi.org/project/mypy-boto3-kms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kms)](https://pepy.tech/project/mypy-boto3-kms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KMS 1.34.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
+[boto3.KMS 1.34.84](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -283,14 +283,15 @@
 
 from mypy_boto3_kms import KMSClient
 from mypy_boto3_kms.paginator import (
     DescribeCustomKeyStoresPaginator,
     ListAliasesPaginator,
     ListGrantsPaginator,
     ListKeyPoliciesPaginator,
+    ListKeyRotationsPaginator,
     ListKeysPaginator,
     ListResourceTagsPaginator,
     ListRetirableGrantsPaginator,
 )
 
 client: KMSClient = Session().client("kms")
 
@@ -298,14 +299,15 @@
 # Types should be correctly discovered by mypy and IDEs
 describe_custom_key_stores_paginator: DescribeCustomKeyStoresPaginator = client.get_paginator(
     "describe_custom_key_stores"
 )
 list_aliases_paginator: ListAliasesPaginator = client.get_paginator("list_aliases")
 list_grants_paginator: ListGrantsPaginator = client.get_paginator("list_grants")
 list_key_policies_paginator: ListKeyPoliciesPaginator = client.get_paginator("list_key_policies")
+list_key_rotations_paginator: ListKeyRotationsPaginator = client.get_paginator("list_key_rotations")
 list_keys_paginator: ListKeysPaginator = client.get_paginator("list_keys")
 list_resource_tags_paginator: ListResourceTagsPaginator = client.get_paginator("list_resource_tags")
 list_retirable_grants_paginator: ListRetirableGrantsPaginator = client.get_paginator(
     "list_retirable_grants"
 )
 ```
```

### Comparing `mypy-boto3-kms-1.34.65/mypy_boto3_kms.egg-info/SOURCES.txt` & `mypy_boto3_kms-1.34.84/mypy_boto3_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kms-1.34.65/setup.py` & `mypy_boto3_kms-1.34.84/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kms",
-    version="1.34.65",
+    version="1.34.84",
     packages=["mypy_boto3_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.KMS 1.34.65 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.KMS 1.34.84 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

