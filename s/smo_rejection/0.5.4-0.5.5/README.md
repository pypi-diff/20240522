# Comparing `tmp/smo_rejection-0.5.4.tar.gz` & `tmp/smo_rejection-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.5.4.tar", max compression
+gzip compressed data, was "smo_rejection-0.5.5.tar", max compression
```

## Comparing `smo_rejection-0.5.4.tar` & `smo_rejection-0.5.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      305 2024-05-21 21:18:54.154757 smo_rejection-0.5.4/pyproject.toml
--rw-r--r--   0        0        0    16387 2024-05-21 11:13:02.127103 smo_rejection-0.5.4/README.md
--rw-r--r--   0        0        0      496 2024-05-21 11:13:02.130096 smo_rejection-0.5.4/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-21 11:13:02.136049 smo_rejection-0.5.4/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-21 11:13:02.136049 smo_rejection-0.5.4/smo_rejection/models.py
--rw-r--r--   0        0        0     4409 2024-05-21 21:18:28.009912 smo_rejection-0.5.4/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4403 2024-05-21 11:13:28.975815 smo_rejection-0.5.4/smo_rejection/processing.py
--rw-r--r--   0        0        0     4306 2024-05-21 11:13:02.137051 smo_rejection-0.5.4/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-21 11:13:02.138052 smo_rejection-0.5.4/smo_rejection/utils.py
--rw-r--r--   0        0        0     4797 2024-05-21 11:13:02.138052 smo_rejection-0.5.4/smo_rejection/xml_export.py
--rw-r--r--   0        0        0    16527 1970-01-01 00:00:00.000000 smo_rejection-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      305 2024-05-21 21:28:53.671352 smo_rejection-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0    16387 2024-05-21 11:13:02.127103 smo_rejection-0.5.5/README.md
+-rw-r--r--   0        0        0      496 2024-05-21 11:13:02.130096 smo_rejection-0.5.5/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-21 11:13:02.136049 smo_rejection-0.5.5/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-21 11:13:02.136049 smo_rejection-0.5.5/smo_rejection/models.py
+-rw-r--r--   0        0        0     4460 2024-05-21 21:28:13.676370 smo_rejection-0.5.5/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4403 2024-05-21 11:13:28.975815 smo_rejection-0.5.5/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4306 2024-05-21 11:13:02.137051 smo_rejection-0.5.5/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-21 11:13:02.138052 smo_rejection-0.5.5/smo_rejection/utils.py
+-rw-r--r--   0        0        0     4797 2024-05-21 11:13:02.138052 smo_rejection-0.5.5/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0    16527 1970-01-01 00:00:00.000000 smo_rejection-0.5.5/PKG-INFO
```

### Comparing `smo_rejection-0.5.4/README.md` & `smo_rejection-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/exception.py` & `smo_rejection-0.5.5/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/models.py` & `smo_rejection-0.5.5/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/pdf_export.py` & `smo_rejection-0.5.5/smo_rejection/pdf_export.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from reportlab.lib.pagesizes import letter
 from reportlab.platypus import SimpleDocTemplate, Table, TableStyle, Paragraph, Spacer
 from reportlab.lib.styles import getSampleStyleSheet, ParagraphStyle
 from reportlab.lib.units import inch
 from reportlab.lib import colors
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.pdfbase import pdfmetrics
+from .utils import calculate_mean_served_requests
 import io
 
 def export_to_pdf(results):
     """
     Экспортирует результаты симуляции в PDF-файл.
 
     ### Параметры:
```

### Comparing `smo_rejection-0.5.4/smo_rejection/processing.py` & `smo_rejection-0.5.5/smo_rejection/processing.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/simulation.py` & `smo_rejection-0.5.5/smo_rejection/simulation.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/utils.py` & `smo_rejection-0.5.5/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/smo_rejection/xml_export.py` & `smo_rejection-0.5.5/smo_rejection/xml_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.5.4/PKG-INFO` & `smo_rejection-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.5.4
+Version: 0.5.5
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

