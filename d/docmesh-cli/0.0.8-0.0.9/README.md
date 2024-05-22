# Comparing `tmp/docmesh_cli-0.0.8.tar.gz` & `tmp/docmesh_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_cli-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_cli-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_cli-0.0.8.tar` & `docmesh_cli-0.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.8/README.md
--rw-r--r--   0        0        0       83 2024-05-20 03:20:54.906887 docmesh_cli-0.0.8/docmesh_cli/__init__.py
--rw-r--r--   0        0        0     8264 2024-05-20 03:20:17.042021 docmesh_cli-0.0.8/docmesh_cli/client.py
--rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.8/docmesh_cli/logos.py
--rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       17 2024-05-10 11:02:39.301355 docmesh_cli-0.0.9/README.md
+-rw-r--r--   0        0        0       83 2024-05-20 07:06:58.796246 docmesh_cli-0.0.9/docmesh_cli/__init__.py
+-rw-r--r--   0        0        0     8404 2024-05-20 07:06:06.631136 docmesh_cli-0.0.9/docmesh_cli/client.py
+-rw-r--r--   0        0        0     3896 2024-05-11 05:09:55.588764 docmesh_cli-0.0.9/docmesh_cli/logos.py
+-rw-r--r--   0        0        0      598 2024-05-10 11:02:39.301355 docmesh_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      418 1970-01-01 00:00:00.000000 docmesh_cli-0.0.9/PKG-INFO
```

### Comparing `docmesh_cli-0.0.8/docmesh_cli/client.py` & `docmesh_cli-0.0.9/docmesh_cli/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 SHORTCUTS = {
     "/add": {
         "path": "/add_paper",
         "args": "paper",
         "description": "add a new paper, usage: /add PAPER_TITLE/ARXIV_ID",
     },
     "/mark": {
-        "path": "/mark_paper",
-        "args": "paper_id",
-        "description": "read a paper, usage: /mark PAPER_ID",
+        "path": "/add_and_mark_paper",
+        "args": "paper",
+        "description": "add and mark a paper read, usage: /mark PAPER_TITLE/ARXIV_ID",
     },
     "/help": {
         "description": "show this help menu",
     },
     "/clear": {
         "description": "clear the session memory",
     },
@@ -236,21 +236,21 @@
             data = {"session_id": session_id, "query": query}
             if streaming:
                 chunks: list[bytes] = []
                 with requests.post(
                     url=f"{server}/async_agent", headers=headers, json=data, stream=True, timeout=300
                 ) as r:
                     for chunk in r.iter_content(chunk_size=64):
+                        # some special symbol may be splitted by chunk size
+                        # so we use a temporal chunks to store these part
+                        # and we will try to decode these chunks asap
+                        chunks.append(chunk)
                         try:
-                            if chunks:
-                                s = b"".join(chunks.append(chunk)).decode()
-                            else:
-                                s = chunk.decode()
-
+                            s = b"".join(chunks).decode()
                             chunks = []
                             print(s, end="", flush=True)
                         except UnicodeDecodeError:
-                            chunks.append(chunk)
+                            continue
             else:
                 rsp = requests.post(url=f"{server}/agent", headers=headers, json=data, timeout=300)
                 msg = rsp.json()["data"]["msg"]
                 print(msg, end="", flush=True)
```

### Comparing `docmesh_cli-0.0.8/docmesh_cli/logos.py` & `docmesh_cli-0.0.9/docmesh_cli/logos.py`

 * *Files identical despite different names*

### Comparing `docmesh_cli-0.0.8/pyproject.toml` & `docmesh_cli-0.0.9/pyproject.toml`

 * *Files identical despite different names*

