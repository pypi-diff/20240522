# Comparing `tmp/mypy-boto3-chatbot-1.34.45.tar.gz` & `tmp/mypy-boto3-chatbot-1.34.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chatbot-1.34.45.tar", last modified: Mon Feb 19 20:21:45 2024, max compression
+gzip compressed data, was "mypy-boto3-chatbot-1.34.56.tar", last modified: Tue Mar  5 20:22:17 2024, max compression
```

## Comparing `mypy-boto3-chatbot-1.34.45.tar` & `mypy-boto3-chatbot-1.34.56.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.354639 mypy-boto3-chatbot-1.34.45/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-02-19 20:21:45.354639 mypy-boto3-chatbot-1.34.45/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.350639 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-02-19 20:21:27.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 20:21:45.354639 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-19 20:21:45.000000 mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 20:21:45.354639 mypy-boto3-chatbot-1.34.45/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-19 20:21:26.000000 mypy-boto3-chatbot-1.34.45/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:17.583457 mypy-boto3-chatbot-1.34.56/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-03-05 20:22:17.583457 mypy-boto3-chatbot-1.34.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:17.583457 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22446 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22443 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 20:22:17.583457 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12061 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-05 20:22:17.000000 mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 20:22:17.583457 mypy-boto3-chatbot-1.34.56/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-03-05 20:22:02.000000 mypy-boto3-chatbot-1.34.56/setup.py
```

### Comparing `mypy-boto3-chatbot-1.34.45/LICENSE` & `mypy-boto3-chatbot-1.34.56/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chatbot-1.34.45/PKG-INFO` & `mypy-boto3-chatbot-1.34.56/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chatbot
-Version: 1.34.45
-Summary: Type annotations for boto3.chatbot 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.56
+Summary: Type annotations for boto3.Chatbot 1.34.56 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chatbot.svg?color=blue)](https://pypi.org/project/mypy-boto3-chatbot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chatbot)](https://pepy.tech/project/mypy-boto3-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.chatbot 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[boto3.Chatbot 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chatbot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -96,21 +96,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `chatbot`.
+Click `Modify` and select `boto3 common` and `Chatbot`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `chatbot` service.
+Install `boto3-stubs` for `Chatbot` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -255,51 +255,51 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `boto3.client("chatbot")`.
+`ChatbotClient` provides annotations for `boto3.client("chatbot")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_chatbot import chatbotClient
+from mypy_boto3_chatbot import ChatbotClient
 
-client: chatbotClient = Session().client("chatbot")
+client: ChatbotClient = Session().client("chatbot")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_chatbot.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/literals/).
 
 ```python
-from mypy_boto3_chatbot.literals import chatbotServiceName
+from mypy_boto3_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_chatbot.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/type_defs/).
 
 ```python
 from mypy_boto3_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `mypy-boto3-chatbot-1.34.45/README.md` & `mypy-boto3-chatbot-1.34.56/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chatbot.svg?color=blue)](https://pypi.org/project/mypy-boto3-chatbot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chatbot)](https://pepy.tech/project/mypy-boto3-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.chatbot 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[boto3.Chatbot 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chatbot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -63,21 +63,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `chatbot`.
+Click `Modify` and select `boto3 common` and `Chatbot`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `chatbot` service.
+Install `boto3-stubs` for `Chatbot` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -222,51 +222,51 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `boto3.client("chatbot")`.
+`ChatbotClient` provides annotations for `boto3.client("chatbot")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_chatbot import chatbotClient
+from mypy_boto3_chatbot import ChatbotClient
 
-client: chatbotClient = Session().client("chatbot")
+client: ChatbotClient = Session().client("chatbot")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_chatbot.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/literals/).
 
 ```python
-from mypy_boto3_chatbot.literals import chatbotServiceName
+from mypy_boto3_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_chatbot.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/type_defs/).
 
 ```python
 from mypy_boto3_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/__main__.py` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.chatbot 1.34.45\n"
-        "Version:         1.34.45\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.Chatbot 1.34.56\n"
+        "Version:         1.34.56\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot//\n"
-        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot\n"
+        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.45")
+    print("1.34.56")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/client.py` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_chatbot.client import chatbotClient
+    from mypy_boto3_chatbot.client import ChatbotClient
 
     session = Session()
-    client: chatbotClient = session.client("chatbot")
+    client: ChatbotClient = session.client("chatbot")
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
@@ -33,15 +33,15 @@
     ListTeamsChannelConfigurationsResultTypeDef,
     UpdateAccountPreferencesResultTypeDef,
     UpdateChimeWebhookConfigurationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     UpdateTeamsChannelConfigurationResultTypeDef,
 )
 
-__all__ = ("chatbotClient",)
+__all__ = ("ChatbotClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
@@ -76,44 +76,44 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     UpdateAccountPreferencesException: Type[BotocoreClientError]
     UpdateChimeWebhookConfigurationException: Type[BotocoreClientError]
     UpdateSlackChannelConfigurationException: Type[BotocoreClientError]
     UpdateTeamsChannelConfigurationException: Type[BotocoreClientError]
 
 
-class chatbotClient(BaseClient):
+class ChatbotClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        chatbotClient exceptions.
+        ChatbotClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#can_paginate)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#close)
         """
 
     def create_chime_webhook_configuration(
         self,
         *,
         WebhookDescription: str,
@@ -123,15 +123,15 @@
         ConfigurationName: str,
         LoggingLevel: str = ...,
     ) -> CreateChimeWebhookConfigurationResultTypeDef:
         """
         Creates Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_chime_webhook_configuration)
         """
 
     def create_microsoft_teams_channel_configuration(
         self,
         *,
         ChannelId: str,
@@ -146,15 +146,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateTeamsChannelConfigurationResultTypeDef:
         """
         Creates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_microsoft_teams_channel_configuration)
         """
 
     def create_slack_channel_configuration(
         self,
         *,
         SlackTeamId: str,
@@ -167,209 +167,209 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateSlackChannelConfigurationResultTypeDef:
         """
         Creates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_slack_channel_configuration)
         """
 
     def delete_chime_webhook_configuration(self, *, ChatConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_chime_webhook_configuration)
         """
 
     def delete_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_channel_configuration)
         """
 
     def delete_microsoft_teams_configured_team(self, *, TeamId: str) -> Dict[str, Any]:
         """
         Deletes the Microsoft Teams team authorization allowing for channels to be
         configured in that Microsoft Teams
         team.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_configured_team)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_configured_team)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_configured_team)
         """
 
     def delete_microsoft_teams_user_identity(
         self, *, ChatConfigurationArn: str, UserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Teams user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_user_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_user_identity)
         """
 
     def delete_slack_channel_configuration(self, *, ChatConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_channel_configuration)
         """
 
     def delete_slack_user_identity(
         self, *, ChatConfigurationArn: str, SlackTeamId: str, SlackUserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Slack user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_user_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_user_identity)
         """
 
     def delete_slack_workspace_authorization(self, *, SlackTeamId: str) -> Dict[str, Any]:
         """
         Deletes the Slack workspace authorization that allows channels to be configured
         in that
         workspace.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_workspace_authorization)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_workspace_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_workspace_authorization)
         """
 
     def describe_chime_webhook_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeChimeWebhookConfigurationsResultTypeDef:
         """
         Lists Chime Webhook Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeChimeWebhookConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_chime_webhook_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_chime_webhook_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_chime_webhook_configurations)
         """
 
     def describe_slack_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeSlackChannelConfigurationsResultTypeDef:
         """
         Lists Slack Channel Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_channel_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_channel_configurations)
         """
 
     def describe_slack_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeSlackUserIdentitiesResultTypeDef:
         """
         Lists all Slack user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_user_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_user_identities)
         """
 
     def describe_slack_workspaces(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeSlackWorkspacesResultTypeDef:
         """
         Lists all authorized Slack Workspaces for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackWorkspaces).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_workspaces)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_workspaces)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#generate_presigned_url)
         """
 
     def get_account_preferences(self) -> GetAccountPreferencesResultTypeDef:
         """
         Get Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_account_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#get_account_preferences)
         """
 
     def get_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> GetTeamsChannelConfigurationResultTypeDef:
         """
         Get a single MS Teams Channel Configurations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#get_microsoft_teams_channel_configuration)
         """
 
     def list_microsoft_teams_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., TeamId: str = ...
     ) -> ListTeamsChannelConfigurationsResultTypeDef:
         """
         Lists MS Teams Channel Configurations optionally filtered by TeamId See also:
         [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_channel_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_channel_configurations)
         """
 
     def list_microsoft_teams_configured_teams(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMicrosoftTeamsConfiguredTeamsResultTypeDef:
         """
         Lists all authorized MS teams for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsConfiguredTeams).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_configured_teams)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_configured_teams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_configured_teams)
         """
 
     def list_microsoft_teams_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListMicrosoftTeamsUserIdentitiesResultTypeDef:
         """
         Lists all Microsoft Teams user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_user_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_user_identities)
         """
 
     def update_account_preferences(
         self, *, UserAuthorizationRequired: bool = ..., TrainingDataCollectionEnabled: bool = ...
     ) -> UpdateAccountPreferencesResultTypeDef:
         """
         Update Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_account_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_account_preferences)
         """
 
     def update_chime_webhook_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -379,15 +379,15 @@
         IamRoleArn: str = ...,
         LoggingLevel: str = ...,
     ) -> UpdateChimeWebhookConfigurationResultTypeDef:
         """
         Updates a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_chime_webhook_configuration)
         """
 
     def update_microsoft_teams_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -399,15 +399,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateTeamsChannelConfigurationResultTypeDef:
         """
         Updates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_microsoft_teams_channel_configuration)
         """
 
     def update_slack_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -419,10 +419,10 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_slack_channel_configuration)
         """
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/client.pyi` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/)
 
 Usage::
 
     ```python
     from boto3.session import Session
-    from mypy_boto3_chatbot.client import chatbotClient
+    from mypy_boto3_chatbot.client import ChatbotClient
 
     session = Session()
-    client: chatbotClient = session.client("chatbot")
+    client: ChatbotClient = session.client("chatbot")
     ```
 """
 
 from typing import Any, Dict, Mapping, Sequence, Type
 
 from botocore.client import BaseClient, ClientMeta
 
@@ -33,15 +33,15 @@
     ListTeamsChannelConfigurationsResultTypeDef,
     UpdateAccountPreferencesResultTypeDef,
     UpdateChimeWebhookConfigurationResultTypeDef,
     UpdateSlackChannelConfigurationResultTypeDef,
     UpdateTeamsChannelConfigurationResultTypeDef,
 )
 
-__all__ = ("chatbotClient",)
+__all__ = ("ChatbotClient",)
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
@@ -73,44 +73,44 @@
     ListTeamsChannelConfigurationsException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     UpdateAccountPreferencesException: Type[BotocoreClientError]
     UpdateChimeWebhookConfigurationException: Type[BotocoreClientError]
     UpdateSlackChannelConfigurationException: Type[BotocoreClientError]
     UpdateTeamsChannelConfigurationException: Type[BotocoreClientError]
 
-class chatbotClient(BaseClient):
+class ChatbotClient(BaseClient):
     """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client)
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/)
     """
 
     meta: ClientMeta
 
     @property
     def exceptions(self) -> Exceptions:
         """
-        chatbotClient exceptions.
+        ChatbotClient exceptions.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.exceptions)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.exceptions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#exceptions)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.can_paginate)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#can_paginate)
         """
 
     def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.close)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#close)
         """
 
     def create_chime_webhook_configuration(
         self,
         *,
         WebhookDescription: str,
@@ -120,15 +120,15 @@
         ConfigurationName: str,
         LoggingLevel: str = ...,
     ) -> CreateChimeWebhookConfigurationResultTypeDef:
         """
         Creates Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_chime_webhook_configuration)
         """
 
     def create_microsoft_teams_channel_configuration(
         self,
         *,
         ChannelId: str,
@@ -143,15 +143,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateTeamsChannelConfigurationResultTypeDef:
         """
         Creates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_microsoft_teams_channel_configuration)
         """
 
     def create_slack_channel_configuration(
         self,
         *,
         SlackTeamId: str,
@@ -164,209 +164,209 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> CreateSlackChannelConfigurationResultTypeDef:
         """
         Creates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/CreateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.create_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.create_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#create_slack_channel_configuration)
         """
 
     def delete_chime_webhook_configuration(self, *, ChatConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_chime_webhook_configuration)
         """
 
     def delete_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> Dict[str, Any]:
         """
         Deletes MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_channel_configuration)
         """
 
     def delete_microsoft_teams_configured_team(self, *, TeamId: str) -> Dict[str, Any]:
         """
         Deletes the Microsoft Teams team authorization allowing for channels to be
         configured in that Microsoft Teams
         team.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_configured_team)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_configured_team)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_configured_team)
         """
 
     def delete_microsoft_teams_user_identity(
         self, *, ChatConfigurationArn: str, UserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Teams user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteMicrosoftTeamsUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_microsoft_teams_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_microsoft_teams_user_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_microsoft_teams_user_identity)
         """
 
     def delete_slack_channel_configuration(self, *, ChatConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_channel_configuration)
         """
 
     def delete_slack_user_identity(
         self, *, ChatConfigurationArn: str, SlackTeamId: str, SlackUserId: str
     ) -> Dict[str, Any]:
         """
         Deletes a Slack user identity See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DeleteSlackUserIdentity).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_user_identity)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_user_identity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_user_identity)
         """
 
     def delete_slack_workspace_authorization(self, *, SlackTeamId: str) -> Dict[str, Any]:
         """
         Deletes the Slack workspace authorization that allows channels to be configured
         in that
         workspace.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.delete_slack_workspace_authorization)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.delete_slack_workspace_authorization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#delete_slack_workspace_authorization)
         """
 
     def describe_chime_webhook_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeChimeWebhookConfigurationsResultTypeDef:
         """
         Lists Chime Webhook Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeChimeWebhookConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_chime_webhook_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_chime_webhook_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_chime_webhook_configurations)
         """
 
     def describe_slack_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., ChatConfigurationArn: str = ...
     ) -> DescribeSlackChannelConfigurationsResultTypeDef:
         """
         Lists Slack Channel Configurations optionally filtered by ChatConfigurationArn
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_channel_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_channel_configurations)
         """
 
     def describe_slack_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> DescribeSlackUserIdentitiesResultTypeDef:
         """
         Lists all Slack user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_user_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_user_identities)
         """
 
     def describe_slack_workspaces(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> DescribeSlackWorkspacesResultTypeDef:
         """
         Lists all authorized Slack Workspaces for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/DescribeSlackWorkspaces).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.describe_slack_workspaces)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.describe_slack_workspaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#describe_slack_workspaces)
         """
 
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.generate_presigned_url)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#generate_presigned_url)
         """
 
     def get_account_preferences(self) -> GetAccountPreferencesResultTypeDef:
         """
         Get Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_account_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#get_account_preferences)
         """
 
     def get_microsoft_teams_channel_configuration(
         self, *, ChatConfigurationArn: str
     ) -> GetTeamsChannelConfigurationResultTypeDef:
         """
         Get a single MS Teams Channel Configurations See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/GetMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.get_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.get_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#get_microsoft_teams_channel_configuration)
         """
 
     def list_microsoft_teams_channel_configurations(
         self, *, MaxResults: int = ..., NextToken: str = ..., TeamId: str = ...
     ) -> ListTeamsChannelConfigurationsResultTypeDef:
         """
         Lists MS Teams Channel Configurations optionally filtered by TeamId See also:
         [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsChannelConfigurations).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_channel_configurations)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_channel_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_channel_configurations)
         """
 
     def list_microsoft_teams_configured_teams(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListMicrosoftTeamsConfiguredTeamsResultTypeDef:
         """
         Lists all authorized MS teams for AWS Account See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/ListMicrosoftTeamsConfiguredTeams).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_configured_teams)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_configured_teams)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_configured_teams)
         """
 
     def list_microsoft_teams_user_identities(
         self, *, ChatConfigurationArn: str = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListMicrosoftTeamsUserIdentitiesResultTypeDef:
         """
         Lists all Microsoft Teams user identities with a mapped role.
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.list_microsoft_teams_user_identities)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.list_microsoft_teams_user_identities)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#list_microsoft_teams_user_identities)
         """
 
     def update_account_preferences(
         self, *, UserAuthorizationRequired: bool = ..., TrainingDataCollectionEnabled: bool = ...
     ) -> UpdateAccountPreferencesResultTypeDef:
         """
         Update Chatbot account level preferences See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateAccountPreferences).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_account_preferences)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_account_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_account_preferences)
         """
 
     def update_chime_webhook_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -376,15 +376,15 @@
         IamRoleArn: str = ...,
         LoggingLevel: str = ...,
     ) -> UpdateChimeWebhookConfigurationResultTypeDef:
         """
         Updates a Chime Webhook Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateChimeWebhookConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_chime_webhook_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_chime_webhook_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_chime_webhook_configuration)
         """
 
     def update_microsoft_teams_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -396,15 +396,15 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateTeamsChannelConfigurationResultTypeDef:
         """
         Updates MS Teams Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateMicrosoftTeamsChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_microsoft_teams_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_microsoft_teams_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_microsoft_teams_channel_configuration)
         """
 
     def update_slack_channel_configuration(
         self,
         *,
         ChatConfigurationArn: str,
@@ -416,10 +416,10 @@
         GuardrailPolicyArns: Sequence[str] = ...,
         UserAuthorizationRequired: bool = ...,
     ) -> UpdateSlackChannelConfigurationResultTypeDef:
         """
         Updates Slack Channel Configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/chatbot-2017-10-11/UpdateSlackChannelConfiguration).
 
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot.Client.update_slack_channel_configuration)
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot.Client.update_slack_channel_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/client/#update_slack_channel_configuration)
         """
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/literals.py` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/literals.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Type annotations for chatbot service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chatbot.literals import chatbotServiceName
+    from mypy_boto3_chatbot.literals import ChatbotServiceName
 
-    data: chatbotServiceName = "chatbot"
+    data: ChatbotServiceName = "chatbot"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("chatbotServiceName", "ServiceName", "ResourceServiceName")
+__all__ = ("ChatbotServiceName", "ServiceName", "ResourceServiceName")
 
-chatbotServiceName = Literal["chatbot"]
+ChatbotServiceName = Literal["chatbot"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/literals.pyi` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Type annotations for chatbot service literal definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/literals/)
 
 Usage::
 
     ```python
-    from mypy_boto3_chatbot.literals import chatbotServiceName
+    from mypy_boto3_chatbot.literals import ChatbotServiceName
 
-    data: chatbotServiceName = "chatbot"
+    data: ChatbotServiceName = "chatbot"
     ```
 """
 
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-__all__ = ("chatbotServiceName", "ServiceName", "ResourceServiceName")
+__all__ = ("ChatbotServiceName", "ServiceName", "ResourceServiceName")
 
-chatbotServiceName = Literal["chatbot"]
+ChatbotServiceName = Literal["chatbot"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
     "amp",
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/type_defs.py` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,18 @@
         "LoggingLevel": NotRequired[str],
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
 CreateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "CreateSlackChannelConfigurationRequestRequestTypeDef",
     {
         "SlackTeamId": str,
         "SlackChannelId": str,
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot/type_defs.pyi` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,18 @@
         "LoggingLevel": NotRequired[str],
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
 CreateSlackChannelConfigurationRequestRequestTypeDef = TypedDict(
     "CreateSlackChannelConfigurationRequestRequestTypeDef",
     {
         "SlackTeamId": str,
         "SlackChannelId": str,
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/PKG-INFO` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chatbot
-Version: 1.34.45
-Summary: Type annotations for boto3.chatbot 1.34.45 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.56
+Summary: Type annotations for boto3.Chatbot 1.34.56 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chatbot.svg?color=blue)](https://pypi.org/project/mypy-boto3-chatbot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-chatbot)](https://pepy.tech/project/mypy-boto3-chatbot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.chatbot 1.34.45](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot)
+[boto3.Chatbot 1.34.56](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#Chatbot)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chatbot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -96,21 +96,21 @@
 
 ### VSCode extension
 
 Add
 [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
 extension to your VSCode and run `AWS boto3: Quick Start` command.
 
-Click `Modify` and select `boto3 common` and `chatbot`.
+Click `Modify` and select `boto3 common` and `Chatbot`.
 
 <a id="from-pypi-with-pip"></a>
 
 ### From PyPI with pip
 
-Install `boto3-stubs` for `chatbot` service.
+Install `boto3-stubs` for `Chatbot` service.
 
 ```bash
 # install with boto3 type annotations
 python -m pip install 'boto3-stubs[chatbot]'
 
 
 # Lite version does not provide session.client/resource overloads
@@ -255,51 +255,51 @@
 
 ## Explicit type annotations
 
 <a id="client-annotations"></a>
 
 ### Client annotations
 
-`chatbotClient` provides annotations for `boto3.client("chatbot")`.
+`ChatbotClient` provides annotations for `boto3.client("chatbot")`.
 
 ```python
 from boto3.session import Session
 
-from mypy_boto3_chatbot import chatbotClient
+from mypy_boto3_chatbot import ChatbotClient
 
-client: chatbotClient = Session().client("chatbot")
+client: ChatbotClient = Session().client("chatbot")
 
 # now client usage is checked by mypy and IDE should provide code completion
 ```
 
 <a id="literals"></a>
 
 ### Literals
 
 `mypy_boto3_chatbot.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
-Full list of `chatbot` Literals can be found in
+Full list of `Chatbot` Literals can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/literals/).
 
 ```python
-from mypy_boto3_chatbot.literals import chatbotServiceName
+from mypy_boto3_chatbot.literals import ChatbotServiceName
 
 
-def check_value(value: chatbotServiceName) -> bool: ...
+def check_value(value: ChatbotServiceName) -> bool: ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `mypy_boto3_chatbot.type_defs` module contains structures and shapes assembled
 to typed dictionaries and unions for additional type checking.
 
-Full list of `chatbot` TypeDefs can be found in
+Full list of `Chatbot` TypeDefs can be found in
 [docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chatbot/type_defs/).
 
 ```python
 from mypy_boto3_chatbot.type_defs import AccountPreferencesTypeDef
 
 
 def get_value() -> AccountPreferencesTypeDef:
```

### Comparing `mypy-boto3-chatbot-1.34.45/mypy_boto3_chatbot.egg-info/SOURCES.txt` & `mypy-boto3-chatbot-1.34.56/mypy_boto3_chatbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chatbot-1.34.45/setup.py` & `mypy-boto3-chatbot-1.34.56/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chatbot",
-    version="1.34.45",
+    version="1.34.56",
     packages=["mypy_boto3_chatbot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.chatbot 1.34.45 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.Chatbot 1.34.56 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

