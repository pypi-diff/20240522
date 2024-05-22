# Comparing `tmp/sdkfabric_discord-0.2.4.tar.gz` & `tmp/sdkfabric_discord-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_discord-0.2.4.tar", last modified: Sun May 19 21:33:53 2024, max compression
+gzip compressed data, was "sdkfabric_discord-0.2.5.tar", last modified: Wed May 22 21:47:01 2024, max compression
```

## Comparing `sdkfabric_discord-0.2.4.tar` & `sdkfabric_discord-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:33:53.615944 sdkfabric_discord-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 21:33:53.615944 sdkfabric_discord-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 21:33:50.000000 sdkfabric_discord-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:33:53.615944 sdkfabric_discord-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:33:53.611944 sdkfabric_discord-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:33:53.615944 sdkfabric_discord-0.2.4/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/channel_message_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/channel_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/message_allowed_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/message_embed.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-19 21:33:49.000000 sdkfabric_discord-0.2.4/src/sdk/message_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 21:33:53.615944 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-19 21:33:53.000000 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-19 21:33:53.000000 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 21:33:53.000000 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 21:33:53.000000 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 21:33:53.000000 sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:47:01.497310 sdkfabric_discord-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 21:47:01.497310 sdkfabric_discord-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:47:01.497310 sdkfabric_discord-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:47:01.493310 sdkfabric_discord-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:47:01.497310 sdkfabric_discord-0.2.5/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7495 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/channel_message_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/channel_reaction_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/channel_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/message_allowed_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/message_embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/message_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-22 21:46:57.000000 sdkfabric_discord-0.2.5/src/sdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:47:01.497310 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-22 21:47:01.000000 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-22 21:47:01.000000 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:47:01.000000 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 21:47:01.000000 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 21:47:01.000000 sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/top_level.txt
```

### Comparing `sdkfabric_discord-0.2.4/LICENSE` & `sdkfabric_discord-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/PKG-INFO` & `sdkfabric_discord-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.2.4
+Version: 0.2.5
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_discord-0.2.4/README.md` & `sdkfabric_discord-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/pyproject.toml` & `sdkfabric_discord-0.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-discord"
-version = "0.2.4"
+version = "0.2.5"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Discord Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_discord-0.2.4/src/sdk/channel.py` & `sdkfabric_discord-0.2.5/src/sdk/channel.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdk/channel_message_tag.py` & `sdkfabric_discord-0.2.5/src/sdk/channel_message_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdk/channel_tag.py` & `sdkfabric_discord-0.2.5/src/sdk/channel_tag.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,33 @@
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .channel import Channel
 from .channel_message_tag import ChannelMessageTag
+from .channel_reaction_tag import ChannelReactionTag
 from .message import Message
 
 class ChannelTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
     def message(self) -> ChannelMessageTag:
         return ChannelMessageTag(
             self.http_client,
             self.parser
         )
 
+    def reaction(self) -> ChannelReactionTag:
+        return ChannelReactionTag(
+            self.http_client,
+            self.parser
+        )
+
 
     def get(self, channel_id: str) -> Channel:
         """
         Get a channel by ID. Returns a channel object.
         """
         try:
             path_params = {}
```

### Comparing `sdkfabric_discord-0.2.4/src/sdk/client.py` & `sdkfabric_discord-0.2.5/src/sdk/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,10 +19,10 @@
             self.http_client,
             self.parser
         )
 
 
 
     @staticmethod
-    def build(clientId: str, clientSecret: str, tokenStore: sdkgen.TokenStoreInterface, scopes: List[str]):
-        return Client("https://discord.com/api/v10", sdkgen.OAuth2(clientId, clientSecret, "https://discord.com/api/oauth2/token", "https://discord.com/oauth2/authorize", tokenStore, scopes))
+    def build(token: str):
+        return Client("https://discord.com/api/v10", sdkgen.HttpBearer(token))
```

### Comparing `sdkfabric_discord-0.2.4/src/sdk/message.py` & `sdkfabric_discord-0.2.5/src/sdk/message.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdk/message_allowed_mentions.py` & `sdkfabric_discord-0.2.5/src/sdk/message_allowed_mentions.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdk/message_embed.py` & `sdkfabric_discord-0.2.5/src/sdk/message_embed.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdk/message_reference.py` & `sdkfabric_discord-0.2.5/src/sdk/message_reference.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_discord-0.2.4/src/sdkfabric_discord.egg-info/PKG-INFO` & `sdkfabric_discord-0.2.5/src/sdkfabric_discord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-discord
-Version: 0.2.4
+Version: 0.2.5
 Summary: Discord Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/discord-python
 Project-URL: Issues, https://github.com/sdk-fabric/discord-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

