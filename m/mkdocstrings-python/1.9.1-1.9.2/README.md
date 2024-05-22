# Comparing `tmp/mkdocstrings_python-1.9.1.tar.gz` & `tmp/mkdocstrings_python-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings_python-1.9.1.tar", last modified: Tue Apr  2 16:48:14 2024, max compression
+gzip compressed data, was "mkdocstrings_python-1.9.2.tar", last modified: Tue Apr  2 19:28:04 2024, max compression
```

## Comparing `mkdocstrings_python-1.9.1.tar` & `mkdocstrings_python-1.9.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      754 2024-03-13 18:37:57.897079 mkdocstrings_python-1.9.1/LICENSE
--rw-r--r--   0        0        0     4043 2024-03-13 18:43:23.554055 mkdocstrings_python-1.9.1/README.md
--rw-r--r--   0        0        0     1649 2024-04-02 16:48:14.142973 mkdocstrings_python-1.9.1/pyproject.toml
--rw-r--r--   0        0        0      128 2024-03-13 18:37:58.007075 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/__init__.py
--rw-r--r--   0        0        0     2764 2024-03-13 18:47:50.869435 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/debug.py
--rw-r--r--   0        0        0    23165 2024-04-02 14:58:09.507865 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/handler.py
--rw-r--r--   0        0        0        0 2024-03-13 18:37:58.043741 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/py.typed
--rw-r--r--   0        0        0    16542 2024-03-28 17:33:18.921686 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/rendering.py
--rw-r--r--   0        0        0     2944 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
--rw-r--r--   0        0        0     5709 2024-01-08 15:33:33.297408 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html
--rw-r--r--   0        0        0     5413 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html
--rw-r--r--   0        0        0     2163 2024-01-08 15:33:33.354072 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
--rw-r--r--   0        0        0      274 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
--rw-r--r--   0        0        0     3101 2024-01-31 11:17:41.321947 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
--rw-r--r--   0        0        0     2144 2024-01-31 11:18:21.618366 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html
--rw-r--r--   0        0        0      460 2024-01-08 15:33:33.444069 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
--rw-r--r--   0        0        0     2667 2024-01-31 11:18:34.984950 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html
--rw-r--r--   0        0        0     2158 2024-01-31 11:18:43.178233 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html
--rw-r--r--   0        0        0     2887 2024-01-31 11:30:21.673669 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
--rw-r--r--   0        0        0     3844 2024-01-31 11:30:30.813558 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
--rw-r--r--   0        0        0     2499 2024-01-31 11:30:38.240136 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
--rw-r--r--   0        0        0     3524 2024-01-31 11:30:44.303396 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
--rw-r--r--   0        0        0     3500 2024-01-31 11:30:52.079970 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
--rw-r--r--   0        0        0     2474 2024-01-31 11:30:58.983221 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
--rw-r--r--   0        0        0     3465 2024-01-31 11:31:06.949793 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
--rw-r--r--   0        0        0     2078 2024-01-08 15:33:33.277408 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
--rw-r--r--   0        0        0     3515 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html
--rw-r--r--   0        0        0      273 2024-03-24 15:10:20.465351 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
--rw-r--r--   0        0        0      966 2024-01-08 15:33:33.317407 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
--rw-r--r--   0        0        0      984 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
--rw-r--r--   0        0        0      902 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
--rw-r--r--   0        0        0     2480 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html
--rw-r--r--   0        0        0     2833 2024-02-20 12:56:18.816418 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/summary.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/summary/attributes.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/summary/classes.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/summary/functions.html
--rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/summary/modules.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/attribute.html
--rw-r--r--   0        0        0       36 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/children.html
--rw-r--r--   0        0        0       33 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/class.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/classes.html
--rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
--rw-r--r--   0        0        0       47 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/functions.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/modules.html
--rw-r--r--   0        0        0       54 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
--rw-r--r--   0        0        0       48 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
--rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
--rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
--rw-r--r--   0        0        0       45 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
--rw-r--r--   0        0        0       43 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
--rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
--rw-r--r--   0        0        0       38 2024-01-08 15:33:33.254076 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/expression.html
--rw-r--r--   0        0        0       36 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/function.html
--rw-r--r--   0        0        0       34 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/labels.html
--rw-r--r--   0        0        0      431 2024-01-08 15:33:33.154079 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/language.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/languages/en.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
--rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
--rw-r--r--   0        0        0       34 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/module.html
--rw-r--r--   0        0        0       37 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/signature.html
--rw-r--r--   0        0        0     2631 2024-03-24 15:10:29.598590 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/style.css
--rw-r--r--   0        0        0       35 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/summary.html
--rw-r--r--   0        0        0       46 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/summary/attributes.html
--rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/summary/classes.html
--rw-r--r--   0        0        0       45 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/summary/functions.html
--rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/summary/modules.html
--rw-r--r--   0        0        0     1001 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
--rw-r--r--   0        0        0     1007 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
--rw-r--r--   0        0        0     1279 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
--rw-r--r--   0        0        0      928 2024-01-08 15:33:33.810723 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
--rw-r--r--   0        0        0     1131 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
--rw-r--r--   0        0        0     1080 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
--rw-r--r--   0        0        0      923 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
--rw-r--r--   0        0        0     1114 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
--rw-r--r--   0        0        0      431 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
--rw-r--r--   0        0        0      966 2024-01-08 15:33:33.600731 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
--rw-r--r--   0        0        0      984 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
--rw-r--r--   0        0        0      902 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
--rw-r--r--   0        0        0      971 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
--rw-r--r--   0        0        0      174 2024-03-13 18:38:00.683662 mkdocstrings_python-1.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2915 2024-03-13 18:52:36.467604 mkdocstrings_python-1.9.1/tests/conftest.py
--rw-r--r--   0        0        0     5206 2024-01-08 15:33:33.874055 mkdocstrings_python-1.9.1/tests/test_handler.py
--rw-r--r--   0        0        0     5450 2024-01-08 15:33:33.890721 mkdocstrings_python-1.9.1/tests/test_rendering.py
--rw-r--r--   0        0        0     1281 2024-03-13 18:54:08.091544 mkdocstrings_python-1.9.1/tests/test_themes.py
--rw-r--r--   0        0        0     5524 1970-01-01 00:00:00.000000 mkdocstrings_python-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-13 18:37:57.897079 mkdocstrings_python-1.9.2/LICENSE
+-rw-r--r--   0        0        0     4043 2024-03-13 18:43:23.554055 mkdocstrings_python-1.9.2/README.md
+-rw-r--r--   0        0        0     1625 2024-04-02 19:28:04.380673 mkdocstrings_python-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-03-13 18:37:58.007075 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/__init__.py
+-rw-r--r--   0        0        0     2764 2024-03-13 18:47:50.869435 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/debug.py
+-rw-r--r--   0        0        0    23165 2024-04-02 14:58:09.507865 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/handler.py
+-rw-r--r--   0        0        0        0 2024-03-13 18:37:58.043741 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/py.typed
+-rw-r--r--   0        0        0    16542 2024-03-28 17:33:18.921686 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/rendering.py
+-rw-r--r--   0        0        0     2944 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html
+-rw-r--r--   0        0        0     5709 2024-01-08 15:33:33.297408 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/children.html
+-rw-r--r--   0        0        0     5413 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html
+-rw-r--r--   0        0        0     2163 2024-01-08 15:33:33.354072 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html
+-rw-r--r--   0        0        0      274 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/admonition.html
+-rw-r--r--   0        0        0     3101 2024-01-31 11:17:41.321947 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html
+-rw-r--r--   0        0        0     2144 2024-01-31 11:18:21.618366 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html
+-rw-r--r--   0        0        0      460 2024-01-08 15:33:33.444069 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/examples.html
+-rw-r--r--   0        0        0     2667 2024-01-31 11:18:34.984950 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html
+-rw-r--r--   0        0        0     2158 2024-01-31 11:18:43.178233 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html
+-rw-r--r--   0        0        0     2887 2024-01-31 11:30:21.673669 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html
+-rw-r--r--   0        0        0     3844 2024-01-31 11:30:30.813558 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html
+-rw-r--r--   0        0        0     2499 2024-01-31 11:30:38.240136 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html
+-rw-r--r--   0        0        0     3524 2024-01-31 11:30:44.303396 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html
+-rw-r--r--   0        0        0     3500 2024-01-31 11:30:52.079970 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html
+-rw-r--r--   0        0        0     2474 2024-01-31 11:30:58.983221 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html
+-rw-r--r--   0        0        0     3465 2024-01-31 11:31:06.949793 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html
+-rw-r--r--   0        0        0     2078 2024-01-08 15:33:33.277408 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html
+-rw-r--r--   0        0        0     3515 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html
+-rw-r--r--   0        0        0      273 2024-03-24 15:10:20.465351 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/labels.html
+-rw-r--r--   0        0        0      966 2024-01-08 15:33:33.317407 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html
+-rw-r--r--   0        0        0      984 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html
+-rw-r--r--   0        0        0      902 2024-01-08 15:33:33.320740 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html
+-rw-r--r--   0        0        0     2480 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html
+-rw-r--r--   0        0        0     2833 2024-02-20 12:56:18.816418 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.064308 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/summary.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/summary/attributes.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/summary/classes.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/summary/functions.html
+-rw-r--r--   0        0        0        0 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/summary/modules.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/attribute.html
+-rw-r--r--   0        0        0       36 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/children.html
+-rw-r--r--   0        0        0       33 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/class.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.217410 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/admonition.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/attributes.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/classes.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/examples.html
+-rw-r--r--   0        0        0       47 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/functions.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.500734 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/modules.html
+-rw-r--r--   0        0        0       54 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/other_parameters.html
+-rw-r--r--   0        0        0       48 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/parameters.html
+-rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/raises.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/receives.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/returns.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:33:33.517400 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/warns.html
+-rw-r--r--   0        0        0       44 2024-01-08 15:33:33.520733 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/docstring/yields.html
+-rw-r--r--   0        0        0       38 2024-01-08 15:33:33.254076 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/expression.html
+-rw-r--r--   0        0        0       36 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/function.html
+-rw-r--r--   0        0        0       34 2024-01-08 15:33:33.230743 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/labels.html
+-rw-r--r--   0        0        0      431 2024-01-08 15:33:33.154079 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/language.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/languages/en.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/languages/ja.html
+-rw-r--r--   0        0        0       39 2024-01-08 15:33:33.180745 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/languages/zh.html
+-rw-r--r--   0        0        0       34 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/module.html
+-rw-r--r--   0        0        0       37 2024-01-08 15:33:33.250743 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/signature.html
+-rw-r--r--   0        0        0     2631 2024-03-24 15:10:29.598590 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/style.css
+-rw-r--r--   0        0        0       35 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/summary.html
+-rw-r--r--   0        0        0       46 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/summary/attributes.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/summary/classes.html
+-rw-r--r--   0        0        0       45 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/summary/functions.html
+-rw-r--r--   0        0        0       43 2024-01-08 15:59:07.067641 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/summary/modules.html
+-rw-r--r--   0        0        0     1001 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html
+-rw-r--r--   0        0        0     1007 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html
+-rw-r--r--   0        0        0     1279 2024-01-08 15:33:33.614064 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html
+-rw-r--r--   0        0        0      928 2024-01-08 15:33:33.810723 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html
+-rw-r--r--   0        0        0     1131 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html
+-rw-r--r--   0        0        0     1080 2024-01-08 15:33:33.837389 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html
+-rw-r--r--   0        0        0      923 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html
+-rw-r--r--   0        0        0     1114 2024-01-08 15:33:33.840722 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html
+-rw-r--r--   0        0        0      431 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/language.html
+-rw-r--r--   0        0        0      966 2024-01-08 15:33:33.600731 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html
+-rw-r--r--   0        0        0      984 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html
+-rw-r--r--   0        0        0      902 2024-01-08 15:33:33.610730 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html
+-rw-r--r--   0        0        0      971 2024-01-08 15:33:33.557399 mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css
+-rw-r--r--   0        0        0      174 2024-03-13 18:38:00.683662 mkdocstrings_python-1.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2915 2024-03-13 18:52:36.467604 mkdocstrings_python-1.9.2/tests/conftest.py
+-rw-r--r--   0        0        0     5206 2024-01-08 15:33:33.874055 mkdocstrings_python-1.9.2/tests/test_handler.py
+-rw-r--r--   0        0        0     5450 2024-01-08 15:33:33.890721 mkdocstrings_python-1.9.2/tests/test_rendering.py
+-rw-r--r--   0        0        0     1281 2024-03-13 18:54:08.091544 mkdocstrings_python-1.9.2/tests/test_themes.py
+-rw-r--r--   0        0        0     5492 1970-01-01 00:00:00.000000 mkdocstrings_python-1.9.2/PKG-INFO
```

### Comparing `mkdocstrings_python-1.9.1/LICENSE` & `mkdocstrings_python-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/README.md` & `mkdocstrings_python-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/pyproject.toml` & `mkdocstrings_python-1.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -27,19 +27,18 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Documentation",
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
-    "markdown>=3.3,<3.6",
-    "mkdocstrings>=0.20",
+    "mkdocstrings>=0.24.2",
     "griffe>=0.37",
 ]
-version = "1.9.1"
+version = "1.9.2"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://mkdocstrings.github.io/python"
 Documentation = "https://mkdocstrings.github.io/python"
```

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/debug.py` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/debug.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/handler.py` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/rendering.py` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/attribute.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/children.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/children.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/class.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/class.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/classes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/functions.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/modules.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/expression.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/expression.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/function.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/function.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/en.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/ja.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/languages/zh.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/module.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/module.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/_base/signature.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/_base/signature.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/material/style.css` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/attributes.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/other_parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/parameters.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/raises.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/receives.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/returns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/warns.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/docstring/yields.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/en.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/ja.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/languages/zh.html`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/src/mkdocstrings_handlers/python/templates/readthedocs/style.css` & `mkdocstrings_python-1.9.2/src/mkdocstrings_handlers/python/templates/readthedocs/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/tests/conftest.py` & `mkdocstrings_python-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/tests/test_handler.py` & `mkdocstrings_python-1.9.2/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/tests/test_rendering.py` & `mkdocstrings_python-1.9.2/tests/test_rendering.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/tests/test_themes.py` & `mkdocstrings_python-1.9.2/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `mkdocstrings_python-1.9.1/PKG-INFO` & `mkdocstrings_python-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocstrings-python
-Version: 1.9.1
+Version: 1.9.2
 Summary: A Python handler for mkdocstrings.
 Author-Email: Timothée Mazzucotelli <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -23,16 +23,15 @@
 Project-URL: Changelog, https://mkdocstrings.github.io/python/changelog
 Project-URL: Repository, https://github.com/mkdocstrings/python
 Project-URL: Issues, https://github.com/mkdocstrings/python/issues
 Project-URL: Discussions, https://github.com/mkdocstrings/python/discussions
 Project-URL: Gitter, https://gitter.im/mkdocstrings/python
 Project-URL: Funding, https://github.com/sponsors/pawamoy
 Requires-Python: >=3.8
-Requires-Dist: markdown<3.6,>=3.3
-Requires-Dist: mkdocstrings>=0.20
+Requires-Dist: mkdocstrings>=0.24.2
 Requires-Dist: griffe>=0.37
 Description-Content-Type: text/markdown
 
 <h1 align="center">mkdocstrings-python</h1>
 
 <p align="center">A Python handler for <a href="https://github.com/mkdocstrings/mkdocstrings"><i>mkdocstrings</i></a>.</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.9.1 Summary: A
+Metadata-Version: 2.1 Name: mkdocstrings-python Version: 1.9.2 Summary: A
 Python handler for mkdocstrings. Author-Email: TimothÃ©e Mazzucotelli
 pawamoy.fr> License: ISC Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
@@ -12,17 +12,16 @@
 mkdocstrings.github.io/python Project-URL: Documentation, https://
 mkdocstrings.github.io/python Project-URL: Changelog, https://
 mkdocstrings.github.io/python/changelog Project-URL: Repository, https://
 github.com/mkdocstrings/python Project-URL: Issues, https://github.com/
 mkdocstrings/python/issues Project-URL: Discussions, https://github.com/
 mkdocstrings/python/discussions Project-URL: Gitter, https://gitter.im/
 mkdocstrings/python Project-URL: Funding, https://github.com/sponsors/pawamoy
-Requires-Python: >=3.8 Requires-Dist: markdown<3.6,>=3.3 Requires-Dist:
-mkdocstrings>=0.20 Requires-Dist: griffe>=0.37 Description-Content-Type: text/
-markdown
+Requires-Python: >=3.8 Requires-Dist: mkdocstrings>=0.24.2 Requires-Dist:
+griffe>=0.37 Description-Content-Type: text/markdown
                        ************ mmkkddooccssttrriinnggss--ppyytthhoonn ************
                       A Python handler for _m_k_d_o_c_s_t_r_i_n_g_s.
 [![ci](https://github.com/mkdocstrings/python/workflows/ci/badge.svg)](https://
 github.com/mkdocstrings/python/actions?query=workflow%3Aci) [![documentation]
 (https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)]
 (https://mkdocstrings.github.io/python/) [![pypi version](https://
 img.shields.io/pypi/v/mkdocstrings-python.svg)](https://pypi.org/project/
```

