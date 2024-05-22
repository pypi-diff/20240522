# Comparing `tmp/odio-0.0.8.tar.gz` & `tmp/odio-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odio-0.0.8.tar", last modified: Sun Aug  2 08:37:37 2015, max compression
+gzip compressed data, was "dist/odio-0.0.9.tar", last modified: Fri Mar  3 14:44:47 2017, max compression
```

## Comparing `odio-0.0.8.tar` & `odio-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2015-08-02 08:37:37.000000 odio-0.0.8/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1328 2015-08-02 08:34:56.000000 odio-0.0.8/setup.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    40346 2015-05-25 19:55:08.000000 odio-0.0.8/versioneer.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       74 2015-05-25 20:20:55.000000 odio-0.0.8/setup.cfg
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      904 2015-08-02 08:37:37.000000 odio-0.0.8/PKG-INFO
-drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2015-08-02 08:37:37.000000 odio-0.0.8/odio/
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      417 2015-08-02 08:37:37.000000 odio-0.0.8/odio/_version.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      456 2015-08-01 09:52:12.000000 odio-0.0.8/odio/__init__.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    15827 2015-08-01 18:13:37.000000 odio-0.0.8/odio/spreadsheet.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)        0 2015-08-01 09:25:32.000000 odio-0.0.8/odio/common.py
--rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    45666 2015-08-01 20:50:33.000000 odio-0.0.8/odio/text.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2017-03-03 14:44:47.000000 odio-0.0.9/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)       74 2017-03-03 11:37:31.000000 odio-0.0.9/setup.cfg
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     1349 2017-03-03 11:37:31.000000 odio-0.0.9/setup.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    40346 2017-03-03 11:37:31.000000 odio-0.0.9/versioneer.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2017-03-03 14:44:47.000000 odio-0.0.9/odio/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      417 2017-03-03 14:44:47.000000 odio-0.0.9/odio/_version.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     2247 2017-03-03 11:37:31.000000 odio-0.0.9/odio/common.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2017-03-03 14:44:47.000000 odio-0.0.9/odio/v1_2/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)    17408 2017-03-03 13:09:13.000000 odio-0.0.9/odio/v1_2/__init__.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     2562 2017-03-03 13:49:24.000000 odio-0.0.9/odio/__init__.py
+drwxrwxr-x   0 tlocke    (1000) tlocke    (1000)        0 2017-03-03 14:44:47.000000 odio-0.0.9/odio/v1_1/
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)     8961 2017-03-03 13:10:00.000000 odio-0.0.9/odio/v1_1/__init__.py
+-rw-rw-r--   0 tlocke    (1000) tlocke    (1000)      900 2017-03-03 14:44:47.000000 odio-0.0.9/PKG-INFO
```

### Comparing `odio-0.0.8/setup.py` & `odio-0.0.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,11 +31,11 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: Implementation",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
     ],
-    keywords="odf ods odt",
-    packages=("odio",),
+    keywords="odf ods",
+    packages=("odio", "odio.v1_1", "odio.v1_2"),
     install_requires=['six'],
 )
```

### Comparing `odio-0.0.8/versioneer.py` & `odio-0.0.9/versioneer.py`

 * *Files identical despite different names*

### Comparing `odio-0.0.8/PKG-INFO` & `odio-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 1.1
 Name: odio
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for the input / output of ODF documents.
 Home-page: https://github.com/tlocke/odio
 Author: Tony Locke
 Author-email: tlocke@tlocke.org.uk
 License: MIT
 Description: UNKNOWN
-Keywords: odf ods odt
+Keywords: odf ods
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `odio-0.0.8/odio/spreadsheet.py` & `odio-0.0.9/odio/v1_2/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,81 +1,74 @@
 import xml.dom.minidom
+from xml.dom import Node
 import datetime
 import zipfile
 import odio
-
-
-class Formula():
-    def __init__(self, formula):
-        self.formula = formula
-
-    def __repr__(self):
-        return "odio.Formula('" + self.formula + "')"
-
-    def __str__(self):
-        return self.formula
-
-    def __eq__(self, other):
-        return isinstance(other, Formula) and self.formula == other.formula
+from odio.common import P, H, Span
 
 
 class SpreadsheetWriter():
-    def __init__(self, f, version='1.2'):
+    def __init__(self, f, compressed):
         self.f = f
-        self.z = zipfile.ZipFile(f, 'w')
+        if compressed:
+            compression = zipfile.ZIP_DEFLATED
+        else:
+            compression = zipfile.ZIP_STORED
+        self.z = zipfile.ZipFile(f, 'w', compression)
         self.z.writestr(
             'mimetype', 'application/vnd.oasis.opendocument.spreadsheet')
-        if version == '1.1':
-            self.z.writestr(
-                'META-INF/manifest.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'META-INF/manifest.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <manifest:manifest
+    manifest:version="1.2"
     xmlns:manifest="urn:oasis:names:tc:opendocument:xmlns:manifest:1.0">
   <manifest:file-entry
       manifest:full-path="/"
       manifest:media-type="application/vnd.oasis.opendocument.spreadsheet"/>
   <manifest:file-entry
       manifest:full-path="settings.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="content.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="meta.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="styles.xml" manifest:media-type="text/xml"/>
-</manifest:manifest>""")
-            self.z.writestr(
-                'meta.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+</manifest:manifest>
+""")
+        self.z.writestr(
+            'meta.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-meta
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     xmlns:dc="http://purl.org/dc/elements/1.1/"
     xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
-    office:version="1.1">
+    office:version="1.2">
   <office:meta>
-    <meta:generator>ODFIO</meta:generator>
+      <meta:generator>Odio</meta:generator>
   </office:meta>
 </office:document-meta>
 """)
 
-            self.z.writestr(
-                'settings.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'settings.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-settings
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
-    office:version="1.1">
+    office:version="1.2">
 </office:document-settings>
 """)
 
-            self.z.writestr(
-                'styles.xml', """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'styles.xml', """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-styles
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
     xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
     xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
     xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
     xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
@@ -90,19 +83,19 @@
     xmlns:math="http://www.w3.org/1998/Math/MathML"
     xmlns:form="urn:oasis:names:tc:opendocument:xmlns:form:1.0"
     xmlns:script="urn:oasis:names:tc:opendocument:xmlns:script:1.0"
     xmlns:dom="http://www.w3.org/2001/xml-events"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
     xmlns:xhtml="http://www.w3.org/1999/xhtml"
     xmlns:css3t="http://www.w3.org/TR/css3-text/"
-    office:version="1.1">
+    office:version="1.2">
 </office:document-styles>
 """)
-            self.doc = xml.dom.minidom.parseString(
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.doc = xml.dom.minidom.parseString(
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-content
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
     xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
     xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
     xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
     xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
@@ -120,15 +113,15 @@
     xmlns:dom="http://www.w3.org/2001/xml-events"
     xmlns:xforms="http://www.w3.org/2002/xforms"
     xmlns:xsd="http://www.w3.org/2001/XMLSchema"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
     xmlns:xhtml="http://www.w3.org/1999/xhtml"
     xmlns:css3t="http://www.w3.org/TR/css3-text/"
-    office:version="1.1">
+    office:version="1.2">
   <office:scripts/>
   <office:automatic-styles>
     <number:date-style style:name="date">
       <number:year number:style="long"/>
       <number:text>-</number:text>
       <number:month number:style="long"/>
       <number:text>-</number:text>
@@ -142,64 +135,153 @@
       style:parent-style-name="Default" style:data-style-name="date"/>
   </office:automatic-styles>
   <office:body>
     <office:spreadsheet>
     </office:spreadsheet>
   </office:body>
 </office:document-content>""")
-        elif version == '1.2':
-            self.z.writestr(
-                'META-INF/manifest.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.spreadsheet_elem = self.doc.getElementsByTagName(
+            'office:spreadsheet')[0]
+
+    def append_table(self, name):
+        table_elem = self.spreadsheet_elem.appendChild(
+            self.doc.createElement('table:table'))
+        table_elem.setAttribute('table:name', name)
+        table_elem.appendChild(self.doc.createElement('table:table-column'))
+        return TableWriter(self.doc, table_elem)
+
+    def close(self):
+        self.z.writestr('content.xml', self.doc.toprettyxml(encoding='utf-8'))
+        self.z.close()
+        self.f.close()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.close()
+
+
+class TableWriter():
+    def __init__(self, doc, table_elem):
+        self.doc = doc
+        self.table_elem = table_elem
+
+    def append_row(self, vals):
+        row_elem = self.table_elem.appendChild(
+            self.doc.createElement('table:table-row'))
+        for val in vals:
+            cell_elem = row_elem.appendChild(
+                self.doc.createElement('table:table-cell'))
+            if isinstance(val, datetime.datetime):
+                cell_elem.setAttribute('office:value-type', 'date')
+                cell_elem.setAttribute(
+                    'office:date-value', val.strftime('%Y-%m-%dT%H:%M:%S'))
+                cell_elem.setAttribute('table:style-name', 'cell_date')
+            elif isinstance(val, str):
+                cell_elem.setAttribute('office:value-type', 'string')
+                cell_elem.setAttribute('office:string-value', val)
+            elif isinstance(val, (float, int)):
+                cell_elem.setAttribute('office:value-type', 'float')
+                cell_elem.setAttribute('office:value', str(val))
+            elif isinstance(val, odio.Formula):
+                cell_elem.setAttribute('table:formula', 'of:' + str(val))
+            else:
+                raise Exception("Type of '" + str(val) + "' not recognized.")
+
+
+class SpreadsheetReader():
+    def __init__(self, spreadsheet_elem):
+        self.tables = []
+        for table_elem in spreadsheet_elem.getElementsByTagName('table:table'):
+            self.tables.append(TableReader(table_elem))
+
+
+class TableReader():
+    def __init__(self, table_elem):
+        self.name = table_elem.getAttribute('table:name')
+        self.rows = []
+        for row_elem in table_elem.getElementsByTagName('table:table-row'):
+            row = []
+            self.rows.append(row)
+            for cell_elem in row_elem.getElementsByTagName('table:table-cell'):
+                if cell_elem.hasAttribute('table:formula'):
+                    formula = cell_elem.getAttribute('table:formula')
+                    eq_idx = formula.index('=')
+                    row.append(odio.Formula(formula[eq_idx:]))
+                else:
+                    val_type = cell_elem.getAttribute('office:value-type')
+                    if val_type == 'date':
+                        row.append(
+                            datetime.datetime.strptime(
+                                cell_elem.getAttribute('office:date-value'),
+                                '%Y-%m-%dT%H:%M:%S'))
+                    elif val_type == 'string':
+                        row.append(
+                            cell_elem.getAttribute('office:string-value'))
+                    elif val_type == 'float':
+                        row.append(
+                            float(cell_elem.getAttribute('office:value')))
+
+
+class TextWriter():
+    def __init__(self, f):
+        self.f = f
+        self.z = zipfile.ZipFile(f, 'w')
+        self.z.writestr(
+            'mimetype', 'application/vnd.oasis.opendocument.text')
+        self.z.writestr(
+            'META-INF/manifest.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <manifest:manifest
     manifest:version="1.2"
     xmlns:manifest="urn:oasis:names:tc:opendocument:xmlns:manifest:1.0">
   <manifest:file-entry
       manifest:full-path="/"
-      manifest:media-type="application/vnd.oasis.opendocument.spreadsheet"/>
+      manifest:media-type="application/vnd.oasis.opendocument.text"/>
   <manifest:file-entry
       manifest:full-path="settings.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="content.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="meta.xml" manifest:media-type="text/xml"/>
   <manifest:file-entry
       manifest:full-path="styles.xml" manifest:media-type="text/xml"/>
 </manifest:manifest>
 """)
-            self.z.writestr(
-                'meta.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'meta.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-meta
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     xmlns:dc="http://purl.org/dc/elements/1.1/"
     xmlns:meta="urn:oasis:names:tc:opendocument:xmlns:meta:1.0"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
     office:version="1.2">
   <office:meta>
       <meta:generator>Odio</meta:generator>
   </office:meta>
 </office:document-meta>
 """)
 
-            self.z.writestr(
-                'settings.xml',
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'settings.xml',
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-settings
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:xlink="http://www.w3.org/1999/xlink"
     xmlns:config="urn:oasis:names:tc:opendocument:xmlns:config:1.0"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
     office:version="1.2">
 </office:document-settings>
 """)
 
-            self.z.writestr(
-                'styles.xml', """<?xml version="1.0" encoding="UTF-8"?>
+        self.z.writestr(
+            'styles.xml', """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-styles
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
     xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
     xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
     xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
     xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
@@ -217,16 +299,16 @@
     xmlns:dom="http://www.w3.org/2001/xml-events"
     xmlns:of="urn:oasis:names:tc:opendocument:xmlns:of:1.2"
     xmlns:xhtml="http://www.w3.org/1999/xhtml"
     xmlns:css3t="http://www.w3.org/TR/css3-text/"
     office:version="1.2">
 </office:document-styles>
 """)
-            self.doc = xml.dom.minidom.parseString(
-                """<?xml version="1.0" encoding="UTF-8"?>
+        self.doc = xml.dom.minidom.parseString(
+            """<?xml version="1.0" encoding="UTF-8"?>
 <office:document-content
     xmlns:office="urn:oasis:names:tc:opendocument:xmlns:office:1.0"
     xmlns:style="urn:oasis:names:tc:opendocument:xmlns:style:1.0"
     xmlns:text="urn:oasis:names:tc:opendocument:xmlns:text:1.0"
     xmlns:table="urn:oasis:names:tc:opendocument:xmlns:table:1.0"
     xmlns:draw="urn:oasis:names:tc:opendocument:xmlns:drawing:1.0"
     xmlns:fo="urn:oasis:names:tc:opendocument:xmlns:xsl-fo-compatible:1.0"
@@ -262,105 +344,72 @@
       <number:text>:</number:text>
       <number:minutes number:style="long"/>
     </number:date-style>
     <style:style style:name="cell_date" style:family="table-cell"
       style:parent-style-name="Default" style:data-style-name="date"/>
   </office:automatic-styles>
   <office:body>
-    <office:spreadsheet>
-    </office:spreadsheet>
+    <office:text>
+    </office:text>
   </office:body>
-</office:document-content>
-""")
-        else:
-            raise Exception(
-                "The version '" + str(version) +
-                "' isn't recognized. The valid version strings are '1.1' "
-                "and '1.2'.")
-        self.spreadsheet_elem = self.doc.getElementsByTagName(
-            'office:spreadsheet')[0]
+</office:document-content>""")
+        self.text_elem = self.doc.getElementsByTagName(
+            'office:text')[0]
 
-    def append_table(self, name):
-        table_elem = self.spreadsheet_elem.appendChild(
-            self.doc.createElement('table:table'))
-        table_elem.setAttribute('table:name', name)
-        table_elem.appendChild(self.doc.createElement('table:table-column'))
-        return TableWriter(self.doc, table_elem)
+    def append(self, *subnodes):
+        for node in subnodes:
+            node.attach(self.doc, self.text_elem)
 
     def close(self):
         self.z.writestr('content.xml', self.doc.toprettyxml(encoding='utf-8'))
         self.z.close()
         self.f.close()
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
 
 
-class TableWriter():
-    def __init__(self, doc, table_elem):
-        self.doc = doc
-        self.table_elem = table_elem
-
-    def append_row(self, vals):
-        row_elem = self.table_elem.appendChild(
-            self.doc.createElement('table:table-row'))
-        for val in vals:
-            cell_elem = row_elem.appendChild(
-                self.doc.createElement('table:table-cell'))
-            if isinstance(val, datetime.datetime):
-                cell_elem.setAttribute('office:value-type', 'date')
-                cell_elem.setAttribute(
-                    'office:date-value', val.strftime('%Y-%m-%dT%H:%M:%S'))
-                cell_elem.setAttribute('table:style-name', 'cell_date')
-            elif isinstance(val, str):
-                cell_elem.setAttribute('office:value-type', 'string')
-                cell_elem.setAttribute('office:string-value', val)
-            elif isinstance(val, (float, int)):
-                cell_elem.setAttribute('office:value-type', 'float')
-                cell_elem.setAttribute('office:value', str(val))
-            elif isinstance(val, odio.Formula):
-                cell_elem.setAttribute('table:formula', 'of:' + str(val))
+class TextReader():
+    def __init__(self, text_elem):
+        self.nodes = []
+        self.attributes = {}
+        for node_elem in text_elem.childNodes:
+            self._parse_node(self, node_elem)
+
+    def _parse_node(self, parent_node, node_dom):
+        node_type = node_dom.nodeType
+        if node_type == Node.ELEMENT_NODE:
+            name = node_dom.tagName
+            if name == 'text:p':
+                node = P()
+            elif name == 'text:h':
+                node = H()
+            elif name == 'text:span':
+                node = Span()
             else:
-                raise Exception("Type of '" + str(val) + "' not recognized.")
-
-
-class SpreadsheetReader():
-    def __init__(self, f):
-        with zipfile.ZipFile(f, 'r') as z:
-            content = z.read('content.xml')
-        f.close()
-        dom = xml.dom.minidom.parseString(content)
-        spreadsheet_elem = dom.getElementsByTagName('office:spreadsheet')[0]
-
-        self.tables = []
-        for table_elem in spreadsheet_elem.getElementsByTagName('table:table'):
-            self.tables.append(TableReader(table_elem))
-
-
-class TableReader():
-    def __init__(self, table_elem):
-        self.name = table_elem.getAttribute('table:name')
-        self.rows = []
-        for row_elem in table_elem.getElementsByTagName('table:table-row'):
-            row = []
-            self.rows.append(row)
-            for cell_elem in row_elem.getElementsByTagName('table:table-cell'):
-                if cell_elem.hasAttribute('table:formula'):
-                    formula = cell_elem.getAttribute('table:formula')
-                    eq_idx = formula.index('=')
-                    row.append(odio.Formula(formula[eq_idx:]))
-                else:
-                    val_type = cell_elem.getAttribute('office:value-type')
-                    if val_type == 'date':
-                        row.append(
-                            datetime.datetime.strptime(
-                                cell_elem.getAttribute('office:date-value'),
-                                '%Y-%m-%dT%H:%M:%S'))
-                    elif val_type == 'string':
-                        row.append(
-                            cell_elem.getAttribute('office:string-value'))
-                    elif val_type == 'float':
-                        row.append(
-                            float(cell_elem.getAttribute('office:value')))
+                raise Exception("Node name " + name + " not recognized.")
+            if node_dom.hasAttributes():
+                attrs = node_dom.attributes
+                for i in range(len(attrs)):
+                    attr = attrs.item(i)
+                    attr_name = attr.name.replace(':', '_').replace('-', '_')
+                    node.attributes[attr_name] = attr.value
+            for subnode_dom in node_dom.childNodes:
+                self._parse_node(node, subnode_dom)
+        elif node_type == Node.TEXT_NODE:
+            fnode = node_dom.nodeValue
+            snode = fnode.strip()
+            if len(snode) == 0:
+                return
+            node = snode
+            rnode = node.rstrip()
+            if len(rnode) < len(fnode):
+                node += ' '
+            lnode = node.lstrip()
+            if len(lnode) < len(fnode):
+                node = ' ' + node
+        else:
+            raise Exception("Node type " + str(node_type) + " not recognized.")
+        parent_node.nodes.append(node)
```

