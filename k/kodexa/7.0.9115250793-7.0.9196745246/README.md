# Comparing `tmp/kodexa-7.0.9115250793.tar.gz` & `tmp/kodexa-7.0.9196745246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-7.0.9115250793.tar", max compression
+gzip compressed data, was "kodexa-7.0.9196745246.tar", max compression
```

## Comparing `kodexa-7.0.9115250793.tar` & `kodexa-7.0.9196745246.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2024-05-16 15:42:25.072823 kodexa-7.0.9115250793/LICENSE
--rw-r--r--   0        0        0     2178 2024-05-16 15:42:25.072823 kodexa-7.0.9115250793/README.md
--rw-r--r--   0        0        0      957 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    14663 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      328 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0    10413 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      796 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/__init__.py
--rw-r--r--   0        0        0      521 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/base.py
--rw-r--r--   0        0        0        0 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/entities/__init__.py
--rw-r--r--   0        0        0     3526 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/entities/product.py
--rw-r--r--   0        0        0     3810 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/entities/product_subscription.py
--rw-r--r--   0        0        0   115561 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/model.py
--rw-r--r--   0        0        0   174335 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/objects.py
--rw-r--r--   0        0        0    62032 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    25221 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   218218 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/platform/client.py
--rw-r--r--   0        0        0     1055 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/platform/interaction.py
--rw-r--r--   0        0        0    34024 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13269 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3691 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3447 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     3155 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       61 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7068 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       61 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    71452 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       61 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2024-05-16 15:42:25.080823 kodexa-7.0.9115250793/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    30564 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     5975 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    44214 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      179 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/steps/__init__.py
--rw-r--r--   0        0        0    10428 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/steps/common.py
--rw-r--r--   0        0        0      323 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/testing/__init__.py
--rw-r--r--   0        0        0     1052 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    14021 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:42:25.084823 kodexa-7.0.9115250793/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1373 2024-05-16 15:42:38.820824 kodexa-7.0.9115250793/pyproject.toml
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9115250793/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:44:12.918826 kodexa-7.0.9196745246/LICENSE
+-rw-r--r--   0        0        0     2178 2024-05-22 18:44:12.918826 kodexa-7.0.9196745246/README.md
+-rw-r--r--   0        0        0      957 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    14663 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      328 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      796 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      521 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/base.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/__init__.py
+-rw-r--r--   0        0        0     3526 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/product.py
+-rw-r--r--   0        0        0     3810 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/entities/product_subscription.py
+-rw-r--r--   0        0        0   115561 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/model.py
+-rw-r--r--   0        0        0   174335 2024-05-22 18:44:12.922826 kodexa-7.0.9196745246/kodexa/model/objects.py
+-rw-r--r--   0        0        0    62032 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    25221 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   218016 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/client.py
+-rw-r--r--   0        0        0     1055 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/interaction.py
+-rw-r--r--   0        0        0    34024 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13269 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3691 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3447 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     3155 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7068 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    71452 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       61 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    30564 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     5975 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    44214 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      179 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0    10428 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/steps/common.py
+-rw-r--r--   0        0        0      323 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0     1052 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    14021 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:44:12.926826 kodexa-7.0.9196745246/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1373 2024-05-22 18:44:29.730774 kodexa-7.0.9196745246/pyproject.toml
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 kodexa-7.0.9196745246/PKG-INFO
```

### Comparing `kodexa-7.0.9115250793/LICENSE` & `kodexa-7.0.9196745246/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/README.md` & `kodexa-7.0.9196745246/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/__init__.py` & `kodexa-7.0.9196745246/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/assistant/assistant.py` & `kodexa-7.0.9196745246/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/connectors/connectors.py` & `kodexa-7.0.9196745246/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/__init__.py` & `kodexa-7.0.9196745246/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/base.py` & `kodexa-7.0.9196745246/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/entities/product.py` & `kodexa-7.0.9196745246/kodexa/model/entities/product.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/entities/product_subscription.py` & `kodexa-7.0.9196745246/kodexa/model/entities/product_subscription.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/model.py` & `kodexa-7.0.9196745246/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/objects.py` & `kodexa-7.0.9196745246/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/model/persistence.py` & `kodexa-7.0.9196745246/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/pipeline/pipeline.py` & `kodexa-7.0.9196745246/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/platform/client.py` & `kodexa-7.0.9196745246/kodexa/platform/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2147,21 +2147,21 @@
 
         Returns:
             TaxonomyEndpoint: The instance class of the project taxonomies endpoint.
         """
         return TaxonomyEndpoint
 
 
-class ProjectGuidanceEndpoint(ProjectResourceEndpoint):
+class ProjectGuidanceSetsEndpoint(ProjectResourceEndpoint):
 
     def get_type(self) -> str:
         return "guidance"
 
     def get_instance_class(self, object_dict=None):
-        return GuidanceSetEndpoint
+        return GuidanceSetsEndpoint
 
 
 class ProjectDataFormEndpoint(ProjectResourceEndpoint):
 
     def get_type(self) -> str:
         return "dataForms"
 
@@ -2455,15 +2455,15 @@
         return "projects"
 
     def update_resources(
             self,
             stores: List["StoreEndpoint"] = None,
             taxonomies: List["TaxonomyEndpoint"] = None,
             data_forms: List["DataFormEndpoint"] = None,
-            guidance: List["GuidanceSetEndpoint"] = None,
+            guidance: List["GuidanceSetsEndpoint"] = None,
             dashboards: List["DashboardEndpoint"] = None,
     ):
         """Update the resources of the project.
 
         Args:
             stores (List["StoreEndpoint"], optional): List of store endpoints to update.
             taxonomies (List["TaxonomyEndpoint"], optional): List of taxonomy endpoints to update.
@@ -2536,21 +2536,21 @@
 
         Returns:
             ProjectTaxonomiesEndpoint: The taxonomies endpoint of the project.
         """
         return ProjectTaxonomiesEndpoint().set_client(self.client).set_project(self)
 
     @property
-    def guidance(self) -> "GuidanceEndpoint":
+    def guidance(self) -> "ProjectGuidanceEndpoint":
         """Get the guidance sets endpoint of the project.
 
         Returns:
             GuidanceSetsEndpoint: The guidance sets endpoint of the project.
         """
-        return ProjectGuidanceEndpoint().set_client(self.client).set_project(self)
+        return ProjectGuidanceSetEndpoint().set_client(self.client).set_project(self)
 
     @property
     def assistants(self) -> ProjectAssistantsEndpoint:
         """Get the assistants endpoint of the project.
 
         Returns:
             ProjectAssistantsEndpoint: The assistants endpoint of the project.
@@ -2578,50 +2578,14 @@
         response = self.client.put(
             f"/api/projects/{self.id}/tags",
             body=[tag.model_dump(by_alias=True) for tag in tags],
         )
         return [ProjectTag.model_validate(tag) for tag in response.json()]
 
 
-class GuidanceSetsEndpoint(EntitiesEndpoint):
-    """Represents a message endpoint"""
-
-    def get_type(self) -> str:
-        """
-        Get the type of the endpoint.
-
-        Returns:
-            str: The type of the endpoint, in this case "guidance".
-        """
-        return "guidance"
-
-    def get_instance_class(self, object_dict=None):
-        """
-        Get the instance class of the endpoint.
-
-        Args:
-            object_dict (dict, optional): An optional dictionary object. Defaults to None.
-
-        Returns:
-            GuidanceSetEndpoint: The instance class of the endpoint.
-        """
-        return GuidanceSetEndpoint
-
-    def get_page_class(self, object_dict=None):
-        """
-        Get the page class of the endpoint.
-
-        Args:
-            object_dict (dict, optional): An optional dictionary object. Defaults to None.
-
-        Returns:
-            PageGuidanceSetEndpoint: The page class of the endpoint.
-        """
-        return PageGuidanceSetEndpoint
-
 
 class MessagesEndpoint(EntitiesEndpoint):
     """Represents a message endpoint"""
 
     def get_type(self) -> str:
         """
         Get the type of the endpoint.
@@ -2999,17 +2963,17 @@
             return ModelStoreEndpoint
         elif object_dict["storeType"] == "TABLE":
             return DataStoreEndpoint
         else:
             raise ValueError(f"Unknown store type {object_dict['storeType']}")
 
 
-class GuidanceEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
+class GuidanceSetsEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
     """
-    Represents a guidance endpoint.
+    Represents a guidance set endpoint.
 
     This class is used to interact with the guidance endpoint of the API.
     It provides methods to get the type, page class, and instance class of the endpoint,
     as well as to deploy an extension pack from a URL.
     """
 
     def get_type(self) -> str:
@@ -6023,15 +5987,15 @@
         "type": PromptEndpoint,
         "endpoint": PromptsEndpoint,
     },
     "guidance": {
         "name": "guidance",
         "plural": "guidance",
         "type": GuidanceSetEndpoint,
-        "endpoint": GuidanceEndpoint,
+        "endpoint": GuidanceSetsEndpoint,
     },
     "modelRuntimes": {
         "name": "modelRuntime",
         "plural": "modelRuntimes",
         "type": ModelRuntimeEndpoint,
         "endpoint": ModelRuntimesEndpoint,
     },
@@ -6648,14 +6612,26 @@
             with open(taxonomy_file, "w") as f:
                 f.write(
                     json.dumps(
                         taxonomy.model_dump(mode="json", by_alias=True), indent=4
                     )
                 )
 
+        for guidance in project.guidance.list():
+            guidance_file = os.path.join(
+                project_export_dir, f"guidance-{guidance.slug}-{guidance.version}.json"
+            )
+            with open(guidance_file, "w") as f:
+                f.write(
+                    json.dumps(
+                        guidance.model_dump(mode="json", by_alias=True), indent=4
+                    )
+                )
+
+
     def import_project(self, organization: OrganizationEndpoint, import_path: str):
         """
         A method to import a project.
 
         Args:
             organization (OrganizationEndpoint): The organization to import the project to.
             import_path (str): The path to import the project from.
@@ -6741,14 +6717,21 @@
         for taxonomy_file in glob.glob(os.path.join(import_path, "taxonomy-*.json")):
             with open(taxonomy_file, "r") as f:
                 taxonomy = TaxonomyEndpoint.model_validate(json.load(f))
                 taxonomy.org_slug = None
                 taxonomy.ref = None
                 taxonomies.append(organization.taxonomies.create(taxonomy))
 
+        for guidance_file in glob.glob(os.path.join(import_path, "guidance-*.json")):
+            with open(guidance_file, "r") as f:
+                guidance = GuidanceSetEndpoint.model_validate(json.load(f))
+                guidance.org_slug = None
+                guidance.ref = None
+                organization.guidance.create(guidance)
+
         import time
 
         time.sleep(4)
 
         new_project.update_resources(stores=stores, taxonomies=taxonomies)
 
     def deserialize(
```

### Comparing `kodexa-7.0.9115250793/kodexa/platform/interaction.py` & `kodexa-7.0.9196745246/kodexa/platform/interaction.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/platform/kodexa.py` & `kodexa-7.0.9196745246/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/ast.py` & `kodexa-7.0.9196745246/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/core.py` & `kodexa-7.0.9196745246/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/lexrules.py` & `kodexa-7.0.9196745246/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/lextab.py` & `kodexa-7.0.9196745246/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/parserules.py` & `kodexa-7.0.9196745246/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/selectors/parsetab.py` & `kodexa-7.0.9196745246/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/spatial/azure_models.py` & `kodexa-7.0.9196745246/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/spatial/bbox_common.py` & `kodexa-7.0.9196745246/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/spatial/table_form_common.py` & `kodexa-7.0.9196745246/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/steps/common.py` & `kodexa-7.0.9196745246/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/testing/test_components.py` & `kodexa-7.0.9196745246/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/kodexa/testing/test_utils.py` & `kodexa-7.0.9196745246/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-7.0.9115250793/pyproject.toml` & `kodexa-7.0.9196745246/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "7.0.09115250793"
+version = "7.0.09196745246"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-7.0.9115250793/PKG-INFO` & `kodexa-7.0.9196745246/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 7.0.9115250793
+Version: 7.0.9196745246
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

