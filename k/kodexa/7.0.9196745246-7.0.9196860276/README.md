# Comparing `tmp/kodexa-7.0.9196745246.tar.gz` & `tmp/kodexa-7.0.9196860276.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9196745246.tar", max compression
+gzip compressed data, was "kodexa-7.0.9196860276.tar", max compression
```

## Comparing `kodexa-7.0.9196745246.tar` & `kodexa-7.0.9196860276.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-22 18:44:12.918826 kodexa-7.0.9196745246/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-22 18:44:12.918826 kodexa-7.0.9196745246/README.md
--rw-r--r--   0        0        0      957 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/model.py
--rw-r--r--   0        0        0   174335 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   218016 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1373 2024-05-22 18:44:29.730774 kodexa-7.0.9196745246/pyproject.toml
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9196745246/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:54:32.698099 kodexa-7.0.9196860276/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-22 18:54:32.698099 kodexa-7.0.9196860276/README.md
+-rw-r--r--   0        0        0      957 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/model.py
+-rw-r--r--   0        0        0   174335 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-22 18:54:32.702099 kodexa-7.0.9196860276/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   218349 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:54:32.706099 kodexa-7.0.9196860276/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1373 2024-05-22 18:56:47.256330 kodexa-7.0.9196860276/pyproject.toml
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9196860276/PKG-INFO
```

### Comparing `kodexa-7.0.9196745246/LICENSE` & `kodexa-7.0.9196860276/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/README.md` & `kodexa-7.0.9196860276/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/__init__.py` & `kodexa-7.0.9196860276/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/assistant/assistant.py` & `kodexa-7.0.9196860276/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/connectors/connectors.py` & `kodexa-7.0.9196860276/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/__init__.py` & `kodexa-7.0.9196860276/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/base.py` & `kodexa-7.0.9196860276/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/entities/product.py` & `kodexa-7.0.9196860276/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9196860276/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/model.py` & `kodexa-7.0.9196860276/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/objects.py` & `kodexa-7.0.9196860276/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/model/persistence.py` & `kodexa-7.0.9196860276/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9196860276/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/platform/client.py` & `kodexa-7.0.9196860276/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1547,14 +1547,28 @@
         return (
             AssistantDefinitionsEndpoint()
             .set_organization(self)
             .set_client(self.client)
         )
 
     @property
+    def guidance_sets(self) -> "GuidanceSetsEndpoint":
+        """
+        Get the guidance sets endpoint of the organization.
+
+        Returns:
+            GuidanceSetsEndpoint: The guidance sets endpoint of the organization.
+        """
+        return (
+            GuidanceSetsEndpoint()
+            .set_organization(self)
+            .set_client(self.client)
+        )
+
+    @property
     def credentials(self):
         """
         Get the credentials endpoint of the organization.
 
         Returns:
             CredentialDefinitionsEndpoint: The credentials endpoint of the organization.
         """
@@ -6225,15 +6239,14 @@
         self.memberships = MembershipsEndpoint(self)
         self.executions = ExecutionsEndpoint(self)
         self.channels = ChannelsEndpoint(self)
         self.assistants = AssistantsEndpoint(self)
         self.messages = MessagesEndpoint(self)
         from kodexa.model.entities.product import ProductsEndpoint
         self.products = ProductsEndpoint(self)
-        self.guidance_sets = GuidanceSetsEndpoint(self)
 
     @staticmethod
     def login(url, token):
         """
         A static method to login to the Kodexa platform.
 
         Args:
```

### Comparing `kodexa-7.0.9196745246/kodexa/platform/interaction.py` & `kodexa-7.0.9196860276/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/platform/kodexa.py` & `kodexa-7.0.9196860276/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/ast.py` & `kodexa-7.0.9196860276/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/core.py` & `kodexa-7.0.9196860276/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/lexrules.py` & `kodexa-7.0.9196860276/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/lextab.py` & `kodexa-7.0.9196860276/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/parserules.py` & `kodexa-7.0.9196860276/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/selectors/parsetab.py` & `kodexa-7.0.9196860276/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/spatial/azure_models.py` & `kodexa-7.0.9196860276/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9196860276/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9196860276/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/steps/common.py` & `kodexa-7.0.9196860276/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/testing/test_components.py` & `kodexa-7.0.9196860276/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/kodexa/testing/test_utils.py` & `kodexa-7.0.9196860276/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9196745246/pyproject.toml` & `kodexa-7.0.9196860276/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09196745246"
+version = "7.0.09196860276"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9196745246/PKG-INFO` & `kodexa-7.0.9196860276/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9196745246
+Version: 7.0.9196860276
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

