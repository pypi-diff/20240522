# Comparing `tmp/yankee-0.1.8.tar.gz` & `tmp/yankee-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yankee-0.1.8.tar", max compression
+gzip compressed data, was "yankee-0.1.9.tar", max compression
```

## Comparing `yankee-0.1.8.tar` & `yankee-0.1.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2598 2022-06-02 21:40:55.485809 yankee-0.1.8/README.md
--rw-r--r--   0        0        0      787 2022-06-14 20:08:41.858026 yankee-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-02 21:35:29.587282 yankee-0.1.8/yankee/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 03:45:29.435723 yankee-0.1.8/yankee/base/__init__.py
--rw-r--r--   0        0        0     1479 2022-06-14 18:29:14.555322 yankee-0.1.8/yankee/base/deserializer.py
--rw-r--r--   0        0        0     5620 2022-06-14 18:33:51.232078 yankee-0.1.8/yankee/base/fields.py
--rw-r--r--   0        0        0     1105 2022-06-14 17:08:43.113322 yankee-0.1.8/yankee/base/fields_test.py
--rw-r--r--   0        0        0     3028 2022-06-14 18:45:34.650171 yankee-0.1.8/yankee/base/schema.py
--rw-r--r--   0        0        0       38 2022-06-02 21:39:24.988642 yankee-0.1.8/yankee/io/__init__.py
--rw-r--r--   0        0        0     3494 2022-06-02 21:39:46.113888 yankee-0.1.8/yankee/io/iterparse.py
--rw-r--r--   0        0        0        0 2022-05-31 16:44:31.339677 yankee-0.1.8/yankee/io/test/__init__.py
--rw-r--r--   0        0        0       44 2022-05-31 16:43:38.905917 yankee-0.1.8/yankee/io/test/sample.txt
--rw-r--r--   0        0        0      253 2022-06-02 21:39:46.118317 yankee-0.1.8/yankee/io/test/test_iterparse.py
--rw-r--r--   0        0        0       80 2022-06-14 18:35:47.337186 yankee-0.1.8/yankee/json/__init__.py
--rw-r--r--   0        0        0       67 2022-06-02 21:39:46.168198 yankee-0.1.8/yankee/json/schema/__init__.py
--rw-r--r--   0        0        0      822 2022-06-02 21:39:46.163742 yankee-0.1.8/yankee/json/schema/fields.py
--rw-r--r--   0        0        0     1452 2022-06-14 18:48:09.912349 yankee-0.1.8/yankee/json/schema/key.py
--rw-r--r--   0        0        0      208 2022-06-14 18:35:11.455026 yankee-0.1.8/yankee/json/schema/schema.py
--rw-r--r--   0        0        0     1296 2022-06-14 18:35:57.249063 yankee-0.1.8/yankee/json/schema/test_schema.py
--rw-r--r--   0        0        0      966 2022-06-14 17:57:26.794690 yankee-0.1.8/yankee/util.py
--rw-r--r--   0        0        0       94 2022-06-14 18:35:33.991234 yankee-0.1.8/yankee/xml/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 03:22:54.041149 yankee-0.1.8/yankee/xml/io/__init__.py
--rw-r--r--   0        0        0     1579 2022-06-02 21:39:46.132977 yankee-0.1.8/yankee/xml/io/aps.py
--rw-r--r--   0        0        0     1490 2022-06-02 21:39:46.135877 yankee-0.1.8/yankee/xml/io/aps_test.py
--rw-r--r--   0        0        0     1391 2022-06-02 21:39:46.126810 yankee-0.1.8/yankee/xml/io/autodetect.py
--rw-r--r--   0        0        0     7271 2022-06-02 21:39:25.201029 yankee-0.1.8/yankee/xml/io/autodetect_test.py
--rw-r--r--   0        0        0      337 2022-06-02 21:39:25.180184 yankee-0.1.8/yankee/xml/io/iterparse.py
--rw-r--r--   0        0        0      372 2022-06-02 21:39:46.131137 yankee-0.1.8/yankee/xml/io/iterparse_test.py
--rw-r--r--   0        0        0     2027 2022-06-02 21:39:46.142521 yankee-0.1.8/yankee/xml/io/process.py
--rw-r--r--   0        0        0      514 2022-06-02 21:39:25.216101 yankee-0.1.8/yankee/xml/io/sample.py
--rw-r--r--   0        0        0        0 2022-06-02 21:35:07.435665 yankee-0.1.8/yankee/xml/schema/__init__.py
--rw-r--r--   0        0        0      808 2022-06-02 21:39:46.148234 yankee-0.1.8/yankee/xml/schema/fields.py
--rw-r--r--   0        0        0      914 2022-06-14 18:43:43.332193 yankee-0.1.8/yankee/xml/schema/key.py
--rw-r--r--   0        0        0      308 2022-06-14 18:34:58.940888 yankee-0.1.8/yankee/xml/schema/schema.py
--rw-r--r--   0        0        0     2649 2022-06-14 18:45:48.261944 yankee-0.1.8/yankee/xml/schema/test_schema.py
--rw-r--r--   0        0        0     3583 2022-06-14 20:09:08.058984 yankee-0.1.8/setup.py
--rw-r--r--   0        0        0     3529 2022-06-14 20:09:08.059364 yankee-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2598 2022-06-02 21:40:55.485809 yankee-0.1.9/README.md
+-rw-r--r--   0        0        0      787 2022-06-14 20:36:54.054785 yankee-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-02 21:35:29.587282 yankee-0.1.9/yankee/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 03:45:29.435723 yankee-0.1.9/yankee/base/__init__.py
+-rw-r--r--   0        0        0     2179 2022-06-14 20:35:45.335246 yankee-0.1.9/yankee/base/deserializer.py
+-rw-r--r--   0        0        0     5620 2022-06-14 18:33:51.232078 yankee-0.1.9/yankee/base/fields.py
+-rw-r--r--   0        0        0     1105 2022-06-14 17:08:43.113322 yankee-0.1.9/yankee/base/fields_test.py
+-rw-r--r--   0        0        0     3028 2022-06-14 18:45:34.650171 yankee-0.1.9/yankee/base/schema.py
+-rw-r--r--   0        0        0       38 2022-06-02 21:39:24.988642 yankee-0.1.9/yankee/io/__init__.py
+-rw-r--r--   0        0        0     3494 2022-06-02 21:39:46.113888 yankee-0.1.9/yankee/io/iterparse.py
+-rw-r--r--   0        0        0        0 2022-05-31 16:44:31.339677 yankee-0.1.9/yankee/io/test/__init__.py
+-rw-r--r--   0        0        0       44 2022-05-31 16:43:38.905917 yankee-0.1.9/yankee/io/test/sample.txt
+-rw-r--r--   0        0        0      253 2022-06-02 21:39:46.118317 yankee-0.1.9/yankee/io/test/test_iterparse.py
+-rw-r--r--   0        0        0       80 2022-06-14 18:35:47.337186 yankee-0.1.9/yankee/json/__init__.py
+-rw-r--r--   0        0        0       67 2022-06-02 21:39:46.168198 yankee-0.1.9/yankee/json/schema/__init__.py
+-rw-r--r--   0        0        0      822 2022-06-02 21:39:46.163742 yankee-0.1.9/yankee/json/schema/fields.py
+-rw-r--r--   0        0        0     1517 2022-06-14 20:26:14.498530 yankee-0.1.9/yankee/json/schema/key.py
+-rw-r--r--   0        0        0      208 2022-06-14 18:35:11.455026 yankee-0.1.9/yankee/json/schema/schema.py
+-rw-r--r--   0        0        0     1466 2022-06-14 20:24:22.753367 yankee-0.1.9/yankee/json/schema/test_schema.py
+-rw-r--r--   0        0        0      966 2022-06-14 17:57:26.794690 yankee-0.1.9/yankee/util.py
+-rw-r--r--   0        0        0       94 2022-06-14 18:35:33.991234 yankee-0.1.9/yankee/xml/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-27 03:22:54.041149 yankee-0.1.9/yankee/xml/io/__init__.py
+-rw-r--r--   0        0        0     1579 2022-06-02 21:39:46.132977 yankee-0.1.9/yankee/xml/io/aps.py
+-rw-r--r--   0        0        0     1490 2022-06-02 21:39:46.135877 yankee-0.1.9/yankee/xml/io/aps_test.py
+-rw-r--r--   0        0        0     1391 2022-06-02 21:39:46.126810 yankee-0.1.9/yankee/xml/io/autodetect.py
+-rw-r--r--   0        0        0     7271 2022-06-02 21:39:25.201029 yankee-0.1.9/yankee/xml/io/autodetect_test.py
+-rw-r--r--   0        0        0      337 2022-06-02 21:39:25.180184 yankee-0.1.9/yankee/xml/io/iterparse.py
+-rw-r--r--   0        0        0      372 2022-06-02 21:39:46.131137 yankee-0.1.9/yankee/xml/io/iterparse_test.py
+-rw-r--r--   0        0        0     2027 2022-06-02 21:39:46.142521 yankee-0.1.9/yankee/xml/io/process.py
+-rw-r--r--   0        0        0      514 2022-06-02 21:39:25.216101 yankee-0.1.9/yankee/xml/io/sample.py
+-rw-r--r--   0        0        0        0 2022-06-02 21:35:07.435665 yankee-0.1.9/yankee/xml/schema/__init__.py
+-rw-r--r--   0        0        0      808 2022-06-02 21:39:46.148234 yankee-0.1.9/yankee/xml/schema/fields.py
+-rw-r--r--   0        0        0      914 2022-06-14 18:43:43.332193 yankee-0.1.9/yankee/xml/schema/key.py
+-rw-r--r--   0        0        0      308 2022-06-14 18:34:58.940888 yankee-0.1.9/yankee/xml/schema/schema.py
+-rw-r--r--   0        0        0     2649 2022-06-14 18:45:48.261944 yankee-0.1.9/yankee/xml/schema/test_schema.py
+-rw-r--r--   0        0        0     3583 2022-06-14 20:37:10.208568 yankee-0.1.9/setup.py
+-rw-r--r--   0        0        0     3529 2022-06-14 20:37:10.209010 yankee-0.1.9/PKG-INFO
```

### Comparing `yankee-0.1.8/README.md` & `yankee-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/pyproject.toml` & `yankee-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yankee"
-version = "0.1.8"
+version = "0.1.9"
 description = "lightweight, simple, and fast declarative XML and JSON data extraction"
 authors = ["Parker Hancock <633163+parkerhancock@users.noreply.github.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/parkerhancock/gelatin_extract"
 keywords = ["deserialization", "xml", "json", "deserialize"]
 classifiers =[
```

### Comparing `yankee-0.1.8/yankee/base/deserializer.py` & `yankee-0.1.9/yankee/base/deserializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,56 @@
-from yankee.util import camelize, underscore, do_nothing
+from yankee.util import do_nothing
+from collections.abc import Mapping, Sequence
+
+class DefaultPath():
+    def __init__(self, data_key):
+        self.key = data_key.split(".")
+
+    def __call__(self, obj):
+        try:
+            result = obj
+            for k in self.key:
+                if isinstance(result, Sequence) and k.isdigit():
+                    result = result[int(k)]
+                elif isinstance(result, Mapping):
+                    result = result[k]
+                else:
+                    result = getattr(result, k)
+            return result
+        except (AttributeError, KeyError, IndexError):
+            return None
+
 
 
 class Deserializer(object):
-    data_key = None
     many = False
 
     class Meta:
         pass
 
     def __init__(self, data_key=None, required=False):
-        if self.data_key is None:
-            self.data_key = data_key
+        self.data_key = data_key
         self.required = required
         self.bind()
 
     def bind(self, name=None, parent=None):
         self.name = name
         self.parent = parent
         if self.parent is not None:
             self.Meta = parent.Meta
         self.accessor = self.make_accessor()
         return self
 
     def make_accessor(self):
-        return do_nothing
+        if self.data_key == False:
+            return do_nothing
+        key = self.data_key or self.name
+        if key is None:
+            return do_nothing
+        return DefaultPath(key)
 
     def load(self, obj):
         plucked_obj = self.get_obj(obj)
         loaded_obj = self.deserialize(plucked_obj)
         return self.post_load(loaded_obj)
 
     def deserialize(self, obj):
```

### Comparing `yankee-0.1.8/yankee/base/fields.py` & `yankee-0.1.9/yankee/base/fields.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/base/fields_test.py` & `yankee-0.1.9/yankee/base/fields_test.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/base/schema.py` & `yankee-0.1.9/yankee/base/schema.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/io/iterparse.py` & `yankee-0.1.9/yankee/io/iterparse.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/json/schema/fields.py` & `yankee-0.1.9/yankee/json/schema/fields.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/json/schema/key.py` & `yankee-0.1.9/yankee/json/schema/key.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,11 +36,13 @@
             if self.many:
                 return list()
             return None
 
 
 class JsonMixin(object):
     def make_accessor(self):
+        if self.data_key == False:
+            return do_nothing
         data_key = self.data_key or self.name
         if data_key is None:
             return do_nothing
         return JsonPath(camelize(data_key), many=self.many)
```

### Comparing `yankee-0.1.8/yankee/json/schema/test_schema.py` & `yankee-0.1.9/yankee/json/schema/test_schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,31 +21,37 @@
 class NameSchema(f.Combine):
     part1 = f.Str()
     part2 = f.Str()
 
     def combine_func(self, obj):
         return f"{obj['part1']} {obj['part2']}"
 
+class SubSchema(Schema):
+    string = f.Str()
+    float = f.Float()
 
 class ExampleSchema(Schema):
     string = f.Str()
     date_time = f.DT()
     date = f.Date()
     booleans = f.List(f.Bool, data_key="booleans")
     float = f.Float()
     int = f.Int()
     exists = f.Exists()
     does_not_exist = f.Exists()
     name = NameSchema()
+    sub = SubSchema(False)
 
 
 def test_fields():
-    data = ExampleSchema().load(doc)
+    schema = ExampleSchema()
+    data = schema.load(doc)
     assert data["string"] == "Some String Data"
     assert data["date_time"] == datetime.datetime(2021, 5, 4, 12, 5)
     assert data["date"] == datetime.date(2021, 5, 4)
     assert data["booleans"] == [True, True, False, False]
     assert data["float"] - 1.234 < 0.001
     assert data["int"] == 23
     assert data["exists"] == True
     assert data["does_not_exist"] == False
     assert data["name"] == "George Burdell"
+    assert data['sub']['string'] == "Some String Data"
```

### Comparing `yankee-0.1.8/yankee/util.py` & `yankee-0.1.9/yankee/util.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/aps.py` & `yankee-0.1.9/yankee/xml/io/aps.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/aps_test.py` & `yankee-0.1.9/yankee/xml/io/aps_test.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/autodetect.py` & `yankee-0.1.9/yankee/xml/io/autodetect.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/autodetect_test.py` & `yankee-0.1.9/yankee/xml/io/autodetect_test.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/process.py` & `yankee-0.1.9/yankee/xml/io/process.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/io/sample.py` & `yankee-0.1.9/yankee/xml/io/sample.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/schema/fields.py` & `yankee-0.1.9/yankee/xml/schema/fields.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/schema/key.py` & `yankee-0.1.9/yankee/xml/schema/key.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/yankee/xml/schema/test_schema.py` & `yankee-0.1.9/yankee/xml/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `yankee-0.1.8/setup.py` & `yankee-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 {'': ['*']}
 
 install_requires = \
 ['lxml>=4.8.0,<5.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'yankee',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'lightweight, simple, and fast declarative XML and JSON data extraction',
     'long_description': '# Yankee - Simple Declarative Data Extraction from XML and JSON\n\nThis is kind of like Marshmallow, but only does deserialization. What it lacks in reversibility, it makes up for in speed. Schemas are compiled in advance allowing\ndata extraction to occur very quickly.\n\n## Motivation\n\nI have another package called patent_client. I also do a lot with legal data, some of which is in XML, and some of which is in JSON. But there\'s a lot of it. And I mean *a lot*, so speed matters.\n\n## Quick Start\n\nThere are two main modules: `yankee.json.schema` and `yankee.xml.schema`. Those modules support defining class-style deserializers. Both start by subclassing a `Schema` class, and then defining attributes from the `fields` submodule.\n\n### JSON Deserializer Example\n\n```python\n    from yankee.json import Schema, fields\n\n    class JsonExample(Schema):\n        name = fields.String()\n        birthday = fields.Date("birthdate")\n        deep_data = fields.Int("something.0.many.levels.deep")\n\n    obj = {\n        "name": "Johnny Appleseed",\n        "birthdate": "2000-01-01",\n        "something": [\n            {"many": {\n                "levels": {\n                    "deep": 123\n                }\n            }}\n        ]\n    }\n\n    JsonExample().deserialize(obj)\n    # Returns\n    {\n        "name": "Johnny Appleseed",\n        "birthday": datetime.date(2000, 1, 1),\n        "deep_data": 123\n    }\n\n```\n\nFor JSON, the attributes are filled by pulling values off of the JSON object. If no\npath is provided, then the attribute name is used. Otherwise, a dotted string\ncan be used to pluck an item from the JSON object.\n\n### XML Deserializer Example\n\n```python\n    import lxml.etree as ET\n    from yankee.xml import Schema, fields\n\n    class XmlExample(Schema):\n        name = fields.String("./name")\n        birthday = fields.Date("./birthdate")\n        deep_data = fields.Int("./something/many/levels/deep")\n\n    obj = ET.fromstring(b"""\n    <xmlObject>\n        <name>Johnny Appleseed</name>\n        <birthdate>2000-01-01</birthdate>\n        <something>\n            <many>\n                <levels>\n                    <deep>123</deep>\n                </levels>\n            </many>\n        </something>\n    </xmlObject>\n    """.strip())\n\n    XmlExample().deserialize(obj)\n    # Returns\n    {\n        "name": "Johnny Appleseed",\n        "birthday": datetime.date(2000, 1, 1),\n        "deep_data": 123\n    }\n```\n\nFor XML, the attributes are filled using XPath expressions. If no path is provided,\nthen the entire object is passed to the field (no implicit paths). Any valid Xpath\nexpression can be used.\n\n',
     'author': 'Parker Hancock',
     'author_email': '633163+parkerhancock@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/parkerhancock/gelatin_extract',
```

### Comparing `yankee-0.1.8/PKG-INFO` & `yankee-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yankee
-Version: 0.1.8
+Version: 0.1.9
 Summary: lightweight, simple, and fast declarative XML and JSON data extraction
 Home-page: https://github.com/parkerhancock/gelatin_extract
 License: Apache Software License 2.0
 Keywords: deserialization,xml,json,deserialize
 Author: Parker Hancock
 Author-email: 633163+parkerhancock@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
```

