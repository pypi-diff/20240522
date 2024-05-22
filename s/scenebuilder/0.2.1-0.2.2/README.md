# Comparing `tmp/scenebuilder-0.2.1.tar.gz` & `tmp/scenebuilder-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenebuilder-0.2.1.tar", max compression
+gzip compressed data, was "scenebuilder-0.2.2.tar", max compression
```

## Comparing `scenebuilder-0.2.1.tar` & `scenebuilder-0.2.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-10-19 10:53:34.751175 scenebuilder-0.2.1/LICENSE
--rw-r--r--   0        0        0     3618 2024-05-13 12:27:12.389926 scenebuilder-0.2.1/README.md
--rw-r--r--   0        0        0      486 2024-05-13 12:26:34.562734 scenebuilder-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       39 2024-05-06 09:11:58.678352 scenebuilder-0.2.1/scenebuilder/__init__.py
--rw-r--r--   0        0        0     1019 2024-05-13 07:57:11.213416 scenebuilder-0.2.1/scenebuilder/actions_stack.py
--rw-r--r--   0        0        0     5205 2024-05-13 12:27:11.416187 scenebuilder-0.2.1/scenebuilder/entities.py
--rw-r--r--   0        0        0      471 2024-05-13 11:58:07.494491 scenebuilder-0.2.1/scenebuilder/main.py
--rw-r--r--   0        0        0      454 2024-05-13 06:48:29.276267 scenebuilder-0.2.1/scenebuilder/mixins.py
--rw-r--r--   0        0        0     2196 2024-05-13 06:48:28.415383 scenebuilder-0.2.1/scenebuilder/observer_utils.py
--rw-r--r--   0        0        0     4207 2024-05-13 06:48:27.525252 scenebuilder-0.2.1/scenebuilder/patch_manager.py
--rw-r--r--   0        0        0     4333 2024-05-13 06:48:26.526321 scenebuilder-0.2.1/scenebuilder/patches.py
--rw-r--r--   0        0        0    24724 2024-05-13 12:27:11.554771 scenebuilder-0.2.1/scenebuilder/scenebuilder.py
--rw-r--r--   0        0        0     7157 2024-05-13 12:27:11.420498 scenebuilder-0.2.1/scenebuilder/ui_components.py
--rw-r--r--   0        0        0     7773 2024-05-13 12:27:11.446336 scenebuilder-0.2.1/scenebuilder/utils.py
--rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 scenebuilder-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4205 2024-05-15 14:52:52.630508 scenebuilder-0.2.2/README.md
+-rw-r--r--   0        0        0      486 2024-05-22 13:03:53.567143 scenebuilder-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-05-13 12:34:00.208538 scenebuilder-0.2.2/scenebuilder/__init__.py
+-rw-r--r--   0        0        0     1019 2024-05-22 13:02:21.441055 scenebuilder-0.2.2/scenebuilder/actions_stack.py
+-rw-r--r--   0        0        0     5118 2024-05-22 13:02:22.513522 scenebuilder-0.2.2/scenebuilder/entities.py
+-rw-r--r--   0        0        0      832 2024-05-22 13:02:23.030691 scenebuilder-0.2.2/scenebuilder/main.py
+-rw-r--r--   0        0        0      454 2024-05-22 13:02:23.481805 scenebuilder-0.2.2/scenebuilder/mixins.py
+-rw-r--r--   0        0        0     2196 2024-05-22 13:02:24.814981 scenebuilder-0.2.2/scenebuilder/observer_utils.py
+-rw-r--r--   0        0        0     4231 2024-05-22 13:02:25.370139 scenebuilder-0.2.2/scenebuilder/patch_manager.py
+-rw-r--r--   0        0        0     4345 2024-05-22 13:02:25.870949 scenebuilder-0.2.2/scenebuilder/patches.py
+-rw-r--r--   0        0        0    26155 2024-05-22 13:02:26.588949 scenebuilder-0.2.2/scenebuilder/scenebuilder.py
+-rw-r--r--   0        0        0     7164 2024-05-22 13:02:27.289875 scenebuilder-0.2.2/scenebuilder/ui_components.py
+-rw-r--r--   0        0        0     7785 2024-05-22 13:02:27.792935 scenebuilder-0.2.2/scenebuilder/utils.py
+-rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 scenebuilder-0.2.2/PKG-INFO
```

### Comparing `scenebuilder-0.2.1/README.md` & `scenebuilder-0.2.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 # SceneBuilder
 
 ## Overview
 
-**SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments in a 10x10m grid for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
+**SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
 
 <!-- ![Scene Example 1](/assets/scene1.png){width=10 height=10} -->
 <p align="center">
-  <img src="/assets/scene1.png" alt="First Image" width="40%" />
-  <img src="/assets/scene2.png" alt="Second Image" width="40%" />
+  <img src="/assets/scene1.png" alt="Example Scene 1" width="40%" />
+  <img src="/assets/scene2.png" alt="Example Scene 2" width="40%" />
 </p>
 
+
 ## Installation
 
-To install SceneBuilder, run the following command:
+To install SceneBuilder, you have two options:
 
-```bash
-pip install scenebuilder
-```
-
-This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
+1. **Using pip (recommended)**:
+   ```bash
+   pip install scenebuilder
+   ```
+
+2. **From source**:
+   ```bash
+   git clone git@github.com:enac-drones/scenebuilder.git
+   pip install -e .
+   ```
 
 ## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
 ## Quick Start Guide
 
@@ -49,33 +55,40 @@
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
 
 # Open the GUI to draw a scene
 scene.draw_scene()
 ```
 
-Load in an existing compatible json file for modification:
+Alternatively, load in an existing compatible json file for modification:
 
 ```python
+scene = SceneBuilder()
 scene.load_scene("path/to/your_file.json")
 scene.draw_scene()
 ```
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Clear temporary points**: To clear building vertices prior to completing the building, or to remove a drone's starting point before placing the goal, press 'esc' or 'escape'.
-- **Undo drone/obstacle placement**: To remove the last obstacle or drone that was placed, press ctrl+z.
+- **Undo drone/obstacle placement**: To remove the last obstacle or drone that was placed, press z or ctrl+z. *
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
+**_*Note: due to a quirk in tkinter, some standard keystrokes starting with ctrl/cmd are sometimes captured by the system instead of SceneBuilder, for this reason we provide the option to use them without the leading ctrl/cmd, for example "z" instead of "ctrl/cmd + z" for undo. This applies for the following commands usually found in the 'edit' dropdown menu on most systems:  <u>undo, redo, copy, paste, cut</u>_** **
+
+**_**Not all of <u>undo, redo, copy, paste, cut</u> are currently implemented, this is a work in progress._**
+
+
+
 ## Saving Scenes
 
 Once you have created a scene, you can save it to a JSON or GeoJSON file by clicking the 'Save' button in the GUI. You will then be prompted to select whether you want to use our basic JSON format or GeoGSON.
 
 **_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
```

### Comparing `scenebuilder-0.2.1/scenebuilder/actions_stack.py` & `scenebuilder-0.2.2/scenebuilder/actions_stack.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.1/scenebuilder/entities.py` & `scenebuilder-0.2.2/scenebuilder/entities.py`

 * *Files 22% similar despite different names*

```diff
@@ -101,36 +101,38 @@
 
         Args:
             delta (ArrayLike): 2D array
         """
         for vertex in self.vertices:
             vertex += delta
 
-    def insert_vertex(self, position, tolerance=0.1):
-        """Insert a vertex at a given position if near an edge"""
-        for i in range(len(self.vertices)):
-            start_point = self.vertices[i]
-            end_point = self.vertices[(i + 1) % len(self.vertices)]
-
-            if self._point_near_edge(position, start_point, end_point, tolerance):
-                self.vertices = np.insert(self.vertices, i + 1, position, axis=0)
-                return True
-        return False
-
-    def _point_near_edge(self, point, start, end, tolerance):
-        """Check if the point is near the edge defined by start and end points"""
-        # Compute the distance of the point from the line segment
-        line_vector = np.array(end) - np.array(start)
-        point_vector = np.array(point) - np.array(start)
-        # Compute the projection of point_vector onto line_vector
-        proj_length = np.dot(point_vector, line_vector) / np.linalg.norm(line_vector)
-
-        if 0 <= proj_length <= np.linalg.norm(line_vector):
-            # The projection is on the line segment
-            proj_vector = proj_length * line_vector / np.linalg.norm(line_vector)
-            distance = np.linalg.norm(point_vector - proj_vector)
-            return distance < tolerance
+    def insert_vertex(self, position, tolerance):
+        """Insert a vertex at a given position if near an edge (position and tolerance in data coordinates)"""
+        position = np.array(position)
+
+        # Compute vectors
+        start_points = self.vertices
+        end_points = np.roll(self.vertices, -1, axis=0)
+        line_vectors = end_points - start_points
+        point_vectors = position - start_points
+
+        # Compute projections
+        line_norms = np.linalg.norm(line_vectors, axis=1)
+        proj_lengths = np.einsum('ij,ij->i', point_vectors, line_vectors) / line_norms
+        valid_projs = (proj_lengths >= 0) & (proj_lengths <= line_norms)
+
+        # Compute distances
+        proj_vectors = np.outer(proj_lengths, np.ones(2)) * line_vectors / line_norms[:, None]
+        distances = np.linalg.norm(point_vectors - proj_vectors, axis=1)
+
+        # Find the edge with minimum distance within tolerance
+        near_edges = distances < tolerance
+        if np.any(near_edges & valid_projs):
+            i = np.where(near_edges & valid_projs)[0][0]
+            self.vertices = np.insert(self.vertices, i + 1, position, axis=0)
+            return True
         return False
+    
 
     def contains_point(self, point):
         polygon = Polygon(self.vertices)
         return polygon.contains_point(point)
```

### Comparing `scenebuilder-0.2.1/scenebuilder/observer_utils.py` & `scenebuilder-0.2.2/scenebuilder/observer_utils.py`

 * *Files identical despite different names*

### Comparing `scenebuilder-0.2.1/scenebuilder/patch_manager.py` & `scenebuilder-0.2.2/scenebuilder/patch_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import matplotlib.pyplot as plt
 
 from matplotlib.lines import Line2D
 from typing import List
 import numpy as np
-from .entities import Obstacle, Drone
-from .patches import ObstaclePatch, DronePatch, Marker
+from scenebuilder.entities import Obstacle, Drone
+from scenebuilder.patches import ObstaclePatch, DronePatch, Marker
 
 
 class PatchManager:
     def __init__(self, ax: plt.Axes):
         self.ax = ax
         self.building_patches: dict[Obstacle, ObstaclePatch] = {}
         self.drone_patches: dict[Drone, DronePatch] = {}
```

### Comparing `scenebuilder-0.2.1/scenebuilder/patches.py` & `scenebuilder-0.2.2/scenebuilder/patches.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numpy.typing import ArrayLike
 
 import numpy as np
 from matplotlib.patches import FancyArrow, Polygon
 from matplotlib.lines import Line2D
 import matplotlib.pyplot as plt
 
-from .entities import Drone, Obstacle
+from scenebuilder.entities import Drone, Obstacle
 
 
 class Arrow:
     """Class to create a FancyArrow object"""
 
     def __init__(self, start: ArrayLike, end: ArrayLike, ax: plt.Axes) -> None:
         self.start = np.array(start)
```

### Comparing `scenebuilder-0.2.1/scenebuilder/scenebuilder.py` & `scenebuilder-0.2.2/scenebuilder/scenebuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 
 import numpy as np
 
-from .entities import Drone, Obstacle
-from .utils import (
+from scenebuilder.entities import Drone, Obstacle
+from scenebuilder.utils import (
     distance_between_points,
     create_json,
     get_case_from_dict,
     convert_from_geojson,
 )
-from .utils import load_from_json, validate_json_path
-from .patch_manager import PatchManager
-from .actions_stack import ActionsStack
-from .ui_components import UIComponents
-from .observer_utils import Observer, Observable
+from scenebuilder.utils import load_from_json, validate_json_path
+from scenebuilder.patch_manager import PatchManager
+from scenebuilder.actions_stack import ActionsStack
+from scenebuilder.ui_components import UIComponents
+from scenebuilder.observer_utils import Observer, Observable
 from threading import Timer
 from pathlib import Path
 import traceback
 import os
 
 
 class SceneBuilder(Observer, Observable):
 
     CLICK_THRESHOLD = 0.14
     FIG_SIZE = (8, 8.5)
     AXIS_LIMITS = (-5, 5)
+    PIXEL_TOLERANCE = 20 #within this many pixels a click is considered "on" a line or point
 
     def __init__(self):
         # initialise Observable (Observer has no init)
         super().__init__()
         self._selected_building: Obstacle = None
         self.original_colors: dict = {}
         # Setup the default plot
@@ -183,15 +184,21 @@
         self.on_click = self.fig.canvas.mpl_connect(
             "button_press_event", self._on_click
         )
         self.on_key = self.fig.canvas.mpl_connect("key_press_event", self._on_key_press)
         self.fig.canvas.mpl_connect("button_release_event", self._on_button_release)
         self.fig.canvas.mpl_connect("motion_notify_event", self._on_mouse_move)
         # self.resize=self.fig.canvas.mpl_connect('resize_event', lambda x:print("tool triggered"))
+        self.ax.callbacks.connect("xlim_changed", self._on_axes_change)
+        self.ax.callbacks.connect("ylim_changed", self._on_axes_change)
         return None
+    
+    def _on_axes_change(self, event):
+        self._reset_click_threshold()
+        # print('axes changed')
 
     def _disconnect_event_handlers(self) -> None:
         self.fig.canvas.mpl_disconnect(self.on_click)
         self.fig.canvas.mpl_disconnect(self.on_key)
         self.fig.canvas.mpl_disconnect(self.on_pick)
 
         return None
@@ -303,22 +310,44 @@
 
             # add drone patch to patch_manager
             self.patch_manager.add_drone_patch(self.current_drone)
             self.current_drone = None
             self._update()
         return None
 
-    def _add_new_vertex(self, event) -> bool:
+    
+    def _reset_click_threshold(self)->None:
+            """Convert pixel tolerance to data coordinates and call Obstacle's insert_vertex"""
+            # Get the axis limits
+            xlim = self.ax.get_xlim()
+            ylim = self.ax.get_ylim()
+
+            # Calculate the display-to-data ratio for both x and y axes
+            bbox = self.ax.get_window_extent().transformed(self.fig.dpi_scale_trans.inverted())
+            width_pixels = bbox.width * self.fig.dpi
+            height_pixels = bbox.height * self.fig.dpi
+
+            x_ratio = (xlim[1] - xlim[0]) / width_pixels
+            y_ratio = (ylim[1] - ylim[0]) / height_pixels
+
+            # Use the larger of the two ratios to ensure tolerance covers both dimensions
+            threshold = self.PIXEL_TOLERANCE * max(x_ratio, y_ratio)
+            self.CLICK_THRESHOLD = threshold
+            return None
+
+    
+    def _add_new_vertex(self, event):
+        """Tries to add a new vertex if user clicks near an building edge"""
+        position = (event.xdata, event.ydata)
         for building in self.buildings:
-            if building.insert_vertex((event.xdata, event.ydata)):
+            if building.insert_vertex(position, tolerance = self.CLICK_THRESHOLD):
                 # Redraw the building if a vertex was added
                 self.patch_manager.redraw_building(building)
                 self._update()
                 return True
-        return False
 
     def _handle_deselect(self, event):
         if self.selected_building:
             if not self.selected_building.contains_point([event.xdata, event.ydata]):
                 self.selected_building = None
             return True
 
@@ -446,15 +475,15 @@
         # switch between building and drone placement modes
         self._switch_mode(event)
 
         if event.key == "tab" and self.mode == "building":
             # plot the building
             self._finalize_building()
 
-        if event.key in ["cmd+z", "ctrl+z"]:
+        if event.key in ["z","cmd+z", "ctrl+z"]:
             self._undo_last_action()
 
         # if event.key in ["cmd+s", "ctrl+s"]:
         #     self._create_json(self.output_path)
 
         elif event.key in ["backspace", "delete"]:
             self._delete_selected_building()
```

### Comparing `scenebuilder-0.2.1/scenebuilder/ui_components.py` & `scenebuilder-0.2.2/scenebuilder/ui_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
-from .observer_utils import Observable
+from scenebuilder.observer_utils import Observable
 from matplotlib.widgets import TextBox
 from tkinter import Tk, filedialog
 from pathlib import Path
 import os
 
 # Initialize Tkinter just once
 root = Tk()
@@ -33,15 +33,15 @@
             "save": {
                 "axis": self.fig.add_axes([0.33, button_y_val, 0.15, 0.05]),
                 "label": "Save",
                 "callback": self.show_format_options,
             },
             "load_json": {
                 "axis": self.fig.add_axes([0.49, button_y_val, 0.15, 0.05]),
-                "label": "Load JSON",
+                "label": "Load",
                 "callback": self.on_load,
             },
         }
 
         # Initialize buttons and register callbacks
         for key, btn_info in self.buttons.items():
             button = plt.Button(btn_info["axis"], btn_info["label"])
@@ -65,15 +65,15 @@
         # self.text_box.set_val("")
         #################OUTPUT FILE INFO#####################
         # self.fig.text(
         #     0.1,
         #     0.86,
         #     "Current output file: ",
         #     fontsize=10,  # Makes the font larger
-        #     fontweight="bold",  # Makes the font bold
+        #     fontweight="bold",  # Makes  the font bold
         #     color="k",  # Changes the text color
         # )
 
         # self.current_file_text = self.fig.text(
         #     0.32,
         #     0.86,
         #     "scenebuilder.json",
@@ -153,15 +153,14 @@
         # Get the current working directory
         current_directory = os.getcwd()
         filename = filedialog.asksaveasfilename(
             initialdir=current_directory,
             initialfile="scenebuilder",
             defaultextension=extension,
         )
-
         if not filename:
             return
 
         self.notify_observers("save", input=filename)
 
     def on_load(self, event):
         # Get the current working directory
```

### Comparing `scenebuilder-0.2.1/scenebuilder/utils.py` & `scenebuilder-0.2.2/scenebuilder/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.typing import ArrayLike
 
 # from scenebuilder.json_utils import dump_to_json
-from .entities import Drone, Obstacle
+from scenebuilder.entities import Drone, Obstacle
 
 # file to store useful json utilities
 import json, os, sys
 from pathlib import Path
 
 
 def distance_between_points(p1: ArrayLike, p2: ArrayLike) -> float:
```

### Comparing `scenebuilder-0.2.1/PKG-INFO` & `scenebuilder-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scenebuilder
-Version: 0.2.1
+Version: 0.2.2
 Summary: A simple GUI to create 2D scenes with obstacles and drone paths for multi-agent path planning algorithms
 Author: Adrian del Ser
 Author-email: adrian.delser@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -12,31 +12,37 @@
 Requires-Dist: numpy (>=1.26.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # SceneBuilder
 
 ## Overview
 
-**SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments in a 10x10m grid for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
+**SceneBuilder** is a Python package that provides a Matplotlib-based GUI for designing 2D test environments for use in multiagent path planning algorithms. Users can draw polygons to represent obstacles and arrows to indicate the starting and ending points of each agent's path.
 
 <!-- ![Scene Example 1](/assets/scene1.png){width=10 height=10} -->
 <p align="center">
-  <img src="/assets/scene1.png" alt="First Image" width="40%" />
-  <img src="/assets/scene2.png" alt="Second Image" width="40%" />
+  <img src="/assets/scene1.png" alt="Example Scene 1" width="40%" />
+  <img src="/assets/scene2.png" alt="Example Scene 2" width="40%" />
 </p>
 
+
 ## Installation
 
-To install SceneBuilder, run the following command:
+To install SceneBuilder, you have two options:
 
-```bash
-pip install scenebuilder
-```
-
-This command installs SceneBuilder along with numpy and matplotlib, ensuring that everything needed to run the GUI is properly set up.
+1. **Using pip (recommended)**:
+   ```bash
+   pip install scenebuilder
+   ```
+
+2. **From source**:
+   ```bash
+   git clone git@github.com:enac-drones/scenebuilder.git
+   pip install -e .
+   ```
 
 ## Prerequisites
 
 SceneBuilder's prerequisites are defined in the pyproject.toml file and include Matplotlib and numpy.
 
 ## Quick Start Guide
 
@@ -63,33 +69,40 @@
 # Create an instance of the SceneBuilder
 scene = SceneBuilder()
 
 # Open the GUI to draw a scene
 scene.draw_scene()
 ```
 
-Load in an existing compatible json file for modification:
+Alternatively, load in an existing compatible json file for modification:
 
 ```python
+scene = SceneBuilder()
 scene.load_scene("path/to/your_file.json")
 scene.draw_scene()
 ```
 
 ## Features
 
 - **Draw Obstacles**: Click within the GUI to place vertices of polygons that represent obstacles. Press Tab to complete an obstacle.
 - **Add new obstacle vertices**: To add new vertices, click somewhere on the polygon's perimeter and drag to move the vertex to its desired location.
 - **Set Drone Paths**: Click once to place the starting point, and again to place the goal of an agent/drone. An arrow will automatically be drawn from start to goal.
 - **Move or adjust existing obstacles/drones**: Obstacles and drones can be moved by clicking and dragging. Drone start and goal points, as well as existing obstacle vertices can be moved in the same way.
 - **Switch between Obstacle and Drone Modes**: Press b to switch to building/obstacle mode. Press d to switch to drone/agent mode. Alternatively click the Switch button on the bottom left of the gui.
 - **Delete obstacles**: Select the obstacle and press delete or backspace. NOTE this is not yet available for drones.
 - **Clear temporary points**: To clear building vertices prior to completing the building, or to remove a drone's starting point before placing the goal, press 'esc' or 'escape'.
-- **Undo drone/obstacle placement**: To remove the last obstacle or drone that was placed, press ctrl+z.
+- **Undo drone/obstacle placement**: To remove the last obstacle or drone that was placed, press z or ctrl+z. *
 - **Reset Scene**: To reset the scene to a blank canvas, click the Reset button in the gui.
 
+**_*Note: due to a quirk in tkinter, some standard keystrokes starting with ctrl/cmd are sometimes captured by the system instead of SceneBuilder, for this reason we provide the option to use them without the leading ctrl/cmd, for example "z" instead of "ctrl/cmd + z" for undo. This applies for the following commands usually found in the 'edit' dropdown menu on most systems:  <u>undo, redo, copy, paste, cut</u>_** **
+
+**_**Not all of <u>undo, redo, copy, paste, cut</u> are currently implemented, this is a work in progress._**
+
+
+
 ## Saving Scenes
 
 Once you have created a scene, you can save it to a JSON or GeoJSON file by clicking the 'Save' button in the GUI. You will then be prompted to select whether you want to use our basic JSON format or GeoGSON.
 
 **_Unless otherwise specified, the file is saved as "scenebuilder.json" in the current working directory._**
 
 ## Contributing
```

