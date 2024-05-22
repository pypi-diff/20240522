# Comparing `tmp/pygame_canvas-1.4.7.tar.gz` & `tmp/pygame_canvas-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.7.tar", last modified: Tue May 21 15:04:19 2024, max compression
+gzip compressed data, was "pygame_canvas-1.4.8.tar", last modified: Tue May 21 15:06:13 2024, max compression
```

## Comparing `pygame_canvas-1.4.7.tar` & `pygame_canvas-1.4.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.913055 pygame_canvas-1.4.7/
--rw-rw-rw-   0        0        0     1797 2024-05-21 15:04:19.912039 pygame_canvas-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1554 2024-05-21 15:04:12.000000 pygame_canvas-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.894287 pygame_canvas-1.4.7/pygame_canvas/
--rw-rw-rw-   0        0        0       28 2024-05-21 14:59:55.000000 pygame_canvas-1.4.7/pygame_canvas/__init__.py
--rw-rw-rw-   0        0        0    16813 2024-05-21 15:01:48.000000 pygame_canvas-1.4.7/pygame_canvas/pygame_canvas.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.911007 pygame_canvas-1.4.7/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0     1797 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 15:04:19.913055 pygame_canvas-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-21 15:02:25.000000 pygame_canvas-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:06:13.883742 pygame_canvas-1.4.8/
+-rw-rw-rw-   0        0        0     1797 2024-05-21 15:06:13.882730 pygame_canvas-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2024-05-21 15:04:12.000000 pygame_canvas-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:06:13.865508 pygame_canvas-1.4.8/pygame_canvas/
+-rw-rw-rw-   0        0        0       28 2024-05-21 14:59:55.000000 pygame_canvas-1.4.8/pygame_canvas/__init__.py
+-rw-rw-rw-   0        0        0    16813 2024-05-21 15:05:47.000000 pygame_canvas-1.4.8/pygame_canvas/pygame_canvas.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:06:13.880707 pygame_canvas-1.4.8/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1797 2024-05-21 15:06:13.000000 pygame_canvas-1.4.8/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-21 15:06:13.000000 pygame_canvas-1.4.8/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:06:13.000000 pygame_canvas-1.4.8/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 15:06:13.000000 pygame_canvas-1.4.8/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 15:06:13.000000 pygame_canvas-1.4.8/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:06:13.883742 pygame_canvas-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-21 15:06:02.000000 pygame_canvas-1.4.8/setup.py
```

### Comparing `pygame_canvas-1.4.7/PKG-INFO` & `pygame_canvas-1.4.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.7
+Version: 1.4.8
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.7/README.md` & `pygame_canvas-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pygame_canvas-1.4.7/pygame_canvas/pygame_canvas.py` & `pygame_canvas-1.4.8/pygame_canvas/pygame_canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 def default_template(fileName):
     """
     fileName should be: __file__
 
     functions loads default template for pygame2.
     """
     with open(fileName, "w") as file:
-        file.write("""import pygame-canvas as c
+        file.write("""import pygame_canvas as c
 
 c.window(title = "game")
 
 # sprite declaration here:
 object = c.sprite((c.rectangle(50,50,(0,200,255)),),(240,180))
 
 while c.loop(60):
```

### Comparing `pygame_canvas-1.4.7/pygame_canvas.egg-info/PKG-INFO` & `pygame_canvas-1.4.8/pygame_canvas.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.7
+Version: 1.4.8
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
```

### Comparing `pygame_canvas-1.4.7/setup.py` & `pygame_canvas-1.4.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 setup(
     name='pygame_canvas',
-    version='1.4.7',
+    version='1.4.8',
     packages=find_packages(),
     include_package_data=True,
     description='A library for canvas operations using pygame',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://x.com/gioseaxmc',
     install_requires=[
```

