# Comparing `tmp/nvidia_haystack-0.0.2.tar.gz` & `tmp/nvidia_haystack-0.0.3.tar.gz`

## Comparing `nvidia_haystack-0.0.2.tar` & `nvidia_haystack-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/pydoc/config.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/_nim_backend.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/_nvcf_backend.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/backend.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/document_embedder.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/text_embedder.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/__init__.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_nim_backend.py
--rw-r--r--   0        0        0     3472 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_nvcf_backend.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_schema.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/backend.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/chat/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/utils/nvidia/__init__.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/src/haystack_integrations/utils/nvidia/client.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/tests/test_document_embedder.py
--rw-r--r--   0        0        0     7332 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/tests/test_generator.py
--rw-r--r--   0        0        0     6017 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/tests/test_text_embedder.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/.gitignore
--rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/README.md
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/pydoc/config.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/__init__.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/_nim_backend.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/_nvcf_backend.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/backend.py
+-rw-r--r--   0        0        0     8061 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/document_embedder.py
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/text_embedder.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/truncate.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/__init__.py
+-rw-r--r--   0        0        0     2671 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_nim_backend.py
+-rw-r--r--   0        0        0     3597 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_nvcf_backend.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_schema.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/backend.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/chat/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/utils/nvidia/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/src/haystack_integrations/utils/nvidia/client.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0    16993 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/tests/test_document_embedder.py
+-rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/tests/test_generator.py
+-rw-r--r--   0        0        0     7774 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/tests/test_text_embedder.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/.gitignore
+-rw-r--r--   0        0        0    11350 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/README.md
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 nvidia_haystack-0.0.3/PKG-INFO
```

### Comparing `nvidia_haystack-0.0.2/pydoc/config.yml` & `nvidia_haystack-0.0.3/pydoc/config.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 loaders:
   - type: haystack_pydoc_tools.loaders.CustomPythonLoader
     search_path: [../src]
     modules:
       [
         "haystack_integrations.components.embedders.nvidia.document_embedder",
         "haystack_integrations.components.embedders.nvidia.text_embedder",
-        "haystack_integrations.components.embedders.nvidia.models",
+        "haystack_integrations.components.generators.nvidia.generator",
       ]
     ignore_when_discovered: ["__init__"]
 processors:
   - type: filter
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Nvidia integration for Haystack
   category_slug: integrations-api
   title: Nvidia
   slug: integrations-nvidia
-  order: 50
+  order: 165
   markdown:
     descriptive_class_title: false
     classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_nvidia.md
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/_nvcf_backend.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/_nvcf_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, List, Literal, Optional, Tuple, Union
 
 from haystack.utils.auth import Secret
 from haystack_integrations.utils.nvidia import NvidiaCloudFunctionsClient
 
 from .backend import EmbedderBackend
@@ -13,14 +14,15 @@
 class NvcfBackend(EmbedderBackend):
     def __init__(
         self,
         model: str,
         api_key: Secret,
         model_kwargs: Optional[Dict[str, Any]] = None,
     ):
+        warnings.warn("Nvidia NGC is deprecated, use Nvidia NIM instead.", DeprecationWarning, stacklevel=2)
         if not model.startswith("playground_"):
             model = f"playground_{model}"
 
         super().__init__(model=model, model_kwargs=model_kwargs)
 
         self.api_key = api_key
         self.client = NvidiaCloudFunctionsClient(
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/backend.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/backend.py`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/document_embedder.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/document_embedder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from haystack import Document, component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
 from tqdm import tqdm
 
 from ._nim_backend import NimBackend
 from ._nvcf_backend import NvcfBackend
 from .backend import EmbedderBackend
+from .truncate import EmbeddingTruncateMode
 
 
 @component
 class NvidiaDocumentEmbedder:
     """
     A component for embedding documents using embedding models provided by
     [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/)
-    and NVIDIA NeMo Inference Microservices.
+    and NVIDIA Inference Microservices.
 
     Usage example:
     ```python
-    from haystack_integrations.components.embedders.nvidia import NvidiaDocumentEmbedder, NvidiaEmbeddingModel
+    from haystack_integrations.components.embedders.nvidia import NvidiaDocumentEmbedder
 
     doc = Document(content="I love pizza!")
 
     text_embedder = NvidiaDocumentEmbedder(model="nvolveqa_40k")
     text_embedder.warm_up()
 
     result = document_embedder.run([doc])
@@ -37,49 +38,57 @@
         api_url: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
         batch_size: int = 32,
         progress_bar: bool = True,
         meta_fields_to_embed: Optional[List[str]] = None,
         embedding_separator: str = "\n",
+        truncate: Optional[Union[EmbeddingTruncateMode, str]] = None,
     ):
         """
         Create a NvidiaTextEmbedder component.
 
         :param model:
             Embedding model to use.
         :param api_key:
             API key for the NVIDIA AI Foundation Endpoints.
         :param api_url:
-            Custom API URL for the NVIDIA NeMo Inference Microservices.
+            Custom API URL for the NVIDIA Inference Microservices.
         :param prefix:
             A string to add to the beginning of each text.
         :param suffix:
             A string to add to the end of each text.
         :param batch_size:
             Number of Documents to encode at once.
             Cannot be greater than 50.
         :param progress_bar:
             Whether to show a progress bar or not.
         :param meta_fields_to_embed:
             List of meta fields that should be embedded along with the Document text.
         :param embedding_separator:
             Separator used to concatenate the meta fields to the Document text.
+        :param truncate:
+            Specifies how inputs longer that the maximum token length should be truncated.
+            If None the behavior is model-dependent, see the official documentation for more information.
         """
 
         self.api_key = api_key
         self.model = model
         self.api_url = api_url
         self.prefix = prefix
         self.suffix = suffix
         self.batch_size = batch_size
         self.progress_bar = progress_bar
         self.meta_fields_to_embed = meta_fields_to_embed or []
         self.embedding_separator = embedding_separator
 
+        if isinstance(truncate, str):
+            truncate = EmbeddingTruncateMode.from_str(truncate)
+        self.truncate = truncate
+
         self.backend: Optional[EmbedderBackend] = None
         self._initialized = False
 
     def warm_up(self):
         """
         Initializes the component.
         """
@@ -89,15 +98,23 @@
         if self.api_url is None:
             if self.api_key is None:
                 msg = "API key is required for NVIDIA AI Foundation Endpoints."
                 raise ValueError(msg)
 
             self.backend = NvcfBackend(self.model, api_key=self.api_key, model_kwargs={"model": "passage"})
         else:
-            self.backend = NimBackend(self.model, api_url=self.api_url, model_kwargs={"input_type": "passage"})
+            model_kwargs = {"input_type": "passage"}
+            if self.truncate is not None:
+                model_kwargs["truncate"] = str(self.truncate)
+            self.backend = NimBackend(
+                self.model,
+                api_url=self.api_url,
+                api_key=self.api_key,
+                model_kwargs=model_kwargs,
+            )
 
         self._initialized = True
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
@@ -111,14 +128,15 @@
             api_url=self.api_url,
             prefix=self.prefix,
             suffix=self.suffix,
             batch_size=self.batch_size,
             progress_bar=self.progress_bar,
             meta_fields_to_embed=self.meta_fields_to_embed,
             embedding_separator=self.embedding_separator,
+            truncate=str(self.truncate) if self.truncate is not None else None,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "NvidiaDocumentEmbedder":
         """
         Deserializes the component from a dictionary.
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/embedders/nvidia/text_embedder.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/embedders/nvidia/text_embedder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from haystack import component, default_from_dict, default_to_dict
 from haystack.utils import Secret, deserialize_secrets_inplace
 
 from ._nim_backend import NimBackend
 from ._nvcf_backend import NvcfBackend
 from .backend import EmbedderBackend
+from .truncate import EmbeddingTruncateMode
 
 
 @component
 class NvidiaTextEmbedder:
     """
     A component for embedding strings using embedding models provided by
     [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/)
-    and NVIDIA NeMo Inference Microservices.
+    and NVIDIA Inference Microservices.
 
     For models that differentiate between query and document inputs,
     this component embeds the input string as a query.
 
     Usage example:
     ```python
-    from haystack_integrations.components.embedders.nvidia import NvidiaTextEmbedder, NvidiaEmbeddingModel
+    from haystack_integrations.components.embedders.nvidia import NvidiaTextEmbedder
 
     text_to_embed = "I love pizza!"
 
     text_embedder = NvidiaTextEmbedder(model="nvolveqa_40k")
     text_embedder.warm_up()
 
     print(text_embedder.run(text_to_embed))
@@ -34,36 +35,44 @@
     def __init__(
         self,
         model: str,
         api_key: Optional[Secret] = Secret.from_env_var("NVIDIA_API_KEY"),
         api_url: Optional[str] = None,
         prefix: str = "",
         suffix: str = "",
+        truncate: Optional[Union[EmbeddingTruncateMode, str]] = None,
     ):
         """
         Create a NvidiaTextEmbedder component.
 
         :param model:
             Embedding model to use.
         :param api_key:
             API key for the NVIDIA AI Foundation Endpoints.
         :param api_url:
-            Custom API URL for the NVIDIA NeMo Inference Microservices.
+            Custom API URL for the NVIDIA Inference Microservices.
         :param prefix:
             A string to add to the beginning of each text.
         :param suffix:
             A string to add to the end of each text.
+        :param truncate:
+            Specifies how inputs longer that the maximum token length should be truncated.
+            If None the behavior is model-dependent, see the official documentation for more information.
         """
 
         self.api_key = api_key
         self.model = model
         self.api_url = api_url
         self.prefix = prefix
         self.suffix = suffix
 
+        if isinstance(truncate, str):
+            truncate = EmbeddingTruncateMode.from_str(truncate)
+        self.truncate = truncate
+
         self.backend: Optional[EmbedderBackend] = None
         self._initialized = False
 
     def warm_up(self):
         """
         Initializes the component.
         """
@@ -73,15 +82,23 @@
         if self.api_url is None:
             if self.api_key is None:
                 msg = "API key is required for NVIDIA AI Foundation Endpoints."
                 raise ValueError(msg)
 
             self.backend = NvcfBackend(self.model, api_key=self.api_key, model_kwargs={"model": "query"})
         else:
-            self.backend = NimBackend(self.model, api_url=self.api_url, model_kwargs={"input_type": "query"})
+            model_kwargs = {"input_type": "query"}
+            if self.truncate is not None:
+                model_kwargs["truncate"] = str(self.truncate)
+            self.backend = NimBackend(
+                self.model,
+                api_url=self.api_url,
+                api_key=self.api_key,
+                model_kwargs=model_kwargs,
+            )
 
         self._initialized = True
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
 
@@ -91,14 +108,15 @@
         return default_to_dict(
             self,
             api_key=self.api_key.to_dict() if self.api_key else None,
             model=self.model,
             api_url=self.api_url,
             prefix=self.prefix,
             suffix=self.suffix,
+            truncate=str(self.truncate) if self.truncate is not None else None,
         )
 
     @classmethod
     def from_dict(cls, data: Dict[str, Any]) -> "NvidiaTextEmbedder":
         """
         Deserializes the component from a dictionary.
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_nim_backend.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_nim_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
+from haystack.utils import Secret
 
 from .backend import GeneratorBackend
 
 REQUEST_TIMEOUT = 60
 
 
 class NimBackend(GeneratorBackend):
     def __init__(
         self,
         model: str,
         api_url: str,
+        api_key: Optional[Secret] = Secret.from_env_var("NVIDIA_API_KEY"),
         model_kwargs: Optional[Dict[str, Any]] = None,
     ):
         headers = {
             "Content-Type": "application/json",
             "accept": "application/json",
         }
+
+        if api_key:
+            headers["authorization"] = f"Bearer {api_key.resolve_value()}"
+
         self.session = requests.Session()
         self.session.headers.update(headers)
 
         self.model = model
         self.api_url = api_url
         self.model_kwargs = model_kwargs or {}
 
     def generate(self, prompt: str) -> Tuple[List[str], List[Dict[str, Any]]]:
-        # We're using the chat completion endpoint as the local containers don't support
+        # We're using the chat completion endpoint as the NIM API doesn't support
         # the /completions endpoint. So both the non-chat and chat generator will use this.
+        # This is the same for local containers and the cloud API.
         url = f"{self.api_url}/chat/completions"
 
         res = self.session.post(
             url,
             json={
                 "model": self.model,
                 "messages": [
@@ -53,17 +60,21 @@
         replies = []
         meta = []
         for choice in choices:
             message = choice["message"]
             replies.append(message["content"])
             choice_meta = {
                 "role": message["role"],
-                "finish_reason": choice["finish_reason"],
                 "usage": {
                     "prompt_tokens": completions["usage"]["prompt_tokens"],
-                    "completion_tokens": completions["usage"]["completion_tokens"],
                     "total_tokens": completions["usage"]["total_tokens"],
                 },
             }
+            # These fields could be null, the others will always be present
+            if "finish_reason" in choice:
+                choice_meta["finish_reason"] = choice["finish_reason"]
+            if "completion_tokens" in completions["usage"]:
+                choice_meta["usage"]["completion_tokens"] = completions["usage"]["completion_tokens"]
+
             meta.append(choice_meta)
 
         return replies, meta
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_nvcf_backend.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_nvcf_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 from haystack.utils.auth import Secret
 from haystack_integrations.utils.nvidia import NvidiaCloudFunctionsClient
 
 from .backend import GeneratorBackend
@@ -10,14 +11,15 @@
 class NvcfBackend(GeneratorBackend):
     def __init__(
         self,
         model: str,
         api_key: Secret,
         model_kwargs: Optional[Dict[str, Any]] = None,
     ):
+        warnings.warn("Nvidia NGC is deprecated, use Nvidia NIM instead.", DeprecationWarning, stacklevel=2)
         if not model.startswith("playground_"):
             model = f"playground_{model}"
 
         super().__init__(model=model, model_kwargs=model_kwargs)
 
         self.api_key = api_key
         self.client = NvidiaCloudFunctionsClient(
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/_schema.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/_schema.py`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/backend.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/backend.py`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/components/generators/nvidia/generator.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/components/generators/nvidia/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 from .backend import GeneratorBackend
 
 
 @component
 class NvidiaGenerator:
     """
     A component for generating text using generative models provided by
-    [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/).
+    [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/)
+    and NVIDIA Inference Microservices.
 
     Usage example:
     ```python
-    from haystack_integrations.components.generators.nvidia import NvidiaGenerator, NvidiaGeneratorModel
+    from haystack_integrations.components.generators.nvidia import NvidiaGenerator
 
     generator = NvidiaGenerator(
         model="nv_llama2_rlhf_70b",
         model_arguments={
             "temperature": 0.2,
             "top_p": 0.7,
             "max_tokens": 1024,
@@ -51,15 +52,15 @@
         :param model:
             Name of the model to use for text generation.
             See the [Nvidia catalog](https://catalog.ngc.nvidia.com/ai-foundation-models)
             for more information on the supported models.
         :param api_key:
             API key for the NVIDIA AI Foundation Endpoints.
         :param api_url:
-            Custom API URL for the NVIDIA NeMo Inference Microservices.
+            Custom API URL for the NVIDIA Inference Microservices.
         :param model_arguments:
             Additional arguments to pass to the model provider. Different models accept different arguments.
             Search your model in the [Nvidia catalog](https://catalog.ngc.nvidia.com/ai-foundation-models)
             to know the supported arguments.
         """
         self._model = model
         self._api_url = api_url
@@ -80,14 +81,15 @@
                 msg = "API key is required for NVIDIA AI Foundation Endpoints."
                 raise ValueError(msg)
             self._backend = NvcfBackend(self._model, api_key=self._api_key, model_kwargs=self._model_arguments)
         else:
             self._backend = NimBackend(
                 self._model,
                 api_url=self._api_url,
+                api_key=self._api_key,
                 model_kwargs=self._model_arguments,
             )
 
     def to_dict(self) -> Dict[str, Any]:
         """
         Serializes the component to a dictionary.
```

### Comparing `nvidia_haystack-0.0.2/src/haystack_integrations/utils/nvidia/client.py` & `nvidia_haystack-0.0.3/src/haystack_integrations/utils/nvidia/client.py`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/tests/test_document_embedder.py` & `nvidia_haystack-0.0.3/tests/test_document_embedder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from unittest.mock import Mock, patch
 
 import pytest
 from haystack import Document
 from haystack.utils import Secret
-from haystack_integrations.components.embedders.nvidia import NvidiaDocumentEmbedder
+from haystack_integrations.components.embedders.nvidia import EmbeddingTruncateMode, NvidiaDocumentEmbedder
 
 
 class TestNvidiaDocumentEmbedder:
     def test_init_default(self, monkeypatch):
         monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
         embedder = NvidiaDocumentEmbedder("nvolveqa_40k")
 
@@ -60,45 +60,76 @@
                 "model": "playground_nvolveqa_40k",
                 "prefix": "",
                 "suffix": "",
                 "batch_size": 32,
                 "progress_bar": True,
                 "meta_fields_to_embed": [],
                 "embedding_separator": "\n",
+                "truncate": None,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self, monkeypatch):
         monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
         component = NvidiaDocumentEmbedder(
             model="playground_nvolveqa_40k",
             api_url="https://example.com",
             prefix="prefix",
             suffix="suffix",
             batch_size=10,
             progress_bar=False,
             meta_fields_to_embed=["test_field"],
             embedding_separator=" | ",
+            truncate=EmbeddingTruncateMode.END,
         )
         data = component.to_dict()
         assert data == {
             "type": "haystack_integrations.components.embedders.nvidia.document_embedder.NvidiaDocumentEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["NVIDIA_API_KEY"], "strict": True, "type": "env_var"},
                 "api_url": "https://example.com",
                 "model": "playground_nvolveqa_40k",
                 "prefix": "prefix",
                 "suffix": "suffix",
                 "batch_size": 10,
                 "progress_bar": False,
                 "meta_fields_to_embed": ["test_field"],
                 "embedding_separator": " | ",
+                "truncate": "END",
             },
         }
 
+    def from_dict(self, monkeypatch):
+        monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
+        data = {
+            "type": "haystack_integrations.components.embedders.nvidia.document_embedder.NvidiaDocumentEmbedder",
+            "init_parameters": {
+                "api_key": {"env_vars": ["NVIDIA_API_KEY"], "strict": True, "type": "env_var"},
+                "api_url": "https://example.com",
+                "model": "playground_nvolveqa_40k",
+                "prefix": "prefix",
+                "suffix": "suffix",
+                "batch_size": 10,
+                "progress_bar": False,
+                "meta_fields_to_embed": ["test_field"],
+                "embedding_separator": " | ",
+                "truncate": "START",
+            },
+        }
+        component = NvidiaDocumentEmbedder.from_dict(data)
+        assert component.model == "nvolveqa_40k"
+        assert component.api_url is None
+        assert component.prefix == "prefix"
+        assert component.suffix == "suffix"
+        assert component.batch_size == 32
+        assert component.progress_bar
+        assert component.meta_fields_to_embed == []
+        assert component.embedding_separator == "\n"
+        assert component.truncate == EmbeddingTruncateMode.START
+
     def test_prepare_texts_to_embed_w_metadata(self):
         documents = [
             Document(content=f"document number {i}:\ncontent", meta={"meta_field": f"meta_value {i}"}) for i in range(5)
         ]
 
         embedder = NvidiaDocumentEmbedder(
             "playground_nvolveqa_40k",
@@ -345,13 +376,40 @@
         docs = [
             Document(content="I love cheese", meta={"topic": "Cuisine"}),
             Document(content="A transformer is a deep learning architecture", meta={"topic": "ML"}),
         ]
 
         result = embedder.run(docs)
         docs_with_embeddings = result["documents"]
+
+        assert isinstance(docs_with_embeddings, list)
+        assert len(docs_with_embeddings) == len(docs)
+        for doc in docs_with_embeddings:
+            assert isinstance(doc.embedding, list)
+            assert isinstance(doc.embedding[0], float)
+
+    @pytest.mark.skipif(
+        not os.environ.get("NVIDIA_CATALOG_API_KEY", None),
+        reason="Export an env var called NVIDIA_CATALOG_API_KEY containing the Nvidia API key to run this test.",
+    )
+    @pytest.mark.integration
+    def test_run_integration_with_api_catalog(self):
+        embedder = NvidiaDocumentEmbedder(
+            model="NV-Embed-QA",
+            api_url="https://ai.api.nvidia.com/v1/retrieval/nvidia",
+            api_key=Secret.from_env_var("NVIDIA_CATALOG_API_KEY"),
+        )
+        embedder.warm_up()
+
+        docs = [
+            Document(content="I love cheese", meta={"topic": "Cuisine"}),
+            Document(content="A transformer is a deep learning architecture", meta={"topic": "ML"}),
+        ]
+
+        result = embedder.run(docs)
+        docs_with_embeddings = result["documents"]
 
         assert isinstance(docs_with_embeddings, list)
         assert len(docs_with_embeddings) == len(docs)
         for doc in docs_with_embeddings:
             assert isinstance(doc.embedding, list)
             assert isinstance(doc.embedding[0], float)
```

### Comparing `nvidia_haystack-0.0.2/tests/test_generator.py` & `nvidia_haystack-0.0.3/tests/test_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,7 +198,27 @@
             },
         )
         generator.warm_up()
         result = generator.run(prompt="What is the answer?")
 
         assert result["replies"]
         assert result["meta"]
+
+    @pytest.mark.skipif(
+        not os.environ.get("NVIDIA_CATALOG_API_KEY", None),
+        reason="Export an env var called NVIDIA_CATALOG_API_KEY containing the Nvidia API key to run this test.",
+    )
+    @pytest.mark.integration
+    def test_run_integration_with_api_catalog(self):
+        generator = NvidiaGenerator(
+            model="meta/llama3-70b-instruct",
+            api_url="https://integrate.api.nvidia.com/v1",
+            api_key=Secret.from_env_var("NVIDIA_CATALOG_API_KEY"),
+            model_arguments={
+                "temperature": 0.2,
+            },
+        )
+        generator.warm_up()
+        result = generator.run(prompt="What is the answer?")
+
+        assert result["replies"]
+        assert result["meta"]
```

### Comparing `nvidia_haystack-0.0.2/tests/test_text_embedder.py` & `nvidia_haystack-0.0.3/tests/test_text_embedder.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from unittest.mock import Mock, patch
 
 import pytest
 from haystack.utils import Secret
-from haystack_integrations.components.embedders.nvidia import NvidiaTextEmbedder
+from haystack_integrations.components.embedders.nvidia import EmbeddingTruncateMode, NvidiaTextEmbedder
 
 
 class TestNvidiaTextEmbedder:
     def test_init_default(self, monkeypatch):
         monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
         embedder = NvidiaTextEmbedder("nvolveqa_40k")
 
@@ -42,36 +42,59 @@
             "type": "haystack_integrations.components.embedders.nvidia.text_embedder.NvidiaTextEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["NVIDIA_API_KEY"], "strict": True, "type": "env_var"},
                 "api_url": None,
                 "model": "nvolveqa_40k",
                 "prefix": "",
                 "suffix": "",
+                "truncate": None,
             },
         }
 
     def test_to_dict_with_custom_init_parameters(self, monkeypatch):
         monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
         component = NvidiaTextEmbedder(
             model="nvolveqa_40k",
             prefix="prefix",
             suffix="suffix",
+            truncate=EmbeddingTruncateMode.START,
         )
         data = component.to_dict()
         assert data == {
             "type": "haystack_integrations.components.embedders.nvidia.text_embedder.NvidiaTextEmbedder",
             "init_parameters": {
                 "api_key": {"env_vars": ["NVIDIA_API_KEY"], "strict": True, "type": "env_var"},
                 "api_url": None,
                 "model": "nvolveqa_40k",
                 "prefix": "prefix",
                 "suffix": "suffix",
+                "truncate": "START",
             },
         }
 
+    def from_dict(self, monkeypatch):
+        monkeypatch.setenv("NVIDIA_API_KEY", "fake-api-key")
+        data = {
+            "type": "haystack_integrations.components.embedders.nvidia.text_embedder.NvidiaTextEmbedder",
+            "init_parameters": {
+                "api_key": {"env_vars": ["NVIDIA_API_KEY"], "strict": True, "type": "env_var"},
+                "api_url": None,
+                "model": "nvolveqa_40k",
+                "prefix": "prefix",
+                "suffix": "suffix",
+                "truncate": "START",
+            },
+        }
+        component = NvidiaTextEmbedder.from_dict(data)
+        assert component.model == "nvolveqa_40k"
+        assert component.api_url is None
+        assert component.prefix == "prefix"
+        assert component.suffix == "suffix"
+        assert component.truncate == "START"
+
     @patch("haystack_integrations.components.embedders.nvidia._nvcf_backend.NvidiaCloudFunctionsClient")
     def test_run(self, mock_client_class):
         embedder = NvidiaTextEmbedder(
             "playground_nvolveqa_40k", api_key=Secret.from_token("fake-api-key"), prefix="prefix ", suffix=" suffix"
         )
         mock_client = Mock(
             get_model_nvcf_id=Mock(return_value="some_id"),
@@ -144,9 +167,29 @@
         )
         embedder.warm_up()
 
         result = embedder.run("A transformer is a deep learning architecture")
         embedding = result["embedding"]
         meta = result["meta"]
 
+        assert all(isinstance(x, float) for x in embedding)
+        assert "usage" in meta
+
+    @pytest.mark.skipif(
+        not os.environ.get("NVIDIA_CATALOG_API_KEY", None),
+        reason="Export an env var called NVIDIA_CATALOG_API_KEY containing the Nvidia API key to run this test.",
+    )
+    @pytest.mark.integration
+    def test_run_integration_with_api_catalog(self):
+        embedder = NvidiaTextEmbedder(
+            model="NV-Embed-QA",
+            api_url="https://ai.api.nvidia.com/v1/retrieval/nvidia",
+            api_key=Secret.from_env_var("NVIDIA_CATALOG_API_KEY"),
+        )
+        embedder.warm_up()
+
+        result = embedder.run("A transformer is a deep learning architecture")
+        embedding = result["embedding"]
+        meta = result["meta"]
+
         assert all(isinstance(x, float) for x in embedding)
         assert "usage" in meta
```

### Comparing `nvidia_haystack-0.0.2/.gitignore` & `nvidia_haystack-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/LICENSE.txt` & `nvidia_haystack-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/README.md` & `nvidia_haystack-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nvidia_haystack-0.0.2/pyproject.toml` & `nvidia_haystack-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 description = ''
 readme = "README.md"
 requires-python = ">=3.8"
 license = "Apache-2.0"
 keywords = []
 authors = [{ name = "deepset GmbH", email = "info@deepset.ai" }]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
@@ -43,35 +44,35 @@
 [tool.hatch.envs.default]
 dependencies = ["coverage[toml]>=6.5", "pytest", "haystack-pydoc-tools"]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
-docs = ["echo 'skip doc gen'"]
+docs = ["pydoc-markdown pydoc/config.yml"]
 
 [[tool.hatch.envs.all.matrix]]
-python = ["3.7", "3.8", "3.9", "3.10", "3.11"]
+python = ["3.8", "3.9", "3.10", "3.11"]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = ["black>=23.1.0", "mypy>=1.0.0", "ruff>=0.0.243"]
 [tool.hatch.envs.lint.scripts]
 typing = "mypy --install-types --non-interactive --explicit-package-bases {args:src/ tests}"
 style = ["ruff {args:.}", "black --check --diff {args:.}"]
 fmt = ["black {args:.}", "ruff --fix {args:.}", "style"]
 all = ["style", "typing"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
@@ -112,15 +113,14 @@
   "B008",
   "S101",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
-extend-exclude = ["tests", "example"]
 
 [tool.ruff.isort]
 known-first-party = ["src"]
 
 [tool.ruff.flake8-tidy-imports]
 ban-relative-imports = "parents"
 
@@ -132,20 +132,16 @@
 source = ["haystack_integrations"]
 branch = true
 parallel = false
 
 
 [tool.coverage.report]
 omit = ["*/tests/*", "*/__init__.py"]
-show_missing=true
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+show_missing = true
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 
 [[tool.mypy.overrides]]
 module = [
   "nvidia.*",
   "haystack.*",
   "haystack_integrations.*",
```

### Comparing `nvidia_haystack-0.0.2/PKG-INFO` & `nvidia_haystack-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.3
 Name: nvidia-haystack
-Version: 0.0.2
+Version: 0.0.3
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/nvidia#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/nvidia
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

