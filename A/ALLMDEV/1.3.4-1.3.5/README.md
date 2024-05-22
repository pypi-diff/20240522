# Comparing `tmp/ALLMDEV-1.3.4-py3-none-any.whl.zip` & `tmp/ALLMDEV-1.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 26062 bytes, number of entries: 22
+Zip file size: 26441 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-17 06:01 ALLMDEV/__init__.py
 -rw-rw-rw-  2.0 fat     3706 b- defN 24-May-04 14:17 ALLMDEV/agentapi.py
 -rw-rw-rw-  2.0 fat     3440 b- defN 24-Apr-27 08:48 ALLMDEV/agentchat.py
 -rw-rw-rw-  2.0 fat     4986 b- defN 24-May-11 17:03 ALLMDEV/azureagentapi.py
 -rw-rw-rw-  2.0 fat     3298 b- defN 24-May-11 16:47 ALLMDEV/azureagentchat.py
 -rw-rw-rw-  2.0 fat     2435 b- defN 24-May-11 16:47 ALLMDEV/azurecli.py
--rw-rw-rw-  2.0 fat    21141 b- defN 24-May-18 15:40 ALLMDEV/backend.py
+-rw-rw-rw-  2.0 fat    21304 b- defN 24-May-22 04:58 ALLMDEV/backend.py
 -rw-rw-rw-  2.0 fat     3221 b- defN 24-May-15 11:30 ALLMDEV/cli.py
 -rw-rw-rw-  2.0 fat    12685 b- defN 24-May-15 08:32 ALLMDEV/instruct.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-Apr-27 08:57 ALLMDEV/newagent.py
--rw-rw-rw-  2.0 fat     1432 b- defN 24-May-15 08:34 ALLMDEV/serve.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 24-May-22 04:35 ALLMDEV/serve.py
 -rw-rw-rw-  2.0 fat     1932 b- defN 24-May-15 12:35 ALLMDEV/studio.py
 -rw-rw-rw-  2.0 fat      683 b- defN 24-May-04 14:32 ALLMDEV/test.py
 -rw-rw-rw-  2.0 fat     3096 b- defN 24-May-05 07:54 ALLMDEV/updateagent.py
 -rw-rw-rw-  2.0 fat     4530 b- defN 24-May-11 16:47 ALLMDEV/vertexagentapi.py
 -rw-rw-rw-  2.0 fat     2826 b- defN 24-May-14 10:42 ALLMDEV/vertexagentchat.py
 -rw-rw-rw-  2.0 fat     2126 b- defN 24-May-14 10:42 ALLMDEV/vertexcli.py
--rw-rw-rw-  2.0 fat     6060 b- defN 24-May-18 15:41 ALLMDEV-1.3.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-18 15:41 ALLMDEV-1.3.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      591 b- defN 24-May-18 15:41 ALLMDEV-1.3.4.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        8 b- defN 24-May-18 15:41 ALLMDEV-1.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1698 b- defN 24-May-18 15:41 ALLMDEV-1.3.4.dist-info/RECORD
-22 files, 83121 bytes uncompressed, 23358 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat     6093 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      591 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        8 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1698 b- defN 24-May-22 08:35 ALLMDEV-1.3.5.dist-info/RECORD
+22 files, 84116 bytes uncompressed, 23737 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: ALLMDEV/vertexagentchat.py
 Comment: 
 
 Filename: ALLMDEV/vertexcli.py
 Comment: 
 
-Filename: ALLMDEV-1.3.4.dist-info/METADATA
+Filename: ALLMDEV-1.3.5.dist-info/METADATA
 Comment: 
 
-Filename: ALLMDEV-1.3.4.dist-info/WHEEL
+Filename: ALLMDEV-1.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: ALLMDEV-1.3.4.dist-info/entry_points.txt
+Filename: ALLMDEV-1.3.5.dist-info/entry_points.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.4.dist-info/top_level.txt
+Filename: ALLMDEV-1.3.5.dist-info/top_level.txt
 Comment: 
 
-Filename: ALLMDEV-1.3.4.dist-info/RECORD
+Filename: ALLMDEV-1.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ALLMDEV/backend.py

```diff
@@ -1,34 +1,35 @@
-from fastapi import FastAPI, WebSocket, Request
+from fastapi import FastAPI, WebSocket, Request, File, UploadFile, Form
 from flask import request
 from pydantic import BaseModel
 from llama_index.llms.llama_cpp import LlamaCPP
 from langchain.embeddings import SentenceTransformerEmbeddings
 from langchain.vectorstores import Chroma
 import asyncio
 import os
 import json
 from fastapi.middleware.cors import CORSMiddleware
 import vertexai
 from vertexai.generative_models import GenerativeModel
 from openai import AzureOpenAI
-from fastapi import FastAPI, File, UploadFile, Form
 from fastapi.responses import JSONResponse
 from langchain.document_loaders import CSVLoader, PDFMinerLoader, TextLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
-from typing import Annotated
+from fastapi import FastAPI
+from fastapi.middleware.cors import CORSMiddleware
+
 
-app = FastAPI()
 
 app = FastAPI()
 
-# Add CORS middleware
+
+
 app.add_middleware(
     CORSMiddleware,
-    allow_origins=["http://localhost:5173"],
+    allow_origins=["*"],  # Replace with your frontend's origin
     allow_credentials=True,
     allow_methods=["*"],
     allow_headers=["*"],
 )
 
 
 max_new_tokens = 512
@@ -335,14 +336,16 @@
                 docs = db.similarity_search(prompt, k=3)
                 context = docs[0].page_content
                 prompt_template = "You are a friendly assistant, who gives context aware responses on user query. Kindly analyse the provided context and give proper response\n   Context: {context}\n query:<s>[INST] {prompt} [/INST]"
                 prompt = prompt_template.format(context=context, prompt=prompt)
                 response = multimodal_model.generate_content(prompt)
                 await websocket.send_text(response.text)
 
+            
+
 
             # model_kwargs = {"n_gpu_layers" : -1 if config["gpu"] else 0}
             # llm = LlamaCPP(
             #     model_path=config["model_path"],
             #     temperature=config["temperature"],
             #     max_new_tokens=max_new_tokens,
             #     context_window=3900,
@@ -481,18 +484,18 @@
     finally:
         await websocket.close()
 
 
 # class RequestData(BaseModel):
 #     agent: str
 #     file: UploadFile
-@app.route("/create_agent", methods=["POST"])
-async def upload_file(agent: Annotated[str, Form()], file: UploadFile):
+@app.post("/create_agent")
+async def upload_file(name: str = Form(...),file: UploadFile = File(...)):
         try:
-            agentname = agent
+            agentname = name
             uploaded_file = file
             # Process the uploaded file
             # Example: Save the file locally
             if not os.path.exists("uploads"):
                 os.mkdir("uploads")
             file_path = f"uploads/{uploaded_file.filename}"
             with open(file_path, "wb") as file_object:
@@ -529,32 +532,37 @@
             doc_ids_path = os.path.join(agent_directory, f"{agentname}_docids.txt")
 
             # Store document IDs in a file
             with open(doc_ids_path, "a") as f:
                 for text_id, _ in enumerate(texts):
                     document_id = f"doc_{text_id}"
                     f.write(f"{document_id}\n")
-            return JSONResponse(content={"agentname": agent_directory, "message": "agent created successfully"}) 
+            return JSONResponse(content={"agentname": name, "message": "agent created successfully"}) 
         
 
 
 
         except Exception as e:
             print(e)
 
 @app.websocket("/configdata")
 async def websocket_endpoint(websocket: WebSocket):
     await websocket.accept()
     try:
-        config=load_config()
-        azure_config=load_azure_config()
-        vertex_config=load_vertex_config()
-        await websocket.send_json(config)
-        await websocket.send_json(azure_config)
-        await websocket.send_json(vertex_config)
+        data = await websocket.receive_json()
+        print(data)
+        if data == "Azure":
+            azure_config=load_azure_config()
+            await websocket.send_json(azure_config)
+        elif data == "Vertex":
+            vertex_config=load_vertex_config()
+            await websocket.send_json(vertex_config)
+        else:
+            config=load_config()
+            await websocket.send_json(config)
 
     except Exception as e:
         print(e)
     finally:
         await websocket.close()
 
 def main():
```

## ALLMDEV/serve.py

```diff
@@ -1,10 +1,11 @@
-from flask import Flask
+from flask import Flask, request, jsonify
 from .instruct import load_model, api_serve
 import os
+from llama_index.llms.llama_cpp import LlamaCPP
 import json
 
 app = Flask(__name__)
 
 model_dir = "model"
 
 config = {
@@ -15,17 +16,41 @@
 }
 
 file_path=os.path.join(model_dir, "apiconfig.json")
 if not os.path.exists(file_path):
     with open(file_path, "w") as json_file:
         json.dump(config, json_file)
 
+
+model_files = [f for f in os.listdir('model') if f.endswith('.gguf')]
+model_path = load_model(model_files[0]) if model_files else None
+
+llm = LlamaCPP(
+    model_path=model_path,
+    temperature=0.1,
+    max_new_tokens=512,
+    context_window=3900,
+    model_kwargs={"n_gpu_layers": 0},
+    verbose=False,
+)
+
 @app.route('/v1/chat/completions', methods=['POST'])
 def chat():
-    api_serve()
+    user_input = request.json.get("input")
+
+    if user_input.lower() == "exit":
+        return jsonify({"response": "Exiting chat."})
+
+    prompt_template = "<s>[INST] {prompt} [/INST]"
+    prompt = prompt_template.format(prompt=user_input)
+
+    response_iter = llm.stream_complete(prompt)
+    response_text = ''.join(response.delta for response in response_iter)
+
+    return jsonify({"response": response_text})
 
 def main():
         with open(file_path, "r") as json_file:
             config = json.load(json_file)
             host=config["host"]
             port=config["port"]
             cert_file=config["cert_file"]
```

## Comparing `ALLMDEV-1.3.4.dist-info/METADATA` & `ALLMDEV-1.3.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ALLMDEV
-Version: 1.3.4
+Version: 1.3.5
 Summary: A simple and efficient python library for fast inference of GGUF Large Language Models.
 Author: All Advance AI
 Author-email: allmdev@allaai.com
 Maintainer: Soham Ghadge
 Maintainer-email: soham.ghadge@allaai.com
 Keywords: GGUF,GGUF Large Language Model,GGUF Large Language Models,GGUF Large Language Modeling,GGUF Large Language Modeling Library
 Description-Content-Type: text/markdown
@@ -19,14 +19,15 @@
 Requires-Dist: chromadb ==0.3.26
 Requires-Dist: pdfminer.six
 Requires-Dist: pydantic ==1.10.13
 Requires-Dist: sentence-transformers
 Requires-Dist: vertexai
 Requires-Dist: google-cloud-aiplatform
 Requires-Dist: openai
+Requires-Dist: python-multipart
 
 # ALLM
 
 ALLM is a Python library designed for fast inference of GGUF (Generic Global Unsupervised Features) Large Language Models (LLMs) on both CPU and GPU. It provides a convenient interface for loading pre-trained GGUF models and performing inference using them. This library is ideal for applications where quick response times are crucial, such as chatbots, text generation, and more.
 
 ## Features
```

## Comparing `ALLMDEV-1.3.4.dist-info/entry_points.txt` & `ALLMDEV-1.3.5.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `ALLMDEV-1.3.4.dist-info/RECORD` & `ALLMDEV-1.3.5.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ALLMDEV/__init__.py,sha256=8XSO2SVH9cZ_Iut8rNwcDxtEaBp4LIdXP6hAKGRgeaI,39
 ALLMDEV/agentapi.py,sha256=vnkpCaviW0w5EQTE99els4Nb8QABv0TgNoP2FdFsWVQ,3706
 ALLMDEV/agentchat.py,sha256=UHLn4mVEBz6C77G8aaf3DWrzuVPfA-PCEp6uFZpcGyM,3440
 ALLMDEV/azureagentapi.py,sha256=dzMwkJHfRBqRxYAwpe_aQRgASqnsNBaEzT9jsc791QQ,4986
 ALLMDEV/azureagentchat.py,sha256=6L9m2B6dfe9LUWdd_Vj6_TT1n1GBXxVvqOeA-yTuV_Q,3298
 ALLMDEV/azurecli.py,sha256=nLoSVPpxWwIJWhiddB0_qzNw53hrAE6ijK0diDlaGYs,2435
-ALLMDEV/backend.py,sha256=cK_F9Dhi5m_AZTej9K_VeWQ71iA6lstw7OnhH8xQE58,21141
+ALLMDEV/backend.py,sha256=01c2CYAhM4jdKfld2A06i0UnfL-48bfEy-9QR8MIaVU,21304
 ALLMDEV/cli.py,sha256=13o2i7g_DtOyP8N8x7QdMr8iUGr4raJX26NJ9oqpgNw,3221
 ALLMDEV/instruct.py,sha256=-3ybhrmAwgLy_MptpJHhFnbQq1NcT4DHeMV2-46Tzl8,12685
 ALLMDEV/newagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
-ALLMDEV/serve.py,sha256=Pv5L5mMVcBeHttoNLQmrE43NBLjEQW7RUYU47RrwMrc,1432
+ALLMDEV/serve.py,sha256=RUKwji_795izII7XlYku1KUK6bvgR_SYBB9N34GwqUA,2231
 ALLMDEV/studio.py,sha256=LlrIEWcs-o8cIjnprJVijR8cNxrOsnFvl9AgTrk43iw,1932
 ALLMDEV/test.py,sha256=CxP_WW9ZXEiLCJh_9MLdieFU-yfNMwWlXrcrs7gtXx8,683
 ALLMDEV/updateagent.py,sha256=BzdKTA6gutbZbJS3nL1aWZqmTxe7QABkrLz9zpxlQZc,3096
 ALLMDEV/vertexagentapi.py,sha256=fPbLJoy8Wirh7wPc31EzlgLSqfF2e4PkEwYCO9h4yqk,4530
 ALLMDEV/vertexagentchat.py,sha256=dYvJ2_teBGeEN3TTrXq4pSulYJW5kmNPKFa9xg9ec9s,2826
 ALLMDEV/vertexcli.py,sha256=-5BgOKO7oMsjcsJRluAM0ivWllzpBpWmVQIzHbq_Xrk,2126
-ALLMDEV-1.3.4.dist-info/METADATA,sha256=l-7tnsLgU0nujd-WTPTSETKJcg9-5ykuiA0TBwVVawU,6060
-ALLMDEV-1.3.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ALLMDEV-1.3.4.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
-ALLMDEV-1.3.4.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
-ALLMDEV-1.3.4.dist-info/RECORD,,
+ALLMDEV-1.3.5.dist-info/METADATA,sha256=Rcy8ENFYB-53J9q82bog0Jl3TR8W9VAPTz-R1hC46KU,6093
+ALLMDEV-1.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ALLMDEV-1.3.5.dist-info/entry_points.txt,sha256=u71vTXywZkZgH8fa1luPKfAsQCbItzqCHI6DgWpJGH4,591
+ALLMDEV-1.3.5.dist-info/top_level.txt,sha256=zQYMpzphh7BJt_BseuV6ImX-bYvNZcuXsmNLbIr57Ts,8
+ALLMDEV-1.3.5.dist-info/RECORD,,
```

