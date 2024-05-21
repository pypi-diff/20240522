# Comparing `tmp/pih-doc-0.17.tar.gz` & `tmp/pih-doc-0.17.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-doc-0.17.tar", last modified: Tue May 21 19:20:19 2024, max compression
+gzip compressed data, was "pih-doc-0.17.2.tar", last modified: Tue May 21 23:32:12 2024, max compression
```

## Comparing `pih-doc-0.17.tar` & `pih-doc-0.17.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.598162 pih-doc-0.17/
-drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.131886 pih-doc-0.17/DocsService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.17/DocsService/__init__.py
--rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.17/DocsService/__main__.py
--rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.17/DocsService/api.py
--rw-rw-rw-   0        0        0     1634 2024-05-21 19:20:04.000000 pih-doc-0.17/DocsService/const.py
--rw-rw-rw-   0        0        0     5242 2024-05-20 23:01:06.000000 pih-doc-0.17/DocsService/service.py
--rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.17/DocsService/tools.py
--rw-rw-rw-   0        0        0      595 2024-05-21 19:20:19.533547 pih-doc-0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 19:20:19.486696 pih-doc-0.17/pih_doc.egg-info/
--rw-rw-rw-   0        0        0      595 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      123 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 19:20:18.000000 pih-doc-0.17/pih_doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 19:20:19.598162 pih-doc-0.17/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 23:32:12.123503 pih-doc-0.17.2/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:32:11.669180 pih-doc-0.17.2/DocsService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-doc-0.17.2/DocsService/__init__.py
+-rw-rw-rw-   0        0        0      146 2024-02-13 08:06:49.000000 pih-doc-0.17.2/DocsService/__main__.py
+-rw-rw-rw-   0        0        0    41563 2024-05-06 00:47:28.000000 pih-doc-0.17.2/DocsService/api.py
+-rw-rw-rw-   0        0        0     1636 2024-05-21 23:29:33.000000 pih-doc-0.17.2/DocsService/const.py
+-rw-rw-rw-   0        0        0     5316 2024-05-21 23:25:47.000000 pih-doc-0.17.2/DocsService/service.py
+-rw-rw-rw-   0        0        0      729 2024-02-17 13:43:10.000000 pih-doc-0.17.2/DocsService/tools.py
+-rw-rw-rw-   0        0        0      597 2024-05-21 23:32:12.076630 pih-doc-0.17.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 23:32:12.045388 pih-doc-0.17.2/pih_doc.egg-info/
+-rw-rw-rw-   0        0        0      597 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      123 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 23:32:11.000000 pih-doc-0.17.2/pih_doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:32:12.139129 pih-doc-0.17.2/setup.cfg
```

### Comparing `pih-doc-0.17/DocsService/api.py` & `pih-doc-0.17.2/DocsService/api.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.17/DocsService/const.py` & `pih-doc-0.17.2/DocsService/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     QUANTITY_COLUMN_NAME: str = "фактическое наличие"
     NAME_MAX_LENTH: int = 120
     QUANTITY_NOT_SET: str = "-"
 
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.17"
+VERSION: str = "0.17.2"
 
 PACKAGES: tuple[str, ...] = (
     "xlsxwriter",
     "xlrd",
     "xlutils",
     "openpyxl",
     "python-barcode",
```

### Comparing `pih-doc-0.17/DocsService/service.py` & `pih-doc-0.17.2/DocsService/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,59 +2,59 @@
 
 from pih import A
 from typing import Any
 from DocsService.const import SD
 
 SC = A.CT_SC
 
-ISOLATED: bool = False
+ISOLATED: bool = True
 
 
 def start(as_standalone: bool = False) -> None:
 
     if A.U.for_service(SD, as_standalone=as_standalone):
-        from datetime import datetime
+        from datetime import date
         import grpc
-        from pih.tools import ParameterList
+        from pih.tools import ParameterList, nnt
         from DocsService.api import DocumentApi
         from pih.consts.errors import IncorrectInputFile
         from pih.collections import FullName, LoginPasswordPair, Result, Note
 
         api: DocumentApi = DocumentApi(ISOLATED)
 
         def service_call_handler(sc: SC, pl: ParameterList, context) -> Any:
             if sc == SC.create_statistics_chart:
                 return api.create_statistics_chart(pl.next())
             if sc == SC.create_user_document:
                 path: str = pl.next()
-                date: str = pl.next()
+                date_value: str = pl.next()
                 web_site_name: str = pl.next()
                 web_site: str = pl.next()
                 email_address: str = pl.next()
                 full_name: FullName = pl.next(FullName())
                 tab_number: str = pl.next()
                 pc: LoginPasswordPair = pl.next(LoginPasswordPair())
                 polibase: LoginPasswordPair = pl.next(LoginPasswordPair())
                 email: LoginPasswordPair = pl.next(LoginPasswordPair())
                 return api.create_user_document(
                     path,
-                    date,
+                    date_value,
                     web_site_name,
                     web_site,
                     email_address,
                     full_name,
                     tab_number,
                     pc,
                     polibase,
                     email,
                 )
             if sc == SC.save_time_tracking_report:
-                path: str = pl.next()
-                start_date: datetime = pl.next()
-                end_date: datetime = pl.next()
+                path: str = pl.next()                
+                start_date: date = nnt(A.D.date_from_string(pl.next()))
+                end_date: date = nnt(A.D.date_from_string(pl.next()))
                 tab_number: list[str] = pl.next()
                 plain_format: bool = pl.next()
                 return api.save_time_tracking_report(
                     A.R_TT.create(start_date, end_date, tab_number), path, plain_format
                 )
             if sc == SC.create_barcodes_for_inventory:
                 try:
```

### Comparing `pih-doc-0.17/DocsService/tools.py` & `pih-doc-0.17.2/DocsService/tools.py`

 * *Files identical despite different names*

### Comparing `pih-doc-0.17/PKG-INFO` & `pih-doc-0.17.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.17
+Version: 0.17.2
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

### Comparing `pih-doc-0.17/pih_doc.egg-info/PKG-INFO` & `pih-doc-0.17.2/pih_doc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pih-doc
-Version: 0.17
+Version: 0.17.2
 Summary: PIH Documents service package
 Home-page: https://pacifichosp.com/
 Author: Nikita Karachentsev
 Author-email: it@pacifichosp.com
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: ipih
```

