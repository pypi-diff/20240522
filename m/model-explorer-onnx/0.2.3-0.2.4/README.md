# Comparing `tmp/model_explorer_onnx-0.2.3.tar.gz` & `tmp/model_explorer_onnx-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_explorer_onnx-0.2.3.tar", last modified: Tue May 21 02:12:36 2024, max compression
+gzip compressed data, was "model_explorer_onnx-0.2.4.tar", last modified: Wed May 22 03:00:19 2024, max compression
```

## Comparing `model_explorer_onnx-0.2.3.tar` & `model_explorer_onnx-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:36.400175 model_explorer_onnx-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-21 02:12:36.400175 model_explorer_onnx-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:12:36.400175 model_explorer_onnx-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:36.396175 model_explorer_onnx-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:36.396175 model_explorer_onnx-0.2.3/src/model_explorer_onnx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:36.396175 model_explorer_onnx-0.2.3/src/model_explorer_onnx/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx/bin/onnxvis.py
--rw-r--r--   0 runner    (1001) docker     (127)    22097 2024-05-21 02:12:32.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:12:36.400175 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 02:12:36.000000 model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.288561 model_explorer_onnx-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/bin/onnxvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22798 2024-05-22 03:00:15.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:00:19.292561 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-22 03:00:19.000000 model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/top_level.txt
```

### Comparing `model_explorer_onnx-0.2.3/LICENSE` & `model_explorer_onnx-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `model_explorer_onnx-0.2.3/PKG-INFO` & `model_explorer_onnx-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.3
+Version: 0.2.4
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -46,14 +46,18 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+## Notes on representation
+
+Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

### Comparing `model_explorer_onnx-0.2.3/README.md` & `model_explorer_onnx-0.2.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+## Notes on representation
+
+Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

### Comparing `model_explorer_onnx-0.2.3/pyproject.toml` & `model_explorer_onnx-0.2.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "model-explorer-onnx"
-version = "0.2.3"
+version = "0.2.4"
 description = "Adapter for ai-edge-model-explorer to support ONNX models"
 authors = [{ name = "Justin Chu", email = "justinchu@microsoft.com" }]
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT License"}
 keywords = ["onnx", "model-explorer", "visualization"]
 classifiers = [
```

### Comparing `model_explorer_onnx-0.2.3/src/model_explorer_onnx/main.py` & `model_explorer_onnx-0.2.4/src/model_explorer_onnx/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         return "Data not available"
     return str(tensor)
 
 
 def can_display_tensor_json(
     tensor: ir.TensorProtocol | None, settings: Settings
 ) -> bool:
+    """Check if the tensor can be displayed as JSON."""
+    del settings  # Unused
     if tensor is None:
         return False
-    if tensor.size > settings.const_element_count_limit:
-        return False
     if isinstance(tensor, ir.ExternalTensor):
         return False
     return True
 
 
 def display_tensor_json(
     tensor: ir.TensorProtocol | np.ndarray, settings: Settings
@@ -75,30 +75,27 @@
     return ""
 
 
 def format_shape(shape: ir.ShapeProtocol | None) -> str:
     return str(shape) if shape is not None else "[?]"
 
 
-def format_type(type: ir.TypeProtocol | None) -> str:
-    return str(type) if type is not None else "?"
+def format_type(type_: ir.TypeProtocol | None) -> str:
+    return str(type_) if type_ is not None else "?"
 
 
 def format_tensor_shape(value: ir.Value | ir.TensorProtocol) -> str:
     if isinstance(value, ir.Value):
         return f"{format_type(value.type)}{format_shape(value.shape)}"
     return f"{value.dtype or '?'}{format_shape(value.shape)}"
 
 
-def get_graph_io_node_name(value: ir.Value) -> str:
-    return f"[io] {value.name}"
-
-
-def get_initializer_node_name(value: ir.Value) -> str:
-    return f"[initializer] {value.name}"
+def get_value_node_name(value: ir.Value) -> str:
+    """Create name for node that is created from a value, that is for visualization only. E.g. Input."""
+    return f"[value] {value.name}"
 
 
 def get_function_graph_name(identifier: ir.OperatorIdentifier) -> str:
     name = f"[function]{identifier[0]}::{identifier[1]}"
     if identifier[2]:
         name += f"::{identifier[2]}"
     return name
@@ -215,22 +212,28 @@
 
 def add_node_attrs(
     onnx_node: ir.Node, node: graph_builder.GraphNode, settings: Settings
 ) -> None:
     for attr in onnx_node.attributes.values():
         if isinstance(attr, ir.Attr):
             if attr.type == ir.AttributeType.TENSOR:
-                if can_display_tensor_json(attr.value, settings=settings):
-                    assert attr.value is not None
-                    set_attr(
-                        node,
-                        "__value",
-                        display_tensor_json(attr.value, settings=settings),
-                    )
-                attr_value = display_tensor_repr(attr.value)
+                if onnx_node.op_type in {"Constant", "Initializer"}:
+                    if can_display_tensor_json(attr.value, settings=settings):
+                        assert attr.value is not None
+                        set_attr(
+                            node,
+                            "__value",
+                            display_tensor_json(attr.value, settings=settings),
+                        )
+                    attr_value = display_tensor_repr(attr.value)
+                else:
+                    if can_display_tensor_json(attr.value, settings=settings):
+                        attr_value = display_tensor_json(attr.value, settings=settings)
+                    else:
+                        attr_value = display_tensor_repr(attr.value)
             elif onnx_node.op_type == "Constant" and attr.name in {
                 "value_float",
                 "value_int",
                 "value_string",
                 "value_floats",
                 "value_ints",
                 "value_strings",
@@ -261,24 +264,24 @@
     graph_inputs: set[ir.Value],
 ) -> None:
     for target_input_id, input_value in enumerate(onnx_node.inputs):
         if input_value is None:
             continue
         if input_value in graph_inputs:
             # The input is a graph input. Create an input edge.
-            source_node_id = get_graph_io_node_name(input_value)
+            source_node_id = get_value_node_name(input_value)
             source_node_output_id = "0"
         else:
             input_node = input_value.producer()
             if input_node is None:
                 logger.debug(
                     "Input value %s does not have a producer. Treating as initializer.",
                     input_value,
                 )
-                source_node_id = get_initializer_node_name(input_value)
+                source_node_id = get_value_node_name(input_value)
                 source_node_output_id = "0"
             else:
                 assert input_node.name, "Bug: Node name is required"
                 source_node_id = input_node.name
                 source_node_output_id = str(input_value.index())
         assert source_node_id is not None
         node.incomingEdges.append(
@@ -346,15 +349,15 @@
     graph: graph_builder.Graph,
     input_or_outputs: Sequence[ir.Value],
     type_: Literal["Input", "Output"],
     all_nodes: dict[str, graph_builder.GraphNode],
 ) -> None:
     for i, value in enumerate(input_or_outputs):
         node = graph_builder.GraphNode(
-            id=get_graph_io_node_name(value),
+            id=get_value_node_name(value),
             label=type_,
         )
         producer = value.producer()
         if producer is not None:
             assert producer.name, "Bug: Node name is required"
             node.incomingEdges.append(
                 graph_builder.IncomingEdge(
@@ -427,26 +430,32 @@
 ) -> None:
     for initializer in initializers:
         if not initializer.name:
             logger.warning(
                 "Initializer does not have a name. Skipping: %s", initializer
             )
             continue
-        initializer_node_name = get_initializer_node_name(initializer)
+        initializer_node_name = get_value_node_name(initializer)
         if initializer_node_name in all_nodes:
-            # The initializer is also a graph input. Fill in the missing metadata.
+            # The initializer is also a graph input.
+            # Convert it into an InitializedInput and fill in the missing metadata
             node = all_nodes[initializer_node_name]
-            metadata = node.outputsMetadata[0]
+            node.label = "InitializedInput"
+            # Push the initializer closer to the user node's namespace
+            node.namespace = get_constant_namespace(initializer, namespace)
+            # Display the constant value
             if can_display_tensor_json(initializer.const_value, settings=settings):
                 assert initializer.const_value is not None
                 set_attr(
                     node,
                     "__value",
                     display_tensor_json(initializer.const_value, settings=settings),
                 )
+            # Set output metadata
+            metadata = node.outputsMetadata[0]
             set_attr(metadata, "value", display_tensor_repr(initializer.const_value))
             continue
         node = graph_builder.GraphNode(
             id=initializer_node_name,
             label="Initializer",
             namespace=get_constant_namespace(initializer, namespace),
         )
```

### Comparing `model_explorer_onnx-0.2.3/src/model_explorer_onnx.egg-info/PKG-INFO` & `model_explorer_onnx-0.2.4/src/model_explorer_onnx.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-explorer-onnx
-Version: 0.2.3
+Version: 0.2.4
 Summary: Adapter for ai-edge-model-explorer to support ONNX models
 Author-email: Justin Chu <justinchu@microsoft.com>
 License: MIT License
 Project-URL: Repository, https://github.com/justinchuby/model-explorer-onnx
 Keywords: onnx,model-explorer,visualization
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -46,14 +46,18 @@
 # Or as a shortcut
 onnxvis
 
 # Supply model path
 onnxvis model.onnx
 ```
 
+## Notes on representation
+
+Graph input/output/initializers in ONNX are values (edges), not nodes. A node is displayed here for visualization. Graph inputs that are initialized by initializers are displayed as `InitializedInput`, and are displayed closer to nodes that use them.
+
 ## Screenshots
 
 <img width="1294" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/ed7e1eee-a693-48bd-811d-b384f784ef9b">
 
 <img width="1291" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b266d8e9-9760-4860-a0a7-eda1de31e1a1">
 
 <img width="1285" alt="image" src="https://github.com/justinchuby/model-explorer-onnx/assets/11205048/b772aa13-4cc3-4034-a729-f134fa3cf818">
```

