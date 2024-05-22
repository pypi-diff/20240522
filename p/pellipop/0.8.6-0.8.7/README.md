# Comparing `tmp/pellipop-0.8.6.tar.gz` & `tmp/pellipop-0.8.7.tar.gz`

## Comparing `pellipop-0.8.6.tar` & `pellipop-0.8.7.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/Video.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/__about__.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/__init__.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/cli.py
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/file_finder.py
--rw-r--r--   0        0        0    16545 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/gui.py
--rw-r--r--   0        0        0    17144 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/main.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/path_fixer.py
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/pip.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/whisper_from_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/speech_to_text/__init__.py
--rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.6/pellipop/speech_to_text/whisperMode.py
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.6/.gitignore
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.6/.hgignore
--rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.6/LICENSE.txt
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 pellipop-0.8.6/pyproject.toml
--rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.6/readme.md
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.6/PKG-INFO
+-rw-r--r--   0        0        0     7123 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/Video.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/__about__.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/__init__.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/cli.py
+-rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/file_finder.py
+-rw-r--r--   0        0        0    16627 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/gui.py
+-rw-r--r--   0        0        0    17144 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/main.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/path_fixer.py
+-rw-r--r--   0        0        0    25977 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/pellipop.ico
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/pip.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/whisper_from_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/speech_to_text/__init__.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 pellipop-0.8.7/pellipop/speech_to_text/whisperMode.py
+-rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 pellipop-0.8.7/.gitignore
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pellipop-0.8.7/.hgignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pellipop-0.8.7/LICENSE.txt
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 pellipop-0.8.7/pyproject.toml
+-rw-r--r--   0        0        0     4421 2020-02-02 00:00:00.000000 pellipop-0.8.7/readme.md
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 pellipop-0.8.7/PKG-INFO
```

### Comparing `pellipop-0.8.6/pellipop/Video.py` & `pellipop-0.8.7/pellipop/Video.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/cli.py` & `pellipop-0.8.7/pellipop/cli.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/file_finder.py` & `pellipop-0.8.7/pellipop/file_finder.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/gui.py` & `pellipop-0.8.7/pellipop/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import tkinter as tk
 from tkinter import filedialog
 
 import ttkbootstrap as ttk
+from PIL import Image, ImageTk
 
 from pellipop.Video import DummyVideo
 from pellipop.file_finder import how_many_files
 from pellipop.main import Pellipop, default_output_path
 from pellipop.path_fixer import Path
 from pellipop.whisper_from_url import WhisperFromUrl, URLImportError
 
@@ -308,19 +309,20 @@
 
 
 ## ROOT
 
 root = ttk.Window(
     "Pellipop",
     themename="journal",
-    iconphoto="pellipop.ico",
-    size=(1400, 1000),
+    size=(1000, 850),
     resizable=(True, True),
-    minsize=(1050, 900),
+    minsize=(1000, 850),
 )
+icon = Image.open("pellipop.ico")
+root.iconphoto(False, ImageTk.PhotoImage(icon))
 
 main_frame = ttk.Frame(root, padding=10)
 main_frame.pack(fill="both", expand=True)
 
 main_frame.columnconfigure(0, weight=1)
 main_frame.columnconfigure(1, weight=1)
 main_frame.rowconfigure(0, weight=1)
```

### Comparing `pellipop-0.8.6/pellipop/main.py` & `pellipop-0.8.7/pellipop/main.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/path_fixer.py` & `pellipop-0.8.7/pellipop/path_fixer.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/pip.py` & `pellipop-0.8.7/pellipop/pip.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/whisper_from_url.py` & `pellipop-0.8.7/pellipop/whisper_from_url.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pellipop/speech_to_text/whisperMode.py` & `pellipop-0.8.7/pellipop/speech_to_text/whisperMode.py`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/.gitignore` & `pellipop-0.8.7/.gitignore`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/LICENSE.txt` & `pellipop-0.8.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/pyproject.toml` & `pellipop-0.8.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/readme.md` & `pellipop-0.8.7/readme.md`

 * *Files identical despite different names*

### Comparing `pellipop-0.8.6/PKG-INFO` & `pellipop-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pellipop
-Version: 0.8.6
+Version: 0.8.7
 Summary: A graphical and command-line tool to extract key frames from videos along with their retranscription. It uses the Whisper API to transcribe the audio. It also generates a CSV file with the extracted key frames and their corresponding text.
 Project-URL: Homepage, https://github.com/CERES-Sorbonne/Pellipop
 Project-URL: Documentation, https://github.com/CERES-Sorbonne/Pellipop#readme
 Project-URL: Issues, https://github.com/CERES-Sorbonne/Pellipop/issues
 Project-URL: Source, https://github.com/CERES-Sorbonne/Pellipop
 Author: EdouardBoute
 Author-email: Marceau-h <pypi@marceau-h.fr>, Orion Alié <someonefefe@gmail.com>
```

