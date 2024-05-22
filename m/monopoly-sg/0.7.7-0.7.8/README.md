# Comparing `tmp/monopoly_sg-0.7.7.tar.gz` & `tmp/monopoly_sg-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monopoly_sg-0.7.7.tar", max compression
+gzip compressed data, was "monopoly_sg-0.7.8.tar", max compression
```

## Comparing `monopoly_sg-0.7.7.tar` & `monopoly_sg-0.7.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.7/LICENSE.md
--rw-r--r--   0        0        0     2624 2024-04-21 03:16:26.522623 monopoly_sg-0.7.7/README.md
--rw-r--r--   0        0        0     2052 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/pyproject.toml
--rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.7/src/monopoly/__init__.py
--rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.7/src/monopoly/cli.py
--rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.7/src/monopoly/config.py
--rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.7/src/monopoly/constants.py
--rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.7/src/monopoly/examples/example_statement.pdf
--rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/examples/multiple_statements.py
--rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.7/src/monopoly/examples/single_statement.py
--rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.7/src/monopoly/log.py
--rw-r--r--   0        0        0     5935 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/src/monopoly/pdf.py
--rw-r--r--   0        0        0     3808 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/src/monopoly/processor.py
--rw-r--r--   0        0        0     3032 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/src/monopoly/processors/__init__.py
--rw-r--r--   0        0        0     4100 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/src/monopoly/processors/base.py
--rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/processors/citibank/__init__.py
--rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.7/src/monopoly/processors/citibank/citibank.py
--rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/processors/dbs/__init__.py
--rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.7/src/monopoly/processors/dbs/dbs.py
--rw-r--r--   0        0        0      964 2024-04-21 07:51:47.386734 monopoly_sg-0.7.7/src/monopoly/processors/example_bank.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/processors/hsbc/__init__.py
--rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.7/src/monopoly/processors/hsbc/hsbc.py
--rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/processors/ocbc/__init__.py
--rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.7/src/monopoly/processors/ocbc/ocbc.py
--rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.7/src/monopoly/processors/standard_chartered/__init__.py
--rw-r--r--   0        0        0     1007 2024-01-12 14:33:27.070256 monopoly_sg-0.7.7/src/monopoly/processors/standard_chartered/standard_chartered.py
--rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.7/src/monopoly/statements/__init__.py
--rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.7/src/monopoly/statements/base.py
--rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.7/src/monopoly/statements/credit_statement.py
--rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.7/src/monopoly/statements/debit_statement.py
--rw-r--r--   0        0        0     1465 2024-04-21 10:11:19.943749 monopoly_sg-0.7.7/src/monopoly/write.py
--rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.7/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.7/tests/test_utils/skip.py
--rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 monopoly_sg-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-11-25 08:00:21.000000 monopoly_sg-0.7.8/LICENSE.md
+-rw-r--r--   0        0        0     2624 2024-04-21 03:16:26.522623 monopoly_sg-0.7.8/README.md
+-rw-r--r--   0        0        0     2052 2024-04-21 10:15:23.763661 monopoly_sg-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-11-25 08:00:21.000000 monopoly_sg-0.7.8/src/monopoly/__init__.py
+-rw-r--r--   0        0        0     8005 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/cli.py
+-rw-r--r--   0        0        0     3389 2024-01-14 10:44:28.918012 monopoly_sg-0.7.8/src/monopoly/config.py
+-rw-r--r--   0        0        0     4005 2024-01-14 09:33:42.855330 monopoly_sg-0.7.8/src/monopoly/constants.py
+-rw-r--r--   0        0        0   299608 2023-12-28 09:49:25.899409 monopoly_sg-0.7.8/src/monopoly/examples/example_statement.pdf
+-rw-r--r--   0        0        0      620 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/examples/multiple_statements.py
+-rw-r--r--   0        0        0      742 2023-12-02 13:07:54.000000 monopoly_sg-0.7.8/src/monopoly/examples/single_statement.py
+-rw-r--r--   0        0        0      491 2024-01-01 12:59:34.183692 monopoly_sg-0.7.8/src/monopoly/log.py
+-rw-r--r--   0        0        0     5935 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/pdf.py
+-rw-r--r--   0        0        0     3808 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processor.py
+-rw-r--r--   0        0        0     3032 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processors/__init__.py
+-rw-r--r--   0        0        0     4100 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/processors/base.py
+-rw-r--r--   0        0        0       55 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/citibank/__init__.py
+-rw-r--r--   0        0        0     1020 2024-01-14 07:44:48.150290 monopoly_sg-0.7.8/src/monopoly/processors/citibank/citibank.py
+-rw-r--r--   0        0        0       40 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/dbs/__init__.py
+-rw-r--r--   0        0        0     1365 2024-04-19 14:20:45.535418 monopoly_sg-0.7.8/src/monopoly/processors/dbs/dbs.py
+-rw-r--r--   0        0        0      964 2024-04-21 07:51:47.386734 monopoly_sg-0.7.8/src/monopoly/processors/example_bank.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/hsbc/__init__.py
+-rw-r--r--   0        0        0     1158 2024-01-11 15:47:10.530736 monopoly_sg-0.7.8/src/monopoly/processors/hsbc/hsbc.py
+-rw-r--r--   0        0        0       43 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/ocbc/__init__.py
+-rw-r--r--   0        0        0     1506 2024-04-19 14:18:09.005435 monopoly_sg-0.7.8/src/monopoly/processors/ocbc/ocbc.py
+-rw-r--r--   0        0        0       83 2023-12-01 13:26:34.000000 monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/__init__.py
+-rw-r--r--   0        0        0     1007 2024-04-21 10:15:14.953665 monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/standard_chartered.py
+-rw-r--r--   0        0        0      216 2023-12-28 15:35:17.896832 monopoly_sg-0.7.8/src/monopoly/statements/__init__.py
+-rw-r--r--   0        0        0     7669 2024-04-19 14:24:09.875401 monopoly_sg-0.7.8/src/monopoly/statements/base.py
+-rw-r--r--   0        0        0     3105 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/statements/credit_statement.py
+-rw-r--r--   0        0        0     4278 2024-02-11 14:35:16.392192 monopoly_sg-0.7.8/src/monopoly/statements/debit_statement.py
+-rw-r--r--   0        0        0     1465 2024-04-21 10:11:19.943749 monopoly_sg-0.7.8/src/monopoly/write.py
+-rw-r--r--   0        0        0       69 2023-11-25 10:08:54.000000 monopoly_sg-0.7.8/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      790 2023-11-25 10:08:54.000000 monopoly_sg-0.7.8/tests/test_utils/skip.py
+-rw-r--r--   0        0        0     3588 1970-01-01 00:00:00.000000 monopoly_sg-0.7.8/PKG-INFO
```

### Comparing `monopoly_sg-0.7.7/LICENSE.md` & `monopoly_sg-0.7.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/README.md` & `monopoly_sg-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/pyproject.toml` & `monopoly_sg-0.7.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monopoly-sg"
-version = "0.7.7"
+version = "0.7.8"
 description = "PDF parsing for Singaporean banks"
 repository = "https://github.com/benjamin-awd/monopoly"
 authors = ["benjamin-awd <benjamindornel@gmail.com>"]
 packages = [
     { include = "monopoly", from = "src" },
     { include = "test_utils", from = "tests" }
 ]
```

### Comparing `monopoly_sg-0.7.7/src/monopoly/cli.py` & `monopoly_sg-0.7.8/src/monopoly/cli.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/config.py` & `monopoly_sg-0.7.8/src/monopoly/config.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/constants.py` & `monopoly_sg-0.7.8/src/monopoly/constants.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/examples/example_statement.pdf` & `monopoly_sg-0.7.8/src/monopoly/examples/example_statement.pdf`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/examples/multiple_statements.py` & `monopoly_sg-0.7.8/src/monopoly/examples/multiple_statements.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/examples/single_statement.py` & `monopoly_sg-0.7.8/src/monopoly/examples/single_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/pdf.py` & `monopoly_sg-0.7.8/src/monopoly/pdf.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processor.py` & `monopoly_sg-0.7.8/src/monopoly/processor.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/__init__.py` & `monopoly_sg-0.7.8/src/monopoly/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/base.py` & `monopoly_sg-0.7.8/src/monopoly/processors/base.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/citibank/citibank.py` & `monopoly_sg-0.7.8/src/monopoly/processors/citibank/citibank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/dbs/dbs.py` & `monopoly_sg-0.7.8/src/monopoly/processors/dbs/dbs.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/example_bank.py` & `monopoly_sg-0.7.8/src/monopoly/processors/example_bank.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/hsbc/hsbc.py` & `monopoly_sg-0.7.8/src/monopoly/processors/hsbc/hsbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/ocbc/ocbc.py` & `monopoly_sg-0.7.8/src/monopoly/processors/ocbc/ocbc.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/processors/standard_chartered/standard_chartered.py` & `monopoly_sg-0.7.8/src/monopoly/processors/standard_chartered/standard_chartered.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 logger = logging.getLogger(__name__)
 
 
 class StandardChartered(ProcessorBase):
     credit_config = CreditStatementConfig(
         bank_name=BankNames.STANDARD_CHARTERED,
         statement_date_pattern=r"(\d{2}\s\w+\s\d{4})",
-        statement_date_format=r"%d %B %Y",
+        statement_date_format=r"%d %b %Y",
         prev_balance_pattern=StatementBalancePatterns.STANDARD_CHARTERED,
         transaction_pattern=CreditTransactionPatterns.STANDARD_CHARTERED,
         transaction_date_format="%d %b",
     )
 
     pdf_config = PdfConfig(
         passwords=settings.standard_chartered_pdf_passwords,
```

### Comparing `monopoly_sg-0.7.7/src/monopoly/statements/base.py` & `monopoly_sg-0.7.8/src/monopoly/statements/base.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/statements/credit_statement.py` & `monopoly_sg-0.7.8/src/monopoly/statements/credit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/statements/debit_statement.py` & `monopoly_sg-0.7.8/src/monopoly/statements/debit_statement.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/src/monopoly/write.py` & `monopoly_sg-0.7.8/src/monopoly/write.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/tests/test_utils/skip.py` & `monopoly_sg-0.7.8/tests/test_utils/skip.py`

 * *Files identical despite different names*

### Comparing `monopoly_sg-0.7.7/PKG-INFO` & `monopoly_sg-0.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monopoly-sg
-Version: 0.7.7
+Version: 0.7.8
 Summary: PDF parsing for Singaporean banks
 Home-page: https://github.com/benjamin-awd/monopoly
 License: MIT
 Author: benjamin-awd
 Author-email: benjamindornel@gmail.com
 Requires-Python: >=3.11,<3.12
 Classifier: Development Status :: 3 - Alpha
```

