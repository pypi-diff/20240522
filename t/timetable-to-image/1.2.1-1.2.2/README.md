# Comparing `tmp/timetable-to-image-1.2.1.tar.gz` & `tmp/timetable-to-image-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetable-to-image-1.2.1.tar", last modified: Tue Mar 21 11:18:56 2023, max compression
+gzip compressed data, was "timetable-to-image-1.2.2.tar", last modified: Wed May 22 15:19:51 2024, max compression
```

## Comparing `timetable-to-image-1.2.1.tar` & `timetable-to-image-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.558896 timetable-to-image-1.2.1/
--rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.1/LICENSE
--rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1990 2023-03-21 11:18:56.558896 timetable-to-image-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.1/README.md
--rw-rw-rw-   0        0        0     1166 2023-03-21 11:18:01.000000 timetable-to-image-1.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 11:18:56.558896 timetable-to-image-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.418294 timetable-to-image-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.433928 timetable-to-image-1.2.1/src/TimetableToImage/
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.449547 timetable-to-image-1.2.1/src/TimetableToImage/Image/
--rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.1/src/TimetableToImage/Image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.402324 timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.449547 timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/
--rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
--rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
--rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
--rw-rw-rw-   0        0        0    19704 2023-03-21 11:17:01.000000 timetable-to-image-1.2.1/src/TimetableToImage/Image/func.py
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.512036 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/
--rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/__init__.py
--rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/bell.py
--rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/bells.py
--rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/day.py
--rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/func.py
--rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/lesson.py
--rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/pair.py
--rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.1/src/TimetableToImage/Timetable/week.py
--rw-rw-rw-   0        0        0       71 2023-03-21 11:18:01.000000 timetable-to-image-1.2.1/src/TimetableToImage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 11:18:56.543279 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-03-21 11:18:56.000000 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      880 2023-03-21 11:18:56.000000 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 11:18:56.000000 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-21 11:18:56.000000 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-03-21 11:18:56.000000 timetable-to-image-1.2.1/src/timetable_to_image.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:51.057753 timetable-to-image-1.2.2/
+-rw-rw-rw-   0        0        0     1065 2023-02-13 13:34:29.000000 timetable-to-image-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0      196 2023-02-16 16:03:06.000000 timetable-to-image-1.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1990 2024-05-22 15:19:51.055749 timetable-to-image-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2023-02-13 13:51:19.000000 timetable-to-image-1.2.2/README.md
+-rw-rw-rw-   0        0        0     1166 2024-05-22 15:14:01.000000 timetable-to-image-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:19:51.057753 timetable-to-image-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-13 14:06:26.000000 timetable-to-image-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:50.949750 timetable-to-image-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:50.959748 timetable-to-image-1.2.2/src/TimetableToImage/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:50.965751 timetable-to-image-1.2.2/src/TimetableToImage/Image/
+-rw-rw-rw-   0        0        0       89 2023-02-10 21:03:52.000000 timetable-to-image-1.2.2/src/TimetableToImage/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:50.947751 timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:51.021748 timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/
+-rw-rw-rw-   0        0        0   142424 2023-02-01 20:49:45.000000 timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf
+-rw-rw-rw-   0        0        0   142196 2023-02-01 20:49:45.000000 timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf
+-rw-rw-rw-   0        0        0   142340 2023-02-01 20:49:45.000000 timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf
+-rw-rw-rw-   0        0        0    20042 2024-05-22 15:07:19.000000 timetable-to-image-1.2.2/src/TimetableToImage/Image/func.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:51.042749 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/
+-rw-rw-rw-   0        0        0      444 2023-02-10 21:03:52.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-02-10 21:03:52.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/bell.py
+-rw-rw-rw-   0        0        0       87 2023-02-10 20:33:49.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/bells.py
+-rw-rw-rw-   0        0        0      137 2023-02-10 20:33:49.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/day.py
+-rw-rw-rw-   0        0        0    12655 2023-02-13 15:13:38.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/func.py
+-rw-rw-rw-   0        0        0      304 2023-02-27 20:04:02.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/lesson.py
+-rw-rw-rw-   0        0        0       93 2023-02-10 20:33:49.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/pair.py
+-rw-rw-rw-   0        0        0      710 2023-02-16 15:57:33.000000 timetable-to-image-1.2.2/src/TimetableToImage/Timetable/week.py
+-rw-rw-rw-   0        0        0       71 2024-05-22 15:13:40.000000 timetable-to-image-1.2.2/src/TimetableToImage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:19:51.053750 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/
+-rw-rw-rw-   0        0        0     1990 2024-05-22 15:19:50.000000 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      880 2024-05-22 15:19:50.000000 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:19:50.000000 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-22 15:19:50.000000 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 15:19:50.000000 timetable-to-image-1.2.2/src/timetable_to_image.egg-info/top_level.txt
```

### Comparing `timetable-to-image-1.2.1/LICENSE` & `timetable-to-image-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/PKG-INFO` & `timetable-to-image-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.1/pyproject.toml` & `timetable-to-image-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timetable-to-image"
-version = "1.2.1"
+version = "1.2.2"
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
-current_version = "1.2.1"
+current_version = "1.2.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf` & `timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_bold.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf` & `timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_medium.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf` & `timetable-to-image-1.2.2/src/TimetableToImage/Image/fonts/Golos-UI/font_regular.ttf`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Image/func.py` & `timetable-to-image-1.2.2/src/TimetableToImage/Image/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,63 +64,69 @@
     """
     Return lesson text splitted by symbols limit in string
 
     :param lesson:
     :param limit:
     :return:
     """
-    room = ""
-    for letter in lesson.room:
-        if letter != ' ':
-            room += letter
-
-    teacher = lesson.teacher
-    teacher_words = teacher.split()
-    teacher_flag = True
-    if len(teacher_words) != 2:
-        teacher_flag = False
-
-    name = lesson.name
-    if teacher_flag:
-        t = ', '.join([name, teacher, room])
-    else:
-        t = name
+    string = ""
+    try:
+        room = ""
+        for letter in lesson.room:
+            if letter != ' ':
+                room += letter
+
+        teacher = lesson.teacher
+        teacher_words = teacher.split()
+        teacher_flag = True
+        if len(teacher_words) != 2:
+            teacher_flag = False
+
+        name = lesson.name
+        if teacher_flag:
+            t = ', '.join([name, teacher, room])
+        else:
+            t = name
 
-    if teacher_flag:
-        return textwrap.fill(text=t, width=limit)
+        if teacher_flag:
+            return textwrap.fill(text=t, width=limit)
 
-    t_lines = textwrap.wrap(text=t, width=limit)
+        t_lines = textwrap.wrap(text=t, width=limit)
 
-    if t_lines:
-        last_line = t_lines[-1]
-    else:
-        last_line = ""
-
-    t_last_line = last_line + ', ' + teacher
-    t_wrap = textwrap.wrap(text=t_last_line, width=limit)
-    if len(t_wrap) > 1:
-        if len(textwrap.wrap(text=teacher + ',', width=limit)) == 1:
-            t_lines[-1] += ','
-            t_lines.append(teacher)
-
-    else:
         if t_lines:
-            t_lines.pop()
-        t_lines += t_wrap
+            last_line = t_lines[-1]
+        else:
+            last_line = ""
+
+        t_last_line = last_line + ', ' + teacher
+        t_wrap = textwrap.wrap(text=t_last_line, width=limit)
+        if len(t_wrap) > 1:
+            if len(textwrap.wrap(text=teacher + ',', width=limit)) == 1:
+                t_lines[-1] += ','
+                t_lines.append(teacher)
+
+        else:
+            if t_lines:
+                t_lines.pop()
+            t_lines += t_wrap
 
-    last_line = t_lines[-1]
-    t_last = last_line + ', ' + room
-    if len(textwrap.wrap(text=t_last, width=limit)) == 1:
-        t_lines[-1] = t_last
-    else:
-        t_lines[-1] += ',\n' + room
-
-    string = '\n'.join(t_lines)
-
-    string = string.strip()
+        last_line = t_lines[-1]
+        t_last = last_line + ', ' + room
+        if len(textwrap.wrap(text=t_last, width=limit)) == 1:
+            t_lines[-1] = t_last
+        else:
+            t_lines[-1] += ',\n' + room
+
+        string = '\n'.join(t_lines)
+
+        string = string.strip()
+
+    except Exception:
+        string = ', '.join([lesson.name, lesson.teacher, lesson.room])
+        string = textwrap.wrap(text=string, width=limit)
 
     return string
 
 
 def get_table_row_letters_count(font: ImageFont.FreeTypeFont, column_width: float) -> int:
     """
     Function calculate letters number in row with font by average symbol
```

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Timetable/func.py` & `timetable-to-image-1.2.2/src/TimetableToImage/Timetable/func.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/src/TimetableToImage/Timetable/week.py` & `timetable-to-image-1.2.2/src/TimetableToImage/Timetable/week.py`

 * *Files identical despite different names*

### Comparing `timetable-to-image-1.2.1/src/timetable_to_image.egg-info/PKG-INFO` & `timetable-to-image-1.2.2/src/timetable_to_image.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetable-to-image
-Version: 1.2.1
+Version: 1.2.2
 Summary: The Python library provides functionality for generating a timetable image from an object representation
 Author-email: potapovns <ns.potapov73@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 potapovns
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `timetable-to-image-1.2.1/src/timetable_to_image.egg-info/SOURCES.txt` & `timetable-to-image-1.2.2/src/timetable_to_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

