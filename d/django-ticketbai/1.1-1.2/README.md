# Comparing `tmp/django_ticketbai-1.1.tar.gz` & `tmp/django_ticketbai-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ticketbai-1.1.tar", last modified: Wed May 22 13:00:20 2024, max compression
+gzip compressed data, was "django_ticketbai-1.2.tar", last modified: Wed May 22 13:06:21 2024, max compression
```

## Comparing `django_ticketbai-1.1.tar` & `django_ticketbai-1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:20.144399 django_ticketbai-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 13:00:13.000000 django_ticketbai-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:13.000000 django_ticketbai-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 13:00:20.144399 django_ticketbai-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-22 13:00:13.000000 django_ticketbai-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:20.136399 django_ticketbai-1.1/django_ticketbai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:20.140399 django_ticketbai-1.1/django_ticketbai/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0006_config_is_active.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0007_invoice_errorxml.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:20.144399 django_ticketbai-1.1/django_ticketbai/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/utils/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/utils/pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 13:00:13.000000 django_ticketbai-1.1/django_ticketbai/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:00:20.144399 django_ticketbai-1.1/django_ticketbai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-22 13:00:20.000000 django_ticketbai-1.1/django_ticketbai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-22 13:00:20.000000 django_ticketbai-1.1/django_ticketbai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:00:20.000000 django_ticketbai-1.1/django_ticketbai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 13:00:20.000000 django_ticketbai-1.1/django_ticketbai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 13:00:20.000000 django_ticketbai-1.1/django_ticketbai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:00:20.144399 django_ticketbai-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-22 13:00:13.000000 django_ticketbai-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:21.017196 django_ticketbai-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-22 13:06:16.000000 django_ticketbai-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:16.000000 django_ticketbai-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-22 13:06:21.017196 django_ticketbai-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-22 13:06:16.000000 django_ticketbai-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:21.009196 django_ticketbai-1.2/django_ticketbai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:21.013196 django_ticketbai-1.2/django_ticketbai/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0006_config_is_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0007_invoice_errorxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0010_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0011_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:21.013196 django_ticketbai-1.2/django_ticketbai/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/utils/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/utils/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-22 13:06:16.000000 django_ticketbai-1.2/django_ticketbai/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:06:21.013196 django_ticketbai-1.2/django_ticketbai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-22 13:06:20.000000 django_ticketbai-1.2/django_ticketbai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-22 13:06:21.000000 django_ticketbai-1.2/django_ticketbai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:06:20.000000 django_ticketbai-1.2/django_ticketbai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-22 13:06:20.000000 django_ticketbai-1.2/django_ticketbai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 13:06:20.000000 django_ticketbai-1.2/django_ticketbai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:06:21.017196 django_ticketbai-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-05-22 13:06:16.000000 django_ticketbai-1.2/setup.py
```

### Comparing `django_ticketbai-1.1/LICENSE` & `django_ticketbai-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/PKG-INFO` & `django_ticketbai-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.1
+Version: 1.2
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytbaiqrcode
+Requires-Dist: pytbai
+Requires-Dist: qrcode
 Requires-Dist: weasyprint==59.0
 Requires-Dist: crc8==0.2.0
 
 # django-ticketbai
 
 django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `django_ticketbai-1.1/django_ticketbai/admin.py` & `django_ticketbai-1.2/django_ticketbai/admin.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0001_initial.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0002_invoice_pdf_invoice_signedxml.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0003_alter_invoice_pdf_invoiceline.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0004_invoice_csv_code_invoice_tbai_code_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0005_config_alter_invoice_simplified_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0008_remove_invoice_user_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0009_alter_config_options_alter_invoice_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0010_alter_invoice_signature_value.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0010_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0012_invoice_pre_invoice_alter_invoice_signature_value.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0013_invoice_vat_breakdown_alter_invoice_pre_invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py` & `django_ticketbai-1.2/django_ticketbai/migrations/0014_config_logo_alter_invoice_email.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/models.py` & `django_ticketbai-1.2/django_ticketbai/models.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/utils/invoice.py` & `django_ticketbai-1.2/django_ticketbai/utils/invoice.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/utils/pdf.py` & `django_ticketbai-1.2/django_ticketbai/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/validators.py` & `django_ticketbai-1.2/django_ticketbai/validators.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai/views.py` & `django_ticketbai-1.2/django_ticketbai/views.py`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/django_ticketbai.egg-info/PKG-INFO` & `django_ticketbai-1.2/django_ticketbai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ticketbai
-Version: 1.1
+Version: 1.2
 Summary: django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
 Home-page: https://github.com/codesyntax/django-ticketbai
 Author: Urtzi Odriozola
 Author-email: uodriozola@codesyntax.com
 License: Copyright 2023 CodeSyntax
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytbaiqrcode
+Requires-Dist: pytbai
+Requires-Dist: qrcode
 Requires-Dist: weasyprint==59.0
 Requires-Dist: crc8==0.2.0
 
 # django-ticketbai
 
 django-ticketbai allows to create, manage, store and send TicketBai invoices to the Basque tax authorities.
```

### Comparing `django_ticketbai-1.1/django_ticketbai.egg-info/SOURCES.txt` & `django_ticketbai-1.2/django_ticketbai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_ticketbai-1.1/setup.py` & `django_ticketbai-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 
 with open("LICENSE") as f:
     license = f.read()
 
 
 setup(
     name="django-ticketbai",
-    version="1.1",
+    version="1.2",
     description=(
         "django-ticketbai allows to create, manage, store and send TicketBai"
         " invoices to the Basque tax authorities."
     ),
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="",
     author="Urtzi Odriozola",
     author_email="uodriozola@codesyntax.com",
     url="https://github.com/codesyntax/django-ticketbai",
     license=license,
     packages=find_packages(exclude=("tests", "docs")),
     install_requires=[
-        "pytbai"
+        "pytbai",
         "qrcode",
         "weasyprint==59.0",
         "crc8==0.2.0",
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

