# Comparing `tmp/pytvpaint-1.0.0b7.tar.gz` & `tmp/pytvpaint-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytvpaint-1.0.0b7.tar", max compression
+gzip compressed data, was "pytvpaint-1.0.0b8.tar", max compression
```

## Comparing `pytvpaint-1.0.0b7.tar` & `pytvpaint-1.0.0b8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2024-04-30 10:31:39.746839 pytvpaint-1.0.0b7/LICENSE.md
--rw-r--r--   0        0        0     3515 2024-04-30 10:31:39.746839 pytvpaint-1.0.0b7/README.md
--rw-r--r--   0        0        0     2229 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     1233 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/__init__.py
--rw-r--r--   0        0        0     8570 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/camera.py
--rw-r--r--   0        0        0    33490 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/clip.py
--rw-r--r--   0        0        0      573 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/__init__.py
--rw-r--r--   0        0        0     4890 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/__init__.py
--rw-r--r--   0        0        0     9747 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/parse.py
--rw-r--r--   0        0        0     5389 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/client/rpc.py
--rw-r--r--   0        0        0      687 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/exceptions.py
--rw-r--r--   0        0        0    28228 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_base.py
--rw-r--r--   0        0        0     2719 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_camera.py
--rw-r--r--   0        0        0    19188 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_clip.py
--rw-r--r--   0        0        0    31138 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_layer.py
--rw-r--r--   0        0        0    14902 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_project.py
--rw-r--r--   0        0        0     1189 2024-04-30 10:31:39.754839 pytvpaint-1.0.0b7/pytvpaint/george/grg_scene.py
--rw-r--r--   0        0        0    41808 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/layer.py
--rw-r--r--   0        0        0    23105 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/project.py
--rw-r--r--   0        0        0        0 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/py.typed
--rw-r--r--   0        0        0     4384 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/scene.py
--rw-r--r--   0        0        0     8745 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/sound.py
--rw-r--r--   0        0        0    17136 2024-04-30 10:31:39.758839 pytvpaint-1.0.0b7/pytvpaint/utils.py
--rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-22 18:39:25.575981 pytvpaint-1.0.0b8/LICENSE.md
+-rw-r--r--   0        0        0     3515 2024-05-22 18:39:25.575981 pytvpaint-1.0.0b8/README.md
+-rw-r--r--   0        0        0     2229 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     1233 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/__init__.py
+-rw-r--r--   0        0        0     8570 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/camera.py
+-rw-r--r--   0        0        0    33490 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/clip.py
+-rw-r--r--   0        0        0      573 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/__init__.py
+-rw-r--r--   0        0        0     4936 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/__init__.py
+-rw-r--r--   0        0        0     9747 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/parse.py
+-rw-r--r--   0        0        0     5389 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/client/rpc.py
+-rw-r--r--   0        0        0      687 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/exceptions.py
+-rw-r--r--   0        0        0    28228 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_base.py
+-rw-r--r--   0        0        0     2719 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_camera.py
+-rw-r--r--   0        0        0    19130 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_clip.py
+-rw-r--r--   0        0        0    31138 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_layer.py
+-rw-r--r--   0        0        0    14926 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_project.py
+-rw-r--r--   0        0        0     1189 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/george/grg_scene.py
+-rw-r--r--   0        0        0    41942 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/layer.py
+-rw-r--r--   0        0        0    23105 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/project.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/py.typed
+-rw-r--r--   0        0        0     4384 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/scene.py
+-rw-r--r--   0        0        0     8745 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/sound.py
+-rw-r--r--   0        0        0    17136 2024-05-22 18:39:25.583981 pytvpaint-1.0.0b8/pytvpaint/utils.py
+-rw-r--r--   0        0        0     4420 1970-01-01 00:00:00.000000 pytvpaint-1.0.0b8/PKG-INFO
```

### Comparing `pytvpaint-1.0.0b7/LICENSE.md` & `pytvpaint-1.0.0b8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/README.md` & `pytvpaint-1.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pyproject.toml` & `pytvpaint-1.0.0b8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytvpaint"
-version = "1.0.0b7"
+version = "1.0.0b8"
 description = "Python scripting for TVPaint"
 authors = [
     "Brunch Studio Developers <dev@brunchstudio.tv>",
     "Radouane Lahmidi <rlahmidi@brunchstudio.tv>",
     "Joseph Henry <jhenry@brunchstudio.tv>",
 ]
 license = "MIT"
```

### Comparing `pytvpaint-1.0.0b7/pytvpaint/__init__.py` & `pytvpaint-1.0.0b8/pytvpaint/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/camera.py` & `pytvpaint-1.0.0b8/pytvpaint/camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/clip.py` & `pytvpaint-1.0.0b8/pytvpaint/clip.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/__init__.py` & `pytvpaint-1.0.0b8/pytvpaint/george/__init__.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/client/__init__.py` & `pytvpaint-1.0.0b8/pytvpaint/george/client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,23 +122,27 @@
     """
     tv_args = [
         tv_handle_string(arg) if handle_string and isinstance(arg, str) else arg
         for arg in args
     ]
     cmd_str = " ".join([str(arg) for arg in [command, *tv_args]])
 
-    is_stack = command in ["tv_UndoOpenStack", "tv_UpdateUndo", "tv_UndoCloseStack"]
+    is_undo_stack = command in [
+        "tv_UndoOpenStack",
+        "tv_UpdateUndo",
+        "tv_UndoCloseStack",
+    ]
 
-    if not is_stack:
+    if not is_undo_stack:
         log.debug(f"[RPC] >> {cmd_str}")
 
     response = rpc_client.execute_remote("execute_george", [cmd_str])
     result = response["result"]
 
-    if not is_stack:
+    if not is_undo_stack:
         log.debug(f"[RPC] << {result}")
 
     # Test for basic ERROR X values and user provided custom errors
     res_in_error_values = error_values and result in list(map(str, error_values))
     if res_in_error_values or re.match(r"ERROR -?\d+", result, re.IGNORECASE):
         msg = f"Received value: '{result}' considered as an error"
         raise GeorgeError(msg, error_value=result)
```

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/client/parse.py` & `pytvpaint-1.0.0b8/pytvpaint/george/client/parse.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/client/rpc.py` & `pytvpaint-1.0.0b8/pytvpaint/george/client/rpc.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/exceptions.py` & `pytvpaint-1.0.0b8/pytvpaint/george/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_base.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_base.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_camera.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_camera.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_clip.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_clip.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,28 +406,28 @@
     file_format: SaveFormat,
     fill_background: bool = False,
     folder_pattern: str | None = None,
     file_pattern: str | None = None,
     visible_layers_only: bool = True,
     all_images: bool = False,
     ignore_duplicates: bool = False,
-    exclude_instance_names: list[str] | None = None,
+    exclude_names: list[str] | None = None,
 ) -> None:
     """Save the current clip structure in json.
 
     Args:
         export_path: the JSON export path
         file_format: file format to use for rendering
         fill_background: add a background. Defaults to None.
         folder_pattern: the folder name pattern (%li: layer index, %ln: layer name, %fi: file index (added in 11.0.8)). Defaults to None.
         file_pattern: the file name pattern (%li: layer index, %ln: layer name, %ii: image index, %in: image name, %fi: file index (added in 11.0.8)). Defaults to None.
         visible_layers_only: export only visible layers. Defaults to None.
         all_images: export all images. Defaults to None.
         ignore_duplicates: Ignore duplicates images. Defaults to None.
-        exclude_instance_names: the instances names which won't be processed/exported. Defaults to None.
+        exclude_names: the instances names which won't be processed/exported. Defaults to None.
 
     Raises:
         ValueError: the parent folder doesn't exist
     """
     export_path = Path(export_path).resolve()
 
     if not export_path.parent.exists():
@@ -441,17 +441,15 @@
         "fileformat": file_format.value,
         "background": int(fill_background) if fill_background else None,
         "patternfolder": folder_pattern,
         "patternfile": file_pattern,
         "onlyvisiblelayers": int(visible_layers_only),
         "allimages": int(all_images),
         "ignoreduplicateimages": int(ignore_duplicates),
-        "excludenames": (
-            ";".join(exclude_instance_names) if exclude_instance_names else None
-        ),
+        "excludenames": (";".join(exclude_names) if exclude_names else None),
     }
     args.extend(args_dict_to_list(dict_args))
 
     send_cmd("tv_ClipSaveStructure", *args, error_values=[-1])
 
 
 def tv_clip_save_structure_psd(
```

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_layer.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_layer.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_project.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,15 @@
 ) -> None:
     """Save the current project."""
     export_path = Path(export_path).resolve()
     args: list[Any] = [export_path.as_posix()]
 
     if use_camera:
         args.append("camera")
-    if start and end:
+    if start is not None and end is not None:
         args.extend((start, end))
 
     send_cmd(
         "tv_ProjectSaveSequence",
         *args,
         error_values=[-1],
     )
```

### Comparing `pytvpaint-1.0.0b7/pytvpaint/george/grg_scene.py` & `pytvpaint-1.0.0b8/pytvpaint/george/grg_scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/layer.py` & `pytvpaint-1.0.0b8/pytvpaint/layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -781,22 +781,24 @@
             color: the layer color
             image: the background image to load
             stretch: whether to stretch the image to fit the view
 
         Returns:
             Layer: the new animation layer
         """
+        clip = clip or Clip.current_clip()
         layer = cls.new(name, clip, color)
         layer.pre_behavior = george.LayerBehavior.HOLD
         layer.post_behavior = george.LayerBehavior.HOLD
         layer.thumbnails_visible = True
 
         image = Path(image or "")
         if image.is_file():
-            layer.load_image(image, stretch=stretch)
+            layer.convert_to_anim_layer()
+            layer.load_image(image, frame=clip.start, stretch=stretch)
 
         return layer
 
     @set_as_current
     @george.undoable
     def duplicate(self, name: str) -> Layer:
         """Duplicate this layer.
@@ -815,14 +817,15 @@
     def remove(self) -> None:
         """Remove the layer from the clip.
 
         Warning:
             The current instance won't be usable after this call since it will be mark removed.
         """
         self.clip.make_current()
+        self.is_locked = False
         george.tv_layer_kill(self.id)
         self.mark_removed()
 
     @set_as_current
     def render(
         self,
         output_path: Path | str | FileSequence,
```

### Comparing `pytvpaint-1.0.0b7/pytvpaint/project.py` & `pytvpaint-1.0.0b8/pytvpaint/project.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/scene.py` & `pytvpaint-1.0.0b8/pytvpaint/scene.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/sound.py` & `pytvpaint-1.0.0b8/pytvpaint/sound.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/pytvpaint/utils.py` & `pytvpaint-1.0.0b8/pytvpaint/utils.py`

 * *Files identical despite different names*

### Comparing `pytvpaint-1.0.0b7/PKG-INFO` & `pytvpaint-1.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytvpaint
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: Python scripting for TVPaint
 Home-page: https://github.com/brunchstudio/pytvpaint
 License: MIT
 Keywords: tvpaint,brunch,tvp,george
 Author: Brunch Studio Developers
 Author-email: dev@brunchstudio.tv
 Requires-Python: >=3.9
```

