# Comparing `tmp/pytbai-1.4.9.tar.gz` & `tmp/pytbai-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.4.9.tar", last modified: Tue May 21 12:55:46 2024, max compression
+gzip compressed data, was "pytbai-1.5.0.tar", last modified: Wed May 22 10:30:27 2024, max compression
```

## Comparing `pytbai-1.4.9.tar` & `pytbai-1.5.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3483 2024-05-21 12:55:44.000000 pytbai-1.4.9/CHANGELOG.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      111 2024-05-21 12:55:44.000000 pytbai-1.4.9/CODE_OF_CONDUCT.md
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1058 2024-05-21 12:55:44.000000 pytbai-1.4.9/LICENSE
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      322 2024-05-21 12:55:44.000000 pytbai-1.4.9/MANIFEST.in
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 12:55:44.000000 pytbai-1.4.9/Makefile
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 12:55:46.049950 pytbai-1.4.9/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1786 2024-05-21 12:55:44.000000 pytbai-1.4.9/README.md
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       23 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    11308 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/core.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/definitions.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/PDF/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      121 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/ticketbai.css
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1221 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/PDF/ticketbai.html
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/XML/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XML/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     2085 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XML/tbai_structure.xml
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/templates/XSD/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    12637 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)    35760 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/templates/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai/utils/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/__init__.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      444 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/crypto.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     5251 2024-05-21 12:55:44.000000 pytbai-1.4.9/pytbai/utils/xml.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/pytbai.egg-info/
--rw-r--r--   0 urtzi     (1000) urtzi     (1000)     3622 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/PKG-INFO
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      819 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/SOURCES.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        1 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/dependency_links.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        7 2024-05-21 12:55:46.000000 pytbai-1.4.9/pytbai.egg-info/top_level.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       63 2024-05-21 12:55:44.000000 pytbai-1.4.9/requirements.txt
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)       38 2024-05-21 12:55:46.049950 pytbai-1.4.9/setup.cfg
--rwxrwxr-x   0 urtzi     (1000) urtzi     (1000)     1131 2024-05-21 12:55:44.000000 pytbai-1.4.9/setup.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/__init__.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/certs/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     1939 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/cert.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4384 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/cert_for_tests.p12
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3272 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/certs/key.pem
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)      151 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/context.py
-drwxrwxr-x   0 urtzi     (1000) urtzi     (1000)        0 2024-05-21 12:55:46.049950 pytbai-1.4.9/tests/data/
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     3187 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/data/tbai_json.py
--rw-rw-r--   0 urtzi     (1000) urtzi     (1000)     4553 2024-05-21 12:55:44.000000 pytbai-1.4.9/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.063183 pytbai-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 10:30:20.000000 pytbai-1.5.0/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 10:30:20.000000 pytbai-1.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 10:30:20.000000 pytbai-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 10:30:20.000000 pytbai-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:30:20.000000 pytbai-1.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 10:30:27.063183 pytbai-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 10:30:20.000000 pytbai-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/PDF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.059183 pytbai-1.5.0/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 10:30:20.000000 pytbai-1.5.0/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.063183 pytbai-1.5.0/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-22 10:30:27.000000 pytbai-1.5.0/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 10:30:27.000000 pytbai-1.5.0/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:30:27.000000 pytbai-1.5.0/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:30:27.000000 pytbai-1.5.0/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:30:20.000000 pytbai-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:30:27.063183 pytbai-1.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1131 2024-05-22 10:30:20.000000 pytbai-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.063183 pytbai-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.063183 pytbai-1.5.0/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:30:27.063183 pytbai-1.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 10:30:20.000000 pytbai-1.5.0/tests/test_basic.py
```

### Comparing `pytbai-1.4.9/CHANGELOG.txt` & `pytbai-1.5.0/CHANGELOG.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+1.4.10 (unreleased)
+-------------------
+
+- Nothing changed yet.
+
+
 1.4.9 (2024-05-21)
 ------------------
 
 - Update core.py [Urtzi Odriozola <uodriozola@codesyntax.com>]
```

### Comparing `pytbai-1.4.9/LICENSE` & `pytbai-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/PKG-INFO` & `pytbai-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.9
+Version: 1.5.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytbai)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/codesyntax/pytbai/python-package.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/pytbai)
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
 
 ## Usage
 
@@ -82,15 +82,15 @@
 - [ ] Recipient data
 - [ ] Multiple recipient data
 - [ ] Third party / Recipient's invoices
 - [ ] Corrective invoices
 - [ ] Corrected or replaced invoices
 - [ ] Tax free invoices
 - [ ] Invoices without national counterparty
-- [ ] Chaining of previous invoice
+- [x] Chaining of previous invoice
 
 ## How to contribute
 
 Please read the [Code of Conduct documentation](CODE_OF_CONDUCT.md) first, then all contributions are done via Pull Requests on GitHub but don´t hesitate to open a new issue.
 
 ## Credits
```

### Comparing `pytbai-1.4.9/README.md` & `pytbai-1.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytbai)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/codesyntax/pytbai/python-package.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/pytbai)
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
 
 ## Usage
 
@@ -56,15 +56,15 @@
 - [ ] Recipient data
 - [ ] Multiple recipient data
 - [ ] Third party / Recipient's invoices
 - [ ] Corrective invoices
 - [ ] Corrected or replaced invoices
 - [ ] Tax free invoices
 - [ ] Invoices without national counterparty
-- [ ] Chaining of previous invoice
+- [x] Chaining of previous invoice
 
 ## How to contribute
 
 Please read the [Code of Conduct documentation](CODE_OF_CONDUCT.md) first, then all contributions are done via Pull Requests on GitHub but don´t hesitate to open a new issue.
 
 ## Credits
```

### Comparing `pytbai-1.4.9/pytbai/core.py` & `pytbai-1.5.0/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/definitions.py` & `pytbai-1.5.0/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.5.0/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.5.0/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.5.0/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.5.0/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai/utils/xml.py` & `pytbai-1.5.0/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/pytbai.egg-info/PKG-INFO` & `pytbai-1.5.0/pytbai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.4.9
+Version: 1.5.0
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytbai)
-![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/codesyntax/pytbai/python-package.yml)
+![PyPI - Version](https://img.shields.io/pypi/v/pytbai)
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
 
 ## Usage
 
@@ -82,15 +82,15 @@
 - [ ] Recipient data
 - [ ] Multiple recipient data
 - [ ] Third party / Recipient's invoices
 - [ ] Corrective invoices
 - [ ] Corrected or replaced invoices
 - [ ] Tax free invoices
 - [ ] Invoices without national counterparty
-- [ ] Chaining of previous invoice
+- [x] Chaining of previous invoice
 
 ## How to contribute
 
 Please read the [Code of Conduct documentation](CODE_OF_CONDUCT.md) first, then all contributions are done via Pull Requests on GitHub but don´t hesitate to open a new issue.
 
 ## Credits
```

### Comparing `pytbai-1.4.9/pytbai.egg-info/SOURCES.txt` & `pytbai-1.5.0/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/setup.py` & `pytbai-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.4.9",
+    version="1.5.0",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
```

### Comparing `pytbai-1.4.9/tests/certs/cert.pem` & `pytbai-1.5.0/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/tests/certs/cert_for_tests.p12` & `pytbai-1.5.0/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/tests/certs/key.pem` & `pytbai-1.5.0/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/tests/data/tbai_json.py` & `pytbai-1.5.0/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.4.9/tests/test_basic.py` & `pytbai-1.5.0/tests/test_basic.py`

 * *Files identical despite different names*

