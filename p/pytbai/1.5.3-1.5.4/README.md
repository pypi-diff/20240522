# Comparing `tmp/pytbai-1.5.3.tar.gz` & `tmp/pytbai-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytbai-1.5.3.tar", last modified: Wed May 22 12:57:22 2024, max compression
+gzip compressed data, was "pytbai-1.5.4.tar", last modified: Wed May 22 13:19:14 2024, max compression
```

## Comparing `pytbai-1.5.3.tar` & `pytbai-1.5.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.883208 pytbai-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 12:57:18.000000 pytbai-1.5.3/CHANGELOG.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 12:57:18.000000 pytbai-1.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 12:57:18.000000 pytbai-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 12:57:18.000000 pytbai-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 12:57:18.000000 pytbai-1.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-22 12:57:22.883208 pytbai-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 12:57:18.000000 pytbai-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/templates/PDF/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/PDF/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/PDF/ticketbai.css
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/PDF/ticketbai.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/templates/XML/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/XML/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/XML/tbai_structure.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/templates/XSD/
--rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/XSD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/pytbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/utils/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 12:57:18.000000 pytbai-1.5.3/pytbai/utils/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.883208 pytbai-1.5.3/pytbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-22 12:57:22.000000 pytbai-1.5.3/pytbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 12:57:22.000000 pytbai-1.5.3/pytbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:57:22.000000 pytbai-1.5.3/pytbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 12:57:22.000000 pytbai-1.5.3/pytbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 12:57:22.000000 pytbai-1.5.3/pytbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:57:22.883208 pytbai-1.5.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1236 2024-05-22 12:57:18.000000 pytbai-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.879208 pytbai-1.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.883208 pytbai-1.5.3/tests/certs/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/certs/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/certs/cert_for_tests.p12
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/certs/key.pem
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:57:22.883208 pytbai-1.5.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/data/tbai_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 12:57:18.000000 pytbai-1.5.3/tests/test_basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-22 13:19:07.000000 pytbai-1.5.4/CHANGELOG.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 13:19:07.000000 pytbai-1.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 13:19:07.000000 pytbai-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 13:19:07.000000 pytbai-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 13:19:07.000000 pytbai-1.5.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-22 13:19:14.095631 pytbai-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-22 13:19:07.000000 pytbai-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.091631 pytbai-1.5.4/pytbai/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11308 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.091631 pytbai-1.5.4/pytbai/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.091631 pytbai-1.5.4/pytbai/templates/PDF/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/PDF/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/PDF/ticketbai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/PDF/ticketbai.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.091631 pytbai-1.5.4/pytbai/templates/XML/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/XML/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/XML/tbai_structure.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/pytbai/templates/XSD/
+-rw-r--r--   0 runner    (1001) docker     (127)    12637 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/XSD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35760 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/XSD/ticketBaiV1-2-1.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/pytbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/utils/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-22 13:19:07.000000 pytbai-1.5.4/pytbai/utils/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/pytbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-22 13:19:14.000000 pytbai-1.5.4/pytbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 13:19:14.000000 pytbai-1.5.4/pytbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:19:14.000000 pytbai-1.5.4/pytbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 13:19:14.000000 pytbai-1.5.4/pytbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 13:19:14.000000 pytbai-1.5.4/pytbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:19:14.095631 pytbai-1.5.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1236 2024-05-22 13:19:07.000000 pytbai-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/tests/certs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/certs/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/certs/cert_for_tests.p12
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/certs/key.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:19:14.095631 pytbai-1.5.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/data/tbai_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-22 13:19:07.000000 pytbai-1.5.4/tests/test_basic.py
```

### Comparing `pytbai-1.5.3/CHANGELOG.txt` & `pytbai-1.5.4/CHANGELOG.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/LICENSE` & `pytbai-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/PKG-INFO` & `pytbai-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.3
+Version: 1.5.4
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: signxml<=3.2.1
 Requires-Dist: pyOpenSSL<=23.2.0
+Requires-Dist: signxml<=3.2.1
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytbai)
 ![PyPI - Version](https://img.shields.io/pypi/v/pytbai)
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `pytbai-1.5.3/README.md` & `pytbai-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/core.py` & `pytbai-1.5.4/pytbai/core.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/definitions.py` & `pytbai-1.5.4/pytbai/definitions.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/templates/PDF/ticketbai.html` & `pytbai-1.5.4/pytbai/templates/PDF/ticketbai.html`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/templates/XML/tbai_structure.xml` & `pytbai-1.5.4/pytbai/templates/XML/tbai_structure.xml`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd` & `pytbai-1.5.4/pytbai/templates/XSD/Anula_ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/templates/XSD/ticketBaiV1-2-1.xsd` & `pytbai-1.5.4/pytbai/templates/XSD/ticketBaiV1-2-1.xsd`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai/utils/xml.py` & `pytbai-1.5.4/pytbai/utils/xml.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/pytbai.egg-info/PKG-INFO` & `pytbai-1.5.4/pytbai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytbai
-Version: 1.5.3
+Version: 1.5.4
 Summary: pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities
 Home-page: https://github.com/codesyntax/pytbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
-Requires-Dist: signxml<=3.2.1
 Requires-Dist: pyOpenSSL<=23.2.0
+Requires-Dist: signxml<=3.2.1
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pytbai)
 ![PyPI - Version](https://img.shields.io/pypi/v/pytbai)
 
 # pytbai
 
 pytbai allows to create, manage and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `pytbai-1.5.3/pytbai.egg-info/SOURCES.txt` & `pytbai-1.5.4/pytbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/setup.py` & `pytbai-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="pytbai",
-    version="1.5.3",
+    version="1.5.4",
     description=(
         "pytbai allows to create, manage and send TicketBai invoices to the"
         " Basque tax authorities"
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Urtzi Odriozola",
@@ -25,16 +25,16 @@
     packages=find_packages(exclude=("tests",)),
     include_package_data = True,
     package_data={
         "pytbai": ["templates/*"],
     },
     install_requires=[
         "requests",
-        "signxml<=3.2.1",
         "pyOpenSSL<=23.2.0",
+        "signxml<=3.2.1",
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
```

### Comparing `pytbai-1.5.3/tests/certs/cert.pem` & `pytbai-1.5.4/tests/certs/cert.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/tests/certs/cert_for_tests.p12` & `pytbai-1.5.4/tests/certs/cert_for_tests.p12`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/tests/certs/key.pem` & `pytbai-1.5.4/tests/certs/key.pem`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/tests/data/tbai_json.py` & `pytbai-1.5.4/tests/data/tbai_json.py`

 * *Files identical despite different names*

### Comparing `pytbai-1.5.3/tests/test_basic.py` & `pytbai-1.5.4/tests/test_basic.py`

 * *Files identical despite different names*

