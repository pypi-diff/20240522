# Comparing `tmp/tksheet-7.1.9.tar.gz` & `tmp/tksheet-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tksheet-7.1.9.tar", last modified: Sun Apr 21 17:20:29 2024, max compression
+gzip compressed data, was "tksheet-7.2.0.tar", last modified: Wed May 22 16:10:33 2024, max compression
```

## Comparing `tksheet-7.1.9.tar` & `tksheet-7.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:29.001799 tksheet-7.1.9/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.1.9/LICENSE.txt
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-21 17:20:28.997799 tksheet-7.1.9/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)     3914 2024-01-30 18:05:54.000000 tksheet-7.1.9/README.md
--rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-04-18 17:49:38.000000 tksheet-7.1.9/pyproject.toml
--rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-04-21 17:20:29.001799 tksheet-7.1.9/setup.cfg
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:28.997799 tksheet-7.1.9/tksheet/
--rw-rw-r--   0 rg        (1000) rg        (1000)     1994 2024-04-18 17:49:41.000000 tksheet-7.1.9/tksheet/__init__.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/colors.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   100204 2024-04-18 17:26:28.000000 tksheet-7.1.9/tksheet/column_headers.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/formatters.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    39697 2024-04-19 13:45:43.000000 tksheet-7.1.9/tksheet/functions.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   318310 2024-04-21 14:51:11.000000 tksheet-7.1.9/tksheet/main_table.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-04-18 07:38:29.000000 tksheet-7.1.9/tksheet/other_classes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   105673 2024-04-18 17:25:32.000000 tksheet-7.1.9/tksheet/row_index.py
--rw-rw-r--   0 rg        (1000) rg        (1000)   258919 2024-04-21 14:40:22.000000 tksheet-7.1.9/tksheet/sheet.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    11978 2024-04-20 18:10:51.000000 tksheet-7.1.9/tksheet/sheet_options.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     6681 2024-03-30 19:35:35.000000 tksheet-7.1.9/tksheet/text_editor.py
--rw-rw-r--   0 rg        (1000) rg        (1000)    13398 2024-03-19 10:12:20.000000 tksheet-7.1.9/tksheet/themes.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     8275 2024-02-08 18:45:37.000000 tksheet-7.1.9/tksheet/top_left_rectangle.py
--rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.1.9/tksheet/types.py
--rw-rw-r--   0 rg        (1000) rg        (1000)     2288 2024-04-18 17:22:58.000000 tksheet-7.1.9/tksheet/vars.py
-drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-04-21 17:20:28.997799 tksheet-7.1.9/tksheet.egg-info/
--rw-r--r--   0 rg        (1000) rg        (1000)     6013 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/PKG-INFO
--rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/SOURCES.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/dependency_links.txt
--rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-04-21 17:20:28.000000 tksheet-7.1.9/tksheet.egg-info/top_level.txt
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 16:10:33.647251 tksheet-7.2.0/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1101 2024-01-20 17:50:45.000000 tksheet-7.2.0/LICENSE.txt
+-rw-r--r--   0 rg        (1000) rg        (1000)     6145 2024-05-22 16:10:33.647251 tksheet-7.2.0/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)     4046 2024-05-15 18:18:34.000000 tksheet-7.2.0/README.md
+-rw-rw-r--   0 rg        (1000) rg        (1000)     1099 2024-05-21 09:44:44.000000 tksheet-7.2.0/pyproject.toml
+-rw-rw-r--   0 rg        (1000) rg        (1000)       38 2024-05-22 16:10:33.647251 tksheet-7.2.0/setup.cfg
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 16:10:33.647251 tksheet-7.2.0/tksheet/
+-rw-rw-r--   0 rg        (1000) rg        (1000)     2124 2024-05-21 18:44:16.000000 tksheet-7.2.0/tksheet/__init__.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    51594 2024-01-25 08:44:04.000000 tksheet-7.2.0/tksheet/colors.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   100805 2024-05-22 14:14:12.000000 tksheet-7.2.0/tksheet/column_headers.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    10037 2024-01-25 08:44:04.000000 tksheet-7.2.0/tksheet/formatters.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    40835 2024-05-20 07:30:00.000000 tksheet-7.2.0/tksheet/functions.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   323910 2024-05-22 15:53:03.000000 tksheet-7.2.0/tksheet/main_table.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    13628 2024-05-17 10:30:02.000000 tksheet-7.2.0/tksheet/other_classes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   107199 2024-05-22 14:26:41.000000 tksheet-7.2.0/tksheet/row_index.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)   267442 2024-05-22 16:00:15.000000 tksheet-7.2.0/tksheet/sheet.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)    12262 2024-05-20 09:45:04.000000 tksheet-7.2.0/tksheet/sheet_options.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     6548 2024-05-21 08:53:42.000000 tksheet-7.2.0/tksheet/text_editor.py
+-rw-r--r--   0 rg        (1000) rg        (1000)    14474 2024-05-21 08:36:35.000000 tksheet-7.2.0/tksheet/themes.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     8356 2024-05-19 18:22:05.000000 tksheet-7.2.0/tksheet/top_left_rectangle.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)      340 2024-01-25 08:44:04.000000 tksheet-7.2.0/tksheet/types.py
+-rw-rw-r--   0 rg        (1000) rg        (1000)     3452 2024-05-20 09:29:16.000000 tksheet-7.2.0/tksheet/vars.py
+drwxrwxr-x   0 rg        (1000) rg        (1000)        0 2024-05-22 16:10:33.647251 tksheet-7.2.0/tksheet.egg-info/
+-rw-r--r--   0 rg        (1000) rg        (1000)     6145 2024-05-22 16:10:33.000000 tksheet-7.2.0/tksheet.egg-info/PKG-INFO
+-rw-rw-r--   0 rg        (1000) rg        (1000)      481 2024-05-22 16:10:33.000000 tksheet-7.2.0/tksheet.egg-info/SOURCES.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        1 2024-05-22 16:10:33.000000 tksheet-7.2.0/tksheet.egg-info/dependency_links.txt
+-rw-rw-r--   0 rg        (1000) rg        (1000)        8 2024-05-22 16:10:33.000000 tksheet-7.2.0/tksheet.egg-info/top_level.txt
```

### Comparing `tksheet-7.1.9/LICENSE.txt` & `tksheet-7.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.9/PKG-INFO` & `tksheet-7.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.9
+Version: 7.2.0
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # tksheet
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
 ### **A python tkinter table widget**
 
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
@@ -97,14 +97,14 @@
 # add 2 empty columns and add the change to undo stack
 sheet.insert_columns(columns=2, idx=4, undo=True)
 
 # delete columns 0 and 3 and add the change to undo stack
 sheet.delete_columns(columns=[0, 3], undo=True)
 ```
 
-### **light blue theme**
+### **light green theme**
 
-![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light green theme](https://github.com/ragardner/tksheet/assets/26602401/790ee9bd-b4de-48df-8c44-33f303061d84)
 
-### **black theme**
+### **dark theme**
 
-![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet dark theme](https://github.com/ragardner/tksheet/assets/26602401/fc8a0407-1486-46cf-b852-9bcff23160e5)
```

### Comparing `tksheet-7.1.9/README.md` & `tksheet-7.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # tksheet
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
 ### **A python tkinter table widget**
 
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
@@ -55,14 +55,14 @@
 # add 2 empty columns and add the change to undo stack
 sheet.insert_columns(columns=2, idx=4, undo=True)
 
 # delete columns 0 and 3 and add the change to undo stack
 sheet.delete_columns(columns=[0, 3], undo=True)
 ```
 
-### **light blue theme**
+### **light green theme**
 
-![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light green theme](https://github.com/ragardner/tksheet/assets/26602401/790ee9bd-b4de-48df-8c44-33f303061d84)
 
-### **black theme**
+### **dark theme**
 
-![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet dark theme](https://github.com/ragardner/tksheet/assets/26602401/fc8a0407-1486-46cf-b852-9bcff23160e5)
```

### Comparing `tksheet-7.1.9/pyproject.toml` & `tksheet-7.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tksheet"
 description = "Tkinter table / sheet widget"
 readme = "README.md"
-version = "7.1.9"
+version = "7.2.0"
 authors = [{ name = "ragardner", email = "github@ragardner.simplelogin.com" }]
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["tkinter", "table", "widget", "sheet", "grid", "tk"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `tksheet-7.1.9/tksheet/__init__.py` & `tksheet-7.2.0/tksheet/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ruff: noqa: F401
 
 """
 tksheet - A Python tkinter table widget
 """
 
-__version__ = "7.1.9"
+__version__ = "7.2.0"
 
 from .colors import (
     color_map,
 )
 from .column_headers import ColumnHeaders
 from .formatters import (
     Formatter,
@@ -28,46 +28,52 @@
     to_bool,
     to_float,
     to_int,
     to_str,
     try_to_bool,
 )
 from .functions import (
+    add_highlight,
     alpha2idx,
     alpha2num,
     consecutive_chunks,
     consecutive_ranges,
     data_to_displayed_idxs,
     displayed_to_data_idxs,
     dropdown_search_function,
     event_dict,
     get_checkbox_dict,
     get_checkbox_kwargs,
+    get_csv_str_dialect,
+    get_data_from_clipboard,
     get_dropdown_dict,
     get_dropdown_kwargs,
     get_index_of_gap_in_sorted_integer_seq_forward,
     get_index_of_gap_in_sorted_integer_seq_reverse,
     get_n2a,
     get_new_indexes,
     get_seq_without_gaps_at_index,
+    insert_items,
     is_iterable,
     move_elements_by_mapping,
     move_elements_to,
+    new_tk_event,
     num2alpha,
     rounded_box_coords,
     span_dict,
     tksheet_type_error,
 )
 from .main_table import MainTable
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DrawnItem,
     EventDataDict,
     GeneratedMouseEvent,
+    Highlight,
     Selected,
     Span,
     SpanRange,
     TextCfg,
 )
 from .row_index import RowIndex
 from .sheet import Dropdown, Sheet
```

### Comparing `tksheet-7.1.9/tksheet/colors.py` & `tksheet-7.2.0/tksheet/colors.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.9/tksheet/column_headers.py` & `tksheet-7.2.0/tksheet/column_headers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import tkinter as tk
 from collections import defaultdict
 from collections.abc import (
     Callable,
+    Sequence,
 )
 from functools import (
     partial,
 )
 from itertools import (
     cycle,
     islice,
@@ -17,18 +18,19 @@
 
 from .colors import (
     color_map,
 )
 from .formatters import is_bool_like, try_to_bool
 from .functions import (
     consecutive_ranges,
-    ev_stack_dict,
     event_dict,
     get_n2a,
     is_contiguous,
+    new_tk_event,
+    pickled_event_dict,
     rounded_box_coords,
     try_binding,
 )
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DropdownStorage,
@@ -37,14 +39,16 @@
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
     USER_OS,
     rc_binding,
     symbols_set,
+    text_editor_close_bindings,
+    text_editor_newline_bindings,
     text_editor_to_unbind,
 )
 
 
 class ColumnHeaders(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
@@ -119,31 +123,44 @@
         self.hidd_checkbox = {}
         self.hidd_boxes = set()
 
         self.default_header = kwargs["default_header"].lower()
         self.align = kwargs["header_align"]
         self.basic_bindings()
 
+    def event_generate(self, *args, **kwargs) -> None:
+        for arg in args:
+            if self.MT and arg in self.MT.event_linker:
+                self.MT.event_linker[arg]()
+            else:
+                super().event_generate(*args, **kwargs)
+
     def basic_bindings(self, enable: bool = True):
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
             self.bind(rc_binding, self.rc)
             self.bind("<MouseWheel>", self.mousewheel)
+            if USER_OS == "linux":
+                self.bind("<Button-4>", self.mousewheel)
+                self.bind("<Button-5>", self.mousewheel)
         else:
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
             self.unbind(rc_binding)
             self.unbind("<MouseWheel>")
+            if USER_OS == "linux":
+                self.unbind("<Button-4>")
+                self.unbind("<Button-5>")
 
     def mousewheel(self, event: object):
         maxlines = 0
         if isinstance(self.MT._headers, int):
             if len(self.MT.data) > self.MT._headers:
                 maxlines = max(
                     len(
@@ -669,19 +686,19 @@
             return self.MT.col_positions[col]
         elif col > self.dragged_col.to_move[-1]:
             return self.MT.col_positions[col + 1]
         return self.MT.col_positions[col]
 
     def show_drag_and_drop_indicators(
         self,
-        xpos,
-        y1,
-        y2,
-        cols,
-    ):
+        xpos: float,
+        y1: float,
+        y2: float,
+        cols: Sequence[int],
+    ) -> None:
         self.hide_resize_and_ctrl_lines()
         self.create_resize_line(
             xpos,
             0,
             xpos,
             self.current_height,
             width=3,
@@ -694,21 +711,21 @@
                 start_cell=(boxst, 0),
                 end_cell=(boxend, len(self.MT.row_positions) - 1),
                 dash=(),
                 outline=self.PAR.ops.drag_and_drop_bg,
                 delete_on_timer=False,
             )
 
-    def hide_resize_and_ctrl_lines(self, ctrl_lines=True):
+    def hide_resize_and_ctrl_lines(self, ctrl_lines: bool = True) -> None:
         self.delete_resize_lines()
         self.MT.delete_resize_lines()
         if ctrl_lines:
             self.MT.delete_ctrl_outlines()
 
-    def scroll_if_event_offscreen(self, event: object):
+    def scroll_if_event_offscreen(self, event: object) -> bool:
         xcheck = self.xview()
         need_redraw = False
         if event.x > self.winfo_width() and len(xcheck) > 1 and xcheck[1] < 1:
             try:
                 self.MT.xview_scroll(1, "units")
                 self.xview_scroll(1, "units")
             except Exception:
@@ -723,54 +740,54 @@
             except Exception:
                 pass
             self.fix_xview()
             self.MT.x_move_synced_scrolls("moveto", self.MT.xview()[0])
             need_redraw = True
         return need_redraw
 
-    def fix_xview(self):
+    def fix_xview(self) -> None:
         xcheck = self.xview()
         if xcheck and xcheck[0] < 0:
             self.MT.set_xviews("moveto", 0)
         elif len(xcheck) > 1 and xcheck[1] > 1:
             self.MT.set_xviews("moveto", 1)
 
-    def event_over_dropdown(self, c, datacn, event: object, canvasx):
+    def event_over_dropdown(self, c: int, datacn: int, event: object, canvasx: float) -> bool:
         if (
             event.y < self.MT.header_txt_height + 5
             and self.get_cell_kwargs(datacn, key="dropdown")
             and canvasx < self.MT.col_positions[c + 1]
             and canvasx > self.MT.col_positions[c + 1] - self.MT.header_txt_height - 4
         ):
             return True
         return False
 
-    def event_over_checkbox(self, c, datacn, event: object, canvasx):
+    def event_over_checkbox(self, c: int, datacn: int, event: object, canvasx: float) -> bool:
         if (
             event.y < self.MT.header_txt_height + 5
             and self.get_cell_kwargs(datacn, key="checkbox")
             and canvasx < self.MT.col_positions[c] + self.MT.header_txt_height + 4
         ):
             return True
         return False
 
-    def b1_release(self, event: object):
-        if self.being_drawn_item is not None:
-            to_sel = self.MT.coords_and_type(self.being_drawn_item)
+    def b1_release(self, event: object) -> None:
+        if self.being_drawn_item is not None and (to_sel := self.MT.coords_and_type(self.being_drawn_item)):
             r_to_sel, c_to_sel = self.MT.selected.row, self.MT.selected.column
             self.MT.hide_selection_box(self.being_drawn_item)
-            self.being_drawn_item = None
             self.MT.set_currently_selected(
                 r_to_sel,
                 c_to_sel,
                 item=self.MT.create_selection_box(*to_sel, set_current=False),
             )
             sel_event = self.MT.get_select_event(being_drawn_item=self.being_drawn_item)
             try_binding(self.drag_selection_binding_func, sel_event)
             self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
+        else:
+            self.being_drawn_item = None
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
         if self.width_resizing_enabled and self.rsz_w is not None and self.currently_resizing_width:
             self.currently_resizing_width = False
             new_col_pos = int(self.coords("rwl")[0])
             self.hide_resize_and_ctrl_lines(ctrl_lines=False)
             old_width = self.MT.col_positions[self.rsz_w] - self.MT.col_positions[self.rsz_w - 1]
             size = new_col_pos - self.MT.col_positions[self.rsz_w - 1]
@@ -822,33 +839,35 @@
                 )
             ):
                 if c >= len(self.MT.col_positions) - 1:
                     c -= 1
                 event_data = event_dict(
                     name="move_columns",
                     sheet=self.PAR.name,
+                    widget=self,
                     boxes=self.MT.get_boxes(),
                     selected=self.MT.selected,
                     value=c,
                 )
                 if try_binding(self.ch_extra_begin_drag_drop_func, event_data, "begin_move_columns"):
                     data_new_idxs, disp_new_idxs, event_data = self.MT.move_columns_adjust_options_dict(
                         *self.MT.get_args_for_move_columns(
                             move_to=c,
                             to_move=self.dragged_col.to_move,
                         ),
                         move_data=self.PAR.ops.column_drag_and_drop_perform,
+                        move_widths=self.PAR.ops.column_drag_and_drop_perform,
                         event_data=event_data,
                     )
                     event_data["moved"]["columns"] = {
                         "data": data_new_idxs,
                         "displayed": disp_new_idxs,
                     }
                     if self.MT.undo_enabled:
-                        self.MT.undo_stack.append(ev_stack_dict(event_data))
+                        self.MT.undo_stack.append(pickled_event_dict(event_data))
                     self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     try_binding(self.ch_extra_end_drag_drop_func, event_data, "end_move_columns")
                     self.MT.sheet_modified(event_data)
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             c = self.MT.identify_col(x=event.x)
             if (
                 c is not None
@@ -905,16 +924,15 @@
                 fill_iid = self.MT.deselect(c=column, redraw=redraw)
             else:
                 fill_iid = self.select_col(column, redraw=redraw)
         return fill_iid
 
     def select_col(self, c, redraw=False, run_binding_func=True):
         self.MT.deselect("all", redraw=False)
-        box = (0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
-        fill_iid = self.MT.create_selection_box(*box)
+        fill_iid = self.MT.create_selection_box(0, c, len(self.MT.row_positions) - 1, c + 1, "columns")
         if redraw:
             self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         if run_binding_func:
             self.MT.run_selection_binding("columns")
         return fill_iid
 
     def add_selection(self, c, redraw=False, run_binding_func=True, set_as_current=True):
@@ -1274,20 +1292,17 @@
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill)
                 else:
                     self.itemconfig(t, fill=fill, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_line(
+                t = self.create_polygon(
                     points,
                     fill=fill,
-                    width=2,
-                    capstyle=tk.ROUND,
-                    joinstyle=tk.ROUND,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
     def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
         points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
@@ -1316,33 +1331,36 @@
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
+    def configure_scrollregion(self, last_col_line_pos: float) -> None:
+        self.configure(
+            scrollregion=(
+                0,
+                0,
+                last_col_line_pos + self.PAR.ops.empty_horizontal + 2,
+                self.current_height,
+            )
+        )
+
     def redraw_grid_and_text(
         self,
         last_col_line_pos,
         scrollpos_left,
         x_stop,
         start_col,
         end_col,
         scrollpos_right,
         col_pos_exists,
     ):
         try:
-            self.configure(
-                scrollregion=(
-                    0,
-                    0,
-                    last_col_line_pos + self.PAR.ops.empty_horizontal + 2,
-                    self.current_height,
-                )
-            )
+            self.configure_scrollregion(last_col_line_pos=last_col_line_pos)
         except Exception:
             return
         self.hidd_text.update(self.disp_text)
         self.disp_text = {}
         self.hidd_high.update(self.disp_high)
         self.disp_high = {}
         self.hidd_grid.update(self.disp_grid)
@@ -1585,19 +1603,19 @@
                 if showing:
                     self.itemconfig(iid, state="hidden")
                     dct[iid] = False
         return True
 
     def get_redraw_selections(self, startc: int, endc: int) -> dict[str, set[int]]:
         d = defaultdict(set)
-        for item, box in self.MT.get_selection_items(rows=False):
+        for item, box in self.MT.get_selection_items():
             r1, c1, r2, c2 = box.coords
             for c in range(startc, endc):
                 if c1 <= c and c2 > c:
-                    d[box.type_].add(c)
+                    d[box.type_ if box.type_ != "rows" else "cells"].add(c)
         return d
 
     def open_cell(self, event: object = None, ignore_existing_editor=False):
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
@@ -1720,29 +1738,24 @@
             self.text_editor.window = TextEditor(self, newline_binding=self.text_editor_newline_binding)
             self.text_editor.canvas_id = self.create_window((x, y), window=self.text_editor.window, anchor="nw")
         self.text_editor.window.reset(**kwargs)
         if not self.text_editor.open:
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
+        for b in text_editor_newline_bindings:
+            self.text_editor.tktext.bind(b, self.text_editor_newline_binding)
+        for b in text_editor_close_bindings:
+            self.text_editor.tktext.bind(b, self.close_text_editor)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
-        self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(c=c))
-        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(c=c))
-        if USER_OS == "darwin":
-            self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(c=c))
+            self.text_editor.tktext.bind("<FocusOut>", self.close_text_editor)
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
-        self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((c, "Tab")))
-        self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((c, "Return")))
-        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((c, "Return")))
-        if not dropdown:
-            self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((c, "FocusOut")))
-        self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((c, "Escape")))
         return True
 
     # displayed indexes                         #just here to receive text editor arg
     def text_editor_has_wrapped(self, r=0, c=0, check_lines=None):
         if self.width_resizing_enabled:
             curr_width = self.text_editor.window.winfo_width()
             new_width = curr_width + (self.MT.header_txt_height * 2)
@@ -1753,28 +1766,29 @@
                     self.itemconfig(self.dropdown.canvas_id, width=new_width)
                     self.dropdown.window.update_idletasks()
                     self.dropdown.window._reselect()
                 self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False, redraw_table=True)
                 self.coords(self.text_editor.canvas_id, self.MT.col_positions[c] + 1, 0)
 
     # displayed indexes
-    def text_editor_newline_binding(self, r=0, c=0, event: object = None, check_lines=True):
+    def text_editor_newline_binding(self, event: object = None, check_lines=True):
         if not self.height_resizing_enabled:
             return
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_header_height:
             return
         if (
             not check_lines
             or self.MT.get_lines_cell_height(
                 self.text_editor.window.get_num_lines() + 1,
                 font=self.text_editor.tktext.cget("font"),
             )
             > curr_height
         ):
+            c = self.text_editor.column
             new_height = curr_height + self.MT.header_xtra_lines_increment
             space_bot = self.MT.get_space_bot(0)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.text_editor.window.config(height=new_height)
                 self.set_height(new_height, set_TL=True)
@@ -1835,39 +1849,41 @@
                 self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # c is displayed col
-    def close_text_editor(
-        self,
-        editor_info: tuple,
-    ):
+    def close_text_editor(self, event: tk.Event) -> Literal["break"] | None:
         # checking if text editor should be closed or not
-        focused = self.focus_get()
+        # errors if __tk_filedialog is open
+        try:
+            focused = self.focus_get()
+        except Exception:
+            focused = None
         try:
             if focused == self.text_editor.tktext.rc_popup_menu:
                 return "break"
         except Exception:
             pass
-        if focused is None and editor_info:
+        if focused is None:
             return "break"
-        if editor_info[1] == "Escape":
+        if event.keysym == "Escape":
             self.hide_text_editor_and_dropdown()
             return
         # setting cell data with text editor value
         text_editor_value = self.text_editor.get()
-        c = editor_info[0]
+        c = self.text_editor.column
         datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         event_data = event_dict(
             name="end_edit_header",
             sheet=self.PAR.name,
+            widget=self,
             cells_header={datacn: self.get_cell_data(datacn)},
-            key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
+            key=event.keysym,
             value=text_editor_value,
             loc=c,
             column=c,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
@@ -1883,15 +1899,15 @@
                 edited = set_data(value=text_editor_value)
         elif self.input_valid_for_cell(datacn, text_editor_value):
             edited = set_data(value=text_editor_value)
         if edited:
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
-        if editor_info[1] != "FocusOut":
+        if event.keysym != "FocusOut":
             self.focus_set()
         return "break"
 
     def get_dropdown_height_anchor(self, c, text_editor_h=None):
         win_h = 5
         datacn = self.MT.datacn(c)
         for i, v in enumerate(self.get_cell_kwargs(datacn, key="dropdown")["values"]):
@@ -1946,14 +1962,15 @@
             "align": self.get_cell_align(c),
             "values": kwargs["values"],
         }
         if self.dropdown.window:
             self.dropdown.window.reset(**reset_kwargs)
             self.itemconfig(self.dropdown.canvas_id, state="normal")
             self.coords(self.dropdown.canvas_id, self.MT.col_positions[c], ypos)
+            self.dropdown.window.tkraise()
         else:
             self.dropdown.window = self.PAR.dropdown_class(
                 self.winfo_toplevel(),
                 **reset_kwargs,
                 single_index="c",
                 close_dropdown_window=self.close_dropdown_window,
                 search_function=kwargs["search_function"],
@@ -2003,14 +2020,15 @@
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
             kwargs = self.get_cell_kwargs(datacn, key="dropdown")
             pre_edit_value = self.get_cell_data(datacn)
             edited = False
             event_data = event_dict(
                 name="end_edit_header",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_header={datacn: pre_edit_value},
                 key="??",
                 value=selection,
                 loc=c,
                 column=c,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
@@ -2034,15 +2052,15 @@
         self.hide_dropdown_window()
         if redraw:
             self.MT.refresh()
 
     def mouseclick_outside_editor_or_dropdown(self, inside: bool = False):
         closed_dd_coords = self.dropdown.get_coords()
         if self.text_editor.open:
-            self.close_text_editor((self.text_editor.column, "ButtonPress-1"))
+            self.close_text_editor(new_tk_event("ButtonPress-1"))
         if closed_dd_coords is not None:
             self.hide_dropdown_window()
             if inside:
                 self.MT.main_table_redraw_grid_and_text(
                     redraw_header=True,
                     redraw_row_index=False,
                     redraw_table=False,
@@ -2072,26 +2090,27 @@
         check_input_valid=True,
     ):
         if datacn is None:
             datacn = c if self.MT.all_columns_displayed else self.MT.displayed_columns[c]
         event_data = event_dict(
             name="edit_header",
             sheet=self.PAR.name,
+            widget=self,
             cells_header={datacn: self.get_cell_data(datacn)},
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         if isinstance(self.MT._headers, int):
             edited = self.MT.set_cell_data_undo(r=self.MT._headers, c=c, datacn=datacn, value=value, undo=True)
         else:
             self.fix_header(datacn)
             if not check_input_valid or self.input_valid_for_cell(datacn, value):
                 if self.MT.undo_enabled and undo:
-                    self.MT.undo_stack.append(ev_stack_dict(event_data))
+                    self.MT.undo_stack.append(pickled_event_dict(event_data))
                 self.set_cell_data(datacn=datacn, value=value)
                 edited = True
         if edited and cell_resize and self.PAR.ops.cell_auto_resize_enabled:
             if self.height_resizing_enabled:
                 self.set_height_of_header_to_text(self.get_valid_cell_data_as_str(datacn, fix=False))
             self.set_col_width_run_binding(c)
         if redraw:
@@ -2229,14 +2248,15 @@
                 )
             else:
                 value = False
             self.set_cell_data_undo(c, datacn=datacn, value=value, cell_resize=False)
             event_data = event_dict(
                 name="end_edit_header",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_header={datacn: pre_edit_value},
                 key="??",
                 value=value,
                 loc=c,
                 column=c,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
```

### Comparing `tksheet-7.1.9/tksheet/formatters.py` & `tksheet-7.2.0/tksheet/formatters.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.9/tksheet/functions.py` & `tksheet-7.2.0/tksheet/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,49 +1,81 @@
 from __future__ import annotations
 
 import bisect
+import csv
+import io
 import pickle
 import re
+import tkinter as tk
 import zlib
 from collections import deque
 from collections.abc import (
     Callable,
     Generator,
     Iterator,
     Sequence,
 )
 from functools import partial
 from itertools import islice, repeat
 
+from .formatters import (
+    to_bool,
+)
 from .other_classes import (
     Box_nt,
     DotDict,
     EventDataDict,
     Highlight,
+    Loc,
     Span,
 )
 
 compress = partial(zlib.compress, level=1)
 pickle_obj = partial(pickle.dumps, protocol=pickle.HIGHEST_PROTOCOL)
 unpickle_obj = pickle.loads
 
 
+def get_csv_str_dialect(s: str, delimiters: str) -> csv.Dialect:
+    try:
+        return csv.Sniffer().sniff(s[:5000] if len(s) > 5000 else s, delimiters=delimiters)
+    except Exception:
+        return csv.excel_tab
+
+
+def get_data_from_clipboard(
+    widget: tk.Misc,
+    delimiters: str,
+    lineterminator: str = "\n",
+) -> list[list[str]]:
+    data = widget.clipboard_get()
+    dialect = get_csv_str_dialect(data, delimiters=delimiters)
+    if dialect.delimiter in data or lineterminator in data:
+        return list(csv.reader(io.StringIO(data), dialect=dialect, skipinitialspace=True))
+    return [[data]]
+
+
 def pickle_compress(obj: object) -> bytes:
     return compress(pickle_obj(obj))
 
 
 def decompress_load(b: bytes) -> object:
     return pickle.loads(zlib.decompress(b))
 
 
 def tksheet_type_error(kwarg: str, valid_types: list[str], not_type: object) -> str:
     valid_types = ", ".join(f"{type_}" for type_ in valid_types)
     return f"Argument '{kwarg}' must be one of the following types: {valid_types}, " f"not {type(not_type)}."
 
 
+def new_tk_event(keysym: str) -> tk.Event:
+    event = tk.Event()
+    event.keysym = keysym
+    return event
+
+
 def dropdown_search_function(
     search_for: object,
     data: Sequence[object],
 ) -> None | int:
     search_len = len(search_for)
     # search_for in data
     match_rn = float("inf")
@@ -89,14 +121,15 @@
 def selection_box_tup_to_dict(box: tuple) -> dict:
     return {Box_nt(*box[:-1]): box[-1]}
 
 
 def event_dict(
     name: str = None,
     sheet: object = None,
+    widget: tk.Canvas | None = None,
     boxes: None | dict | tuple = None,
     cells_table: None | dict = None,
     cells_header: None | dict = None,
     cells_index: None | dict = None,
     selected: None | tuple = None,
     data: object = None,
     key: None | str = None,
@@ -153,26 +186,24 @@
         column=column,
         resized=DotDict(
             rows=DotDict() if resized_rows is None else resized_rows,
             columns=DotDict() if resized_columns is None else resized_columns,
             # "header": DotDict() if resized_header is None else resized_header,
             # "index": DotDict() if resized_index is None else resized_index,
         ),
+        widget=widget,
     )
 
 
 def change_eventname(event_dict: EventDataDict, newname: str) -> EventDataDict:
     return EventDataDict({**event_dict, **{"eventname": newname}})
 
 
-def ev_stack_dict(d: DotDict) -> DotDict:
-    return DotDict(
-        name=d["eventname"],
-        data=pickle_compress(d),
-    )
+def pickled_event_dict(d: DotDict) -> DotDict:
+    return DotDict(name=d["eventname"], data=pickle_compress(DotDict({k: v for k, v in d.items() if k != "widget"})))
 
 
 def len_to_idx(n: int) -> int:
     if n < 1:
         return 0
     return n - 1
 
@@ -200,16 +231,14 @@
         "text": text,
     }
 
 
 def get_dropdown_dict(**kwargs) -> dict:
     return {
         "values": kwargs["values"],
-        "window": "no dropdown open",
-        "canvas_id": "no dropdown open",
         "select_function": kwargs["selection_function"],
         "modified_function": kwargs["modified_function"],
         "search_function": kwargs["search_function"],
         "validate_input": kwargs["validate_input"],
         "text": kwargs["text"],
         "state": kwargs["state"],
     }
@@ -263,14 +292,21 @@
     return t
 
 
 def is_type_int(o: object) -> bool:
     return isinstance(o, int) and not isinstance(o, bool)
 
 
+def force_bool(o: object) -> bool:
+    try:
+        return to_bool(o)
+    except Exception:
+        return False
+
+
 def str_to_coords(s: str) -> None | tuple[int]:
     s = s.split(":")
 
 
 def alpha2idx(a: str) -> int | None:
     try:
         a = a.upper()
@@ -404,19 +440,21 @@
     except Exception:
         return False
 
 
 def move_elements_by_mapping(
     seq: list[object],
     new_idxs: dict[int, int],
-    old_idxs: dict[int, int],
+    old_idxs: dict[int, int] | None = None,
 ) -> list[object]:
     # move elements of a list around, displacing
     # other elements based on mapping
     # of {old index: new index, ...}
+    if old_idxs is None:
+        old_idxs = dict(zip(new_idxs.values(), new_idxs))
 
     # create dummy list
     res = [0] * len(seq)
 
     # create generator of values yet to be put into res
     remaining = (e for i, e in enumerate(seq) if i not in new_idxs)
 
@@ -1291,18 +1329,20 @@
     span.widget = widget
     return span
 
 
 def mod_event_val(
     event_data: EventDataDict,
     val: object,
-    loc: tuple[int, int] | int,
+    loc: Loc | int,
 ) -> EventDataDict:
     event_data.value = val
-    event_data.loc = loc
+    event_data.loc = Loc(*loc)
+    event_data.row = loc[0]
+    event_data.column = loc[1]
     return event_data
 
 
 def pop_positions(
     itr: Iterator[int],
     to_pop: dict[int, int],  # displayed index: data index
     save_to: dict[int, int],
```

### Comparing `tksheet-7.1.9/tksheet/main_table.py` & `tksheet-7.2.0/tksheet/main_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,30 +48,32 @@
     try_to_bool,
 )
 from .functions import (
     consecutive_ranges,
     decompress_load,
     diff_gen,
     diff_list,
-    ev_stack_dict,
     event_dict,
     gen_formatted,
+    get_data_from_clipboard,
     get_new_indexes,
     get_seq_without_gaps_at_index,
     index_exists,
     insert_items,
     int_x_iter,
     is_iterable,
     is_type_int,
     len_to_idx,
     mod_event_val,
     mod_span,
     mod_span_widget,
     move_elements_by_mapping,
+    new_tk_event,
     pickle_obj,
+    pickled_event_dict,
     rounded_box_coords,
     span_idxs_post_move,
     try_binding,
     unpickle_obj,
 )
 from .other_classes import (
     Box_nt,
@@ -87,17 +89,23 @@
     TextEditorStorage,
 )
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
     USER_OS,
+    bind_add_columns,
+    bind_add_rows,
+    bind_del_columns,
+    bind_del_rows,
     ctrl_key,
     rc_binding,
     symbols_set,
+    text_editor_close_bindings,
+    text_editor_newline_bindings,
     text_editor_to_unbind,
     val_modifying_options,
 )
 
 
 class MainTable(tk.Canvas):
     def __init__(self, *args, **kwargs):
@@ -118,14 +126,23 @@
         self.c_align_cyc = cycle(self.centre_alignment_text_mod_indexes)
         self.allow_auto_resize_columns = True
         self.allow_auto_resize_rows = True
         self.span = self.PAR.span
         self.synced_scrolls = set()
         self.dropdown = DropdownStorage()
         self.text_editor = TextEditorStorage()
+        self.event_linker = {
+            "<<Copy>>": self.ctrl_c,
+            "<<Cut>>": self.ctrl_x,
+            "<<Paste>>": self.ctrl_v,
+            "<<Delete>>": self.delete_key,
+            "<<Undo>>": self.undo,
+            "<<Redo>>": self.redo,
+            "<<SelectAll>>": self.select_all,
+        }
 
         self.disp_ctrl_outline = {}
         self.disp_text = {}
         self.disp_high = {}
         self.disp_grid = {}
         self.disp_resize_lines = {}
         self.disp_dropdown = {}
@@ -332,14 +349,21 @@
         self.reset_col_positions()
 
         self.rc_popup_menu = None
         self.empty_rc_popup_menu = None
         self.basic_bindings()
         self.create_rc_menus()
 
+    def event_generate(self, *args, **kwargs) -> None:
+        for arg in args:
+            if arg in self.event_linker:
+                self.event_linker[arg]()
+            else:
+                super().event_generate(*args, **kwargs)
+
     def refresh(self, event: object = None) -> None:
         self.main_table_redraw_grid_and_text(True, True)
 
     def window_configured(self, event: object) -> None:
         w = self.PAR.winfo_width()
         if w != self.PAR_width:
             self.PAR_width = w
@@ -355,18 +379,18 @@
             ("<Configure>", self, self.window_configured),
             ("<Motion>", self, self.mouse_motion),
             ("<ButtonPress-1>", self, self.b1_press),
             ("<B1-Motion>", self, self.b1_motion),
             ("<ButtonRelease-1>", self, self.b1_release),
             ("<Double-Button-1>", self, self.double_b1),
             ("<MouseWheel>", self, self.mousewheel),
+            ("<MouseWheel>", self.RI, self.mousewheel),
             ("<Shift-ButtonPress-1>", self, self.shift_b1_press),
             ("<Shift-ButtonPress-1>", self.CH, self.CH.shift_b1_press),
             ("<Shift-ButtonPress-1>", self.RI, self.RI.shift_b1_press),
-            ("<MouseWheel>", self.RI, self.mousewheel),
             (rc_binding, self, self.rc),
             (f"<{ctrl_key}-ButtonPress-1>", self, self.ctrl_b1_press),
             (f"<{ctrl_key}-ButtonPress-1>", self.CH, self.CH.ctrl_b1_press),
             (f"<{ctrl_key}-ButtonPress-1>", self.RI, self.RI.ctrl_b1_press),
             (f"<{ctrl_key}-Shift-ButtonPress-1>", self, self.ctrl_shift_b1_press),
             (f"<{ctrl_key}-Shift-ButtonPress-1>", self.CH, self.CH.ctrl_shift_b1_press),
             (f"<{ctrl_key}-Shift-ButtonPress-1>", self.RI, self.RI.ctrl_shift_b1_press),
@@ -377,39 +401,47 @@
         all_canvas_bindings = (
             ("<Shift-MouseWheel>", self.shift_mousewheel),
             ("<Control-MouseWheel>", self.ctrl_mousewheel),
             ("<Control-plus>", self.zoom_in),
             ("<Control-equal>", self.zoom_in),
             ("<Control-minus>", self.zoom_out),
         )
-        all_canvas_linux_bindings = {
+        mt_ri_canvas_linux_bindings = {
             ("<Button-4>", self.mousewheel),
             ("<Button-5>", self.mousewheel),
+        }
+        all_canvas_linux_bindings = {
             ("<Shift-Button-4>", self.shift_mousewheel),
             ("<Shift-Button-5>", self.shift_mousewheel),
             ("<Control-Button-4>", self.ctrl_mousewheel),
             ("<Control-Button-5>", self.ctrl_mousewheel),
         }
         if enable:
             for b in bindings:
                 b[1].bind(b[0], b[2])
             for b in all_canvas_bindings:
                 for canvas in (self, self.RI, self.CH):
                     canvas.bind(b[0], b[1])
             if USER_OS == "linux":
+                for b in mt_ri_canvas_linux_bindings:
+                    for canvas in (self, self.RI):
+                        canvas.bind(b[0], b[1])
                 for b in all_canvas_linux_bindings:
                     for canvas in (self, self.RI, self.CH):
                         canvas.bind(b[0], b[1])
         else:
             for b in bindings:
                 b[1].unbind(b[0])
             for b in all_canvas_bindings:
                 for canvas in (self, self.RI, self.CH):
                     canvas.unbind(b[0])
             if USER_OS == "linux":
+                for b in mt_ri_canvas_linux_bindings:
+                    for canvas in (self, self.RI):
+                        canvas.unbind(b[0])
                 for b in all_canvas_linux_bindings:
                     for canvas in (self, self.RI, self.CH):
                         canvas.unbind(b[0])
 
     def reset_tags(self) -> None:
         self.tagged_cells = {}
         self.tagged_rows = {}
@@ -487,14 +519,16 @@
             if sh:
                 self.itemconfig(t, state="hidden")
                 self.hidd_ctrl_outline[t] = False
 
     def get_ctrl_x_c_boxes(self) -> tuple[dict[tuple[int, int, int, int], str], int]:
         boxes = {}
         maxrows = 0
+        if not self.selected:
+            return boxes, maxrows
         if self.selected.type_ in ("cells", "columns"):
             curr_box = self.selection_boxes[self.selected.fill_iid].coords
             maxrows = curr_box[2] - curr_box[0]
             for item, box in self.get_selection_items(rows=False):
                 if maxrows >= box.coords[2] - box.coords[0]:
                     boxes[box.coords] = box.type_
         else:
@@ -509,22 +543,23 @@
             dialect=csv.excel_tab,
             delimiter=self.PAR.ops.to_clipboard_delimiter,
             quotechar=self.PAR.ops.to_clipboard_quotechar,
             lineterminator=self.PAR.ops.to_clipboard_lineterminator,
         )
         return s, writer
 
-    def ctrl_c(self, event=None) -> None:
+    def ctrl_c(self, event=None) -> None | EventDataDict:
         if not self.selected:
             return
         event_data = event_dict(
+            name="begin_ctrl_c",
             sheet=self.PAR.name,
+            widget=self,
             selected=self.selected,
         )
-        event_data["eventname"] = "begin_ctrl_c"
         boxes, maxrows = self.get_ctrl_x_c_boxes()
         event_data["selection_boxes"] = boxes
         s, writer = self.io_csv_writer()
         if not try_binding(self.extra_begin_ctrl_c_func, event_data):
             return
         if self.selected.type_ in ("cells", "columns"):
             for rn in range(maxrows):
@@ -547,24 +582,32 @@
                         v = self.get_cell_clipboard(datarn, datacn)
                         event_data["cells"]["table"][(datarn, datacn)] = v
                         row.append(v)
                     writer.writerow(row)
         for r1, c1, r2, c2 in boxes:
             self.show_ctrl_outline(canvas="table", start_cell=(c1, r1), end_cell=(c2, r2))
         self.clipboard_clear()
-        self.clipboard_append(s.getvalue())
+        if len(event_data["cells"]["table"]) == 1 and self.PAR.ops.to_clipboard_lineterminator not in next(
+            iter(event_data["cells"]["table"].values())
+        ):
+            self.clipboard_append(next(iter(event_data["cells"]["table"].values())))
+        else:
+            self.clipboard_append(s.getvalue())
         self.update_idletasks()
-        try_binding(self.extra_end_ctrl_c_func, event_data, "end_ctrl_c")
+        try_binding(self.extra_end_ctrl_c_func, event_data, new_name="end_ctrl_c")
+        self.PAR.emit_event("<<Copy>>", EventDataDict({**event_data, **{"eventname": "copy"}}))
+        return event_data
 
-    def ctrl_x(self, event=None) -> None:
+    def ctrl_x(self, event=None, validation: bool = True) -> None | EventDataDict:
         if not self.selected:
             return
         event_data = event_dict(
             name="edit_table",
             sheet=self.PAR.name,
+            widget=self,
             selected=self.selected,
         )
         boxes, maxrows = self.get_ctrl_x_c_boxes()
         event_data["selection_boxes"] = boxes
         s, writer = self.io_csv_writer()
         if not try_binding(self.extra_begin_ctrl_x_func, event_data, "begin_ctrl_x"):
             return
@@ -575,18 +618,22 @@
                     if r2 - r1 < maxrows:
                         continue
                     datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
                         datacn = self.datacn(c)
                         row.append(self.get_cell_clipboard(datarn, datacn))
                         val = self.get_value_for_empty_cell(datarn, datacn)
-                        if not self.edit_validation_func or (
-                            self.edit_validation_func
-                            and (val := self.edit_validation_func(mod_event_val(event_data, val, (r1 + rn, c))))
-                            is not None
+                        if (
+                            not self.edit_validation_func
+                            or not validation
+                            or (
+                                self.edit_validation_func
+                                and (val := self.edit_validation_func(mod_event_val(event_data, val, (r1 + rn, c))))
+                                is not None
+                            )
                         ):
                             event_data = self.event_data_set_cell(
                                 datarn,
                                 datacn,
                                 val,
                                 event_data,
                             )
@@ -596,113 +643,122 @@
                 for rn in range(r2 - r1):
                     row = []
                     datarn = (r1 + rn) if self.all_rows_displayed else self.displayed_rows[r1 + rn]
                     for c in range(c1, c2):
                         datacn = self.datacn(c)
                         row.append(self.get_cell_clipboard(datarn, datacn))
                         val = self.get_value_for_empty_cell(datarn, datacn)
-                        if not self.edit_validation_func or (
-                            self.edit_validation_func
-                            and (val := self.edit_validation_func(mod_event_val(event_data, val, (r1 + rn, c))))
-                            is not None
+                        if (
+                            not self.edit_validation_func
+                            or not validation
+                            or (
+                                self.edit_validation_func
+                                and (val := self.edit_validation_func(mod_event_val(event_data, val, (r1 + rn, c))))
+                                is not None
+                            )
                         ):
                             event_data = self.event_data_set_cell(
                                 datarn,
                                 datacn,
                                 val,
                                 event_data,
                             )
                     writer.writerow(row)
         if event_data["cells"]["table"]:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.clipboard_clear()
-        self.clipboard_append(s.getvalue())
+        if len(event_data["cells"]["table"]) == 1 and self.PAR.ops.to_clipboard_lineterminator not in next(
+            iter(event_data["cells"]["table"].values())
+        ):
+            self.clipboard_append(next(iter(event_data["cells"]["table"].values())))
+        else:
+            self.clipboard_append(s.getvalue())
         self.update_idletasks()
         self.refresh()
         for r1, c1, r2, c2 in boxes:
             self.show_ctrl_outline(canvas="table", start_cell=(c1, r1), end_cell=(c2, r2))
         if event_data["cells"]["table"]:
             try_binding(self.extra_end_ctrl_x_func, event_data, "end_ctrl_x")
         self.sheet_modified(event_data)
+        self.PAR.emit_event("<<Cut>>", event_data)
+        return event_data
 
-    def ctrl_v(self, event: object = None) -> None:
-        if not self.PAR.ops.expand_sheet_if_paste_too_big and (
-            len(self.col_positions) == 1 or len(self.row_positions) == 1
-        ):
+    def ctrl_v(self, event: object = None, validation: bool = True) -> None | EventDataDict:
+        if not self.PAR.ops.paste_can_expand_x and len(self.col_positions) == 1:
+            return
+        if not self.PAR.ops.paste_can_expand_y and len(self.row_positions) == 1:
             return
         event_data = event_dict(
             name="edit_table",
             sheet=self.PAR.name,
+            widget=self,
             selected=self.selected,
         )
         if self.selected:
             selected_r = self.selected.row
             selected_c = self.selected.column
-        elif not self.selected and not self.PAR.ops.expand_sheet_if_paste_too_big:
+        elif not self.selected and not self.PAR.ops.paste_can_expand_x and not self.PAR.ops.paste_can_expand_y:
             return
         else:
             if not self.data:
                 selected_c, selected_r = 0, 0
             else:
                 if len(self.col_positions) == 1 and len(self.row_positions) > 1:
                     selected_c, selected_r = 0, len(self.row_positions) - 1
                 elif len(self.row_positions) == 1 and len(self.col_positions) > 1:
                     selected_c, selected_r = len(self.col_positions) - 1, 0
                 elif len(self.row_positions) > 1 and len(self.col_positions) > 1:
                     selected_c, selected_r = 0, len(self.row_positions) - 1
         try:
-            data = self.clipboard_get()
-        except Exception:
-            return
-        try:
-            dialect = csv.Sniffer().sniff(data, delimiters=self.PAR.ops.from_clipboard_delimiters)
+            data = get_data_from_clipboard(
+                widget=self,
+                delimiters=self.PAR.ops.from_clipboard_delimiters,
+                lineterminator=self.PAR.ops.to_clipboard_lineterminator,
+            )
         except Exception:
-            dialect = csv.excel_tab
-        data = list(csv.reader(io.StringIO(data), dialect=dialect, skipinitialspace=True))
-        if not data:
             return
         new_data_numcols = max(map(len, data))
         new_data_numrows = len(data)
         for rn, r in enumerate(data):
             if len(r) < new_data_numcols:
                 data[rn] += list(repeat("", new_data_numcols - len(r)))
-        (
-            lastbox_r1,
-            lastbox_c1,
-            lastbox_r2,
-            lastbox_c2,
-        ) = self.selection_boxes[self.selected.fill_iid].coords
-        lastbox_numrows = lastbox_r2 - lastbox_r1
-        lastbox_numcols = lastbox_c2 - lastbox_c1
-        if lastbox_numrows > new_data_numrows and not lastbox_numrows % new_data_numrows:
-            nd = []
-            for _ in range(int(lastbox_numrows / new_data_numrows)):
-                nd.extend(r.copy() for r in data)
-            data.extend(nd)
-            new_data_numrows *= int(lastbox_numrows / new_data_numrows)
-
-        if lastbox_numcols > new_data_numcols and not lastbox_numcols % new_data_numcols:
-            for rn, r in enumerate(data):
-                for _ in range(int(lastbox_numcols / new_data_numcols)):
-                    data[rn].extend(r.copy())
-            new_data_numcols *= int(lastbox_numcols / new_data_numcols)
+        if self.selected:
+            (
+                lastbox_r1,
+                lastbox_c1,
+                lastbox_r2,
+                lastbox_c2,
+            ) = self.selection_boxes[self.selected.fill_iid].coords
+            lastbox_numrows = lastbox_r2 - lastbox_r1
+            lastbox_numcols = lastbox_c2 - lastbox_c1
+            if lastbox_numrows > new_data_numrows and not lastbox_numrows % new_data_numrows:
+                nd = []
+                for _ in range(int(lastbox_numrows / new_data_numrows)):
+                    nd.extend(r.copy() for r in data)
+                data.extend(nd)
+                new_data_numrows *= int(lastbox_numrows / new_data_numrows)
+            if lastbox_numcols > new_data_numcols and not lastbox_numcols % new_data_numcols:
+                for rn, r in enumerate(data):
+                    for _ in range(int(lastbox_numcols / new_data_numcols)):
+                        data[rn].extend(r.copy())
+                new_data_numcols *= int(lastbox_numcols / new_data_numcols)
         event_data["data"] = data
         added_rows = 0
         added_cols = 0
         total_data_cols = None
-        if self.PAR.ops.expand_sheet_if_paste_too_big:
-            # determine number of columns and/or rows to add to sheet
+        if self.PAR.ops.paste_can_expand_x:
             if selected_c + new_data_numcols > len(self.col_positions) - 1:
                 total_data_cols = self.equalize_data_row_lengths()
                 added_cols = selected_c + new_data_numcols - len(self.col_positions) + 1
                 if (
                     isinstance(self.PAR.ops.paste_insert_column_limit, int)
                     and self.PAR.ops.paste_insert_column_limit < len(self.col_positions) - 1 + added_cols
                 ):
                     added_cols = self.PAR.ops.paste_insert_column_limit - len(self.col_positions) - 1
+        if self.PAR.ops.paste_can_expand_y:
             if selected_r + new_data_numrows > len(self.row_positions) - 1:
                 added_rows = selected_r + new_data_numrows - len(self.row_positions) + 1
                 if (
                     isinstance(self.PAR.ops.paste_insert_row_limit, int)
                     and self.PAR.ops.paste_insert_row_limit < len(self.row_positions) - 1 + added_rows
                 ):
                     added_rows = self.PAR.ops.paste_insert_row_limit - len(self.row_positions) - 1
@@ -712,14 +768,15 @@
             adjusted_new_data_numcols = new_data_numcols
         if selected_r + new_data_numrows > len(self.row_positions) - 1:
             adjusted_new_data_numrows = len(self.row_positions) - 1 - selected_r
         else:
             adjusted_new_data_numrows = new_data_numrows
         selected_r_adjusted_new_data_numrows = selected_r + adjusted_new_data_numrows
         selected_c_adjusted_new_data_numcols = selected_c + adjusted_new_data_numcols
+        endrow = selected_r_adjusted_new_data_numrows
         boxes = {
             (
                 selected_r,
                 selected_c,
                 selected_r_adjusted_new_data_numrows,
                 selected_c_adjusted_new_data_numcols,
             ): "cells"
@@ -733,34 +790,39 @@
         # then if there are any added rows/columns:
         # create empty rows/columns dicts for any added rows/columns
         # edit those dicts with so far unused cells of data from clipboard
         # instead of editing table using set cell data, add any new rows then columns with pasted data
         for ndr, r in enumerate(range(selected_r, selected_r_adjusted_new_data_numrows)):
             for ndc, c in enumerate(range(selected_c, selected_c_adjusted_new_data_numcols)):
                 val = data[ndr][ndc]
-                if not self.edit_validation_func or (
-                    self.edit_validation_func
-                    and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                if (
+                    not self.edit_validation_func
+                    or not validation
+                    or (
+                        self.edit_validation_func
+                        and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                    )
                 ):
                     event_data = self.event_data_set_cell(
                         datarn=self.datarn(r),
                         datacn=self.datacn(c),
                         value=val,
                         event_data=event_data,
                     )
-        if added_rows > 0:
+        if added_rows:
             ctr = 0
             data_ins_row = len(self.data)
             displayed_ins_row = len(self.row_positions) - 1
             if total_data_cols is None:
                 total_data_cols = self.total_data_cols()
             rows, index, row_heights = self.get_args_for_add_rows(
                 data_ins_row=data_ins_row,
                 displayed_ins_row=displayed_ins_row,
                 numrows=added_rows,
+                total_data_cols=total_data_cols,
             )
             for ndr, r in zip(
                 range(
                     adjusted_new_data_numrows,
                     new_data_numrows,
                 ),
                 reversed(rows),
@@ -769,74 +831,97 @@
                     range(
                         selected_c,
                         selected_c_adjusted_new_data_numcols,
                     )
                 ):
                     val = data[ndr][ndc]
                     datacn = self.datacn(c)
-                    if not self.edit_validation_func or (
-                        self.edit_validation_func
-                        and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
-                        and self.input_valid_for_cell(r, datacn, val, ignore_empty=True)
+                    if (
+                        not self.edit_validation_func
+                        or not validation
+                        or (
+                            self.edit_validation_func
+                            and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                            and self.input_valid_for_cell(r, datacn, val, ignore_empty=True)
+                        )
                     ):
                         rows[r][datacn] = val
                         ctr += 1
             if ctr:
                 event_data = self.add_rows(
                     rows=rows,
                     index=index,
                     row_heights=row_heights,
                     event_data=event_data,
                 )
-        if added_cols > 0:
+        if added_cols:
             ctr = 0
+            if total_data_cols is None:
+                total_data_cols = self.total_data_cols()
             data_ins_col = total_data_cols
             displayed_ins_col = len(self.col_positions) - 1
             columns, headers, column_widths = self.get_args_for_add_columns(
                 data_ins_col=data_ins_col,
                 displayed_ins_col=displayed_ins_col,
                 numcols=added_cols,
             )
+            # only add the extra rows if expand_y is allowed
+            if self.PAR.ops.paste_can_expand_x and self.PAR.ops.paste_can_expand_y:
+                endrow = selected_r + new_data_numrows
+            else:
+                endrow = selected_r + adjusted_new_data_numrows
             for ndr, r in enumerate(
                 range(
                     selected_r,
-                    selected_r + new_data_numrows,
+                    endrow,
                 )
             ):
                 for ndc, c in zip(
                     range(
                         adjusted_new_data_numcols,
                         new_data_numcols,
                     ),
                     reversed(columns),
                 ):
                     val = data[ndr][ndc]
                     datarn = self.datarn(r)
-                    if not self.edit_validation_func or (
-                        self.edit_validation_func
-                        and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
-                        and self.input_valid_for_cell(datarn, c, val, ignore_empty=True)
+                    if (
+                        not self.edit_validation_func
+                        or not validation
+                        or (
+                            self.edit_validation_func
+                            and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                            and self.input_valid_for_cell(datarn, c, val, ignore_empty=True)
+                        )
                     ):
                         columns[c][datarn] = val
                         ctr += 1
             if ctr:
                 event_data = self.add_columns(
                     columns=columns,
                     header=headers,
                     column_widths=column_widths,
                     event_data=event_data,
                 )
         self.deselect("all", redraw=False)
         if event_data["cells"]["table"] or event_data["added"]["rows"] or event_data["added"]["columns"]:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
+        if added_rows:
+            selboxr = selected_r + new_data_numrows
+        else:
+            selboxr = selected_r_adjusted_new_data_numrows
+        if added_cols:
+            selboxc = selected_c + new_data_numcols
+        else:
+            selboxc = selected_c_adjusted_new_data_numcols
         self.create_selection_box(
             selected_r,
             selected_c,
-            selected_r_adjusted_new_data_numrows,
-            selected_c_adjusted_new_data_numcols,
+            selboxr,
+            selboxc,
             "cells",
             run_binding=True,
         )
         self.see(
             r=selected_r,
             c=selected_c,
             keep_yscroll=False,
@@ -845,47 +930,56 @@
             check_cell_visibility=True,
             redraw=False,
         )
         self.refresh()
         if event_data["cells"]["table"] or event_data["added"]["rows"] or event_data["added"]["columns"]:
             try_binding(self.extra_end_ctrl_v_func, event_data, "end_ctrl_v")
         self.sheet_modified(event_data)
+        self.PAR.emit_event("<<Paste>>", event_data)
+        return event_data
 
-    def delete_key(self, event: object = None) -> None:
+    def delete_key(self, event: object = None, validation: bool = True) -> None | EventDataDict:
         if not self.selected:
             return
         event_data = event_dict(
             name="edit_table",
             sheet=self.PAR.name,
+            widget=self,
             selected=self.selected,
         )
         boxes = self.get_boxes()
         event_data["selection_boxes"] = boxes
         if not try_binding(self.extra_begin_delete_key_func, event_data, "begin_delete"):
             return
         for r1, c1, r2, c2 in boxes:
             for r in range(r1, r2):
                 for c in range(c1, c2):
                     datarn, datacn = self.datarn(r), self.datacn(c)
                     val = self.get_value_for_empty_cell(datarn, datacn)
-                    if not self.edit_validation_func or (
-                        self.edit_validation_func
-                        and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                    if (
+                        not self.edit_validation_func
+                        or not validation
+                        or (
+                            self.edit_validation_func
+                            and (val := self.edit_validation_func(mod_event_val(event_data, val, (r, c)))) is not None
+                        )
                     ):
                         event_data = self.event_data_set_cell(
                             datarn,
                             datacn,
                             val,
                             event_data,
                         )
         if event_data["cells"]["table"]:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
             try_binding(self.extra_end_delete_key_func, event_data, "end_delete")
         self.refresh()
         self.sheet_modified(event_data)
+        self.PAR.emit_event("<<Delete>>", event_data)
+        return event_data
 
     def event_data_set_cell(self, datarn: int, datacn: int, value: object, event_data: dict) -> EventDataDict:
         if self.input_valid_for_cell(datarn, datacn, value):
             event_data["cells"]["table"][(datarn, datacn)] = self.get_cell_data(datarn, datacn)
             self.set_cell_data(datarn, datacn, value)
         return event_data
 
@@ -904,54 +998,63 @@
         else:
             disp_new_idxs = {}
         totalcols = self.equalize_data_row_lengths(at_least_cols=move_to + 1)
         if self.all_columns_displayed or data_indexes:
             data_new_idxs = get_new_indexes(seqlen=totalcols, move_to=move_to, to_move=to_move)
         elif not self.all_columns_displayed and not data_indexes:
             data_new_idxs = get_new_indexes(seqlen=len(self.displayed_columns), move_to=move_to, to_move=to_move)
-            data_old_idxs = dict(zip(data_new_idxs.values(), data_new_idxs))
+            moved = {self.displayed_columns[i] for i in to_move}
             data_new_idxs = dict(
-                zip(
-                    move_elements_by_mapping(self.displayed_columns, data_new_idxs, data_old_idxs),
-                    self.displayed_columns,
+                filter(
+                    lambda tup: tup[0] in moved,
+                    zip(
+                        move_elements_by_mapping(
+                            self.displayed_columns,
+                            data_new_idxs,
+                            dict(zip(data_new_idxs.values(), data_new_idxs)),
+                        ),
+                        self.displayed_columns,
+                    ),
                 )
             )
         return data_new_idxs, dict(zip(data_new_idxs.values(), data_new_idxs)), totalcols, disp_new_idxs
 
     def move_columns_adjust_options_dict(
         self,
         data_new_idxs: dict[int, int],
         data_old_idxs: dict[int, int],
         totalcols: int | None,
         disp_new_idxs: None | dict[int, int] = None,
         move_data: bool = True,
+        move_widths: bool = True,
         create_selections: bool = True,
         data_indexes: bool = False,
         event_data: EventDataDict | None = None,
     ) -> tuple[dict[int, int], dict[int, int], EventDataDict]:
         self.saved_column_widths = {}
         if not isinstance(totalcols, int):
             totalcols = max(data_new_idxs.values(), default=0)
             if totalcols:
                 totalcols += 1
             totalcols = self.equalize_data_row_lengths(at_least_cols=totalcols)
         if event_data is None:
             event_data = event_dict(
                 name="move_columns",
                 sheet=self.PAR.name,
+                widget=self,
                 boxes=self.get_boxes(),
                 selected=self.selected,
             )
             event_data["moved"]["columns"] = {
                 "data": data_new_idxs,
                 "displayed": {} if disp_new_idxs is None else disp_new_idxs,
             }
         event_data["options"] = self.pickle_options()
         event_data["named_spans"] = {k: span.pickle_self() for k, span in self.named_spans.items()}
-        if disp_new_idxs and (not data_indexes or self.all_columns_displayed):
+        if move_widths and disp_new_idxs and (not data_indexes or self.all_columns_displayed):
             self.deselect("all", run_binding=False, redraw=False)
             self.set_col_positions(
                 itr=move_elements_by_mapping(
                     self.get_column_widths(),
                     disp_new_idxs,
                     dict(
                         zip(
@@ -1135,56 +1238,65 @@
             self.total_data_rows(),
             len(self.row_positions) - 1,
         )
         if self.all_rows_displayed or data_indexes:
             data_new_idxs = get_new_indexes(seqlen=totalrows, move_to=move_to, to_move=to_move)
         elif not self.all_rows_displayed and not data_indexes:
             data_new_idxs = get_new_indexes(seqlen=len(self.displayed_rows), move_to=move_to, to_move=to_move)
-            data_old_idxs = dict(zip(data_new_idxs.values(), data_new_idxs))
+            moved = {self.displayed_rows[i] for i in to_move}
             data_new_idxs = dict(
-                zip(
-                    move_elements_by_mapping(self.displayed_rows, data_new_idxs, data_old_idxs),
-                    self.displayed_rows,
+                filter(
+                    lambda tup: tup[0] in moved,
+                    zip(
+                        move_elements_by_mapping(
+                            self.displayed_rows,
+                            data_new_idxs,
+                            dict(zip(data_new_idxs.values(), data_new_idxs)),
+                        ),
+                        self.displayed_rows,
+                    ),
                 )
             )
         return data_new_idxs, dict(zip(data_new_idxs.values(), data_new_idxs)), totalrows, disp_new_idxs
 
     def move_rows_adjust_options_dict(
         self,
         data_new_idxs: dict[int, int],
         data_old_idxs: dict[int, int],
         totalrows: int | None,
         disp_new_idxs: None | dict[int, int] = None,
         move_data: bool = True,
+        move_heights: bool = True,
         create_selections: bool = True,
         data_indexes: bool = False,
         event_data: EventDataDict | None = None,
     ) -> tuple[dict[int, int], dict[int, int], EventDataDict]:
         self.saved_row_heights = {}
         if not isinstance(totalrows, int):
             totalrows = max(
                 self.total_data_rows(),
                 len(self.row_positions) - 1,
                 max(data_new_idxs.values(), default=0),
             )
-            totalrows = self.fix_data_len(totalrows)
+            self.fix_data_len(totalrows)
         if event_data is None:
             event_data = event_dict(
                 name="move_rows",
                 sheet=self.PAR.name,
+                widget=self,
                 boxes=self.get_boxes(),
                 selected=self.selected,
             )
             event_data["moved"]["rows"] = {
                 "data": data_new_idxs,
                 "displayed": {} if disp_new_idxs is None else disp_new_idxs,
             }
         event_data["options"] = self.pickle_options()
         event_data["named_spans"] = {k: span.pickle_self() for k, span in self.named_spans.items()}
-        if disp_new_idxs and (not data_indexes or self.all_rows_displayed):
+        if move_heights and disp_new_idxs and (not data_indexes or self.all_rows_displayed):
             self.deselect("all", run_binding=False, redraw=False)
             self.set_row_positions(
                 itr=move_elements_by_mapping(
                     self.get_row_heights(),
                     disp_new_idxs,
                     dict(
                         zip(
@@ -1354,47 +1466,48 @@
         # return a dict of all row or column indexes
         # old indexes and new indexes, not just the
         # ones that were moved e.g.
         # {old index: new index, ...}
         # all the way from 0 to max_idx
         if old_idxs is None:
             old_idxs = dict(zip(new_idxs.values(), new_idxs))
-        seq = tuple(range(max_idx + 1))
         return dict(
             zip(
-                move_elements_by_mapping(seq, new_idxs, old_idxs),
-                seq,
+                move_elements_by_mapping(tuple(range(max_idx + 1)), new_idxs, old_idxs),
+                range(max_idx + 1),
             )
         )
 
-    def undo(self, event: object = None) -> None:
+    def undo(self, event: object = None) -> None | EventDataDict:
         if not self.undo_stack:
             return
-        if isinstance(self.undo_stack[-1]["data"], dict):
-            modification = self.undo_stack[-1]["data"]
-        else:
-            modification = decompress_load(self.undo_stack[-1]["data"])
+        modification = decompress_load(self.undo_stack[-1]["data"])
         if not try_binding(self.extra_begin_ctrl_z_func, modification, "begin_undo"):
             return
-        self.redo_stack.append(self.undo_modification_invert_event(modification))
+        event_data = self.undo_modification_invert_event(modification)
+        self.redo_stack.append(pickled_event_dict(event_data))
         self.undo_stack.pop()
-        try_binding(self.extra_end_ctrl_z_func, modification, "end_undo")
+        self.sheet_modified(event_data, purge_redo=False)
+        try_binding(self.extra_end_ctrl_z_func, event_data, "end_undo")
+        self.PAR.emit_event("<<Undo>>", event_data)
+        return event_data
 
-    def redo(self, event: object = None) -> None:
+    def redo(self, event: object = None) -> None | EventDataDict:
         if not self.redo_stack:
             return
-        if isinstance(self.redo_stack[-1]["data"], dict):
-            modification = self.redo_stack[-1]["data"]
-        else:
-            modification = decompress_load(self.redo_stack[-1]["data"])
+        modification = decompress_load(self.redo_stack[-1]["data"])
         if not try_binding(self.extra_begin_ctrl_z_func, modification, "begin_redo"):
             return
-        self.undo_stack.append(self.undo_modification_invert_event(modification, name="redo"))
+        event_data = self.undo_modification_invert_event(modification, name="redo")
+        self.undo_stack.append(pickled_event_dict(event_data))
         self.redo_stack.pop()
-        try_binding(self.extra_end_ctrl_z_func, modification, "end_redo")
+        self.sheet_modified(event_data, purge_redo=False)
+        try_binding(self.extra_end_ctrl_z_func, event_data, "end_redo")
+        self.PAR.emit_event("<<Redo>>", event_data)
+        return event_data
 
     def sheet_modified(self, event_data: EventDataDict, purge_redo: bool = True) -> None:
         self.PAR.emit_event("<<SheetModified>>", event_data)
         if purge_redo:
             self.purge_redo_stack()
 
     def edit_cells_using_modification(self, modification: dict, event_data: dict) -> EventDataDict:
@@ -1434,19 +1547,20 @@
             self.tagged_rows = modification["options"]["tagged_rows"]
         if "tagged_columns" in modification["options"]:
             self.tagged_columns = modification["options"]["tagged_columns"]
         self.named_spans = {
             k: mod_span_widget(unpickle_obj(v), self.PAR) for k, v in modification["named_spans"].items()
         }
 
-    def undo_modification_invert_event(self, modification: EventDataDict, name: str = "undo") -> bytes | EventDataDict:
+    def undo_modification_invert_event(self, modification: EventDataDict, name: str = "undo") -> EventDataDict:
         self.deselect("all", redraw=False)
         event_data = event_dict(
             name=modification["eventname"],
             sheet=self.PAR.name,
+            widget=self,
         )
         event_data["selection_boxes"] = modification["selection_boxes"]
         event_data["selected"] = modification["selected"]
         saved_cells = False
 
         if modification["added"]["rows"] or modification["added"]["columns"]:
             event_data = self.save_cells_using_modification(modification, event_data)
@@ -1597,17 +1711,16 @@
                 keep_yscroll=False,
                 keep_xscroll=False,
                 bottom_right_corner=False,
                 check_cell_visibility=True,
                 redraw=False,
             )
 
-        self.sheet_modified(event_data, purge_redo=False)
         self.refresh()
-        return ev_stack_dict(event_data)
+        return event_data
 
     def see(
         self,
         r: int | None = None,
         c: int | None = None,
         keep_yscroll: bool = False,
         keep_xscroll: bool = False,
@@ -1724,15 +1837,17 @@
             if redraw:
                 self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             if run_binding_func:
                 if self.select_all_binding_func:
                     self.select_all_binding_func(
                         self.get_select_event(being_drawn_item=self.being_drawn_item),
                     )
-                self.PAR.emit_event("<<SheetSelect>>", data=self.get_select_event(self.being_drawn_item))
+                event_data = self.get_select_event(self.being_drawn_item)
+                self.PAR.emit_event("<<SheetSelect>>", data=event_data)
+                self.PAR.emit_event("<<SelectAll>>", data=event_data)
 
     def select_cell(
         self,
         r: int,
         c: int,
         redraw: bool = False,
         run_binding_func: bool = True,
@@ -2199,106 +2314,14 @@
                         r,
                         c + 1,
                         keep_yscroll=True,
                         bottom_right_corner=False if self.PAR.ops.arrow_key_down_right_scroll_page else True,
                         check_cell_visibility=False,
                     )
 
-    def key_bindings(self) -> None:
-        for widget in (self, self.RI, self.CH, self.TL):
-            for binding in self.PAR.ops.copy_bindings:
-                if self.copy_enabled:
-                    widget.bind(binding, self.ctrl_c)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.cut_bindings:
-                if self.cut_enabled:
-                    widget.bind(binding, self.ctrl_x)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.paste_bindings:
-                if self.paste_enabled:
-                    widget.bind(binding, self.ctrl_v)
-                else:
-                    widget.unbind(binding)
-
-            if self.undo_enabled:
-                for binding in self.PAR.ops.undo_bindings:
-                    widget.bind(binding, self.undo)
-                for binding in self.PAR.ops.redo_bindings:
-                    widget.bind(binding, self.redo)
-            else:
-                for binding in self.PAR.ops.undo_bindings:
-                    widget.unbind(binding)
-                for binding in self.PAR.ops.redo_bindings:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.delete_bindings:
-                if self.delete_key_enabled:
-                    widget.bind(binding, self.delete_key)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.select_all_bindings:
-                if self.select_all_enabled:
-                    widget.bind(binding, self.select_all)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.tab_bindings:
-                if self.tab_enabled:
-                    widget.bind(binding, self.tab_key)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.up_bindings:
-                if self.up_enabled:
-                    widget.bind(binding, self.arrowkey_UP)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.right_bindings:
-                if self.right_enabled:
-                    widget.bind(binding, self.arrowkey_RIGHT)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.down_bindings:
-                if self.down_enabled:
-                    widget.bind(binding, self.arrowkey_DOWN)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.left_bindings:
-                if self.left_enabled:
-                    widget.bind(binding, self.arrowkey_LEFT)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.prior_bindings:
-                if self.prior_enabled:
-                    widget.bind(binding, self.page_UP)
-                else:
-                    widget.unbind(binding)
-
-            for binding in self.PAR.ops.next_bindings:
-                if self.next_enabled:
-                    widget.bind(binding, self.page_DOWN)
-                else:
-                    widget.unbind(binding)
-
-        if self.edit_cell_enabled:
-            for w in (self, self.RI, self.CH):
-                w.bind("<Key>", self.open_cell)
-        else:
-            for w in (self, self.RI, self.CH):
-                w.unbind("<Key>")
-
     def menu_add_command(self, menu: tk.Menu, **kwargs) -> None:
         if "label" not in kwargs:
             return
         try:
             index = menu.index(kwargs["label"])
             menu.delete(index)
         except TclError:
@@ -2411,15 +2434,15 @@
             self.menu_add_command(
                 self.RI.ri_rc_popup_menu,
                 label=self.PAR.ops.paste_label,
                 accelerator=self.PAR.ops.paste_accelerator,
                 command=self.ctrl_v,
                 **mnkwgs,
             )
-            if self.PAR.ops.expand_sheet_if_paste_too_big:
+            if self.PAR.ops.paste_can_expand_x or self.PAR.ops.paste_can_expand_y:
                 self.menu_add_command(
                     self.empty_rc_popup_menu,
                     label=self.PAR.ops.paste_label,
                     accelerator=self.PAR.ops.paste_accelerator,
                     command=self.ctrl_v,
                     **mnkwgs,
                 )
@@ -2524,56 +2547,51 @@
                 label=label,
                 command=func,
                 **mnkwgs,
             )
 
     def enable_bindings(self, bindings):
         if not bindings:
-            self.enable_bindings_internal("all")
+            self._enable_binding("all")
         elif isinstance(bindings, (list, tuple)):
             for binding in bindings:
                 if isinstance(binding, (list, tuple)):
                     for bind in binding:
-                        self.enable_bindings_internal(bind.lower())
+                        self._enable_binding(bind.lower())
                 elif isinstance(binding, str):
-                    self.enable_bindings_internal(binding.lower())
+                    self._enable_binding(binding.lower())
         elif isinstance(bindings, str):
-            self.enable_bindings_internal(bindings.lower())
+            self._enable_binding(bindings.lower())
         self.create_rc_menus()
-        self.key_bindings()
 
     def disable_bindings(self, bindings):
         if not bindings:
-            self.disable_bindings_internal("all")
+            self._disable_binding("all")
         elif isinstance(bindings, (list, tuple)):
             for binding in bindings:
                 if isinstance(binding, (list, tuple)):
                     for bind in binding:
-                        self.disable_bindings_internal(bind.lower())
+                        self._disable_binding(bind.lower())
                 elif isinstance(binding, str):
-                    self.disable_bindings_internal(binding.lower())
+                    self._disable_binding(binding.lower())
         elif isinstance(bindings, str):
-            self.disable_bindings_internal(bindings)
+            self._disable_binding(bindings)
         self.create_rc_menus()
-        self.key_bindings()
 
-    def enable_bindings_internal(self, binding):
+    def _enable_binding(self, binding):
         if binding == "enable_all":
             binding = "all"
         if binding in ("all", "single", "single_selection_mode", "single_select"):
             self.single_selection_enabled = True
             self.toggle_selection_enabled = False
         elif binding in ("toggle", "toggle_selection_mode", "toggle_select"):
             self.toggle_selection_enabled = True
             self.single_selection_enabled = False
         if binding in ("all", "drag_select"):
             self.drag_selection_enabled = True
-        if binding in ("all", "select_all"):
-            self.select_all_enabled = True
-            self.TL.sa_state()
         if binding in ("all", "column_width_resize"):
             self.CH.width_resizing_enabled = True
         if binding in ("all", "column_select"):
             self.CH.col_selection_enabled = True
         if binding in ("all", "column_height_resize"):
             self.CH.height_resizing_enabled = True
             self.TL.rh_state()
@@ -2588,83 +2606,104 @@
         if binding in ("all", "row_width_resize"):
             self.RI.width_resizing_enabled = True
             self.TL.rw_state()
         if binding in ("all", "row_select"):
             self.RI.row_selection_enabled = True
         if binding in ("all", "row_drag_and_drop", "move_rows"):
             self.RI.drag_and_drop_enabled = True
+        if binding in ("all", "select_all"):
+            self.select_all_enabled = True
+            self.TL.sa_state()
+            self._tksheet_bind("select_all_bindings", self.select_all)
         if binding in ("all", "arrowkeys", "tab"):
             self.tab_enabled = True
+            self._tksheet_bind("tab_bindings", self.tab_key)
         if binding in ("all", "arrowkeys", "up"):
             self.up_enabled = True
+            self._tksheet_bind("up_bindings", self.arrowkey_UP)
         if binding in ("all", "arrowkeys", "right"):
             self.right_enabled = True
+            self._tksheet_bind("right_bindings", self.arrowkey_RIGHT)
         if binding in ("all", "arrowkeys", "down"):
             self.down_enabled = True
+            self._tksheet_bind("down_bindings", self.arrowkey_DOWN)
         if binding in ("all", "arrowkeys", "left"):
             self.left_enabled = True
+            self._tksheet_bind("left_bindings", self.arrowkey_LEFT)
         if binding in ("all", "arrowkeys", "prior"):
             self.prior_enabled = True
+            self._tksheet_bind("prior_bindings", self.page_UP)
         if binding in ("all", "arrowkeys", "next"):
             self.next_enabled = True
-        if binding in ("all", "rc_delete_column"):
+            self._tksheet_bind("next_bindings", self.page_DOWN)
+        if binding in ("all", "copy", "edit_bindings", "edit"):
+            self.copy_enabled = True
+            self._tksheet_bind("copy_bindings", self.ctrl_c)
+        if binding in ("all", "cut", "edit_bindings", "edit"):
+            self.cut_enabled = True
+            self._tksheet_bind("cut_bindings", self.ctrl_x)
+        if binding in ("all", "paste", "edit_bindings", "edit"):
+            self.paste_enabled = True
+            self._tksheet_bind("paste_bindings", self.ctrl_v)
+        if binding in ("all", "delete", "edit_bindings", "edit"):
+            self.delete_key_enabled = True
+            self._tksheet_bind("delete_bindings", self.delete_key)
+        if binding in ("all", "undo", "redo", "edit_bindings", "edit"):
+            self.undo_enabled = True
+            self._tksheet_bind("undo_bindings", self.undo)
+            self._tksheet_bind("redo_bindings", self.redo)
+        if binding in bind_del_columns:
             self.rc_delete_column_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
-        if binding in ("all", "rc_delete_row"):
+        if binding in bind_del_rows:
             self.rc_delete_row_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
-        if binding in ("all", "rc_insert_column"):
+        if binding in bind_add_columns:
             self.rc_insert_column_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
-        if binding in ("all", "rc_insert_row"):
+        if binding in bind_add_rows:
             self.rc_insert_row_enabled = True
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
-        if binding in ("all", "copy", "edit_bindings"):
-            self.copy_enabled = True
-        if binding in ("all", "cut", "edit_bindings"):
-            self.cut_enabled = True
-        if binding in ("all", "paste", "edit_bindings"):
-            self.paste_enabled = True
-        if binding in ("all", "delete", "edit_bindings"):
-            self.delete_key_enabled = True
         if binding in ("all", "right_click_popup_menu", "rc_popup_menu"):
             self.rc_popup_menus_enabled = True
             self.rc_select_enabled = True
         if binding in ("all", "right_click_select", "rc_select"):
             self.rc_select_enabled = True
-        if binding in ("all", "undo", "edit_bindings"):
-            self.undo_enabled = True
-        if binding in ("all", "edit_cell", "edit_bindings"):
+        if binding in ("all", "edit_cell", "edit_bindings", "edit"):
             self.edit_cell_enabled = True
+            for w in (self, self.RI, self.CH):
+                w.bind("<Key>", self.open_cell)
         if binding in ("edit_header"):
             self.CH.edit_cell_enabled = True
         if binding in ("edit_index"):
             self.RI.edit_cell_enabled = True
         # has to be specifically enabled
         if binding in ("ctrl_click_select", "ctrl_select"):
             self.ctrl_select_enabled = True
 
-    def disable_bindings_internal(self, binding):
+    def _tksheet_bind(self, bindings_key: str, func: Callable) -> None:
+        for widget in (self, self.RI, self.CH, self.TL):
+            for binding in self.PAR.ops[bindings_key]:
+                widget.bind(binding, func)
+
+    def _disable_binding(self, binding):
         if binding == "disable_all":
             binding = "all"
         if binding in ("all", "single", "single_selection_mode", "single_select"):
             self.single_selection_enabled = False
             self.toggle_selection_enabled = False
         elif binding in ("toggle", "toggle_selection_mode", "toggle_select"):
             self.toggle_selection_enabled = False
             self.single_selection_enabled = False
         if binding in ("all", "drag_select"):
             self.drag_selection_enabled = False
-        if binding in ("all", "select_all"):
-            self.select_all_enabled = False
-            self.TL.sa_state("hidden")
         if binding in ("all", "column_width_resize"):
             self.CH.width_resizing_enabled = False
         if binding in ("all", "column_select"):
             self.CH.col_selection_enabled = False
         if binding in ("all", "column_height_resize"):
             self.CH.height_resizing_enabled = False
             self.TL.rh_state("hidden")
@@ -2679,67 +2718,82 @@
         if binding in ("all", "row_width_resize"):
             self.RI.width_resizing_enabled = False
             self.TL.rw_state("hidden")
         if binding in ("all", "row_select"):
             self.RI.row_selection_enabled = False
         if binding in ("all", "row_drag_and_drop", "move_rows"):
             self.RI.drag_and_drop_enabled = False
+        if binding in bind_del_columns:
+            self.rc_delete_column_enabled = False
+        if binding in bind_del_rows:
+            self.rc_delete_row_enabled = False
+        if binding in bind_add_columns:
+            self.rc_insert_column_enabled = False
+        if binding in bind_add_rows:
+            self.rc_insert_row_enabled = False
+        if binding in ("all", "right_click_popup_menu", "rc_popup_menu"):
+            self.rc_popup_menus_enabled = False
+        if binding in ("all", "right_click_select", "rc_select"):
+            self.rc_select_enabled = False
+        if binding in ("all", "edit_cell", "edit_bindings", "edit"):
+            self.edit_cell_enabled = False
+            for w in (self, self.RI, self.CH):
+                w.unbind("<Key>")
+        if binding in ("all", "edit_header", "edit_bindings", "edit"):
+            self.CH.edit_cell_enabled = False
+        if binding in ("all", "edit_index", "edit_bindings", "edit"):
+            self.RI.edit_cell_enabled = False
+        if binding in ("all", "ctrl_click_select", "ctrl_select"):
+            self.ctrl_select_enabled = False
+        if binding in ("all", "select_all"):
+            self.select_all_enabled = False
+            self.TL.sa_state("hidden")
+            self._tksheet_unbind("select_all_bindings")
+        if binding in ("all", "copy", "edit_bindings", "edit"):
+            self.copy_enabled = False
+            self._tksheet_unbind("copy_bindings")
+        if binding in ("all", "cut", "edit_bindings", "edit"):
+            self.cut_enabled = False
+            self._tksheet_unbind("cut_bindings")
+        if binding in ("all", "paste", "edit_bindings", "edit"):
+            self.paste_enabled = False
+            self._tksheet_unbind("paste_bindings")
+        if binding in ("all", "delete", "edit_bindings", "edit"):
+            self.delete_key_enabled = False
+            self._tksheet_unbind("delete_bindings")
         if binding in ("all", "arrowkeys", "tab"):
             self.tab_enabled = False
+            self._tksheet_unbind("tab_bindings")
         if binding in ("all", "arrowkeys", "up"):
             self.up_enabled = False
+            self._tksheet_unbind("up_bindings")
         if binding in ("all", "arrowkeys", "right"):
             self.right_enabled = False
+            self._tksheet_unbind("right_bindings")
         if binding in ("all", "arrowkeys", "down"):
             self.down_enabled = False
+            self._tksheet_unbind("down_bindings")
         if binding in ("all", "arrowkeys", "left"):
             self.left_enabled = False
+            self._tksheet_unbind("left_bindings")
         if binding in ("all", "arrowkeys", "prior"):
             self.prior_enabled = False
+            self._tksheet_unbind("prior_bindings")
         if binding in ("all", "arrowkeys", "next"):
             self.next_enabled = False
-        if binding in ("all", "rc_delete_column"):
-            self.rc_delete_column_enabled = False
-            self.rc_popup_menus_enabled = False
-            self.rc_select_enabled = False
-        if binding in ("all", "rc_delete_row"):
-            self.rc_delete_row_enabled = False
-            self.rc_popup_menus_enabled = False
-            self.rc_select_enabled = False
-        if binding in ("all", "rc_insert_column"):
-            self.rc_insert_column_enabled = False
-            self.rc_popup_menus_enabled = False
-            self.rc_select_enabled = False
-        if binding in ("all", "rc_insert_row"):
-            self.rc_insert_row_enabled = False
-            self.rc_popup_menus_enabled = False
-            self.rc_select_enabled = False
-        if binding in ("all", "copy", "edit_bindings"):
-            self.copy_enabled = False
-        if binding in ("all", "cut", "edit_bindings"):
-            self.cut_enabled = False
-        if binding in ("all", "paste", "edit_bindings"):
-            self.paste_enabled = False
-        if binding in ("all", "delete", "edit_bindings"):
-            self.delete_key_enabled = False
-        if binding in ("all", "right_click_popup_menu", "rc_popup_menu"):
-            self.rc_popup_menus_enabled = False
-            self.rc_select_enabled = False
-        if binding in ("all", "right_click_select", "rc_select"):
-            self.rc_select_enabled = False
-        if binding in ("all", "undo", "edit_bindings"):
+            self._tksheet_unbind("next_bindings")
+        if binding in ("all", "undo", "redo", "edit_bindings", "edit"):
             self.undo_enabled = False
-        if binding in ("all", "edit_cell", "edit_bindings"):
-            self.edit_cell_enabled = False
-        if binding in ("all", "edit_header", "edit_bindings"):
-            self.CH.edit_cell_enabled = False
-        if binding in ("all", "edit_index", "edit_bindings"):
-            self.RI.edit_cell_enabled = False
-        if binding in ("all", "ctrl_click_select", "ctrl_select"):
-            self.ctrl_select_enabled = False
+            self._tksheet_unbind("undo_bindings", "redo_bindings")
+
+    def _tksheet_unbind(self, *keys) -> None:
+        for widget in (self, self.RI, self.CH, self.TL):
+            for bindings_key in keys:
+                for binding in self.PAR.ops[bindings_key]:
+                    widget.unbind(binding)
 
     def reset_mouse_motion_creations(self) -> None:
         if self.current_cursor != "":
             self.config(cursor="")
             self.RI.config(cursor="")
             self.CH.config(cursor="")
             self.current_cursor = ""
@@ -2778,17 +2832,18 @@
                             self.select_cell(r, c, redraw=True)
                         elif self.toggle_selection_enabled:
                             self.toggle_select_cell(r, c, redraw=True)
                     if self.rc_popup_menus_enabled:
                         popup_menu = self.rc_popup_menu
             else:
                 self.deselect("all")
-                popup_menu = self.empty_rc_popup_menu
+                if self.rc_popup_menus_enabled:
+                    popup_menu = self.empty_rc_popup_menu
         try_binding(self.extra_rc_func, event)
-        if popup_menu is not None:
+        if popup_menu:
             popup_menu.tk_popup(event.x_root, event.y_root)
 
     def b1_press(self, event=None):
         self.closed_dropdown = self.mouseclick_outside_editor_or_dropdown_all_canvases()
         self.focus_set()
         if (
             self.identify_col(x=event.x, allow_end=False) is None
@@ -3020,19 +3075,17 @@
                 need_redraw = True
             if need_redraw:
                 self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True, redraw_table=True)
         elif not self.ctrl_select_enabled:
             self.b1_motion(event)
 
     def b1_release(self, event=None):
-        if self.being_drawn_item is not None:
-            to_sel = self.coords_and_type(self.being_drawn_item)
+        if self.being_drawn_item is not None and (to_sel := self.coords_and_type(self.being_drawn_item)):
             r_to_sel, c_to_sel = self.selected.row, self.selected.column
             self.hide_selection_box(self.being_drawn_item)
-            self.being_drawn_item = None
             self.set_currently_selected(
                 r_to_sel,
                 c_to_sel,
                 item=self.create_selection_box(
                     *to_sel,
                     state=(
                         "hidden"
@@ -3042,14 +3095,16 @@
                     set_current=False,
                 ),
             )
             sel_event = self.get_select_event(being_drawn_item=self.being_drawn_item)
             if self.drag_selection_binding_func:
                 self.drag_selection_binding_func(sel_event)
             self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
+        else:
+            self.being_drawn_item = None
         if self.RI.width_resizing_enabled and self.RI.rsz_w is not None and self.RI.currently_resizing_width:
             self.delete_resize_lines()
             self.RI.delete_resize_lines()
             self.RI.currently_resizing_width = False
             self.RI.set_width(self.new_row_width, set_TL=True)
             self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
             self.b1_pressed_loc = None
@@ -3192,55 +3247,79 @@
                 need_redraw = True
         if need_redraw:
             self.fix_views()
             self.x_move_synced_scrolls("moveto", self.xview()[0])
             self.y_move_synced_scrolls("moveto", self.yview()[0])
         return need_redraw
 
-    def x_move_synced_scrolls(self, *args, redraw: bool = True):
+    def x_move_synced_scrolls(self, *args, redraw: bool = True, use_scrollbar: bool = False):
         for widget in self.synced_scrolls:
             # try:
             if hasattr(widget, "MT"):
-                widget.MT.set_xviews(*args, move_synced=False, redraw=redraw)
+                if use_scrollbar:
+                    widget.MT._xscrollbar(*args, move_synced=False)
+                else:
+                    widget.MT.set_xviews(*args, move_synced=False, redraw=redraw)
             else:
                 widget.xview(*args)
             # except Exception:
             #     continue
 
-    def y_move_synced_scrolls(self, *args, redraw: bool = True):
+    def y_move_synced_scrolls(self, *args, redraw: bool = True, use_scrollbar: bool = False):
         for widget in self.synced_scrolls:
             # try:
             if hasattr(widget, "MT"):
-                widget.MT.set_yviews(*args, move_synced=False, redraw=redraw)
+                if use_scrollbar:
+                    widget.MT._yscrollbar(*args, move_synced=False)
+                else:
+                    widget.MT.set_yviews(*args, move_synced=False, redraw=redraw)
             else:
                 widget.yview(*args)
             # except Exception:
             #     continue
 
+    def _xscrollbar(self, *args, move_synced: bool = True):
+        self.xview(*args)
+        if self.show_header:
+            self.CH.xview(*args)
+        self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
+        if move_synced:
+            self.x_move_synced_scrolls(*args, use_scrollbar=True)
+
+    def _yscrollbar(self, *args, move_synced: bool = True):
+        self.yview(*args)
+        if self.show_index:
+            self.RI.yview(*args)
+        self.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
+        if move_synced:
+            self.y_move_synced_scrolls(*args, use_scrollbar=True)
+
     def set_xviews(self, *args, move_synced: bool = True, redraw: bool = True) -> None:
         self.main_table_redraw_grid_and_text(setting_views=True)
         self.update_idletasks()
         self.xview(*args)
         if self.show_header:
+            self.CH.update_idletasks()
             self.CH.xview(*args)
+        self.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=False)
         if move_synced:
             self.x_move_synced_scrolls(*args)
         self.fix_views()
-        self.PAR.set_refresh_timer(redraw)
 
     def set_yviews(self, *args, move_synced: bool = True, redraw: bool = True) -> None:
         self.main_table_redraw_grid_and_text(setting_views=True)
         self.update_idletasks()
         self.yview(*args)
         if self.show_index:
+            self.RI.update_idletasks()
             self.RI.yview(*args)
+        self.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=True)
         if move_synced:
             self.y_move_synced_scrolls(*args)
         self.fix_views()
-        self.PAR.set_refresh_timer(redraw)
 
     def set_view(self, x_args: list[str, float], y_args: list[str, float]) -> None:
         self.set_xviews(*x_args)
         self.set_yviews(*y_args)
 
     def mousewheel(self, event: object) -> None:
         if event.delta < 0 or event.num == 5:
@@ -3383,15 +3462,15 @@
         )
         b = self.txt_measure_canvas.bbox(self.txt_measure_canvas_text)
         return b[2] - b[0], b[3] - b[1]
 
     def get_lines_cell_height(self, n, font=None):
         return (
             self.get_txt_h(
-                txt="\n".join("|" for lines in range(n)) if n > 1 else "|",
+                txt="\n".join("|" for _ in range(n)) if n > 1 else "|",
                 font=self.PAR.ops.table_font if font is None else font,
             )
             + 5
         )
 
     def set_min_column_width(self):
         self.min_column_width = 1
@@ -3401,20 +3480,28 @@
             isinstance(self.PAR.ops.auto_resize_columns, (int, float))
             and self.PAR.ops.auto_resize_columns < self.min_column_width
         ):
             self.PAR.ops.auto_resize_columns = self.min_column_width
 
     def get_default_row_height(self) -> int:
         if isinstance(self.PAR.ops.default_row_height, str):
-            return self.get_lines_cell_height(int(self.PAR.ops.default_row_height))
+            if int(self.PAR.ops.default_row_height) == 1:
+                return self.min_row_height
+            else:
+                return self.min_row_height + self.get_lines_cell_height(int(self.PAR.ops.default_row_height) - 1)
         return self.PAR.ops.default_row_height
 
     def get_default_header_height(self) -> int:
         if isinstance(self.PAR.ops.default_header_height, str):
-            return self.get_lines_cell_height(int(self.PAR.ops.default_header_height), font=self.PAR.ops.header_font)
+            if int(self.PAR.ops.default_header_height) == 1:
+                return self.min_header_height
+            else:
+                return self.min_header_height + self.get_lines_cell_height(
+                    int(self.PAR.ops.default_header_height) - 1, font=self.PAR.ops.header_font
+                )
         return self.PAR.ops.default_header_height
 
     def set_table_font(self, newfont: tuple | None = None, reset_row_positions: bool = False) -> tuple[str, int, str]:
         if newfont:
             if not isinstance(newfont, tuple):
                 raise ValueError("Argument must be tuple e.g. " "('Carlito', 12, 'normal')")
             if len(newfont) != 3:
@@ -3436,16 +3523,16 @@
     def set_table_font_help(self):
         self.table_txt_width, self.table_txt_height = self.get_txt_dimensions("|", self.PAR.ops.table_font)
         self.table_half_txt_height = ceil(self.table_txt_height / 2)
         if not self.table_half_txt_height % 2:
             self.table_first_ln_ins = self.table_half_txt_height + 2
         else:
             self.table_first_ln_ins = self.table_half_txt_height + 3
+        self.min_row_height = int(self.table_first_ln_ins * 2.25)
         self.table_xtra_lines_increment = int(self.table_txt_height)
-        self.min_row_height = self.table_txt_height + 5
         if self.min_row_height < 12:
             self.min_row_height = 12
         self.set_min_column_width()
 
     def set_header_font(self, newfont: tuple | None = None) -> tuple[str, int, str]:
         if newfont:
             if not isinstance(newfont, tuple):
@@ -3465,15 +3552,15 @@
         self.header_txt_width, self.header_txt_height = self.get_txt_dimensions("|", self.PAR.ops.header_font)
         self.header_half_txt_height = ceil(self.header_txt_height / 2)
         if not self.header_half_txt_height % 2:
             self.header_first_ln_ins = self.header_half_txt_height + 2
         else:
             self.header_first_ln_ins = self.header_half_txt_height + 3
         self.header_xtra_lines_increment = self.header_txt_height
-        self.min_header_height = self.header_txt_height + 5
+        self.min_header_height = int(self.header_first_ln_ins * 2.25)
         if (
             isinstance(self.PAR.ops.default_header_height, int)
             and self.PAR.ops.default_header_height < self.min_header_height
         ):
             self.PAR.ops.default_header_height = int(self.min_header_height)
         self.set_min_column_width()
         self.CH.set_height(self.get_default_header_height(), set_TL=True)
@@ -3515,14 +3602,15 @@
         reset_col_positions: bool = True,
         reset_row_positions: bool = True,
         redraw: bool = False,
         return_id: bool = True,
         keep_formatting: bool = True,
     ) -> object:
         if isinstance(newdataref, (list, tuple)):
+            self.hide_dropdown_editor_all_canvases()
             self.data = newdataref
             if keep_formatting:
                 self.reapply_formatting()
             else:
                 self.delete_all_formatting(clear_values=False)
             self.purge_undo_and_redo_stack()
             if reset_col_positions:
@@ -3618,15 +3706,15 @@
             self.recreate_all_selection_boxes()
             if redraw:
                 self.refresh()
                 return True
             else:
                 return False
 
-    def set_all_cell_sizes_to_text(self, w: int | None = None) -> tuple[list[float], list[float]]:
+    def set_all_cell_sizes_to_text(self, w: int | None = None, slim: bool = False) -> tuple[list[float], list[float]]:
         min_column_width = int(self.min_column_width)
         min_rh = int(self.min_row_height)
         w = min_column_width if w is None else w
         h = min_rh
         rhs = defaultdict(lambda: int(min_rh))
         cws = []
         qconf = self.txt_measure_canvas.itemconfig
@@ -3649,23 +3737,24 @@
                 w_, h = self.RI.get_cell_dimensions(datarn)
                 if h < min_rh:
                     h = int(min_rh)
                 elif h > self.max_row_height:
                     h = int(self.max_row_height)
                 if h > rhs[datarn]:
                     rhs[datarn] = h
+        added_w_space = 1 if slim else 7
         for datacn in itercols:
             if (hw := self.CH.get_cell_dimensions(datacn)[0]) > w:
                 w = hw
             for datarn in iterrows:
                 txt = self.get_valid_cell_data_as_str(datarn, datacn, get_displayed=True)
                 if txt:
                     qconf(qtxtm, text=txt, font=qfont)
                     b = qbbox(qtxtm)
-                    tw = b[2] - b[0] + 7
+                    tw = b[2] - b[0] + added_w_space
                     h = b[3] - b[1] + 5
                 else:
                     tw = min_column_width
                     h = min_rh
                 if self.get_cell_kwargs(
                     datarn,
                     datacn,
@@ -3736,46 +3825,42 @@
             del self.row_positions[-1]
         else:
             w = self.row_positions[idx + 1] - self.row_positions[idx]
             idx += 1
             del self.row_positions[idx]
             self.row_positions[idx:] = [e - w for e in islice(self.row_positions, idx, len(self.row_positions))]
 
+    def del_col_positions(self, idxs: Iterator[int] | None = None):
+        if idxs is None:
+            del self.col_positions[-1]
+        else:
+            if not isinstance(idxs, set):
+                idxs = set(idxs)
+            self.set_col_positions(itr=(w for i, w in enumerate(self.gen_column_widths()) if i not in idxs))
+
+    def del_row_positions(self, idxs: Iterator[int] | None = None):
+        if idxs is None:
+            del self.row_positions[-1]
+        else:
+            if not isinstance(idxs, set):
+                idxs = set(idxs)
+            self.set_row_positions(itr=(h for i, h in enumerate(self.gen_row_heights()) if i not in idxs))
+
     def get_column_widths(self) -> list[int]:
         return diff_list(self.col_positions)
 
     def get_row_heights(self) -> list[int]:
         return diff_list(self.row_positions)
 
     def gen_column_widths(self) -> Generator[int]:
         return diff_gen(self.col_positions)
 
     def gen_row_heights(self) -> Generator[int]:
         return diff_gen(self.row_positions)
 
-    def del_col_positions(self, idx: int, num: int = 1, deselect_all: bool = False):
-        if deselect_all:
-            self.deselect("all", redraw=False)
-        if idx == "end" or len(self.col_positions) <= idx + 1:
-            del self.col_positions[-1]
-        else:
-            cws = self.get_column_widths()
-            cws[idx : idx + num] = []
-            self.set_col_positions(itr=cws)
-
-    def del_row_positions(self, idx: int, numrows: int = 1, deselect_all: bool = False):
-        if deselect_all:
-            self.deselect("all", redraw=False)
-        if idx == "end" or len(self.row_positions) <= idx + 1:
-            del self.row_positions[-1]
-        else:
-            rhs = self.get_row_heights()
-            rhs[idx : idx + numrows] = []
-            self.set_row_positions(itr=rhs)
-
     def insert_col_position(
         self,
         idx: Literal["end"] | int = "end",
         width: int | None = None,
         deselect_all: bool = False,
     ) -> None:
         if deselect_all:
@@ -4204,14 +4289,15 @@
         header: dict,
         column_widths: dict,
         event_data: dict,
         displayed_columns: None | list[int] = None,
         create_ops: bool = True,
         create_selections: bool = True,
         add_row_positions: bool = True,
+        push_ops: bool = True,
     ) -> EventDataDict:
         self.saved_column_widths = {}
         saved_displayed_columns = list(self.displayed_columns)
         if isinstance(displayed_columns, list):
             self.displayed_columns = displayed_columns
         elif not self.all_columns_displayed:
             # push displayed indexes by one for every inserted column
@@ -4230,39 +4316,39 @@
                 column_widths[i] = self.PAR.ops.default_column_width
         self.set_col_positions(
             itr=insert_items(
                 cws,
                 column_widths,
             )
         )
-        # we're inserting so we can use indexes == len for
-        # fix functions, the values will go on the end
+        # rn needed for indexing but cn insert
         maxrn = 0
         for cn, rowdict in reversed(columns.items()):
             for rn, v in rowdict.items():
-                if rn > len(self.data):
-                    self.fix_data_len(rn - 1, cn - 1)
+                if rn >= len(self.data):
+                    self.fix_data_len(rn, cn - 1)
                 if rn > maxrn:
                     maxrn = rn
                 self.data[rn].insert(cn, v)
         # if not hiding rows then we can extend row positions if necessary
         if add_row_positions and self.all_rows_displayed and maxrn + 1 > len(self.row_positions) - 1:
             default_row_height = self.get_default_row_height()
             self.set_row_positions(
                 itr=chain(
                     self.gen_row_heights(),
                     (default_row_height for i in range(len(self.row_positions) - 1, maxrn + 1)),
                 )
             )
-        if isinstance(self._headers, list):
+        if isinstance(self._headers, list) and header:
             self._headers = insert_items(self._headers, header, self.CH.fix_header)
-        self.adjust_options_post_add_columns(
-            cols=tuple(reversed(columns)),
-            create_ops=create_ops,
-        )
+        if push_ops:
+            self.adjust_options_post_add_columns(
+                cols=tuple(reversed(columns)),
+                create_ops=create_ops,
+            )
         if create_selections:
             self.deselect("all")
             for boxst, boxend in consecutive_ranges(tuple(reversed(column_widths))):
                 self.create_selection_box(
                     0,
                     boxst,
                     len(self.row_positions) - 1,
@@ -4310,39 +4396,41 @@
         ):
             numcols = self.PAR.ops.paste_insert_column_limit - len(self.col_positions) - 1
             if numcols < 1:
                 return
         event_data = event_dict(
             name="add_columns",
             sheet=self.PAR.name,
+            widget=self,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         if not try_binding(self.extra_begin_insert_cols_rc_func, event_data, "begin_add_columns"):
             return
         event_data = self.add_columns(
             *self.get_args_for_add_columns(data_ins_col, displayed_ins_col, numcols),
             event_data=event_data,
         )
         if self.undo_enabled:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.refresh()
         try_binding(self.extra_end_insert_cols_rc_func, event_data, "end_add_columns")
         self.sheet_modified(event_data)
 
     def add_rows(
         self,
         rows: dict,
         index: dict,
         row_heights: dict,
         event_data: dict,
         displayed_rows: None | list[int] = None,
         create_ops: bool = True,
         create_selections: bool = True,
         add_col_positions: bool = True,
+        push_ops: bool = True,
     ) -> EventDataDict:
         self.saved_row_heights = {}
         saved_displayed_rows = list(self.displayed_rows)
         if isinstance(displayed_rows, list):
             self.displayed_rows = displayed_rows
         elif not self.all_rows_displayed:
             # push displayed indexes by one for every inserted column
@@ -4363,35 +4451,37 @@
         self.set_row_positions(
             itr=insert_items(
                 rhs,
                 row_heights,
             )
         )
         maxcn = 0
+        # rn needed for insert but cn indexing
         for rn, row in reversed(rows.items()):
             cn = len(row) - 1
             if rn > len(self.data):
                 self.fix_data_len(rn - 1, cn)
             self.data.insert(rn, row)
             if cn > maxcn:
                 maxcn = cn
-        if isinstance(self._row_index, list):
+        if isinstance(self._row_index, list) and index:
             self._row_index = insert_items(self._row_index, index, self.RI.fix_index)
         # if not hiding columns then we can extend col positions if necessary
         if add_col_positions and self.all_columns_displayed and maxcn + 1 > len(self.col_positions) - 1:
             self.set_col_positions(
                 itr=chain(
                     self.gen_column_widths(),
                     (self.PAR.ops.default_column_width for i in range(len(self.col_positions) - 1, maxcn + 1)),
                 )
             )
-        self.adjust_options_post_add_rows(
-            rows=tuple(reversed(rows)),
-            create_ops=create_ops,
-        )
+        if push_ops:
+            self.adjust_options_post_add_rows(
+                rows=tuple(reversed(rows)),
+                create_ops=create_ops,
+            )
         if create_selections:
             self.deselect("all")
             for boxst, boxend in consecutive_ranges(tuple(reversed(row_heights))):
                 self.create_selection_box(
                     boxst,
                     0,
                     boxend,
@@ -4439,25 +4529,26 @@
         ):
             numrows = self.PAR.ops.paste_insert_row_limit - len(self.row_positions) - 1
             if numrows < 1:
                 return
         event_data = event_dict(
             name="add_rows",
             sheet=self.PAR.name,
+            widget=self,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         if not try_binding(self.extra_begin_insert_rows_rc_func, event_data, "begin_add_rows"):
             return
         event_data = self.add_rows(
             *self.get_args_for_add_rows(data_ins_row, displayed_ins_row, numrows),
             event_data=event_data,
         )
         if self.undo_enabled:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.refresh()
         try_binding(self.extra_end_insert_rows_rc_func, event_data, "end_add_rows")
         self.sheet_modified(event_data)
 
     def get_args_for_add_columns(
         self,
         data_ins_col: int,
@@ -4470,24 +4561,24 @@
         header_data = {}
         if isinstance(self._headers, list):
             if headers and columns:
                 header_data = {
                     datacn: column[0]
                     for datacn, column in zip(reversed(range(data_ins_col, data_ins_col + numcols)), reversed(columns))
                 }
-            elif columns:
+            else:
                 header_data = {
                     datacn: self.CH.get_value_for_empty_cell(datacn, c_ops=False)
                     for datacn in reversed(range(data_ins_col, data_ins_col + numcols))
                 }
         if columns is None:
+            rowrange = len(self.data) if self.data else 1
             columns = {
                 datacn: {
-                    datarn: self.get_value_for_empty_cell(datarn, datacn, c_ops=False)
-                    for datarn in range(len(self.data))
+                    datarn: self.get_value_for_empty_cell(datarn, datacn, c_ops=False) for datarn in range(rowrange)
                 }
                 for datacn in reversed(range(data_ins_col, data_ins_col + numcols))
             }
         else:
             if headers:
                 start = 1
             else:
@@ -4521,24 +4612,25 @@
         index_data = {}
         if isinstance(self._row_index, list):
             if row_index and rows:
                 index_data = {
                     datarn: v[0]
                     for datarn, v in zip(reversed(range(data_ins_row, data_ins_row + numrows)), reversed(rows))
                 }
-            elif rows:
+            else:
                 index_data = {
                     datarn: self.RI.get_value_for_empty_cell(datarn, r_ops=False)
                     for datarn in reversed(range(data_ins_row, data_ins_row + numrows))
                 }
         if rows is None:
             if total_data_cols is None:
                 total_data_cols = self.total_data_cols()
+            colrange = total_data_cols if total_data_cols else 1
             rows = {
-                datarn: [self.get_value_for_empty_cell(datarn, c, c_ops=False) for c in range(total_data_cols)]
+                datarn: [self.get_value_for_empty_cell(datarn, c, c_ops=False) for c in range(colrange)]
                 for datarn in reversed(range(data_ins_row, data_ins_row + numrows))
             }
         else:
             if row_index:
                 start = 1
             else:
                 start = 0
@@ -4612,24 +4704,25 @@
     def rc_delete_columns(self, event: object = None):
         selected = sorted(self.get_selected_cols())
         if not self.selected:
             return
         event_data = event_dict(
             name="delete_columns",
             sheet=self.PAR.name,
+            widget=self,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         if not try_binding(self.extra_begin_del_cols_rc_func, event_data, "begin_delete_columns"):
             return
         event_data = self.delete_columns_displayed(selected, event_data)
         data_cols = selected if self.all_columns_displayed else [self.displayed_columns[c] for c in selected]
         event_data = self.delete_columns_data(data_cols, event_data)
         if self.undo_enabled:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.deselect("all")
         try_binding(self.extra_end_del_cols_rc_func, event_data, "end_delete_columns")
         self.sheet_modified(event_data)
 
     def delete_rows_data(self, rows: list, event_data: dict) -> EventDataDict:
         self.mouseclick_outside_editor_or_dropdown_all_canvases()
         event_data["deleted"]["displayed_rows"] = (
@@ -4666,24 +4759,25 @@
     def rc_delete_rows(self, event: object = None):
         selected = sorted(self.get_selected_rows())
         if not self.selected:
             return
         event_data = event_dict(
             name="delete_rows",
             sheet=self.PAR.name,
+            widget=self,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         if not try_binding(self.extra_begin_del_rows_rc_func, event_data, "begin_delete_rows"):
             return
         event_data = self.delete_rows_displayed(selected, event_data)
         data_rows = selected if self.all_rows_displayed else [self.displayed_rows[r] for r in selected]
         event_data = self.delete_rows_data(data_rows, event_data)
         if self.undo_enabled:
-            self.undo_stack.append(ev_stack_dict(event_data))
+            self.undo_stack.append(pickled_event_dict(event_data))
         self.deselect("all")
         try_binding(self.extra_end_del_rows_rc_func, event_data, "end_delete_rows")
         self.sheet_modified(event_data)
 
     def move_row_position(self, idx1: int, idx2: int):
         if not len(self.row_positions) <= 2:
             if idx1 < idx2:
@@ -4898,16 +4992,16 @@
         at_least_cols: int | None = None,
     ) -> int:
         if not isinstance(total_data_cols, int):
             total_data_cols = self.total_data_cols(include_header=include_header)
         if isinstance(at_least_cols, int) and at_least_cols > total_data_cols:
             total_data_cols = at_least_cols
         total_data_cols = max(total_data_cols, len(self.col_positions) - 1)
-        if include_header and total_data_cols > len(self._headers):
-            self.CH.fix_header(total_data_cols)
+        if not isinstance(self._headers, int) and include_header and total_data_cols > len(self._headers):
+            self.CH.fix_header(total_data_cols - 1)
         for rn, r in enumerate(self.data):
             if total_data_cols > (lnr := len(r)):
                 r += self.get_empty_row_seq(rn, end=total_data_cols, start=lnr)
         return total_data_cols
 
     def get_canvas_visible_area(self) -> tuple[float, float, float, float]:
         return (
@@ -5122,20 +5216,17 @@
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill)
                 else:
                     self.itemconfig(t, fill=fill, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_line(
+                t = self.create_polygon(
                     points,
                     fill=fill,
-                    width=2,
-                    capstyle=tk.ROUND,
-                    joinstyle=tk.ROUND,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
     def redraw_checkbox(
         self,
         x1: int | float,
@@ -5190,16 +5281,15 @@
         except Exception:
             return False
         row_pos_exists = self.row_positions != [0] and self.row_positions
         col_pos_exists = self.col_positions != [0] and self.col_positions
         resized_cols = False
         resized_rows = False
         if self.PAR.ops.auto_resize_columns and self.allow_auto_resize_columns and col_pos_exists:
-            max_w = int(can_width)
-            max_w -= self.PAR.ops.empty_horizontal
+            max_w = can_width - self.PAR.ops.empty_horizontal
             if self.PAR.ops.auto_resize_columns < self.min_column_width:
                 min_column_width = self.column_width
             else:
                 min_column_width = self.PAR.ops.auto_resize_columns
             if (len(self.col_positions) - 1) * min_column_width < max_w:
                 resized_cols = True
                 change = int((max_w - self.col_positions[-1]) / (len(self.col_positions) - 1))
@@ -5213,18 +5303,17 @@
                         diffs[i] = min_column_width - w
                         widths[i] = min_column_width
                 if diffs and len(diffs) < len(widths):
                     change = sum(diffs.values()) / (len(widths) - len(diffs))
                     for i, w in enumerate(widths):
                         if i not in diffs:
                             widths[i] -= change
-                self.set_col_positions(itr=widths)
+                self.col_positions = list(accumulate(chain([0], widths)))
         if self.PAR.ops.auto_resize_rows and self.allow_auto_resize_rows and row_pos_exists:
-            max_h = int(can_height)
-            max_h -= self.PAR.ops.empty_vertical
+            max_h = can_height - self.PAR.ops.empty_vertical
             if self.PAR.ops.auto_resize_rows < self.min_row_height:
                 min_row_height = self.min_row_height
             else:
                 min_row_height = self.PAR.ops.auto_resize_rows
             if (len(self.row_positions) - 1) * min_row_height < max_h:
                 resized_rows = True
                 change = int((max_h - self.row_positions[-1]) / (len(self.row_positions) - 1))
@@ -5239,69 +5328,76 @@
                         heights[i] = min_row_height
                 if diffs and len(diffs) < len(heights):
                     change = sum(diffs.values()) / (len(heights) - len(diffs))
                     for i, h in enumerate(heights):
                         if i not in diffs:
                             heights[i] -= change
                 self.row_positions = list(accumulate(chain([0], heights)))
-        last_col_line_pos = self.col_positions[-1] + 1
-        last_row_line_pos = self.row_positions[-1] + 1
-        if can_width >= last_col_line_pos + self.PAR.ops.empty_horizontal and self.PAR.xscroll_showing:
-            self.PAR.xscroll.grid_forget()
-            self.PAR.xscroll_showing = False
-        elif (
-            can_width < last_col_line_pos + self.PAR.ops.empty_horizontal
-            and not self.PAR.xscroll_showing
-            and not self.PAR.xscroll_disabled
-            and can_height > 40
-        ):
-            self.PAR.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
-            self.PAR.xscroll_showing = True
-        if can_height >= last_row_line_pos + self.PAR.ops.empty_vertical and self.PAR.yscroll_showing:
+        if self.PAR.ops.auto_resize_row_index is not True:
+            if can_width >= self.col_positions[-1] + self.PAR.ops.empty_horizontal and self.PAR.xscroll_showing:
+                self.PAR.xscroll.grid_forget()
+                self.PAR.xscroll_showing = False
+            elif (
+                can_width < self.col_positions[-1] + self.PAR.ops.empty_horizontal
+                and not self.PAR.xscroll_showing
+                and not self.PAR.xscroll_disabled
+                and can_height > 40
+            ):
+                self.PAR.xscroll.grid(row=2, column=0, columnspan=2, sticky="nswe")
+                self.PAR.xscroll_showing = True
+        if can_height >= self.row_positions[-1] + self.PAR.ops.empty_vertical and self.PAR.yscroll_showing:
             self.PAR.yscroll.grid_forget()
             self.PAR.yscroll_showing = False
         elif (
-            can_height < last_row_line_pos + self.PAR.ops.empty_vertical
+            can_height < self.row_positions[-1] + self.PAR.ops.empty_vertical
             and not self.PAR.yscroll_showing
             and not self.PAR.yscroll_disabled
             and can_width > 40
         ):
             self.PAR.yscroll.grid(row=0, column=2, rowspan=3, sticky="nswe")
             self.PAR.yscroll_showing = True
+        last_col_line_pos = self.col_positions[-1] + 1
+        last_row_line_pos = self.row_positions[-1] + 1
         scrollregion = (
             0,
             0,
             last_col_line_pos + self.PAR.ops.empty_horizontal + 2,
             last_row_line_pos + self.PAR.ops.empty_vertical + 2,
         )
-        if scrollregion != self.scrollregion:
+        if setting_views or scrollregion != self.scrollregion:
             self.configure(scrollregion=scrollregion)
             self.scrollregion = scrollregion
-        if setting_views:
-            return False
+            self.CH.configure_scrollregion(last_col_line_pos)
+            self.RI.configure_scrollregion(last_row_line_pos)
+            if setting_views:
+                return False
         scrollpos_bot = self.canvasy(can_height)
         end_row = bisect_right(self.row_positions, scrollpos_bot)
         if not scrollpos_bot >= self.row_positions[-1]:
             end_row += 1
         scrollpos_left = self.canvasx(0)
         scrollpos_top = self.canvasy(0)
         scrollpos_right = self.canvasx(can_width)
         start_row = bisect_left(self.row_positions, scrollpos_top)
         start_col = bisect_left(self.col_positions, scrollpos_left)
         end_col = bisect_right(self.col_positions, scrollpos_right)
         changed_w = False
-        if redraw_row_index and self.show_index:
+        if self.PAR.ops.auto_resize_row_index and redraw_row_index and self.show_index:
             changed_w = self.RI.auto_set_index_width(
                 end_row=end_row - 1,
                 only_rows=[self.datarn(r) for r in range(start_row if not start_row else start_row - 1, end_row - 1)],
             )
+        if resized_cols or resized_rows or changed_w:
+            self.recreate_all_selection_boxes()
             if changed_w:
+                self.update_idletasks()
+                self.RI.update_idletasks()
+                self.CH.update_idletasks()
+                self.TL.update_idletasks()
                 return False
-        if resized_cols or resized_rows:
-            self.recreate_all_selection_boxes()
         self.hidd_text.update(self.disp_text)
         self.disp_text = {}
         self.hidd_high.update(self.disp_high)
         self.disp_high = {}
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
@@ -5681,15 +5777,15 @@
         if isinstance(item, int) and item in self.selection_boxes:
             selection_box = self.selection_boxes[item]
             r1, c1, r2, c2 = selection_box.coords
             if r is None:
                 r = r1
             if c is None:
                 c = c1
-            if r1 <= r and c1 <= c and r2 > r and c2 > c:
+            if r1 <= r and c1 <= c and r2 >= r and c2 >= c:
                 self.create_currently_selected_box(
                     r,
                     c,
                     selection_box.type_,
                     selection_box.fill_iid,
                 )
                 return
@@ -5697,28 +5793,28 @@
         if isinstance(box, tuple):
             if r is None:
                 r = box[0]
             if c is None:
                 c = box[1]
             for item, selection_box in self.get_selection_items(reverse=True):
                 r1, c1, r2, c2 = selection_box.coords
-                if box == (r1, c1, r2, c2) and r1 <= r and c1 <= c and r2 > r and c2 > c:
+                if box == (r1, c1, r2, c2) and r1 <= r and c1 <= c and r2 >= r and c2 >= c:
                     self.create_currently_selected_box(
                         r,
                         c,
                         selection_box.type_,
                         selection_box.fill_iid,
                     )
                     return
         # currently selected is just pointed at a coordinate
         # find the top most box there, requires r and c
         if r is not None and c is not None:
             for item, selection_box in self.get_selection_items(reverse=True):
                 r1, c1, r2, c2 = selection_box.coords
-                if r1 <= r and c1 <= c and r2 > r and c2 > c:
+                if r1 <= r and c1 <= c and r2 >= r and c2 >= c:
                     self.create_currently_selected_box(
                         r,
                         c,
                         selection_box.type_,
                         selection_box.fill_iid,
                     )
                     return
@@ -5846,14 +5942,16 @@
         self.hide_box(box.fill_iid)
         self.hide_box(box.bd_iid)
         self.RI.hide_box(box.index)
         self.CH.hide_box(box.header)
         if self.selected.fill_iid == item:
             self.hide_selected()
             self.set_current_to_last()
+        if item == self.being_drawn_item:
+            self.being_drawn_item = None
         return True
 
     def hide_selected(self) -> None:
         if self.selected:
             self.hide_box(self.selected.iid)
             self.selected = tuple()
 
@@ -6081,17 +6179,24 @@
         self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
 
     def recreate_all_selection_boxes(self) -> None:
         if not self.selected:
             return
         for item, box in self.get_selection_items():
             r1, c1, r2, c2 = box.coords
-            if r1 >= len(self.row_positions) - 1 or c1 >= len(self.col_positions) - 1:
-                self.hide_selection_box(item)
-                continue
+            if r1 >= len(self.row_positions) - 1:
+                if len(self.row_positions) > 1:
+                    r1 = len(self.row_positions) - 2
+                else:
+                    r1 = len(self.row_positions) - 1
+            if c1 >= len(self.col_positions) - 1:
+                if len(self.col_positions) > 1:
+                    c1 = len(self.col_positions) - 2
+                else:
+                    c1 = len(self.col_positions) - 1
             if r2 > len(self.row_positions) - 1:
                 r2 = len(self.row_positions) - 1
             if c2 > len(self.col_positions) - 1:
                 c2 = len(self.col_positions) - 1
             self.recreate_selection_box(r1, c1, r2, c2, item)
         if self.selected:
             r = self.selected.row
@@ -6416,39 +6521,33 @@
             self.text_editor.window = TextEditor(self, newline_binding=self.text_editor_newline_binding)
             self.text_editor.canvas_id = self.create_window((x, y), window=self.text_editor.window, anchor="nw")
         self.text_editor.window.reset(**kwargs)
         if not self.text_editor.open:
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
+        for b in text_editor_newline_bindings:
+            self.text_editor.tktext.bind(b, self.text_editor_newline_binding)
+        for b in text_editor_close_bindings:
+            self.text_editor.tktext.bind(b, self.close_text_editor)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
-        self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(r, c))
-        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(r, c))
-        if USER_OS == "darwin":
-            self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(r, c))
+            self.text_editor.tktext.bind("<FocusOut>", self.close_text_editor)
         for key, func in self.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
-        self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((r, c, "Tab")))
-        self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((r, c, "Return")))
-        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((r, c, "Return")))
-        if not dropdown:
-            self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((r, c, "FocusOut")))
-        self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((r, c, "Escape")))
         return True
 
     # displayed indexes
     def text_editor_newline_binding(
         self,
-        r: int = 0,
-        c: int = 0,
         event: object = None,
         check_lines: bool = True,
     ) -> None:
+        r, c = self.text_editor.coords
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.min_row_height:
             return
         if (
             not check_lines
             or self.get_lines_cell_height(
                 self.text_editor.window.get_num_lines() + 1,
@@ -6524,39 +6623,41 @@
             for binding in text_editor_to_unbind:
                 self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
-    def close_text_editor(
-        self,
-        editor_info: tuple | None = None,
-    ) -> str | None:
+    def close_text_editor(self, event: tk.Event) -> Literal["break"] | None:
         # checking if text editor should be closed or not
-        focused = self.focus_get()
+        # errors if __tk_filedialog is open
+        try:
+            focused = self.focus_get()
+        except Exception:
+            focused = None
         try:
             if focused == self.text_editor.tktext.rc_popup_menu:
                 return "break"
         except Exception:
             pass
-        if focused is None and editor_info:
+        if focused is None:
             return "break"
-        if editor_info[2] == "Escape":
+        if event.keysym == "Escape":
             self.hide_text_editor_and_dropdown()
             return
         # setting cell data with text editor value
         text_editor_value = self.text_editor.get()
-        r, c = editor_info[0], editor_info[1]
+        r, c = self.text_editor.coords
         datarn, datacn = self.datarn(r), self.datacn(c)
         event_data = event_dict(
             name="end_edit_table",
             sheet=self.PAR.name,
+            widget=self,
             cells_table={(datarn, datacn): text_editor_value},
-            key=editor_info[2],
+            key=event.keysym,
             value=text_editor_value,
             loc=Loc(r, c),
             row=r,
             column=c,
             boxes=self.get_boxes(),
             selected=self.selected,
         )
@@ -6587,48 +6688,48 @@
             and (self.single_selection_enabled or self.toggle_selection_enabled)
             and (edited or self.cell_equal_to(datarn, datacn, text_editor_value))
         ):
             r1, c1, r2, c2 = self.selection_boxes[self.selected.fill_iid].coords
             numcols = c2 - c1
             numrows = r2 - r1
             if numcols == 1 and numrows == 1:
-                if editor_info[2] == "Return":
+                if event.keysym == "Return":
                     self.select_cell(r + 1 if r < len(self.row_positions) - 2 else r, c)
                     self.see(
                         r + 1 if r < len(self.row_positions) - 2 else r,
                         c,
                         keep_xscroll=True,
                         bottom_right_corner=True,
                         check_cell_visibility=True,
                     )
-                elif editor_info[2] == "Tab":
+                elif event.keysym == "Tab":
                     self.select_cell(r, c + 1 if c < len(self.col_positions) - 2 else c)
                     self.see(
                         r,
                         c + 1 if c < len(self.col_positions) - 2 else c,
                         keep_xscroll=True,
                         bottom_right_corner=True,
                         check_cell_visibility=True,
                     )
             else:
                 moved = False
                 new_r = r
                 new_c = c
-                if editor_info[2] == "Return":
+                if event.keysym == "Return":
                     if r + 1 == r2:
                         new_r = r1
                     elif numrows > 1:
                         new_r = r + 1
                         moved = True
                     if not moved:
                         if c + 1 == c2:
                             new_c = c1
                         elif numcols > 1:
                             new_c = c + 1
-                elif editor_info[2] == "Tab":
+                elif event.keysym == "Tab":
                     if c + 1 == c2:
                         new_c = c1
                     elif numcols > 1:
                         new_c = c + 1
                         moved = True
                     if not moved:
                         if r + 1 == r2:
@@ -6641,15 +6742,15 @@
                     new_c,
                     keep_xscroll=False,
                     bottom_right_corner=True,
                     check_cell_visibility=True,
                 )
         self.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
-        if editor_info[2] != "FocusOut":
+        if event.keysym != "FocusOut":
             self.focus_set()
         return "break"
 
     def tab_key(self, event: object = None) -> str:
         if not self.selected:
             return
         r, c = self.selected.row, self.selected.column
@@ -6761,14 +6862,15 @@
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, r=r, c=c, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(r, c)
         win_w = self.col_positions[c + 1] - self.col_positions[c] + 1
         if anchor == "nw":
             if kwargs["state"] == "normal":
+                self.text_editor.window.update_idletasks()
                 ypos = self.row_positions[r] + self.text_editor.window.winfo_height() - 1
             else:
                 ypos = self.row_positions[r + 1]
         else:
             ypos = self.row_positions[r]
         reset_kwargs = {
             "r": r,
@@ -6779,16 +6881,17 @@
             "ops": self.PAR.ops,
             "outline_color": self.get_selected_box_bg_fg(type_="cells")[1],
             "align": self.get_cell_align(r, c),
             "values": kwargs["values"],
         }
         if self.dropdown.window:
             self.dropdown.window.reset(**reset_kwargs)
-            self.itemconfig(self.dropdown.canvas_id, state="normal", anchor=anchor)
             self.coords(self.dropdown.canvas_id, self.col_positions[c], ypos)
+            self.itemconfig(self.dropdown.canvas_id, state="normal", anchor=anchor)
+            self.dropdown.window.tkraise()
         else:
             self.dropdown.window = self.PAR.dropdown_class(
                 self.winfo_toplevel(),
                 **reset_kwargs,
                 close_dropdown_window=self.close_dropdown_window,
                 search_function=kwargs["search_function"],
                 arrowkey_RIGHT=self.arrowkey_RIGHT,
@@ -6798,15 +6901,15 @@
                 (self.col_positions[c], ypos),
                 window=self.dropdown.window,
                 anchor=anchor,
             )
         if kwargs["state"] == "normal":
             self.text_editor.tktext.bind(
                 "<<TextModified>>",
-                lambda x: self.dropdown.window.search_and_see(
+                lambda _: self.dropdown.window.search_and_see(
                     event_dict(
                         name="table_dropdown_modified",
                         sheet=self.PAR.name,
                         value=self.text_editor.get(),
                         loc=Loc(r, c),
                         row=r,
                         column=c,
@@ -6822,15 +6925,15 @@
                 self.after(1, lambda: self.text_editor.tktext.focus())
                 self.after(2, self.text_editor.window.scroll_to_bottom())
             except Exception:
                 return
             redraw = False
         else:
             self.update_idletasks()
-            self.dropdown.window.bind("<FocusOut>", lambda x: self.close_dropdown_window(r, c))
+            self.dropdown.window.bind("<FocusOut>", lambda _: self.close_dropdown_window(r, c))
             self.dropdown.window.focus()
             redraw = True
         self.dropdown.open = True
         if redraw:
             self.main_table_redraw_grid_and_text(redraw_header=False, redraw_row_index=False)
 
     # displayed indexes, not data
@@ -6845,14 +6948,15 @@
             datacn = self.datacn(c)
             datarn = self.datarn(r)
             kwargs = self.get_cell_kwargs(datarn, datacn, key="dropdown")
             pre_edit_value = self.get_cell_data(datarn, datacn)
             event_data = event_dict(
                 name="end_edit_table",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_table={(datarn, datacn): pre_edit_value},
                 key="??",
                 value=selection,
                 loc=Loc(r, c),
                 row=r,
                 column=c,
                 boxes=self.get_boxes(),
@@ -6891,24 +6995,29 @@
         self.hide_dropdown_window()
         if redraw:
             self.refresh()
 
     def mouseclick_outside_editor_or_dropdown(self) -> tuple[int, int] | None:
         closed_dd_coords = self.dropdown.get_coords()
         if self.text_editor.open:
-            self.close_text_editor(editor_info=self.text_editor.coords + ("ButtonPress-1",))
+            self.close_text_editor(new_tk_event("ButtonPress-1"))
         self.hide_dropdown_window()
         self.focus_set()
         return closed_dd_coords
 
     def mouseclick_outside_editor_or_dropdown_all_canvases(self):
         self.CH.mouseclick_outside_editor_or_dropdown()
         self.RI.mouseclick_outside_editor_or_dropdown()
         return self.mouseclick_outside_editor_or_dropdown()
 
+    def hide_dropdown_editor_all_canvases(self):
+        self.hide_text_editor_and_dropdown(redraw=False)
+        self.RI.hide_text_editor_and_dropdown(redraw=False)
+        self.CH.hide_text_editor_and_dropdown(redraw=False)
+
     def hide_dropdown_window(self) -> None:
         if self.dropdown.open:
             self.dropdown.window.unbind("<FocusOut>")
             self.itemconfig(self.dropdown.canvas_id, state="hidden")
             self.dropdown.open = False
 
     def click_checkbox(
@@ -6935,14 +7044,15 @@
                 undo=undo,
                 cell_resize=False,
                 check_input_valid=False,
             )
             event_data = event_dict(
                 name="end_edit_table",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_table={(datarn, datacn): pre_edit_value},
                 key="??",
                 value=value,
                 loc=Loc(r, c),
                 row=r,
                 column=c,
                 boxes=self.get_boxes(),
@@ -6972,21 +7082,22 @@
         if datacn is None:
             datacn = self.datacn(c)
         if datarn is None:
             datarn = self.datarn(r)
         event_data = event_dict(
             name="edit_table",
             sheet=self.PAR.name,
+            widget=self,
             cells_table={(datarn, datacn): self.get_cell_data(datarn, datacn)},
             boxes=self.get_boxes(),
             selected=self.selected,
         )
         if not check_input_valid or self.input_valid_for_cell(datarn, datacn, value):
             if self.undo_enabled and undo:
-                self.undo_stack.append(ev_stack_dict(event_data))
+                self.undo_stack.append(pickled_event_dict(event_data))
             self.set_cell_data(datarn, datacn, value)
             if cell_resize and self.PAR.ops.cell_auto_resize_enabled:
                 self.set_cell_size_to_text(r, c, only_set_if_too_small=True, redraw=redraw, run_binding=True)
             self.sheet_modified(event_data)
             return True
         return False
```

### Comparing `tksheet-7.1.9/tksheet/other_classes.py` & `tksheet-7.2.0/tksheet/other_classes.py`

 * *Files identical despite different names*

### Comparing `tksheet-7.1.9/tksheet/row_index.py` & `tksheet-7.2.0/tksheet/row_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,36 +25,38 @@
 )
 from .formatters import (
     is_bool_like,
     try_to_bool,
 )
 from .functions import (
     consecutive_chunks,
-    ev_stack_dict,
     event_dict,
     get_n2a,
     is_contiguous,
+    new_tk_event,
     num2alpha,
+    pickled_event_dict,
     rounded_box_coords,
     try_binding,
 )
 from .other_classes import (
     DotDict,
     DraggedRowColumn,
     DropdownStorage,
     Node,
     TextEditorStorage,
 )
 from .text_editor import (
     TextEditor,
 )
 from .vars import (
-    USER_OS,
     rc_binding,
     symbols_set,
+    text_editor_close_bindings,
+    text_editor_newline_bindings,
     text_editor_to_unbind,
 )
 
 
 class RowIndex(tk.Canvas):
     def __init__(self, *args, **kwargs):
         tk.Canvas.__init__(
@@ -113,31 +115,40 @@
         self.disp_high = {}
         self.disp_grid = {}
         self.disp_fill_sels = {}
         self.disp_bord_sels = {}
         self.disp_resize_lines = {}
         self.disp_dropdown = {}
         self.disp_checkbox = {}
+        self.disp_tree_arrow = {}
         self.disp_boxes = set()
         self.hidd_text = {}
         self.hidd_high = {}
         self.hidd_grid = {}
         self.hidd_fill_sels = {}
         self.hidd_bord_sels = {}
         self.hidd_resize_lines = {}
         self.hidd_dropdown = {}
         self.hidd_checkbox = {}
+        self.hidd_tree_arrow = {}
         self.hidd_boxes = set()
 
         self.align = kwargs["row_index_align"]
         self.default_index = kwargs["default_row_index"].lower()
 
         self.tree_reset()
         self.basic_bindings()
 
+    def event_generate(self, *args, **kwargs) -> None:
+        for arg in args:
+            if self.MT and arg in self.MT.event_linker:
+                self.MT.event_linker[arg]()
+            else:
+                super().event_generate(*args, **kwargs)
+
     def basic_bindings(self, enable: bool = True) -> None:
         if enable:
             self.bind("<Motion>", self.mouse_motion)
             self.bind("<ButtonPress-1>", self.b1_press)
             self.bind("<B1-Motion>", self.b1_motion)
             self.bind("<ButtonRelease-1>", self.b1_release)
             self.bind("<Double-Button-1>", self.double_b1)
@@ -158,22 +169,22 @@
         if self.MT:
             self.MT.displayed_rows = []
             self.MT._row_index = []
             self.MT.data = []
             self.MT.row_positions = [0]
             self.MT.saved_row_heights = {}
 
-    def set_width(self, new_width: int, set_TL: bool = False) -> None:
+    def set_width(self, new_width: int, set_TL: bool = False, recreate_selection_boxes: bool = True) -> None:
         self.current_width = new_width
         try:
             self.config(width=new_width)
         except Exception:
             return
         if set_TL:
-            self.TL.set_dimensions(new_w=new_width)
+            self.TL.set_dimensions(new_w=new_width, recreate_selection_boxes=recreate_selection_boxes)
 
     def rc(self, event: object) -> None:
         self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
         self.focus_set()
         popup_menu = None
         if self.MT.identify_row(y=event.y, allow_end=False) is None:
             self.MT.deselect("all")
@@ -387,30 +398,32 @@
                         name="resize",
                         sheet=self.PAR.name,
                         resized_rows={row: {"old_size": old_height, "new_size": new_height}},
                     )
                 )
         elif self.width_resizing_enabled and self.rsz_h is None and self.rsz_w is True:
             self.set_width_of_index_to_text()
-        elif self.row_selection_enabled and self.rsz_h is None and self.rsz_w is None:
+        elif (self.row_selection_enabled or self.PAR.ops.treeview) and self.rsz_h is None and self.rsz_w is None:
             r = self.MT.identify_row(y=event.y)
             if r < len(self.MT.row_positions) - 1:
-                if self.MT.single_selection_enabled:
-                    self.select_row(r, redraw=True)
-                elif self.MT.toggle_selection_enabled:
-                    self.toggle_select_row(r, redraw=True)
+                iid = self.event_over_tree_arrow(r, self.canvasy(event.y), event.x)
+                if self.row_selection_enabled:
+                    if self.MT.single_selection_enabled:
+                        self.select_row(r, redraw=iid is None)
+                    elif self.MT.toggle_selection_enabled:
+                        self.toggle_select_row(r, redraw=iid is None)
                 datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
                 if (
                     self.get_cell_kwargs(datarn, key="dropdown")
                     or self.get_cell_kwargs(datarn, key="checkbox")
                     or self.edit_cell_enabled
                 ):
                     self.open_cell(event)
-                elif (iid := self.event_over_tree_arrow(r, self.canvasy(event.y), event.x)) is not None:
-                    self.PAR.item(iid, open_=iid not in self.tree_open_ids, redraw=False)
+                elif iid is not None:
+                    self.PAR.item(iid, open_=iid not in self.tree_open_ids)
         self.rsz_h = None
         self.mouse_motion(event)
         try_binding(self.extra_double_b1_func, event)
 
     def b1_press(self, event: object):
         self.MT.unbind("<MouseWheel>")
         self.focus_set()
@@ -755,27 +768,27 @@
             and self.get_cell_kwargs(datarn, key="checkbox")
             and event.x < self.MT.index_txt_height + 4
         ):
             return True
         return False
 
     def b1_release(self, event: object) -> None:
-        if self.being_drawn_item is not None:
-            to_sel = self.MT.coords_and_type(self.being_drawn_item)
+        if self.being_drawn_item is not None and (to_sel := self.MT.coords_and_type(self.being_drawn_item)):
             r_to_sel, c_to_sel = self.MT.selected.row, self.MT.selected.column
             self.MT.hide_selection_box(self.being_drawn_item)
-            self.being_drawn_item = None
             self.MT.set_currently_selected(
                 r_to_sel,
                 c_to_sel,
                 item=self.MT.create_selection_box(*to_sel, set_current=False),
             )
             sel_event = self.MT.get_select_event(being_drawn_item=self.being_drawn_item)
             try_binding(self.drag_selection_binding_func, sel_event)
             self.PAR.emit_event("<<SheetSelect>>", data=sel_event)
+        else:
+            self.being_drawn_item = None
         self.MT.bind("<MouseWheel>", self.MT.mousewheel)
         if self.height_resizing_enabled and self.rsz_h is not None and self.currently_resizing_height:
             self.currently_resizing_height = False
             new_row_pos = int(self.coords("rhl")[1])
             self.hide_resize_and_ctrl_lines(ctrl_lines=False)
             old_height = self.MT.row_positions[self.rsz_h] - self.MT.row_positions[self.rsz_h - 1]
             size = new_row_pos - self.MT.row_positions[self.rsz_h - 1]
@@ -827,33 +840,35 @@
                 )
             ):
                 if r >= len(self.MT.row_positions) - 1:
                     r -= 1
                 event_data = event_dict(
                     name="move_rows",
                     sheet=self.PAR.name,
+                    widget=self,
                     boxes=self.MT.get_boxes(),
                     selected=self.MT.selected,
                     value=r,
                 )
                 if try_binding(self.ri_extra_begin_drag_drop_func, event_data, "begin_move_rows"):
                     data_new_idxs, disp_new_idxs, event_data = self.MT.move_rows_adjust_options_dict(
                         *self.MT.get_args_for_move_rows(
                             move_to=r,
                             to_move=self.dragged_row.to_move,
                         ),
                         move_data=self.PAR.ops.row_drag_and_drop_perform,
+                        move_heights=self.PAR.ops.row_drag_and_drop_perform,
                         event_data=event_data,
                     )
                     event_data["moved"]["rows"] = {
                         "data": data_new_idxs,
                         "displayed": disp_new_idxs,
                     }
                     if self.MT.undo_enabled:
-                        self.MT.undo_stack.append(ev_stack_dict(event_data))
+                        self.MT.undo_stack.append(pickled_event_dict(event_data))
                     self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
                     try_binding(self.ri_extra_end_drag_drop_func, event_data, "end_move_rows")
                     self.MT.sheet_modified(event_data)
         elif self.b1_pressed_loc is not None and self.rsz_w is None and self.rsz_h is None:
             r = self.MT.identify_row(y=event.y)
             if (
                 r is not None
@@ -866,15 +881,15 @@
                 if self.event_over_dropdown(r, datarn, event, canvasy) or self.event_over_checkbox(
                     r, datarn, event, canvasy
                 ):
                     self.open_cell(event)
                 elif (iid := self.event_over_tree_arrow(r, canvasy, event.x)) is not None:
                     if self.MT.selection_boxes:
                         self.select_row(r, redraw=False)
-                    self.PAR.item(iid, open_=iid not in self.tree_open_ids, redraw=False)
+                    self.PAR.item(iid, open_=iid not in self.tree_open_ids)
             else:
                 self.mouseclick_outside_editor_or_dropdown_all_canvases(inside=True)
             self.b1_pressed_loc = None
             self.closed_dropdown = None
         self.dragged_row = None
         self.currently_resizing_width = False
         self.currently_resizing_height = False
@@ -1003,23 +1018,23 @@
             b = self.MT.txt_measure_canvas.bbox(self.MT.txt_measure_canvas_text)
             w = b[2] - b[0] + 7
             h = b[3] - b[1] + 5
         else:
             w = self.PAR.ops.default_row_index_width
             h = self.MT.min_row_height
         if self.get_cell_kwargs(datarn, key="dropdown") or self.get_cell_kwargs(datarn, key="checkbox"):
-            w += self.MT.index_txt_height
+            w += self.MT.index_txt_height + 2
         if self.PAR.ops.treeview:
             if datarn in self.cell_options and "align" in self.cell_options[datarn]:
                 align = self.cell_options[datarn]["align"]
             else:
                 align = self.align
             if align == "w":
                 w += self.MT.index_txt_height
-            w += self.get_treeview_indent(self.MT._row_index[datarn].iid)
+            w += self.get_treeview_indent(self.MT._row_index[datarn].iid) + 5
         return w, h
 
     def set_row_height(
         self,
         row: int,
         height: None | int = None,
         only_set_if_too_small: bool = False,
@@ -1173,65 +1188,64 @@
             )
         else:
             self.MT.set_row_positions(itr=(height for r in range(len(self.MT.data))))
         if recreate:
             self.MT.recreate_all_selection_boxes()
 
     def auto_set_index_width(self, end_row: int, only_rows: list) -> bool:
-        if self.PAR.ops.auto_resize_row_index:
-            if not isinstance(self.MT._row_index, int) and not self.MT._row_index:
-                if self.default_index == "letters":
-                    new_w = self.MT.get_txt_w(f"{num2alpha(end_row)}") + 20
-                elif self.default_index == "numbers":
-                    new_w = self.MT.get_txt_w(f"{end_row}") + 20
-                elif self.default_index == "both":
-                    new_w = self.MT.get_txt_w(f"{end_row + 1} {num2alpha(end_row)}") + 20
-            elif self.PAR.ops.auto_resize_row_index is True:
-                new_w = self.set_width_of_index_to_text(only_rows=only_rows, set_width=False)
-            else:
-                new_w = None
-            if new_w is not None and (sheet_w := floor(self.PAR.winfo_width() * 0.5)) < new_w:
-                new_w = sheet_w
-            if new_w and (self.current_width - new_w > 15 or new_w - self.current_width > 5):
-                self.set_width(new_w, set_TL=True)
-                return True
+        if not isinstance(self.MT._row_index, int) and not self.MT._row_index:
+            if self.default_index == "letters":
+                new_w = self.MT.get_txt_w(f"{num2alpha(end_row)}") + 20
+            elif self.default_index == "numbers":
+                new_w = self.MT.get_txt_w(f"{end_row}") + 20
+            elif self.default_index == "both":
+                new_w = self.MT.get_txt_w(f"{end_row + 1} {num2alpha(end_row)}") + 20
+        elif self.PAR.ops.auto_resize_row_index is True:
+            new_w = self.set_width_of_index_to_text(only_rows=only_rows, set_width=False)
+        else:
+            new_w = None
+        if new_w is not None and (sheet_w_x := floor(self.PAR.winfo_width() * 0.7)) < new_w:
+            new_w = sheet_w_x
+        if new_w and (self.current_width - new_w > 20 or new_w - self.current_width > 3):
+            self.set_width(new_w, set_TL=True, recreate_selection_boxes=False)
+            return True
         return False
 
     def redraw_highlight_get_text_fg(self, fr, sr, r, c_2, c_3, selections, datarn):
         redrawn = False
         kwargs = self.get_cell_kwargs(datarn, key="highlight")
         if kwargs:
             if kwargs[0] is not None:
                 c_1 = kwargs[0] if kwargs[0].startswith("#") else color_map[kwargs[0]]
             if "rows" in selections and r in selections["rows"]:
-                tf = (
+                txtfg = (
                     self.PAR.ops.index_selected_rows_fg
                     if kwargs[1] is None or self.PAR.ops.display_selected_fg_over_highlights
                     else kwargs[1]
                 )
                 if kwargs[0] is not None:
                     fill = (
                         f"#{int((int(c_1[1:3], 16) + int(c_3[1:3], 16)) / 2):02X}"
                         + f"{int((int(c_1[3:5], 16) + int(c_3[3:5], 16)) / 2):02X}"
                         + f"{int((int(c_1[5:], 16) + int(c_3[5:], 16)) / 2):02X}"
                     )
             elif "cells" in selections and r in selections["cells"]:
-                tf = (
+                txtfg = (
                     self.PAR.ops.index_selected_cells_fg
                     if kwargs[1] is None or self.PAR.ops.display_selected_fg_over_highlights
                     else kwargs[1]
                 )
                 if kwargs[0] is not None:
                     fill = (
                         f"#{int((int(c_1[1:3], 16) + int(c_2[1:3], 16)) / 2):02X}"
                         + f"{int((int(c_1[3:5], 16) + int(c_2[3:5], 16)) / 2):02X}"
                         + f"{int((int(c_1[5:], 16) + int(c_2[5:], 16)) / 2):02X}"
                     )
             else:
-                tf = self.PAR.ops.index_fg if kwargs[1] is None else kwargs[1]
+                txtfg = self.PAR.ops.index_fg if kwargs[1] is None else kwargs[1]
                 if kwargs[0] is not None:
                     fill = kwargs[0]
             if kwargs[0] is not None:
                 redrawn = self.redraw_highlight(
                     0,
                     fr + 1,
                     self.current_width - 1,
@@ -1240,22 +1254,26 @@
                     outline=(
                         self.PAR.ops.index_fg
                         if self.get_cell_kwargs(datarn, key="dropdown") and self.PAR.ops.show_dropdown_borders
                         else ""
                     ),
                     tag="s",
                 )
+            tree_arrow_fg = txtfg
         elif not kwargs:
             if "rows" in selections and r in selections["rows"]:
-                tf = self.PAR.ops.index_selected_rows_fg
+                txtfg = self.PAR.ops.index_selected_rows_fg
+                tree_arrow_fg = self.PAR.ops.selected_rows_tree_arrow_fg
             elif "cells" in selections and r in selections["cells"]:
-                tf = self.PAR.ops.index_selected_cells_fg
+                txtfg = self.PAR.ops.index_selected_cells_fg
+                tree_arrow_fg = self.PAR.ops.selected_cells_tree_arrow_fg
             else:
-                tf = self.PAR.ops.index_fg
-        return tf, redrawn
+                txtfg = self.PAR.ops.index_fg
+                tree_arrow_fg = self.PAR.ops.tree_arrow_fg
+        return txtfg, tree_arrow_fg, redrawn
 
     def redraw_highlight(self, x1, y1, x2, y2, fill, outline, tag):
         coords = (x1, y1, x2, y2)
         if self.hidd_high:
             iid, showing = self.hidd_high.popitem()
             self.coords(iid, coords)
             if showing:
@@ -1275,91 +1293,118 @@
                 self.itemconfig(t, fill=fill, width=width, tag=tag)
             else:
                 self.itemconfig(t, fill=fill, width=width, tag=tag, state="normal")
             self.disp_grid[t] = True
         else:
             self.disp_grid[self.create_line(points, fill=fill, width=width, tag=tag)] = True
 
+    def redraw_tree_arrow(
+        self,
+        x1,
+        y1,
+        r,
+        fill,
+        tag,
+        indent: float,
+        open_: bool = False,
+    ) -> None:
+        mod = (self.MT.index_txt_height - 1) if self.MT.index_txt_height % 2 else self.MT.index_txt_height
+        half_mod = mod / 2
+        qtr_mod = mod / 4
+        small_mod = int(half_mod / 4) - 1
+        mid_y = int(self.MT.min_row_height / 2)
+        # up arrow
+        if open_:
+            points = (
+                x1 + 2 + indent,
+                y1 + mid_y + qtr_mod,
+                x1 + 2 + half_mod + indent,
+                y1 + mid_y - qtr_mod,
+                x1 + 2 + mod + indent,
+                y1 + mid_y + qtr_mod,
+            )
+        # right pointing arrow
+        else:
+            points = (
+                x1 + half_mod + indent,
+                y1 + mid_y - half_mod + small_mod,
+                x1 + mod + indent - small_mod,
+                y1 + mid_y,
+                x1 + half_mod + indent,
+                y1 + mid_y + half_mod - small_mod,
+            )
+        if self.hidd_tree_arrow:
+            t, sh = self.hidd_tree_arrow.popitem()
+            self.coords(t, points)
+            if sh:
+                self.itemconfig(t, fill=fill)
+            else:
+                self.itemconfig(t, fill=fill, tag=tag, state="normal")
+            self.lift(t)
+        else:
+            t = self.create_line(
+                points,
+                fill=fill,
+                tag=tag,
+                width=2,
+                capstyle=tk.ROUND,
+                joinstyle=tk.BEVEL,
+            )
+        self.disp_tree_arrow[t] = True
+
     def redraw_dropdown(
         self,
         x1,
         y1,
         x2,
         y2,
         fill,
         outline,
         tag,
         draw_outline: bool = True,
         draw_arrow: bool = True,
         open_: bool = False,
-        indent: None | float = None,
     ) -> None:
         if draw_outline and self.PAR.ops.show_dropdown_borders:
             self.redraw_highlight(x1 + 1, y1 + 1, x2, y2, fill="", outline=self.PAR.ops.index_fg, tag=tag)
         if draw_arrow:
             mod = (self.MT.index_txt_height - 1) if self.MT.index_txt_height % 2 else self.MT.index_txt_height
             half_mod = mod / 2
             qtr_mod = mod / 4
             mid_y = (self.MT.index_first_ln_ins - 1) if self.MT.index_first_ln_ins % 2 else self.MT.index_first_ln_ins
-            # treeview
-            if indent is not None:
-                # up arrow
-                if open_:
-                    points = (
-                        x1 + 2 + indent,
-                        y1 + mid_y + qtr_mod,
-                        x1 + 2 + half_mod + indent,
-                        y1 + mid_y - qtr_mod,
-                        x1 + 2 + mod + indent,
-                        y1 + mid_y + qtr_mod,
-                    )
-                # right pointing arrow
-                else:
-                    points = (
-                        x1 + half_mod + indent,
-                        y1 + mid_y - half_mod + 1,
-                        x1 + mod + indent - 1,
-                        y1 + mid_y,
-                        x1 + half_mod + indent,
-                        y1 + mid_y + half_mod - 1,
-                    )
-            else:
-                if open_:
-                    points = (
-                        x2 - 3 - mod,
-                        y1 + mid_y + qtr_mod,
-                        x2 - 3 - half_mod,
-                        y1 + mid_y - qtr_mod,
-                        x2 - 3,
-                        y1 + mid_y + qtr_mod,
-                    )
-                else:
-                    points = (
-                        x2 - 3 - mod,
-                        y1 + mid_y - qtr_mod,
-                        x2 - 3 - half_mod,
-                        y1 + mid_y + qtr_mod,
-                        x2 - 3,
-                        y1 + mid_y - qtr_mod,
-                    )
+            if open_:
+                points = (
+                    x2 - 3 - mod,
+                    y1 + mid_y + qtr_mod,
+                    x2 - 3 - half_mod,
+                    y1 + mid_y - qtr_mod,
+                    x2 - 3,
+                    y1 + mid_y + qtr_mod,
+                )
+            else:
+                points = (
+                    x2 - 3 - mod,
+                    y1 + mid_y - qtr_mod,
+                    x2 - 3 - half_mod,
+                    y1 + mid_y + qtr_mod,
+                    x2 - 3,
+                    y1 + mid_y - qtr_mod,
+                )
             if self.hidd_dropdown:
                 t, sh = self.hidd_dropdown.popitem()
                 self.coords(t, points)
                 if sh:
                     self.itemconfig(t, fill=fill)
                 else:
                     self.itemconfig(t, fill=fill, tag=tag, state="normal")
                 self.lift(t)
             else:
-                t = self.create_line(
+                t = self.create_polygon(
                     points,
                     fill=fill,
-                    width=2,
-                    capstyle=tk.ROUND,
-                    joinstyle=tk.ROUND,
                     tag=tag,
                 )
             self.disp_dropdown[t] = True
 
     def redraw_checkbox(self, x1, y1, x2, y2, fill, outline, tag, draw_check=False):
         points = rounded_box_coords(x1, y1, x2, y2)
         if self.hidd_checkbox:
@@ -1388,45 +1433,50 @@
                 else:
                     self.itemconfig(t, fill=fill, outline=outline, tag=tag, state="normal")
                 self.lift(t)
             else:
                 t = self.create_polygon(points, fill=fill, outline=outline, tag=tag, smooth=True)
             self.disp_checkbox[t] = True
 
+    def configure_scrollregion(self, last_row_line_pos: float) -> None:
+        self.configure(
+            scrollregion=(
+                0,
+                0,
+                self.current_width,
+                last_row_line_pos + self.PAR.ops.empty_vertical + 2,
+            )
+        )
+
     def redraw_grid_and_text(
         self,
-        last_row_line_pos: int,
+        last_row_line_pos: float,
         scrollpos_top: int,
         y_stop: int,
         start_row: int,
         end_row: int,
         scrollpos_bot: int,
         row_pos_exists: bool,
     ) -> None:
         try:
-            self.configure(
-                scrollregion=(
-                    0,
-                    0,
-                    self.current_width,
-                    last_row_line_pos + self.PAR.ops.empty_vertical + 2,
-                )
-            )
+            self.configure_scrollregion(last_row_line_pos=last_row_line_pos)
         except Exception:
             return
         self.hidd_text.update(self.disp_text)
         self.disp_text = {}
         self.hidd_high.update(self.disp_high)
         self.disp_high = {}
         self.hidd_grid.update(self.disp_grid)
         self.disp_grid = {}
         self.hidd_dropdown.update(self.disp_dropdown)
         self.disp_dropdown = {}
         self.hidd_checkbox.update(self.disp_checkbox)
         self.disp_checkbox = {}
+        self.hidd_tree_arrow.update(self.disp_tree_arrow)
+        self.disp_tree_arrow = {}
         self.visible_row_dividers = {}
         draw_y = self.MT.row_positions[start_row]
         xend = self.current_width - 6
         self.row_width_resize_bbox = (
             self.current_width - 2,
             scrollpos_top,
             self.current_width,
@@ -1475,15 +1525,23 @@
 
         for r in range(start_row, end_row - 1):
             rtopgridln = self.MT.row_positions[r]
             rbotgridln = self.MT.row_positions[r + 1]
             if rbotgridln - rtopgridln < self.MT.index_txt_height:
                 continue
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
-            fill, dd_drawn = self.redraw_highlight_get_text_fg(rtopgridln, rbotgridln, r, c_2, c_3, selections, datarn)
+            fill, tree_arrow_fg, dd_drawn = self.redraw_highlight_get_text_fg(
+                rtopgridln,
+                rbotgridln,
+                r,
+                c_2,
+                c_3,
+                selections,
+                datarn,
+            )
 
             if datarn in self.cell_options and "align" in self.cell_options[datarn]:
                 align = self.cell_options[datarn]["align"]
             else:
                 align = self.align
             dropdown_kwargs = self.get_cell_kwargs(datarn, key="dropdown")
             if align == "w":
@@ -1575,28 +1633,24 @@
                 )
             if treeview and isinstance(self.MT._row_index, list) and len(self.MT._row_index) > datarn:
                 iid = self.MT._row_index[datarn].iid
                 mw -= self.MT.index_txt_height
                 if align == "w":
                     draw_x += self.MT.index_txt_height + 1
                 indent = self.get_treeview_indent(iid)
-                draw_x += indent
+                draw_x += indent + 5
                 if self.tree[iid].children:
-                    self.redraw_dropdown(
+                    self.redraw_tree_arrow(
                         0,
                         rtopgridln,
-                        self.current_width - 1,
-                        rbotgridln - 1,
-                        fill=fill,
-                        outline=fill,
-                        tag="dd",
-                        draw_outline=False,
-                        draw_arrow=True,
-                        open_=self.MT._row_index[datarn].iid in self.tree_open_ids,
+                        r=r,
+                        fill=tree_arrow_fg,
+                        tag="ta",
                         indent=indent,
+                        open_=self.MT._row_index[datarn].iid in self.tree_open_ids,
                     )
             lns = self.get_valid_cell_data_as_str(datarn, fix=False)
             if not lns:
                 continue
             lns = lns.split("\n")
             draw_y = rtopgridln + self.MT.index_first_ln_ins
             if mw > 5:
@@ -1668,28 +1722,35 @@
                                     txt = txt[next(self.c_align_cyc)]
                                     self.itemconfig(iid, text=txt)
                                     wd = self.bbox(iid)
                                 self.coords(iid, draw_x, draw_y)
                         draw_y += self.MT.index_xtra_lines_increment
                         if draw_y + self.MT.index_half_txt_height - 1 > rbotgridln:
                             break
-        for dct in (self.hidd_text, self.hidd_high, self.hidd_grid, self.hidd_dropdown, self.hidd_checkbox):
+        for dct in (
+            self.hidd_text,
+            self.hidd_high,
+            self.hidd_grid,
+            self.hidd_dropdown,
+            self.hidd_checkbox,
+            self.hidd_tree_arrow,
+        ):
             for iid, showing in dct.items():
                 if showing:
                     self.itemconfig(iid, state="hidden")
                     dct[iid] = False
         return True
 
     def get_redraw_selections(self, startr: int, endr: int) -> dict[str, set[int]]:
         d = defaultdict(set)
-        for item, box in self.MT.get_selection_items(columns=False):
+        for item, box in self.MT.get_selection_items():
             r1, c1, r2, c2 = box.coords
             for r in range(startr, endr):
                 if r1 <= r and r2 > r:
-                    d[box.type_].add(r)
+                    d[box.type_ if box.type_ != "columns" else "cells"].add(r)
         return d
 
     def open_cell(self, event: object = None, ignore_existing_editor=False):
         if not self.MT.anything_selected() or (not ignore_existing_editor and self.text_editor.open):
             return
         if not self.MT.selected:
             return
@@ -1810,45 +1871,41 @@
             self.text_editor.window = TextEditor(self, newline_binding=self.text_editor_newline_binding)
             self.text_editor.canvas_id = self.create_window((x, y), window=self.text_editor.window, anchor="nw")
         self.text_editor.window.reset(**kwargs)
         if not self.text_editor.open:
             self.itemconfig(self.text_editor.canvas_id, state="normal")
             self.text_editor.open = True
         self.coords(self.text_editor.canvas_id, x, y)
+        for b in text_editor_newline_bindings:
+            self.text_editor.tktext.bind(b, self.text_editor_newline_binding)
+        for b in text_editor_close_bindings:
+            self.text_editor.tktext.bind(b, self.close_text_editor)
         if not dropdown:
             self.text_editor.tktext.focus_set()
             self.text_editor.window.scroll_to_bottom()
-        self.text_editor.tktext.bind("<Alt-Return>", lambda _x: self.text_editor_newline_binding(r=r))
-        self.text_editor.tktext.bind("<Alt-KP_Enter>", lambda _x: self.text_editor_newline_binding(r=r))
-        if USER_OS == "darwin":
-            self.text_editor.tktext.bind("<Option-Return>", lambda _x: self.text_editor_newline_binding(r=r))
+            self.text_editor.tktext.bind("<FocusOut>", self.close_text_editor)
         for key, func in self.MT.text_editor_user_bound_keys.items():
             self.text_editor.tktext.bind(key, func)
-        self.text_editor.tktext.bind("<Tab>", lambda _x: self.close_text_editor((r, "Tab")))
-        self.text_editor.tktext.bind("<Return>", lambda _x: self.close_text_editor((r, "Return")))
-        self.text_editor.tktext.bind("<KP_Enter>", lambda _x: self.close_text_editor((r, "Return")))
-        if not dropdown:
-            self.text_editor.tktext.bind("<FocusOut>", lambda _x: self.close_text_editor((r, "FocusOut")))
-        self.text_editor.tktext.bind("<Escape>", lambda _x: self.close_text_editor((r, "Escape")))
         return True
 
-    def text_editor_newline_binding(self, r=0, c=0, event: object = None, check_lines=True):
+    def text_editor_newline_binding(self, event: object = None, check_lines=True):
         if not self.height_resizing_enabled:
             return
         curr_height = self.text_editor.window.winfo_height()
         if curr_height < self.MT.min_row_height:
             return
         if (
             not check_lines
             or self.MT.get_lines_cell_height(
                 self.text_editor.window.get_num_lines() + 1,
                 font=self.text_editor.tktext.cget("font"),
             )
             > curr_height
         ):
+            r = self.text_editor.row
             new_height = curr_height + self.MT.index_xtra_lines_increment
             space_bot = self.MT.get_space_bot(r)
             if new_height > space_bot:
                 new_height = space_bot
             if new_height != curr_height:
                 self.set_row_height(r, new_height)
                 self.MT.refresh()
@@ -1856,22 +1913,22 @@
                 self.coords(self.text_editor.canvas_id, 0, self.MT.row_positions[r] + 1)
                 if self.dropdown.open and self.dropdown.get_coords() == r:
                     text_editor_h = self.text_editor.window.winfo_height()
                     win_h, anchor = self.get_dropdown_height_anchor(r, text_editor_h)
                     if anchor == "nw":
                         self.coords(
                             self.dropdown.canvas_id,
-                            self.MT.col_positions[c],
+                            0,
                             self.MT.row_positions[r] + text_editor_h - 1,
                         )
                         self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
                     elif anchor == "sw":
                         self.coords(
                             self.dropdown.canvas_id,
-                            self.MT.col_positions[c],
+                            0,
                             self.MT.row_positions[r],
                         )
                         self.itemconfig(self.dropdown.canvas_id, anchor=anchor, height=win_h)
 
     def refresh_open_window_positions(self, zoom: Literal["in", "out"]):
         if self.text_editor.open:
             r = self.text_editor.row
@@ -1917,37 +1974,40 @@
                 self.text_editor.tktext.unbind(binding)
             self.itemconfig(self.text_editor.canvas_id, state="hidden")
             self.text_editor.open = False
         if reason == "Escape":
             self.focus_set()
 
     # r is displayed row
-    def close_text_editor(
-        self,
-        editor_info: tuple | None = None,
-    ) -> str | None:
-        focused = self.focus_get()
+    def close_text_editor(self, event: tk.Event) -> Literal["break"] | None:
+        # checking if text editor should be closed or not
+        # errors if __tk_filedialog is open
+        try:
+            focused = self.focus_get()
+        except Exception:
+            focused = None
         try:
             if focused == self.text_editor.tktext.rc_popup_menu:
                 return "break"
         except Exception:
             pass
-        if focused is None and editor_info:
+        if focused is None:
             return "break"
-        if editor_info is not None and len(editor_info) >= 2 and editor_info[1] == "Escape":
+        if event.keysym == "Escape":
             self.hide_text_editor_and_dropdown()
             return
         text_editor_value = self.text_editor.get()
-        r = editor_info[0]
+        r = self.text_editor.row
         datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         event_data = event_dict(
             name="end_edit_index",
             sheet=self.PAR.name,
+            widget=self,
             cells_index={datarn: self.get_cell_data(datarn)},
-            key=editor_info[1] if len(editor_info) >= 2 else "FocusOut",
+            key=event.keysym,
             value=text_editor_value,
             loc=r,
             row=r,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
@@ -1963,15 +2023,15 @@
                 edited = set_data(value=text_editor_value)
         elif self.input_valid_for_cell(datarn, text_editor_value):
             edited = set_data(value=text_editor_value)
         if edited:
             try_binding(self.extra_end_edit_cell_func, event_data)
         self.MT.recreate_all_selection_boxes()
         self.hide_text_editor_and_dropdown()
-        if editor_info[1] != "FocusOut":
+        if event.keysym != "FocusOut":
             self.focus_set()
         return "break"
 
     def get_dropdown_height_anchor(self, r, text_editor_h=None):
         win_h = 5
         datarn = self.MT.datarn(r)
         for i, v in enumerate(self.get_cell_kwargs(datarn, key="dropdown")["values"]):
@@ -2020,14 +2080,15 @@
         if kwargs["state"] == "normal":
             if not self.open_text_editor(event=event, r=r, dropdown=True):
                 return
         win_h, anchor = self.get_dropdown_height_anchor(r)
         win_w = self.current_width + 1
         if anchor == "nw":
             if kwargs["state"] == "normal":
+                self.text_editor.window.update_idletasks()
                 ypos = self.MT.row_positions[r] + self.text_editor.window.winfo_height() - 1
             else:
                 ypos = self.MT.row_positions[r + 1]
         else:
             ypos = self.MT.row_positions[r]
         reset_kwargs = {
             "r": r,
@@ -2040,14 +2101,15 @@
             "align": self.get_cell_align(r),
             "values": kwargs["values"],
         }
         if self.dropdown.window:
             self.dropdown.window.reset(**reset_kwargs)
             self.itemconfig(self.dropdown.canvas_id, state="normal", anchor=anchor)
             self.coords(self.dropdown.canvas_id, 0, ypos)
+            self.dropdown.window.tkraise()
         else:
             self.dropdown.window = self.PAR.dropdown_class(
                 self.winfo_toplevel(),
                 **reset_kwargs,
                 single_index="r",
                 close_dropdown_window=self.close_dropdown_window,
                 search_function=kwargs["search_function"],
@@ -2098,14 +2160,15 @@
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
             kwargs = self.get_cell_kwargs(datarn, key="dropdown")
             pre_edit_value = self.get_cell_data(datarn)
             edited = False
             event_data = event_dict(
                 name="end_edit_index",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_header={datarn: pre_edit_value},
                 key="??",
                 value=selection,
                 loc=r,
                 row=r,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
@@ -2129,15 +2192,15 @@
         self.hide_dropdown_window()
         if redraw:
             self.MT.refresh()
 
     def mouseclick_outside_editor_or_dropdown(self, inside: bool = False):
         closed_dd_coords = self.dropdown.get_coords()
         if self.text_editor.open:
-            self.close_text_editor((self.text_editor.row, "ButtonPress-1"))
+            self.close_text_editor(new_tk_event("ButtonPress-1"))
         if closed_dd_coords is not None:
             self.hide_dropdown_window()
             if inside:
                 self.MT.main_table_redraw_grid_and_text(
                     redraw_header=False,
                     redraw_row_index=True,
                     redraw_table=False,
@@ -2167,26 +2230,27 @@
         check_input_valid: bool = True,
     ) -> bool:
         if datarn is None:
             datarn = r if self.MT.all_rows_displayed else self.MT.displayed_rows[r]
         event_data = event_dict(
             name="edit_index",
             sheet=self.PAR.name,
+            widget=self,
             cells_index={datarn: self.get_cell_data(datarn)},
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         edited = False
         if isinstance(self.MT._row_index, int):
             edited = self.MT.set_cell_data_undo(r=r, c=self.MT._row_index, datarn=datarn, value=value, undo=True)
         else:
             self.fix_index(datarn)
             if not check_input_valid or self.input_valid_for_cell(datarn, value):
                 if self.MT.undo_enabled and undo:
-                    self.MT.undo_stack.append(ev_stack_dict(event_data))
+                    self.MT.undo_stack.append(pickled_event_dict(event_data))
                 self.set_cell_data(datarn=datarn, value=value)
                 edited = True
         if edited and cell_resize and self.PAR.ops.cell_auto_resize_enabled:
             self.set_row_height_run_binding(r, only_set_if_too_small=False)
         if redraw:
             self.MT.refresh()
         if edited:
@@ -2321,14 +2385,15 @@
                 )
             else:
                 value = False
             self.set_cell_data_undo(r, datarn=datarn, value=value, cell_resize=False)
             event_data = event_dict(
                 name="end_edit_index",
                 sheet=self.PAR.name,
+                widget=self,
                 cells_index={datarn: pre_edit_value},
                 key="??",
                 value=value,
                 loc=r,
                 row=r,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
@@ -2374,15 +2439,15 @@
             if (check_open and cnode.children and cnode.iid in self.tree_open_ids) or (
                 not check_open and cnode.children
             ):
                 yield from self.get_iid_descendants(cnode.iid, check_open)
 
     def get_treeview_indent(self, iid: str) -> int:
         if isinstance(self.PAR.ops.treeview_indent, str):
-            indent = self.MT.index_txt_height * int(self.PAR.ops.treeview_indent)
+            indent = self.MT.index_txt_width * int(self.PAR.ops.treeview_indent)
         else:
             indent = self.PAR.ops.treeview_indent
         return indent * max(self.get_node_level(self.tree[iid]))
 
     def remove_node_from_parents_children(self, node: Node) -> None:
         if node.parent:
             node.parent.children.remove(node)
```

### Comparing `tksheet-7.1.9/tksheet/sheet.py` & `tksheet-7.2.0/tksheet/sheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,27 @@
     add_to_options,
     convert_align,
     data_to_displayed_idxs,
     del_from_options,
     del_named_span_options,
     del_named_span_options_nested,
     dropdown_search_function,
-    ev_stack_dict,
     event_dict,
     fix_format_kwargs,
+    new_tk_event,
+    force_bool,
     get_checkbox_dict,
     get_checkbox_kwargs,
     get_dropdown_dict,
     get_dropdown_kwargs,
     idx_param_to_int,
     is_iterable,
     key_to_span,
     num2alpha,
+    pickled_event_dict,
     pop_positions,
     set_align,
     set_readonly,
     span_froms,
     span_ranges,
     tksheet_type_error,
     unpack,
@@ -124,15 +126,16 @@
         to_clipboard_delimiter: str = "\t",
         to_clipboard_quotechar: str = '"',
         to_clipboard_lineterminator: str = "\n",
         from_clipboard_delimiters: list[str] | str = ["\t"],
         show_default_header_for_empty: bool = True,
         show_default_index_for_empty: bool = True,
         page_up_down_select_row: bool = True,
-        expand_sheet_if_paste_too_big: bool = False,
+        paste_can_expand_x: bool = False,
+        paste_can_expand_y: bool = False,
         paste_insert_column_limit: int | None = None,
         paste_insert_row_limit: int | None = None,
         show_dropdown_borders: bool = False,
         arrow_key_down_right_scroll_page: bool = False,
         cell_auto_resize_enabled: bool = True,
         auto_resize_row_index: bool | Literal["empty"] = "empty",
         auto_resize_columns: int | None = None,
@@ -167,15 +170,15 @@
         horizontal_grid_to_end_of_window: bool = False,
         vertical_grid_to_end_of_window: bool = False,
         show_vertical_grid: bool = True,
         show_horizontal_grid: bool = True,
         display_selected_fg_over_highlights: bool = False,
         show_selected_cells_border: bool = True,
         treeview: bool = False,
-        treeview_indent: str | int = "3",
+        treeview_indent: str | int = "6",
         rounded_boxes: bool = True,
         alternate_color: str = "",
         # colors
         outline_thickness: int = 0,
         outline_color: str = theme_light_blue["outline_color"],
         theme: str = "light blue",
         frame_bg: str = theme_light_blue["table_bg"],
@@ -259,14 +262,15 @@
         vertical_scroll_arrowsize: str | int = "",
         horizontal_scroll_arrowsize: str | int = "",
         # backwards compatibility
         column_width: int | None = None,
         header_height: str | int | None = None,
         row_height: str | int | None = None,
         row_index_width: int | None = None,
+        expand_sheet_if_paste_too_big: bool | None = None,
     ) -> None:
         tk.Frame.__init__(
             self,
             parent,
             background=frame_bg,
             highlightthickness=outline_thickness,
             highlightbackground=outline_color,
@@ -277,14 +281,17 @@
             default_column_width = column_width
         if header_height is not None:
             default_header_height = header_height
         if row_height is not None:
             default_row_height = row_height
         if row_index_width is not None:
             default_row_index_width = row_index_width
+        if expand_sheet_if_paste_too_big is not None:
+            paste_can_expand_x = expand_sheet_if_paste_too_big
+            paste_can_expand_y = expand_sheet_if_paste_too_big
         if treeview:
             index_align = "w"
             auto_resize_row_index = True
         for k, v in locals().items():
             if (xk := backwards_compatibility_keys.get(k, k)) in self.ops and v != self.ops[xk]:
                 self.ops[xk] = v
         self.ops.from_clipboard_delimiters = (
@@ -398,21 +405,21 @@
                             },
                         )
                     ],
                 )
         self.set_scrollbar_options()
         self.yscroll = ttk.Scrollbar(
             self,
-            command=self.MT.set_yviews,
+            command=self.MT._yscrollbar,
             orient="vertical",
             style=f"Sheet{self.unique_id}.Vertical.TScrollbar",
         )
         self.xscroll = ttk.Scrollbar(
             self,
-            command=self.MT.set_xviews,
+            command=self.MT._xscrollbar,
             orient="horizontal",
             style=f"Sheet{self.unique_id}.Horizontal.TScrollbar",
         )
         if show_top_left:
             self.TL.grid(row=0, column=0)
         if show_table:
             self.MT.grid(row=1, column=1, sticky="nswe")
@@ -520,16 +527,15 @@
                 value = list(value)
             self.MT._headers = value
         elif isinstance(c, int):
             self.CH.set_cell_data(c, value)
         elif is_iterable(value) and is_iterable(c):
             for c_, v in zip(c, value):
                 self.CH.set_cell_data(c_, v)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def headers(
         self,
         newheaders: object = None,
         index: None | int = None,
         reset_col_positions: bool = False,
         show_headers_if_not_sheet: bool = True,
@@ -557,16 +563,15 @@
                 value = list(value)
             self.MT._row_index = value
         elif isinstance(r, int):
             self.RI.set_cell_data(r, value)
         elif is_iterable(value) and is_iterable(r):
             for r_, v in zip(r, value):
                 self.RI.set_cell_data(r_, v)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def row_index(
         self,
         newindex: object = None,
         index: None | int = None,
         reset_row_positions: bool = False,
         show_index_if_not_sheet: bool = True,
@@ -579,27 +584,30 @@
             reset_row_positions=reset_row_positions,
             show_index_if_not_sheet=show_index_if_not_sheet,
             redraw=False,
         )
 
     # Bindings and Functionality
 
-    def enable_bindings(self, *bindings) -> Sheet:
+    def enable_bindings(self, *bindings: str) -> Sheet:
         self.MT.enable_bindings(bindings)
         return self
 
     def disable_bindings(self, *bindings) -> Sheet:
         self.MT.disable_bindings(bindings)
         return self
 
     def extra_bindings(
         self,
-        bindings: str | list | tuple,
+        bindings: str | list | tuple | None = None,
         func: Callable | None = None,
     ) -> Sheet:
+        # bindings is None, unbind all
+        if bindings is None:
+            bindings = "all"
         # bindings is str, func arg is None or Callable
         if isinstance(bindings, str):
             iterable = [(bindings, func)]
         # bindings is list or tuple of strings, func arg is None or Callable
         elif is_iterable(bindings) and isinstance(bindings[0], str):
             iterable = [(b, func) for b in bindings]
         # bindings is a list or tuple of two tuples or lists
@@ -914,20 +922,15 @@
 
     def bind(
         self,
         binding: str,
         func: Callable,
         add: str | None = None,
     ) -> Sheet:
-        if binding in emitted_events:
-            if add:
-                self.bound_events[binding].append(func)
-            else:
-                self.bound_events[binding] = [func]
-        elif binding == "<ButtonPress-1>":
+        if binding == "<ButtonPress-1>":
             self.MT.extra_b1_press_func = func
             self.CH.extra_b1_press_func = func
             self.RI.extra_b1_press_func = func
             self.TL.extra_b1_press_func = func
         elif binding == "<ButtonMotion-1>":
             self.MT.extra_b1_motion_func = func
             self.CH.extra_b1_motion_func = func
@@ -949,14 +952,19 @@
             self.RI.extra_motion_func = func
             self.TL.extra_motion_func = func
         elif binding == rc_binding:
             self.MT.extra_rc_func = func
             self.CH.extra_rc_func = func
             self.RI.extra_rc_func = func
             self.TL.extra_rc_func = func
+        elif binding in emitted_events:
+            if add:
+                self.bound_events[binding].append(func)
+            else:
+                self.bound_events[binding] = [func]
         else:
             self.MT.bind(binding, func, add=add)
             self.CH.bind(binding, func, add=add)
             self.RI.bind(binding, func, add=add)
             self.TL.bind(binding, func, add=add)
         return self
 
@@ -1043,37 +1051,31 @@
         return self
 
     def basic_bindings(self, enable: bool = False) -> Sheet:
         for canvas in (self.MT, self.CH, self.RI, self.TL):
             canvas.basic_bindings(enable)
         return self
 
-    def cut(self, event: object = None) -> Sheet:
-        self.MT.ctrl_x(event)
-        return self
+    def cut(self, event: object = None, validation: bool = True) -> None | EventDataDict:
+        return self.MT.ctrl_x(event, validation)
 
-    def copy(self, event: object = None) -> Sheet:
-        self.MT.ctrl_c(event)
-        return self
+    def copy(self, event: object = None) -> None | EventDataDict:
+        return self.MT.ctrl_c(event)
 
-    def paste(self, event: object = None) -> Sheet:
-        self.MT.ctrl_v(event)
-        return self
+    def paste(self, event: object = None, validation: bool = True) -> None | EventDataDict:
+        return self.MT.ctrl_v(event, validation)
 
-    def delete(self, event: object = None) -> Sheet:
-        self.MT.delete_key(event)
-        return self
+    def delete(self, event: object = None, validation: bool = True) -> None | EventDataDict:
+        return self.MT.delete_key(event, validation)
 
-    def undo(self, event: object = None) -> Sheet:
-        self.MT.undo(event)
-        return self
+    def undo(self, event: object = None) -> None | EventDataDict:
+        return self.MT.undo(event)
 
-    def redo(self, event: object = None) -> Sheet:
-        self.MT.redo(event)
-        return self
+    def redo(self, event: object = None) -> None | EventDataDict:
+        return self.MT.redo(event)
 
     def has_focus(
         self,
     ) -> bool:
         """
         Check if any Sheet widgets have focus
         Includes child widgets such as scroll bars
@@ -1458,23 +1460,34 @@
         row_heights: bool = True,
         column_widths: bool = True,
         cell_options: bool = True,
         tags: bool = True,
         undo_stack: bool = True,
         selections: bool = True,
         sheet_options: bool = False,
+        displayed_rows: bool = True,
+        displayed_columns: bool = True,
         tree: bool = True,
         redraw: bool = True,
     ) -> Sheet:
         if table:
+            self.MT.hide_text_editor_and_dropdown(redraw=False)
             self.MT.data = []
         if header:
+            self.CH.hide_text_editor_and_dropdown(redraw=False)
             self.MT._headers = []
         if index:
+            self.RI.hide_text_editor_and_dropdown(redraw=False)
             self.MT._row_index = []
+        if displayed_columns:
+            self.MT.displayed_columns = []
+            self.MT.all_columns_displayed = True
+        if displayed_rows:
+            self.MT.displayed_rows = []
+            self.MT.all_rows_displayed = True
         if row_heights:
             self.MT.saved_row_heights = {}
             self.MT.set_row_positions([])
         if column_widths:
             self.MT.saved_column_widths = {}
             self.MT.set_col_positions([])
         if cell_options:
@@ -1485,16 +1498,17 @@
             self.reset_undos()
         if selections:
             self.MT.deselect(redraw=False)
         if sheet_options:
             self.ops = new_sheet_options()
         if tree:
             self.RI.tree_reset()
-        self.set_refresh_timer(redraw)
-        return self
+        if tree or row_heights or column_widths:
+            self.MT.hide_dropdown_editor_all_canvases()
+        return self.set_refresh_timer(redraw)
 
     def set_sheet_data(
         self,
         data: list | tuple | None = None,
         reset_col_positions: bool = True,
         reset_row_positions: bool = True,
         redraw: bool = True,
@@ -1589,14 +1603,15 @@
         table, index, header = span.table, span.index, span.header
         fmt_kw = span.kwargs if span.type_ == "format" and span.kwargs else None
         transposed = span.transposed
         maxr, maxc = startr, startc
         event_data = event_dict(
             name="edit_table",
             sheet=self.name,
+            widget=self,
             selected=self.MT.selected,
         )
         set_t = self.event_data_set_table_cell
         set_i, set_h = self.event_data_set_index_cell, self.event_data_set_header_cell
         istart = 1 if index else 0
         hstart = 1 if header else 0
         # data is list
@@ -1794,15 +1809,15 @@
             event_data["cells"]["table"]
             or event_data["cells"]["index"]
             or event_data["cells"]["header"]
             or event_data["added"]["columns"]
             or event_data["added"]["rows"]
         ):
             if undo is True or (undo is None and span.undo):
-                self.MT.undo_stack.append(ev_stack_dict(event_data))
+                self.MT.undo_stack.append(pickled_event_dict(event_data))
             if emit_event is True or (emit_event is None and span.emit_event):
                 self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return event_data
 
     def clear(
         self,
@@ -1819,29 +1834,30 @@
         quick_tval = self.MT.get_value_for_empty_cell
         quick_ival = self.RI.get_value_for_empty_cell
         quick_hval = self.CH.get_value_for_empty_cell
         table, index, header = span.table, span.index, span.header
         event_data = event_dict(
             name="edit_table",
             sheet=self.name,
+            widget=self,
             selected=self.MT.selected,
         )
         if index:
             for r in rows:
                 event_data = clear_i(r, quick_ival(r), event_data)
         if header:
             for c in cols:
                 event_data = clear_h(c, quick_hval(c), event_data)
         if table:
             for r in rows:
                 for c in cols:
                     event_data = clear_t(r, c, quick_tval(r, c), event_data)
         if event_data["cells"]["table"] or event_data["cells"]["header"] or event_data["cells"]["index"]:
             if undo is True or (undo is None and span.undo):
-                self.MT.undo_stack.append(ev_stack_dict(event_data))
+                self.MT.undo_stack.append(pickled_event_dict(event_data))
             if emit_event is True or (emit_event is None and span.emit_event):
                 self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return event_data
 
     def event_data_set_table_cell(
         self,
@@ -1931,14 +1947,16 @@
         idx: str | int | None = None,
         heights: list[int] | tuple[int] | None = None,
         row_index: bool = False,
         fill: bool = True,
         undo: bool = False,
         emit_event: bool = False,
         create_selections: bool = True,
+        add_column_widths: bool = True,
+        push_ops: bool = True,
         redraw: bool = True,
     ) -> EventDataDict:
         total_cols = None
         if (idx := idx_param_to_int(idx)) is None:
             idx = len(self.MT.data)
         if isinstance(rows, int):
             if rows < 1:
@@ -1989,24 +2007,26 @@
                 data_ins_row=idx,
                 displayed_ins_row=displayed_ins_idx,
                 numrows=numrows,
                 rows=data,
                 heights=heights,
                 row_index=row_index,
             ),
+            add_col_positions=add_column_widths,
             event_data=event_dict(
                 name="add_rows",
                 sheet=self.name,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             ),
             create_selections=create_selections,
+            push_ops=push_ops,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return event_data
 
     def insert_columns(
         self,
@@ -2014,14 +2034,16 @@
         idx: str | int | None = None,
         widths: list[int] | tuple[int] | None = None,
         headers: bool = False,
         fill: bool = True,
         undo: bool = False,
         emit_event: bool = False,
         create_selections: bool = True,
+        add_row_heights: bool = True,
+        push_ops: bool = True,
         redraw: bool = True,
     ) -> EventDataDict:
         old_total = self.MT.equalize_data_row_lengths()
         total_rows = self.MT.total_data_rows()
         if (idx := idx_param_to_int(idx)) is None:
             idx = old_total
         if isinstance(columns, int):
@@ -2080,24 +2102,26 @@
                 data_ins_col=idx,
                 displayed_ins_col=displayed_ins_idx,
                 numcols=numcols,
                 columns=data,
                 widths=widths,
                 headers=headers,
             ),
+            add_row_positions=add_row_heights,
             event_data=event_dict(
                 name="add_columns",
                 sheet=self.name,
                 boxes=self.MT.get_boxes(),
                 selected=self.MT.selected,
             ),
             create_selections=create_selections,
+            push_ops=push_ops,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return event_data
 
     def del_row(
         self,
@@ -2143,14 +2167,15 @@
         emit_event: bool = False,
         redraw: bool = True,
     ) -> EventDataDict:
         rows = [rows] if isinstance(rows, int) else sorted(rows)
         event_data = event_dict(
             name="delete_rows",
             sheet=self.name,
+            widget=self,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         if not data_indexes:
             event_data = self.MT.delete_rows_displayed(rows, event_data)
             event_data = self.MT.delete_rows_data(
                 rows if self.MT.all_rows_displayed else [self.MT.displayed_rows[r] for r in rows],
@@ -2163,15 +2188,15 @@
                 rows = data_to_displayed_idxs(rows, self.MT.displayed_rows)
             event_data = self.MT.delete_rows_data(rows, event_data)
             event_data = self.MT.delete_rows_displayed(
                 rows,
                 event_data,
             )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.MT.deselect("all", redraw=False)
         self.set_refresh_timer(redraw)
         return event_data
 
     delete_rows = del_rows
@@ -2184,14 +2209,15 @@
         emit_event: bool = False,
         redraw: bool = True,
     ) -> EventDataDict:
         columns = [columns] if isinstance(columns, int) else sorted(columns)
         event_data = event_dict(
             name="delete_columns",
             sheet=self.name,
+            widget=self,
             boxes=self.MT.get_boxes(),
             selected=self.MT.selected,
         )
         if not data_indexes:
             event_data = self.MT.delete_columns_displayed(columns, event_data)
             event_data = self.MT.delete_columns_data(
                 columns if self.MT.all_columns_displayed else [self.MT.displayed_columns[c] for c in columns],
@@ -2204,15 +2230,15 @@
                 columns = data_to_displayed_idxs(columns, self.MT.displayed_columns)
             event_data = self.MT.delete_columns_data(columns, event_data)
             event_data = self.MT.delete_columns_displayed(
                 columns,
                 event_data,
             )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.MT.deselect("all", redraw=False)
         self.set_refresh_timer(redraw)
         return event_data
 
     delete_columns = del_columns
@@ -2292,56 +2318,60 @@
         move_to: int | None = None,
         to_move: list[int] | None = None,
         move_data: bool = True,
         data_indexes: bool = False,
         create_selections: bool = True,
         undo: bool = False,
         emit_event: bool = False,
+        move_heights: bool = True,
         redraw: bool = True,
     ) -> tuple[dict, dict, dict]:
         data_idxs, disp_idxs, event_data = self.MT.move_rows_adjust_options_dict(
             *self.MT.get_args_for_move_rows(
                 move_to=move_to,
                 to_move=to_move,
                 data_indexes=data_indexes,
             ),
             move_data=move_data,
+            move_heights=move_heights,
             create_selections=create_selections,
             data_indexes=data_indexes,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return data_idxs, disp_idxs, event_data
 
     def move_columns(
         self,
         move_to: int | None = None,
         to_move: list[int] | None = None,
         move_data: bool = True,
         data_indexes: bool = False,
         create_selections: bool = True,
         undo: bool = False,
         emit_event: bool = False,
+        move_widths: bool = True,
         redraw: bool = True,
     ) -> tuple[dict, dict, dict]:
         data_idxs, disp_idxs, event_data = self.MT.move_columns_adjust_options_dict(
             *self.MT.get_args_for_move_columns(
                 move_to=move_to,
                 to_move=to_move,
                 data_indexes=data_indexes,
             ),
             move_data=move_data,
+            move_widths=move_widths,
             create_selections=create_selections,
             data_indexes=data_indexes,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return data_idxs, disp_idxs, event_data
 
     def mapping_move_columns(
         self,
@@ -2360,15 +2390,15 @@
             totalcols=None,
             disp_new_idxs=disp_new_idxs,
             move_data=move_data,
             create_selections=create_selections,
             data_indexes=data_indexes,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return data_idxs, disp_idxs, event_data
 
     def mapping_move_rows(
         self,
@@ -2387,15 +2417,15 @@
             totalrows=None,
             disp_new_idxs=disp_new_idxs,
             move_data=move_data,
             create_selections=create_selections,
             data_indexes=data_indexes,
         )
         if undo:
-            self.MT.undo_stack.append(ev_stack_dict(event_data))
+            self.MT.undo_stack.append(pickled_event_dict(event_data))
         if emit_event:
             self.emit_event("<<SheetModified>>", event_data)
         self.set_refresh_timer(redraw)
         return data_idxs, disp_idxs, event_data
 
     def equalize_data_row_lengths(
         self,
@@ -2489,63 +2519,85 @@
             del_from_options(self.MT.row_options, "highlight")
         if columns:
             del_from_options(self.MT.col_options, "highlight")
         if index:
             del_from_options(self.RI.cell_options, "highlight")
         if header:
             del_from_options(self.CH.cell_options, "highlight")
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     # Dropdown Boxes
 
     def dropdown(
         self,
         *key: CreateSpanTypes,
-        **kwargs,
+        values: list = [],
+        edit_data: bool = True,
+        set_values: dict[tuple[int, int], object] = {},
+        set_value: object = None,
+        state: str = "normal",
+        redraw: bool = True,
+        selection_function: Callable | None = None,
+        modified_function: Callable | None = None,
+        search_function: Callable = dropdown_search_function,
+        validate_input: bool = True,
+        text: None | str = None,
     ) -> Span:
-        kwargs = get_dropdown_kwargs(**kwargs)
-        v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
+        v = set_value if set_value is not None else values[0] if values else ""
+        kwargs = {
+            "values": values,
+            "state": state,
+            "selection_function": selection_function,
+            "modified_function": modified_function,
+            "search_function": search_function,
+            "validate_input": validate_input,
+            "text": text,
+        }
         d = get_dropdown_dict(**kwargs)
         span = self.span_from_key(*key)
         rows, cols = self.ranges_from_span(span)
         table, index, header = span.table, span.index, span.header
         set_tdata = self.MT.set_cell_data
         set_idata = self.RI.set_cell_data
         set_hdata = self.CH.set_cell_data
         if index:
             for r in rows:
                 self.del_index_cell_options_dropdown_and_checkbox(r)
                 add_to_options(self.RI.cell_options, r, "dropdown", d)
-                set_idata(r, v)
+                if edit_data:
+                    set_idata(r, value=set_values[r] if r in set_values else v)
         if header:
             for c in cols:
                 self.del_header_cell_options_dropdown_and_checkbox(c)
                 add_to_options(self.CH.cell_options, c, "dropdown", d)
-                set_hdata(c, v)
+                if edit_data:
+                    set_hdata(c, value=set_values[c] if c in set_values else v)
         if table:
             if span.kind == "cell":
                 for r in rows:
                     for c in cols:
                         self.del_cell_options_dropdown_and_checkbox(r, c)
                         add_to_options(self.MT.cell_options, (r, c), "dropdown", d)
-                        set_tdata(r, c, v)
+                        if edit_data:
+                            set_tdata(r, c, value=set_values[(r, c)] if (r, c) in set_values else v)
             elif span.kind == "row":
                 for r in rows:
                     self.del_row_options_dropdown_and_checkbox(r)
                     add_to_options(self.MT.row_options, r, "dropdown", d)
-                    for c in cols:
-                        set_tdata(r, c, v)
+                    if edit_data:
+                        for c in cols:
+                            set_tdata(r, c, value=set_values[(r, c)] if (r, c) in set_values else v)
             elif span.kind == "column":
                 for c in cols:
                     self.del_column_options_dropdown_and_checkbox(c)
                     add_to_options(self.MT.col_options, c, "dropdown", d)
-                    for r in rows:
-                        set_tdata(r, c, v)
-        self.set_refresh_timer(kwargs["redraw"])
+                    if edit_data:
+                        for r in rows:
+                            set_tdata(r, c, value=set_values[(r, c)] if (r, c) in set_values else v)
+        self.set_refresh_timer(redraw)
         return span
 
     def del_dropdown(
         self,
         *key: CreateSpanTypes,
         redraw: bool = True,
     ) -> Span:
@@ -2560,92 +2612,102 @@
         self.set_refresh_timer(redraw)
         return span
 
     def open_dropdown(self, r: int, c: int) -> Sheet:
         self.MT.open_dropdown_window(r, c)
         return self
 
-    def close_dropdown(self, r: int, c: int) -> Sheet:
+    def close_dropdown(self, r: int | None = None, c: int | None = None) -> Sheet:
         self.MT.close_dropdown_window(r, c)
         return self
 
     def open_header_dropdown(self, c: int) -> Sheet:
         self.CH.open_dropdown_window(c)
         return self
 
-    def close_header_dropdown(self, c: int) -> Sheet:
+    def close_header_dropdown(self, c: int | None = None) -> Sheet:
         self.CH.close_dropdown_window(c)
         return self
 
     def open_index_dropdown(self, r: int) -> Sheet:
         self.RI.open_dropdown_window(r)
         return self
 
-    def close_index_dropdown(self, r: int) -> Sheet:
+    def close_index_dropdown(self, r: int | None = None) -> Sheet:
         self.RI.close_dropdown_window(r)
         return self
 
     # Check Boxes
 
     def checkbox(
         self,
         *key: CreateSpanTypes,
-        **kwargs,
+        edit_data: bool = True,
+        checked: bool | None = None,
+        state: str = "normal",
+        redraw: bool = True,
+        check_function: Callable | None = None,
+        text: str = "",
     ) -> Span:
-        kwargs = get_checkbox_kwargs(**kwargs)
-        v = kwargs["checked"]
+        kwargs = {
+            "state": state,
+            "check_function": check_function,
+            "text": text,
+        }
         d = get_checkbox_dict(**kwargs)
         span = self.span_from_key(*key)
         rows, cols = self.ranges_from_span(span)
         table, index, header = span.table, span.index, span.header
         set_tdata = self.MT.set_cell_data
         set_idata = self.RI.set_cell_data
         set_hdata = self.CH.set_cell_data
-        if span.kind == "cell":
-            if header:
-                for c in cols:
-                    self.del_header_cell_options_dropdown_and_checkbox(c)
-                    add_to_options(self.CH.cell_options, c, "checkbox", d)
-                    set_hdata(c, v)
+        if index:
             for r in rows:
-                if index:
-                    self.del_index_cell_options_dropdown_and_checkbox(r)
-                    add_to_options(self.RI.cell_options, r, "checkbox", d)
-                    set_idata(r, v)
-                if table:
+                self.del_index_cell_options_dropdown_and_checkbox(r)
+                add_to_options(self.RI.cell_options, r, "checkbox", d)
+                if edit_data:
+                    set_idata(r, checked if isinstance(checked, bool) else force_bool(self.get_index_data(r)))
+        if header:
+            for c in cols:
+                self.del_header_cell_options_dropdown_and_checkbox(c)
+                add_to_options(self.CH.cell_options, c, "checkbox", d)
+                if edit_data:
+                    set_hdata(c, checked if isinstance(checked, bool) else force_bool(self.get_header_data(c)))
+        if table:
+            if span.kind == "cell":
+                for r in rows:
                     for c in cols:
                         self.MT.delete_cell_format(r, c, clear_values=False)
                         self.del_cell_options_dropdown_and_checkbox(r, c)
                         add_to_options(self.MT.cell_options, (r, c), "checkbox", d)
-                        set_tdata(r, c, v)
-        elif span.kind == "row":
-            for r in rows:
-                if index:
-                    self.del_index_cell_options_dropdown_and_checkbox(r)
-                    add_to_options(self.RI.cell_options, r, "checkbox", d)
-                    set_idata(r, v)
-                if table:
+                        if edit_data:
+                            set_tdata(
+                                r, c, checked if isinstance(checked, bool) else force_bool(self.get_cell_data(r, c))
+                            )
+            elif span.kind == "row":
+                for r in rows:
                     self.MT.delete_row_format(r, clear_values=False)
                     self.del_row_options_dropdown_and_checkbox(r)
                     add_to_options(self.MT.row_options, r, "checkbox", d)
-                    for c in cols:
-                        set_tdata(r, c, v)
-        elif span.kind == "column":
-            for c in cols:
-                if header:
-                    self.del_header_cell_options_dropdown_and_checkbox(c)
-                    add_to_options(self.CH.cell_options, c, "checkbox", d)
-                    set_hdata(c, v)
-                if table:
+                    if edit_data:
+                        for c in cols:
+                            set_tdata(
+                                r, c, checked if isinstance(checked, bool) else force_bool(self.get_cell_data(r, c))
+                            )
+            elif span.kind == "column":
+                for c in cols:
                     self.MT.delete_column_format(c, clear_values=False)
                     self.del_column_options_dropdown_and_checkbox(c)
                     add_to_options(self.MT.col_options, c, "checkbox", d)
-                    for r in rows:
-                        set_tdata(r, c, v)
-        self.set_refresh_timer(kwargs["redraw"])
+                    if edit_data:
+                        for r in rows:
+                            set_tdata(
+                                r, c, checked if isinstance(checked, bool) else force_bool(self.get_cell_data(r, c))
+                            )
+        self.set_refresh_timer(redraw)
         return span
 
     def del_checkbox(
         self,
         *key: CreateSpanTypes,
         redraw: bool = True,
     ) -> Span:
@@ -2838,44 +2900,41 @@
     ) -> str | Sheet:
         if align is None:
             return self.MT.align
         elif convert_align(align):
             self.MT.align = convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def header_align(
         self,
         align: str = None,
         redraw: bool = True,
     ) -> str | Sheet:
         if align is None:
             return self.CH.align
         elif convert_align(align):
             self.CH.align = convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def row_index_align(
         self,
         align: str = None,
         redraw: bool = True,
     ) -> str | Sheet:
         if align is None:
             return self.RI.align
         elif convert_align(align):
             self.RI.align = convert_align(align)
         else:
             raise ValueError("Align must be one of the following values: c, center, w, west, e, east")
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     index_align = row_index_align
 
     def align(
         self,
         *key: CreateSpanTypes,
         align: str | None = None,
@@ -3075,40 +3134,36 @@
 
     def select_row(self, row: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.RI.select_row(
             row if isinstance(row, int) else int(row),
             redraw=False,
             run_binding_func=run_binding_func,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def select_column(self, column: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.CH.select_col(
             column if isinstance(column, int) else int(column),
             redraw=False,
             run_binding_func=run_binding_func,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def select_cell(self, row: int, column: int, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.MT.select_cell(
             row if isinstance(row, int) else int(row),
             column if isinstance(column, int) else int(column),
             redraw=False,
             run_binding_func=run_binding_func,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def select_all(self, redraw: bool = True, run_binding_func: bool = True) -> Sheet:
         self.MT.select_all(redraw=False, run_binding_func=run_binding_func)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def add_cell_selection(
         self,
         row: int,
         column: int,
         redraw: bool = True,
         run_binding_func: bool = True,
@@ -3117,48 +3172,45 @@
         self.MT.add_selection(
             r=row,
             c=column,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def add_row_selection(
         self,
         row: int,
         redraw: bool = True,
         run_binding_func: bool = True,
         set_as_current: bool = True,
     ) -> Sheet:
         self.RI.add_selection(
             r=row,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def add_column_selection(
         self,
         column: int,
         redraw: bool = True,
         run_binding_func: bool = True,
         set_as_current: bool = True,
     ) -> Sheet:
         self.CH.add_selection(
             c=column,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def toggle_select_cell(
         self,
         row: int,
         column: int,
         add_selection: bool = True,
         redraw: bool = True,
@@ -3169,16 +3221,15 @@
             row=row,
             column=column,
             add_selection=add_selection,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def toggle_select_row(
         self,
         row: int,
         add_selection: bool = True,
         redraw: bool = True,
         run_binding_func: bool = True,
@@ -3187,16 +3238,15 @@
         self.RI.toggle_select_row(
             row=row,
             add_selection=add_selection,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def toggle_select_column(
         self,
         column: int,
         add_selection: bool = True,
         redraw: bool = True,
         run_binding_func: bool = True,
@@ -3205,16 +3255,15 @@
         self.CH.toggle_select_col(
             column=column,
             add_selection=add_selection,
             redraw=False,
             run_binding_func=run_binding_func,
             set_as_current=set_as_current,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def create_selection_box(
         self,
         r1: int,
         c1: int,
         r2: int,
         c2: int,
@@ -3230,26 +3279,24 @@
         self,
         row: int | None | Literal["all"] = None,
         column: int | None = None,
         cell: tuple[int, int] | None = None,
         redraw: bool = True,
     ) -> Sheet:
         self.MT.deselect(r=row, c=column, cell=cell, redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def deselect_any(
         self,
         rows: Iterator[int] | int | None,
         columns: Iterator[int] | int | None,
         redraw: bool = True,
     ) -> Sheet:
         self.MT.deselect_any(rows=rows, columns=columns, redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     # Row Heights and Column Widths
 
     def default_column_width(self, width: int | None = None) -> int:
         if isinstance(width, int):
             self.ops.default_column_width = width
         return self.ops.default_column_width
@@ -3268,23 +3315,23 @@
         self,
         row: int,
         column: int,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
     ) -> Sheet:
         self.MT.set_cell_size_to_text(r=row, c=column, only_set_if_too_small=only_set_if_too_small)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def set_all_cell_sizes_to_text(
         self,
         redraw: bool = True,
         width: int | None = None,
+        slim: bool = False,
     ) -> tuple[list[float], list[float]]:
-        self.MT.set_all_cell_sizes_to_text(w=width)
+        self.MT.set_all_cell_sizes_to_text(w=width, slim=slim)
         self.set_refresh_timer(redraw)
         return self.MT.row_positions, self.MT.col_positions
 
     def set_all_column_widths(
         self,
         width: int | None = None,
         only_set_if_too_small: bool = False,
@@ -3292,31 +3339,29 @@
         recreate_selection_boxes: bool = True,
     ) -> Sheet:
         self.CH.set_width_of_all_cols(
             width=width,
             only_set_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def set_all_row_heights(
         self,
         height: int | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
         recreate_selection_boxes: bool = True,
     ) -> Sheet:
         self.RI.set_height_of_all_rows(
             height=height,
             only_set_if_too_small=only_set_if_too_small,
             recreate=recreate_selection_boxes,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def column_width(
         self,
         column: int | Literal["all", "displayed"] | None = None,
         width: int | Literal["default", "text"] | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
@@ -3329,16 +3374,15 @@
                 self.CH.set_col_width(c)
         elif width == "text" and isinstance(column, int):
             self.CH.set_col_width(col=column, width=None, only_set_if_too_small=only_set_if_too_small)
         elif isinstance(width, int) and isinstance(column, int):
             self.CH.set_col_width(col=column, width=width, only_set_if_too_small=only_set_if_too_small)
         elif isinstance(column, int):
             return int(self.MT.col_positions[column + 1] - self.MT.col_positions[column])
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def row_height(
         self,
         row: int | Literal["all", "displayed"] | None = None,
         height: int | Literal["default", "text"] | None = None,
         only_set_if_too_small: bool = False,
         redraw: bool = True,
@@ -3351,16 +3395,15 @@
                 self.RI.set_row_height(r)
         elif height == "text" and isinstance(row, int):
             self.RI.set_row_height(row=row, height=None, only_set_if_too_small=only_set_if_too_small)
         elif isinstance(height, int) and isinstance(row, int):
             self.RI.set_row_height(row=row, height=height, only_set_if_too_small=only_set_if_too_small)
         elif isinstance(row, int):
             return int(self.MT.row_positions[row + 1] - self.MT.row_positions[row])
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def get_column_widths(self, canvas_positions: bool = False) -> list[float]:
         if canvas_positions:
             return self.MT.col_positions
         return self.MT.get_column_widths()
 
     def get_row_heights(self, canvas_positions: bool = False) -> list[float]:
@@ -3402,92 +3445,95 @@
         self.RI.set_width_of_index_to_text(text=text)
         return self
 
     def set_index_width(self, pixels: int, redraw: bool = True) -> Sheet:
         if self.ops.auto_resize_row_index:
             self.ops.auto_resize_row_index = False
         self.RI.set_width(pixels, set_TL=True)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def set_height_of_header_to_text(self, text: None | str = None) -> Sheet:
         self.CH.set_height_of_header_to_text(text=text)
         return self
 
     def set_header_height_pixels(self, pixels: int, redraw: bool = True) -> Sheet:
         self.CH.set_height(pixels, set_TL=True)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def set_header_height_lines(self, nlines: int, redraw: bool = True) -> Sheet:
         self.CH.set_height(
             self.MT.get_lines_cell_height(
                 nlines,
                 font=self.ops.header_font,
             ),
             set_TL=True,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def del_row_position(self, idx: int, deselect_all: bool = False) -> Sheet:
         self.MT.del_row_position(idx=idx, deselect_all=deselect_all)
         return self
 
     delete_row_position = del_row_position
 
+    def del_row_positions(self, idxs: Iterator[int] | None = None) -> Sheet:
+        self.MT.del_row_positions(idxs=idxs)
+        self.set_refresh_timer()
+        return self
+
     def del_column_position(self, idx: int, deselect_all: bool = False) -> Sheet:
         self.MT.del_col_position(idx, deselect_all=deselect_all)
         return self
 
     delete_column_position = del_column_position
 
+    def del_column_positions(self, idxs: Iterator[int] | None = None) -> Sheet:
+        self.MT.del_col_positions(idxs=idxs)
+        self.set_refresh_timer()
+        return self
+
     def insert_column_position(
         self,
         idx: Literal["end"] | int = "end",
         width: int | None = None,
         deselect_all: bool = False,
         redraw: bool = False,
     ) -> Sheet:
         self.MT.insert_col_position(idx=idx, width=width, deselect_all=deselect_all)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def insert_row_position(
         self,
         idx: Literal["end"] | int = "end",
         height: int | None = None,
         deselect_all: bool = False,
         redraw: bool = False,
     ) -> Sheet:
         self.MT.insert_row_position(idx=idx, height=height, deselect_all=deselect_all)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def insert_column_positions(
         self,
         idx: Literal["end"] | int = "end",
         widths: Sequence[float] | int | None = None,
         deselect_all: bool = False,
         redraw: bool = False,
     ) -> Sheet:
         self.MT.insert_col_positions(idx=idx, widths=widths, deselect_all=deselect_all)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def insert_row_positions(
         self,
         idx: Literal["end"] | int = "end",
         heights: Sequence[float] | int | None = None,
         deselect_all: bool = False,
         redraw: bool = False,
     ) -> Sheet:
         self.MT.insert_row_positions(idx=idx, heights=heights, deselect_all=deselect_all)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def sheet_display_dimensions(
         self,
         total_rows: int | None = None,
         total_columns: int | None = None,
     ) -> tuple[int, int] | Sheet:
         if total_rows is None and total_columns is None:
@@ -3542,14 +3588,28 @@
                 x - z < self.MT.min_column_width or not isinstance(x, int) or isinstance(x, bool)
                 for z, x in zip(islice(column_widths, 0, None), islice(column_widths, 1, None))
             )
         return not any(
             z < self.MT.min_column_width or not isinstance(z, int) or isinstance(z, bool) for z in column_widths
         )
 
+    def valid_row_height(self, height: int) -> int:
+        if height < self.MT.min_row_height:
+            return self.MT.min_row_height
+        elif height > self.MT.max_row_height:
+            return self.MT.max_row_height
+        return height
+
+    def valid_column_width(self, width: int) -> int:
+        if width < self.MT.min_column_width:
+            return self.MT.min_column_width
+        elif width > self.MT.max_column_width:
+            return self.MT.max_column_width
+        return width
+
     # Identifying Bound Event Mouse Position
 
     def identify_region(self, event: object) -> Literal["table", "index", "header", "top left"]:
         if event.widget == self.MT:
             return "table"
         elif event.widget == self.RI:
             return "index"
@@ -3629,16 +3689,15 @@
             column,
             keep_yscroll,
             keep_xscroll,
             bottom_right_corner,
             check_cell_visibility=check_cell_visibility,
             redraw=False,
         )
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def cell_visible(self, r: int, c: int) -> bool:
         return self.MT.cell_visible(r, c)
 
     def cell_completely_visible(self, r: int, c: int, seperate_axes: bool = False) -> bool:
         return self.MT.cell_completely_visible(r, c, seperate_axes)
 
@@ -3740,16 +3799,15 @@
                 itr=self.MT.gen_column_widths,
                 to_pop=to_pop,
                 save_to=self.MT.saved_column_widths,
             ),
         )
         if deselect_all:
             self.MT.deselect(redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     # uses data indexes
     def show_columns(
         self,
         columns: int | Iterator[int],
         redraw: bool = True,
         deselect_all: bool = True,
@@ -3761,16 +3819,15 @@
             idx = bisect_left(self.MT.displayed_columns, column)
             if len(self.MT.displayed_columns) == idx or self.MT.displayed_columns[idx] != column:
                 self.MT.displayed_columns.insert(idx, column)
                 cws.insert(idx, self.MT.saved_column_widths.pop(column, self.PAR.ops.default_column_width))
         self.MT.set_col_positions(cws)
         if deselect_all:
             self.MT.deselect(redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def all_columns_displayed(self, a: bool | None = None) -> bool:
         v = bool(self.MT.all_columns_displayed)
         if isinstance(a, bool):
             self.MT.all_columns_displayed = a
         return v
 
@@ -3824,14 +3881,15 @@
 
     def hide_rows(
         self,
         rows: int | set[int] | Iterator[int],
         redraw: bool = True,
         deselect_all: bool = True,
         data_indexes: bool = False,
+        row_heights: bool = True,
     ) -> Sheet:
         if isinstance(rows, int):
             rows = {rows}
         elif not isinstance(rows, set):
             rows = set(rows)
             if not rows:
                 return
@@ -3851,25 +3909,25 @@
                 for i, r in enumerate(self.MT.displayed_rows):
                     if i not in rows:
                         new_disp.append(r)
                     else:
                         to_pop[i] = r
             self.MT.displayed_rows = new_disp
         self.MT.all_rows_displayed = False
-        self.MT.set_row_positions(
-            pop_positions(
-                itr=self.MT.gen_row_heights,
-                to_pop=to_pop,
-                save_to=self.MT.saved_row_heights,
-            ),
-        )
+        if row_heights:
+            self.MT.set_row_positions(
+                pop_positions(
+                    itr=self.MT.gen_row_heights,
+                    to_pop=to_pop,
+                    save_to=self.MT.saved_row_heights,
+                ),
+            )
         if deselect_all:
             self.MT.deselect(redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     # uses data indexes
     def show_rows(
         self,
         rows: int | Iterator[int],
         redraw: bool = True,
         deselect_all: bool = True,
@@ -3881,16 +3939,15 @@
             idx = bisect_left(self.MT.displayed_rows, row)
             if len(self.MT.displayed_rows) == idx or self.MT.displayed_rows[idx] != row:
                 self.MT.displayed_rows.insert(idx, row)
                 rhs.insert(idx, self.MT.saved_row_heights.pop(row, self.MT.get_default_row_height()))
         self.MT.set_row_positions(rhs)
         if deselect_all:
             self.MT.deselect(redraw=False)
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def all_rows_displayed(self, a: bool | None = None) -> bool:
         v = bool(self.MT.all_rows_displayed)
         if isinstance(a, bool):
             self.MT.all_rows_displayed = a
         return v
 
@@ -4069,15 +4126,17 @@
         text: str = "",
     ) -> Sheet:
         if self.CH.text_editor.open:
             self.CH.text_editor.window.set_text(text)
         return self
 
     def destroy_text_editor(self, event: object = None) -> Sheet:
-        self.MT.hide_text_editor(event=event)
+        self.MT.hide_text_editor(reason=event)
+        self.RI.hide_text_editor(reason=event)
+        self.CH.hide_text_editor(reason=event)
         return self
 
     def get_text_editor_widget(self, event: object = None) -> tk.Text | None:
         try:
             return self.MT.text_editor.tktext
         except Exception:
             return None
@@ -4103,25 +4162,33 @@
                 pass
         return self
 
     def get_text_editor_value(self) -> str | None:
         return self.MT.text_editor.get()
 
     def close_text_editor(self, set_data: bool = True) -> Sheet:
+        event = new_tk_event("ButtonPress-1" if set_data else "Escape")
         if self.MT.text_editor.open:
-            event = ("ButtonPress-1",) if set_data else ("Escape",)
-            self.MT.close_text_editor(editor_info=self.MT.text_editor.coords + event)
+            self.MT.close_text_editor(event=event)
+        if self.RI.text_editor.open:
+            self.RI.close_text_editor(event=event)
+        if self.CH.text_editor.open:
+            self.CH.close_text_editor(event=event)
         return self
 
     # Sheet Options and Other Functions
 
     def set_options(self, redraw: bool = True, **kwargs) -> Sheet:
         for k, v in kwargs.items():
             if k in self.ops and v != self.ops[k]:
+                if k.endswith("bindings"):
+                    self.MT._disable_binding(k.split("_")[0])
                 self.ops[k] = v
+                if k.endswith("bindings"):
+                    self.MT._enable_binding(k.split("_")[0])
         if "from_clipboard_delimiters" in kwargs:
             self.ops.from_clipboard_delimiters = (
                 self.ops.from_clipboard_delimiters
                 if isinstance(self.ops.from_clipboard_delimiters, str)
                 else "".join(self.ops.from_clipboard_delimiters)
             )
         if "default_row_height" in kwargs:
@@ -4134,18 +4201,21 @@
             self.MT.max_column_width = float(kwargs["max_column_width"])
         if "max_row_height" in kwargs:
             self.MT.max_row_height = float(kwargs["max_row_height"])
         if "max_header_height" in kwargs:
             self.MT.max_header_height = float(kwargs["max_header_height"])
         if "max_index_width" in kwargs:
             self.MT.max_index_width = float(kwargs["max_index_width"])
+        if "expand_sheet_if_paste_too_big" in kwargs:
+            self.ops.paste_can_expand_x = kwargs["expand_sheet_if_paste_too_big"]
+            self.ops.paste_can_expand_y = kwargs["expand_sheet_if_paste_too_big"]
         if "font" in kwargs:
             self.MT.set_table_font(kwargs["font"])
         elif "table_font" in kwargs:
-            self.MT.set_table_font(kwargs["font"])
+            self.MT.set_table_font(kwargs["table_font"])
         if "header_font" in kwargs:
             self.MT.set_header_font(kwargs["header_font"])
         if "index_font" in kwargs:
             self.MT.set_index_font(kwargs["index_font"])
         if "theme" in kwargs:
             self.change_theme(kwargs["theme"])
         if "header_bg" in kwargs:
@@ -4168,17 +4238,15 @@
             self.config(
                 highlightbackground=kwargs["outline_color"],
                 highlightcolor=kwargs["outline_color"],
             )
         if any(k in kwargs for k in scrollbar_options_keys):
             self.set_scrollbar_options()
         self.MT.create_rc_menus()
-        self.MT.key_bindings()
-        self.set_refresh_timer(redraw)
-        return self
+        return self.set_refresh_timer(redraw)
 
     def set_scrollbar_options(self) -> Sheet:
         style = ttk.Style()
         for orientation in ("vertical", "horizontal"):
             style.configure(
                 f"Sheet{self.unique_id}.{orientation.capitalize()}.TScrollbar",
                 background=self.ops[f"{orientation}_scroll_background"],
@@ -4235,35 +4303,35 @@
             target = self.MT.cell_options
         elif canvas == "row_index":
             target = self.RI.cell_options
         elif canvas == "header":
             target = self.CH.cell_options
         if key is None:
             return target
-        return {k: v for k, v in target.items() if key in v}
+        return {k: v[key] for k, v in target.items() if key in v}
 
     def get_row_options(self, key: None | str = None) -> dict:
         if key is None:
             return self.MT.row_options
-        return {k: v for k, v in self.MT.row_options.items() if key in v}
+        return {k: v[key] for k, v in self.MT.row_options.items() if key in v}
 
     def get_column_options(self, key: None | str = None) -> dict:
         if key is None:
             return self.MT.col_options
-        return {k: v for k, v in self.MT.col_options.items() if key in v}
+        return {k: v[key] for k, v in self.MT.col_options.items() if key in v}
 
     def get_index_options(self, key: None | str = None) -> dict:
         if key is None:
             return self.RI.cell_options
-        return {k: v for k, v in self.RI.cell_options.items() if key in v}
+        return {k: v[key] for k, v in self.RI.cell_options.items() if key in v}
 
     def get_header_options(self, key: None | str = None) -> dict:
         if key is None:
             return self.CH.cell_options
-        return {k: v for k, v in self.CH.cell_options.items() if key in v}
+        return {k: v[key] for k, v in self.CH.cell_options.items() if key in v}
 
     def del_out_of_bounds_options(self) -> Sheet:
         maxc = self.total_columns()
         maxr = self.total_rows()
         for name in tuple(self.MT.named_spans):
             span = self.MT.named_spans[name]
             if (
@@ -4456,37 +4524,47 @@
 
     def tree_build(
         self,
         data: list[list[object]],
         iid_column: int,
         parent_column: int,
         text_column: None | int = None,
+        push_ops: bool = False,
+        row_heights: Sequence[int] | None | False = None,
+        open_ids: Iterator[str] | None = None,
+        safety: bool = True,
+        ncols: int | None = None,
     ) -> Sheet:
+        self.reset(cell_options=False, column_widths=False, header=False, redraw=False)
         if text_column is None:
             text_column = iid_column
         tally_of_ids = defaultdict(lambda: -1)
-        ncols = max(map(len, data), default=0)
+        if not isinstance(ncols, int):
+            ncols = max(map(len, data), default=0)
         for rn, row in enumerate(data):
-            if ncols > (lnr := len(row)):
+            if safety and ncols > (lnr := len(row)):
                 row += self.MT.get_empty_row_seq(rn, end=ncols, start=lnr)
             iid, pid = row[iid_column].lower(), row[parent_column].lower()
-            if not iid:
-                continue
-            tally_of_ids[iid] += 1
-            if tally_of_ids[iid] > 0:
-                x = 1
-                while iid in tally_of_ids:
-                    new = f"{row[iid_column]}_DUPLICATED_{x}"
-                    iid = new.lower()
-                    x += 1
+            if safety:
+                if not iid:
+                    continue
                 tally_of_ids[iid] += 1
-                row[iid_column] = new
-            if iid not in self.RI.tree:
+                if tally_of_ids[iid] > 0:
+                    x = 1
+                    while iid in tally_of_ids:
+                        new = f"{row[iid_column]}_DUPLICATED_{x}"
+                        iid = new.lower()
+                        x += 1
+                    tally_of_ids[iid] += 1
+                    row[iid_column] = new
+            if iid in self.RI.tree:
+                self.RI.tree[iid].text = row[text_column]
+            else:
                 self.RI.tree[iid] = Node(row[text_column], iid, "")
-            if iid == pid or self.RI.pid_causes_recursive_loop(iid, pid):
+            if safety and (iid == pid or self.RI.pid_causes_recursive_loop(iid, pid)):
                 row[parent_column] = ""
                 pid = ""
             if pid:
                 if pid not in self.RI.tree:
                     self.RI.tree[pid] = Node(row[text_column], pid)
                 self.RI.tree[iid].parent = self.RI.tree[pid]
                 self.RI.tree[pid].children.append(self.RI.tree[iid])
@@ -4497,83 +4575,131 @@
             if n.parent is None:
                 n.parent = ""
                 newrow = self.MT.get_empty_row_seq(len(data), ncols)
                 newrow[iid_column] = n.iid
                 self.RI.tree_rns[n.iid] = len(data)
                 data.append(newrow)
         self.insert_rows(
-            idx=0,
             rows=[[self.RI.tree[iid]] + data[self.RI.tree_rns[iid]] for iid in self.get_children()],
+            idx=0,
+            heights={} if row_heights is False else row_heights,
             row_index=True,
             create_selections=False,
             fill=False,
+            push_ops=push_ops,
         )
+        self.MT.all_rows_displayed = False
+        self.MT.displayed_rows = list(range(len(self.MT._row_index)))
         self.RI.tree_rns = {n.iid: i for i, n in enumerate(self.MT._row_index)}
-        self.hide_rows(
-            set(self.RI.tree_rns[iid] for iid in self.get_children() if self.RI.tree[iid].parent),
-            deselect_all=False,
-            data_indexes=True,
-        )
+        if open_ids:
+            self.tree_set_open(open_ids=open_ids)
+        else:
+            self.hide_rows(
+                {self.RI.tree_rns[iid] for iid in self.get_children() if self.RI.tree[iid].parent},
+                deselect_all=False,
+                data_indexes=True,
+                row_heights=False if row_heights is False else True,
+            )
         return self
 
     def tree_reset(self) -> Sheet:
         self.deselect()
         self.RI.tree_reset()
         return self
 
     def tree_get_open(self) -> set[str]:
         """
         Returns the set[str] of iids that are open in the treeview
         """
         return self.RI.tree_open_ids
 
-    def tree_set_open(self, open_ids: set[str]) -> Sheet:
+    def tree_set_open(self, open_ids: Iterator[str]) -> Sheet:
         """
         Accepts set[str] of iids that are open in the treeview
         Closes everything else
         """
-        self.RI.tree_open_ids = open_ids if isinstance(open_ids, set) else set(open_ids)
         self.hide_rows(
-            set(self.MT.displayed_rows),
+            set(rn for rn in self.MT.displayed_rows if self.MT._row_index[rn].parent),
             redraw=False,
             deselect_all=False,
             data_indexes=True,
         )
-        self.show_rows(
-            (self.RI.tree_rns[iid] for iid in self.get_children("")),
-            redraw=False,
-            deselect_all=True,
-        )
+        open_ids = set(filter(self.exists, map(str.lower, open_ids)))
+        self.RI.tree_open_ids = set()
         if open_ids:
-            self.tree_open(*open_ids)
-        return self
+            to_open = self._tree_open(open_ids)
+            self.show_rows(
+                rows=to_open,
+                redraw=False,
+                deselect_all=False,
+            )
+        return self.set_refresh_timer(True)
 
-    def tree_open(self, *items) -> Sheet:
+    def _tree_open(self, items: set[str]) -> list[int]:
+        """
+        Only meant for internal use
+        """
+        to_open = []
+        disp_set = set(self.MT.displayed_rows)
+        quick_rns = self.RI.tree_rns
+        quick_open_ids = self.RI.tree_open_ids
+        for item in filter(items.__contains__, self.get_children()):
+            if self.RI.tree[item].children:
+                quick_open_ids.add(item)
+                if quick_rns[item] in disp_set:
+                    to_disp = [quick_rns[did] for did in self.RI.get_iid_descendants(item, check_open=True)]
+                    for i in to_disp:
+                        disp_set.add(i)
+                    to_open.extend(to_disp)
+        return to_open
+
+    def tree_open(self, *items, redraw: bool = True) -> Sheet:
         """
         If used without args all items are opened
         """
-        if items:
-            for item in unpack(items):
-                self.item(item, open_=True)
+        if items := set(unpack(items)):
+            to_open = self._tree_open(items)
         else:
-            for item in self.get_children():
-                self.item(item, open_=True)
-        return self
+            to_open = self._tree_open(set(self.get_children()))
+        return self.show_rows(
+            rows=to_open,
+            redraw=redraw,
+            deselect_all=False,
+        )
 
-    def tree_close(self, *items) -> Sheet:
+    def _tree_close(self, items: Iterator[str]) -> list[int]:
+        """
+        Only meant for internal use
+        """
+        to_close = set()
+        disp_set = set(self.MT.displayed_rows)
+        quick_rns = self.RI.tree_rns
+        quick_open_ids = self.RI.tree_open_ids
+        for item in items:
+            if self.RI.tree[item].children:
+                quick_open_ids.discard(item)
+                if quick_rns[item] in disp_set:
+                    for did in self.RI.get_iid_descendants(item, check_open=True):
+                        to_close.add(quick_rns[did])
+        return to_close
+
+    def tree_close(self, *items, redraw: bool = True) -> Sheet:
         """
         If used without args all items are closed
         """
         if items:
-            for item in unpack(items):
-                self.item(item, open_=False)
+            to_close = self._tree_close(unpack(items))
         else:
-            for item in self.get_children():
-                self.item(item, open_=False)
-        return self
+            to_close = self._tree_close(self.get_children())
+        return self.hide_rows(
+            rows=to_close,
+            redraw=redraw,
+            deselect_all=False,
+            data_indexes=True,
+        )
 
     def insert(
         self,
         parent: str = "",
         index: None | int | Literal["end"] = None,
         iid: None | str = None,
         text: None | str = None,
@@ -4593,17 +4719,14 @@
             raise ValueError(f"iid '{iid}' cannot be equal to parent '{pid}'.")
         if pid and pid not in self.RI.tree:
             raise ValueError(f"parent '{parent}' does not exist.")
         if text is None:
             text = iid
         parent_node = self.RI.tree[pid] if parent else ""
         self.RI.tree[iid] = Node(text, iid, parent_node)
-        if self.RI.pid_causes_recursive_loop(iid, pid):
-            del self.RI.tree[iid]
-            raise ValueError(f"iid '{iid}' causes a recursive loop with parent '{parent}'.")
         if parent_node:
             if isinstance(index, int):
                 idx = self.RI.tree_rns[pid] + index + 1
                 for count, cid in enumerate(self.get_children(pid)):
                     if count >= index:
                         break
                     idx += sum(1 for _ in self.RI.get_iid_descendants(cid))
@@ -4662,32 +4785,33 @@
             self.RI.tree[item].text = text
         if isinstance(values, list):
             self.set_data(self.RI.tree_rns[item], data=values)
         if isinstance(open_, bool):
             if self.RI.tree[item].children:
                 if open_:
                     self.RI.tree_open_ids.add(item)
-                    self.show_rows(
-                        (self.RI.tree_rns[did] for did in self.RI.get_iid_descendants(item, check_open=True)),
-                        redraw=False,
-                        deselect_all=False,
-                    )
+                    if self.item_displayed(item):
+                        self.show_rows(
+                            rows=(self.RI.tree_rns[did] for did in self.RI.get_iid_descendants(item, check_open=True)),
+                            redraw=False,
+                            deselect_all=False,
+                        )
                 else:
                     self.RI.tree_open_ids.discard(item)
-                    rows = {self.RI.tree_rns[did] for did in self.RI.get_iid_descendants(item, check_open=True)}
-                    self.hide_rows(
-                        rows,
-                        redraw=False,
-                        deselect_all=False,
-                        data_indexes=True,
-                    )
+                    if self.item_displayed(item):
+                        self.hide_rows(
+                            rows={self.RI.tree_rns[did] for did in self.RI.get_iid_descendants(item, check_open=True)},
+                            redraw=False,
+                            deselect_all=False,
+                            data_indexes=True,
+                        )
             else:
                 self.RI.tree_open_ids.discard(item)
         get = not (isinstance(iid, str) or isinstance(text, str) or isinstance(values, list) or isinstance(open_, bool))
-        self.set_refresh_timer(redraw=not get or redraw)
+        self.set_refresh_timer(redraw=not get and redraw)
         if get:
             return DotDict(
                 text=self.RI.tree[item].text,
                 values=self[self.RI.tree_rns[item]].options(ndim=1).data,
                 open_=item in self.RI.tree_open_ids,
             )
         return self
@@ -4695,20 +4819,20 @@
     def itemrow(self, item: str) -> int:
         try:
             return self.RI.tree_rns[item.lower()]
         except Exception:
             raise ValueError(f"item '{item.lower()}' does not exist.")
 
     def rowitem(self, row: int, data_index: bool = False) -> str | None:
-        if isinstance(row, int):
-            if not data_index:
-                row = self.data_r(row)
-            if len(self.MT._row_index) > row:
+        try:
+            if data_index:
                 return self.MT._row_index[row].iid
-        return None
+            return self.MT._row_index[self.MT.displayed_rows[row]].iid
+        except Exception:
+            return None
 
     def get_children(self, item: None | str = None) -> Generator[str]:
         if item is None:
             for n in self.RI.tree.values():
                 if not n.parent:
                     yield n.iid
                     for iid in self.RI.get_iid_descendants(n.iid):
@@ -4929,30 +5053,33 @@
                 add.append(item)
         self.selection_remove(*remove)
         self.selection_add(*add)
         return self
 
     # Functions not in docs
 
+    def event_generate(self, *args, **kwargs):
+        self.MT.event_generate(*args, **kwargs)
+
     def emit_event(
         self,
         event: str,
-        data: None | dict = None,
+        data: EventDataDict | None = None,
     ) -> None:
-        # data is a EventDataDict
         if data is None:
             data = EventDataDict()
         data["sheetname"] = self.name
         self.last_event_data = data
         for func in self.bound_events[event]:
             func(data)
 
-    def set_refresh_timer(self, redraw: bool = True) -> None:
+    def set_refresh_timer(self, redraw: bool = True) -> Sheet:
         if redraw and self.after_redraw_id is None:
             self.after_redraw_id = self.after(self.after_redraw_time_ms, self.after_redraw)
+        return self
 
     def after_redraw(self) -> None:
         self.MT.main_table_redraw_grid_and_text(redraw_header=True, redraw_row_index=True)
         self.after_redraw_id = None
 
     def del_options_using_span(
         self,
@@ -5193,39 +5320,39 @@
 
     def data_reference(
         self,
         newdataref=None,
         reset_col_positions: bool = True,
         reset_row_positions: bool = True,
         redraw: bool = True,
-    ):
+    ) -> object:
         self.set_refresh_timer(redraw)
         return self.MT.data_reference(newdataref, reset_col_positions, reset_row_positions)
 
     def set_cell_data(
         self,
         r: int,
         c: int,
         value: object = "",
         redraw: bool = True,
         keep_formatting: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if not keep_formatting:
             self.MT.delete_cell_format(r, c, clear_values=False)
         self.MT.set_cell_data(r, c, value)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def set_row_data(
         self,
         r: int,
         values=tuple(),
         add_columns: bool = True,
         redraw: bool = True,
         keep_formatting: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if r >= len(self.MT.data):
             raise Exception("Row number is out of range")
         if not keep_formatting:
             self.MT.delete_row_format(r, clear_values=False)
         maxidx = len(self.MT.data[r]) - 1
         if not values:
             self.MT.data[r] = self.MT.get_empty_row_seq(r, len(self.MT.data[r]))
@@ -5240,24 +5367,24 @@
                         self.set_cell_data(r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
             else:
                 for c, v in enumerate(values):
                     if c > maxidx:
                         self.MT.data[r].append(v)
                     else:
                         self.set_cell_data(r=r, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def set_column_data(
         self,
         c: int,
         values=tuple(),
         add_rows: bool = True,
         redraw: bool = True,
         keep_formatting: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if not keep_formatting:
             self.MT.delete_column_format(c, clear_values=False)
         if add_rows:
             maxidx = len(self.MT.data) - 1
             total_cols = None
             height = self.MT.get_default_row_height()
             for rn, v in enumerate(values):
@@ -5272,66 +5399,66 @@
                     self.MT.fix_row_len(rn, c)
                 self.set_cell_data(r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
         else:
             for rn, v in enumerate(values):
                 if c >= len(self.MT.data[rn]):
                     self.MT.fix_row_len(rn, c)
                 self.set_cell_data(r=rn, c=c, value=v, redraw=False, keep_formatting=keep_formatting)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def readonly_rows(
         self,
         rows: list | int = [],
         readonly: bool = True,
         redraw: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(rows, int):
             rows = [rows]
         else:
             rows = rows
         if not readonly:
             for r in rows:
                 if r in self.MT.row_options and "readonly" in self.MT.row_options[r]:
                     del self.MT.row_options[r]["readonly"]
         else:
             for r in rows:
                 if r not in self.MT.row_options:
                     self.MT.row_options[r] = {}
                 self.MT.row_options[r]["readonly"] = True
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def readonly_columns(
         self,
         columns: list | int = [],
         readonly: bool = True,
         redraw: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(columns, int):
             columns = [columns]
         else:
             columns = columns
         if not readonly:
             for c in columns:
                 if c in self.MT.col_options and "readonly" in self.MT.col_options[c]:
                     del self.MT.col_options[c]["readonly"]
         else:
             for c in columns:
                 if c not in self.MT.col_options:
                     self.MT.col_options[c] = {}
                 self.MT.col_options[c]["readonly"] = True
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def readonly_cells(
         self,
         row: int = 0,
         column: int = 0,
         cells: list = [],
         readonly: bool = True,
         redraw: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if not readonly:
             if cells:
                 for r, c in cells:
                     if (r, c) in self.MT.cell_options and "readonly" in self.MT.cell_options[(r, c)]:
                         del self.MT.cell_options[(r, c)]["readonly"]
             else:
                 if (
@@ -5345,39 +5472,39 @@
                     if (r, c) not in self.MT.cell_options:
                         self.MT.cell_options[(r, c)] = {}
                     self.MT.cell_options[(r, c)]["readonly"] = True
             else:
                 if (row, column) not in self.MT.cell_options:
                     self.MT.cell_options[(row, column)] = {}
                 self.MT.cell_options[(row, column)]["readonly"] = True
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def readonly_header(
         self,
         columns: list = [],
         readonly: bool = True,
         redraw: bool = False,
-    ) -> None:
+    ) -> Sheet:
         self.CH.readonly_header(columns=columns, readonly=readonly)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def readonly_index(
         self,
         rows: list = [],
         readonly: bool = True,
         redraw: bool = False,
-    ) -> None:
+    ) -> Sheet:
         self.RI.readonly_index(rows=rows, readonly=readonly)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def dehighlight_rows(
         self,
         rows: list[int] | Literal["all"] = [],
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(rows, int):
             rows = [rows]
         if not rows or rows == "all":
             for r in self.MT.row_options:
                 if "highlight" in self.MT.row_options[r]:
                     del self.MT.row_options[r]["highlight"]
 
@@ -5390,21 +5517,21 @@
                     del self.MT.row_options[r]["highlight"]
                 except Exception:
                     pass
                 try:
                     del self.RI.cell_options[r]["highlight"]
                 except Exception:
                     pass
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def dehighlight_columns(
         self,
         columns: list[int] | Literal["all"] = [],
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(columns, int):
             columns = [columns]
         if not columns or columns == "all":
             for c in self.MT.col_options:
                 if "highlight" in self.MT.col_options[c]:
                     del self.MT.col_options[c]["highlight"]
 
@@ -5417,104 +5544,114 @@
                     del self.MT.col_options[c]["highlight"]
                 except Exception:
                     pass
                 try:
                     del self.CH.cell_options[c]["highlight"]
                 except Exception:
                     pass
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def highlight_rows(
         self,
         rows: Iterator[int] | int,
         bg: None | str = None,
         fg: None | str = None,
         highlight_index: bool = True,
         redraw: bool = True,
         end_of_screen: bool = False,
         overwrite: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if bg is None and fg is None:
             return
         for r in (rows,) if isinstance(rows, int) else rows:
             add_highlight(self.MT.row_options, r, bg, fg, end_of_screen, overwrite)
         if highlight_index:
             self.highlight_cells(cells=rows, canvas="index", bg=bg, fg=fg, redraw=False)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def highlight_columns(
         self,
         columns: Iterator[int] | int,
         bg: bool | None | str = False,
         fg: bool | None | str = False,
         highlight_header: bool = True,
         redraw: bool = True,
         overwrite: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if bg is False and fg is False:
             return
         for c in (columns,) if isinstance(columns, int) else columns:
             add_highlight(self.MT.col_options, c, bg, fg, None, overwrite)
         if highlight_header:
             self.highlight_cells(cells=columns, canvas="header", bg=bg, fg=fg, redraw=False)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def highlight_cells(
         self,
-        row: int = 0,
-        column: int = 0,
-        cells: list = [],
+        row: int | Literal["all"] = 0,
+        column: int | Literal["all"] = 0,
+        cells: list[tuple[int, int]] = [],
         canvas: Literal["table", "index", "header"] = "table",
         bg: bool | None | str = False,
         fg: bool | None | str = False,
         redraw: bool = True,
         overwrite: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if bg is False and fg is False:
             return
         if canvas == "table":
             if cells:
                 for r_, c_ in cells:
                     add_highlight(self.MT.cell_options, (r_, c_), bg, fg, None, overwrite)
             else:
-                if isinstance(row, str) and row.lower() == "all" and isinstance(column, int):
-                    riter = range(self.MT.total_data_rows())
-                    citer = (column,)
+                if (
+                    isinstance(row, str)
+                    and row.lower() == "all"
+                    and isinstance(column, str)
+                    and column.lower() == "all"
+                ):
+                    totalrows, totalcols = self.MT.total_data_rows(), self.MT.total_data_cols()
+                    for r_ in range(totalrows):
+                        for c_ in range(totalcols):
+                            add_highlight(self.MT.cell_options, (r_, c_), bg, fg, None, overwrite)
+                elif isinstance(row, str) and row.lower() == "all" and isinstance(column, int):
+                    for r_ in range(self.MT.total_data_rows()):
+                        add_highlight(self.MT.cell_options, (r_, column), bg, fg, None, overwrite)
                 elif isinstance(column, str) and column.lower() == "all" and isinstance(row, int):
-                    riter = (row,)
-                    citer = range(self.MT.total_data_cols())
+                    for c_ in range(self.MT.total_data_cols()):
+                        add_highlight(self.MT.cell_options, (row, c_), bg, fg, None, overwrite)
                 elif isinstance(row, int) and isinstance(column, int):
-                    riter = (row,)
-                    citer = (column,)
-                for r_ in riter:
-                    for c_ in citer:
-                        add_highlight(self.MT.cell_options, (r_, c_), bg, fg, None, overwrite)
+                    add_highlight(self.MT.cell_options, (row, column), bg, fg, None, overwrite)
         elif canvas in ("row_index", "index"):
-            iterable = (
-                cells if (cells and not isinstance(cells, int)) else (cells,) if isinstance(cells, int) else (row,)
-            )
-            for r_ in iterable:
-                add_highlight(self.RI.cell_options, r_, bg, fg, None, overwrite)
+            if isinstance(cells, int):
+                add_highlight(self.RI.cell_options, cells, bg, fg, None, overwrite)
+            elif cells:
+                for r_ in cells:
+                    add_highlight(self.RI.cell_options, r_, bg, fg, None, overwrite)
+            else:
+                add_highlight(self.RI.cell_options, row, bg, fg, None, overwrite)
         elif canvas == "header":
-            iterable = (
-                cells if (cells and not isinstance(cells, int)) else (cells,) if isinstance(cells, int) else (column,)
-            )
-            for c_ in iterable:
-                add_highlight(self.CH.cell_options, c_, bg, fg, None, overwrite)
-        self.set_refresh_timer(redraw)
+            if isinstance(cells, int):
+                add_highlight(self.CH.cell_options, cells, bg, fg, None, overwrite)
+            elif cells:
+                for c_ in cells:
+                    add_highlight(self.CH.cell_options, c_, bg, fg, None, overwrite)
+            else:
+                add_highlight(self.CH.cell_options, column, bg, fg, None, overwrite)
+        return self.set_refresh_timer(redraw)
 
     def dehighlight_cells(
         self,
         row: int | Literal["all"] = 0,
         column: int = 0,
         cells: list[tuple[int, int]] = [],
         canvas: Literal["table", "row_index", "header"] = "table",
         all_: bool = False,
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if row == "all" and canvas == "table":
             for k, v in self.MT.cell_options.items():
                 if "highlight" in v:
                     del self.MT.cell_options[k]["highlight"]
         elif row == "all" and canvas == "row_index":
             for k, v in self.RI.cell_options.items():
                 if "highlight" in v:
@@ -5525,15 +5662,15 @@
                     del self.CH.cell_options[k]["highlight"]
         if canvas == "table":
             if cells and not all_:
                 for t in cells:
                     try:
                         del self.MT.cell_options[t]["highlight"]
                     except Exception:
-                        pass
+                        continue
             elif not all_:
                 if (
                     row,
                     column,
                 ) in self.MT.cell_options and "highlight" in self.MT.cell_options[(row, column)]:
                     del self.MT.cell_options[(row, column)]["highlight"]
             elif all_:
@@ -5542,37 +5679,37 @@
                         del self.MT.cell_options[k]["highlight"]
         elif canvas == "row_index":
             if cells and not all_:
                 for r in cells:
                     try:
                         del self.RI.cell_options[r]["highlight"]
                     except Exception:
-                        pass
+                        continue
             elif not all_:
                 if row in self.RI.cell_options and "highlight" in self.RI.cell_options[row]:
                     del self.RI.cell_options[row]["highlight"]
             elif all_:
                 for r in self.RI.cell_options:
                     if "highlight" in self.RI.cell_options[r]:
                         del self.RI.cell_options[r]["highlight"]
         elif canvas == "header":
             if cells and not all_:
                 for c in cells:
                     try:
                         del self.CH.cell_options[c]["highlight"]
                     except Exception:
-                        pass
+                        continue
             elif not all_:
                 if column in self.CH.cell_options and "highlight" in self.CH.cell_options[column]:
                     del self.CH.cell_options[column]["highlight"]
             elif all_:
                 for c in self.CH.cell_options:
                     if "highlight" in self.CH.cell_options[c]:
                         del self.CH.cell_options[c]["highlight"]
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def get_highlighted_cells(self, canvas: str = "table") -> dict | None:
         if canvas == "table":
             return {k: v["highlight"] for k, v in self.MT.cell_options.items() if "highlight" in v}
         elif canvas == "row_index":
             return {k: v["highlight"] for k, v in self.RI.cell_options.items() if "highlight" in v}
         elif canvas == "header":
@@ -5581,33 +5718,33 @@
     def align_cells(
         self,
         row: int = 0,
         column: int = 0,
         cells: list = [],
         align: str | None = "global",
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(cells, dict):
             for k, v in cells.items():
                 set_align(self.MT.cell_options, k, convert_align(v))
         elif cells:
             align = convert_align(align)
             for k in cells:
                 set_align(self.MT.cell_options, k, align)
         else:
             set_align(self.MT.cell_options, (row, column), convert_align(align))
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def align_rows(
         self,
         rows: list | dict | int = [],
         align: str | None = "global",
         align_index: bool = False,
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(rows, dict):
             for k, v in rows.items():
                 align = convert_align(v)
                 set_align(self.MT.row_options, k, align)
                 if align_index:
                     set_align(self.RI.cell_options, k, align)
         elif is_iterable(rows):
@@ -5616,23 +5753,23 @@
                 set_align(self.MT.row_options, k, align)
                 if align_index:
                     set_align(self.RI.cell_options, k, align)
         elif isinstance(rows, int):
             set_align(self.MT.row_options, rows, convert_align(align))
             if align_index:
                 set_align(self.RI.cell_options, rows, align)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def align_columns(
         self,
         columns: list | dict | int = [],
         align: str | None = "global",
         align_header: bool = False,
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(columns, dict):
             for k, v in columns.items():
                 align = convert_align(v)
                 set_align(self.MT.col_options, k, align)
                 if align_header:
                     set_align(self.CH.cell_options, k, align)
         elif is_iterable(columns):
@@ -5641,49 +5778,49 @@
                 set_align(self.MT.col_options, k, align)
                 if align_header:
                     set_align(self.CH.cell_options, k, align)
         elif isinstance(columns, int):
             set_align(self.MT.col_options, columns, convert_align(align))
             if align_header:
                 set_align(self.CH.cell_options, columns, align)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def align_header(
         self,
         columns: list | dict | int = [],
         align: str | None = "global",
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(columns, dict):
             for k, v in columns.items():
                 set_align(self.CH.cell_options, k, convert_align(v))
         elif is_iterable(columns):
             align = convert_align(align)
             for k in columns:
                 set_align(self.CH.cell_options, k, align)
         elif isinstance(columns, int):
             set_align(self.CH.cell_options, columns, convert_align(align))
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def align_index(
         self,
         rows: list | dict | int = [],
         align: str | None = "global",
         redraw: bool = True,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(rows, dict):
             for k, v in rows.items():
                 set_align(self.RI.cell_options, k, convert_align(v))
         elif is_iterable(rows):
             align = convert_align(align)
             for k in rows:
                 set_align(self.RI.cell_options, k, align)
         elif isinstance(rows, int):
             set_align(self.RI.cell_options, rows, convert_align(align))
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def get_cell_alignments(self) -> dict:
         return {(r, c): v["align"] for (r, c), v in self.MT.cell_options.items() if "align" in v}
 
     def get_column_alignments(self) -> dict:
         return {c: v["align"] for c, v in self.MT.col_options.items() if "align" in v}
 
@@ -5919,139 +6056,145 @@
 
     def create_dropdown(
         self,
         r: int | Literal["all"] = 0,
         c: int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = get_dropdown_kwargs(*args, **kwargs)
         d = get_dropdown_dict(**kwargs)
-        v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
+        if kwargs["set_value"] is None:
+            if kwargs["values"] and (v := self.MT.get_cell_data(r, c)) not in kwargs["values"]:
+                v = kwargs["values"][0]
+            else:
+                v == ""
+        else:
+            v = kwargs["set_value"]
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
                 self._create_dropdown(r_, c, v, d)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
                 self._create_dropdown(r, c_, v, d)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             totalcols = self.MT.total_data_cols()
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(totalcols):
                     self._create_dropdown(r_, c_, v, d)
         elif isinstance(r, int) and isinstance(c, int):
             self._create_dropdown(r, c, v, d)
-        self.set_refresh_timer(kwargs["redraw"])
+        return self.set_refresh_timer(kwargs["redraw"])
 
     def _create_dropdown(self, r: int, c: int, v: object, d: dict) -> None:
         self.del_cell_options_dropdown_and_checkbox(r, c)
         add_to_options(self.MT.cell_options, (r, c), "dropdown", d)
         self.MT.set_cell_data(r, c, v)
 
     def dropdown_cell(
         self,
         r: int | Literal["all"] = 0,
         c: int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
-        self.create_dropdown(r=r, c=c, **get_dropdown_kwargs(*args, **kwargs))
+    ) -> Sheet:
+        return self.create_dropdown(r=r, c=c, **get_dropdown_kwargs(*args, **kwargs))
 
     def dropdown_row(
         self,
         r: Iterator[int] | int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = get_dropdown_kwargs(*args, **kwargs)
         d = get_dropdown_dict(**kwargs)
         v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
                 self._dropdown_row(r_, v, d)
         elif isinstance(r, int):
             self._dropdown_row(r, v, d)
         elif is_iterable(r):
             for r_ in r:
                 self._dropdown_row(r_, v, d)
-        self.set_refresh_timer(kwargs["redraw"])
+        return self.set_refresh_timer(kwargs["redraw"])
 
     def _dropdown_row(self, r: int, v: object, d: dict) -> None:
         self.del_row_options_dropdown_and_checkbox(r)
         add_to_options(self.MT.row_options, r, "dropdown", d)
         for c in range(self.MT.total_data_cols()):
             self.MT.set_cell_data(r, c, v)
 
     def dropdown_column(
         self,
         c: Iterator[int] | int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = get_dropdown_kwargs(*args, **kwargs)
         d = get_dropdown_dict(**kwargs)
         v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
                 self._dropdown_column(c_, v, d)
         elif isinstance(c, int):
             self._dropdown_column(c, v, d)
         elif is_iterable(c):
             for c_ in c:
                 self._dropdown_column(c_, v, d)
-        self.set_refresh_timer(kwargs["redraw"])
+        return self.set_refresh_timer(kwargs["redraw"])
 
     def _dropdown_column(self, c: int, v: object, d: dict) -> None:
         self.del_column_options_dropdown_and_checkbox(c)
         add_to_options(self.MT.col_options, c, "dropdown", d)
         for r in range(self.MT.total_data_rows()):
             self.MT.set_cell_data(r, c, v)
 
     def create_header_dropdown(
         self,
         c: Iterator[int] | int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = get_dropdown_kwargs(*args, **kwargs)
         d = get_dropdown_dict(**kwargs)
         v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
                 self._create_header_dropdown(c_, v, d)
         elif isinstance(c, int):
             self._create_header_dropdown(c, v, d)
         elif is_iterable(c):
             for c_ in c:
                 self._create_header_dropdown(c_, v, d)
-        self.set_refresh_timer(kwargs["redraw"])
+        return self.set_refresh_timer(kwargs["redraw"])
 
     def _create_header_dropdown(self, c: int, v: object, d: dict) -> None:
         self.del_header_cell_options_dropdown_and_checkbox(c)
         add_to_options(self.CH.cell_options, c, "dropdown", d)
         self.CH.set_cell_data(c, v)
 
     def create_index_dropdown(
         self,
         r: Iterator[int] | int | Literal["all"] = 0,
         *args,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = get_dropdown_kwargs(*args, **kwargs)
         d = get_dropdown_dict(**kwargs)
         v = kwargs["set_value"] if kwargs["set_value"] is not None else kwargs["values"][0] if kwargs["values"] else ""
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
                 self._create_index_dropdown(r_, v, d)
         elif isinstance(r, int):
             self._create_index_dropdown(r, v, d)
         elif is_iterable(r):
             for r_ in r:
                 self._create_index_dropdown(r_, v, d)
-        self.set_refresh_timer(kwargs["redraw"])
+        return self.set_refresh_timer(kwargs["redraw"])
 
     def _create_index_dropdown(self, r: int, v: object, d: dict) -> None:
         self.del_index_cell_options_dropdown_and_checkbox(r)
         add_to_options(self.RI.cell_options, r, "dropdown", d)
         self.RI.set_cell_data(r, v)
 
     def delete_dropdown(
@@ -6216,16 +6359,16 @@
             else:
                 raise Exception("No dropdown box is currently open")
         else:
             r_ = r
         kwargs = self.RI.get_cell_kwargs(r_, key="dropdown")
         if kwargs:
             kwargs["values"] = values
-            if self.RI.current_dropdown_window is not None:
-                self.RI.current_dropdown_window.values(values)
+            if self.RI.dropdown.open:
+                self.RI.dropdown.window.values(values)
             if set_value is not None:
                 self.MT.row_index(newindex=set_value, index=r_)
                 # here
         return self
 
     def get_dropdown_values(self, r: int = 0, c: int = 0) -> None | list:
         kwargs = self.MT.get_cell_kwargs(r, c, key="dropdown")
@@ -6302,75 +6445,76 @@
         self,
         r: int | Literal["all"],
         c: int | Literal["all"],
         formatter_options: dict = {},
         formatter_class: object = None,
         redraw: bool = True,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = fix_format_kwargs({"formatter": formatter_class, **formatter_options, **kwargs})
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_ in range(self.MT.total_data_rows()):
                 self._format_cell(r_, c, kwargs)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for c_ in range(self.MT.total_data_cols()):
                 self._format_cell(r, c_, kwargs)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_ in range(self.MT.total_data_rows()):
                 for c_ in range(self.MT.total_data_cols()):
                     self._format_cell(r_, c_, kwargs)
         else:
             self._format_cell(r, c, kwargs)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def _format_cell(self, r: int, c: int, d: dict) -> None:
         v = d["value"] if "value" in d else self.MT.get_cell_data(r, c)
         self.del_cell_options_checkbox(r, c)
         add_to_options(self.MT.cell_options, (r, c), "format", d)
         self.MT.set_cell_data(r, c, value=v, kwargs=d)
 
     def delete_cell_format(
         self,
         r: Literal["all"] | int = "all",
         c: Literal["all"] | int = "all",
         clear_values: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if isinstance(r, str) and r.lower() == "all" and isinstance(c, int):
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r_, c)]:
                     self.MT.delete_cell_format(r_, c, clear_values=clear_values)
         elif isinstance(c, str) and c.lower() == "all" and isinstance(r, int):
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r, c_)]:
                     self.MT.delete_cell_format(r, c_, clear_values=clear_values)
         elif isinstance(r, str) and r.lower() == "all" and isinstance(c, str) and c.lower() == "all":
             for r_, c_ in self.MT.cell_options:
                 if "format" in self.MT.cell_options[(r_, c_)]:
                     self.MT.delete_cell_format(r_, c_, clear_values=clear_values)
         else:
             self.MT.delete_cell_format(r, c, clear_values=clear_values)
+        return self
 
     def format_row(
         self,
         r: Iterator[int] | int | Literal["all"],
         formatter_options: dict = {},
         formatter_class: object = None,
         redraw: bool = True,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = fix_format_kwargs({"formatter": formatter_class, **formatter_options, **kwargs})
         if isinstance(r, str) and r.lower() == "all":
             for r_ in range(len(self.MT.data)):
                 self._format_row(r_, kwargs)
         elif is_iterable(r):
             for r_ in r:
                 self._format_row(r_, kwargs)
         else:
             self._format_row(r, kwargs)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def _format_row(self, r: int, d: dict) -> None:
         self.del_row_options_checkbox(r)
         add_to_options(self.MT.row_options, r, "format", d)
         for c in range(self.MT.total_data_cols()):
             self.MT.set_cell_data(
                 r,
@@ -6379,39 +6523,40 @@
                 kwargs=d,
             )
 
     def delete_row_format(
         self,
         r: Iterator[int] | int | Literal["all"] = "all",
         clear_values: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if is_iterable(r):
             for r_ in r:
                 self.MT.delete_row_format(r_, clear_values=clear_values)
         else:
             self.MT.delete_row_format(r, clear_values=clear_values)
+        return self
 
     def format_column(
         self,
         c: Iterator[int] | int | Literal["all"],
         formatter_options: dict = {},
         formatter_class: object = None,
         redraw: bool = True,
         **kwargs,
-    ) -> None:
+    ) -> Sheet:
         kwargs = fix_format_kwargs({"formatter": formatter_class, **formatter_options, **kwargs})
         if isinstance(c, str) and c.lower() == "all":
             for c_ in range(self.MT.total_data_cols()):
                 self._format_column(c_, kwargs)
         elif is_iterable(c):
             for c_ in c:
                 self._format_column(c_, kwargs)
         else:
             self._format_column(c, kwargs)
-        self.set_refresh_timer(redraw)
+        return self.set_refresh_timer(redraw)
 
     def _format_column(self, c: int, d: dict) -> None:
         self.del_column_options_checkbox(c)
         add_to_options(self.MT.col_options, c, "format", d)
         for r in range(self.MT.total_data_rows()):
             self.MT.set_cell_data(
                 r,
@@ -6420,60 +6565,63 @@
                 kwargs=d,
             )
 
     def delete_column_format(
         self,
         c: Iterator[int] | int | Literal["all"] = "all",
         clear_values: bool = False,
-    ) -> None:
+    ) -> Sheet:
         if is_iterable(c):
             for c_ in c:
                 self.MT.delete_column_format(c_, clear_values=clear_values)
         else:
             self.MT.delete_column_format(c, clear_values=clear_values)
+        return self
 
 
 class Dropdown(Sheet):
     def __init__(
         self,
         parent: tk.Misc,
         r: int,
         c: int,
         ops: dict,
         outline_color: str,
         width: int | None = None,
         height: int | None = None,
         font: None | tuple[str, int, str] = None,
-        outline_thickness: int = 1,
+        outline_thickness: int = 2,
         values: list[object] = [],
         close_dropdown_window: Callable | None = None,
         search_function: Callable = dropdown_search_function,
         arrowkey_RIGHT: Callable | None = None,
         arrowkey_LEFT: Callable | None = None,
         align: str = "w",
         # False for using r, c
         # "r" for r
         # "c" for c
         single_index: Literal["r", "c"] | bool = False,
     ) -> None:
         Sheet.__init__(
             self,
             parent=parent,
+            name="!SheetDropdown",
             outline_thickness=outline_thickness,
             show_horizontal_grid=True,
             show_vertical_grid=False,
             show_header=False,
             show_row_index=False,
             show_top_left=False,
             empty_horizontal=0,
             empty_vertical=0,
             selected_rows_to_end_of_window=True,
             horizontal_grid_to_end_of_window=True,
             set_cell_sizes_on_zoom=True,
             show_selected_cells_border=False,
+            scrollbar_show_arrows=False,
         )
         self.parent = parent
         self.close_dropdown_window = close_dropdown_window
         self.search_function = search_function
         self.arrowkey_RIGHT = arrowkey_RIGHT
         self.arrowkey_LEFT = arrowkey_LEFT
         self.single_index = single_index
@@ -6497,14 +6645,15 @@
         height: int,
         font: tuple[str, int, str],
         ops: DotDict,
         outline_color: str,
         align: str,
         values: list[object] | None = None,
     ) -> None:
+        self.deselect(redraw=False)
         self.r = r
         self.c = c
         self.row = -1
         self.height_and_width(height=height, width=width)
         self.table_align(align)
         self.set_options(
             outline_color=outline_color,
@@ -6597,8 +6746,8 @@
         self.set_sheet_data(
             [[v] for v in values],
             reset_col_positions=False,
             reset_row_positions=False,
             redraw=False,
             verify=False,
         )
-        self.set_all_cell_sizes_to_text(redraw=redraw, width=width)
+        self.set_all_cell_sizes_to_text(redraw=redraw, width=width, slim=True)
```

### Comparing `tksheet-7.1.9/tksheet/sheet_options.py` & `tksheet-7.2.0/tksheet/sheet_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -145,14 +145,17 @@
             "index_selected_cells_fg": theme_light_blue["index_selected_cells_fg"],
             "top_left_bg": theme_light_blue["top_left_bg"],
             "top_left_fg": theme_light_blue["top_left_fg"],
             "top_left_fg_highlight": theme_light_blue["top_left_fg_highlight"],
             "table_bg": theme_light_blue["table_bg"],
             "table_grid_fg": theme_light_blue["table_grid_fg"],
             "table_fg": theme_light_blue["table_fg"],
+            "tree_arrow_fg": theme_light_blue["tree_arrow_fg"],
+            "selected_cells_tree_arrow_fg": theme_light_blue["selected_cells_tree_arrow_fg"],
+            "selected_rows_tree_arrow_fg": theme_light_blue["selected_rows_tree_arrow_fg"],
             "table_selected_box_cells_fg": theme_light_blue["table_selected_box_cells_fg"],
             "table_selected_box_rows_fg": theme_light_blue["table_selected_box_rows_fg"],
             "table_selected_box_columns_fg": theme_light_blue["table_selected_box_columns_fg"],
             "table_selected_cells_border_fg": theme_light_blue["table_selected_cells_border_fg"],
             "table_selected_cells_bg": theme_light_blue["table_selected_cells_bg"],
             "table_selected_cells_fg": theme_light_blue["table_selected_cells_fg"],
             "resizing_line_fg": theme_light_blue["resizing_line_fg"],
@@ -211,15 +214,16 @@
             "show_default_header_for_empty": True,
             "show_default_index_for_empty": True,
             "default_header_height": "1",
             "default_row_height": "1",
             "default_column_width": 120,
             "default_row_index_width": 70,
             "page_up_down_select_row": True,
-            "expand_sheet_if_paste_too_big": False,
+            "paste_can_expand_x": False,
+            "paste_can_expand_y": False,
             "paste_insert_column_limit": None,
             "paste_insert_row_limit": None,
             "arrow_key_down_right_scroll_page": False,
             "cell_auto_resize_enabled": True,
             "auto_resize_row_index": True,
             "max_undos": 30,
             "column_drag_and_drop_perform": True,
@@ -230,12 +234,12 @@
             "horizontal_grid_to_end_of_window": False,
             "vertical_grid_to_end_of_window": False,
             "show_vertical_grid": True,
             "show_horizontal_grid": True,
             "display_selected_fg_over_highlights": False,
             "show_selected_cells_border": True,
             "treeview": False,
-            "treeview_indent": "3",
+            "treeview_indent": "6",
             "rounded_boxes": True,
             "alternate_color": "",
         }
     )
```

### Comparing `tksheet-7.1.9/tksheet/text_editor.py` & `tksheet-7.2.0/tksheet/text_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         parent: tk.Misc,
         newline_binding: None | Callable = None,
     ) -> None:
         tk.Text.__init__(
             self,
             parent,
             spacing1=0,
-            spacing2=0,
+            spacing2=1,
             spacing3=0,
             bd=0,
             highlightthickness=0,
             undo=True,
             maxundo=30,
         )
         self.parent = parent
@@ -115,19 +115,15 @@
             "delete",
             "replace",
         ):
             self.tag_add("align", 1.0, "end")
             self.event_generate("<<TextModified>>")
             if args and len(args) > 1 and args[1] != "\n" and args != ("1.0", "end"):
                 if self.yview() != (0.0, 1.0) and self.newline_bindng is not None:
-                    self.newline_bindng(
-                        r=self.parent.r,
-                        c=self.parent.c,
-                        check_lines=False,
-                    )
+                    self.newline_bindng(check_lines=False)
         return result
 
     def rc(self, event: object) -> None:
         self.focus_set()
         self.rc_popup_menu.tk_popup(event.x_root, event.y_root)
 
     def select_all(self, event: object = None) -> Literal["break"]:
```

### Comparing `tksheet-7.1.9/tksheet/themes.py` & `tksheet-7.2.0/tksheet/themes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
-theme_light_blue: dict[str, str] = {
+from .other_classes import DotDict
+
+theme_light_blue: dict[str, str] = DotDict({
     "popup_menu_fg": "#000000",
     "popup_menu_bg": "#FFFFFF",
     "popup_menu_highlight_bg": "#DCDEE0",
     "popup_menu_highlight_fg": "#000000",
     "index_hidden_rows_expander_bg": "#747775",
     "header_hidden_columns_expander_bg": "#747775",
     "header_bg": "#FFFFFF",
@@ -28,26 +30,29 @@
     "table_selected_box_cells_fg": "#0B57D0",
     "table_selected_box_rows_fg": "#0B57D0",
     "table_selected_box_columns_fg": "#0B57D0",
     "table_selected_cells_border_fg": "#0B57D0",
     "table_selected_cells_bg": "#E6EFFD",
     "table_selected_cells_fg": "black",
     "resizing_line_fg": "black",
-    "drag_and_drop_bg": "black",
+    "drag_and_drop_bg": "#0B57D0",
     "outline_color": "gray2",
     "header_selected_columns_bg": "#0B57D0",
     "header_selected_columns_fg": "#FFFFFF",
     "index_selected_rows_bg": "#0B57D0",
     "index_selected_rows_fg": "#FFFFFF",
     "table_selected_rows_border_fg": "#0B57D0",
     "table_selected_rows_bg": "#E6EFFD",
     "table_selected_rows_fg": "black",
     "table_selected_columns_border_fg": "#0B57D0",
     "table_selected_columns_bg": "#E6EFFD",
     "table_selected_columns_fg": "black",
+    "tree_arrow_fg": "black",
+    "selected_cells_tree_arrow_fg": "black",
+    "selected_rows_tree_arrow_fg": "#FFFFFF",
     "vertical_scroll_background": "#FFFFFF",
     "horizontal_scroll_background": "#FFFFFF",
     "vertical_scroll_troughcolor": "#f9fbfd",
     "horizontal_scroll_troughcolor": "#f9fbfd",
     "vertical_scroll_lightcolor": "#FFFFFF",
     "horizontal_scroll_lightcolor": "#FFFFFF",
     "vertical_scroll_darkcolor": "gray50",
@@ -66,17 +71,17 @@
     "horizontal_scroll_pressed_bg": "#bdc1c6",
     "vertical_scroll_active_fg": "#bdc1c6",
     "horizontal_scroll_active_fg": "#bdc1c6",
     "vertical_scroll_not_active_fg": "#DADCE0",
     "horizontal_scroll_not_active_fg": "#DADCE0",
     "vertical_scroll_pressed_fg": "#bdc1c6",
     "horizontal_scroll_pressed_fg": "#bdc1c6",
-}
+})
 
-theme_light_green: dict[str, str] = {
+theme_light_green: dict[str, str] = DotDict({
     "popup_menu_fg": "#000000",
     "popup_menu_bg": "#FFFFFF",
     "popup_menu_highlight_bg": "#DCDEE0",
     "popup_menu_highlight_fg": "#000000",
     "index_hidden_rows_expander_bg": "gray30",
     "header_hidden_columns_expander_bg": "gray30",
     "header_bg": "#ECECEC",
@@ -86,40 +91,43 @@
     "header_selected_cells_bg": "#d6d4d2",
     "header_selected_cells_fg": "#217346",
     "index_bg": "#ECECEC",
     "index_border_fg": "#ababab",
     "index_grid_fg": "#ababab",
     "index_fg": "black",
     "index_selected_cells_bg": "#d6d4d2",
-    "index_selected_cells_fg": "#217346",
+    "index_selected_cells_fg": "#107C41",
     "top_left_bg": "#ECECEC",
     "top_left_fg": "#b7b7b7",
     "top_left_fg_highlight": "#5f6368",
     "table_bg": "#FFFFFF",
     "table_grid_fg": "#bfbfbf",
     "table_fg": "black",
-    "table_selected_box_cells_fg": "#217346",
-    "table_selected_box_rows_fg": "#217346",
-    "table_selected_box_columns_fg": "#217346",
-    "table_selected_cells_border_fg": "#217346",
+    "table_selected_box_cells_fg": "#107C41",
+    "table_selected_box_rows_fg": "#107C41",
+    "table_selected_box_columns_fg": "#107C41",
+    "table_selected_cells_border_fg": "#107C41",
     "table_selected_cells_bg": "#E3E3E3",
     "table_selected_cells_fg": "black",
     "resizing_line_fg": "black",
-    "drag_and_drop_bg": "black",
+    "drag_and_drop_bg": "#107C41",
     "outline_color": "gray2",
-    "header_selected_columns_bg": "#d3f0e0",
-    "header_selected_columns_fg": "#217346",
-    "index_selected_rows_bg": "#d3f0e0",
-    "index_selected_rows_fg": "#217346",
-    "table_selected_rows_border_fg": "#217346",
+    "header_selected_columns_bg": "#107C41",
+    "header_selected_columns_fg": "#FFFFFF",
+    "index_selected_rows_bg": "#107C41",
+    "index_selected_rows_fg": "#FFFFFF",
+    "table_selected_rows_border_fg": "#107C41",
     "table_selected_rows_bg": "#E3E3E3",
     "table_selected_rows_fg": "black",
-    "table_selected_columns_border_fg": "#217346",
+    "table_selected_columns_border_fg": "#107C41",
     "table_selected_columns_bg": "#E3E3E3",
     "table_selected_columns_fg": "black",
+    "tree_arrow_fg": "black",
+    "selected_cells_tree_arrow_fg": "#107C41",
+    "selected_rows_tree_arrow_fg": "#FFFFFF",
     "vertical_scroll_background": "#FFFFFF",
     "horizontal_scroll_background": "#FFFFFF",
     "vertical_scroll_troughcolor": "#f1f1f1",
     "horizontal_scroll_troughcolor": "#f1f1f1",
     "vertical_scroll_lightcolor": "#FFFFFF",
     "horizontal_scroll_lightcolor": "#FFFFFF",
     "vertical_scroll_darkcolor": "gray50",
@@ -138,17 +146,17 @@
     "horizontal_scroll_pressed_bg": "#707070",
     "vertical_scroll_active_fg": "#707070",
     "horizontal_scroll_active_fg": "#707070",
     "vertical_scroll_not_active_fg": "#c1c1c1",
     "horizontal_scroll_not_active_fg": "#c1c1c1",
     "vertical_scroll_pressed_fg": "#707070",
     "horizontal_scroll_pressed_fg": "#707070",
-}
+})
 
-theme_dark: dict[str, str] = {
+theme_dark: dict[str, str] = DotDict({
     "popup_menu_fg": "white",
     "popup_menu_bg": "gray15",
     "popup_menu_highlight_bg": "gray40",
     "popup_menu_highlight_fg": "white",
     "index_hidden_rows_expander_bg": "gray30",
     "header_hidden_columns_expander_bg": "gray30",
     "header_bg": "#141414",
@@ -184,14 +192,17 @@
     "index_selected_rows_fg": "white",
     "table_selected_rows_border_fg": "#4489F7",
     "table_selected_rows_bg": "#404040",
     "table_selected_rows_fg": "#F7F7F7",
     "table_selected_columns_border_fg": "#4489F7",
     "table_selected_columns_bg": "#404040",
     "table_selected_columns_fg": "#F7F7F7",
+    "tree_arrow_fg": "#8C8C8C",
+    "selected_cells_tree_arrow_fg": "#6aa2fc",
+    "selected_rows_tree_arrow_fg": "white",
     "vertical_scroll_background": "#3b3b3d",
     "horizontal_scroll_background": "#3b3b3d",
     "vertical_scroll_troughcolor": "#000000",
     "horizontal_scroll_troughcolor": "#000000",
     "vertical_scroll_lightcolor": "gray50",
     "horizontal_scroll_lightcolor": "gray50",
     "vertical_scroll_darkcolor": "gray20",
@@ -210,17 +221,17 @@
     "horizontal_scroll_pressed_bg": "#a0a0a0",
     "vertical_scroll_active_fg": "#a0a0a0",
     "horizontal_scroll_active_fg": "#a0a0a0",
     "vertical_scroll_not_active_fg": "#3b3b3d",
     "horizontal_scroll_not_active_fg": "#3b3b3d",
     "vertical_scroll_pressed_fg": "#a0a0a0",
     "horizontal_scroll_pressed_fg": "#a0a0a0",
-}
+})
 
-theme_black: dict[str, str] = {
+theme_black: dict[str, str] = DotDict({
     "popup_menu_fg": "white",
     "popup_menu_bg": "gray15",
     "popup_menu_highlight_bg": "gray40",
     "popup_menu_highlight_fg": "white",
     "index_hidden_rows_expander_bg": "gray30",
     "header_hidden_columns_expander_bg": "gray30",
     "header_bg": "#000000",
@@ -256,14 +267,17 @@
     "index_selected_rows_fg": "#000000",
     "table_selected_rows_border_fg": "#FBB86C",
     "table_selected_rows_bg": "#404040",
     "table_selected_rows_fg": "#F7F7F7",
     "table_selected_columns_border_fg": "#FBB86C",
     "table_selected_columns_bg": "#404040",
     "table_selected_columns_fg": "#F7F7F7",
+    "tree_arrow_fg": "#8C8C8C",
+    "selected_cells_tree_arrow_fg": "#FBB86C",
+    "selected_rows_tree_arrow_fg": "#000000",
     "vertical_scroll_background": "#3b3a39",
     "horizontal_scroll_background": "#3b3a39",
     "vertical_scroll_troughcolor": "#000000",
     "horizontal_scroll_troughcolor": "#000000",
     "vertical_scroll_lightcolor": "gray50",
     "horizontal_scroll_lightcolor": "gray50",
     "vertical_scroll_darkcolor": "gray20",
@@ -282,38 +296,47 @@
     "horizontal_scroll_pressed_bg": "#a0a0a0",
     "vertical_scroll_active_fg": "#a0a0a0",
     "horizontal_scroll_active_fg": "#a0a0a0",
     "vertical_scroll_not_active_fg": "#3b3a39",
     "horizontal_scroll_not_active_fg": "#3b3a39",
     "vertical_scroll_pressed_fg": "#a0a0a0",
     "horizontal_scroll_pressed_fg": "#a0a0a0",
-}
+})
+
+theme_dark_blue: dict[str, str] = DotDict(theme_dark.copy())
+theme_dark_blue["top_left_fg_highlight"] = "#94EBEB"
+theme_dark_blue["table_selected_box_cells_fg"] = "#94EBEB"
+theme_dark_blue["table_selected_box_rows_fg"] = "#94EBEB"
+theme_dark_blue["table_selected_box_columns_fg"] = "#94EBEB"
+theme_dark_blue["table_selected_cells_border_fg"] = "#94EBEB"
+theme_dark_blue["table_selected_rows_border_fg"] = "#94EBEB"
+theme_dark_blue["table_selected_columns_border_fg"] = "#94EBEB"
+theme_dark_blue["header_fg"] = "#94EBEB"
+theme_dark_blue["header_selected_cells_fg"] = "#94EBEB"
+theme_dark_blue["header_selected_columns_fg"] = "#000000"
+theme_dark_blue["header_selected_columns_bg"] = "#94EBEB"
+theme_dark_blue["index_fg"] = "#94EBEB"
+theme_dark_blue["index_selected_rows_bg"] = "#94EBEB"
+theme_dark_blue["index_selected_rows_fg"] = "#000000"
+theme_dark_blue["index_selected_cells_fg"] = "#94EBEB"
+theme_dark_blue["selected_rows_tree_arrow_fg"] = "#000000"
+theme_dark_blue["selected_cells_tree_arrow_fg"] = "#94EBEB"
 
-theme_dark_blue: dict[str, str] = theme_black.copy()
-theme_dark_blue["header_fg"] = "#6ACAD8"
-theme_dark_blue["header_selected_cells_fg"] = "#6ACAD8"
-theme_dark_blue["index_fg"] = "#6ACAD8"
-theme_dark_blue["index_selected_cells_fg"] = "#6ACAD8"
-theme_dark_blue["top_left_fg_highlight"] = "#6ACAD8"
-theme_dark_blue["table_selected_box_cells_fg"] = "#6ACAD8"
-theme_dark_blue["table_selected_box_rows_fg"] = "#6ACAD8"
-theme_dark_blue["table_selected_box_columns_fg"] = "#6ACAD8"
-theme_dark_blue["table_selected_cells_border_fg"] = "#6ACAD8"
-theme_dark_blue["header_selected_columns_bg"] = "#6ACAD8"
-theme_dark_blue["index_selected_rows_bg"] = "#6ACAD8"
-theme_dark_blue["table_selected_rows_border_fg"] = "#6ACAD8"
-theme_dark_blue["table_selected_columns_border_fg"] = "#6ACAD8"
 
-theme_dark_green: dict[str, str] = theme_black.copy()
+theme_dark_green: dict[str, str] = DotDict(theme_dark.copy())
 theme_dark_green["header_fg"] = "#66FFBF"
 theme_dark_green["header_selected_cells_fg"] = "#66FFBF"
 theme_dark_green["index_fg"] = "#66FFBF"
 theme_dark_green["index_selected_cells_fg"] = "#66FFBF"
 theme_dark_green["top_left_fg_highlight"] = "#66FFBF"
 theme_dark_green["table_selected_box_cells_fg"] = "#66FFBF"
-theme_dark_blue["table_selected_box_rows_fg"] = "#66FFBF"
-theme_dark_blue["table_selected_box_columns_fg"] = "#66FFBF"
+theme_dark_green["table_selected_box_rows_fg"] = "#66FFBF"
+theme_dark_green["table_selected_box_columns_fg"] = "#66FFBF"
 theme_dark_green["table_selected_cells_border_fg"] = "#66FFBF"
 theme_dark_green["header_selected_columns_bg"] = "#66FFBF"
+theme_dark_green["header_selected_columns_fg"] = "#000000"
 theme_dark_green["index_selected_rows_bg"] = "#66FFBF"
+theme_dark_green["index_selected_rows_fg"] = "#000000"
 theme_dark_green["table_selected_rows_border_fg"] = "#66FFBF"
 theme_dark_green["table_selected_columns_border_fg"] = "#66FFBF"
+theme_dark_green["selected_rows_tree_arrow_fg"] = "#000000"
+theme_dark_green["selected_cells_tree_arrow_fg"] = "#000000"
```

### Comparing `tksheet-7.1.9/tksheet/top_left_rectangle.py` & `tksheet-7.2.0/tksheet/top_left_rectangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             self.unbind("<Motion>")
             self.unbind("<ButtonPress-1>")
             self.unbind("<B1-Motion>")
             self.unbind("<ButtonRelease-1>")
             self.unbind("<Double-Button-1>")
             self.unbind(rc_binding)
 
-    def set_dimensions(self, new_w=None, new_h=None) -> None:
+    def set_dimensions(self, new_w=None, new_h=None, recreate_selection_boxes: bool = True) -> None:
         try:
             if new_h is None:
                 h = self.winfo_height()
             if new_w is None:
                 w = self.winfo_width()
             if new_w:
                 self.config(width=new_w)
@@ -178,15 +178,16 @@
             h - 7 - 10,
             w - 7,
             h - 7,
             w - 7 - 10,
             h - 7,
         )
         self.coords(self.select_all_box, 0, 0, w - 5, h - 5)
-        self.MT.recreate_all_selection_boxes()
+        if recreate_selection_boxes:
+            self.MT.recreate_all_selection_boxes()
 
     def mouse_motion(self, event: object = None) -> None:
         self.MT.reset_mouse_motion_creations()
         if self.extra_motion_func is not None:
             self.extra_motion_func(event)
 
     def b1_press(self, event: object = None) -> None:
```

### Comparing `tksheet-7.1.9/tksheet.egg-info/PKG-INFO` & `tksheet-7.2.0/tksheet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tksheet
-Version: 7.1.9
+Version: 7.2.0
 Summary: Tkinter table / sheet widget
 Author-email: ragardner <github@ragardner.simplelogin.com>
 License: Copyright (c) 2019 ragardner and open source contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -38,15 +38,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # tksheet
 
-[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8+-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
+[![PyPI version shields.io](https://img.shields.io/pypi/v/tksheet.svg)](https://pypi.python.org/pypi/tksheet/) ![python](https://img.shields.io/badge/python-3.8|3.9|3.10|3.11|3.12-blue) [![License: MIT](https://img.shields.io/badge/License-MIT%20-blue.svg)](https://github.com/ragardner/tksheet/blob/master/LICENSE.txt)
 
 [![GitHub Release Date](https://img.shields.io/github/release-date-pre/ragardner/tksheet.svg)](https://github.com/ragardner/tksheet/releases) [![Downloads](https://img.shields.io/pypi/dm/tksheet.svg)](https://pypi.org/project/tksheet/)
 
 ### **A python tkinter table widget**
 
 |    **Help**       |                                                                  |
 |-------------------|------------------------------------------------------------------|
@@ -97,14 +97,14 @@
 # add 2 empty columns and add the change to undo stack
 sheet.insert_columns(columns=2, idx=4, undo=True)
 
 # delete columns 0 and 3 and add the change to undo stack
 sheet.delete_columns(columns=[0, 3], undo=True)
 ```
 
-### **light blue theme**
+### **light green theme**
 
-![tksheet light blue theme](https://i.imgur.com/ojU3IQi.jpeg)
+![tksheet light green theme](https://github.com/ragardner/tksheet/assets/26602401/790ee9bd-b4de-48df-8c44-33f303061d84)
 
-### **black theme**
+### **dark theme**
 
-![tksheet black theme](https://i.imgur.com/JeF9vJe.jpeg)
+![tksheet dark theme](https://github.com/ragardner/tksheet/assets/26602401/fc8a0407-1486-46cf-b852-9bcff23160e5)
```

