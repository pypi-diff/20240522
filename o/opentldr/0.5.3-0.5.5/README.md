# Comparing `tmp/opentldr-0.5.3.tar.gz` & `tmp/opentldr-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentldr-0.5.3.tar", last modified: Tue May 21 13:51:58 2024, max compression
+gzip compressed data, was "opentldr-0.5.5.tar", last modified: Wed May 22 14:58:40 2024, max compression
```

## Comparing `opentldr-0.5.3.tar` & `opentldr-0.5.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 13:51:49.000000 opentldr-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:49.000000 opentldr-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-21 13:51:58.714570 opentldr-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-21 13:51:49.000000 opentldr-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 13:51:49.000000 opentldr-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:51:58.714570 opentldr-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.706570 opentldr-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.710570 opentldr-0.5.3/src/opentldr/
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/AbstractDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/DataRepoJson.py
--rw-r--r--   0 runner    (1001) docker     (127)    28658 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/FileSystemDataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    37262 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/KnowledgeGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/S3DataRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 13:51:49.000000 opentldr-0.5.3/src/opentldr/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/src/opentldr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 13:51:58.000000 opentldr-0.5.3/src/opentldr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:51:58.714570 opentldr-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_contentrepo.py
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_knowledgegraph.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-21 13:51:49.000000 opentldr-0.5.3/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 14:58:36.000000 opentldr-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:36.000000 opentldr-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-22 14:58:40.726451 opentldr-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-05-22 14:58:36.000000 opentldr-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-22 14:58:36.000000 opentldr-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:58:40.726451 opentldr-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.718450 opentldr-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.722450 opentldr-0.5.5/src/opentldr/
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/AbstractDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/DataRepoJson.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28557 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/FileSystemDataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37495 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/KnowledgeGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/S3DataRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-22 14:58:36.000000 opentldr-0.5.5/src/opentldr/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/src/opentldr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 14:58:40.000000 opentldr-0.5.5/src/opentldr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:58:40.726451 opentldr-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_contentrepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_knowledgegraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-22 14:58:36.000000 opentldr-0.5.5/tests/test_workflow.py
```

### Comparing `opentldr-0.5.3/LICENSE` & `opentldr-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/PKG-INFO` & `opentldr-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.3
+Version: 0.5.5
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.3/README.md` & `opentldr-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/pyproject.toml` & `opentldr-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "opentldr"
-version = "0.5.3"
+version = "0.5.5"
 authors = [
   { name="Chris Argenta", email="cargenta@rockfishresearch.com" },
 ]
 description = "An open framework for creation of a Tailored Daily Report."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `opentldr-0.5.3/src/opentldr/AbstractDataRepo.py` & `opentldr-0.5.5/src/opentldr/AbstractDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/src/opentldr/DataRepo.py` & `opentldr-0.5.5/src/opentldr/DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/src/opentldr/DataRepoJson.py` & `opentldr-0.5.5/src/opentldr/DataRepoJson.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/src/opentldr/Domain.py` & `opentldr-0.5.5/src/opentldr/Domain.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,39 +582,40 @@
     BasedOn edges connect a TldrEntry node to a Recommendation node to indicate why that
     entry is being included in the TLDR and may be used for things like ordering the entries
     to show the most recommended first.
     '''
     pass
 
 
-class TldrEntry(nm.StructuredNode, OpenTldrMeta, OpenTldrNode):
+class TldrEntry(nm.StructuredNode, OpenTldrMeta, OpenTldrNode, Scored):
     '''
     TldrEntry is one record within a TLDR. In general, there is a one-to-one relationship
     between each TldrEntry, Recommendation, and Summary such that each record within a TLDR
     has a score for the Recommendation, a text blurb from the Summary, and a connection back
     to the original Content (from both the Recommendation and Summary).
     '''
-    link = nm.StringProperty(required=False)
+    link = nm.StringProperty(required=True)
+    title = nm.StringProperty(required=True)
+    type = nm.StringProperty(required=False)
+    summary=nm.StringProperty(required=True)
 
-    includes = nm.RelationshipTo(Summary, 'INCLUDES', model=Includes, cardinality=One)
-    based_on = nm.RelationshipTo(Recommendation, 'BASED_ON', model=BasedOn, cardinality=One)
+    includes = nm.RelationshipTo(Summary, 'INCLUDES', model=Includes, cardinality=ZeroOrOne)
+    based_on = nm.RelationshipTo(Recommendation, 'BASED_ON', model=BasedOn, cardinality=ZeroOrOne)
 
     def get_includes(self) -> Summary:
         return self.includes.single()
     
     def get_based_on(self) -> Recommendation:
         return self.based_on.single()
 
     def to_text(self) -> str:
-        return "The entry '{entry}' summarizes {content_type} '{content_title}' and {score} relevance to the request '{request}'.".format(
-            entry=self.includes.single().summarizes.single().title,
-            content_title=self.includes.single().summarizes.single().title,
-            content_type= self.includes.single().summarizes.single().type,
-            request= self.based_on.single().relates_to.single().title,
-            score=self.based_on.single().score_to_text())
+        return "The entry summarizes {content_type} '{content_title}' and {score} relevance to the request.".format(
+            content_title=self.title,
+            content_type= self.type,
+            score=self.score_to_text())
 
 
 class Contains(nm.StructuredRel, OpenTldrMeta, OpenTldrEdge, Scored):
     '''
     Connects a Tldr to each of the TldrEntry objects that makes it up. The assumption
     here is that the score property (float 0.0 - 1.0) on the edge provides a descending ordering for
     the entries connected by these links.
```

### Comparing `opentldr-0.5.3/src/opentldr/FileSystemDataRepo.py` & `opentldr-0.5.5/src/opentldr/FileSystemDataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/src/opentldr/KnowledgeGraph.py` & `opentldr-0.5.5/src/opentldr/KnowledgeGraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -857,15 +857,20 @@
             self.delete_tldr(tldr)
 
     # -----------------
     # Tldr Entries
     # -----------------
 
     def add_entry_to_tldr(self, tldr:Tldr, score:float, recommendation:Recommendation, summary:Summary, content:Content) -> TldrEntry:
-        tldr_entry=TldrEntry(link=content.url).save()
+        tldr_entry=TldrEntry(link=content.url,
+                            title=content.title,
+                            type=content.type,
+                            score=recommendation.score,
+                            summary=summary.text,
+                             ).save()
         tldr_entry.includes.connect(summary)
         tldr_entry.based_on.connect(recommendation)
         tldr.contains.connect(tldr_entry, {'score': score })
         return tldr_entry
 
     def get_tldr_entry_by_uid(self, uid:str) -> Tldr:
         tldr_entry = TldrEntry.nodes.get_or_none(uid=uid)
```

### Comparing `opentldr-0.5.3/src/opentldr/S3DataRepo.py` & `opentldr-0.5.5/src/opentldr/S3DataRepo.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/src/opentldr/Workflow.py` & `opentldr-0.5.5/src/opentldr/Workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,14 @@
         workflow["Output"] = output_folder
         nblist = []
         for notebook in notebook_order:
             nblist.append([notebook, variables])
         workflow["Notebooks"] = nblist
         return cls(workflow)
 
-    def import_json(self,j):                        # TODO: This method doesn't import anything to anywhere
-        output = j["Output"]                        # TODO: Never used
-        notebooks:list[list] = j["Notebooks"]
-        for step in notebooks:
-            notebook:str=step[0]
-            config:dict=step[1]
-            print ("Notebook: {notebook} is config is: {config}".format(notebook=notebook,config=config))
-
     def verify(self):
         '''
         Walk thru the structure of the workflow and ensure it is setup correctly.
         '''
         has_errors:bool=False
         errors:str=""
```

### Comparing `opentldr-0.5.3/src/opentldr.egg-info/PKG-INFO` & `opentldr-0.5.5/src/opentldr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentldr
-Version: 0.5.3
+Version: 0.5.5
 Summary: An open framework for creation of a Tailored Daily Report.
 Author-email: Chris Argenta <cargenta@rockfishresearch.com>
 Project-URL: Source, https://github.com/RockfishResearch/OpenTLDR-Core.git
 Project-URL: Issues, https://github.com/RockfishResearch/OpenTLDR-Core/issues
 Project-URL: Documentation, http://www.opentldr.org/docs
 Project-URL: Homepage, http://www.opentldr.org
 Classifier: Programming Language :: Python :: 3
```

### Comparing `opentldr-0.5.3/src/opentldr.egg-info/SOURCES.txt` & `opentldr-0.5.5/src/opentldr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/tests/test_knowledgegraph.py` & `opentldr-0.5.5/tests/test_knowledgegraph.py`

 * *Files identical despite different names*

### Comparing `opentldr-0.5.3/tests/test_workflow.py` & `opentldr-0.5.5/tests/test_workflow.py`

 * *Files identical despite different names*

