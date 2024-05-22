# Comparing `tmp/pytbai-1.4.8.tar.gz` & `tmp/pytbai-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.4.8.tar", last modified: Tue May 21 11:21:48 2024, max compression
+gzip compressed data, was "pytbai-1.4.9.tar", last modified: Tue May 21 12:55:46 2024, max compression
```

## Comparing `pytbai-1.4.8.tar` & `pytbai-1.4.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.571967 pytbai-1.4.8/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3378 2024-05-21 11:21:47.000000 pytbai-1.4.8/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2024-05-21 11:21:47.000000 pytbai-1.4.8/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2024-05-21 11:21:47.000000 pytbai-1.4.8/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2024-05-21 11:21:47.000000 pytbai-1.4.8/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 11:21:47.000000 pytbai-1.4.8/Makefile
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 11:21:48.571967 pytbai-1.4.8/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2024-05-21 11:21:47.000000 pytbai-1.4.8/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11352 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.567966 pytbai-1.4.8/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2024-05-21 11:21:47.000000 pytbai-1.4.8/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.571967 pytbai-1.4.8/pytbai.egg-info/
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 11:21:48.000000 pytbai-1.4.8/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      819 2024-05-21 11:21:48.000000 pytbai-1.4.8/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2024-05-21 11:21:48.000000 pytbai-1.4.8/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2024-05-21 11:21:48.000000 pytbai-1.4.8/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 11:21:47.000000 pytbai-1.4.8/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2024-05-21 11:21:48.571967 pytbai-1.4.8/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1131 2024-05-21 11:21:47.000000 pytbai-1.4.8/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.571967 pytbai-1.4.8/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.571967 pytbai-1.4.8/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 11:21:48.571967 pytbai-1.4.8/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2024-05-21 11:21:47.000000 pytbai-1.4.8/tests/test_basic.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3483 2024-05-21 12:55:44.000000 pytbai-1.4.9/CHANGELOG.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2024-05-21 12:55:44.000000 pytbai-1.4.9/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2024-05-21 12:55:44.000000 pytbai-1.4.9/LICENSE
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2024-05-21 12:55:44.000000 pytbai-1.4.9/MANIFEST.in
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 12:55:44.000000 pytbai-1.4.9/Makefile
+-rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 12:55:46.049950 pytbai-1.4.9/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2024-05-21 12:55:44.000000 pytbai-1.4.9/README.md
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11308 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/core.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/definitions.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/PDF/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/ticketbai.css
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/ticketbai.html
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/XML/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XML/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XML/tbai_structure.xml
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/XSD/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/utils/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/__init__.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/crypto.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/xml.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai.egg-info/
+-rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/PKG-INFO
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      819 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/SOURCES.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/dependency_links.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/top_level.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 12:55:44.000000 pytbai-1.4.9/requirements.txt
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2024-05-21 12:55:46.049950 pytbai-1.4.9/setup.cfg
+-rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1131 2024-05-21 12:55:44.000000 pytbai-1.4.9/setup.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/__init__.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/certs/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/cert.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/cert_for_tests.p12
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/key.pem
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/context.py
+drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/data/
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/data/tbai_json.py
+-rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/test_basic.py
```

### Comparing `pytbai-1.4.8/CHANGELOG.txt` & `pytbai-1.4.9/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+1.4.9 (2024-05-21)
+------------------
+
+- Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
+
+
+
 1.4.8 (2024-05-21)
 ------------------
 
 - Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.4.8/LICENSE` & `pytbai-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/PKG-INFO` & `pytbai-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.8
+Version: 1.4.9
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.8/README.md` & `pytbai-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/core.py` & `pytbai-1.4.9/pytbai/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,23 +31,21 @@
 
 
 class Subject:
     def __init__(
         self,
         entity_id,
         name,
-        logo=None,
         territory=GIPUZKOA,
         multi_recipient=N,
         external_invoice=N,
         env="DEV",
     ):
         self.entity_id = entity_id
         self.name = name
-        self.logo = logo
         if not territory:
             self.authority_api = GIPUZKOA[env]["invoice"]
             self.qr_api = GIPUZKOA[env]["qr"]
         elif territory in AUTHORITY_APIS:
             self.authority_api = AUTHORITY_APIS[territory][env]["invoice"]
             self.qr_api = AUTHORITY_APIS[territory][env]["qr"]
         else:
```

### Comparing `pytbai-1.4.8/pytbai/definitions.py` & `pytbai-1.4.9/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.4.9/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.4.9/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.4.9/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.4.9/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai/utils/xml.py` & `pytbai-1.4.9/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/pytbai.egg-info/PKG-INFO` & `pytbai-1.4.9/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.8
+Version: 1.4.9
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `pytbai-1.4.8/pytbai.egg-info/SOURCES.txt` & `pytbai-1.4.9/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/setup.py` & `pytbai-1.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.4.8",
+    version="1.4.9",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.4.8/tests/certs/cert.pem` & `pytbai-1.4.9/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/tests/certs/cert_for_tests.p12` & `pytbai-1.4.9/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/tests/certs/key.pem` & `pytbai-1.4.9/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/tests/data/tbai_json.py` & `pytbai-1.4.9/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.8/tests/test_basic.py` & `pytbai-1.4.9/tests/test_basic.py`

 * *Files identical despite different names*

