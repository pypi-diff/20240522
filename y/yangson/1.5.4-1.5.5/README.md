# Comparing `tmp/yangson-1.5.4.tar.gz` & `tmp/yangson-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yangson-1.5.4.tar", max compression
+gzip compressed data, was "yangson-1.5.5.tar", max compression
```

## Comparing `yangson-1.5.4.tar` & `yangson-1.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    35147 2024-02-29 08:55:55.092925 yangson-1.5.4/COPYING
--rw-r--r--   0        0        0     7650 2024-02-29 08:55:55.093015 yangson-1.5.4/COPYING.LESSER
--rw-r--r--   0        0        0     1022 2024-02-29 08:55:55.093144 yangson-1.5.4/README.rst
--rw-r--r--   0        0        0      768 2024-05-07 17:21:16.136034 yangson-1.5.4/pyproject.toml
--rw-r--r--   0        0        0       43 2024-02-29 08:55:55.099132 yangson-1.5.4/yangson/__init__.py
--rw-r--r--   0        0        0     6474 2024-02-29 08:55:55.099203 yangson-1.5.4/yangson/__main__.py
--rw-r--r--   0        0        0     5768 2024-02-29 08:55:55.099269 yangson-1.5.4/yangson/constraint.py
--rw-r--r--   0        0        0     9850 2024-02-29 08:55:55.099326 yangson-1.5.4/yangson/convert8525.py
--rw-r--r--   0        0        0     7787 2024-02-29 08:55:55.099400 yangson-1.5.4/yangson/datamodel.py
--rw-r--r--   0        0        0    36945 2024-02-29 08:55:55.099523 yangson-1.5.4/yangson/datatype.py
--rw-r--r--   0        0        0     3442 2024-02-29 08:55:55.099596 yangson-1.5.4/yangson/enumerations.py
--rw-r--r--   0        0        0    15491 2024-02-29 08:55:55.099675 yangson-1.5.4/yangson/exceptions.py
--rw-r--r--   0        0        0    53791 2024-02-29 08:55:55.099794 yangson-1.5.4/yangson/instance.py
--rw-r--r--   0        0        0     3491 2024-02-29 08:55:55.099867 yangson-1.5.4/yangson/instvalue.py
--rw-r--r--   0        0        0     4314 2024-02-29 08:55:55.099930 yangson-1.5.4/yangson/nodeset.py
--rw-r--r--   0        0        0     7621 2024-02-29 08:55:55.099997 yangson-1.5.4/yangson/parser.py
--rw-r--r--   0        0        0    23038 2024-02-29 08:55:55.100080 yangson-1.5.4/yangson/schemadata.py
--rw-r--r--   0        0        0    68715 2024-02-29 08:55:55.100224 yangson-1.5.4/yangson/schemanode.py
--rw-r--r--   0        0        0    12000 2024-02-29 08:55:55.100314 yangson-1.5.4/yangson/schpattern.py
--rw-r--r--   0        0        0    12882 2024-02-29 08:55:55.100390 yangson-1.5.4/yangson/statement.py
--rw-r--r--   0        0        0     2935 2024-02-29 08:55:55.100454 yangson-1.5.4/yangson/typealiases.py
--rw-r--r--   0        0        0     2243 2024-02-29 08:55:55.100515 yangson-1.5.4/yangson/xmlparser.py
--rw-r--r--   0        0        0    27458 2024-02-29 08:55:55.100602 yangson-1.5.4/yangson/xpathast.py
--rw-r--r--   0        0        0    15191 2024-02-29 08:55:55.100699 yangson-1.5.4/yangson/xpathparser.py
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 yangson-1.5.4/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-02-29 08:55:55.092925 yangson-1.5.5/COPYING
+-rw-r--r--   0        0        0     7650 2024-02-29 08:55:55.093015 yangson-1.5.5/COPYING.LESSER
+-rw-r--r--   0        0        0     1022 2024-02-29 08:55:55.093144 yangson-1.5.5/README.rst
+-rw-r--r--   0        0        0      768 2024-05-22 06:13:07.778939 yangson-1.5.5/pyproject.toml
+-rw-r--r--   0        0        0       43 2024-02-29 08:55:55.099132 yangson-1.5.5/yangson/__init__.py
+-rw-r--r--   0        0        0     6474 2024-02-29 08:55:55.099203 yangson-1.5.5/yangson/__main__.py
+-rw-r--r--   0        0        0     5768 2024-02-29 08:55:55.099269 yangson-1.5.5/yangson/constraint.py
+-rw-r--r--   0        0        0     9850 2024-02-29 08:55:55.099326 yangson-1.5.5/yangson/convert8525.py
+-rw-r--r--   0        0        0     7787 2024-02-29 08:55:55.099400 yangson-1.5.5/yangson/datamodel.py
+-rw-r--r--   0        0        0    36945 2024-02-29 08:55:55.099523 yangson-1.5.5/yangson/datatype.py
+-rw-r--r--   0        0        0     3442 2024-02-29 08:55:55.099596 yangson-1.5.5/yangson/enumerations.py
+-rw-r--r--   0        0        0    15491 2024-02-29 08:55:55.099675 yangson-1.5.5/yangson/exceptions.py
+-rw-r--r--   0        0        0    53791 2024-02-29 08:55:55.099794 yangson-1.5.5/yangson/instance.py
+-rw-r--r--   0        0        0     3491 2024-02-29 08:55:55.099867 yangson-1.5.5/yangson/instvalue.py
+-rw-r--r--   0        0        0     4314 2024-02-29 08:55:55.099930 yangson-1.5.5/yangson/nodeset.py
+-rw-r--r--   0        0        0     7621 2024-02-29 08:55:55.099997 yangson-1.5.5/yangson/parser.py
+-rw-r--r--   0        0        0    23038 2024-02-29 08:55:55.100080 yangson-1.5.5/yangson/schemadata.py
+-rw-r--r--   0        0        0    68715 2024-02-29 08:55:55.100224 yangson-1.5.5/yangson/schemanode.py
+-rw-r--r--   0        0        0    12000 2024-02-29 08:55:55.100314 yangson-1.5.5/yangson/schpattern.py
+-rw-r--r--   0        0        0    12882 2024-02-29 08:55:55.100390 yangson-1.5.5/yangson/statement.py
+-rw-r--r--   0        0        0     2935 2024-02-29 08:55:55.100454 yangson-1.5.5/yangson/typealiases.py
+-rw-r--r--   0        0        0     2243 2024-02-29 08:55:55.100515 yangson-1.5.5/yangson/xmlparser.py
+-rw-r--r--   0        0        0    27458 2024-02-29 08:55:55.100602 yangson-1.5.5/yangson/xpathast.py
+-rw-r--r--   0        0        0    15191 2024-02-29 08:55:55.100699 yangson-1.5.5/yangson/xpathparser.py
+-rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 yangson-1.5.5/PKG-INFO
```

### Comparing `yangson-1.5.4/COPYING` & `yangson-1.5.5/COPYING`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/COPYING.LESSER` & `yangson-1.5.5/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/README.rst` & `yangson-1.5.5/README.rst`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/pyproject.toml` & `yangson-1.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yangson"
-version = "1.5.4"
+version = "1.5.5"
 description = "Library for working with data modelled in YANG"
 authors = ["Ladislav Lhotka <ladislav@lhotka.name>"]
 license = "GNU Lesser General Public License v3 (LGPLv3)"
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `yangson-1.5.4/yangson/__main__.py` & `yangson-1.5.5/yangson/__main__.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/constraint.py` & `yangson-1.5.5/yangson/constraint.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/convert8525.py` & `yangson-1.5.5/yangson/convert8525.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/datamodel.py` & `yangson-1.5.5/yangson/datamodel.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/datatype.py` & `yangson-1.5.5/yangson/datatype.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/enumerations.py` & `yangson-1.5.5/yangson/enumerations.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/exceptions.py` & `yangson-1.5.5/yangson/exceptions.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/instance.py` & `yangson-1.5.5/yangson/instance.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/instvalue.py` & `yangson-1.5.5/yangson/instvalue.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/nodeset.py` & `yangson-1.5.5/yangson/nodeset.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/parser.py` & `yangson-1.5.5/yangson/parser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/schemadata.py` & `yangson-1.5.5/yangson/schemadata.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/schemanode.py` & `yangson-1.5.5/yangson/schemanode.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/schpattern.py` & `yangson-1.5.5/yangson/schpattern.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/statement.py` & `yangson-1.5.5/yangson/statement.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/typealiases.py` & `yangson-1.5.5/yangson/typealiases.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/xmlparser.py` & `yangson-1.5.5/yangson/xmlparser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/xpathast.py` & `yangson-1.5.5/yangson/xpathast.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/yangson/xpathparser.py` & `yangson-1.5.5/yangson/xpathparser.py`

 * *Files identical despite different names*

### Comparing `yangson-1.5.4/PKG-INFO` & `yangson-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yangson
-Version: 1.5.4
+Version: 1.5.5
 Summary: Library for working with data modelled in YANG
 License: GNU Lesser General Public License v3 (LGPLv3)
 Author: Ladislav Lhotka
 Author-email: ladislav@lhotka.name
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

