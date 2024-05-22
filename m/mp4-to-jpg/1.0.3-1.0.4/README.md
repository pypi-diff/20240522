# Comparing `tmp/mp4_to_jpg-1.0.3.tar.gz` & `tmp/mp4_to_jpg-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mp4_to_jpg-1.0.3.tar", last modified: Thu May 16 14:53:19 2024, max compression
+gzip compressed data, was "mp4_to_jpg-1.0.4.tar", last modified: Wed May 22 11:42:41 2024, max compression
```

## Comparing `mp4_to_jpg-1.0.3.tar` & `mp4_to_jpg-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-16 14:53:19.346954 mp4_to_jpg-1.0.3/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4512 2024-05-16 14:53:19.346785 mp4_to_jpg-1.0.3/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4065 2024-05-16 13:42:55.000000 mp4_to_jpg-1.0.3/README.md
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-16 14:53:19.345321 mp4_to_jpg-1.0.3/mp4_to_jpg/
--rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-16 13:47:00.000000 mp4_to_jpg-1.0.3/mp4_to_jpg/__init__.py
--rw-r--r--   0 tadeasfort   (501) staff       (20)    10271 2024-05-16 13:06:53.000000 mp4_to_jpg-1.0.3/mp4_to_jpg/mp4_to_jpg.py
-drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-16 14:53:19.346593 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/
--rw-r--r--   0 tadeasfort   (501) staff       (20)     4512 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/PKG-INFO
--rw-r--r--   0 tadeasfort   (501) staff       (20)      272 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/SOURCES.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/dependency_links.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       58 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/entry_points.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       46 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/requires.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       11 2024-05-16 14:53:19.000000 mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/top_level.txt
--rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-16 14:53:19.347018 mp4_to_jpg-1.0.3/setup.cfg
--rw-r--r--   0 tadeasfort   (501) staff       (20)      891 2024-05-16 14:52:08.000000 mp4_to_jpg-1.0.3/setup.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.444969 mp4_to_jpg-1.0.4/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4648 2024-05-22 11:42:41.444707 mp4_to_jpg-1.0.4/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4065 2024-05-16 13:42:55.000000 mp4_to_jpg-1.0.4/README.md
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.443310 mp4_to_jpg-1.0.4/mp4_to_jpg/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        0 2024-05-16 13:47:00.000000 mp4_to_jpg-1.0.4/mp4_to_jpg/__init__.py
+-rw-r--r--   0 tadeasfort   (501) staff       (20)    11373 2024-05-22 11:40:31.000000 mp4_to_jpg-1.0.4/mp4_to_jpg/mp4_to_jpg.py
+drwxr-xr-x   0 tadeasfort   (501) staff       (20)        0 2024-05-22 11:42:41.444286 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/
+-rw-r--r--   0 tadeasfort   (501) staff       (20)     4648 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/PKG-INFO
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      272 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/SOURCES.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)        1 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/dependency_links.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       58 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/entry_points.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       46 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/requires.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       11 2024-05-22 11:42:41.000000 mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/top_level.txt
+-rw-r--r--   0 tadeasfort   (501) staff       (20)       38 2024-05-22 11:42:41.445024 mp4_to_jpg-1.0.4/setup.cfg
+-rw-r--r--   0 tadeasfort   (501) staff       (20)      891 2024-05-22 11:42:38.000000 mp4_to_jpg-1.0.4/setup.py
```

### Comparing `mp4_to_jpg-1.0.3/PKG-INFO` & `mp4_to_jpg-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: mp4_to_jpg
-Version: 1.0.3
-Summary: A tool to extract frames from MP4 videos and remove duplicates
-Home-page: https://github.com/tadeasf/mp4-to-jpg_click
-Author: Tadeas Fort
-Author-email: taddy.fort@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
 # Video Frame Extraction Tool
 
 This tool allows you to extract frames from video files, with features like deduplication and dynamic frame skipping.
 
 ## Features
 
 This Video Frame Extraction Tool is designed to optimize your workflow with powerful, customizable features for handling video frame processing. Below are the standout capabilities:
```

### Comparing `mp4_to_jpg-1.0.3/README.md` & `mp4_to_jpg-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: mp4_to_jpg
+Version: 1.0.4
+Summary: A tool to extract frames from MP4 videos and remove duplicates
+Home-page: https://github.com/tadeasf/mp4-to-jpg_click
+Author: Tadeas Fort
+Author-email: taddy.fort@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+Requires-Dist: click
+Requires-Dist: opencv-python
+Requires-Dist: tk
+Requires-Dist: tqdm
+Requires-Dist: loguru
+Requires-Dist: imagededup
+
 # Video Frame Extraction Tool
 
 This tool allows you to extract frames from video files, with features like deduplication and dynamic frame skipping.
 
 ## Features
 
 This Video Frame Extraction Tool is designed to optimize your workflow with powerful, customizable features for handling video frame processing. Below are the standout capabilities:
```

### Comparing `mp4_to_jpg-1.0.3/mp4_to_jpg/mp4_to_jpg.py` & `mp4_to_jpg-1.0.4/mp4_to_jpg/mp4_to_jpg.py`

 * *Files 8% similar despite different names*

```diff
@@ -238,28 +238,61 @@
     except Exception as e:
         logger.error(f"Error finding duplicates: {e}")
         return 0
 
 
 def select_input_files():
     """Open file dialog to select multiple video files."""
-    root = tk.Tk()
-    root.withdraw()
-    input_files = filedialog.askopenfilenames(
-        title="Select Video Files", filetypes=[("Video Files", "*.mp4 *.mov")]
-    )
-    return input_files
+    try:
+        root = tk.Tk()
+        root.withdraw()
+        input_files = filedialog.askopenfilenames(
+            title="Select Video Files", filetypes=[("Video Files", "*.mp4 *.mov")]
+        )
+        return input_files
+    except Exception as e:
+        logger.error(f"Tkinter file dialog failed: {e}")
+        return cli_select_input_files()
 
 
 def select_output_directory():
     """Open file dialog to select output directory."""
-    root = tk.Tk()
-    root.withdraw()
-    output_dir = filedialog.askdirectory(title="Select Output Directory")
-    return output_dir
+    try:
+        root = tk.Tk()
+        root.withdraw()
+        output_dir = filedialog.askdirectory(title="Select Output Directory")
+        return output_dir
+    except Exception as e:
+        logger.error(f"Tkinter file dialog failed: {e}")
+        return cli_select_output_directory()
+
+
+def cli_select_input_files():
+    """Fallback method to select multiple video files via CLI."""
+    input_files = []
+    print("Enter the paths of the video files (type 'done' when finished):")
+    while True:
+        path = input("Path: ").strip()
+        if path.lower() == "done":
+            break
+        if os.path.isfile(path):
+            input_files.append(path)
+        else:
+            print(f"File does not exist: {path}")
+    return input_files
+
+
+def cli_select_output_directory():
+    """Fallback method to select output directory via CLI."""
+    while True:
+        output_dir = input("Enter the output directory path: ").strip()
+        if os.path.isdir(output_dir):
+            return output_dir
+        else:
+            print(f"Directory does not exist: {output_dir}")
 
 
 @click.command()
 @click.option(
     "--threshold",
     default=0.99,
     type=float,
```

### Comparing `mp4_to_jpg-1.0.3/mp4_to_jpg.egg-info/PKG-INFO` & `mp4_to_jpg-1.0.4/mp4_to_jpg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 2.1
-Name: mp4-to-jpg
-Version: 1.0.3
+Name: mp4_to_jpg
+Version: 1.0.4
 Summary: A tool to extract frames from MP4 videos and remove duplicates
 Home-page: https://github.com/tadeasf/mp4-to-jpg_click
 Author: Tadeas Fort
 Author-email: taddy.fort@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
+Requires-Dist: click
+Requires-Dist: opencv-python
+Requires-Dist: tk
+Requires-Dist: tqdm
+Requires-Dist: loguru
+Requires-Dist: imagededup
 
 # Video Frame Extraction Tool
 
 This tool allows you to extract frames from video files, with features like deduplication and dynamic frame skipping.
 
 ## Features
```

### Comparing `mp4_to_jpg-1.0.3/setup.py` & `mp4_to_jpg-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mp4_to_jpg",
-    version="1.0.3",
+    version="1.0.4",
     author="Tadeas Fort",
     author_email="taddy.fort@gmail.com",
     description="A tool to extract frames from MP4 videos and remove duplicates",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tadeasf/mp4-to-jpg_click",
     packages=find_packages(),
```

