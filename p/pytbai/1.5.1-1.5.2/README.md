# Comparing `tmp/pytbai-1.5.1.tar.gz` & `tmp/pytbai-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.5.1.tar", last modified: Wed May 22 10:41:06 2024, max compression
+gzip compressed data, was "pytbai-1.5.2.tar", last modified: Wed May 22 11:35:11 2024, max compression
```

## Comparing `pytbai-1.5.1.tar` & `pytbai-1.5.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 10:41:02.000000 pytbai-1.5.1/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 10:41:02.000000 pytbai-1.5.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 10:41:02.000000 pytbai-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 10:41:02.000000 pytbai-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:41:02.000000 pytbai-1.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 10:41:06.450615 pytbai-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 10:41:02.000000 pytbai-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.446615 pytbai-1.5.1/pytbai/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai/templates/PDF/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/PDF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/PDF/ticketbai.css
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/PDF/ticketbai.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai/templates/XML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/XML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/XML/tbai_structure.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai/templates/XSD/
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/XSD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 10:41:02.000000 pytbai-1.5.1/pytbai/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/pytbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 10:41:06.000000 pytbai-1.5.1/pytbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 10:41:06.000000 pytbai-1.5.1/pytbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:41:06.000000 pytbai-1.5.1/pytbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:41:06.000000 pytbai-1.5.1/pytbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-22 10:41:02.000000 pytbai-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:41:06.450615 pytbai-1.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-22 10:41:02.000000 pytbai-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/certs/cert_for_tests.p12
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:41:06.450615 pytbai-1.5.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/data/tbai_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 10:41:02.000000 pytbai-1.5.1/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.418427 pytbai-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 11:35:04.000000 pytbai-1.5.2/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 11:35:04.000000 pytbai-1.5.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 11:35:04.000000 pytbai-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 11:35:04.000000 pytbai-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 11:35:04.000000 pytbai-1.5.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 11:35:11.418427 pytbai-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 11:35:04.000000 pytbai-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/PDF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 11:35:04.000000 pytbai-1.5.2/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.418427 pytbai-1.5.2/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 11:35:11.000000 pytbai-1.5.2/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 11:35:11.000000 pytbai-1.5.2/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:35:11.000000 pytbai-1.5.2/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 11:35:11.000000 pytbai-1.5.2/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-22 11:35:04.000000 pytbai-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:35:11.418427 pytbai-1.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-22 11:35:04.000000 pytbai-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.414427 pytbai-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.418427 pytbai-1.5.2/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:35:11.418427 pytbai-1.5.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 11:35:04.000000 pytbai-1.5.2/tests/test_basic.py
```

### Comparing `pytbai-1.5.1/CHANGELOG.txt` & `pytbai-1.5.2/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/LICENSE` & `pytbai-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/PKG-INFO` & `pytbai-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.1
+Version: 1.5.2
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.1/README.md` & `pytbai-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/core.py` & `pytbai-1.5.2/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/definitions.py` & `pytbai-1.5.2/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.5.2/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.5.2/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.5.2/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.5.2/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai/utils/xml.py` & `pytbai-1.5.2/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/pytbai.egg-info/PKG-INFO` & `pytbai-1.5.2/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.1
+Version: 1.5.2
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.5.1/pytbai.egg-info/SOURCES.txt` & `pytbai-1.5.2/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/setup.py` & `pytbai-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.5.1",
+    version="1.5.2",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.5.1/tests/certs/cert.pem` & `pytbai-1.5.2/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/tests/certs/cert_for_tests.p12` & `pytbai-1.5.2/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/tests/certs/key.pem` & `pytbai-1.5.2/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/tests/data/tbai_json.py` & `pytbai-1.5.2/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.1/tests/test_basic.py` & `pytbai-1.5.2/tests/test_basic.py`

 * *Files identical despite different names*

