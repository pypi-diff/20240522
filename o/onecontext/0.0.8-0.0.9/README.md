# Comparing `tmp/onecontext-0.0.8.tar.gz` & `tmp/onecontext-0.0.9.tar.gz`

## Comparing `onecontext-0.0.8.tar` & `onecontext-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 onecontext-0.0.8/src/onecontext/__about__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 onecontext-0.0.8/src/onecontext/__init__.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 onecontext-0.0.8/src/onecontext/api.py
--rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 onecontext-0.0.8/src/onecontext/core.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 onecontext-0.0.8/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 onecontext-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 onecontext-0.0.8/README.md
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 onecontext-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 onecontext-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 onecontext-0.0.9/src/onecontext/__about__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 onecontext-0.0.9/src/onecontext/__init__.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 onecontext-0.0.9/src/onecontext/api.py
+-rw-r--r--   0        0        0     8042 2020-02-02 00:00:00.000000 onecontext-0.0.9/src/onecontext/core.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 onecontext-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 onecontext-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 onecontext-0.0.9/README.md
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 onecontext-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 onecontext-0.0.9/PKG-INFO
```

### Comparing `onecontext-0.0.8/src/onecontext/api.py` & `onecontext-0.0.9/src/onecontext/api.py`

 * *Files identical despite different names*

### Comparing `onecontext-0.0.8/src/onecontext/core.py` & `onecontext-0.0.9/src/onecontext/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import json
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 import requests
 
 from onecontext.api import URLS, ApiClient
@@ -32,37 +33,55 @@
         name (str): The name of the knowledge bases
     """
 
     name: str
     id: Optional[str] = None
     sync_status: Optional[str] = None
 
-    def upload_file(self, file_path: Union[str, Path]) -> None:
+    def upload_file(self, file_path: Union[str, Path], metadata: Optional[dict] = None) -> None:
+
+        if metadata is not None:
+            metadata_json = json.dumps(metadata)
+        else:
+            metadata_json = None
+
         file_path = Path(file_path)
         suffix = file_path.suffix
+
         if suffix not in SUPPORTED_FILE_TYPES:
             msg = f"{suffix} files are not supported. Supported file types: {SUPPORTED_FILE_TYPES}"
             raise ValueError(msg)
 
         file_path = file_path.expanduser().resolve()
+
         with open(file_path, "rb") as file:
             files = {"files": (str(file_path), file)}
             data = {"knowledge_base_name": self.name}
+            if metadata_json:
+                data.update({"metadata_json": metadata_json})
+
             api.post(urls.upload(), data=data, files=files)
 
-    def upload_from_directory(self, directory: Union[str, Path]) -> None:
+    def upload_from_directory(self, directory: Union[str, Path], metadata: Optional[Union[dict, List[dict]]] = None) -> None:
         directory = Path(directory).expanduser().resolve()
         if not directory.is_dir():
             msg = "You must provide a direcotry"
             raise ValueError(msg)
         directory = str(directory)
         all_files = [os.path.join(directory, file) for file in os.listdir(directory)]
         files_to_upload = [file for file in all_files if file.endswith(SUPPORTED_FILE_TYPES)]
-        for file_path in files_to_upload:
-            self.upload_file(file_path)
+
+        if isinstance(metadata, list):
+            if len(metadata) != len(files_to_upload):
+                raise ValueError("Metadata list len does not match the number of files in directory")
+        else:
+            metadata = [metadata] * len(files_to_upload)
+
+        for file_path, metadata in zip(files_to_upload, metadata):
+            self.upload_file(file_path, metadata)
 
     def list_files(self) -> List[Dict[str, Any]]:
         return api.get(urls.knowledge_base_files(self.name))
 
     def get_info(self) -> None:
         info = api.get(urls.knowledge_base(self.name))
         self.sync_status = info["sync_status"]
@@ -128,17 +147,17 @@
 
     knowledge_bases: List[KnowledgeBase]
 
     def __post_init__(self):
 
         for knowledge_base in self.knowledge_bases:
             if not isinstance(knowledge_base, KnowledgeBase):
-                raise ValueError(f"knowledge_bases parameter should be a list of KnowledgeBase, recieved {type(knowledge_base)} instead.")
+                raise TypeError(f"knowledge_bases parameter should be a list of KnowledgeBase, recieved {type(knowledge_base)} instead.")
 
-    def query(self, query: str, output_k: int = 10, *, rerank_pool_size: int = 50, rerank_fast=True) -> List[Document]:
+    def query(self, query: str, output_k: int = 10, *, rerank_pool_size: int = 50, rerank_fast=True, metadata_filters: Optional[Dict] = None) -> List[Document]:
         """
 
         The preferred query method. The query pipeline is composed of two stages behind the scenes:
             1. Fast Retrieval of a larger sample set by our base model
             2. Cross-Encoder re ranking to get the most relevant results
 
         Note that only the final results are returned by the API. To access the
@@ -154,27 +173,39 @@
               the initial pool of documents to fetch in stage 1. Higher values
               increase recall at the cost of latency
             rerank_fast (bool):
                 set to False to access an experimental more powerful cross-encoder
                 pipeline. Note that this will increase latency and is often
                 not required depending on the use case. We recommend evaluating
                 the default pipeline first .
+            metadata_filters (dict):
+                used to filter the query based on metadata provided at file
+                upload.
+                eg:
+                    {"category" : "legal"}
+                will restrict the query to files with a "category" key
+                matching "legal" value
 
+                to filter the search to multiple values pass a list instead:
+                    {"category" : ["legal", "finance"]
+
+                Note: "file_name" filter is available by default. Be sure
+                to provide the full file name including the extension.
         Returns:
             list[Document] : the most relevant document chunks
         """
         params = {
             "query": query,
             "output_k": output_k,
             "knowledge_base_names": [kb.name for kb in self.knowledge_bases],
             "rerank_pool_size": rerank_pool_size,
             "rerank_fast": rerank_fast,
             "rerank": True,
+            "metadata_filters": metadata_filters
         }
-
         return self._post_query(params)
 
     def query_no_rerank(self, query: str, output_k: int = 10) -> List[Document]:
         """
         A simple single stage retrieval query.
 
         Use this method to fetch a large number of Documents with the lowest latency.
```

### Comparing `onecontext-0.0.8/.gitignore` & `onecontext-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `onecontext-0.0.8/LICENSE.txt` & `onecontext-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onecontext-0.0.8/README.md` & `onecontext-0.0.9/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 - [Quick Start](#quick-start)
 - [License](#license)
 
 -----
 
 ## LLM Context as a Service
 
-OneContext makes it easy to augment your LLM application with your own data
-in a few API calls. Simply upload your data to a Knowledge Base and directly
+OneContext makes it really easy and fast to augment your LLM application with your own data
+in a few API calls. Upload your data to a `Knowledge Base` and directly it
 query with natural languge to retrieve relevant context for your LLM application.
 
 We manage the full document processing and retrieval pipeline so that you don't have to:
 
 - document ingestion, chunking and cleaning
 - effcient vector embeddings at scale using state of the art open source models
 - low latency multi stage query pipeline to provide the most relevant context
@@ -45,15 +45,15 @@
 pip install onecontext
 ```
 
 ### Configuration
 
     export ONECONTEXT_API_KEY="YOUR_API_KEY"
 
-You can get the api key for free at  [OneContext](https://www.onecontext.ai)
+You can get an api key by joining our closed beta. Email Ross at ross@onecontext.ai to get on the list.
 
 ### Usage
 
 #### Create a Knowledge Base:
 
 ```python
 from onecontext import KnowledgeBase
@@ -72,23 +72,52 @@
 
 print(list_knowledge_bases())
 
 ```
 
 #### Upload files to the Knowledge Base:
 
+You can upload an entire directory like this:
+
 ```python
 
-my_knowledge_base = KnowledgeBase("my_knowledge_base")
+my_kb = KnowledgeBase("my_knowledge_base")
+
+directory = "/path/to/local_directory"
+
+my_kb.upload_from_directory(directory)
+```
+
+Or, you can upload an individual file like this:
+
+```python
+
+my_kb = KnowledgeBase("my_knowledge_base")
 
-directory = "/path/to/local_folder"
+my_kb.upload_file(
+    "/path/to/local_file.pdf"
+)
 
-my_knowledge_base.upload_from_directory(directory)
 ```
 
+If you like, you can also add metadata to your files. This makes it really easy to filter your query-space later on. Metadata can be any key-value pairs, passed as a dictionary. For example:
+
+```python
+
+my_kb = KnowledgeBase("my_knowledge_base")
+
+my_kb.upload_file(
+    "/path/to/local_file.pdf", metadata={"ContainsPII": True, "author": "ross", "description": "passport", "file-type": "scan", "category": "personal"}
+)
+
+```
+
+Currently, you can upload any of [.pdf, .docx, .txt] files. Don't worry if the PDF is a scan (and doesn't have easily extractable text), OneContext will figure it out via OCR.
+In the near future you'll be able to upload video, audio, and connect to multiple file-storage platforms. 
+
 Once the files have been uploaded they will be processed, chunked
 and embedded by OneContext.
 
 Check sync status:
 
 ```python
 print(my_knowledge_base.is_synced)
@@ -97,34 +126,47 @@
 #### Query the Knowledge Base
 
 
 ```python
 
 from onecontext import Retriever
 
-retriever = Retriever(knowledge_bases=[my_knowledge_base])
+retriever = Retriever(knowledge_bases=[my_kb])
 
 documents = retriever.query("what is onecontext?", output_k=20)
 
 ```
 
+And, filtering by metadata: 
+
+```python
+
+from onecontext import Retriever
+
+retriever = Retriever(knowledge_bases=[my_kb])
+
+documents = retriever.query("what is onecontext?", output_k=20, metadata_filters={"ContainsPII": True, "author": "ross"})
+
+```
+
+
 By default the query pipeline is composed of two steps:
 
 - Retrieval: fetch the larger pool of documents (rerank_pool_size)
 - Re-ranking: re-rank the results with a downstream model to get most relevant documents
 
 To improve recall you can increase the rerank_pool_size:
 
 ```python
 
 documents = retriever.query("what is onecontext?", output_k=10, rerank_pool_size=80)
 
 ```
 
-You can also skip the re-ranking step entirely:
+You can also skip the re-ranking step entirely if you want to prioritise speed over accuracy of results.
 
 ```python
 
 documents = retriever.query_no_rerank("what is onecontext?")
 
 ```
```

### Comparing `onecontext-0.0.8/pyproject.toml` & `onecontext-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `onecontext-0.0.8/PKG-INFO` & `onecontext-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onecontext
-Version: 0.0.8
+Version: 0.0.9
 Project-URL: Documentation, https://github.com/onecontext/python_sdk#readme
 Project-URL: Issues, https://github.com/onecontext/python_sdk/issues
 Project-URL: Source, https://github.com/onecontext/python_sdk
 Author-email: Serge Mosesov <smosesov@gmail.com>, Ross Murphy <ross@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -31,16 +31,16 @@
 - [Quick Start](#quick-start)
 - [License](#license)
 
 -----
 
 ## LLM Context as a Service
 
-OneContext makes it easy to augment your LLM application with your own data
-in a few API calls. Simply upload your data to a Knowledge Base and directly
+OneContext makes it really easy and fast to augment your LLM application with your own data
+in a few API calls. Upload your data to a `Knowledge Base` and directly it
 query with natural languge to retrieve relevant context for your LLM application.
 
 We manage the full document processing and retrieval pipeline so that you don't have to:
 
 - document ingestion, chunking and cleaning
 - effcient vector embeddings at scale using state of the art open source models
 - low latency multi stage query pipeline to provide the most relevant context
@@ -67,15 +67,15 @@
 pip install onecontext
 ```
 
 ### Configuration
 
     export ONECONTEXT_API_KEY="YOUR_API_KEY"
 
-You can get the api key for free at  [OneContext](https://www.onecontext.ai)
+You can get an api key by joining our closed beta. Email Ross at ross@onecontext.ai to get on the list.
 
 ### Usage
 
 #### Create a Knowledge Base:
 
 ```python
 from onecontext import KnowledgeBase
@@ -94,23 +94,52 @@
 
 print(list_knowledge_bases())
 
 ```
 
 #### Upload files to the Knowledge Base:
 
+You can upload an entire directory like this:
+
 ```python
 
-my_knowledge_base = KnowledgeBase("my_knowledge_base")
+my_kb = KnowledgeBase("my_knowledge_base")
+
+directory = "/path/to/local_directory"
+
+my_kb.upload_from_directory(directory)
+```
+
+Or, you can upload an individual file like this:
+
+```python
+
+my_kb = KnowledgeBase("my_knowledge_base")
 
-directory = "/path/to/local_folder"
+my_kb.upload_file(
+    "/path/to/local_file.pdf"
+)
 
-my_knowledge_base.upload_from_directory(directory)
 ```
 
+If you like, you can also add metadata to your files. This makes it really easy to filter your query-space later on. Metadata can be any key-value pairs, passed as a dictionary. For example:
+
+```python
+
+my_kb = KnowledgeBase("my_knowledge_base")
+
+my_kb.upload_file(
+    "/path/to/local_file.pdf", metadata={"ContainsPII": True, "author": "ross", "description": "passport", "file-type": "scan", "category": "personal"}
+)
+
+```
+
+Currently, you can upload any of [.pdf, .docx, .txt] files. Don't worry if the PDF is a scan (and doesn't have easily extractable text), OneContext will figure it out via OCR.
+In the near future you'll be able to upload video, audio, and connect to multiple file-storage platforms. 
+
 Once the files have been uploaded they will be processed, chunked
 and embedded by OneContext.
 
 Check sync status:
 
 ```python
 print(my_knowledge_base.is_synced)
@@ -119,34 +148,47 @@
 #### Query the Knowledge Base
 
 
 ```python
 
 from onecontext import Retriever
 
-retriever = Retriever(knowledge_bases=[my_knowledge_base])
+retriever = Retriever(knowledge_bases=[my_kb])
 
 documents = retriever.query("what is onecontext?", output_k=20)
 
 ```
 
+And, filtering by metadata: 
+
+```python
+
+from onecontext import Retriever
+
+retriever = Retriever(knowledge_bases=[my_kb])
+
+documents = retriever.query("what is onecontext?", output_k=20, metadata_filters={"ContainsPII": True, "author": "ross"})
+
+```
+
+
 By default the query pipeline is composed of two steps:
 
 - Retrieval: fetch the larger pool of documents (rerank_pool_size)
 - Re-ranking: re-rank the results with a downstream model to get most relevant documents
 
 To improve recall you can increase the rerank_pool_size:
 
 ```python
 
 documents = retriever.query("what is onecontext?", output_k=10, rerank_pool_size=80)
 
 ```
 
-You can also skip the re-ranking step entirely:
+You can also skip the re-ranking step entirely if you want to prioritise speed over accuracy of results.
 
 ```python
 
 documents = retriever.query_no_rerank("what is onecontext?")
 
 ```
```

