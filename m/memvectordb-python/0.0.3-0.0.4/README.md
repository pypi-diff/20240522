# Comparing `tmp/memvectordb_python-0.0.3.tar.gz` & `tmp/memvectordb_python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memvectordb_python-0.0.3.tar", max compression
+gzip compressed data, was "memvectordb_python-0.0.4.tar", max compression
```

## Comparing `memvectordb_python-0.0.3.tar` & `memvectordb_python-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2042 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/memvectordb/__init__.py
--rw-r--r--   0        0        0     8103 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/memvectordb/collection.py
--rw-r--r--   0        0        0      445 2024-05-20 07:46:07.387898 memvectordb_python-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 memvectordb_python-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2042 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/memvectordb/__init__.py
+-rw-r--r--   0        0        0     8100 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/memvectordb/collection.py
+-rw-r--r--   0        0        0      445 2024-05-22 16:42:04.800517 memvectordb_python-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 memvectordb_python-0.0.4/PKG-INFO
```

### Comparing `memvectordb_python-0.0.3/README.md` & `memvectordb_python-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `memvectordb_python-0.0.3/memvectordb/collection.py` & `memvectordb_python-0.0.4/memvectordb/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             dict: Information about the collection.
         """
         payload = {
             "collection_name": collection_name
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/get_collection"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.get(url, json=payload, headers=headers)
 
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             return response_data
         
@@ -85,15 +85,15 @@
             dict: Confirmation statement.
         """
         payload = {
             "collection_name": collection_name
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/delete_collection"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.delete(url, json=payload, headers=headers)
 
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             return response_data
 
@@ -123,15 +123,15 @@
         }
         payload = {
             "collection_name": collection_name,
             "embedding": embedding
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/insert_embeddings"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.put(url, json=payload, headers=headers)
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             raise Exception(f"Failed to insert embedding: {response.status_code}")
         
     def batch_insert_embeddings(
@@ -176,15 +176,15 @@
         """
         payload = {
             "collection_name": collection_name,
             "embeddings": embeddings
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/batch_insert_embeddings"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.put(url, json=payload, headers=headers)
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             raise Exception(f"Failed to insert embedding: {response_data}")
 
     def get_embeddings(
@@ -201,15 +201,15 @@
             List[Dict[str, Any]]: A list of dictionaries representing the retrieved embeddings.
         """
         payload = {
             "collection_name": collection_name
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/get_embeddings"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.get(url, json=payload, headers=headers)
 
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             return response_data
         
@@ -233,14 +233,14 @@
         payload = {
             "collection_name": collection_name,
             "query_vector": query_vector,
             "k": k
         }
         headers = {"Content-Type": "application/json"}
         url = f"{self.base_url}/get_similarity"
-        response = requests.post(url, json=payload, headers=headers)
+        response = requests.get(url, json=payload, headers=headers)
 
         response_data = response.json()
         if response.status_code == 200:
             return response_data
         else:
             return response_data
```

### Comparing `memvectordb_python-0.0.3/PKG-INFO` & `memvectordb_python-0.0.4/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memvectordb-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: memvectordb python client.
 Home-page: https://github.com/KevKibe/memvectordb-python-client
 License: MIT
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

