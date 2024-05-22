# Comparing `tmp/causadb-1.8.8.tar.gz` & `tmp/causadb-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.8.8.tar", max compression
+gzip compressed data, was "causadb-1.9.0.tar", max compression
```

## Comparing `causadb-1.8.8.tar` & `causadb-1.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1066 2024-04-11 17:25:23.978112 causadb-1.8.8/LICENSE
--rw-r--r--   0        0        0     1167 2024-04-11 17:25:23.978112 causadb-1.8.8/README.md
--rw-r--r--   0        0        0      115 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-04-11 17:25:53.470067 causadb-1.8.8/causadb/__version__.py
--rw-r--r--   0        0        0     5338 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/causadb.py
--rw-r--r--   0        0        0     2109 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/cli/account.py
--rw-r--r--   0        0        0     3153 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/cli/data.py
--rwxr-xr-x   0        0        0      962 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/cli/main.py
--rw-r--r--   0        0        0     7104 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/cli/utils.py
--rw-r--r--   0        0        0     2646 2024-04-11 17:25:23.978112 causadb-1.8.8/causadb/data.py
--rw-r--r--   0        0        0        0 2024-04-11 17:25:23.982112 causadb-1.8.8/causadb/examples/__init__.py
--rw-r--r--   0        0        0     1876 2024-04-11 17:25:23.982112 causadb-1.8.8/causadb/examples/heating.py
--rw-r--r--   0        0        0    15743 2024-04-11 17:25:23.982112 causadb-1.8.8/causadb/model.py
--rw-r--r--   0        0        0     2555 2024-04-11 17:25:23.982112 causadb-1.8.8/causadb/plotting.py
--rw-r--r--   0        0        0      215 2024-04-11 17:25:23.982112 causadb-1.8.8/causadb/utils.py
--rw-r--r--   0        0        0      797 2024-04-11 17:25:51.962070 causadb-1.8.8/pyproject.toml
--rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 causadb-1.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-23 08:53:31.446915 causadb-1.9.0/LICENSE
+-rw-r--r--   0        0        0     1167 2024-04-23 08:53:31.446915 causadb-1.9.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-23 08:54:03.727219 causadb-1.9.0/causadb/__version__.py
+-rw-r--r--   0        0        0     5338 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/causadb.py
+-rw-r--r--   0        0        0     2109 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/cli/account.py
+-rw-r--r--   0        0        0     3153 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      962 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/cli/main.py
+-rw-r--r--   0        0        0     7104 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/data.py
+-rw-r--r--   0        0        0        0 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/examples/__init__.py
+-rw-r--r--   0        0        0     1876 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/examples/heating.py
+-rw-r--r--   0        0        0    15819 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/model.py
+-rw-r--r--   0        0        0     2555 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/plotting.py
+-rw-r--r--   0        0        0      215 2024-04-23 08:53:31.446915 causadb-1.9.0/causadb/utils.py
+-rw-r--r--   0        0        0      797 2024-04-23 08:54:02.759210 causadb-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2181 1970-01-01 00:00:00.000000 causadb-1.9.0/PKG-INFO
```

### Comparing `causadb-1.8.8/LICENSE` & `causadb-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/README.md` & `causadb-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/causadb.py` & `causadb-1.9.0/causadb/causadb.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/cli/account.py` & `causadb-1.9.0/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/cli/data.py` & `causadb-1.9.0/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/cli/main.py` & `causadb-1.9.0/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/cli/models.py` & `causadb-1.9.0/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/cli/utils.py` & `causadb-1.9.0/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/data.py` & `causadb-1.9.0/causadb/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/examples/heating.py` & `causadb-1.9.0/causadb/examples/heating.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/causadb/model.py` & `causadb-1.9.0/causadb/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
 
         if "outcome" in response:
             return pd.DataFrame.from_dict(response["outcome"])
 
         raise Exception("CausaDB server request failed - unexpected response.")
 
     @validate_call
-    def find_best_actions(self, targets: dict[str, float], actionable: list[str], fixed: dict[str, float] = {}) -> pd.DataFrame:
+    def find_best_actions(self, targets: dict[str, float], actionable: list[str], fixed: dict[str, float] = {}, constraints: dict[str, tuple] = {}) -> pd.DataFrame:
         """Get the optimal actions for a given set of target outcomes.
 
         Args:
             targets (dict[str, float]): A dictionary representing the target outcomes.
             actionable (list[str]): A list of actionable nodes.
             fixed (dict[str, float]): A dictionary representing the fixed nodes.
 
@@ -402,15 +402,16 @@
             ...     {"y": 0.5}
         """
         headers = {"token": self.client.token}
 
         query = {
             "targets": targets,
             "actionable": actionable,
-            "fixed": fixed
+            "fixed": fixed,
+            "constraints": constraints
         }
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/find-best-actions",
                 headers=headers,
                 json=query,
```

### Comparing `causadb-1.8.8/causadb/plotting.py` & `causadb-1.9.0/causadb/plotting.py`

 * *Files identical despite different names*

### Comparing `causadb-1.8.8/pyproject.toml` & `causadb-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.8.8"
+version = "1.9.0"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.8.8/PKG-INFO` & `causadb-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.8.8
+Version: 1.9.0
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

