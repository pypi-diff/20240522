# Comparing `tmp/LogseqMarkdownParser-2.4.tar.gz` & `tmp/logseqmarkdownparser-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogseqMarkdownParser-2.4.tar", last modified: Tue Mar 26 17:45:31 2024, max compression
+gzip compressed data, was "logseqmarkdownparser-2.5.tar", last modified: Wed May 22 16:41:57 2024, max compression
```

## Comparing `LogseqMarkdownParser-2.4.tar` & `logseqmarkdownparser-2.5.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-03-26 17:45:31.695515 LogseqMarkdownParser-2.4/
--rwxr-xr-x   0 g         (1000) g         (1000)    35149 2021-03-24 13:18:27.000000 LogseqMarkdownParser-2.4/LICENSE
--rw-r--r--   0 g         (1000) g         (1000)    42679 2024-03-26 17:45:31.695515 LogseqMarkdownParser-2.4/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)     1507 2024-03-24 12:34:16.000000 LogseqMarkdownParser-2.4/README.md
--rw-rw-r--   0 g         (1000) g         (1000)      864 2024-03-26 17:44:59.000000 LogseqMarkdownParser-2.4/pyproject.toml
--rw-rw-r--   0 g         (1000) g         (1000)       38 2024-03-26 17:45:31.695515 LogseqMarkdownParser-2.4/setup.cfg
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-03-26 17:45:31.691515 LogseqMarkdownParser-2.4/src/
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-03-26 17:45:31.691515 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/
--rw-rw-r--   0 g         (1000) g         (1000)      871 2024-03-24 12:31:32.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/__init__.py
--rw-rw-r--   0 g         (1000) g         (1000)       55 2023-09-02 12:43:29.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/__main__.py
--rw-rw-r--   0 g         (1000) g         (1000)    18235 2024-03-26 17:44:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/classes.py
-drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-03-26 17:45:31.695515 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/
--rw-r--r--   0 g         (1000) g         (1000)    42679 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/PKG-INFO
--rw-rw-r--   0 g         (1000) g         (1000)      447 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/SOURCES.txt
--rw-rw-r--   0 g         (1000) g         (1000)        1 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/dependency_links.txt
--rw-rw-r--   0 g         (1000) g         (1000)       66 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/entry_points.txt
--rw-rw-r--   0 g         (1000) g         (1000)       12 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/requires.txt
--rw-rw-r--   0 g         (1000) g         (1000)       29 2024-03-26 17:45:31.000000 LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/top_level.txt
--rw-rw-r--   0 g         (1000) g         (1000)    16473 2024-03-23 13:38:44.000000 LogseqMarkdownParser-2.4/src/classes.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-05-22 16:41:57.612865 logseqmarkdownparser-2.5/
+-rwxr-xr-x   0 g         (1000) g         (1000)    35149 2021-03-24 13:18:27.000000 logseqmarkdownparser-2.5/LICENSE
+-rw-r--r--   0 g         (1000) g         (1000)    42679 2024-05-22 16:41:57.608865 logseqmarkdownparser-2.5/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)     1507 2024-03-24 12:34:16.000000 logseqmarkdownparser-2.5/README.md
+-rw-rw-r--   0 g         (1000) g         (1000)      864 2024-05-22 16:40:18.000000 logseqmarkdownparser-2.5/pyproject.toml
+-rw-rw-r--   0 g         (1000) g         (1000)       38 2024-05-22 16:41:57.612865 logseqmarkdownparser-2.5/setup.cfg
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-05-22 16:41:57.604865 logseqmarkdownparser-2.5/src/
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-05-22 16:41:57.604865 logseqmarkdownparser-2.5/src/LogseqMarkdownParser/
+-rw-rw-r--   0 g         (1000) g         (1000)      890 2024-05-22 16:41:12.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser/__init__.py
+-rw-rw-r--   0 g         (1000) g         (1000)       55 2023-09-02 12:43:29.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser/__main__.py
+-rw-rw-r--   0 g         (1000) g         (1000)    18461 2024-05-22 16:36:55.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser/classes.py
+drwxrwxr-x   0 g         (1000) g         (1000)        0 2024-05-22 16:41:57.608865 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/
+-rw-r--r--   0 g         (1000) g         (1000)    42679 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/PKG-INFO
+-rw-rw-r--   0 g         (1000) g         (1000)      432 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/SOURCES.txt
+-rw-rw-r--   0 g         (1000) g         (1000)        1 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/dependency_links.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       66 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/entry_points.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       12 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/requires.txt
+-rw-rw-r--   0 g         (1000) g         (1000)       21 2024-05-22 16:41:57.000000 logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/top_level.txt
```

### Comparing `LogseqMarkdownParser-2.4/LICENSE` & `logseqmarkdownparser-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LogseqMarkdownParser-2.4/PKG-INFO` & `logseqmarkdownparser-2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogseqMarkdownParser
-Version: 2.4
+Version: 2.5
 Summary: parse logseq markdown text with easy access to properties, hierarchy, TODO etc
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `LogseqMarkdownParser-2.4/README.md` & `logseqmarkdownparser-2.5/README.md`

 * *Files identical despite different names*

### Comparing `LogseqMarkdownParser-2.4/pyproject.toml` & `logseqmarkdownparser-2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "LogseqMarkdownParser"
-version = "2.4"
+version = "2.5"
 description = "parse logseq markdown text with easy access to properties, hierarchy, TODO etc"
 readme = "README.md"
 authors = [{ name = "thiswillbeyourgithub"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
```

### Comparing `LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/__init__.py` & `logseqmarkdownparser-2.5/src/LogseqMarkdownParser/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import fire
 
 try:
     from . import classes
 except:
     import classes
 
+__VERSION__="2.5"
+
 def parse_file(
         file_path,
         verbose=False,
         as_json=False,
         ):
     """
     Parameters:
```

### Comparing `LogseqMarkdownParser-2.4/src/LogseqMarkdownParser/classes.py` & `logseqmarkdownparser-2.5/src/LogseqMarkdownParser/classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,21 @@
             ):
         self.verbose = verbose
         assert isinstance(content, str), (
             f"content must be of type string, not '{type(content)}'")
 
         # detect each block (read each line then merge with the latest block)
         lines = content.split("\n")
+
+        # convert any leading * to -
+        lines = [
+            li.replace("* ", "- ", 1) if li.lstrip().startswith("* ") else li
+            for li in lines
+        ]
+
         assert lines[0].lstrip().startswith("- ") or ":: " in lines[0] or (len(lines)==1 and not lines[0].strip()), f"First line of document must start with '[ \t]*- ' or contain a page property or the document must be empty"
         lines = [l for l in lines if l.strip()]  # remove empty lines
         pageprop = ""  # as string first
         first_block_reached = False
         for i, line in enumerate(lines):
             if not line.strip():
                 lines[i] = None
@@ -55,14 +62,17 @@
                         if i-ii <= 0:
                             raise Exception("Endless loop")
             else:
                 first_block_reached = True
 
         blocks = [line for line in lines if line is not None]
 
+        if blocks:
+            assert first_block_reached
+
         self.page_properties = {}  # the property of the whole page have to be stored separatly
         prop = re.findall(self.PAGE_PROP_REGEX, pageprop)
         for found in prop:
             assert found == found.lstrip(), f"Incorrect page property? {found}"
             try:
                 key, value = found.split(":: ")
                 self.page_properties[key.strip()] = value.strip()
@@ -86,15 +96,15 @@
 
             if self.verbose:
                 print("\n\n---------------------------------\n")
                 print(block)
                 print("\n")
                 print(f"* indentation level: {block.indentation_level}")
                 print(f"* TODO state: {block.TODO_state}")
-                print(f"* properties: {block.get_properties()}")
+                print(f"* properties: {block.properties}")
                 print(f"* UUID: {block.UUID}")
 
             self.blocks.append(block)
 
         if not check_parsing:
             return
         reformed = self.content
```

### Comparing `LogseqMarkdownParser-2.4/src/LogseqMarkdownParser.egg-info/PKG-INFO` & `logseqmarkdownparser-2.5/src/LogseqMarkdownParser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogseqMarkdownParser
-Version: 2.4
+Version: 2.5
 Summary: parse logseq markdown text with easy access to properties, hierarchy, TODO etc
 Author: thiswillbeyourgithub
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

