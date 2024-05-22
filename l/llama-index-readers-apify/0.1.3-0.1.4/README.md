# Comparing `tmp/llama_index_readers_apify-0.1.3.tar.gz` & `tmp/llama_index_readers_apify-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_apify-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_apify-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_apify-0.1.3.tar` & `llama_index_readers_apify-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3390 2024-02-13 13:53:01.732193 llama_index_readers_apify-0.1.3/README.md
--rw-r--r--   0        0        0      166 2024-02-13 13:53:01.732388 llama_index_readers_apify-0.1.3/llama_index/readers/apify/__init__.py
--rw-r--r--   0        0        0      104 2024-02-13 13:53:01.732519 llama_index_readers_apify-0.1.3/llama_index/readers/apify/actor/__init__.py
--rw-r--r--   0        0        0     2257 2024-02-13 13:53:01.732578 llama_index_readers_apify-0.1.3/llama_index/readers/apify/actor/base.py
--rw-r--r--   0        0        0      110 2024-02-13 13:53:01.732708 llama_index_readers_apify-0.1.3/llama_index/readers/apify/dataset/__init__.py
--rw-r--r--   0        0        0     1374 2024-02-13 13:53:01.732772 llama_index_readers_apify-0.1.3/llama_index/readers/apify/dataset/base.py
--rw-r--r--   0        0        0     1560 2024-02-21 19:23:05.063054 llama_index_readers_apify-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4099 1970-01-01 00:00:00.000000 llama_index_readers_apify-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2991 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/README.md
+-rw-r--r--   0        0        0      166 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/llama_index/readers/apify/__init__.py
+-rw-r--r--   0        0        0      104 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/llama_index/readers/apify/actor/__init__.py
+-rw-r--r--   0        0        0     2460 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/llama_index/readers/apify/actor/base.py
+-rw-r--r--   0        0        0      110 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/llama_index/readers/apify/dataset/__init__.py
+-rw-r--r--   0        0        0     1577 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/llama_index/readers/apify/dataset/base.py
+-rw-r--r--   0        0        0     1560 2024-05-22 14:50:50.196684 llama_index_readers_apify-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 llama_index_readers_apify-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_apify-0.1.3/README.md` & `llama_index_readers_apify-0.1.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,32 @@
+Metadata-Version: 2.1
+Name: llama-index-readers-apify
+Version: 0.1.4
+Summary: llama-index readers apify integration
+License: MIT
+Keywords: apify,crawler,scraper,scraping
+Author: Your Name
+Author-email: you@example.com
+Maintainer: drobnikj
+Requires-Python: >=3.8.1,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: apify-client (>=1.6.2,<2.0.0)
+Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Description-Content-Type: text/markdown
+
 # Apify Loaders
 
+```bash
+pip install llama-index-readers-apify
+```
+
 ## Apify Actor Loader
 
 [Apify](https://apify.com/) is a cloud platform for web scraping and data extraction,
 which provides an [ecosystem](https://apify.com/store) of more than a thousand
 ready-made apps called _Actors_ for various scraping, crawling, and extraction use cases.
 
 This loader runs a specific Actor and loads its results.
@@ -16,44 +39,36 @@
 The extracted text then can be fed to a vector index or language model like GPT
 in order to answer questions from it.
 
 To use this loader, you need to have a (free) Apify account
 and set your [Apify API token](https://console.apify.com/account/integrations) in the code.
 
 ```python
-from llama_index import download_loader
-from llama_index.readers.schema import Document
-
-
-# Converts a single record from the Actor's resulting dataset to the LlamaIndex format
-def tranform_dataset_item(item):
-    return Document(
-        text=item.get("text"),
-        extra_info={
-            "url": item.get("url"),
-        },
-    )
-
-
-ApifyActor = download_loader("ApifyActor")
+from llama_index.core import Document
+from llama_index.readers.apify import ApifyActor
 
 reader = ApifyActor("<My Apify API token>")
+
 documents = reader.load_data(
     actor_id="apify/website-content-crawler",
     run_input={
-        "startUrls": [{"url": "https://gpt-index.readthedocs.io/en/latest"}]
+        "startUrls": [{"url": "https://docs.llamaindex.ai/en/latest/"}]
     },
-    dataset_mapping_function=tranform_dataset_item,
+    dataset_mapping_function=lambda item: Document(
+        text=item.get("text"),
+        metadata={
+            "url": item.get("url"),
+        },
+    ),
 )
 ```
 
 This loader is designed to be used as a way to load data into
 [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently
 used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
-See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
 
 ## Apify Dataset Loader
 
 [Apify](https://apify.com/) is a cloud platform for web scraping and data extraction,
 which provides an [ecosystem](https://apify.com/store) of more than a thousand
 ready-made apps called _Actors_ for various scraping, crawling, and extraction use cases.
 
@@ -68,29 +83,22 @@
 The extracted text then can be fed to a vector index or language model like GPT
 in order to answer questions from it.
 
 To use this loader, you need to have a (free) Apify account
 and set your [Apify API token](https://console.apify.com/account/integrations) in the code.
 
 ```python
-from llama_index import download_loader
-from llama_index.readers.schema import Document
-
-
-# Converts a single record from the Apify dataset to the LlamaIndex format
-def tranform_dataset_item(item):
-    return Document(
-        text=item.get("text"),
-        extra_info={
-            "url": item.get("url"),
-        },
-    )
-
-
-ApifyDataset = download_loader("ApifyDataset")
+from llama_index.core import Document
+from llama_index.readers.apify import ApifyDataset
 
 reader = ApifyDataset("<Your Apify API token>")
 documents = reader.load_data(
     dataset_id="<Apify Dataset ID>",
-    dataset_mapping_function=tranform_dataset_item,
+    dataset_mapping_function=lambda item: Document(
+        text=item.get("text"),
+        metadata={
+            "url": item.get("url"),
+        },
+    ),
 )
 ```
+
```

### Comparing `llama_index_readers_apify-0.1.3/llama_index/readers/apify/actor/base.py` & `llama_index_readers_apify-0.1.4/llama_index/readers/apify/actor/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,21 @@
     """
 
     def __init__(self, apify_api_token: str) -> None:
         """Initialize the Apify Actor reader."""
         from apify_client import ApifyClient
 
         self.apify_api_token = apify_api_token
-        self.apify_client = ApifyClient(apify_api_token)
+
+        client = ApifyClient(apify_api_token)
+        if hasattr(client.http_client, "httpx_client"):
+            client.http_client.httpx_client.headers[
+                "user-agent"
+            ] += "; Origin/llama_index"
+        self.apify_client = client
 
     def load_data(
         self,
         actor_id: str,
         run_input: Dict,
         dataset_mapping_function: Callable[[Dict], Document],
         *,
```

### Comparing `llama_index_readers_apify-0.1.3/llama_index/readers/apify/dataset/base.py` & `llama_index_readers_apify-0.1.4/llama_index/readers/apify/dataset/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,21 @@
         apify_api_token (str): Apify API token.
     """
 
     def __init__(self, apify_api_token: str) -> None:
         """Initialize Apify dataset reader."""
         from apify_client import ApifyClient
 
-        self.apify_client = ApifyClient(apify_api_token)
+        client = ApifyClient(apify_api_token)
+        if hasattr(client.http_client, "httpx_client"):
+            client.http_client.httpx_client.headers[
+                "user-agent"
+            ] += "; Origin/llama_index"
+
+        self.apify_client = client
 
     def load_data(
         self, dataset_id: str, dataset_mapping_function: Callable[[Dict], Document]
     ) -> List[Document]:
         """Load data from the Apify dataset.
 
         Args:
```

### Comparing `llama_index_readers_apify-0.1.3/pyproject.toml` & `llama_index_readers_apify-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 description = "llama-index readers apify integration"
 exclude = ["**/BUILD"]
 keywords = ["apify", "crawler", "scraper", "scraping"]
 license = "MIT"
 maintainers = ["drobnikj"]
 name = "llama-index-readers-apify"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 apify-client = "^1.6.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_readers_apify-0.1.3/PKG-INFO` & `llama_index_readers_apify-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-Metadata-Version: 2.1
-Name: llama-index-readers-apify
-Version: 0.1.3
-Summary: llama-index readers apify integration
-License: MIT
-Keywords: apify,crawler,scraper,scraping
-Author: Your Name
-Author-email: you@example.com
-Maintainer: drobnikj
-Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: apify-client (>=1.6.2,<2.0.0)
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Description-Content-Type: text/markdown
-
 # Apify Loaders
 
+```bash
+pip install llama-index-readers-apify
+```
+
 ## Apify Actor Loader
 
 [Apify](https://apify.com/) is a cloud platform for web scraping and data extraction,
 which provides an [ecosystem](https://apify.com/store) of more than a thousand
 ready-made apps called _Actors_ for various scraping, crawling, and extraction use cases.
 
 This loader runs a specific Actor and loads its results.
@@ -36,44 +20,36 @@
 The extracted text then can be fed to a vector index or language model like GPT
 in order to answer questions from it.
 
 To use this loader, you need to have a (free) Apify account
 and set your [Apify API token](https://console.apify.com/account/integrations) in the code.
 
 ```python
-from llama_index import download_loader
-from llama_index.readers.schema import Document
-
-
-# Converts a single record from the Actor's resulting dataset to the LlamaIndex format
-def tranform_dataset_item(item):
-    return Document(
-        text=item.get("text"),
-        extra_info={
-            "url": item.get("url"),
-        },
-    )
-
-
-ApifyActor = download_loader("ApifyActor")
+from llama_index.core import Document
+from llama_index.readers.apify import ApifyActor
 
 reader = ApifyActor("<My Apify API token>")
+
 documents = reader.load_data(
     actor_id="apify/website-content-crawler",
     run_input={
-        "startUrls": [{"url": "https://gpt-index.readthedocs.io/en/latest"}]
+        "startUrls": [{"url": "https://docs.llamaindex.ai/en/latest/"}]
     },
-    dataset_mapping_function=tranform_dataset_item,
+    dataset_mapping_function=lambda item: Document(
+        text=item.get("text"),
+        metadata={
+            "url": item.get("url"),
+        },
+    ),
 )
 ```
 
 This loader is designed to be used as a way to load data into
 [LlamaIndex](https://github.com/run-llama/llama_index/tree/main/llama_index) and/or subsequently
 used as a Tool in a [LangChain](https://github.com/hwchase17/langchain) Agent.
-See [here](https://github.com/emptycrown/llama-hub/tree/main) for examples.
 
 ## Apify Dataset Loader
 
 [Apify](https://apify.com/) is a cloud platform for web scraping and data extraction,
 which provides an [ecosystem](https://apify.com/store) of more than a thousand
 ready-made apps called _Actors_ for various scraping, crawling, and extraction use cases.
 
@@ -88,30 +64,21 @@
 The extracted text then can be fed to a vector index or language model like GPT
 in order to answer questions from it.
 
 To use this loader, you need to have a (free) Apify account
 and set your [Apify API token](https://console.apify.com/account/integrations) in the code.
 
 ```python
-from llama_index import download_loader
-from llama_index.readers.schema import Document
-
-
-# Converts a single record from the Apify dataset to the LlamaIndex format
-def tranform_dataset_item(item):
-    return Document(
-        text=item.get("text"),
-        extra_info={
-            "url": item.get("url"),
-        },
-    )
-
-
-ApifyDataset = download_loader("ApifyDataset")
+from llama_index.core import Document
+from llama_index.readers.apify import ApifyDataset
 
 reader = ApifyDataset("<Your Apify API token>")
 documents = reader.load_data(
     dataset_id="<Apify Dataset ID>",
-    dataset_mapping_function=tranform_dataset_item,
+    dataset_mapping_function=lambda item: Document(
+        text=item.get("text"),
+        metadata={
+            "url": item.get("url"),
+        },
+    ),
 )
 ```
-
```

