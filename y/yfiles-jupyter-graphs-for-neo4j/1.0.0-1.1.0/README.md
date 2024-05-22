# Comparing `tmp/yfiles_jupyter_graphs_for_neo4j-1.0.0.tar.gz` & `tmp/yfiles_jupyter_graphs_for_neo4j-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yfiles_jupyter_graphs_for_neo4j-1.0.0.tar", last modified: Fri Apr 19 10:02:29 2024, max compression
+gzip compressed data, was "yfiles_jupyter_graphs_for_neo4j-1.1.0.tar", last modified: Wed May 22 12:36:07 2024, max compression
```

## Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0.tar` & `yfiles_jupyter_graphs_for_neo4j-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:02:29.071726 yfiles_jupyter_graphs_for_neo4j-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 10:02:23.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-19 10:02:29.067726 yfiles_jupyter_graphs_for_neo4j-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-04-19 10:02:23.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-19 10:02:23.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 10:02:29.071726 yfiles_jupyter_graphs_for_neo4j-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:02:29.067726 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:02:29.067726 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j/
--rw-r--r--   0 runner    (1001) docker     (127)     6159 2024-04-19 10:02:23.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j/Yfiles_Neo4j_Graphs.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 10:02:23.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 10:02:29.067726 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-04-19 10:02:29.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-19 10:02:29.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 10:02:29.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 10:02:29.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-19 10:02:29.000000 yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:36:07.556906 yfiles_jupyter_graphs_for_neo4j-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 12:35:59.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-22 12:36:07.556906 yfiles_jupyter_graphs_for_neo4j-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9873 2024-05-22 12:35:59.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-22 12:35:59.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:36:07.556906 yfiles_jupyter_graphs_for_neo4j-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:36:07.552906 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:36:07.552906 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j/
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-22 12:35:59.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j/Yfiles_Neo4j_Graphs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 12:35:59.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:36:07.556906 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-22 12:36:07.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-22 12:36:07.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:36:07.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 12:36:07.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 12:36:07.000000 yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/top_level.txt
```

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/LICENSE.md` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/PKG-INFO` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfiles_jupyter_graphs_for_neo4j
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Neo4j graph visualization package that uses the yfiles-jupyter-graphs widget
 Author-email: yWorks Support Team <yfileshtml@yworks.com>
 License: MIT License
         
         Copyright (c) 2024 yWorks GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -106,14 +106,18 @@
 
 - `show_cypher(cypher, **kwargs)`
     - `cypher`: The [cypher query](https://neo4j.com/docs/cypher-manual/current/introduction/) that should be
       visualized.
     - `**kwargs`: Additional parameters that should be passed to the cypher query (e.g., see
       the [selection example](https://github.com/yWorks/yfiles-jupyter-graphs-for-neo4j/blob/main/examples/selection_example.ipynb)).
 
+The default behavior is to only show the nodes and relationships returned by the cypher query.
+This can be changed to autocomplete relationships like in neo4j browser:
+- `set_autocomplete_relationships(autocomplete_relationships)`: Sets whether to autocomplete relationships in the graph or not.
+
 The cypher queries are executed by the provided Neo4j driver. If you have not specified a driver when instantiating the
 class, you can set
 a driver afterward:
 
 - `set_driver(driver)`: Sets the given driver and uses this to send cypher queries to Databases.
 - `get_driver()`: Returns the current driver.
```

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/README.md` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,18 @@
 
 - `show_cypher(cypher, **kwargs)`
     - `cypher`: The [cypher query](https://neo4j.com/docs/cypher-manual/current/introduction/) that should be
       visualized.
     - `**kwargs`: Additional parameters that should be passed to the cypher query (e.g., see
       the [selection example](https://github.com/yWorks/yfiles-jupyter-graphs-for-neo4j/blob/main/examples/selection_example.ipynb)).
 
+The default behavior is to only show the nodes and relationships returned by the cypher query.
+This can be changed to autocomplete relationships like in neo4j browser:
+- `set_autocomplete_relationships(autocomplete_relationships)`: Sets whether to autocomplete relationships in the graph or not.
+
 The cypher queries are executed by the provided Neo4j driver. If you have not specified a driver when instantiating the
 class, you can set
 a driver afterward:
 
 - `set_driver(driver)`: Sets the given driver and uses this to send cypher queries to Databases.
 - `get_driver()`: Returns the current driver.
```

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/pyproject.toml` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yfiles_jupyter_graphs_for_neo4j"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   {name = "yWorks Support Team", email= "yfileshtml@yworks.com"},
 ]
 description = "A Neo4j graph visualization package that uses the yfiles-jupyter-graphs widget"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j/Yfiles_Neo4j_Graphs.py` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j/Yfiles_Neo4j_Graphs.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,22 +14,24 @@
 class Neo4jGraphWidget:
     _driver = None
     _node_configurations = {}
     _edge_configurations = {}
     _widget = GraphWidget()
 
     def __init__(self, driver=None, widget_layout=None,
-                 overview_enabled=None, context_start_with='About', license=None):
+                 overview_enabled=None, context_start_with='About', license=None,
+                 autocomplete_relationships=False):
         if driver is not None:
             self._driver = driver
         self._session = driver.session()
         self._license = license
         self._overview = overview_enabled
         self._layout = widget_layout
         self._context_start_with = context_start_with
+        self.set_autocomplete_relationships(autocomplete_relationships)
 
     def set_driver(self, driver):
         """
         Setter for the driver attribute.
         If a new driver is used, there is also a new session
         :param driver: neo4j._sync.driver.Neo4jDriver
 
@@ -40,21 +42,64 @@
     def get_driver(self):
         """
         Getter for the driver attribute
         :return: neo4j._sync.driver.Neo4jDriver
         """
         return self._driver
 
+    def set_autocomplete_relationships(self, autocomplete_relationships):
+        """
+        Sets the flag to enable or disable autocomplete for relationships.
+        When autocomplete is enabled, relationships are automatically completed in the graph,
+        similar to the behavior in Neo4j Browser.
+        This can be set to True/False to enable or disable for all relationships,
+        or a single relationship type or a list of relationship types to enable for specific relationships.
+        :param autocomplete_relationships: bool | str | list[str]
+        """
+        if not isinstance(autocomplete_relationships, (bool, str, list)):
+            raise ValueError("autocomplete_relationships must be a bool, a string, or a list of strings")
+        if isinstance(autocomplete_relationships, str):
+            self._autocomplete_relationships = [autocomplete_relationships]
+        else:
+            self._autocomplete_relationships = autocomplete_relationships
+
+    def _is_autocomplete_enabled(self):
+        if isinstance(self._autocomplete_relationships, bool):
+            return self._autocomplete_relationships
+        return len(self._autocomplete_relationships) > 0
+
+    def _get_relationship_types_expression(self):
+        if isinstance(self._autocomplete_relationships, list) and len(self._autocomplete_relationships) > 0:
+            return "AND type(rel) IN $relationship_types"
+        return ""
+
     def show_cypher(self, cypher, **kwargs):
         """
         main function
         :param cypher: str, Send a data query to the neo4j database
                **kwargs: variable declarations usable in cypher
         """
         if self._driver is not None:
+            if self._is_autocomplete_enabled():
+                nodes = self._session.run(cypher, **kwargs).graph().nodes
+                node_ids = [node.element_id for node in nodes]
+                reltypes_expr = self._get_relationship_types_expression()
+                cypher = f"""
+                    MATCH (n) WHERE elementId(n) IN $node_ids
+                    RETURN n as start, NULL as rel, NULL as end
+                    UNION ALL
+                    MATCH (n)-[rel]-(m)
+                    WHERE elementId(n) IN $node_ids
+                    AND elementId(m) IN $node_ids
+                    {reltypes_expr}
+                    RETURN n as start, rel, m as end
+                """
+                kwargs = {"node_ids": node_ids}
+                if reltypes_expr:
+                    kwargs["relationship_types"] = self._autocomplete_relationships
             widget = GraphWidget(overview_enabled=self._overview, context_start_with=self._context_start_with,
                                  widget_layout=self._layout, license=self._license,
                                  graph=self._session.run(cypher, **kwargs).graph())
             self.apply_node_mappings(widget)
             self.apply_edge_mappings(widget)
 
             self._widget = widget
```

### Comparing `yfiles_jupyter_graphs_for_neo4j-1.0.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/PKG-INFO` & `yfiles_jupyter_graphs_for_neo4j-1.1.0/src/yfiles_jupyter_graphs_for_neo4j.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yfiles_jupyter_graphs_for_neo4j
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Neo4j graph visualization package that uses the yfiles-jupyter-graphs widget
 Author-email: yWorks Support Team <yfileshtml@yworks.com>
 License: MIT License
         
         Copyright (c) 2024 yWorks GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -106,14 +106,18 @@
 
 - `show_cypher(cypher, **kwargs)`
     - `cypher`: The [cypher query](https://neo4j.com/docs/cypher-manual/current/introduction/) that should be
       visualized.
     - `**kwargs`: Additional parameters that should be passed to the cypher query (e.g., see
       the [selection example](https://github.com/yWorks/yfiles-jupyter-graphs-for-neo4j/blob/main/examples/selection_example.ipynb)).
 
+The default behavior is to only show the nodes and relationships returned by the cypher query.
+This can be changed to autocomplete relationships like in neo4j browser:
+- `set_autocomplete_relationships(autocomplete_relationships)`: Sets whether to autocomplete relationships in the graph or not.
+
 The cypher queries are executed by the provided Neo4j driver. If you have not specified a driver when instantiating the
 class, you can set
 a driver afterward:
 
 - `set_driver(driver)`: Sets the given driver and uses this to send cypher queries to Databases.
 - `get_driver()`: Returns the current driver.
```

