# Comparing `tmp/mypy-boto3-opensearch-1.34.43.tar.gz` & `tmp/mypy_boto3_opensearch-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.34.43.tar", last modified: Thu Feb 15 20:47:29 2024, max compression
+gzip compressed data, was "mypy_boto3_opensearch-1.34.95.tar", last modified: Tue Apr 30 19:34:52 2024, max compression
```

## Comparing `mypy-boto3-opensearch-1.34.43.tar` & `mypy_boto3_opensearch-1.34.95.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.757509 mypy-boto3-opensearch-1.34.43/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-02-15 20:47:29.757509 mypy-boto3-opensearch-1.34.43/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.757509 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46642 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46639 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    17240 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    70806 2024-02-15 20:46:56.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    70806 2024-02-15 20:46:56.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 20:47:29.757509 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-15 20:47:29.000000 mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 20:47:29.757509 mypy-boto3-opensearch-1.34.43/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-15 20:46:55.000000 mypy-boto3-opensearch-1.34.43/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.819045 mypy_boto3_opensearch-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-30 19:34:52.819045 mypy_boto3_opensearch-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10723 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.819045 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46652 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46649 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-04-30 19:32:14.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17344 2024-04-30 19:32:14.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    71930 2024-04-30 19:32:15.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71930 2024-04-30 19:32:15.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:32:13.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:52.819045 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12297 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:34:52.000000 mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:52.819045 mypy_boto3_opensearch-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-30 19:32:12.000000 mypy_boto3_opensearch-1.34.95/setup.py
```

### Comparing `mypy-boto3-opensearch-1.34.43/LICENSE` & `mypy_boto3_opensearch-1.34.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.34.43/PKG-INFO` & `mypy_boto3_opensearch-1.34.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.34.43
-Summary: Type annotations for boto3.OpenSearchService 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.95
+Summary: Type annotations for boto3.OpenSearchService 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.34.43/README.md` & `mypy_boto3_opensearch-1.34.95/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/__main__.py` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.34.43\n"
-        "Version:         1.34.43\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.OpenSearchService 1.34.95\n"
+        "Version:         1.34.95\n"
+        "Builder version: 7.24.0\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.43")
+    print("1.34.95")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/client.py` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AddDataSourceResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelDomainConfigChangeResponseTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
@@ -874,15 +874,15 @@
         AccessPolicies: str = ...,
         IPAddressType: IPAddressTypeType = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/client.pyi` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 from .type_defs import (
     AcceptInboundConnectionResponseTypeDef,
     AddDataSourceResponseTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
     AssociatePackageResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     AutoTuneOptionsInputTypeDef,
-    AutoTuneOptionsTypeDef,
+    AutoTuneOptionsUnionTypeDef,
     CancelDomainConfigChangeResponseTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsTypeDef,
     ConnectionPropertiesTypeDef,
     CreateDomainResponseTypeDef,
     CreateOutboundConnectionResponseTypeDef,
@@ -871,15 +871,15 @@
         AccessPolicies: str = ...,
         IPAddressType: IPAddressTypeType = ...,
         LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,
         EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,
         DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,
         NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,
         AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,
-        AutoTuneOptions: AutoTuneOptionsTypeDef = ...,
+        AutoTuneOptions: AutoTuneOptionsUnionTypeDef = ...,
         DryRun: bool = ...,
         DryRunMode: DryRunModeType = ...,
         OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,
         SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,
     ) -> UpdateDomainConfigResponseTypeDef:
         """
         Modifies the cluster configuration of the specified Amazon OpenSearch Service
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/literals.py` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -365,14 +366,15 @@
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
@@ -385,24 +387,26 @@
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
@@ -463,15 +467,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -600,14 +603,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -651,14 +655,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/literals.pyi` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -340,14 +340,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -365,14 +366,15 @@
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
@@ -385,24 +387,26 @@
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
@@ -463,15 +467,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -600,14 +603,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -651,14 +655,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/type_defs.py` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     "IPAddressTypeStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelDomainConfigChangeResponseTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
@@ -251,14 +252,15 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -288,14 +290,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
@@ -325,18 +328,18 @@
         "ConnectionId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 OptionStatusTypeDef = TypedDict(
     "OptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
@@ -1162,16 +1165,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVersionsResponseTypeDef = TypedDict(
     "ListVersionsResponseTypeDef",
     {
         "Versions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
     "PurchaseReservedInstanceOfferingResponseTypeDef",
     {
         "ReservedInstanceId": str,
         "ReservationName": str,
@@ -1251,14 +1254,22 @@
 )
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": NotRequired[ScheduledAutoTuneDetailsTypeDef],
     },
 )
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": NotRequired[datetime],
+        "Duration": NotRequired[DurationTypeDef],
+        "CronExpressionForRecurrence": NotRequired[str],
+    },
+)
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": NotRequired[TimestampTypeDef],
         "Duration": NotRequired[DurationTypeDef],
         "CronExpressionForRecurrence": NotRequired[str],
     },
@@ -1506,16 +1517,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainMaintenancesResponseTypeDef = TypedDict(
     "ListDomainMaintenancesResponseTypeDef",
     {
         "DomainMaintenances": List[DomainMaintenanceDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": NotRequired[str],
         "PackageName": NotRequired[str],
@@ -1562,24 +1573,24 @@
         "InstanceCountLimits": NotRequired[InstanceCountLimitsTypeDef],
     },
 )
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1700,28 +1711,37 @@
 AutoTuneTypeDef = TypedDict(
     "AutoTuneTypeDef",
     {
         "AutoTuneType": NotRequired[Literal["SCHEDULED_ACTION"]],
         "AutoTuneDetails": NotRequired[AutoTuneDetailsTypeDef],
     },
 )
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": NotRequired[AutoTuneDesiredStateType],
+        "RollbackOnDisable": NotRequired[RollbackOnDisableType],
+        "MaintenanceSchedules": NotRequired[List[AutoTuneMaintenanceScheduleOutputTypeDef]],
+        "UseOffPeakWindow": NotRequired[bool],
+    },
+)
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": NotRequired[AutoTuneDesiredStateType],
         "MaintenanceSchedules": NotRequired[Sequence[AutoTuneMaintenanceScheduleTypeDef]],
         "UseOffPeakWindow": NotRequired[bool],
     },
 )
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": NotRequired[AutoTuneDesiredStateType],
         "RollbackOnDisable": NotRequired[RollbackOnDisableType],
-        "MaintenanceSchedules": NotRequired[List[AutoTuneMaintenanceScheduleTypeDef]],
+        "MaintenanceSchedules": NotRequired[Sequence[AutoTuneMaintenanceScheduleTypeDef]],
         "UseOffPeakWindow": NotRequired[bool],
     },
 )
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
     {
         "DomainState": DomainStateType,
@@ -1838,24 +1858,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1897,48 +1917,48 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
-        "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
-        "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "InternalUserDatabaseEnabled": NotRequired[bool],
@@ -1965,16 +1985,16 @@
         "AdditionalLimits": NotRequired[List[AdditionalLimitTypeDef]],
     },
 )
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1987,53 +2007,54 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": NotRequired[AutoTuneOptionsTypeDef],
+        "Options": NotRequired[AutoTuneOptionsExtraOutputTypeDef],
         "Status": NotRequired[AutoTuneStatusTypeDef],
     },
 )
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "DataSources": List[DataSourceDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2109,14 +2130,15 @@
         "ARN": str,
         "ClusterConfig": ClusterConfigTypeDef,
         "Created": NotRequired[bool],
         "Deleted": NotRequired[bool],
         "Endpoint": NotRequired[str],
         "EndpointV2": NotRequired[str],
         "Endpoints": NotRequired[Dict[str, str]],
+        "DomainEndpointV2HostedZoneId": NotRequired[str],
         "Processing": NotRequired[bool],
         "UpgradeProcessing": NotRequired[bool],
         "EngineVersion": NotRequired[str],
         "EBSOptions": NotRequired[EBSOptionsTypeDef],
         "AccessPolicies": NotRequired[str],
         "IPAddressType": NotRequired[IPAddressTypeType],
         "SnapshotOptions": NotRequired[SnapshotOptionsTypeDef],
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch/type_defs.pyi` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -200,14 +200,15 @@
     "IPAddressTypeStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelDomainConfigChangeResponseTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
@@ -251,14 +252,15 @@
     "ReservedInstanceTypeDef",
     "SAMLOptionsInputTypeDef",
     "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
+    "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
     "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
@@ -288,14 +290,15 @@
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
+    "AutoTuneOptionsUnionTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
     "AdvancedSecurityOptionsStatusTypeDef",
@@ -325,18 +328,18 @@
         "ConnectionId": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 OptionStatusTypeDef = TypedDict(
     "OptionStatusTypeDef",
     {
         "CreationDate": datetime,
         "UpdateDate": datetime,
@@ -1162,16 +1165,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListVersionsResponseTypeDef = TypedDict(
     "ListVersionsResponseTypeDef",
     {
         "Versions": List[str],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 PurchaseReservedInstanceOfferingResponseTypeDef = TypedDict(
     "PurchaseReservedInstanceOfferingResponseTypeDef",
     {
         "ReservedInstanceId": str,
         "ReservationName": str,
@@ -1251,14 +1254,22 @@
 )
 AutoTuneDetailsTypeDef = TypedDict(
     "AutoTuneDetailsTypeDef",
     {
         "ScheduledAutoTuneDetails": NotRequired[ScheduledAutoTuneDetailsTypeDef],
     },
 )
+AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
+    "AutoTuneMaintenanceScheduleOutputTypeDef",
+    {
+        "StartAt": NotRequired[datetime],
+        "Duration": NotRequired[DurationTypeDef],
+        "CronExpressionForRecurrence": NotRequired[str],
+    },
+)
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
     {
         "StartAt": NotRequired[TimestampTypeDef],
         "Duration": NotRequired[DurationTypeDef],
         "CronExpressionForRecurrence": NotRequired[str],
     },
@@ -1506,16 +1517,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainMaintenancesResponseTypeDef = TypedDict(
     "ListDomainMaintenancesResponseTypeDef",
     {
         "DomainMaintenances": List[DomainMaintenanceDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DomainPackageDetailsTypeDef = TypedDict(
     "DomainPackageDetailsTypeDef",
     {
         "PackageID": NotRequired[str],
         "PackageName": NotRequired[str],
@@ -1562,24 +1573,24 @@
         "InstanceCountLimits": NotRequired[InstanceCountLimitsTypeDef],
     },
 )
 ListInstanceTypeDetailsResponseTypeDef = TypedDict(
     "ListInstanceTypeDetailsResponseTypeDef",
     {
         "InstanceTypeDetails": List[InstanceTypeDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListScheduledActionsResponseTypeDef = TypedDict(
     "ListScheduledActionsResponseTypeDef",
     {
         "ScheduledActions": List[ScheduledActionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateScheduledActionResponseTypeDef = TypedDict(
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1700,28 +1711,37 @@
 AutoTuneTypeDef = TypedDict(
     "AutoTuneTypeDef",
     {
         "AutoTuneType": NotRequired[Literal["SCHEDULED_ACTION"]],
         "AutoTuneDetails": NotRequired[AutoTuneDetailsTypeDef],
     },
 )
+AutoTuneOptionsExtraOutputTypeDef = TypedDict(
+    "AutoTuneOptionsExtraOutputTypeDef",
+    {
+        "DesiredState": NotRequired[AutoTuneDesiredStateType],
+        "RollbackOnDisable": NotRequired[RollbackOnDisableType],
+        "MaintenanceSchedules": NotRequired[List[AutoTuneMaintenanceScheduleOutputTypeDef]],
+        "UseOffPeakWindow": NotRequired[bool],
+    },
+)
 AutoTuneOptionsInputTypeDef = TypedDict(
     "AutoTuneOptionsInputTypeDef",
     {
         "DesiredState": NotRequired[AutoTuneDesiredStateType],
         "MaintenanceSchedules": NotRequired[Sequence[AutoTuneMaintenanceScheduleTypeDef]],
         "UseOffPeakWindow": NotRequired[bool],
     },
 )
 AutoTuneOptionsTypeDef = TypedDict(
     "AutoTuneOptionsTypeDef",
     {
         "DesiredState": NotRequired[AutoTuneDesiredStateType],
         "RollbackOnDisable": NotRequired[RollbackOnDisableType],
-        "MaintenanceSchedules": NotRequired[List[AutoTuneMaintenanceScheduleTypeDef]],
+        "MaintenanceSchedules": NotRequired[Sequence[AutoTuneMaintenanceScheduleTypeDef]],
         "UseOffPeakWindow": NotRequired[bool],
     },
 )
 DescribeDomainHealthResponseTypeDef = TypedDict(
     "DescribeDomainHealthResponseTypeDef",
     {
         "DomainState": DomainStateType,
@@ -1838,24 +1858,24 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDomainsForPackageResponseTypeDef = TypedDict(
     "ListDomainsForPackageResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListPackagesForDomainResponseTypeDef = TypedDict(
     "ListPackagesForDomainResponseTypeDef",
     {
         "DomainPackageDetailsList": List[DomainPackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateVpcEndpointResponseTypeDef = TypedDict(
     "CreateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1897,48 +1917,48 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribePackagesResponseTypeDef = TypedDict(
     "DescribePackagesResponseTypeDef",
     {
         "PackageDetailsList": List[PackageDetailsTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdatePackageResponseTypeDef = TypedDict(
     "UpdatePackageResponseTypeDef",
     {
         "PackageDetails": PackageDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 GetPackageVersionHistoryResponseTypeDef = TypedDict(
     "GetPackageVersionHistoryResponseTypeDef",
     {
         "PackageID": str,
         "PackageVersionHistoryList": List[PackageVersionHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstanceOfferingsResponseTypeDef = TypedDict(
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     {
-        "NextToken": str,
         "ReservedInstanceOfferings": List[ReservedInstanceOfferingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeReservedInstancesResponseTypeDef = TypedDict(
     "DescribeReservedInstancesResponseTypeDef",
     {
-        "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AdvancedSecurityOptionsInputTypeDef = TypedDict(
     "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "InternalUserDatabaseEnabled": NotRequired[bool],
@@ -1965,16 +1985,16 @@
         "AdditionalLimits": NotRequired[List[AdditionalLimitTypeDef]],
     },
 )
 GetUpgradeHistoryResponseTypeDef = TypedDict(
     "GetUpgradeHistoryResponseTypeDef",
     {
         "UpgradeHistories": List[UpgradeHistoryTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AcceptInboundConnectionResponseTypeDef = TypedDict(
     "AcceptInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1987,53 +2007,54 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeInboundConnectionsResponseTypeDef = TypedDict(
     "DescribeInboundConnectionsResponseTypeDef",
     {
         "Connections": List[InboundConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RejectInboundConnectionResponseTypeDef = TypedDict(
     "RejectInboundConnectionResponseTypeDef",
     {
         "Connection": InboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeDomainAutoTunesResponseTypeDef = TypedDict(
     "DescribeDomainAutoTunesResponseTypeDef",
     {
         "AutoTunes": List[AutoTuneTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 AutoTuneOptionsStatusTypeDef = TypedDict(
     "AutoTuneOptionsStatusTypeDef",
     {
-        "Options": NotRequired[AutoTuneOptionsTypeDef],
+        "Options": NotRequired[AutoTuneOptionsExtraOutputTypeDef],
         "Status": NotRequired[AutoTuneStatusTypeDef],
     },
 )
+AutoTuneOptionsUnionTypeDef = Union[AutoTuneOptionsTypeDef, AutoTuneOptionsExtraOutputTypeDef]
 DeleteOutboundConnectionResponseTypeDef = TypedDict(
     "DeleteOutboundConnectionResponseTypeDef",
     {
         "Connection": OutboundConnectionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeOutboundConnectionsResponseTypeDef = TypedDict(
     "DescribeOutboundConnectionsResponseTypeDef",
     {
         "Connections": List[OutboundConnectionTypeDef],
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "DataSources": List[DataSourceDetailsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2109,14 +2130,15 @@
         "ARN": str,
         "ClusterConfig": ClusterConfigTypeDef,
         "Created": NotRequired[bool],
         "Deleted": NotRequired[bool],
         "Endpoint": NotRequired[str],
         "EndpointV2": NotRequired[str],
         "Endpoints": NotRequired[Dict[str, str]],
+        "DomainEndpointV2HostedZoneId": NotRequired[str],
         "Processing": NotRequired[bool],
         "UpgradeProcessing": NotRequired[bool],
         "EngineVersion": NotRequired[str],
         "EBSOptions": NotRequired[EBSOptionsTypeDef],
         "AccessPolicies": NotRequired[str],
         "IPAddressType": NotRequired[IPAddressTypeType],
         "SnapshotOptions": NotRequired[SnapshotOptionsTypeDef],
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.34.43
-Summary: Type annotations for boto3.OpenSearchService 1.34.43 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.95
+Summary: Type annotations for boto3.OpenSearchService 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.34.43](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-opensearch-1.34.43/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy_boto3_opensearch-1.34.95/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.34.43/setup.py` & `mypy_boto3_opensearch-1.34.95/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.34.43",
+    version="1.34.95",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.OpenSearchService 1.34.43 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.OpenSearchService 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

