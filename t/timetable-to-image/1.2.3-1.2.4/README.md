# Comparing `tmp/timetable-to-image-1.2.3.tar.gz` & `tmp/timetable-to-image-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetable-to-image-1.2.3.tar", last modified: Wed May 22 15:56:08 2024, max compression
+gzip compressed data, was "timetable-to-image-1.2.4.tar", last modified: Wed May 22 16:02:43 2024, max compression
```

## Comparing `timetable-to-image-1.2.3.tar` & `timetable-to-image-1.2.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.924972 timetable-to-image-1.2.3/
--rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.3/LICENSE
--rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-05-22 15:56:08.923974 timetable-to-image-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.3/README.md
--rw-rw-rw-   0        0        0     1166 2024-05-22 15:55:13.000000 timetable-to-image-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 15:56:08.925944 timetable-to-image-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.870523 timetable-to-image-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.885524 timetable-to-image-1.2.3/src/TimetableToImage/
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.888546 timetable-to-image-1.2.3/src/TimetableToImage/Image/
--rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.3/src/TimetableToImage/Image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.869524 timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.894524 timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/
--rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
--rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
--rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
--rw-rw-rw-   0        0        0    20126 2024-05-22 15:52:32.000000 timetable-to-image-1.2.3/src/TimetableToImage/Image/func.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.910523 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/
--rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/__init__.py
--rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/bell.py
--rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/bells.py
--rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/day.py
--rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/func.py
--rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/lesson.py
--rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/pair.py
--rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.3/src/TimetableToImage/Timetable/week.py
--rw-rw-rw-   0        0        0       71 2024-05-22 15:53:11.000000 timetable-to-image-1.2.3/src/TimetableToImage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 15:56:08.921949 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-22 15:56:08.000000 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2024-05-22 15:56:08.000000 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 15:56:08.000000 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-22 15:56:08.000000 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 15:56:08.000000 timetable-to-image-1.2.3/src/timetable_to_image.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.056330 timetable-to-image-1.2.4/
+-rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-22 16:02:43.055329 timetable-to-image-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.4/README.md
+-rw-rw-rw-   0        0        0     1166 2024-05-22 16:02:23.000000 timetable-to-image-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:02:43.056330 timetable-to-image-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.002332 timetable-to-image-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.014333 timetable-to-image-1.2.4/src/TimetableToImage/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.018332 timetable-to-image-1.2.4/src/TimetableToImage/Image/
+-rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.001329 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.025331 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/
+-rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
+-rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
+-rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
+-rw-rw-rw-   0        0        0    20279 2024-05-22 16:01:57.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/func.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.041329 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/
+-rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/bell.py
+-rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/bells.py
+-rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/day.py
+-rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/func.py
+-rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/lesson.py
+-rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/pair.py
+-rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/week.py
+-rw-rw-rw-   0        0        0       71 2024-05-22 16:02:08.000000 timetable-to-image-1.2.4/src/TimetableToImage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.053329 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/top_level.txt
```

### Comparing `timetable-to-image-1.2.3/LICENSE` & `timetable-to-image-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/PKG-INFO` & `timetable-to-image-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.3
+Version: 1.2.4
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.3/pyproject.toml` & `timetable-to-image-1.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timetable-to-image"
-version = "1.2.3"
+version = "1.2.4"
 description = "The Python library provides functionality for generating a timetable image from an object representation"
 readme = "README.md"
 authors = [{ name = "potapovns", email = "ns.potapov73@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -23,15 +23,15 @@
 [project.optional-dependencies]
 dev = ["bumpver", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/potapovns/timetable_to_image"
 
 [tool.bumpver]
-current_version = "1.2.3"
+current_version = "1.2.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf` & `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf` & `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf` & `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Image/func.py` & `timetable-to-image-1.2.4/src/TimetableToImage/Image/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     """
     Return lesson text splitted by symbols limit in string
 
     :param lesson:
     :param limit:
     :return:
     """
-    string = ""
     try:
         room = ""
         for letter in lesson.room:
             if letter != ' ':
                 room += letter
 
         teacher = lesson.teacher
@@ -86,15 +85,18 @@
         name = lesson.name
         if teacher_flag:
             t = ', '.join([name, teacher, room])
         else:
             t = name
 
         if teacher_flag:
-            return textwrap.fill(text=t, width=limit)
+            obj = textwrap.fill(text=t, width=limit)
+            if isinstance(obj, list):
+                obj = ' '.join(obj)
+            return obj
 
         t_lines = textwrap.wrap(text=t, width=limit)
 
         if t_lines:
             last_line = t_lines[-1]
         else:
             last_line = ""
@@ -122,14 +124,17 @@
 
         string = string.strip()
 
     except Exception:
         string = ', '.join([lesson.name, lesson.teacher, lesson.room])
         string = textwrap.wrap(text=string, width=limit)
 
+    if isinstance(string, list):
+        string = ' '.join(string)
+
     return string
 
 
 def get_table_row_letters_count(font: ImageFont.FreeTypeFont, column_width: float) -> int:
     """
     Function calculate letters number in row with font by average symbol
     :param font:
```

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Timetable/func.py` & `timetable-to-image-1.2.4/src/TimetableToImage/Timetable/func.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/src/TimetableToImage/Timetable/week.py` & `timetable-to-image-1.2.4/src/TimetableToImage/Timetable/week.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.3/src/timetable_to_image.egg-info/PKG-INFO` & `timetable-to-image-1.2.4/src/timetable_to_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.3
+Version: 1.2.4
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.3/src/timetable_to_image.egg-info/SOURCES.txt` & `timetable-to-image-1.2.4/src/timetable_to_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

