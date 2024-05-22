# Comparing `tmp/langgraph_sdk-0.1.8.tar.gz` & `tmp/langgraph_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph_sdk-0.1.8.tar", max compression
+gzip compressed data, was "langgraph_sdk-0.1.9.tar", max compression
```

## Comparing `langgraph_sdk-0.1.8.tar` & `langgraph_sdk-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       12 2024-05-02 00:35:49.778092 langgraph_sdk-0.1.8/README.md
--rw-r--r--   0        0        0       70 2024-05-02 17:41:01.189167 langgraph_sdk-0.1.8/langgraph_sdk/__init__.py
--rw-r--r--   0        0        0    11521 2024-05-10 23:22:35.925150 langgraph_sdk-0.1.8/langgraph_sdk/client.py
--rw-r--r--   0        0        0     3212 2024-05-03 18:21:58.272136 langgraph_sdk-0.1.8/langgraph_sdk/schema.py
--rw-r--r--   0        0        0     1004 2024-05-11 00:20:29.377803 langgraph_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-05-08 04:47:04.090972 langgraph_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0       70 2024-05-08 04:47:04.091058 langgraph_sdk-0.1.9/langgraph_sdk/__init__.py
+-rw-r--r--   0        0        0    12542 2024-05-16 14:18:07.451140 langgraph_sdk-0.1.9/langgraph_sdk/client.py
+-rw-r--r--   0        0        0     3212 2024-05-08 04:47:04.091240 langgraph_sdk-0.1.9/langgraph_sdk/schema.py
+-rw-r--r--   0        0        0     1004 2024-05-16 14:34:46.347492 langgraph_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 langgraph_sdk-0.1.9/PKG-INFO
```

### Comparing `langgraph_sdk-0.1.8/langgraph_sdk/client.py` & `langgraph_sdk-0.1.9/langgraph_sdk/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,14 +85,28 @@
             body = (await r.aread()).decode()
             if sys.version_info >= (3, 11):
                 e.add_note(body)
             logger.error(f"Error from langgraph-api: {body}", exc_info=e)
             raise e
         return await decode_json(r)
 
+    async def patch(self, path: str, *, json: dict) -> dict:
+        """Make a PATCH request."""
+        headers, content = await encode_json(json)
+        r = await self.client.patch(path, headers=headers, content=content)
+        try:
+            r.raise_for_status()
+        except httpx.HTTPStatusError as e:
+            body = (await r.aread()).decode()
+            if sys.version_info >= (3, 11):
+                e.add_note(body)
+            logger.error(f"Error from langgraph-api: {body}", exc_info=e)
+            raise e
+        return await decode_json(r)
+
     async def delete(self, path: str) -> None:
         """Make a DELETE request."""
         r = await self.client.delete(path)
         try:
             r.raise_for_status()
         except httpx.HTTPStatusError as e:
             body = (await r.aread()).decode()
@@ -255,14 +269,29 @@
             thread_id_ = thread_id
             config = None
         return await self.http.post(
             f"/threads/{thread_id_}/state",
             json={"values": values, "config": config, "as_node": as_node},
         )
 
+    async def patch_state(
+        self,
+        thread_id: Union[str, Config],
+        metadata: dict,
+    ) -> None:
+        """Patch the state of a thread."""
+        if isinstance(thread_id, dict):
+            thread_id_: str = thread_id["configurable"]["thread_id"]
+        else:
+            thread_id_ = thread_id
+        return await self.http.patch(
+            f"/threads/{thread_id_}/state",
+            json={"metadata": metadata},
+        )
+
     async def get_history(
         self, thread_id: str, limit: int = 10, before: Optional[Config] = None
     ) -> list[dict]:
         """Get the history of a thread."""
         return await self.http.get(
             f"/threads/{thread_id}/history", params={"limit": limit, "before": before}
         )
```

### Comparing `langgraph_sdk-0.1.8/langgraph_sdk/schema.py` & `langgraph_sdk-0.1.9/langgraph_sdk/schema.py`

 * *Files identical despite different names*

### Comparing `langgraph_sdk-0.1.8/pyproject.toml` & `langgraph_sdk-0.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langgraph-sdk"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Nuno Campos <nuno@langchain.dev>"]
 readme = "README.md"
 packages = [{include = "langgraph_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.9.0,<4.0"
```

### Comparing `langgraph_sdk-0.1.8/PKG-INFO` & `langgraph_sdk-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langgraph-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Nuno Campos
 Author-email: nuno@langchain.dev
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

