# Comparing `tmp/excel-formulas-calculator-0.4.2.tar.gz` & `tmp/excel_formulas_calculator-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel-formulas-calculator-0.4.2.tar", last modified: Thu Nov 30 16:48:05 2023, max compression
+gzip compressed data, was "excel_formulas_calculator-0.5.0.tar", last modified: Wed May 22 16:14:49 2024, max compression
```

## Comparing `excel-formulas-calculator-0.4.2.tar` & `excel_formulas_calculator-0.5.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.417537 excel-formulas-calculator-0.4.2/efc/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.417537 excel-formulas-calculator-0.4.2/efc/base/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/base/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.417537 excel-formulas-calculator-0.4.2/efc/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/interfaces/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/interfaces/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/interfaces/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/interfaces/iopenpyxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.421537 excel-formulas-calculator-0.4.2/efc/rpn_builder/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.421537 excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.421537 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    26433 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/metaclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    16751 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/operands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/rpn_builder/rpn.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/efc/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2023-11-30 16:48:05.000000 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-11-30 16:48:05.000000 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-30 16:48:05.000000 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-30 16:48:05.000000 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-30 16:48:05.000000 excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.421537 excel-formulas-calculator-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.421537 excel-formulas-calculator-0.4.2/tests/test_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_interfaces/test_iopenpyxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/tests/test_lexer/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_lexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_lexer/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_lexer/test_lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_lexer/test_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/tests/test_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_parser/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-30 16:48:05.425537 excel-formulas-calculator-0.4.2/tests/test_rpn/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/test_arith.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_rpn/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2023-11-30 16:47:56.000000 excel-formulas-calculator-0.4.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.857416 excel_formulas_calculator-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/base/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/base/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/interfaces/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/interfaces/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/interfaces/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/interfaces/iopenpyxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/rpn_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.849416 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26778 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/metaclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17086 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/operands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/rpn_builder/rpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/efc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-05-22 16:14:49.000000 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-22 16:14:49.000000 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:14:49.000000 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 16:14:49.000000 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 16:14:49.000000 excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 16:14:49.857416 excel_formulas_calculator-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/tests/test_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_interfaces/test_iopenpyxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/tests/test_lexer/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_lexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_lexer/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_lexer/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_lexer/test_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/tests/test_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_parser/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:49.853416 excel_formulas_calculator-0.5.0/tests/test_rpn/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/test_arith.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27439 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_rpn/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 16:14:42.000000 excel_formulas_calculator-0.5.0/tests/test_utils.py
```

### Comparing `excel-formulas-calculator-0.4.2/LICENSE` & `excel_formulas_calculator-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/PKG-INFO` & `excel_formulas_calculator-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-formulas-calculator
-Version: 0.4.2
+Version: 0.5.0
 Summary: Library to calculate excel formulas
 Home-page: https://github.com/ulalka/excel-formulas-calculator
 Author: Gleb Orlov
 Author-email: orlovgb@mail.ru
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 2
```

### Comparing `excel-formulas-calculator-0.4.2/README.md` & `excel_formulas_calculator-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/base/errors.py` & `excel_formulas_calculator-0.5.0/efc/base/errors.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/interfaces/base.py` & `excel_formulas_calculator-0.5.0/efc/interfaces/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import partial
 
 from six import add_metaclass
 
 from efc import Lexer, Parser
 from efc.interfaces.cache import CacheManager
 from efc.interfaces.errors import NamedRangeNotFound
-from efc.rpn_builder.parser.operands import CellAddress, RPNOperand, SingleCellOperand
+from efc.rpn_builder.parser.operands import CellAddress, HyperlinkOperand, RPNOperand, SingleCellOperand
 
 
 class CellInfo:
     def __init__(self, value, formula=None):
         self.value = value
         self.formula = formula
 
@@ -47,57 +47,85 @@
     def _caches(self):
         return self._cache_manager
 
     def clear_cache(self):
         """Clear all caches"""
         self._caches.clear()
 
+    def _get_cell_formula_hyperlink(self, address):
+        """
+        :type address: CellAddress
+        :rtype: str | None
+        """
+        if not self._caches:
+            cell_info = self._get_cell_info(address)
+            v = self._calc_extended_value(address, cell_info)
+            return v[1].link if isinstance(v[1], HyperlinkOperand) else None
+        else:
+            self._cell_to_value(address)
+            return self._caches['hyperlinks'].get(address)
+
     @abstractmethod
     def _get_cell_info(self, address):
         """
         :type address: CellAddress
         :rtype: CellInfo
         """
         pass
 
-    def _get_value_with_target_computable_cell(self, cell_addr, cell_info):
+    def _calc_extended_value(self, cell_addr, cell_info):
         """
         :type cell_addr: CellAddress
         :type cell_info: CellInfo
         """
         last_cell_address = cell_addr
         calc = partial(self._build_rpn(cell_info.formula, cell_addr.ws_name).calc, cell_addr.ws_name, self)
         while True:
             partial_result = calc()
             if isinstance(partial_result, SingleCellOperand):
                 value, last_cell_address = self._cell_to_value(partial_result.cell_address)
                 break
             elif isinstance(partial_result, RPNOperand):
-                calc = partial(partial_result.rpn.calc, ws_name=partial_result.ws_name, source=partial_result.source)
+                calc = partial(partial_result.rpn.calc,
+                               ws_name=partial_result.ws_name,
+                               source=partial_result.source)
             else:
                 value = partial_result.value
                 break
-        return value, last_cell_address
+        return value, partial_result, last_cell_address
+    
+    def _store_to_cache(self, cell_addr, value, partial_result, last_cell_address):
+        if isinstance(partial_result, HyperlinkOperand):
+            self._caches['hyperlinks'][cell_addr] = partial_result.link
+        self._caches['cells'][cell_addr] = (value, last_cell_address)
+        
+    def _get_or_calc_extended_value(self, cell_addr, cell_info):
+        """
+        :type cell_addr: CellAddress
+        :type cell_info: CellInfo
+        """
+        if self._caches:
+            if cell_addr not in self._caches['cells']:
+                v, pr, lca = self._calc_extended_value(cell_addr, cell_info)
+                self._store_to_cache(cell_addr, v, pr, lca)
+            return self._caches['cells'][cell_addr]
+        else:
+            v, _, lca = self._calc_extended_value(cell_addr, cell_info)
+            return v, lca
 
     def _cell_to_value(self, cell_addr):
         """
         rtype: tuple[Any, CellAddress]
         """
         cell_info = self._get_cell_info(cell_addr)  # type: CellInfo
 
         if cell_info.formula is None:
             return cell_info.value, cell_addr
         else:
-            if self._caches is not None:
-                if cell_addr not in self._caches['cells']:
-                    self._caches['cells'][cell_addr] = self._get_value_with_target_computable_cell(cell_addr, cell_info)
-                value = self._caches['cells'][cell_addr]
-            else:
-                value = self._get_value_with_target_computable_cell(cell_addr, cell_info)
-            return value
+            return self._get_or_calc_extended_value(cell_addr, cell_info)
 
     @abstractmethod
     def _get_named_range_formula(self, name, ws_name):
         """
         Should raise NamedRangeNotFound if named range not found
         :type name: basestring
         :type ws_name: basestring
```

### Comparing `excel-formulas-calculator-0.4.2/efc/interfaces/cache.py` & `excel_formulas_calculator-0.5.0/efc/interfaces/cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 class CacheManager(object):
     CACHE_TYPES = {
         'single': SingleCellCache,  # cache SingleCellOperand instances
         'cells': SingleCellCache,  # cache calculated Cells
         'range': RangeCache,  # cache CellRangeOperand instances
         'ifs': RangeCache,  # cache IFS expressions for ranges
+        'hyperlinks': SingleCellCache,  # cache hyperlinks for cells
     }
 
     def __init__(self):
         self._caches = {}
 
     def __getitem__(self, item):
         if item not in self._caches:
```

### Comparing `excel-formulas-calculator-0.4.2/efc/interfaces/iopenpyxl.py` & `excel_formulas_calculator-0.5.0/efc/interfaces/iopenpyxl.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,18 @@
         return value
 
     def _deserialize_value(self, value, data_type):
         if data_type == 'd':
             value = parse_date(value)
         return value
 
+    def get_cell_formula_hyperlink(self, cell_index, ws_name):
+        row, column = coordinate_to_tuple(cell_index)
+        return self._get_cell_formula_hyperlink(CellAddress(ws_name, row, column, False, False))
+
     def calc_cell(self, cell_index, ws_name):
         """
         Calculate the cell formula by str index.
         If the cell does not have the formula it returns the cell's value.
         :type cell_index: basestring
         :type ws_name: basestring
         """
```

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/lexer.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/lexer.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/lexer/tokens.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/lexer/tokens.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/errors.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/errors.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/functions.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from efc.rpn_builder.parser.operands import (
     BadReference,
     CellRangeOperand,
     CellSetOperand,
     EmptyOperand,
     ErrorOperand,
+    HyperlinkOperand,
     NamedRangeOperand,
     NotFoundErrorOperand,
     NumErrorOperand,
     RPNOperand,
     SetOperand,
     SimpleOperand,
     SimpleSetOperand,
@@ -671,14 +672,24 @@
         idx = match_function(op, first_row, 1)
     else:
         idx = match_function(op, first_row, 0)
     return SingleCellOperand(row=(rg.row1 or 1) + row.digit - 1, column=(rg.column1 or 1) + idx - 1,
                              ws_name=rg.ws_name, source=rg.source)
 
 
+def hyperlink_function(link, text=None):
+    if isinstance(link, RPNOperand):
+        link = link.evaluated_value
+
+    if isinstance(text, RPNOperand):
+        text = text.evaluated_value
+
+    return HyperlinkOperand(link.value, text.value if text is not None else None)
+
+
 def index_function(rg, row, column=None):
     if isinstance(column, EmptyOperand):
         column = None
 
     if isinstance(rg, RPNOperand):
         rg = rg.evaluated_value
 
@@ -935,14 +946,15 @@
 EXCEL_FUNCTIONS['IFS'] = ifs_func
 EXCEL_FUNCTIONS['IFERROR'] = if_error_func
 EXCEL_FUNCTIONS['INDEX'] = index_function
 EXCEL_FUNCTIONS['ISBLANK'] = is_blank_func
 EXCEL_FUNCTIONS['ISERROR'] = is_error_func
 
 EXCEL_FUNCTIONS['HLOOKUP'] = hlookup_function
+EXCEL_FUNCTIONS['HYPERLINK'] = hyperlink_function
 
 EXCEL_FUNCTIONS['LARGE'] = large_function
 EXCEL_FUNCTIONS['LEN'] = len_func
 EXCEL_FUNCTIONS['LEFT'] = left_func
 EXCEL_FUNCTIONS['LOWER'] = lower_func
 
 EXCEL_FUNCTIONS['MATCH'] = match_function
```

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/metaclasses.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/metaclasses.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/operands.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/operands.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 __all__ = (
     'CellAddress', 'Operand', 'ErrorOperand', 'ValueErrorOperand', 'WorksheetNotExist',
     'ZeroDivisionErrorOperand', 'SimpleOperand', 'SingleCellOperand',
     'CellSetOperand', 'SimpleSetOperand', 'NamedRangeOperand', 'CellRangeOperand',
     'FunctionNotSupported', 'NotFoundErrorOperand', 'RPNOperand', 'OperandLikeObject', 'OffsetMixin',
     'SetOperand', 'BadReference', 'ValueNotAvailable', 'EmptyOperand', 'NamedRangeNotExist', 'NumErrorOperand',
+    'HyperlinkOperand',
 )
 
 CellAddress = namedtuple('CellAddress', ('ws_name', 'row', 'column', 'row_fixed', 'column_fixed'))
 
 
 class OperandLikeObject(object):
     def __init__(self, ws_name=None, source=None, *args, **kwargs):
@@ -537,7 +538,18 @@
         return text_type(self.evaluated_value)
 
     def __trunc__(self):
         return self.__int__()
 
     def __iter__(self):
         return iter(self.evaluated_value)
+
+
+class HyperlinkOperand(Operand):
+    def __init__(self, link, text=None, *args, **kwargs):
+        self.link = link
+        self.text = text
+        super(HyperlinkOperand, self).__init__(*args, **kwargs)
+
+    @cached_property
+    def value(self):
+        return self.link if self.text is None else self.text
```

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/operations.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/operations.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/parser/parser.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/parser/parser.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/rpn_builder/rpn.py` & `excel_formulas_calculator-0.5.0/efc/rpn_builder/rpn.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/efc/utils.py` & `excel_formulas_calculator-0.5.0/efc/utils.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/PKG-INFO` & `excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel-formulas-calculator
-Version: 0.4.2
+Version: 0.5.0
 Summary: Library to calculate excel formulas
 Home-page: https://github.com/ulalka/excel-formulas-calculator
 Author: Gleb Orlov
 Author-email: orlovgb@mail.ru
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 2
```

### Comparing `excel-formulas-calculator-0.4.2/excel_formulas_calculator.egg-info/SOURCES.txt` & `excel_formulas_calculator-0.5.0/excel_formulas_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/setup.py` & `excel_formulas_calculator-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_interfaces/test_iopenpyxl.py` & `excel_formulas_calculator-0.5.0/tests/test_interfaces/test_iopenpyxl.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,7 +95,29 @@
 
 
 def test_openpyxl_cache_disabled(workbook):
     interface = OpenpyxlInterface(workbook, use_cache=False)
     assert interface.calc_cell('B1', 'ws1') == 2
     workbook['ws1']['A1'].value = 3
     assert interface.calc_cell('B1', 'ws1') == 4
+
+
+@pytest.mark.parametrize('use_cache', (False, True))
+@pytest.mark.parametrize(
+    ('cell', 'hyperlink', 'value'),
+    [
+        ('A1', 'https://ya.ru', 'https://ya.ru'),
+        ('A2', 'https://ya.ru', 'text'),
+        ('A3', 'https://ya.ru', 'lalala'),
+        ('A4', 'https://ya2.ru', 'bababa'),
+        ('A5', 'https://ya2.ru', 'bababa'),
+        ('A6', 'https://ya.ru', 'https://ya.ru'),
+        ('A7', 'http://ya.ru', 'Яндекс'),
+        ('A8', None, 2468),
+        ('A9', None, 'https://ya.rutext'),
+        ('A10', None, 'https://ya.ru'),
+    ]
+)
+def test_hyperlink(workbook, cell, hyperlink, value, use_cache):
+    interface = OpenpyxlInterface(workbook, use_cache=use_cache)
+    assert interface.calc_cell(cell, 'hyperlink') == value
+    assert interface.get_cell_formula_hyperlink(cell, 'hyperlink') == hyperlink
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `excel-formulas-calculator-0.4.2/tests/test_lexer/test_errors.py` & `excel_formulas_calculator-0.5.0/tests/test_lexer/test_errors.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_lexer/test_lexer.py` & `excel_formulas_calculator-0.5.0/tests/test_lexer/test_lexer.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_lexer/test_tokens.py` & `excel_formulas_calculator-0.5.0/tests/test_lexer/test_tokens.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_parser/test_parser.py` & `excel_formulas_calculator-0.5.0/tests/test_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_rpn/mock.py` & `excel_formulas_calculator-0.5.0/tests/test_rpn/mock.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_rpn/test_arith.py` & `excel_formulas_calculator-0.5.0/tests/test_rpn/test_arith.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_rpn/test_cells.py` & `excel_formulas_calculator-0.5.0/tests/test_rpn/test_cells.py`

 * *Files identical despite different names*

### Comparing `excel-formulas-calculator-0.4.2/tests/test_rpn/test_functions.py` & `excel_formulas_calculator-0.5.0/tests/test_rpn/test_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pytest
 from openpyxl import load_workbook
 from openpyxl.utils.cell import get_column_letter
 
 from efc.interfaces.iopenpyxl import OpenpyxlInterface
 from efc.rpn_builder.parser.operands import (
     BadReference,
-    NotFoundErrorOperand, NumErrorOperand,
-    ValueErrorOperand,
+    HyperlinkOperand, NotFoundErrorOperand, NumErrorOperand,
+    RPNOperand, ValueErrorOperand,
     ValueNotAvailable,
     ZeroDivisionErrorOperand,
 )
 from .mock import ExcelMock, get_calculator
 
 
 @pytest.fixture(scope='session')
@@ -253,14 +253,35 @@
      pytest.param('HLOOKUP(24,TestHLookup!A1:B3,2)', 12435,
                   marks=pytest.mark.xfail(raises=NotFoundErrorOperand, strict=True))),
 )
 def test_HLOOKUP(calc, formula, result):
     assert calc(formula, 'Sheet4').value == result
 
 
+@pytest.mark.parametrize(
+    ('formula', 'link', 'text'),
+    (('HYPERLINK("https://ya.ru")', 'https://ya.ru', None),
+     ('HYPERLINK("https://ya.ru", "text")', 'https://ya.ru', 'text'),
+     ('HYPERLINK("https://ya.ru", IF(TRUE, "lalala", "bababa"))', 'https://ya.ru', 'lalala'),
+     ('HYPERLINK(IF(FALSE, "https://ya.ru", "https://yandex.ru"),  "bababa")', 'https://yandex.ru', 'bababa'),
+     ('HYPERLINK(IF(FALSE, "https://ya.ru", "https://ya2.ru"),  IF(FALSE, "lalala", "ba"))', 'https://ya2.ru', 'ba'),
+     ('IF(TRUE, HYPERLINK("https://ya.ru"), HYPERLINK("https://ya2.ru"))', 'https://ya.ru', None),
+     ('IF(FALSE, HYPERLINK("https://ya.ru"), HYPERLINK("https://ya2.ru"))', 'https://ya2.ru', None),
+     ),
+)
+def test_HYPERLINK(calc, formula, link, text):
+    result = calc(formula, 'Sheet4')
+    if isinstance(result, RPNOperand):
+        result = result.evaluated_value
+
+    assert isinstance(result, HyperlinkOperand)
+    assert result.link == link
+    assert result.text == text
+
+
 def test_SEARCH(calc):
     assert calc('SEARCH("abc", "abc")', 'Yet another sheet').value == 1
     assert calc('SEARCH("abc", "abc", 1)', 'Yet another sheet').value == 1
     assert calc('SEARCH("abc", "aabc", 1)', 'Yet another sheet').value == 2
 
     with pytest.raises(ValueErrorOperand):
         assert calc('SEARCH("abcd", "abc")', 'Yet another sheet').value
```

### Comparing `excel-formulas-calculator-0.4.2/tests/test_utils.py` & `excel_formulas_calculator-0.5.0/tests/test_utils.py`

 * *Files identical despite different names*

