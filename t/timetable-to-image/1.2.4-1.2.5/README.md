# Comparing `tmp/timetable-to-image-1.2.4.tar.gz` & `tmp/timetable-to-image-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetable-to-image-1.2.4.tar", last modified: Wed May 22 16:02:43 2024, max compression
+gzip compressed data, was "timetable-to-image-1.2.5.tar", last modified: Wed May 22 18:44:03 2024, max compression
```

## Comparing `timetable-to-image-1.2.4.tar` & `timetable-to-image-1.2.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.056330 timetable-to-image-1.2.4/
--rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.4/LICENSE
--rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2024-05-22 16:02:43.055329 timetable-to-image-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.4/README.md
--rw-rw-rw-   0        0        0     1166 2024-05-22 16:02:23.000000 timetable-to-image-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 16:02:43.056330 timetable-to-image-1.2.4/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.002332 timetable-to-image-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.014333 timetable-to-image-1.2.4/src/TimetableToImage/
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.018332 timetable-to-image-1.2.4/src/TimetableToImage/Image/
--rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.001329 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.025331 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/
--rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
--rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
--rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
--rw-rw-rw-   0        0        0    20279 2024-05-22 16:01:57.000000 timetable-to-image-1.2.4/src/TimetableToImage/Image/func.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.041329 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/
--rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/__init__.py
--rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/bell.py
--rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/bells.py
--rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/day.py
--rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/func.py
--rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/lesson.py
--rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/pair.py
--rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.4/src/TimetableToImage/Timetable/week.py
--rw-rw-rw-   0        0        0       71 2024-05-22 16:02:08.000000 timetable-to-image-1.2.4/src/TimetableToImage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 16:02:43.053329 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/
--rw-rw-rw-   0        0        0     1990 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-22 16:02:42.000000 timetable-to-image-1.2.4/src/timetable_to_image.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.573595 timetable-to-image-1.2.5/
+-rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-22 18:44:03.571594 timetable-to-image-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.5/README.md
+-rw-rw-rw-   0        0        0     1166 2024-05-22 18:43:32.000000 timetable-to-image-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:44:03.573595 timetable-to-image-1.2.5/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.507062 timetable-to-image-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.525593 timetable-to-image-1.2.5/src/TimetableToImage/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.530590 timetable-to-image-1.2.5/src/TimetableToImage/Image/
+-rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.5/src/TimetableToImage/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.504061 timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.538592 timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/
+-rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
+-rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
+-rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
+-rw-rw-rw-   0        0        0    18735 2024-05-22 18:42:59.000000 timetable-to-image-1.2.5/src/TimetableToImage/Image/func.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.556599 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/
+-rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/bell.py
+-rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/bells.py
+-rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/day.py
+-rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/func.py
+-rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/lesson.py
+-rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/pair.py
+-rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.5/src/TimetableToImage/Timetable/week.py
+-rw-rw-rw-   0        0        0       71 2024-05-22 18:43:23.000000 timetable-to-image-1.2.5/src/TimetableToImage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:44:03.569593 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-22 18:44:03.000000 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2024-05-22 18:44:03.000000 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:44:03.000000 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-22 18:44:03.000000 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 18:44:03.000000 timetable-to-image-1.2.5/src/timetable_to_image.egg-info/top_level.txt
```

### Comparing `timetable-to-image-1.2.4/LICENSE` & `timetable-to-image-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/PKG-INFO` & `timetable-to-image-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.4
+Version: 1.2.5
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.4/pyproject.toml` & `timetable-to-image-1.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timetable-to-image"
-version = "1.2.4"
+version = "1.2.5"
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
-current_version = "1.2.4"
+current_version = "1.2.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf` & `timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf` & `timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf` & `timetable-to-image-1.2.5/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Image/func.py` & `timetable-to-image-1.2.5/src/TimetableToImage/Image/func.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,84 +58,26 @@
         shift_x = (place_width - text_width) / 2
     if place_height is not None:
         shift_y = (place_height - text_height) / 2
 
     return shift_x, shift_y
 
 
-def get_splitted_string(lesson: Timetable.Lesson, limit: int) -> str:
+def get_wrapped_string(lesson: Timetable.Lesson, limit: int) -> str:
     """
-    Return lesson text splitted by symbols limit in string
+    Return lesson text wrapped by symbols limit in string
 
     :param lesson:
     :param limit:
     :return:
     """
-    try:
-        room = ""
-        for letter in lesson.room:
-            if letter != ' ':
-                room += letter
-
-        teacher = lesson.teacher
-        teacher_words = teacher.split()
-        teacher_flag = True
-        if len(teacher_words) != 2:
-            teacher_flag = False
-
-        name = lesson.name
-        if teacher_flag:
-            t = ', '.join([name, teacher, room])
-        else:
-            t = name
-
-        if teacher_flag:
-            obj = textwrap.fill(text=t, width=limit)
-            if isinstance(obj, list):
-                obj = ' '.join(obj)
-            return obj
-
-        t_lines = textwrap.wrap(text=t, width=limit)
-
-        if t_lines:
-            last_line = t_lines[-1]
-        else:
-            last_line = ""
-
-        t_last_line = last_line + ', ' + teacher
-        t_wrap = textwrap.wrap(text=t_last_line, width=limit)
-        if len(t_wrap) > 1:
-            if len(textwrap.wrap(text=teacher + ',', width=limit)) == 1:
-                t_lines[-1] += ','
-                t_lines.append(teacher)
-
-        else:
-            if t_lines:
-                t_lines.pop()
-            t_lines += t_wrap
-
-        last_line = t_lines[-1]
-        t_last = last_line + ', ' + room
-        if len(textwrap.wrap(text=t_last, width=limit)) == 1:
-            t_lines[-1] = t_last
-        else:
-            t_lines[-1] += ',\n' + room
-
-        string = '\n'.join(t_lines)
-
-        string = string.strip()
-
-    except Exception:
-        string = ', '.join([lesson.name, lesson.teacher, lesson.room])
-        string = textwrap.wrap(text=string, width=limit)
-
-    if isinstance(string, list):
-        string = ' '.join(string)
-
-    return string
+    lesson_info = str(lesson)
+    wrapped_lines = textwrap.wrap(lesson_info, width=limit, break_long_words=False, break_on_hyphens=False)
+    result = '\n'.join(wrapped_lines)
+    return result
 
 
 def get_table_row_letters_count(font: ImageFont.FreeTypeFont, column_width: float) -> int:
     """
     Function calculate letters number in row with font by average symbol
     :param font:
     :param column_width:
@@ -235,15 +177,15 @@
                     font_lesson.path,
                     font_lesson.size - 1
                 )
             first = False
             letters_count_limit = get_table_row_letters_count(
                 font_lesson, width_lesson
             )
-            text_lesson_split = get_splitted_string(lesson, letters_count_limit)
+            text_lesson_split = get_wrapped_string(lesson, letters_count_limit)
             text_lesson_split_width, text_lesson_split_height = get_multiline_text_size(
                 text_lesson_split, font, interval
             )
 
         x_shift_lesson, y_shift_lesson = get_shifts_to_place_center(
             text_lesson_split, font_lesson,
             place_width=width_lesson,
```

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Timetable/func.py` & `timetable-to-image-1.2.5/src/TimetableToImage/Timetable/func.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/src/TimetableToImage/Timetable/week.py` & `timetable-to-image-1.2.5/src/TimetableToImage/Timetable/week.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.4/src/timetable_to_image.egg-info/PKG-INFO` & `timetable-to-image-1.2.5/src/timetable_to_image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.4
+Version: 1.2.5
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.4/src/timetable_to_image.egg-info/SOURCES.txt` & `timetable-to-image-1.2.5/src/timetable_to_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

