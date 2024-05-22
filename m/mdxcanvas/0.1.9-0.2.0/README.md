# Comparing `tmp/mdxcanvas-0.1.9.tar.gz` & `tmp/mdxcanvas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdxcanvas-0.1.9.tar", max compression
+gzip compressed data, was "mdxcanvas-0.2.0.tar", max compression
```

## Comparing `mdxcanvas-0.1.9.tar` & `mdxcanvas-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1065 2023-08-18 21:11:52.811761 mdxcanvas-0.1.9/LICENSE
--rw-r--r--   0        0        0      156 2024-02-22 01:16:53.597390 mdxcanvas-0.1.9/mdxcanvas/__init__.py
--rw-r--r--   0        0        0    24001 2024-05-17 17:52:45.112664 mdxcanvas-0.1.9/mdxcanvas/canvas_creator.py
--rw-r--r--   0        0        0     1053 2024-05-10 18:35:51.774805 mdxcanvas-0.1.9/mdxcanvas/deploy.py
--rw-r--r--   0        0        0     3393 2024-05-03 23:06:22.147341 mdxcanvas-0.1.9/mdxcanvas/document_schema.py
--rw-r--r--   0        0        0     2381 2024-05-17 17:52:45.113016 mdxcanvas-0.1.9/mdxcanvas/extensions.py
--rw-r--r--   0        0        0     2689 2024-05-01 19:18:15.400257 mdxcanvas-0.1.9/mdxcanvas/jinja_parser.py
--rw-r--r--   0        0        0    25520 2024-05-17 17:52:47.600436 mdxcanvas-0.1.9/mdxcanvas/parser.py
--rw-r--r--   0        0        0      559 2024-04-16 18:49:19.290278 mdxcanvas-0.1.9/mdxcanvas/question_schema.py
--rw-r--r--   0        0        0     1878 2024-04-16 18:48:46.610576 mdxcanvas-0.1.9/mdxcanvas/templating.py
--rw-r--r--   0        0        0    15263 2024-05-03 23:06:22.147893 mdxcanvas-0.1.9/mdxcanvas/yaml_parser.py
--rw-r--r--   0        0        0      651 2024-05-17 17:52:47.601034 mdxcanvas-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 mdxcanvas-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-01-31 20:08:12.653583 mdxcanvas-0.2.0/LICENSE
+-rw-r--r--   0        0        0      156 2024-02-23 19:51:14.711484 mdxcanvas-0.2.0/mdxcanvas/__init__.py
+-rw-r--r--   0        0        0    26881 2024-05-22 17:27:48.103533 mdxcanvas-0.2.0/mdxcanvas/canvas_creator.py
+-rw-r--r--   0        0        0     1053 2024-05-22 17:27:48.104910 mdxcanvas-0.2.0/mdxcanvas/deploy.py
+-rw-r--r--   0        0        0     3393 2024-04-23 21:59:22.722245 mdxcanvas-0.2.0/mdxcanvas/document_schema.py
+-rw-r--r--   0        0        0     2446 2024-05-22 17:27:48.105889 mdxcanvas-0.2.0/mdxcanvas/extensions.py
+-rw-r--r--   0        0        0     2689 2024-04-22 22:07:08.576782 mdxcanvas-0.2.0/mdxcanvas/jinja_parser.py
+-rw-r--r--   0        0        0    25520 2024-05-22 17:27:48.108373 mdxcanvas-0.2.0/mdxcanvas/parser.py
+-rw-r--r--   0        0        0      559 2024-04-22 22:07:08.577386 mdxcanvas-0.2.0/mdxcanvas/question_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-22 22:07:08.577697 mdxcanvas-0.2.0/mdxcanvas/templating.py
+-rw-r--r--   0        0        0    15263 2024-04-23 21:58:15.572059 mdxcanvas-0.2.0/mdxcanvas/yaml_parser.py
+-rw-r--r--   0        0        0      651 2024-05-22 17:28:07.701786 mdxcanvas-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 mdxcanvas-0.2.0/PKG-INFO
```

### Comparing `mdxcanvas-0.1.9/LICENSE` & `mdxcanvas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/canvas_creator.py` & `mdxcanvas-0.2.0/mdxcanvas/canvas_creator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import json
 import random
 import sys
 import textwrap
 import uuid
 from datetime import datetime
 
-
 import pytz
 from canvasapi import Canvas
 from canvasapi.assignment import Assignment
 from canvasapi.course import Course
 from canvasapi.module import Module
 from canvasapi.folder import Folder
 from canvasapi.quiz import Quiz
 
 import markdown as md
+import re
 
 from pathlib import Path
 from bs4 import BeautifulSoup, Tag
 
 from markdown.extensions.codehilite import makeExtension as makeCodehiliteExtension
 
-import zipfile
+from zipfile import ZipFile, ZipInfo
 
 from .jinja_parser import process_jinja
 from .extensions import BlackInlineCodeExtension, CustomTagExtension
 from .parser import DocumentParser, make_iso
 from .yaml_parser import DocumentWalker, parse_yaml
 
 
@@ -47,15 +47,14 @@
 
 def upload_file(folder: Folder, file_path: Path):
     """
     Uploads a file to Canvas, and returns the id of the uploaded file.
     """
     print(f"Uploading {file_path.name} ... ", end="")
     file_id = folder.upload(file_path)[1]["id"]
-    print("Done")
     return file_id
 
 
 def create_file_tag(course: Course, canvas_folder: Folder, file_path: Path, display_text: str) -> Tag:
     """
     Returns a tag that links to a file in Canvas.
     """
@@ -75,37 +74,121 @@
     """
     file_path = parent_folder / tag.get("path")
     file_name = tag.get("name") or file_path.name
     display_text = tag.text if tag.text.strip() else file_name
     return create_file_tag(course, canvas_folder, file_path, display_text)
 
 
-def link_zip(course: Course, canvas_folder: Folder, parent_folder: Path, tag: Tag) -> Tag:
+def link_zip_tag(course: Course, canvas_folder: Folder, parent_folder: Path, tag: Tag) -> Tag:
     """
     Zips a folder and uploads it to Canvas.
-    Syntax: <zip path="./resources/assignment" name="progresscheck1.zip">Download Progress Check 1</zip>
+    Syntax: <zip
+                path="./resources/solution"
+                name="progresscheck1.zip"
+                priority_path="./resources/assignment"
+                exclude="*.jpg|*.png"
+            >
+            Download Progress Check 1
+            </zip>
     Alternate: <zip path="./resources/progress_check_1" />
     This would use progress_check_1.zip as the name, and "progress_check_1" as the display text.
     """
-    folder_to_zip = tag.get("path")
-    name = tag.get("name") or f"{folder_to_zip}.zip"
-    print(f"Zipping {folder_to_zip} ... ", end="")
-    folder_path = parent_folder / folder_to_zip
+    folder_name = tag.get("path")
+    name = tag.get("name") or f"{folder_name}.zip"
+    priority_folder = tag.get("priority_path")
+    if priority_folder:
+        priority_folder = parent_folder / priority_folder
+        if not priority_folder.exists():
+            print(f"Priority folder {priority_folder} does not exist, ignoring", file=sys.stderr)
+            priority_folder = None
+    exclude = tag.get("exclude")
+    if exclude:
+        exclude = re.compile(exclude)
+
+    folder_path = parent_folder / folder_name
     path_to_zip = parent_folder / name
-    with zipfile.ZipFile(path_to_zip, "w") as zipf:
-        for file in folder_path.iterdir():
-            zipf.write(file, file.name)
-    print("Done")
     display_text = tag.text if tag.text.strip() else name
+
+    print(f"Zipping {folder_path.name} ... ", end="")
+    zip_folder(folder_path, path_to_zip, exclude, priority_folder)
+    print("Done")
     tag = create_file_tag(course, canvas_folder, path_to_zip, display_text)
+
     # Then delete the zip
     path_to_zip.unlink()
     return tag
 
 
+def zip_folder(folder_path: Path, path_to_zip: Path, exclude: re.Pattern = None, priority_fld: Path = None):
+    """
+    Zips a folder, excluding files that match the exclude pattern.
+    Items from the priority folder are added to the zip if they are not in the standard folder.
+    Items in the priority folder take precedence over items in the standard folder.
+    """
+    with ZipFile(path_to_zip, "w") as zipf:
+        for item in folder_path.glob("*"):
+            write_item_to_zip(item, zipf, exclude, priority_fld=priority_fld)
+
+
+def write_item_to_zip(item: Path, zipf: ZipFile, exclude: re.Pattern = None, prefix='', priority_fld: Path = None):
+    if exclude and exclude.match(item.name):
+        print(f"Excluding file {item.name} ... ", end="")
+        return
+    if item.is_dir():
+        write_directory(item, zipf, exclude, prefix, priority_fld / item.name)
+    else:
+        write_file(item, zipf, prefix, priority_fld)
+
+
+def write_directory(folder: Path, zipf: ZipFile, exclude: re.Pattern = None, prefix='',
+                    priority_fld: Path = None):
+    prefix = prefix + folder.name + '/'
+
+    # Get all items in the folder
+    paths = list(folder.glob("*"))
+
+    # Add items from priority folder that are not in the folder
+    item_names = {i.name for i in folder.glob("*")}
+    if priority_fld:
+        for item in priority_fld.glob("*"):
+            if item.name not in item_names:
+                paths.append(item)
+                print(f"Using additional file {item.name} .. ", end="")
+
+    for path in paths:
+        write_item_to_zip(path, zipf, exclude, prefix, priority_fld)
+
+
+def set_time_1980(file, prefix=''):
+    """
+    Ensures that the zip file stays consistent between runs.
+    """
+    zinfo = ZipInfo(
+        prefix + file.name,
+        date_time=(1980, 1, 1, 0, 0, 0)
+    )
+    return zinfo
+
+
+def write_file(file: Path, zipf: ZipFile, prefix='', priority_fld: Path = None):
+    # Use the file from the priority folder if it exists
+    if priority_fld and (priority_file := priority_fld / file.name).exists():
+        file = priority_file
+        print(f"Prioritizing file {file.name} .. ", end="")
+
+    # For consistency, set the time to 1980
+    zinfo = set_time_1980(file, prefix)
+    try:
+        with open(file) as f:
+            zipf.writestr(zinfo, f.read())
+    except UnicodeDecodeError as _:
+        with open(file, 'rb') as f:
+            zipf.writestr(zinfo, f.read())
+
+
 def get_fancy_html(markdown_or_file: str, course: Course, canvas_folder: Folder, files_folder: Path = None):
     """
     Converts markdown to html, and adds syntax highlighting to code blocks.
     """
     if markdown_or_file.endswith('.md'):
         markdown_or_file = readfile(files_folder / markdown_or_file)
 
@@ -120,22 +203,20 @@
 
         # This forces the color of inline code to be black
         # as a workaround for Canvas's super-ugly default red :P
         BlackInlineCodeExtension(),
 
         CustomTagExtension({
             "file": lambda tag: link_file(course, canvas_folder, files_folder, tag),
-            "zip": lambda tag: link_zip(course, canvas_folder, files_folder, tag)
+            "zip": lambda tag: link_zip_tag(course, canvas_folder, files_folder, tag)
         })
     ])
     return fenced
 
 
-
-
 def get_canvas_folder(course: Course, folder_name: str, parent_folder_path="") -> Folder:
     """
     Retrieves an object representing a digital folder in Canvas. If the folder does not exist, it is created.
     """
     folders = list(course.get_folders())
     if not any(fl.name == folder_name for fl in folders):
         print(f"Created {folder_name} folder")
@@ -573,21 +654,19 @@
     assignment_groups = list(course.get_assignment_groups())
     names_to_ids = {g.name: g.id for g in assignment_groups}
 
     if "jinja" in file_path.name:
         content = process_jinja(file_path)
     else:
         content = file_path.read_text()
-        
-    print("Done")
-    print(f"Getting course folders ... ", end="")
+
+    print(f"Getting course folders ... ")
     course_folders = list(course.get_folders())
     name_of_file = file_path.name.split(".")[0]
     canvas_folder = get_canvas_folder(course, name_of_file)
-    print("Done")
 
     if "yaml" in file_path.name:
         walker = DocumentWalker(
             path_to_resources=file_path.parent,
             path_to_canvas_files=file_path.parent,
             markdown_processor=lambda text: process_markdown(text, course, canvas_folder, file_path.parent),
             time_zone=time_zone,
```

### Comparing `mdxcanvas-0.1.9/mdxcanvas/deploy.py` & `mdxcanvas-0.2.0/mdxcanvas/deploy.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/document_schema.py` & `mdxcanvas-0.2.0/mdxcanvas/document_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/extensions.py` & `mdxcanvas-0.2.0/mdxcanvas/extensions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import xml.etree.ElementTree as etree
 
 from markdown.inlinepatterns import BacktickInlineProcessor, BACKTICK_RE
 from markdown.extensions import Extension
 
 from markdown.preprocessors import HtmlBlockPreprocessor
 from bs4 import BeautifulSoup
-from bs4.element import Tag, NavigableString, PageElement
+from bs4.element import Tag
 
 from typing import Protocol
 
 
 class BlackInlineCodeProcessor(BacktickInlineProcessor):
     def handleMatch(self, m: re.Match[str], data: str) -> tuple[etree.Element | str, int, int]:
         el, start, end = super().handleMatch(m, data)
@@ -28,25 +28,27 @@
 
 
 # Make a Protocol for any tag processor, it should take a Tag and return a Tag
 # This way we can define a type hint for the tag_processors dictionary
 class TagProcessor(Protocol):
     def __call__(self, tag: Tag) -> Tag:
         ...
-    
 
 class CustomHTMLBlockTagProcessor(HtmlBlockPreprocessor):
     tag_processors: dict[str, TagProcessor]
     
     def __init__(self, md, tag_processors: dict[str, TagProcessor]):
         super().__init__(md)
         self.custom_tag_processors = tag_processors
     
     def run(self, lines: list[str]) -> list[str]:
-        soup = BeautifulSoup("\n".join(lines), "html.parser")
+        joined = "\n".join(lines)
+        if "<" not in joined or ">" not in joined:
+            return lines
+        soup = BeautifulSoup(joined, "html.parser")
         for tag in soup.find_all():
             if tag.name in self.custom_tag_processors:
                 processor = self.custom_tag_processors[tag.name]
                 tag.replace_with(processor(tag))
         return str(soup).split("\n")
```

### Comparing `mdxcanvas-0.1.9/mdxcanvas/jinja_parser.py` & `mdxcanvas-0.2.0/mdxcanvas/jinja_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/parser.py` & `mdxcanvas-0.2.0/mdxcanvas/parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/question_schema.py` & `mdxcanvas-0.2.0/mdxcanvas/question_schema.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/templating.py` & `mdxcanvas-0.2.0/mdxcanvas/templating.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/mdxcanvas/yaml_parser.py` & `mdxcanvas-0.2.0/mdxcanvas/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `mdxcanvas-0.1.9/pyproject.toml` & `mdxcanvas-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mdxcanvas"
-version = "0.1.9"
+version = "0.2.0"
 description = "A Canvas LMS API wrapper for maintaining content in markdown"
 authors = ["Gordon Bean <gbean@cs.byu.edu>", "Preston Raab <phr23@byu.edu>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 Jinja2 = "^3.1.2"
```

### Comparing `mdxcanvas-0.1.9/PKG-INFO` & `mdxcanvas-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: mdxcanvas
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Canvas LMS API wrapper for maintaining content in markdown
 License: MIT
 Author: Gordon Bean
 Author-email: gbean@cs.byu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: CanvasAPI (>=3.2.0,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: Markdown (>=3.1.1,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.0.1,<3.0.0)
 Requires-Dist: Pygments (>=2.17.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.0,<5.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
```

