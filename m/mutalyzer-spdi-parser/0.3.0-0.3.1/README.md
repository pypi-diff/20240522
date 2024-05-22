# Comparing `tmp/mutalyzer_spdi_parser-0.3.0.tar.gz` & `tmp/mutalyzer_spdi_parser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/mihai/projects/lumc/mutalyzer/spdi-parser/dist/tmpdhtt2alc/mutalyzer_spdi_parser-0.3.0.tar", last modified: Tue Jan 11 15:31:33 2022, max compression
+gzip compressed data, was "/home/mihai/projects/mutalyzer/spdi-parser/dist/.tmp-4iyvuqpn/mutalyzer_spdi_parser-0.3.1.tar", last modified: Wed May 22 13:53:00 2024, max compression
```

## Comparing `mutalyzer_spdi_parser-0.3.0.tar` & `mutalyzer_spdi_parser-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/LICENSE
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       40 2021-10-13 19:28:00.000000 mutalyzer_spdi_parser-0.3.0/MANIFEST.in
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3491 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2845 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/README.rst
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      788 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/__init__.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     2458 2021-10-13 19:28:00.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/cli.py
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3358 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/convert.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/ebnf/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      831 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/ebnf/top.g
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1980 2022-01-11 15:25:05.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/spdi_parser.py
-drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     3491 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/PKG-INFO
--rw-rw-r--   0 mihai     (1000) mihai     (1000)      531 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/SOURCES.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/dependency_links.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       74 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/entry_points.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2021-10-08 10:44:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/not-zip-safe
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       27 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/requires.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2022-01-11 15:31:33.000000 mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/top_level.txt
--rw-rw-r--   0 mihai     (1000) mihai     (1000)     1273 2022-01-11 15:31:33.169982 mutalyzer_spdi_parser-0.3.0/setup.cfg
--rw-r--r--   0 mihai     (1000) mihai     (1000)       39 2021-10-08 10:27:16.000000 mutalyzer_spdi_parser-0.3.0/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1089 2021-10-18 08:57:59.000000 mutalyzer_spdi_parser-0.3.1/LICENSE
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       40 2021-10-14 13:27:46.000000 mutalyzer_spdi_parser-0.3.1/MANIFEST.in
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3537 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2845 2021-10-18 08:58:50.000000 mutalyzer_spdi_parser-0.3.1/README.rst
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      788 2021-10-18 08:53:54.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/__init__.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     2401 2024-05-22 13:48:18.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/cli.py
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     3763 2024-05-22 13:32:38.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/convert.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/ebnf/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      888 2024-05-22 11:56:22.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/ebnf/top.g
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1980 2021-10-18 06:29:46.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/spdi_parser.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/
+-rw-r--r--   0 mihai     (1000) mihai     (1000)     3537 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/PKG-INFO
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)      553 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/SOURCES.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/dependency_links.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       73 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/entry_points.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)        1 2021-10-18 06:20:25.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/not-zip-safe
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       27 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/requires.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       22 2024-05-22 13:53:00.000000 mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/top_level.txt
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)     1273 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/setup.cfg
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)       39 2021-10-14 13:27:46.000000 mutalyzer_spdi_parser-0.3.1/setup.py
+drwxrwxr-x   0 mihai     (1000) mihai     (1000)        0 2024-05-22 13:53:00.665424 mutalyzer_spdi_parser-0.3.1/tests/
+-rw-rw-r--   0 mihai     (1000) mihai     (1000)    10289 2024-05-22 13:40:42.000000 mutalyzer_spdi_parser-0.3.1/tests/test_convert.py
```

### Comparing `mutalyzer_spdi_parser-0.3.0/LICENSE` & `mutalyzer_spdi_parser-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mutalyzer_spdi_parser-0.3.0/PKG-INFO` & `mutalyzer_spdi_parser-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mutalyzer_spdi_parser
-Version: 0.3.0
+Version: 0.3.1
 Summary: Mutalyzer SPDI variant description parser.
 Home-page: https://github.com/mutalyzer/spdi-parser
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,SPDI,description,parser,genomic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: lark>=1.0.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 Mutalyzer HGVS Parser
 =====================
 
 .. image:: https://img.shields.io/github/last-commit/mutalyzer/spdi-parser.svg
    :target: https://github.com/mutalyzer/spdi-parser/graphs/commit-activity
 .. image:: https://readthedocs.org/projects/mutalyzer-spdi-parser/badge/?version=latest
@@ -102,9 +103,7 @@
 
 .. code:: python
 
     >>> from mutalyzer_spdi_parser import to_hgvs_internal_model
     >>> model = to_hgvs_internal_model("NG_012337.3:10:C:T")
     >>> model['reference']
     {'id': 'NG_012337.3'}
-
-
```

### Comparing `mutalyzer_spdi_parser-0.3.0/README.rst` & `mutalyzer_spdi_parser-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/__init__.py` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/cli.py` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,38 +13,38 @@
 
 
 def _parse(description, grammar_path):
     """
     CLI wrapper for parsing with no conversion to model.
     """
     parse_tree = parse(description, grammar_path)
-    print("Successfully parsed:\n {}".format(description))
+    print(f"Successfully parsed:\n {description}")
     return parse_tree
 
 
 def _to_spdi_model(description):
     """
     CLI wrapper for parsing, converting, and printing the model.
     """
     parse_tree = parse(description)
     model = parse_tree_to_model(parse_tree)
-    if isinstance(model, dict) or isinstance(model, list):
+    if isinstance(model, (dict, list)):
         print(json.dumps(model, indent=2))
     else:
         print(model)
     return parse_tree
 
 
 def _to_hgvs_internal_model(description):
     """
     CLI wrapper for parsing, converting, and printing the HGVS internal model.
     """
     parse_tree = parse(description)
     model = to_hgvs_internal_model(description)
-    if isinstance(model, dict) or isinstance(model, list):
+    if isinstance(model, (dict, list)):
         print(json.dumps(model, indent=2))
     else:
         print(model)
     return parse_tree
 
 
 def _arg_parser():
@@ -84,21 +84,18 @@
     if args.cs:
         parse_tree = _to_spdi_model(args.description)
     elif args.ch:
         parse_tree = _to_hgvs_internal_model(args.description)
 
     if args.i and parse_tree:
         pydot__tree_to_png(parse_tree, args.i)
-        print("Parse tree image saved to:\n {}".format(args.i))
+        print(f"Parse tree image saved to:\n {args.i}")
 
 
 def main():
-
     parser = _arg_parser()
-
     args = parser.parse_args()
-
     _cli(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/convert.py` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/convert.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,15 +37,25 @@
     :rtype: dict
     """
     return Converter().transform(parse_tree)
 
 
 class Converter(Transformer):
     def description(self, children):
-        return {k: v for d in children for k, v in d.items()}
+        output = {k: v for d in children for k, v in d.items()}
+        output["seq_id"] = output["id"]
+        output.pop("id")
+        return output
+
+    def reference(self, children):
+        output = {"id": children[0]["seq_id"]}
+        if len(children) == 2:
+            output["id"] = children[0]["seq_id"]
+            output["selector"] = children[1]
+        return output
 
     def deleted_sequence(self, children):
         return {"deleted_sequence": children[0]}
 
     def inserted_sequence(self, children):
         return {"inserted_sequence": children[0]}
 
@@ -72,29 +82,31 @@
 
     def ID(self, name):
         return {"seq_id": name.value}
 
 
 def _to_hgvs_internal(s_m):
     m = {"type": "description_dna", "reference": {"id": s_m["seq_id"]}}
+    if s_m.get("selector"):
+        m["reference"]["selector"]= s_m["selector"]
+
     v = {"type": "deletion_insertion"}
     if s_m.get("deleted_sequence"):
         v["location"] = _range(
             s_m["position"], s_m["position"] + len(s_m["deleted_sequence"])
         )
         v["deleted"] = [{"sequence": s_m["deleted_sequence"], "source": "description"}]
     elif s_m.get("deleted_length"):
         v["location"] = _range(s_m["position"], s_m["position"] + s_m["deleted_length"])
     else:
         v["location"] = _range(s_m["position"], s_m["position"])
 
+    v["inserted"] = []
     if s_m.get("inserted_sequence"):
-        v["inserted"] = [
-            {"sequence": s_m["inserted_sequence"], "source": "description"}
-        ]
+        v["inserted"].append({"sequence": s_m["inserted_sequence"], "source": "description"})
 
     if not s_m.get("inserted_sequence") and not (
         s_m.get("deleted_sequence") or s_m.get("deleted_length")
     ):
         v["location"] = _range(s_m["position"], s_m["position"] + 1)
         v["inserted"] = [
             {
```

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/ebnf/top.g` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/ebnf/top.g`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-description: ID ":" position ":" (deleted_sequence | deleted_length)? ":" inserted_sequence?
+description: reference ":" position ":" (deleted_sequence | deleted_length)? ":" inserted_sequence?
+
+reference: ID reference? | "(" ID reference? ")"
 
 position: NUMBER
 
 deleted_sequence: sequence
 
 deleted_length: NUMBER
```

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser/spdi_parser.py` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser/spdi_parser.py`

 * *Files identical despite different names*

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/PKG-INFO` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
-Name: mutalyzer-spdi-parser
-Version: 0.3.0
+Name: mutalyzer_spdi_parser
+Version: 0.3.1
 Summary: Mutalyzer SPDI variant description parser.
 Home-page: https://github.com/mutalyzer/spdi-parser
 Author: Mihai Lefter
 Author-email: M.Lefter@lumc.nl
 License: MIT
 Keywords: Mutalyzer,HGVS,SPDI,description,parser,genomic
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: lark>=1.0.0
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
 
 Mutalyzer HGVS Parser
 =====================
 
 .. image:: https://img.shields.io/github/last-commit/mutalyzer/spdi-parser.svg
    :target: https://github.com/mutalyzer/spdi-parser/graphs/commit-activity
 .. image:: https://readthedocs.org/projects/mutalyzer-spdi-parser/badge/?version=latest
@@ -102,9 +103,7 @@
 
 .. code:: python
 
     >>> from mutalyzer_spdi_parser import to_hgvs_internal_model
     >>> model = to_hgvs_internal_model("NG_012337.3:10:C:T")
     >>> model['reference']
     {'id': 'NG_012337.3'}
-
-
```

### Comparing `mutalyzer_spdi_parser-0.3.0/mutalyzer_spdi_parser.egg-info/SOURCES.txt` & `mutalyzer_spdi_parser-0.3.1/mutalyzer_spdi_parser.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 mutalyzer_spdi_parser.egg-info/PKG-INFO
 mutalyzer_spdi_parser.egg-info/SOURCES.txt
 mutalyzer_spdi_parser.egg-info/dependency_links.txt
 mutalyzer_spdi_parser.egg-info/entry_points.txt
 mutalyzer_spdi_parser.egg-info/not-zip-safe
 mutalyzer_spdi_parser.egg-info/requires.txt
 mutalyzer_spdi_parser.egg-info/top_level.txt
-mutalyzer_spdi_parser/ebnf/top.g
+mutalyzer_spdi_parser/ebnf/top.g
+tests/test_convert.py
```

### Comparing `mutalyzer_spdi_parser-0.3.0/setup.cfg` & `mutalyzer_spdi_parser-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mutalyzer_spdi_parser
-version = 0.3.0
+version = 0.3.1
 description = Mutalyzer SPDI variant description parser.
 long_description = file: README.rst
 long_description_content_type = text/markdown
 author = Mihai Lefter
 author_email = M.Lefter@lumc.nl
 url = https://github.com/mutalyzer/spdi-parser
 keywords = Mutalyzer, HGVS, SPDI, description, parser, genomic
```

