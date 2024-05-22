# Comparing `tmp/tgadmin-0.9.0.tar.gz` & `tmp/tgadmin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgadmin-0.9.0.tar", last modified: Tue Mar 12 22:57:21 2024, max compression
+gzip compressed data, was "tgadmin-0.9.1.tar", last modified: Wed Mar 13 07:46:14 2024, max compression
```

## Comparing `tgadmin-0.9.0.tar` & `tgadmin-0.9.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 22:57:21.509054 tgadmin-0.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2024-03-12 22:57:09.000000 tgadmin-0.9.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12733 2024-03-12 22:57:21.505054 tgadmin-0.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2760 2024-03-12 22:57:09.000000 tgadmin-0.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-03-12 22:57:09.000000 tgadmin-0.9.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-12 22:57:21.509054 tgadmin-0.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 22:57:21.505054 tgadmin-0.9.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 22:57:21.505054 tgadmin-0.9.0/src/tgadmin/
--rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-12 22:57:09.000000 tgadmin-0.9.0/src/tgadmin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18829 2024-03-12 22:57:09.000000 tgadmin-0.9.0/src/tgadmin/tgadmin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 22:57:21.505054 tgadmin-0.9.0/src/tgadmin.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12733 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      291 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       45 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-12 22:57:21.000000 tgadmin-0.9.0/src/tgadmin.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:46:14.376510 tgadmin-0.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-03-13 07:45:56.000000 tgadmin-0.9.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    12733 2024-03-13 07:46:14.376510 tgadmin-0.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2024-03-13 07:45:56.000000 tgadmin-0.9.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-03-13 07:45:56.000000 tgadmin-0.9.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-13 07:46:14.376510 tgadmin-0.9.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:46:14.376510 tgadmin-0.9.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:46:14.376510 tgadmin-0.9.1/src/tgadmin/
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-03-13 07:45:56.000000 tgadmin-0.9.1/src/tgadmin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19052 2024-03-13 07:45:56.000000 tgadmin-0.9.1/src/tgadmin/tgadmin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 07:46:14.376510 tgadmin-0.9.1/src/tgadmin.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12733 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      291 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-03-13 07:46:14.000000 tgadmin-0.9.1/src/tgadmin.egg-info/top_level.txt
```

### Comparing `tgadmin-0.9.0/LICENSE` & `tgadmin-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgadmin-0.9.0/PKG-INFO` & `tgadmin-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgadmin
-Version: 0.9.0
+Version: 0.9.1
 Summary: TextGrid repository administration cli tool, based on tgclients
 Author-email: Ubbo Veentjer <veentjer@sub.uni-goettingen.de>
 Maintainer-email: Ubbo Veentjer <veentjer@sub.uni-goettingen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `tgadmin-0.9.0/README.md` & `tgadmin-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tgadmin-0.9.0/pyproject.toml` & `tgadmin-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tgadmin-0.9.0/src/tgadmin/tgadmin.py` & `tgadmin-0.9.1/src/tgadmin/tgadmin.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         tguri = tgobj.object_value.generic.generated.textgrid_uri.value
 
         click.echo(f" - {tguri}: {title}")
 
     if int(contents.hits) > limit:
         click.echo(f" ...and ({int(contents.hits) - limit}) more objects")
 
-    if not click.confirm("Do you want to delete all this objects"):
+    if not click.confirm("Do you want to delete all these objects"):
         exit(0)
     else:
 
         with click.progressbar(
             length=int(contents.hits),
             label="deleting object",
             show_eta=True,
@@ -359,15 +359,15 @@
 def put_aggregation(client, project_id, aggregation_file, threaded):
     """upload an aggregation and referenced objects recursively"""
 
     start_time = time.time()
 
     imex_map = {}
 
-    agg_meta = metafile_to_object(aggregation_file.name)
+    agg_meta = metafile_to_object(aggregation_file.name, referenced_in=aggregation_file.name)
     if not is_aggregation(agg_meta):
         exit_with_error(f"File '{aggregation_file.name}' is not of type aggregation")
 
     handle_aggregation_upload(client, project_id, aggregation_file.name, agg_meta, imex_map, threaded)
 
     imex_filename = aggregation_file.name + ".imex"
     write_imex(imex_map, imex_filename)
@@ -419,15 +419,18 @@
 def metafile_to_object(filename: str, referenced_in:str = "") -> TextgridObject:
     metafile_path = PurePath(f"{filename}.meta")
     try:
         with open(metafile_path, "rb") as meta_file:
             meta: TextgridObject = PARSER.parse(meta_file, TextgridObject)
         return meta
     except FileNotFoundError:
-        exit_with_error(f"File '{filename}' not found, which is referenced in '{referenced_in}'")
+        if filename == referenced_in:
+            exit_with_error(f"File '{filename}.meta' not found, which belongs to '{filename}'")
+        else:
+            exit_with_error(f"File '{filename}.meta' not found, which belongs to '{filename}' and is referenced in '{referenced_in}'")
 
 
 def upload_file(client: TGclient, project_id: str, data_path: PurePath, imex_map: dict, referenced_in: str = "" ) -> str:
     """upload an object and its related .meta file to specified project"""
 
     if data_path in imex_map:
         click.echo(f"file already uploaded: {data_path.name} - has uri {imex_map[data_path]}")
```

### Comparing `tgadmin-0.9.0/src/tgadmin.egg-info/PKG-INFO` & `tgadmin-0.9.1/src/tgadmin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgadmin
-Version: 0.9.0
+Version: 0.9.1
 Summary: TextGrid repository administration cli tool, based on tgclients
 Author-email: Ubbo Veentjer <veentjer@sub.uni-goettingen.de>
 Maintainer-email: Ubbo Veentjer <veentjer@sub.uni-goettingen.de>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

