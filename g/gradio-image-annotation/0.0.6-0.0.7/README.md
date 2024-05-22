# Comparing `tmp/gradio_image_annotation-0.0.6.tar.gz` & `tmp/gradio_image_annotation-0.0.7.tar.gz`

## Comparing `gradio_image_annotation-0.0.6.tar` & `gradio_image_annotation-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,55 @@
--rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/Dockerfile
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/package-lock.json
--rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/__init__.py
--rwxr-xr-x   0        0        0    13806 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/image_annotator.py
--rwxr-xr-x   0        0        0    28944 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/image_annotator.pyi
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/__vite-browser-external-2447137e.js
--rw-r--r--   0        0        0   313177 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/index.js
--rw-r--r--   0        0        0    24083 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/style.css
--rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-19fa94bf.js
--rw-r--r--   0        0        0   153257 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/example/index.js
--rw-r--r--   0        0        0    21565 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/example/style.css
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/demo/__init__.py
--rwxr-xr-x   0        0        0     1433 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/demo/app.py
--rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/demo/css.css
--rwxr-xr-x   0        0        0    11275 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/demo/space.py
--rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/Example.svelte
--rwxr-xr-x   0        0        0     3269 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/Index.svelte
--rwxr-xr-x   0        0        0    40890 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/package-lock.json
--rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/package.json
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/AnnotatedImageData.ts
--rwxr-xr-x   0        0        0    10879 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/Box.ts
--rwxr-xr-x   0        0        0     9658 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/Canvas.svelte
--rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/ClearImage.svelte
--rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/Colors.js
--rwxr-xr-x   0        0        0     4481 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/ImageAnnotator.svelte
--rwxr-xr-x   0        0        0     1760 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/ImageCanvas.svelte
--rwxr-xr-x   0        0        0     3893 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/ModalBox.svelte
--rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/index.ts
--rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/utils.ts
--rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/icons/Add.svelte
--rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/icons/index.ts
--rwxr-xr-x   0        0        0    12537 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/CHANGELOG.md
--rwxr-xr-x   0        0        0      980 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Dropdown.stories.svelte
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Example.svelte
--rwxr-xr-x   0        0        0     2722 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Index.svelte
--rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/LICENSE
--rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Multiselect.stories.svelte
--rwxr-xr-x   0        0        0     1218 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/README.md
--rwxr-xr-x   0        0        0    12541 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/dropdown.test.ts
--rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/package.json
--rwxr-xr-x   0        0        0     7987 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/Dropdown.svelte
--rwxr-xr-x   0        0        0     3715 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte
--rwxr-xr-x   0        0        0    10367 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/Multiselect.svelte
--rwxr-xr-x   0        0        0     1405 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/utils.ts
--rwxr-xr-x   0        0        0   174681 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/images/demo_1.png
--rwxr-xr-x   0        0        0  1110082 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/images/demo_2.png
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/.gitignore
--rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/LICENSE
--rwxr-xr-x   0        0        0    11375 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/README.md
--rwxr-xr-x   0        0        0     2117 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.6/PKG-INFO
+-rwxr-xr-x   0        0        0      268 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/Dockerfile
+-rwxr-xr-x   0        0        0      178 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/dev
+-rwxr-xr-x   0        0        0   125888 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/package-lock.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/package.json
+-rwxr-xr-x   0        0        0     1608 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/test.py
+-rwxr-xr-x   0        0        0     1084 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/__init__.py
+-rwxr-xr-x   0        0        0    14309 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/image_annotator.py
+-rwxr-xr-x   0        0        0    29516 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/image_annotator.pyi
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/__vite-browser-external-DYxpcVy9.js
+-rw-r--r--   0        0        0   248135 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/index.js
+-rw-r--r--   0        0        0    24083 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/style.css
+-rw-r--r--   0        0        0    78062 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-DjpFDl6n.js
+-rw-r--r--   0        0        0    81736 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/example/index.js
+-rw-r--r--   0        0        0    21565 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/example/style.css
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/demo/__init__.py
+-rwxr-xr-x   0        0        0     1731 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/demo/app.py
+-rwxr-xr-x   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/demo/css.css
+-rwxr-xr-x   0        0        0    11953 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/demo/space.py
+-rwxr-xr-x   0        0        0      966 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/Example.svelte
+-rwxr-xr-x   0        0        0     3487 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/Index.svelte
+-rwxr-xr-x   0        0        0    40890 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/package-lock.json
+-rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/package.json
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/AnnotatedImageData.ts
+-rwxr-xr-x   0        0        0    13223 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/Box.ts
+-rwxr-xr-x   0        0        0     9887 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/Canvas.svelte
+-rwxr-xr-x   0        0        0      558 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/ClearImage.svelte
+-rwxr-xr-x   0        0        0      351 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/Colors.js
+-rwxr-xr-x   0        0        0     4700 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/ImageAnnotator.svelte
+-rwxr-xr-x   0        0        0     1967 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/ImageCanvas.svelte
+-rwxr-xr-x   0        0        0     3893 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/ModalBox.svelte
+-rwxr-xr-x   0        0        0       51 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/index.ts
+-rwxr-xr-x   0        0        0     1079 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/utils.ts
+-rwxr-xr-x   0        0        0      459 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/icons/Add.svelte
+-rwxr-xr-x   0        0        0       46 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/icons/index.ts
+-rwxr-xr-x   0        0        0    12537 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/CHANGELOG.md
+-rwxr-xr-x   0        0        0      980 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Dropdown.stories.svelte
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Example.svelte
+-rwxr-xr-x   0        0        0     2722 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Index.svelte
+-rwxr-xr-x   0        0        0    11357 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/LICENSE
+-rwxr-xr-x   0        0        0      868 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Multiselect.stories.svelte
+-rwxr-xr-x   0        0        0     1218 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/README.md
+-rwxr-xr-x   0        0        0    12541 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/dropdown.test.ts
+-rwxr-xr-x   0        0        0      474 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/package.json
+-rwxr-xr-x   0        0        0     7987 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/Dropdown.svelte
+-rwxr-xr-x   0        0        0     3715 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte
+-rwxr-xr-x   0        0        0    10367 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/Multiselect.svelte
+-rwxr-xr-x   0        0        0     1405 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/utils.ts
+-rwxr-xr-x   0        0        0   174681 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/images/demo_1.png
+-rwxr-xr-x   0        0        0  1110082 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/images/demo_2.png
+-rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/.gitignore
+-rwxr-xr-x   0        0        0     1069 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/LICENSE
+-rwxr-xr-x   0        0        0    12401 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/README.md
+-rwxr-xr-x   0        0        0     2117 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13705 2020-02-02 00:00:00.000000 gradio_image_annotation-0.0.7/PKG-INFO
```

### Comparing `gradio_image_annotation-0.0.6/.github/workflows/python-publish.yml` & `gradio_image_annotation-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/backend/gradio_image_annotation/image_annotator.py` & `gradio_image_annotation-0.0.7/backend/gradio_image_annotation/image_annotator.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         self,
         value: dict | None = None,
         *,
         boxes_alpha: float | None = None,
         label_list: list[str] | None = None,
         label_colors: list[str] | None = None,
         box_min_size: int | None = None,
+        handle_size: int | None = None,
+        box_thickness: int | None = None,
+        box_selected_thickness: int | None = None,
         height: int | str | None = None,
         width: int | str | None = None,
         image_mode: Literal[
             "1", "L", "P", "RGB", "RGBA", "CMYK", "YCbCr", "LAB", "HSV", "I", "F"
         ] = "RGB",
         sources: list[Literal["upload", "clipboard"]] | None = ["upload", "clipboard"],
         image_type: Literal["numpy", "pil", "filepath"] = "numpy",
@@ -74,14 +77,17 @@
         """
         Parameters:
             value: A dict or None. The dictionary must contain a key 'image' with either an URL to an image, a numpy image or a PIL image. Optionally it may contain a key 'boxes' with a list of boxes. Each box must be a dict wit the keys: 'xmin', 'ymin', 'xmax' and 'ymax' with the absolute image coordinates of the box. Optionally can also include the keys 'label' and 'color' describing the label and color of the box. Color must be a tuple of RGB values (e.g. `(255,255,255)`).
             boxes_alpha: Opacity of the bounding boxes 0 and 1.
             label_list: List of valid labels.
             label_colors: Optional list of colors for each label when `label_list` is used. Colors must be a tuple of RGB values (e.g. `(255,255,255)`).
             box_min_size: Minimum valid bounding box size.
+            handle_size: Size of the bounding box resize handles.
+            box_thickness: Thickness of the bounding box outline.
+            box_selected_thickness: Thickness of the bounding box outline when it is selected.
             height: The height of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.
             width: The width of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.
             image_mode: "RGB" if color, or "L" if black and white. See https://pillow.readthedocs.io/en/stable/handbook/concepts.html for other supported image modes and their meaning.
             sources: List of sources for the image. "upload" creates a box where user can drop an image file, "clipboard" allows users to paste an image from the clipboard. If None, defaults to ["upload", "clipboard"].
             image_type: The format the image is converted before being passed into the prediction function. "numpy" converts the image to a numpy array with shape (height, width, 3) and values from 0 to 255, "pil" converts the image to a PIL image object, "filepath" passes a str path to a temporary file containing the image. If the image is SVG, the `type` is ignored and the filepath of the SVG is returned.
             label: The label for this component. Appears above the component and is also used as the header if there are a table of examples for this component. If None and used in a `gr.Interface`, the label will be the name of the parameter this component is assigned to.
             container: If True, will place the component in a container - providing some extra padding around the border.
@@ -127,14 +133,17 @@
             if show_share_button is None
             else show_share_button
         )
         self.show_clear_button = show_clear_button
 
         self.boxes_alpha = boxes_alpha
         self.box_min_size = box_min_size
+        self.handle_size = handle_size
+        self.box_thickness = box_thickness
+        self.box_selected_thickness = box_selected_thickness
         if label_list:
             self.label_list = [(l, i) for i, l in enumerate(label_list)]
         else:
             self.label_list = None
         
         # Parse colors
         self.label_colors = label_colors
```

### Comparing `gradio_image_annotation-0.0.6/backend/gradio_image_annotation/image_annotator.pyi` & `gradio_image_annotation-0.0.7/backend/gradio_image_annotation/image_annotator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         self,
         value: dict | None = None,
         *,
         boxes_alpha: float | None = None,
         label_list: list[str] | None = None,
         label_colors: list[str] | None = None,
         box_min_size: int | None = None,
+        handle_size: int | None = None,
+        box_thickness: int | None = None,
+        box_selected_thickness: int | None = None,
         height: int | str | None = None,
         width: int | str | None = None,
         image_mode: Literal[
             "1", "L", "P", "RGB", "RGBA", "CMYK", "YCbCr", "LAB", "HSV", "I", "F"
         ] = "RGB",
         sources: list[Literal["upload", "clipboard"]] | None = ["upload", "clipboard"],
         image_type: Literal["numpy", "pil", "filepath"] = "numpy",
@@ -65,14 +68,17 @@
         """
         Parameters:
             value: A dict or None. The dictionary must contain a key 'image' with either an URL to an image, a numpy image or a PIL image. Optionally it may contain a key 'boxes' with a list of boxes. Each box must be a dict wit the keys: 'xmin', 'ymin', 'xmax' and 'ymax' with the absolute image coordinates of the box. Optionally can also include the keys 'label' and 'color' describing the label and color of the box. Color must be a tuple of RGB values (e.g. `(255,255,255)`).
             boxes_alpha: Opacity of the bounding boxes 0 and 1.
             label_list: List of valid labels.
             label_colors: Optional list of colors for each label when `label_list` is used. Colors must be a tuple of RGB values (e.g. `(255,255,255)`).
             box_min_size: Minimum valid bounding box size.
+            handle_size: Size of the bounding box resize handles.
+            box_thickness: Thickness of the bounding box outline.
+            box_selected_thickness: Thickness of the bounding box outline when it is selected.
             height: The height of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.
             width: The width of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.
             image_mode: "RGB" if color, or "L" if black and white. See https://pillow.readthedocs.io/en/stable/handbook/concepts.html for other supported image modes and their meaning.
             sources: List of sources for the image. "upload" creates a box where user can drop an image file, "clipboard" allows users to paste an image from the clipboard. If None, defaults to ["upload", "clipboard"].
             image_type: The format the image is converted before being passed into the prediction function. "numpy" converts the image to a numpy array with shape (height, width, 3) and values from 0 to 255, "pil" converts the image to a PIL image object, "filepath" passes a str path to a temporary file containing the image. If the image is SVG, the `type` is ignored and the filepath of the SVG is returned.
             label: The label for this component. Appears above the component and is also used as the header if there are a table of examples for this component. If None and used in a `gr.Interface`, the label will be the name of the parameter this component is assigned to.
             container: If True, will place the component in a container - providing some extra padding around the border.
@@ -118,14 +124,17 @@
             if show_share_button is None
             else show_share_button
         )
         self.show_clear_button = show_clear_button
 
         self.boxes_alpha = boxes_alpha
         self.box_min_size = box_min_size
+        self.handle_size = handle_size
+        self.box_thickness = box_thickness
+        self.box_selected_thickness = box_selected_thickness
         if label_list:
             self.label_list = [(l, i) for i, l in enumerate(label_list)]
         else:
             self.label_list = None
         
         # Parse colors
         self.label_colors = label_colors
@@ -321,15 +330,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def change(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -363,15 +372,15 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
     
     def upload(self,
         fn: Callable | None,
         inputs: Component | Sequence[Component] | set[Component] | None = None,
         outputs: Component | Sequence[Component] | None = None,
@@ -405,10 +414,10 @@
             postprocess: If False, will not run postprocessing of component data before returning 'fn' output to the browser.
             cancels: A list of other events to cancel when this listener is triggered. For example, setting cancels=[click_event] will cancel the click_event, where click_event is the return value of another components .click method. Functions that have not yet run (or generators that are iterating) will be cancelled, but functions that are currently running will be allowed to finish.
             every: Run this event 'every' number of seconds while the client connection is open. Interpreted in seconds.
             trigger_mode: If "once" (default for all events except `.change()`) would not allow any submissions while an event is pending. If set to "multiple", unlimited submissions are allowed while pending, and "always_last" (default for `.change()` and `.key_up()` events) would allow a second submission after the pending event is complete.
             js: Optional frontend js method to run before running 'fn'. Input arguments for js method are values of 'inputs' and 'outputs', return should be a list of values for output components.
             concurrency_limit: If set, this is the maximum number of this event that can be running simultaneously. Can be set to None to mean no concurrency_limit (any number of this event can be running simultaneously). Set to "default" to use the default concurrency limit (defined by the `default_concurrency_limit` parameter in `Blocks.queue()`, which itself is 1 by default).
             concurrency_id: If set, this is the id of the concurrency group. Events with the same concurrency_id will be limited by the lowest set concurrency_limit.
-            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps to use this event. If fn is None, show_api will automatically be set to False.
+            show_api: whether to show this event in the "view API" page of the Gradio app, or in the ".view_api()" method of the Gradio clients. Unlike setting api_name to False, setting show_api to False will still allow downstream apps as well as the Clients to use this event. If fn is None, show_api will automatically be set to False.
         """
         ...
```

### Comparing `gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/style.css` & `gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-19fa94bf.js` & `gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/component/wrapper-6f348d45-DjpFDl6n.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-import S from "./__vite-browser-external-2447137e.js";
+import S from "./__vite-browser-external-DYxpcVy9.js";
 
 function z(s) {
     return s && s.__esModule && Object.prototype.hasOwnProperty.call(s, "default") ? s.default : s;
 }
 
 function gt(s) {
     if (s.__esModule)
```

### Comparing `gradio_image_annotation-0.0.6/backend/gradio_image_annotation/templates/example/style.css` & `gradio_image_annotation-0.0.7/backend/gradio_image_annotation/templates/example/style.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/demo/app.py` & `gradio_image_annotation-0.0.7/demo/app.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,21 +31,28 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
+
+            handle_size=6,
+            box_thickness=0,
+            box_selected_thickness=1,
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
     with gr.Tab("Crop"):
         with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
+            annotator_crop = image_annotator(example, image_type="numpy",
+                                                handle_size=6,
+                                                box_thickness=1,
+                                                box_selected_thickness=1,)
             image_crop = gr.Image()
         button_crop = gr.Button("Crop")
         button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_image_annotation-0.0.6/demo/css.css` & `gradio_image_annotation-0.0.7/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/demo/space.py` & `gradio_image_annotation-0.0.7/demo/space.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import gradio as gr
 from app import demo as app
 import os
 
-_docs = {'image_annotator': {'description': 'Creates a component to annotate images with bounding boxes. The bounding boxes can be created and edited by the user or be passed by code.\nIt is also possible to predefine a set of valid classes and colors.', 'members': {'__init__': {'value': {'type': 'dict | None', 'default': 'None', 'description': "A dict or None. The dictionary must contain a key 'image' with either an URL to an image, a numpy image or a PIL image. Optionally it may contain a key 'boxes' with a list of boxes. Each box must be a dict wit the keys: 'xmin', 'ymin', 'xmax' and 'ymax' with the absolute image coordinates of the box. Optionally can also include the keys 'label' and 'color' describing the label and color of the box. Color must be a tuple of RGB values (e.g. `(255,255,255)`)."}, 'boxes_alpha': {'type': 'float | None', 'default': 'None', 'description': 'Opacity of the bounding boxes 0 and 1.'}, 'label_list': {'type': 'list[str] | None', 'default': 'None', 'description': 'List of valid labels.'}, 'label_colors': {'type': 'list[str] | None', 'default': 'None', 'description': 'Optional list of colors for each label when `label_list` is used. Colors must be a tuple of RGB values (e.g. `(255,255,255)`).'}, 'box_min_size': {'type': 'int | None', 'default': 'None', 'description': 'Minimum valid bounding box size.'}, 'height': {'type': 'int | str | None', 'default': 'None', 'description': 'The height of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.'}, 'width': {'type': 'int | str | None', 'default': 'None', 'description': 'The width of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.'}, 'image_mode': {'type': '"1"\n    | "L"\n    | "P"\n    | "RGB"\n    | "RGBA"\n    | "CMYK"\n    | "YCbCr"\n    | "LAB"\n    | "HSV"\n    | "I"\n    | "F"', 'default': '"RGB"', 'description': '"RGB" if color, or "L" if black and white. See https://pillow.readthedocs.io/en/stable/handbook/concepts.html for other supported image modes and their meaning.'}, 'sources': {'type': 'list["upload" | "clipboard"] | None', 'default': '["upload", "clipboard"]', 'description': 'List of sources for the image. "upload" creates a box where user can drop an image file, "clipboard" allows users to paste an image from the clipboard. If None, defaults to ["upload", "clipboard"].'}, 'image_type': {'type': '"numpy" | "pil" | "filepath"', 'default': '"numpy"', 'description': 'The format the image is converted before being passed into the prediction function. "numpy" converts the image to a numpy array with shape (height, width, 3) and values from 0 to 255, "pil" converts the image to a PIL image object, "filepath" passes a str path to a temporary file containing the image. If the image is SVG, the `type` is ignored and the filepath of the SVG is returned.'}, 'label': {'type': 'str | None', 'default': 'None', 'description': 'The label for this component. Appears above the component and is also used as the header if there are a table of examples for this component. If None and used in a `gr.Interface`, the label will be the name of the parameter this component is assigned to.'}, 'container': {'type': 'bool', 'default': 'True', 'description': 'If True, will place the component in a container - providing some extra padding around the border.'}, 'scale': {'type': 'int | None', 'default': 'None', 'description': 'relative size compared to adjacent Components. For example if Components A and B are in a Row, and A has scale=2, and B has scale=1, A will be twice as wide as B. Should be an integer. scale applies in Rows, and to top-level Components in Blocks where fill_height=True.'}, 'min_width': {'type': 'int', 'default': '160', 'description': 'minimum pixel width, will wrap if not sufficient screen space to satisfy this value. If a certain scale value results in this Component being narrower than min_width, the min_width parameter will be respected first.'}, 'interactive': {'type': 'bool | None', 'default': 'True', 'description': 'if True, will allow users to upload and annotate an image; if False, can only be used to display annotated images.'}, 'visible': {'type': 'bool', 'default': 'True', 'description': 'If False, component will be hidden.'}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': 'An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': 'An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'render': {'type': 'bool', 'default': 'True', 'description': 'If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.'}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': 'if True, will display label.'}, 'show_download_button': {'type': 'bool', 'default': 'True', 'description': 'If True, will show a button to download the image.'}, 'show_share_button': {'type': 'bool | None', 'default': 'None', 'description': 'If True, will show a share icon in the corner of the component that allows user to share outputs to Hugging Face Spaces Discussions. If False, icon does not appear. If set to None (default behavior), then the icon appears if this Gradio app is launched on Spaces, but not otherwise.'}, 'show_clear_button': {'type': 'bool | None', 'default': 'True', 'description': 'If True, will show a clear button.'}}, 'postprocess': {'value': {'type': 'dict | None', 'description': 'A dict with an image and an optional list of boxes or None.'}}, 'preprocess': {'return': {'type': 'dict | None', 'description': 'A dict with the image and boxes or None.'}, 'value': None}}, 'events': {'clear': {'type': None, 'default': None, 'description': 'This listener is triggered when the user clears the image_annotator using the X button for the component.'}, 'change': {'type': None, 'default': None, 'description': 'Triggered when the value of the image_annotator changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input.'}, 'upload': {'type': None, 'default': None, 'description': 'This listener is triggered when the user uploads a file into the image_annotator.'}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'image_annotator': []}}}
+_docs = {'image_annotator': {'description': 'Creates a component to annotate images with bounding boxes. The bounding boxes can be created and edited by the user or be passed by code.\nIt is also possible to predefine a set of valid classes and colors.', 'members': {'__init__': {'value': {'type': 'dict | None', 'default': 'None', 'description': "A dict or None. The dictionary must contain a key 'image' with either an URL to an image, a numpy image or a PIL image. Optionally it may contain a key 'boxes' with a list of boxes. Each box must be a dict wit the keys: 'xmin', 'ymin', 'xmax' and 'ymax' with the absolute image coordinates of the box. Optionally can also include the keys 'label' and 'color' describing the label and color of the box. Color must be a tuple of RGB values (e.g. `(255,255,255)`)."}, 'boxes_alpha': {'type': 'float | None', 'default': 'None', 'description': 'Opacity of the bounding boxes 0 and 1.'}, 'label_list': {'type': 'list[str] | None', 'default': 'None', 'description': 'List of valid labels.'}, 'label_colors': {'type': 'list[str] | None', 'default': 'None', 'description': 'Optional list of colors for each label when `label_list` is used. Colors must be a tuple of RGB values (e.g. `(255,255,255)`).'}, 'box_min_size': {'type': 'int | None', 'default': 'None', 'description': 'Minimum valid bounding box size.'}, 'handle_size': {'type': 'int | None', 'default': 'None', 'description': 'Size of the bounding box resize handles.'}, 'box_thickness': {'type': 'int | None', 'default': 'None', 'description': 'Thickness of the bounding box outline.'}, 'box_selected_thickness': {'type': 'int | None', 'default': 'None', 'description': 'Thickness of the bounding box outline when it is selected.'}, 'height': {'type': 'int | str | None', 'default': 'None', 'description': 'The height of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.'}, 'width': {'type': 'int | str | None', 'default': 'None', 'description': 'The width of the displayed image, specified in pixels if a number is passed, or in CSS units if a string is passed.'}, 'image_mode': {'type': '"1"\n    | "L"\n    | "P"\n    | "RGB"\n    | "RGBA"\n    | "CMYK"\n    | "YCbCr"\n    | "LAB"\n    | "HSV"\n    | "I"\n    | "F"', 'default': '"RGB"', 'description': '"RGB" if color, or "L" if black and white. See https://pillow.readthedocs.io/en/stable/handbook/concepts.html for other supported image modes and their meaning.'}, 'sources': {'type': 'list["upload" | "clipboard"] | None', 'default': '["upload", "clipboard"]', 'description': 'List of sources for the image. "upload" creates a box where user can drop an image file, "clipboard" allows users to paste an image from the clipboard. If None, defaults to ["upload", "clipboard"].'}, 'image_type': {'type': '"numpy" | "pil" | "filepath"', 'default': '"numpy"', 'description': 'The format the image is converted before being passed into the prediction function. "numpy" converts the image to a numpy array with shape (height, width, 3) and values from 0 to 255, "pil" converts the image to a PIL image object, "filepath" passes a str path to a temporary file containing the image. If the image is SVG, the `type` is ignored and the filepath of the SVG is returned.'}, 'label': {'type': 'str | None', 'default': 'None', 'description': 'The label for this component. Appears above the component and is also used as the header if there are a table of examples for this component. If None and used in a `gr.Interface`, the label will be the name of the parameter this component is assigned to.'}, 'container': {'type': 'bool', 'default': 'True', 'description': 'If True, will place the component in a container - providing some extra padding around the border.'}, 'scale': {'type': 'int | None', 'default': 'None', 'description': 'relative size compared to adjacent Components. For example if Components A and B are in a Row, and A has scale=2, and B has scale=1, A will be twice as wide as B. Should be an integer. scale applies in Rows, and to top-level Components in Blocks where fill_height=True.'}, 'min_width': {'type': 'int', 'default': '160', 'description': 'minimum pixel width, will wrap if not sufficient screen space to satisfy this value. If a certain scale value results in this Component being narrower than min_width, the min_width parameter will be respected first.'}, 'interactive': {'type': 'bool | None', 'default': 'True', 'description': 'if True, will allow users to upload and annotate an image; if False, can only be used to display annotated images.'}, 'visible': {'type': 'bool', 'default': 'True', 'description': 'If False, component will be hidden.'}, 'elem_id': {'type': 'str | None', 'default': 'None', 'description': 'An optional string that is assigned as the id of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'elem_classes': {'type': 'list[str] | str | None', 'default': 'None', 'description': 'An optional list of strings that are assigned as the classes of this component in the HTML DOM. Can be used for targeting CSS styles.'}, 'render': {'type': 'bool', 'default': 'True', 'description': 'If False, component will not render be rendered in the Blocks context. Should be used if the intention is to assign event listeners now but render the component later.'}, 'show_label': {'type': 'bool | None', 'default': 'None', 'description': 'if True, will display label.'}, 'show_download_button': {'type': 'bool', 'default': 'True', 'description': 'If True, will show a button to download the image.'}, 'show_share_button': {'type': 'bool | None', 'default': 'None', 'description': 'If True, will show a share icon in the corner of the component that allows user to share outputs to Hugging Face Spaces Discussions. If False, icon does not appear. If set to None (default behavior), then the icon appears if this Gradio app is launched on Spaces, but not otherwise.'}, 'show_clear_button': {'type': 'bool | None', 'default': 'True', 'description': 'If True, will show a clear button.'}}, 'postprocess': {'value': {'type': 'dict | None', 'description': 'A dict with an image and an optional list of boxes or None.'}}, 'preprocess': {'return': {'type': 'dict | None', 'description': 'A dict with the image and boxes or None.'}, 'value': None}}, 'events': {'clear': {'type': None, 'default': None, 'description': 'This listener is triggered when the user clears the image_annotator using the X button for the component.'}, 'change': {'type': None, 'default': None, 'description': 'Triggered when the value of the image_annotator changes either because of user input (e.g. a user types in a textbox) OR because of a function update (e.g. an image receives a value from the output of an event trigger). See `.input()` for a listener that is only triggered by user input.'}, 'upload': {'type': None, 'default': None, 'description': 'This listener is triggered when the user uploads a file into the image_annotator.'}}}, '__meta__': {'additional_interfaces': {}, 'user_fn_refs': {'image_annotator': []}}}
 
 abs_path = os.path.join(os.path.dirname(__file__), "css.css")
 
 with gr.Blocks(
     css=abs_path,
     theme=gr.themes.Default(
         font_mono=[
@@ -71,21 +71,28 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
+
+            handle_size=6,
+            box_thickness=0,
+            box_selected_thickness=1,
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
     with gr.Tab("Crop"):
         with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
+            annotator_crop = image_annotator(example, image_type="numpy",
+                                                handle_size=6,
+                                                box_thickness=1,
+                                                box_selected_thickness=1,)
             image_crop = gr.Image()
         button_crop = gr.Button("Crop")
         button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
```

### Comparing `gradio_image_annotation-0.0.6/frontend/Example.svelte` & `gradio_image_annotation-0.0.7/frontend/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/Index.svelte` & `gradio_image_annotation-0.0.7/frontend/Index.svelte`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 	export let show_share_button: boolean;
 	export let show_clear_button: boolean;
 	export let interactive: boolean;
 	export let boxes_alpha: number;
 	export let label_list: string[];
 	export let label_colors: string[];
 	export let box_min_size: number;
+	export let handle_size: number;
+	export let box_thickness: number;
+	export let box_selected_thickness: number;
 
 	export let gradio: Gradio<{
 		change: never;
 		error: string;
 		edit: never;
 		drag: never;
 		upload: never;
@@ -86,14 +89,17 @@
 		showShareButton={show_share_button}
 		showClearButton={show_clear_button}
 		i18n={gradio.i18n}
 		boxesAlpha={boxes_alpha}
 		labelList={label_list}
 		labelColors={label_colors}
 		boxMinSize={box_min_size}
+		handleSize={handle_size}
+		boxThickness={box_thickness}
+		boxSelectedThickness={box_selected_thickness}
 		on:edit={() => gradio.dispatch("edit")}
 		on:clear={() => {
 			gradio.dispatch("clear");
 		}}
 		on:drag={({ detail }) => (dragging = detail)}
 		on:upload={() => gradio.dispatch("upload")}
 		on:select={({ detail }) => gradio.dispatch("select", detail)}
```

#### html2text {}

```diff
@@ -2,15 +2,16 @@
 {false} {elem_id} {elem_classes} height={height || undefined} {width}
 allow_overflow={false} {container} {scale} {min_width} >
 ...loading_status} />
 > gradio.dispatch("change")} selectable={_selectable} {root} {sources}
 {interactive} showDownloadButton={show_download_button} showShareButton=
 {show_share_button} showClearButton={show_clear_button} i18n={gradio.i18n}
 boxesAlpha={boxes_alpha} labelList={label_list} labelColors={label_colors}
-boxMinSize={box_min_size} on:edit={() => gradio.dispatch("edit")} on:clear={()
-=> { gradio.dispatch("clear"); }} on:drag={({ detail }) => (dragging = detail)}
-on:upload={() => gradio.dispatch("upload")} on:select={({ detail }) =>
-gradio.dispatch("select", detail)} on:share={({ detail }) => gradio.dispatch
-("share", detail)} on:error={({ detail }) => { loading_status = loading_status
-|| {}; loading_status.status = "error"; gradio.dispatch("error", detail); }}
-{label} {show_label} > {#if active_source === "upload"} {:else if active_source
-=== "clipboard"} {:else} {/if}
+boxMinSize={box_min_size} handleSize={handle_size} boxThickness={box_thickness}
+boxSelectedThickness={box_selected_thickness} on:edit={() => gradio.dispatch
+("edit")} on:clear={() => { gradio.dispatch("clear"); }} on:drag={({ detail })
+=> (dragging = detail)} on:upload={() => gradio.dispatch("upload")} on:select={
+({ detail }) => gradio.dispatch("select", detail)} on:share={({ detail }) =>
+gradio.dispatch("share", detail)} on:error={({ detail }) => { loading_status =
+loading_status || {}; loading_status.status = "error"; gradio.dispatch("error",
+detail); }} {label} {show_label} > {#if active_source === "upload"} {:else if
+active_source === "clipboard"} {:else} {/if}
```

### Comparing `gradio_image_annotation-0.0.6/frontend/package-lock.json` & `gradio_image_annotation-0.0.7/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/package.json` & `gradio_image_annotation-0.0.7/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/Box.ts` & `gradio_image_annotation-0.0.7/frontend/shared/Box.ts`

 * *Files 14% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     minSize: number;
     renderCallBack: () => void;
     canvasXmin: number;
     canvasYmin: number;
     canvasXmax: number;
     canvasYmax: number;
     scaleFactor: number;
+    thickness: number;
+    selectedThickness: number;
     resizeHandles: {
         xmin: number;
         ymin: number;
         xmax: number;
         ymax: number;
     }[];
 
@@ -53,14 +55,17 @@
         xmin: number,
         ymin: number,
         xmax: number,
         ymax: number,
         color: string = "rgb(255, 255, 255)",
         alpha: number = 0.5,
         minSize: number = 25,
+        handleSize: number = 8,
+        thickness: number = 2,
+        selectedThickness: number = 4,
         scaleFactor: number = 1
     ) {
         this.renderCallBack = renderCallBack;
         this.canvasXmin = canvasXmin;
         this.canvasYmin = canvasYmin;
         this.canvasXmax = canvasXmax;
         this.canvasYmax = canvasYmax;
@@ -71,15 +76,17 @@
         this.ymin = ymin;
         this.xmax = xmax;
         this.ymax = ymax;
         this.isResizing = false;
         this.isSelected = false;
         this.offsetMouseX = 0;
         this.offsetMouseY = 0;
-        this.resizeHandleSize = 8;
+        this.resizeHandleSize = handleSize;
+        this.thickness = thickness;
+        this.selectedThickness = selectedThickness;
         this.updateHandles();
         this.resizingHandleIndex = -1;
         this.minSize = minSize;
         this.color = color;
         this.alpha = alpha;
     }
 
@@ -107,39 +114,73 @@
         this.ymax = Math.round(this.ymax * scale);
         this.updateHandles();
         this.scaleFactor = scaleFactor;
     }
 
     updateHandles(): void {
         const halfSize = this.resizeHandleSize / 2;
+        const width = this.getWidth();
+        const height = this.getHeight();
         this.resizeHandles = [
             {
+                // Top left
                 xmin: this.xmin - halfSize,
                 ymin: this.ymin - halfSize,
                 xmax: this.xmin + halfSize,
                 ymax: this.ymin + halfSize,
             },
             {
+                // Top right
                 xmin: this.xmax - halfSize,
                 ymin: this.ymin - halfSize,
                 xmax: this.xmax + halfSize,
                 ymax: this.ymin + halfSize,
             },
             {
+                // Bottom right
                 xmin: this.xmax - halfSize,
                 ymin: this.ymax - halfSize,
                 xmax: this.xmax + halfSize,
                 ymax: this.ymax + halfSize,
             },
             {
+                // Bottom left
                 xmin: this.xmin - halfSize,
                 ymin: this.ymax - halfSize,
                 xmax: this.xmin + halfSize,
                 ymax: this.ymax + halfSize,
             },
+            {
+                // Top center
+                xmin: this.xmin + (width / 2) - halfSize,
+                ymin: this.ymin - halfSize,
+                xmax: this.xmin + (width / 2) + halfSize,
+                ymax: this.ymin + halfSize,
+            },
+            {
+                // Right center
+                xmin: this.xmax - halfSize,
+                ymin: this.ymin + (height / 2) - halfSize,
+                xmax: this.xmax + halfSize,
+                ymax: this.ymin + (height / 2) + halfSize,
+            },
+            {
+                // Bottom center
+                xmin: this.xmin + (width / 2) - halfSize,
+                ymin: this.ymax - halfSize,
+                xmax: this.xmin + (width / 2) + halfSize,
+                ymax: this.ymax + halfSize,
+            },
+            {
+                // Left center
+                xmin: this.xmin - halfSize,
+                ymin: this.ymin + (height / 2) - halfSize,
+                xmax: this.xmin + halfSize,
+                ymax: this.ymin + (height / 2) + halfSize,
+            },
         ];
     }
 
     getWidth(): number {
         return this.xmax - this.xmin;
     }
 
@@ -165,19 +206,20 @@
         // Render the box and border
         ctx.beginPath();
         [xmin, ymin] = this.toCanvasCoordinates(this.xmin, this.ymin);
         ctx.rect(xmin, ymin, this.getWidth(), this.getHeight());
         ctx.fillStyle = setAlpha(this.color, this.alpha);
         ctx.fill();
         if (this.isSelected) {
-            ctx.lineWidth = 4;
+            ctx.lineWidth = this.selectedThickness;
         } else {
-            ctx.lineWidth = 2;
+            ctx.lineWidth = this.thickness;
         }
         ctx.strokeStyle = setAlpha(this.color, 1);
+        
         ctx.stroke();
         ctx.closePath();
 
         // Render the label and background
         if (this.label !== null && this.label.trim() !== ""){
             if (this.isSelected) {
                 ctx.font = "bold 14px Arial";
@@ -307,14 +349,30 @@
                     break;
                 case 3: // Bottom-left handle
                     this.xmin += deltaX;
                     this.ymax += deltaY;
                     this.xmin = clamp(this.xmin, 0, this.xmax - this.minSize);
                     this.ymax = clamp(this.ymax, this.ymin + this.minSize, canvasH);
                     break;
+                case 4: // Top center handle
+                    this.ymin += deltaY;
+                    this.ymin = clamp(this.ymin, 0, this.ymax - this.minSize);
+                    break;
+                case 5: // Right center handle
+                    this.xmax += deltaX;
+                    this.xmax = clamp(this.xmax, this.xmin + this.minSize, canvasW);
+                    break;
+                case 6: // Bottom center handle
+                    this.ymax += deltaY;
+                    this.ymax = clamp(this.ymax, this.ymin + this.minSize, canvasH);
+                    break;
+                case 7: // Left center handle
+                    this.xmin += deltaX;
+                    this.xmin = clamp(this.xmin, 0, this.xmax - this.minSize);
+                    break;
             }
             // Update the resize handles
             this.updateHandles();
             this.renderCallBack();
         }
     };
```

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/Canvas.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/Canvas.svelte`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 	import { Colors } from './Colors.js';
 	import AnnotatedImageData from "./AnnotatedImageData";
 
     export let imageUrl: string | null = null;
 	export let interactive: boolean;
 	export let boxAlpha = 0.5;
 	export let boxMinSize = 25;
+	export let handleSize: number;
+	export let boxThickness: number;
+	export let boxSelectedThickness: number;
 	export let value: null | AnnotatedImageData;
 	export let choices = [];
     export let choicesColors = [];
 
     let canvas: HTMLCanvasElement;
 	let ctx: CanvasRenderingContext2D;
     let image = null;
@@ -149,14 +152,17 @@
 				Math.round(xmin),
 				Math.round(ymin),
 				Math.round(xmax),
 				Math.round(ymax),
 				color,
 				boxAlpha,
 				boxMinSize,
+				handleSize,
+				boxThickness,
+				boxSelectedThickness
 			);
 			value.boxes = [box, ...value.boxes];
 			draw();
 			dispatch("change");
 		}
 	}
 
@@ -270,14 +276,17 @@
 					box["xmin"],
 					box["ymin"],
 					box["xmax"],
 					box["ymax"],
 					color,
 					boxAlpha,
 					boxMinSize,
+					handleSize,
+					boxThickness,
+					boxSelectedThickness
 				);
 				value.boxes[i] = box;
 			}
 		}
 	}
 
 	$: {
```

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/ClearImage.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/ClearImage.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/ImageAnnotator.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/ImageAnnotator.svelte`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 	export let showShareButton: boolean;
 	export let showDownloadButton: boolean;
 	export let showClearButton: boolean;
 	export let boxesAlpha;
 	export let labelList: string[];
 	export let labelColors: string[];
 	export let boxMinSize: number;
+	export let handleSize: number;
+	export let boxThickness: number;
+	export let boxSelectedThickness: number;
 
 	let upload: Upload;
 	let uploading = false;
 	export let active_source: source_type = null;
 
 	function handle_upload({ detail }: CustomEvent<FileData>): void {
 		value = new AnnotatedImageData();
@@ -136,14 +139,17 @@
 					bind:value
 					on:change={() => dispatch("change")}
 					{boxesAlpha}
 					{labelList}
 					{labelColors}
 					{boxMinSize}
 					{interactive}
+					handleSize={handleSize}
+					boxThickness={boxThickness}
+					boxSelectedThickness={boxSelectedThickness}
 					src={value.image.url}
 				/>
 			</div>
 		{/if}
 	</div>
 	{#if (sources.length > 1 || sources.includes("clipboard")) && value === null && interactive}
 		<SelectSource
```

#### html2text {}

```diff
@@ -7,13 +7,14 @@
 /> {/if} {#if showClearButton && value !== null && interactive}
 {/if}
 == null} bind:this={upload} bind:uploading bind:dragging filetype=
 {active_source === "clipboard" ? "clipboard" : "image/*"} on:load=
 {handle_upload} on:error {root} disable_click={!sources.includes("upload")} >
 {#if value === null} {/if} {#if value !== null}
 > dispatch("change")} {boxesAlpha} {labelList} {labelColors} {boxMinSize}
-{interactive} src={value.image.url} />
+{interactive} handleSize={handleSize} boxThickness={boxThickness}
+boxSelectedThickness={boxSelectedThickness} src={value.image.url} />
 {/if}
 {#if (sources.length > 1 || sources.includes("clipboard")) && value === null &&
 interactive}
 sources} bind:active_source {handle_clear} handle_select={handle_select_source}
 /> {/if}
```

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/ImageCanvas.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/ImageCanvas.svelte`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 	export let src: HTMLImgAttributes["src"] = undefined;
 	export let interactive: boolean;
 	export let boxesAlpha: number;
 	export let labelList: string[];
 	export let labelColors: string[];
 	export let boxMinSize: number;
+	export let handleSize: number;
+	export let boxThickness: number;
+	export let boxSelectedThickness: number;
 	export let value: null | AnnotatedImageData;
 
 	let resolved_src: typeof src;
 
 	// The `src` prop can be updated before the Promise from `resolve_wasm_src` is resolved.
 	// In such a case, the resolved value for the old `src` has to be discarded,
 	// This variable `latest_src` is used to pick up only the value resolved for the latest `src` prop.
@@ -50,9 +53,12 @@
 	bind:value
 	on:change={() => dispatch("change")}
 	{interactive}
 	boxAlpha={boxesAlpha}
 	choices={labelList}
 	choicesColors={labelColors}
 	{boxMinSize}
+	handleSize={handleSize}
+	boxThickness={boxThickness}
+	boxSelectedThickness={boxSelectedThickness}
 	imageUrl={resolved_src}
 />
```

#### html2text {}

```diff
@@ -1,2 +1,4 @@
 > dispatch("change")} {interactive} boxAlpha={boxesAlpha} choices={labelList}
-choicesColors={labelColors} {boxMinSize} imageUrl={resolved_src} />
+choicesColors={labelColors} {boxMinSize} handleSize={handleSize} boxThickness=
+{boxThickness} boxSelectedThickness={boxSelectedThickness} imageUrl=
+{resolved_src} />
```

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/ModalBox.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/ModalBox.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/utils.ts` & `gradio_image_annotation-0.0.7/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/CHANGELOG.md` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Dropdown.stories.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Dropdown.stories.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Example.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Example.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Index.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/LICENSE` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/Multiselect.stories.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/Multiselect.stories.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/README.md` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/README.md`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/dropdown.test.ts` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/dropdown.test.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/Dropdown.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/Dropdown.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/DropdownOptions.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/Multiselect.svelte` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/Multiselect.svelte`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/frontend/shared/patched_dropdown/shared/utils.ts` & `gradio_image_annotation-0.0.7/frontend/shared/patched_dropdown/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/images/demo_1.png` & `gradio_image_annotation-0.0.7/images/demo_1.png`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/images/demo_2.png` & `gradio_image_annotation-0.0.7/images/demo_2.png`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/LICENSE` & `gradio_image_annotation-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_image_annotation-0.0.6/README.md` & `gradio_image_annotation-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,21 +46,28 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
+
+            handle_size=6,
+            box_thickness=0,
+            box_selected_thickness=1,
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
     with gr.Tab("Crop"):
         with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
+            annotator_crop = image_annotator(example, image_type="numpy",
+                                                handle_size=6,
+                                                box_thickness=1,
+                                                box_selected_thickness=1,)
             image_crop = gr.Image()
         button_crop = gr.Button("Crop")
         button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
@@ -143,14 +150,53 @@
 
 </td>
 <td align="left"><code>None</code></td>
 <td align="left">Minimum valid bounding box size.</td>
 </tr>
 
 <tr>
+<td align="left"><code>handle_size</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Size of the bounding box resize handles.</td>
+</tr>
+
+<tr>
+<td align="left"><code>box_thickness</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Thickness of the bounding box outline.</td>
+</tr>
+
+<tr>
+<td align="left"><code>box_selected_thickness</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Thickness of the bounding box outline when it is selected.</td>
+</tr>
+
+<tr>
 <td align="left"><code>height</code></td>
 <td align="left" style="width: 25%;">
 
 ```python
 int | str | None
 ```
```

### Comparing `gradio_image_annotation-0.0.6/pyproject.toml` & `gradio_image_annotation-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_image_annotation"
-version = "0.0.6"
+version = "0.0.7"
 description = "A Gradio component that can be used to annotate images with bounding boxes."
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
 authors = [{ name = "Edgar Gracia" }]
 keywords = ["gradio-custom-component", "gradio-template-Image", "bounding box", "annotator", "annotate", "boxes"]
 # Add dependencies here
```

### Comparing `gradio_image_annotation-0.0.6/PKG-INFO` & `gradio_image_annotation-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gradio_image_annotation
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Gradio component that can be used to annotate images with bounding boxes.
 Project-URL: Repository, https://github.com/edgarGracia/gradio_image_annotator.git
 Project-URL: Issues, https://github.com/edgarGracia/gradio_image_annotator/issues
 Author: Edgar Gracia
 License-Expression: MIT
 License-File: LICENSE
 Keywords: annotate,annotator,bounding box,boxes,gradio-custom-component,gradio-template-Image
@@ -75,21 +75,28 @@
 
 with gr.Blocks() as demo:
     with gr.Tab("Object annotation"):
         annotator = image_annotator(
             {"image": "https://gradio-builds.s3.amazonaws.com/demo-files/base.png"},
             label_list=["Person", "Vehicle"],
             label_colors=[(0, 255, 0), (255, 0, 0)],
+
+            handle_size=6,
+            box_thickness=0,
+            box_selected_thickness=1,
         )
         button_get = gr.Button("Get bounding boxes")
         json_boxes = gr.JSON()
         button_get.click(get_boxes_json, annotator, json_boxes)
     with gr.Tab("Crop"):
         with gr.Row():
-            annotator_crop = image_annotator(example, image_type="numpy")
+            annotator_crop = image_annotator(example, image_type="numpy",
+                                                handle_size=6,
+                                                box_thickness=1,
+                                                box_selected_thickness=1,)
             image_crop = gr.Image()
         button_crop = gr.Button("Crop")
         button_crop.click(crop, annotator_crop, image_crop)
 
 
 if __name__ == "__main__":
     demo.launch()
@@ -172,14 +179,53 @@
 
 </td>
 <td align="left"><code>None</code></td>
 <td align="left">Minimum valid bounding box size.</td>
 </tr>
 
 <tr>
+<td align="left"><code>handle_size</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Size of the bounding box resize handles.</td>
+</tr>
+
+<tr>
+<td align="left"><code>box_thickness</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Thickness of the bounding box outline.</td>
+</tr>
+
+<tr>
+<td align="left"><code>box_selected_thickness</code></td>
+<td align="left" style="width: 25%;">
+
+```python
+int | None
+```
+
+</td>
+<td align="left"><code>None</code></td>
+<td align="left">Thickness of the bounding box outline when it is selected.</td>
+</tr>
+
+<tr>
 <td align="left"><code>height</code></td>
 <td align="left" style="width: 25%;">
 
 ```python
 int | str | None
 ```
```

