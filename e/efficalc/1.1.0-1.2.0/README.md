# Comparing `tmp/efficalc-1.1.0.tar.gz` & `tmp/efficalc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efficalc-1.1.0.tar", last modified: Sun Mar 24 06:06:31 2024, max compression
+gzip compressed data, was "efficalc-1.2.0.tar", last modified: Wed May 22 00:30:45 2024, max compression
```

## Comparing `efficalc-1.1.0.tar` & `efficalc-1.2.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.063204 efficalc-1.1.0/
--rw-rw-rw-   0        0        0     1090 2024-02-14 18:49:25.000000 efficalc-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     7175 2024-03-24 06:06:31.061961 efficalc-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6414 2024-03-24 06:05:53.000000 efficalc-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.025963 efficalc-1.1.0/efficalc/
--rw-rw-rw-   0        0        0     1349 2024-03-23 23:13:22.000000 efficalc-1.1.0/efficalc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.042038 efficalc-1.1.0/efficalc/base_definitions/
--rw-rw-rw-   0        0        0        0 2024-03-02 05:16:31.000000 efficalc-1.1.0/efficalc/base_definitions/__init__.py
--rw-rw-rw-   0        0        0      703 2024-02-24 06:33:48.000000 efficalc-1.1.0/efficalc/base_definitions/assumption.py
--rw-rw-rw-   0        0        0     5978 2024-03-06 17:42:09.000000 efficalc-1.1.0/efficalc/base_definitions/calculation.py
--rw-rw-rw-   0        0        0     7377 2024-03-06 17:41:42.000000 efficalc-1.1.0/efficalc/base_definitions/comparison.py
--rw-rw-rw-   0        0        0     3666 2024-03-06 17:42:28.000000 efficalc-1.1.0/efficalc/base_definitions/comparison_statement.py
--rw-rw-rw-   0        0        0     3891 2024-03-23 23:13:22.000000 efficalc-1.1.0/efficalc/base_definitions/figure.py
--rw-rw-rw-   0        0        0     1776 2024-03-06 16:54:52.000000 efficalc-1.1.0/efficalc/base_definitions/heading.py
--rw-rw-rw-   0        0        0     5221 2024-03-06 17:32:47.000000 efficalc-1.1.0/efficalc/base_definitions/input.py
--rw-rw-rw-   0        0        0     2419 2024-03-23 23:32:35.000000 efficalc-1.1.0/efficalc/base_definitions/shared.py
--rw-rw-rw-   0        0        0      658 2024-03-06 17:38:35.000000 efficalc-1.1.0/efficalc/base_definitions/text_block.py
--rw-rw-rw-   0        0        0      499 2024-03-06 17:39:50.000000 efficalc-1.1.0/efficalc/base_definitions/title.py
--rw-rw-rw-   0        0        0     3885 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/calculation_runner.py
--rw-rw-rw-   0        0        0      660 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/constants.py
--rw-rw-rw-   0        0        0     9746 2024-03-23 23:59:30.000000 efficalc-1.1.0/efficalc/generate_html.py
--rw-rw-rw-   0        0        0     5951 2024-03-24 04:56:24.000000 efficalc-1.1.0/efficalc/report_builder.py
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.055459 efficalc-1.1.0/efficalc/sections/
--rw-rw-rw-   0        0        0      665 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/__init__.py
--rw-rw-rw-   0        0        0     8013 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/aisc_angle.py
--rw-rw-rw-   0        0        0     6214 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/aisc_channel.py
--rw-rw-rw-   0        0        0     6050 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/aisc_circular.py
--rw-rw-rw-   0        0        0    19040 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/aisc_double_angle.py
--rw-rw-rw-   0        0        0    10930 2024-03-20 18:38:33.000000 efficalc-1.1.0/efficalc/sections/aisc_rectangular.py
--rw-rw-rw-   0        0        0     9701 2024-03-20 18:38:34.000000 efficalc-1.1.0/efficalc/sections/aisc_tee.py
--rw-rw-rw-   0        0        0    10045 2024-03-20 18:38:34.000000 efficalc-1.1.0/efficalc/sections/aisc_wide_flange.py
--rw-rw-rw-   0        0        0   647168 2024-03-07 04:59:50.000000 efficalc-1.1.0/efficalc/sections/section_properties.db
--rw-rw-rw-   0        0        0     7724 2024-03-20 18:38:34.000000 efficalc-1.1.0/efficalc/sections/section_query.py
--rw-rw-rw-   0        0        0     1295 2024-03-20 18:38:34.000000 efficalc-1.1.0/efficalc/unit_conversions.py
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.060961 efficalc-1.1.0/efficalc.egg-info/
--rw-rw-rw-   0        0        0     7175 2024-03-24 06:06:30.000000 efficalc-1.1.0/efficalc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1246 2024-03-24 06:06:31.000000 efficalc-1.1.0/efficalc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 06:06:30.000000 efficalc-1.1.0/efficalc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-03-24 06:06:30.000000 efficalc-1.1.0/efficalc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-24 06:06:30.000000 efficalc-1.1.0/efficalc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1029 2024-03-23 23:13:57.000000 efficalc-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-24 06:06:31.063204 efficalc-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-24 06:06:31.059955 efficalc-1.1.0/tests/
--rw-rw-rw-   0        0        0     3890 2024-03-20 18:38:34.000000 efficalc-1.1.0/tests/test_calculation_runner.py
--rw-rw-rw-   0        0        0    12291 2024-03-24 00:05:01.000000 efficalc-1.1.0/tests/test_generate_html.py
--rw-rw-rw-   0        0        0    13011 2024-02-28 17:10:29.000000 efficalc-1.1.0/tests/test_math_operations.py
--rw-rw-rw-   0        0        0     8220 2024-03-24 04:33:55.000000 efficalc-1.1.0/tests/test_report_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.600422 efficalc-1.2.0/
+-rw-rw-rw-   0        0        0     1090 2024-02-14 18:49:25.000000 efficalc-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     7582 2024-05-22 00:30:45.598421 efficalc-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6821 2024-05-22 00:24:33.000000 efficalc-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.535962 efficalc-1.2.0/efficalc/
+-rw-rw-rw-   0        0        0     1398 2024-04-23 03:54:19.000000 efficalc-1.2.0/efficalc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.563445 efficalc-1.2.0/efficalc/base_definitions/
+-rw-rw-rw-   0        0        0        0 2024-03-02 05:16:31.000000 efficalc-1.2.0/efficalc/base_definitions/__init__.py
+-rw-rw-rw-   0        0        0      703 2024-02-24 06:33:48.000000 efficalc-1.2.0/efficalc/base_definitions/assumption.py
+-rw-rw-rw-   0        0        0     6036 2024-05-21 21:39:09.000000 efficalc-1.2.0/efficalc/base_definitions/calculation.py
+-rw-rw-rw-   0        0        0     7376 2024-05-21 21:04:51.000000 efficalc-1.2.0/efficalc/base_definitions/comparison.py
+-rw-rw-rw-   0        0        0     3666 2024-03-06 17:42:28.000000 efficalc-1.2.0/efficalc/base_definitions/comparison_statement.py
+-rw-rw-rw-   0        0        0     3891 2024-03-23 23:13:22.000000 efficalc-1.2.0/efficalc/base_definitions/figure.py
+-rw-rw-rw-   0        0        0     1776 2024-03-06 16:54:52.000000 efficalc-1.2.0/efficalc/base_definitions/heading.py
+-rw-rw-rw-   0        0        0     5214 2024-05-21 21:04:51.000000 efficalc-1.2.0/efficalc/base_definitions/input.py
+-rw-rw-rw-   0        0        0     2535 2024-05-21 21:39:08.000000 efficalc-1.2.0/efficalc/base_definitions/shared.py
+-rw-rw-rw-   0        0        0     5469 2024-05-22 00:20:49.000000 efficalc-1.2.0/efficalc/base_definitions/symbolic.py
+-rw-rw-rw-   0        0        0      658 2024-03-06 17:38:35.000000 efficalc-1.2.0/efficalc/base_definitions/text_block.py
+-rw-rw-rw-   0        0        0      499 2024-03-06 17:39:50.000000 efficalc-1.2.0/efficalc/base_definitions/title.py
+-rw-rw-rw-   0        0        0     3985 2024-05-21 20:59:45.000000 efficalc-1.2.0/efficalc/calculation_runner.py
+-rw-rw-rw-   0        0        0      660 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/constants.py
+-rw-rw-rw-   0        0        0    10572 2024-05-21 21:17:01.000000 efficalc-1.2.0/efficalc/generate_html.py
+-rw-rw-rw-   0        0        0     5951 2024-03-24 06:17:46.000000 efficalc-1.2.0/efficalc/report_builder.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.586800 efficalc-1.2.0/efficalc/sections/
+-rw-rw-rw-   0        0        0      665 2024-04-23 02:48:48.000000 efficalc-1.2.0/efficalc/sections/__init__.py
+-rw-rw-rw-   0        0        0     8013 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/sections/aisc_angle.py
+-rw-rw-rw-   0        0        0     6214 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/sections/aisc_channel.py
+-rw-rw-rw-   0        0        0     6050 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/sections/aisc_circular.py
+-rw-rw-rw-   0        0        0    19040 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/sections/aisc_double_angle.py
+-rw-rw-rw-   0        0        0    10930 2024-03-20 18:38:33.000000 efficalc-1.2.0/efficalc/sections/aisc_rectangular.py
+-rw-rw-rw-   0        0        0     9701 2024-03-20 18:38:34.000000 efficalc-1.2.0/efficalc/sections/aisc_tee.py
+-rw-rw-rw-   0        0        0    10045 2024-03-20 18:38:34.000000 efficalc-1.2.0/efficalc/sections/aisc_wide_flange.py
+-rw-rw-rw-   0        0        0   647168 2024-04-23 02:48:48.000000 efficalc-1.2.0/efficalc/sections/section_properties.db
+-rw-rw-rw-   0        0        0     7724 2024-04-23 02:48:48.000000 efficalc-1.2.0/efficalc/sections/section_query.py
+-rw-rw-rw-   0        0        0     1295 2024-03-20 18:38:34.000000 efficalc-1.2.0/efficalc/unit_conversions.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.597413 efficalc-1.2.0/efficalc.egg-info/
+-rw-rw-rw-   0        0        0     7582 2024-05-22 00:30:45.000000 efficalc-1.2.0/efficalc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1284 2024-05-22 00:30:45.000000 efficalc-1.2.0/efficalc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 00:30:45.000000 efficalc-1.2.0/efficalc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-22 00:30:45.000000 efficalc-1.2.0/efficalc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 00:30:45.000000 efficalc-1.2.0/efficalc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1029 2024-05-22 00:26:49.000000 efficalc-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 00:30:45.601421 efficalc-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 00:30:45.596204 efficalc-1.2.0/tests/
+-rw-rw-rw-   0        0        0     3890 2024-03-20 18:38:34.000000 efficalc-1.2.0/tests/test_calculation_runner.py
+-rw-rw-rw-   0        0        0    13632 2024-05-21 23:56:17.000000 efficalc-1.2.0/tests/test_generate_html.py
+-rw-rw-rw-   0        0        0    13011 2024-02-28 17:10:29.000000 efficalc-1.2.0/tests/test_math_operations.py
+-rw-rw-rw-   0        0        0     8220 2024-03-24 06:17:46.000000 efficalc-1.2.0/tests/test_report_builder.py
```

### Comparing `efficalc-1.1.0/LICENSE` & `efficalc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/PKG-INFO` & `efficalc-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficalc
-Version: 1.1.0
+Version: 1.2.0
 Summary: Feature-rich open source library for building well-formatted and extensible engineering calculations.
 Author-email: Andrew Young <youandvern@gmail.com>
 Project-URL: Homepage, https://github.com/youandvern/efficalc
 Project-URL: Documentation, https://youandvern.github.io/efficalc
 Project-URL: Issues, https://github.com/youandvern/efficalc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,87 +18,68 @@
 
 <p align="center">
   <img src="https://github.com/youandvern/efficalc/raw/main/docs_src/efficalc.png" alt="Logo" width="200"/>
 </p>
 
 <p align="center">
   <a href="https://github.com/youandvern/efficalc/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/youandvern/efficalc/actions/workflows/tests.yml/badge.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.1.0"></a>&nbsp;&nbsp;&nbsp;
+  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.2.0"></a>&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/youandvern/efficalc/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.1.0"></a>
+  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.2.0"></a>
 </p>
 
 
 # efficalc
 
 ### A feature-rich Python library for reimagined engineering calculations.
 
 <!-- TABLE OF CONTENTS -->
 <details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li><a href="#introduction">Introduction</a></li>
-    <li><a href="#links">Links</a></li>
+  <summary style="font-size:1.5rem;"><b>Contents</b></summary>
+  <ul>
+    <li><a href="#introduction">Introduction</a><ul>
+        <li><a href="#examples">Examples</a></li>
+        <li><a href="#documentation-and-distribution">Documentation</a></li></ul></li>
+    <li><a href="#quickstart">Quickstart</a><ul>
+        <li><a href="#installation">Installation</a></li>
+        <li><a href="#first-calculation-function">First Calculation</a></li>
+        <li><a href="#view-the-report">View Report</a></li></ul></li>
     <li><a href="#features">Features</a></li>
-    <li><a href="#quickstart">Quickstart</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#built-with">Built With</a></li>
-    <li><a href="#license">License</a></li>
-  </ol>
+  </ul>
 </details>
 
 
-
-## Introduction
+# Introduction
 
 ##### efficalc provides an extensible, testable, and powerful framework for building and managing complex calculations.
 
 **efficalc** is designed to transform how engineers approach calculations, moving away from traditional methods like manual spreadsheets and toward a more efficient, accurate, and collaborative engineering calculation process.
 
-![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
-
-![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
+### Simple syntax for Python calculations:
 
+![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
 
-## Links
-
-- [Read the full documentation](https://youandvern.github.io/efficalc) 
-- [See more examples](https://github.com/youandvern/efficalc/tree/main/examples)
-- [The PyPI distribution](https://pypi.org/project/efficalc/)
+### Turns into submittal-ready reports:
 
+![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
 
 
-## Features
+## Examples
 
+- [Simple Examples](https://github.com/youandvern/efficalc/tree/main/examples/simple)
+- [More Advanced Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
 
-#### Automated report generation
-Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+## Documentation and Distribution
 
-#### Open source
-efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+- [Full documentation](https://youandvern.github.io/efficalc)
+- [PyPI distribution](https://pypi.org/project/efficalc/)
 
-#### Engineering-specific features
-Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
 
-#### Reusable
-Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
-
-#### Testable
-Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
-
-#### Integrate with other workflows
-Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
-
-#### Figures now supported
-Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
-
-#### Control your content
-Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
 
-## Quickstart
+# Quickstart
 
 ### Installation
 
 Install efficalc with pip:
 
 ```bash
 pip install efficalc
@@ -135,43 +116,71 @@
 builder = ReportBuilder(calculation)
 builder.view_report()
 ```
 
 ![The resulting calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/pythagorean_default.png)
 
 
-### Update Input Values
+### Updating Input Values
 
-The value proved to the `Input` class in your calculation function is treated as a default value. 
+The value provided to the `Input` class in your calculation function is treated as a default value. 
 
-If you want to change any of your input values, pass in a dictionary of the default overrides as an optional second parameter to the `ReportBuilder`:
+When you run your calculation with different input values, pass in a dictionary of the default overrides into the optional second parameter of the `ReportBuilder`:
 
 
 ```python
 new_inputs = {"a": 9.2, "b": 0.87}
 builder = ReportBuilder(calculation, new_inputs)
 builder.view_report()
 ```
 
-## Contributing
+
+# Features
+
+
+#### Automated report generation
+Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+
+#### Open source
+efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+
+#### Engineering-specific features
+Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
+
+#### Reusable
+Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
+
+#### Testable
+Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
+
+#### Integrate with other workflows
+Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
+
+#### Figures now supported
+Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
+
+#### Control your content
+Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
+
+# Contributing
 
 We welcome contributions of all kinds from the community! Whether it's reporting a bug, requesting a feature, or submitting a pull request, your input and engagement is invaluable to efficalc's development.
 
 - Report issues [here](https://github.com/youandvern/efficalc/issues).
 - Submit pull requests [here](https://github.com/youandvern/efficalc/pulls).
 
-## Built With
+# Built With
 
 * [latexexpr](https://github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/youandvern/latexexpr_efficalc)
 * [pylatexenc](https://github.com/phfaist/pylatexenc)
 
 #### Documentation
 
 * [sphinx](https://www.sphinx-doc.org/en/master/)
 * [furo](https://github.com/pradyunsg/furo/)
 * [sphinx-copybutton](https://github.com/executablebooks/sphinx-copybutton)
 * [sphinxcontrib-video](https://github.com/sphinx-contrib/video)
 
-## License
+# License
 
 efficalc is released under the [MIT License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,85 +1,90 @@
-Metadata-Version: 2.1 Name: efficalc Version: 1.1.0 Summary: Feature-rich open
+Metadata-Version: 2.1 Name: efficalc Version: 1.2.0 Summary: Feature-rich open
 source library for building well-formatted and extensible engineering
 calculations. Author-email: Andrew Young
 gmail.com> Project-URL: Homepage, https://github.com/youandvern/efficalc
 Project-URL: Documentation, https://youandvern.github.io/efficalc Project-URL:
 Issues, https://github.com/youandvern/efficalc/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 latexexpr_efficalc>=0.5.3 Requires-Dist: pylatexenc>=2.10 Requires-Dist:
 pytest>=8.0.2
                                     [Logo]
         _[_T_e_s_t_s_]    _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]    _[_L_i_c_e_n_s_e_:_ _M_I_T_]   _[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # efficalc ### A feature-rich Python library for reimagined engineering
-calculations. Table of Contents
-   1. _I_n_t_r_o_d_u_c_t_i_o_n
-   2. _L_i_n_k_s
-   3. _F_e_a_t_u_r_e_s
-   4. _Q_u_i_c_k_s_t_a_r_t
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _B_u_i_l_t_ _W_i_t_h
-   7. _L_i_c_e_n_s_e
-## Introduction ##### efficalc provides an extensible, testable, and powerful
+calculations. CCoonntteennttss
+    * _I_n_t_r_o_d_u_c_t_i_o_n
+          o _E_x_a_m_p_l_e_s
+          o _D_o_c_u_m_e_n_t_a_t_i_o_n
+    * _Q_u_i_c_k_s_t_a_r_t
+          o _I_n_s_t_a_l_l_a_t_i_o_n
+          o _F_i_r_s_t_ _C_a_l_c_u_l_a_t_i_o_n
+          o _V_i_e_w_ _R_e_p_o_r_t
+    * _F_e_a_t_u_r_e_s
+# Introduction ##### efficalc provides an extensible, testable, and powerful
 framework for building and managing complex calculations. **efficalc** is
 designed to transform how engineers approach calculations, moving away from
 traditional methods like manual spreadsheets and toward a more efficient,
-accurate, and collaborative engineering calculation process. ![Efficalc Demo
-Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo_typing.jpg?raw=true) ![Efficalc Demo Report](https://
-github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo2.png?raw=true) ## Links - [Read the full documentation]
-(https://youandvern.github.io/efficalc) - [See more examples](https://
-github.com/youandvern/efficalc/tree/main/examples) - [The PyPI distribution]
-(https://pypi.org/project/efficalc/) ## Features #### Automated report
-generation Generate detailed, professional reports automatically, ensuring
-clarity and precision in communication. #### Open source efficalc welcomes
-community contributions. Request features or contribute directly to enhance its
-capabilities. #### Engineering-specific features Benefit from built-in tools
-tailored to solving common engineering challenges. [See our section property
-library in action](https://github.com/youandvern/efficalc/blob/main/examples/
-advanced/steel_beam_moment_strength.py#L53). #### Reusable Create calculation
-templates once and reuse them across multiple designs and projects, saving time
-and ensuring consistency. #### Testable Easily test your calculations to reduce
+accurate, and collaborative engineering calculation process. ### Simple syntax
+for Python calculations: ![Efficalc Demo Typing](https://github.com/youandvern/
+efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true) ###
+Turns into submittal-ready reports: ![Efficalc Demo Report](https://github.com/
+youandvern/efficalc/raw/main/docs_src/_static/
+efficalc_basic_demo2.png?raw=true) ## Examples - [Simple Examples](https://
+github.com/youandvern/efficalc/tree/main/examples/simple) - [More Advanced
+Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
+## Documentation and Distribution - [Full documentation](https://
+youandvern.github.io/efficalc) - [PyPI distribution](https://pypi.org/project/
+efficalc/) # Quickstart ### Installation Install efficalc with pip: ```bash pip
+install efficalc ``` ### First Calculation Function Calculations in efficalc
+are written as a function. These calculation functions are primarily composed
+of `Input` and `Calculation` elements, but there are also many more options to
+make a clear and accurate calculation. ```python from efficalc import
+Calculation, Input, Title, sqrt def calculation(): Title("Pythagorean's Theorem
+and Perimeter") a = Input("a", 3, description="Length of side a") b = Input
+("b", 4, description="Length of side b") c = Calculation("c", sqrt(a**2 +
+b**2), description="Length of the hypotenuse") Calculation("P", a + b + c,
+description="Perimeter of the triangle") ``` ### View the Report Instantly view
+or print a report for your calculation in your browser with the
+`ReportBuilder`. ```python from efficalc.report_builder import ReportBuilder
+from pythagorean_perimeter import calculation builder = ReportBuilder
+(calculation) builder.view_report() ``` ![The resulting calculation report]
+(https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
+pythagorean_default.png) ### Updating Input Values The value provided to the
+`Input` class in your calculation function is treated as a default value. When
+you run your calculation with different input values, pass in a dictionary of
+the default overrides into the optional second parameter of the
+`ReportBuilder`: ```python new_inputs = {"a": 9.2, "b": 0.87} builder =
+ReportBuilder(calculation, new_inputs) builder.view_report() ``` # Features
+#### Automated report generation Generate detailed, professional reports
+automatically, ensuring clarity and precision in communication. #### Open
+source efficalc welcomes community contributions. Request features or
+contribute directly to enhance its capabilities. #### Engineering-specific
+features Benefit from built-in tools tailored to solving common engineering
+challenges. [See our section property library in action](https://github.com/
+youandvern/efficalc/blob/main/examples/advanced/
+steel_beam_moment_strength.py#L53). #### Reusable Create calculation templates
+once and reuse them across multiple designs and projects, saving time and
+ensuring consistency. #### Testable Easily test your calculations to reduce
 errors and improve confidence every design. [Read the testing guide.](https://
 youandvern.github.io/efficalc/testing.html) #### Integrate with other workflows
 Seamlessly integrate with your existing Python-enabled workflows to boost
 efficiency and connectivity across tools and platforms. [See some examples of
 this.](https://youandvern.github.io/efficalc/integration.html) #### Figures now
 supported Easily add figures to your calculation reports for even more clarity.
 [Read the full documentation for figures.](https://youandvern.github.io/
 efficalc/figures.html) #### Control your content Tailor your calculation
 reports to include only the most relevant information, making them as concise
-or detailed as you prefer. ## Quickstart ### Installation Install efficalc with
-pip: ```bash pip install efficalc ``` ### First Calculation Function
-Calculations in efficalc are written as a function. These calculation functions
-are primarily composed of `Input` and `Calculation` elements, but there are
-also many more options to make a clear and accurate calculation. ```python from
-efficalc import Calculation, Input, Title, sqrt def calculation(): Title
-("Pythagorean's Theorem and Perimeter") a = Input("a", 3, description="Length
-of side a") b = Input("b", 4, description="Length of side b") c = Calculation
-("c", sqrt(a**2 + b**2), description="Length of the hypotenuse") Calculation
-("P", a + b + c, description="Perimeter of the triangle") ``` ### View the
-Report Instantly view or print a report for your calculation in your browser
-with the `ReportBuilder`. ```python from efficalc.report_builder import
-ReportBuilder from pythagorean_perimeter import calculation builder =
-ReportBuilder(calculation) builder.view_report() ``` ![The resulting
-calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/
-_static/pythagorean_default.png) ### Update Input Values The value proved to
-the `Input` class in your calculation function is treated as a default value.
-If you want to change any of your input values, pass in a dictionary of the
-default overrides as an optional second parameter to the `ReportBuilder`:
-```python new_inputs = {"a": 9.2, "b": 0.87} builder = ReportBuilder
-(calculation, new_inputs) builder.view_report() ``` ## Contributing We welcome
-contributions of all kinds from the community! Whether it's reporting a bug,
-requesting a feature, or submitting a pull request, your input and engagement
-is invaluable to efficalc's development. - Report issues [here](https://
-github.com/youandvern/efficalc/issues). - Submit pull requests [here](https://
-github.com/youandvern/efficalc/pulls). ## Built With * [latexexpr](https://
-github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/
-youandvern/latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/
-pylatexenc) #### Documentation * [sphinx](https://www.sphinx-doc.org/en/master/
-) * [furo](https://github.com/pradyunsg/furo/) * [sphinx-copybutton](https://
-github.com/executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://
-github.com/sphinx-contrib/video) ## License efficalc is released under the [MIT
-License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
+or detailed as you prefer. # Contributing We welcome contributions of all kinds
+from the community! Whether it's reporting a bug, requesting a feature, or
+submitting a pull request, your input and engagement is invaluable to
+efficalc's development. - Report issues [here](https://github.com/youandvern/
+efficalc/issues). - Submit pull requests [here](https://github.com/youandvern/
+efficalc/pulls). # Built With * [latexexpr](https://github.com/kajusK/
+latexexpr) - [we use a forked version](https://github.com/youandvern/
+latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/pylatexenc) ####
+Documentation * [sphinx](https://www.sphinx-doc.org/en/master/) * [furo](https:
+//github.com/pradyunsg/furo/) * [sphinx-copybutton](https://github.com/
+executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://github.com/
+sphinx-contrib/video) # License efficalc is released under the [MIT License]
+(https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

### Comparing `efficalc-1.1.0/README.md` & `efficalc-1.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,67 @@
 <p align="center">
   <img src="https://github.com/youandvern/efficalc/raw/main/docs_src/efficalc.png" alt="Logo" width="200"/>
 </p>
 
 <p align="center">
   <a href="https://github.com/youandvern/efficalc/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/youandvern/efficalc/actions/workflows/tests.yml/badge.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.1.0"></a>&nbsp;&nbsp;&nbsp;
+  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.2.0"></a>&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/youandvern/efficalc/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.1.0"></a>
+  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.2.0"></a>
 </p>
 
 
 # efficalc
 
 ### A feature-rich Python library for reimagined engineering calculations.
 
 <!-- TABLE OF CONTENTS -->
 <details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li><a href="#introduction">Introduction</a></li>
-    <li><a href="#links">Links</a></li>
+  <summary style="font-size:1.5rem;"><b>Contents</b></summary>
+  <ul>
+    <li><a href="#introduction">Introduction</a><ul>
+        <li><a href="#examples">Examples</a></li>
+        <li><a href="#documentation-and-distribution">Documentation</a></li></ul></li>
+    <li><a href="#quickstart">Quickstart</a><ul>
+        <li><a href="#installation">Installation</a></li>
+        <li><a href="#first-calculation-function">First Calculation</a></li>
+        <li><a href="#view-the-report">View Report</a></li></ul></li>
     <li><a href="#features">Features</a></li>
-    <li><a href="#quickstart">Quickstart</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#built-with">Built With</a></li>
-    <li><a href="#license">License</a></li>
-  </ol>
+  </ul>
 </details>
 
 
-
-## Introduction
+# Introduction
 
 ##### efficalc provides an extensible, testable, and powerful framework for building and managing complex calculations.
 
 **efficalc** is designed to transform how engineers approach calculations, moving away from traditional methods like manual spreadsheets and toward a more efficient, accurate, and collaborative engineering calculation process.
 
-![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
-
-![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
+### Simple syntax for Python calculations:
 
+![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
 
-## Links
-
-- [Read the full documentation](https://youandvern.github.io/efficalc) 
-- [See more examples](https://github.com/youandvern/efficalc/tree/main/examples)
-- [The PyPI distribution](https://pypi.org/project/efficalc/)
+### Turns into submittal-ready reports:
 
+![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
 
 
-## Features
+## Examples
 
+- [Simple Examples](https://github.com/youandvern/efficalc/tree/main/examples/simple)
+- [More Advanced Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
 
-#### Automated report generation
-Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+## Documentation and Distribution
 
-#### Open source
-efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+- [Full documentation](https://youandvern.github.io/efficalc)
+- [PyPI distribution](https://pypi.org/project/efficalc/)
 
-#### Engineering-specific features
-Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
 
-#### Reusable
-Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
-
-#### Testable
-Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
-
-#### Integrate with other workflows
-Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
-
-#### Figures now supported
-Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
-
-#### Control your content
-Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
 
-## Quickstart
+# Quickstart
 
 ### Installation
 
 Install efficalc with pip:
 
 ```bash
 pip install efficalc
@@ -117,43 +98,71 @@
 builder = ReportBuilder(calculation)
 builder.view_report()
 ```
 
 ![The resulting calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/pythagorean_default.png)
 
 
-### Update Input Values
+### Updating Input Values
 
-The value proved to the `Input` class in your calculation function is treated as a default value. 
+The value provided to the `Input` class in your calculation function is treated as a default value. 
 
-If you want to change any of your input values, pass in a dictionary of the default overrides as an optional second parameter to the `ReportBuilder`:
+When you run your calculation with different input values, pass in a dictionary of the default overrides into the optional second parameter of the `ReportBuilder`:
 
 
 ```python
 new_inputs = {"a": 9.2, "b": 0.87}
 builder = ReportBuilder(calculation, new_inputs)
 builder.view_report()
 ```
 
-## Contributing
+
+# Features
+
+
+#### Automated report generation
+Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+
+#### Open source
+efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+
+#### Engineering-specific features
+Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
+
+#### Reusable
+Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
+
+#### Testable
+Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
+
+#### Integrate with other workflows
+Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
+
+#### Figures now supported
+Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
+
+#### Control your content
+Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
+
+# Contributing
 
 We welcome contributions of all kinds from the community! Whether it's reporting a bug, requesting a feature, or submitting a pull request, your input and engagement is invaluable to efficalc's development.
 
 - Report issues [here](https://github.com/youandvern/efficalc/issues).
 - Submit pull requests [here](https://github.com/youandvern/efficalc/pulls).
 
-## Built With
+# Built With
 
 * [latexexpr](https://github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/youandvern/latexexpr_efficalc)
 * [pylatexenc](https://github.com/phfaist/pylatexenc)
 
 #### Documentation
 
 * [sphinx](https://www.sphinx-doc.org/en/master/)
 * [furo](https://github.com/pradyunsg/furo/)
 * [sphinx-copybutton](https://github.com/executablebooks/sphinx-copybutton)
 * [sphinxcontrib-video](https://github.com/sphinx-contrib/video)
 
-## License
+# License
 
 efficalc is released under the [MIT License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,74 +1,79 @@
                                     [Logo]
         _[_T_e_s_t_s_]    _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]    _[_L_i_c_e_n_s_e_:_ _M_I_T_]   _[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # efficalc ### A feature-rich Python library for reimagined engineering
-calculations. Table of Contents
-   1. _I_n_t_r_o_d_u_c_t_i_o_n
-   2. _L_i_n_k_s
-   3. _F_e_a_t_u_r_e_s
-   4. _Q_u_i_c_k_s_t_a_r_t
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _B_u_i_l_t_ _W_i_t_h
-   7. _L_i_c_e_n_s_e
-## Introduction ##### efficalc provides an extensible, testable, and powerful
+calculations. CCoonntteennttss
+    * _I_n_t_r_o_d_u_c_t_i_o_n
+          o _E_x_a_m_p_l_e_s
+          o _D_o_c_u_m_e_n_t_a_t_i_o_n
+    * _Q_u_i_c_k_s_t_a_r_t
+          o _I_n_s_t_a_l_l_a_t_i_o_n
+          o _F_i_r_s_t_ _C_a_l_c_u_l_a_t_i_o_n
+          o _V_i_e_w_ _R_e_p_o_r_t
+    * _F_e_a_t_u_r_e_s
+# Introduction ##### efficalc provides an extensible, testable, and powerful
 framework for building and managing complex calculations. **efficalc** is
 designed to transform how engineers approach calculations, moving away from
 traditional methods like manual spreadsheets and toward a more efficient,
-accurate, and collaborative engineering calculation process. ![Efficalc Demo
-Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo_typing.jpg?raw=true) ![Efficalc Demo Report](https://
-github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo2.png?raw=true) ## Links - [Read the full documentation]
-(https://youandvern.github.io/efficalc) - [See more examples](https://
-github.com/youandvern/efficalc/tree/main/examples) - [The PyPI distribution]
-(https://pypi.org/project/efficalc/) ## Features #### Automated report
-generation Generate detailed, professional reports automatically, ensuring
-clarity and precision in communication. #### Open source efficalc welcomes
-community contributions. Request features or contribute directly to enhance its
-capabilities. #### Engineering-specific features Benefit from built-in tools
-tailored to solving common engineering challenges. [See our section property
-library in action](https://github.com/youandvern/efficalc/blob/main/examples/
-advanced/steel_beam_moment_strength.py#L53). #### Reusable Create calculation
-templates once and reuse them across multiple designs and projects, saving time
-and ensuring consistency. #### Testable Easily test your calculations to reduce
+accurate, and collaborative engineering calculation process. ### Simple syntax
+for Python calculations: ![Efficalc Demo Typing](https://github.com/youandvern/
+efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true) ###
+Turns into submittal-ready reports: ![Efficalc Demo Report](https://github.com/
+youandvern/efficalc/raw/main/docs_src/_static/
+efficalc_basic_demo2.png?raw=true) ## Examples - [Simple Examples](https://
+github.com/youandvern/efficalc/tree/main/examples/simple) - [More Advanced
+Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
+## Documentation and Distribution - [Full documentation](https://
+youandvern.github.io/efficalc) - [PyPI distribution](https://pypi.org/project/
+efficalc/) # Quickstart ### Installation Install efficalc with pip: ```bash pip
+install efficalc ``` ### First Calculation Function Calculations in efficalc
+are written as a function. These calculation functions are primarily composed
+of `Input` and `Calculation` elements, but there are also many more options to
+make a clear and accurate calculation. ```python from efficalc import
+Calculation, Input, Title, sqrt def calculation(): Title("Pythagorean's Theorem
+and Perimeter") a = Input("a", 3, description="Length of side a") b = Input
+("b", 4, description="Length of side b") c = Calculation("c", sqrt(a**2 +
+b**2), description="Length of the hypotenuse") Calculation("P", a + b + c,
+description="Perimeter of the triangle") ``` ### View the Report Instantly view
+or print a report for your calculation in your browser with the
+`ReportBuilder`. ```python from efficalc.report_builder import ReportBuilder
+from pythagorean_perimeter import calculation builder = ReportBuilder
+(calculation) builder.view_report() ``` ![The resulting calculation report]
+(https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
+pythagorean_default.png) ### Updating Input Values The value provided to the
+`Input` class in your calculation function is treated as a default value. When
+you run your calculation with different input values, pass in a dictionary of
+the default overrides into the optional second parameter of the
+`ReportBuilder`: ```python new_inputs = {"a": 9.2, "b": 0.87} builder =
+ReportBuilder(calculation, new_inputs) builder.view_report() ``` # Features
+#### Automated report generation Generate detailed, professional reports
+automatically, ensuring clarity and precision in communication. #### Open
+source efficalc welcomes community contributions. Request features or
+contribute directly to enhance its capabilities. #### Engineering-specific
+features Benefit from built-in tools tailored to solving common engineering
+challenges. [See our section property library in action](https://github.com/
+youandvern/efficalc/blob/main/examples/advanced/
+steel_beam_moment_strength.py#L53). #### Reusable Create calculation templates
+once and reuse them across multiple designs and projects, saving time and
+ensuring consistency. #### Testable Easily test your calculations to reduce
 errors and improve confidence every design. [Read the testing guide.](https://
 youandvern.github.io/efficalc/testing.html) #### Integrate with other workflows
 Seamlessly integrate with your existing Python-enabled workflows to boost
 efficiency and connectivity across tools and platforms. [See some examples of
 this.](https://youandvern.github.io/efficalc/integration.html) #### Figures now
 supported Easily add figures to your calculation reports for even more clarity.
 [Read the full documentation for figures.](https://youandvern.github.io/
 efficalc/figures.html) #### Control your content Tailor your calculation
 reports to include only the most relevant information, making them as concise
-or detailed as you prefer. ## Quickstart ### Installation Install efficalc with
-pip: ```bash pip install efficalc ``` ### First Calculation Function
-Calculations in efficalc are written as a function. These calculation functions
-are primarily composed of `Input` and `Calculation` elements, but there are
-also many more options to make a clear and accurate calculation. ```python from
-efficalc import Calculation, Input, Title, sqrt def calculation(): Title
-("Pythagorean's Theorem and Perimeter") a = Input("a", 3, description="Length
-of side a") b = Input("b", 4, description="Length of side b") c = Calculation
-("c", sqrt(a**2 + b**2), description="Length of the hypotenuse") Calculation
-("P", a + b + c, description="Perimeter of the triangle") ``` ### View the
-Report Instantly view or print a report for your calculation in your browser
-with the `ReportBuilder`. ```python from efficalc.report_builder import
-ReportBuilder from pythagorean_perimeter import calculation builder =
-ReportBuilder(calculation) builder.view_report() ``` ![The resulting
-calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/
-_static/pythagorean_default.png) ### Update Input Values The value proved to
-the `Input` class in your calculation function is treated as a default value.
-If you want to change any of your input values, pass in a dictionary of the
-default overrides as an optional second parameter to the `ReportBuilder`:
-```python new_inputs = {"a": 9.2, "b": 0.87} builder = ReportBuilder
-(calculation, new_inputs) builder.view_report() ``` ## Contributing We welcome
-contributions of all kinds from the community! Whether it's reporting a bug,
-requesting a feature, or submitting a pull request, your input and engagement
-is invaluable to efficalc's development. - Report issues [here](https://
-github.com/youandvern/efficalc/issues). - Submit pull requests [here](https://
-github.com/youandvern/efficalc/pulls). ## Built With * [latexexpr](https://
-github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/
-youandvern/latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/
-pylatexenc) #### Documentation * [sphinx](https://www.sphinx-doc.org/en/master/
-) * [furo](https://github.com/pradyunsg/furo/) * [sphinx-copybutton](https://
-github.com/executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://
-github.com/sphinx-contrib/video) ## License efficalc is released under the [MIT
-License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
+or detailed as you prefer. # Contributing We welcome contributions of all kinds
+from the community! Whether it's reporting a bug, requesting a feature, or
+submitting a pull request, your input and engagement is invaluable to
+efficalc's development. - Report issues [here](https://github.com/youandvern/
+efficalc/issues). - Submit pull requests [here](https://github.com/youandvern/
+efficalc/pulls). # Built With * [latexexpr](https://github.com/kajusK/
+latexexpr) - [we use a forked version](https://github.com/youandvern/
+latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/pylatexenc) ####
+Documentation * [sphinx](https://www.sphinx-doc.org/en/master/) * [furo](https:
+//github.com/pradyunsg/furo/) * [sphinx-copybutton](https://github.com/
+executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://github.com/
+sphinx-contrib/video) # License efficalc is released under the [MIT License]
+(https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

### Comparing `efficalc-1.1.0/efficalc/__init__.py` & `efficalc-1.2.0/efficalc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,26 +35,27 @@
 
 from .base_definitions.assumption import Assumption
 from .base_definitions.calculation import Calculation, CalculationLength
 from .base_definitions.comparison import Comparison
 from .base_definitions.comparison_statement import ComparisonStatement
 from .base_definitions.figure import (
     FigureBase,
+    FigureFromBytes,
     FigureFromFile,
     FigureFromMatplotlib,
-    FigureFromBytes,
 )
 from .base_definitions.heading import Heading
 from .base_definitions.input import Input
 from .base_definitions.shared import (
     CalculationItem,
     clear_all_input_default_overrides,
     clear_saved_objects,
     get_all_calc_objects,
     get_override_or_default_value,
     save_calculation_item,
     set_input_default_overrides,
 )
+from .base_definitions.symbolic import Symbolic
 from .base_definitions.text_block import TextBlock
 from .base_definitions.title import Title
 from .constants import ONE, PI, TWO, ZERO, E
 from .unit_conversions import deg_to_rad, ft_to_in, k_to_lb
```

### Comparing `efficalc-1.1.0/efficalc/base_definitions/assumption.py` & `efficalc-1.2.0/efficalc/base_definitions/assumption.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/base_definitions/calculation.py` & `efficalc-1.2.0/efficalc/base_definitions/calculation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from enum import Enum
 
 from latexexpr_efficalc import Expression, Operation, Variable
 from pylatexenc.latex2text import LatexNodes2Text
 
 from .input import Input
-from .shared import CalculationItem, _get_float_safe_operation, save_calculation_item
+from .shared import (
+    CalculationItem,
+    _get_float_or_str_safe_operation,
+    save_calculation_item,
+)
 
 
 class CalculationLength(Enum):
     """Used to indicate the length of a calculation's LaTex formatted operation."""
 
     NUMBER = "number"
     SHORT = "short"
@@ -26,15 +30,15 @@
     :type unit: str, optional
     :param description: A text description for the calculation, defaults to None
     :type description: str, optional
     :param reference: A short reference (e.g. code reference) to accompany the calculation, defaults to None
     :type reference: str, optional
     :param result_check: This is used to indicate any :class:`.Calculation` that should be checked as a final result
         of your calculation template. When set to True, this :class:`.Calculation` will be displayed in the "Results"
-        section of your design portal in the hosted version of efficalc, defaults to False
+        section of your design portal in the cloud version of efficalc, defaults to False
     :type result_check: bool, optional
 
     .. code-block:: python
 
         >>> a = Input("a",1,'ft')
         >>> b = Input('b',4,'ft')
         >>> c = Calculation('c', a + b, 'ft')
@@ -49,15 +53,17 @@
         description: str = None,
         reference: str = None,
         result_check: bool = False,
     ):
 
         if unit is None:
             unit = ""
-        super().__init__(variable_name, _get_float_safe_operation(expression), unit)
+        super().__init__(
+            variable_name, _get_float_or_str_safe_operation(expression), unit
+        )
         self.description: str = description
         self.reference: str = reference
         self.result_check: bool = result_check
         self.error: str | None = None
         save_calculation_item(self)
 
     def str_result_with_description(self) -> str:
```

### Comparing `efficalc-1.1.0/efficalc/base_definitions/comparison.py` & `efficalc-1.2.0/efficalc/base_definitions/comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :type false_message: str, optional
     :param description: A text description for the comparison, defaults to None
     :type description: str, optional
     :param reference: A short text reference (e.g. code reference) to accompany the comparison, defaults to None
     :type reference: str, optional
     :param result_check: This is used to indicate any :class:`.Comparison` that should be checked as a final result
         of your calculation template. When set to True, this :class:`.Comparison` will be displayed in the "Results"
-        section of your design portal in the hosted version of efficalc, defaults to False
+        section of your design portal in the cloud version of efficalc, defaults to False
     :type result_check: bool, optional
 
     .. code-block:: python
 
         >>> a = Input("a",1,'ft')
         >>> b = Input('b',4,'ft')
         >>> Comparison(a, '>', b)
```

### Comparing `efficalc-1.1.0/efficalc/base_definitions/comparison_statement.py` & `efficalc-1.2.0/efficalc/base_definitions/comparison_statement.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/base_definitions/figure.py` & `efficalc-1.2.0/efficalc/base_definitions/figure.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/base_definitions/heading.py` & `efficalc-1.2.0/efficalc/base_definitions/heading.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/base_definitions/input.py` & `efficalc-1.2.0/efficalc/base_definitions/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,36 +20,36 @@
 class Input(Variable, CalculationItem):
     """This is the primary object used to define an input which can change from calculation to calculation. Inputs may
     be numbers, text, or select elements with multiple options.
 
     :param variable_name: The symbolic name for this input variable (LaTex formatted)
     :type variable_name: str
     :param default_value: The default value for the input. This will be overridden when explicit calculation inputs are
-        provided to the calculation runner or in the design portal on the hosted version of efficalc, defaults to 0
+        provided to the calculation runner or in the design portal on the cloud version of efficalc, defaults to 0
     :type default_value: float, int, or str
     :param unit: The physical units of the input variable (LaTex formatted), defaults to None
     :type unit: str, optional
     :param description: A text description for the input variable, defaults to None
     :type description: str, optional
     :param reference: A short text reference (e.g. code reference) to accompany the input, defaults to None
     :type reference: str, optional
-    :param input_type: The type of html input element to use in the design portal on the hosted version of efficalc,
+    :param input_type: The type of html input element to use in the design portal on the cloud version of efficalc,
         defaults to "number".
     :type input_type: "number", "text", or "select", optional
     :param select_options: A list of options for a "select" input_type variable. This is only applicable when
         `.input_type` is "select", defaults to None
     :type select_options: str[], float[], or int[], optional
-    :param min_value: Set the minimum value a number input is allowed to be in the design portal on the hosted version
+    :param min_value: Set the minimum value a number input is allowed to be in the design portal on the cloud version
         of efficalc, defaults to None
     :type min_value: float, int, or None, optional
-    :param max_value: Set the maximum value a number input is allowed to be in the design portal on the hosted version
-        of efficalc, or "any" if the input type is not a number in the design portal on the hosted version of efficalc, defaults to None
+    :param max_value: Set the maximum value a number input is allowed to be in the design portal on the cloud version
+        of efficalc, or "any" if the input type is not a number in the design portal on the cloud version of efficalc, defaults to None
     :type max_value: float, int, or None, optional
     :param num_step: Specifies the interval between legal numbers in a number input field in the design portal on the
-        hosted version of efficalc; see
+        cloud version of efficalc; see
         https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/step, defaults to "any"
     :type num_step: float, int, or None, optional
 
     .. code-block:: python
 
         >>> a = Input("a",1,'ft')
         >>> b = Input("b",4,'ft')
@@ -93,15 +93,15 @@
             self.name,
             self.str_result(),
             self.unit_format % self.unit,
         )
 
     def get_value(self):
         """Returns the value of the input. Note that this will return the overridden input value when one is provided
-        to the calculation runner or in the design portal on the hosted version of efficalc. If no override is provided,
+        to the calculation runner or in the design portal on the cloud version of efficalc. If no override is provided,
         this will return the default value.
 
         :return: The current value of the input variable
         :rtype: float, int, or str
 
         .. code-block:: python
```

### Comparing `efficalc-1.1.0/efficalc/base_definitions/shared.py` & `efficalc-1.2.0/efficalc/base_definitions/shared.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,14 +65,16 @@
 
 
 def clear_all_input_default_overrides():
     """Clear all input default overrides from the global store."""
     _get_thread_local_store()[_DEFAULT_OVERRIDE_KEY] = {}
 
 
-def _get_float_safe_operation(
-    input_operation: Operation | Expression | Variable | float | int,
+def _get_float_or_str_safe_operation(
+    input_operation: Operation | Expression | Variable | float | int | str,
 ):
     if isinstance(input_operation, (float, int)):
         return Operation("", input_operation)
+    elif isinstance(input_operation, str):
+        return Variable(input_operation, input_operation)
     else:
         return input_operation
```

### Comparing `efficalc-1.1.0/efficalc/base_definitions/text_block.py` & `efficalc-1.2.0/efficalc/base_definitions/text_block.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/calculation_runner.py` & `efficalc-1.2.0/efficalc/calculation_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from efficalc import (
     Calculation,
     Comparison,
     clear_all_input_default_overrides,
     clear_saved_objects,
     get_all_calc_objects,
     set_input_default_overrides,
+    Symbolic,
 )
 
 ResultType = Union[Calculation, Comparison]
 
 
 class CalculationRunner(object):
     """A helper class for running calculation functions. It executes the provided calculation function and returns the
@@ -81,10 +82,14 @@
                 if self._is_calculated_result(item)
             }
         else:
             raise ValueError("Invalid return_type specified. Use 'list' or 'dict'.")
 
     @staticmethod
     def _is_calculated_result(ob) -> bool:
-        if not isinstance(ob, Calculation) and not isinstance(ob, Comparison):
+        if (
+            not isinstance(ob, Calculation)
+            and not isinstance(ob, Comparison)
+            and not isinstance(ob, Symbolic)
+        ):
             return False
         return ob.result_check
```

### Comparing `efficalc-1.1.0/efficalc/constants.py` & `efficalc-1.2.0/efficalc/constants.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/generate_html.py` & `efficalc-1.2.0/efficalc/generate_html.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     Calculation,
     CalculationLength,
     Comparison,
     ComparisonStatement,
     FigureBase,
     Heading,
     Input,
+    Symbolic,
     TextBlock,
     Title,
 )
 
 CALC_MARGIN = "margin-left: 2rem;"
 ALIGN = "&"
 LINE_BREAK = r"\\[4pt]"
@@ -72,14 +73,17 @@
         heading_size = min(4, max(1, calculation_item.head_level) + 1)
 
         return _wrap_h(text, heading_size)
 
     elif isinstance(calculation_item, Input):
         return _generate_input_html(calculation_item)
 
+    elif isinstance(calculation_item, Symbolic):
+        return _generate_symbolic_html(calculation_item)
+
     elif isinstance(calculation_item, TextBlock):
         return _wrap_with_reference(
             _wrap_p(_esc(calculation_item.text)), _esc(calculation_item.reference)
         )
 
     elif isinstance(calculation_item, Title):
         return _wrap_h(_esc(calculation_item.text), 1)
@@ -149,14 +153,35 @@
         )
 
     calc_html += _wrap_with_reference(_wrap_p(calc_tex), _esc(item.reference))
 
     return _wrap_div(calc_html, class_name=CALC_ITEM_WRAPPER_CLASS)
 
 
+def _generate_symbolic_html(item: Symbolic) -> str:
+    calc_html = ""
+
+    description = _esc(item.description)
+    if description is not None and description != "":
+        calc_html += _wrap_p(description, CALC_MARGIN)
+
+    if item.error is not None and item.error != "":
+        calc_html += _wrap_p(
+            f"<b>ERROR:</b>{_esc(item.error)}", f"color: red; {CALC_MARGIN}"
+        )
+
+    item_name = _esc(item.name)
+    str_symbolic = _esc(item.str_symbolic())
+
+    calc_tex = _wrap_math(f"{item_name} = {str_symbolic}")
+    calc_html += _wrap_with_reference(_wrap_p(calc_tex), _esc(item.reference))
+
+    return _wrap_div(calc_html, class_name=CALC_ITEM_WRAPPER_CLASS)
+
+
 def _generate_comparison_html(item: Comparison) -> str:
     comp_html = ""
     description = _esc(item.description)
 
     if description is not None and description != "":
         comp_html += _wrap_p(description, CALC_MARGIN)
```

### Comparing `efficalc-1.1.0/efficalc/report_builder.py` & `efficalc-1.2.0/efficalc/report_builder.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/__init__.py` & `efficalc-1.2.0/efficalc/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_angle.py` & `efficalc-1.2.0/efficalc/sections/aisc_angle.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_channel.py` & `efficalc-1.2.0/efficalc/sections/aisc_channel.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_circular.py` & `efficalc-1.2.0/efficalc/sections/aisc_circular.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_double_angle.py` & `efficalc-1.2.0/efficalc/sections/aisc_double_angle.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_rectangular.py` & `efficalc-1.2.0/efficalc/sections/aisc_rectangular.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_tee.py` & `efficalc-1.2.0/efficalc/sections/aisc_tee.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/aisc_wide_flange.py` & `efficalc-1.2.0/efficalc/sections/aisc_wide_flange.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/section_properties.db` & `efficalc-1.2.0/efficalc/sections/section_properties.db`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/sections/section_query.py` & `efficalc-1.2.0/efficalc/sections/section_query.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc/unit_conversions.py` & `efficalc-1.2.0/efficalc/unit_conversions.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/efficalc.egg-info/PKG-INFO` & `efficalc-1.2.0/efficalc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: efficalc
-Version: 1.1.0
+Version: 1.2.0
 Summary: Feature-rich open source library for building well-formatted and extensible engineering calculations.
 Author-email: Andrew Young <youandvern@gmail.com>
 Project-URL: Homepage, https://github.com/youandvern/efficalc
 Project-URL: Documentation, https://youandvern.github.io/efficalc
 Project-URL: Issues, https://github.com/youandvern/efficalc/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,87 +18,68 @@
 
 <p align="center">
   <img src="https://github.com/youandvern/efficalc/raw/main/docs_src/efficalc.png" alt="Logo" width="200"/>
 </p>
 
 <p align="center">
   <a href="https://github.com/youandvern/efficalc/actions/workflows/tests.yml"><img alt="Tests" src="https://github.com/youandvern/efficalc/actions/workflows/tests.yml/badge.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.1.0"></a>&nbsp;&nbsp;&nbsp;
+  <a href="https://coveralls.io/github/youandvern/efficalc?branch=main"><img alt="Coverage Status" src="https://coveralls.io/repos/github/youandvern/efficalc/badge.svg?branch=main&v=1.2.0"></a>&nbsp;&nbsp;&nbsp;
   <a href="https://github.com/youandvern/efficalc/blob/main/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/License-MIT-yellow.svg"></a>&nbsp;&nbsp;&nbsp;
-  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.1.0"></a>
+  <a href="https://badge.fury.io/py/efficalc"><img alt="PyPI version" src="https://badge.fury.io/py/efficalc.svg?version=1.2.0"></a>
 </p>
 
 
 # efficalc
 
 ### A feature-rich Python library for reimagined engineering calculations.
 
 <!-- TABLE OF CONTENTS -->
 <details>
-  <summary>Table of Contents</summary>
-  <ol>
-    <li><a href="#introduction">Introduction</a></li>
-    <li><a href="#links">Links</a></li>
+  <summary style="font-size:1.5rem;"><b>Contents</b></summary>
+  <ul>
+    <li><a href="#introduction">Introduction</a><ul>
+        <li><a href="#examples">Examples</a></li>
+        <li><a href="#documentation-and-distribution">Documentation</a></li></ul></li>
+    <li><a href="#quickstart">Quickstart</a><ul>
+        <li><a href="#installation">Installation</a></li>
+        <li><a href="#first-calculation-function">First Calculation</a></li>
+        <li><a href="#view-the-report">View Report</a></li></ul></li>
     <li><a href="#features">Features</a></li>
-    <li><a href="#quickstart">Quickstart</a></li>
-    <li><a href="#contributing">Contributing</a></li>
-    <li><a href="#built-with">Built With</a></li>
-    <li><a href="#license">License</a></li>
-  </ol>
+  </ul>
 </details>
 
 
-
-## Introduction
+# Introduction
 
 ##### efficalc provides an extensible, testable, and powerful framework for building and managing complex calculations.
 
 **efficalc** is designed to transform how engineers approach calculations, moving away from traditional methods like manual spreadsheets and toward a more efficient, accurate, and collaborative engineering calculation process.
 
-![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
-
-![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
+### Simple syntax for Python calculations:
 
+![Efficalc Demo Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true)
 
-## Links
-
-- [Read the full documentation](https://youandvern.github.io/efficalc) 
-- [See more examples](https://github.com/youandvern/efficalc/tree/main/examples)
-- [The PyPI distribution](https://pypi.org/project/efficalc/)
+### Turns into submittal-ready reports:
 
+![Efficalc Demo Report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/efficalc_basic_demo2.png?raw=true)
 
 
-## Features
+## Examples
 
+- [Simple Examples](https://github.com/youandvern/efficalc/tree/main/examples/simple)
+- [More Advanced Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
 
-#### Automated report generation
-Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+## Documentation and Distribution
 
-#### Open source
-efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+- [Full documentation](https://youandvern.github.io/efficalc)
+- [PyPI distribution](https://pypi.org/project/efficalc/)
 
-#### Engineering-specific features
-Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
 
-#### Reusable
-Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
-
-#### Testable
-Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
-
-#### Integrate with other workflows
-Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
-
-#### Figures now supported
-Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
-
-#### Control your content
-Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
 
-## Quickstart
+# Quickstart
 
 ### Installation
 
 Install efficalc with pip:
 
 ```bash
 pip install efficalc
@@ -135,43 +116,71 @@
 builder = ReportBuilder(calculation)
 builder.view_report()
 ```
 
 ![The resulting calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/pythagorean_default.png)
 
 
-### Update Input Values
+### Updating Input Values
 
-The value proved to the `Input` class in your calculation function is treated as a default value. 
+The value provided to the `Input` class in your calculation function is treated as a default value. 
 
-If you want to change any of your input values, pass in a dictionary of the default overrides as an optional second parameter to the `ReportBuilder`:
+When you run your calculation with different input values, pass in a dictionary of the default overrides into the optional second parameter of the `ReportBuilder`:
 
 
 ```python
 new_inputs = {"a": 9.2, "b": 0.87}
 builder = ReportBuilder(calculation, new_inputs)
 builder.view_report()
 ```
 
-## Contributing
+
+# Features
+
+
+#### Automated report generation
+Generate detailed, professional reports automatically, ensuring clarity and precision in communication.
+
+#### Open source
+efficalc welcomes community contributions. Request features or contribute directly to enhance its capabilities.
+
+#### Engineering-specific features
+Benefit from built-in tools tailored to solving common engineering challenges. [See our section property library in action](https://github.com/youandvern/efficalc/blob/main/examples/advanced/steel_beam_moment_strength.py#L53).
+
+#### Reusable
+Create calculation templates once and reuse them across multiple designs and projects, saving time and ensuring consistency.
+
+#### Testable
+Easily test your calculations to reduce errors and improve confidence every design. [Read the testing guide.](https://youandvern.github.io/efficalc/testing.html)
+
+#### Integrate with other workflows
+Seamlessly integrate with your existing Python-enabled workflows to boost efficiency and connectivity across tools and platforms. [See some examples of this.](https://youandvern.github.io/efficalc/integration.html)
+
+#### Figures now supported
+Easily add figures to your calculation reports for even more clarity. [Read the full documentation for figures.](https://youandvern.github.io/efficalc/figures.html)
+
+#### Control your content
+Tailor your calculation reports to include only the most relevant information, making them as concise or detailed as you prefer.
+
+# Contributing
 
 We welcome contributions of all kinds from the community! Whether it's reporting a bug, requesting a feature, or submitting a pull request, your input and engagement is invaluable to efficalc's development.
 
 - Report issues [here](https://github.com/youandvern/efficalc/issues).
 - Submit pull requests [here](https://github.com/youandvern/efficalc/pulls).
 
-## Built With
+# Built With
 
 * [latexexpr](https://github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/youandvern/latexexpr_efficalc)
 * [pylatexenc](https://github.com/phfaist/pylatexenc)
 
 #### Documentation
 
 * [sphinx](https://www.sphinx-doc.org/en/master/)
 * [furo](https://github.com/pradyunsg/furo/)
 * [sphinx-copybutton](https://github.com/executablebooks/sphinx-copybutton)
 * [sphinxcontrib-video](https://github.com/sphinx-contrib/video)
 
-## License
+# License
 
 efficalc is released under the [MIT License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

#### html2text {}

```diff
@@ -1,85 +1,90 @@
-Metadata-Version: 2.1 Name: efficalc Version: 1.1.0 Summary: Feature-rich open
+Metadata-Version: 2.1 Name: efficalc Version: 1.2.0 Summary: Feature-rich open
 source library for building well-formatted and extensible engineering
 calculations. Author-email: Andrew Young
 gmail.com> Project-URL: Homepage, https://github.com/youandvern/efficalc
 Project-URL: Documentation, https://youandvern.github.io/efficalc Project-URL:
 Issues, https://github.com/youandvern/efficalc/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 latexexpr_efficalc>=0.5.3 Requires-Dist: pylatexenc>=2.10 Requires-Dist:
 pytest>=8.0.2
                                     [Logo]
         _[_T_e_s_t_s_]    _[_C_o_v_e_r_a_g_e_ _S_t_a_t_u_s_]    _[_L_i_c_e_n_s_e_:_ _M_I_T_]   _[_P_y_P_I_ _v_e_r_s_i_o_n_]
 # efficalc ### A feature-rich Python library for reimagined engineering
-calculations. Table of Contents
-   1. _I_n_t_r_o_d_u_c_t_i_o_n
-   2. _L_i_n_k_s
-   3. _F_e_a_t_u_r_e_s
-   4. _Q_u_i_c_k_s_t_a_r_t
-   5. _C_o_n_t_r_i_b_u_t_i_n_g
-   6. _B_u_i_l_t_ _W_i_t_h
-   7. _L_i_c_e_n_s_e
-## Introduction ##### efficalc provides an extensible, testable, and powerful
+calculations. CCoonntteennttss
+    * _I_n_t_r_o_d_u_c_t_i_o_n
+          o _E_x_a_m_p_l_e_s
+          o _D_o_c_u_m_e_n_t_a_t_i_o_n
+    * _Q_u_i_c_k_s_t_a_r_t
+          o _I_n_s_t_a_l_l_a_t_i_o_n
+          o _F_i_r_s_t_ _C_a_l_c_u_l_a_t_i_o_n
+          o _V_i_e_w_ _R_e_p_o_r_t
+    * _F_e_a_t_u_r_e_s
+# Introduction ##### efficalc provides an extensible, testable, and powerful
 framework for building and managing complex calculations. **efficalc** is
 designed to transform how engineers approach calculations, moving away from
 traditional methods like manual spreadsheets and toward a more efficient,
-accurate, and collaborative engineering calculation process. ![Efficalc Demo
-Typing](https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo_typing.jpg?raw=true) ![Efficalc Demo Report](https://
-github.com/youandvern/efficalc/raw/main/docs_src/_static/
-efficalc_basic_demo2.png?raw=true) ## Links - [Read the full documentation]
-(https://youandvern.github.io/efficalc) - [See more examples](https://
-github.com/youandvern/efficalc/tree/main/examples) - [The PyPI distribution]
-(https://pypi.org/project/efficalc/) ## Features #### Automated report
-generation Generate detailed, professional reports automatically, ensuring
-clarity and precision in communication. #### Open source efficalc welcomes
-community contributions. Request features or contribute directly to enhance its
-capabilities. #### Engineering-specific features Benefit from built-in tools
-tailored to solving common engineering challenges. [See our section property
-library in action](https://github.com/youandvern/efficalc/blob/main/examples/
-advanced/steel_beam_moment_strength.py#L53). #### Reusable Create calculation
-templates once and reuse them across multiple designs and projects, saving time
-and ensuring consistency. #### Testable Easily test your calculations to reduce
+accurate, and collaborative engineering calculation process. ### Simple syntax
+for Python calculations: ![Efficalc Demo Typing](https://github.com/youandvern/
+efficalc/raw/main/docs_src/_static/efficalc_basic_demo_typing.jpg?raw=true) ###
+Turns into submittal-ready reports: ![Efficalc Demo Report](https://github.com/
+youandvern/efficalc/raw/main/docs_src/_static/
+efficalc_basic_demo2.png?raw=true) ## Examples - [Simple Examples](https://
+github.com/youandvern/efficalc/tree/main/examples/simple) - [More Advanced
+Examples](https://github.com/youandvern/efficalc/tree/main/examples/advanced)
+## Documentation and Distribution - [Full documentation](https://
+youandvern.github.io/efficalc) - [PyPI distribution](https://pypi.org/project/
+efficalc/) # Quickstart ### Installation Install efficalc with pip: ```bash pip
+install efficalc ``` ### First Calculation Function Calculations in efficalc
+are written as a function. These calculation functions are primarily composed
+of `Input` and `Calculation` elements, but there are also many more options to
+make a clear and accurate calculation. ```python from efficalc import
+Calculation, Input, Title, sqrt def calculation(): Title("Pythagorean's Theorem
+and Perimeter") a = Input("a", 3, description="Length of side a") b = Input
+("b", 4, description="Length of side b") c = Calculation("c", sqrt(a**2 +
+b**2), description="Length of the hypotenuse") Calculation("P", a + b + c,
+description="Perimeter of the triangle") ``` ### View the Report Instantly view
+or print a report for your calculation in your browser with the
+`ReportBuilder`. ```python from efficalc.report_builder import ReportBuilder
+from pythagorean_perimeter import calculation builder = ReportBuilder
+(calculation) builder.view_report() ``` ![The resulting calculation report]
+(https://github.com/youandvern/efficalc/raw/main/docs_src/_static/
+pythagorean_default.png) ### Updating Input Values The value provided to the
+`Input` class in your calculation function is treated as a default value. When
+you run your calculation with different input values, pass in a dictionary of
+the default overrides into the optional second parameter of the
+`ReportBuilder`: ```python new_inputs = {"a": 9.2, "b": 0.87} builder =
+ReportBuilder(calculation, new_inputs) builder.view_report() ``` # Features
+#### Automated report generation Generate detailed, professional reports
+automatically, ensuring clarity and precision in communication. #### Open
+source efficalc welcomes community contributions. Request features or
+contribute directly to enhance its capabilities. #### Engineering-specific
+features Benefit from built-in tools tailored to solving common engineering
+challenges. [See our section property library in action](https://github.com/
+youandvern/efficalc/blob/main/examples/advanced/
+steel_beam_moment_strength.py#L53). #### Reusable Create calculation templates
+once and reuse them across multiple designs and projects, saving time and
+ensuring consistency. #### Testable Easily test your calculations to reduce
 errors and improve confidence every design. [Read the testing guide.](https://
 youandvern.github.io/efficalc/testing.html) #### Integrate with other workflows
 Seamlessly integrate with your existing Python-enabled workflows to boost
 efficiency and connectivity across tools and platforms. [See some examples of
 this.](https://youandvern.github.io/efficalc/integration.html) #### Figures now
 supported Easily add figures to your calculation reports for even more clarity.
 [Read the full documentation for figures.](https://youandvern.github.io/
 efficalc/figures.html) #### Control your content Tailor your calculation
 reports to include only the most relevant information, making them as concise
-or detailed as you prefer. ## Quickstart ### Installation Install efficalc with
-pip: ```bash pip install efficalc ``` ### First Calculation Function
-Calculations in efficalc are written as a function. These calculation functions
-are primarily composed of `Input` and `Calculation` elements, but there are
-also many more options to make a clear and accurate calculation. ```python from
-efficalc import Calculation, Input, Title, sqrt def calculation(): Title
-("Pythagorean's Theorem and Perimeter") a = Input("a", 3, description="Length
-of side a") b = Input("b", 4, description="Length of side b") c = Calculation
-("c", sqrt(a**2 + b**2), description="Length of the hypotenuse") Calculation
-("P", a + b + c, description="Perimeter of the triangle") ``` ### View the
-Report Instantly view or print a report for your calculation in your browser
-with the `ReportBuilder`. ```python from efficalc.report_builder import
-ReportBuilder from pythagorean_perimeter import calculation builder =
-ReportBuilder(calculation) builder.view_report() ``` ![The resulting
-calculation report](https://github.com/youandvern/efficalc/raw/main/docs_src/
-_static/pythagorean_default.png) ### Update Input Values The value proved to
-the `Input` class in your calculation function is treated as a default value.
-If you want to change any of your input values, pass in a dictionary of the
-default overrides as an optional second parameter to the `ReportBuilder`:
-```python new_inputs = {"a": 9.2, "b": 0.87} builder = ReportBuilder
-(calculation, new_inputs) builder.view_report() ``` ## Contributing We welcome
-contributions of all kinds from the community! Whether it's reporting a bug,
-requesting a feature, or submitting a pull request, your input and engagement
-is invaluable to efficalc's development. - Report issues [here](https://
-github.com/youandvern/efficalc/issues). - Submit pull requests [here](https://
-github.com/youandvern/efficalc/pulls). ## Built With * [latexexpr](https://
-github.com/kajusK/latexexpr) - [we use a forked version](https://github.com/
-youandvern/latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/
-pylatexenc) #### Documentation * [sphinx](https://www.sphinx-doc.org/en/master/
-) * [furo](https://github.com/pradyunsg/furo/) * [sphinx-copybutton](https://
-github.com/executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://
-github.com/sphinx-contrib/video) ## License efficalc is released under the [MIT
-License](https://github.com/youandvern/efficalc/tree/main/LICENSE).
+or detailed as you prefer. # Contributing We welcome contributions of all kinds
+from the community! Whether it's reporting a bug, requesting a feature, or
+submitting a pull request, your input and engagement is invaluable to
+efficalc's development. - Report issues [here](https://github.com/youandvern/
+efficalc/issues). - Submit pull requests [here](https://github.com/youandvern/
+efficalc/pulls). # Built With * [latexexpr](https://github.com/kajusK/
+latexexpr) - [we use a forked version](https://github.com/youandvern/
+latexexpr_efficalc) * [pylatexenc](https://github.com/phfaist/pylatexenc) ####
+Documentation * [sphinx](https://www.sphinx-doc.org/en/master/) * [furo](https:
+//github.com/pradyunsg/furo/) * [sphinx-copybutton](https://github.com/
+executablebooks/sphinx-copybutton) * [sphinxcontrib-video](https://github.com/
+sphinx-contrib/video) # License efficalc is released under the [MIT License]
+(https://github.com/youandvern/efficalc/tree/main/LICENSE).
```

### Comparing `efficalc-1.1.0/efficalc.egg-info/SOURCES.txt` & `efficalc-1.2.0/efficalc.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 efficalc/base_definitions/calculation.py
 efficalc/base_definitions/comparison.py
 efficalc/base_definitions/comparison_statement.py
 efficalc/base_definitions/figure.py
 efficalc/base_definitions/heading.py
 efficalc/base_definitions/input.py
 efficalc/base_definitions/shared.py
+efficalc/base_definitions/symbolic.py
 efficalc/base_definitions/text_block.py
 efficalc/base_definitions/title.py
 efficalc/sections/__init__.py
 efficalc/sections/aisc_angle.py
 efficalc/sections/aisc_channel.py
 efficalc/sections/aisc_circular.py
 efficalc/sections/aisc_double_angle.py
```

### Comparing `efficalc-1.1.0/pyproject.toml` & `efficalc-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "efficalc"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Andrew Young", email="youandvern@gmail.com" },
 ]
 description = "Feature-rich open source library for building well-formatted and extensible engineering calculations."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `efficalc-1.1.0/tests/test_calculation_runner.py` & `efficalc-1.2.0/tests/test_calculation_runner.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/tests/test_generate_html.py` & `efficalc-1.2.0/tests/test_generate_html.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     CalculationLength,
     Comparison,
     ComparisonStatement,
     FigureBase,
     FigureFromFile,
     Heading,
     Input,
+    Symbolic,
     TextBlock,
     Title,
     clear_saved_objects,
 )
 from efficalc.generate_html import generate_html_for_calc_items
 
 
@@ -110,14 +111,50 @@
     assert calc.str_substituted() in result
     assert calc.str_result_with_unit() in result
     assert r"\therefore" in result
     assert "ERROR:" in result
     assert "could not be calculated because zero was in the denominator." in result
 
 
+def test_symbolic(common_setup_teardown):
+    a = Input("a", 2, "mm")
+    b = Input("b", 7, "mm")
+    sym = Symbolic("sym", a + b, "describing text", "refer to code")
+    result = generate_html_for_calc_items([sym])
+    assert sym.description in result
+    assert sym.reference in result
+    assert sym.name in result
+    assert sym.str_symbolic() in result
+    assert r"\therefore" not in result
+
+
+def test_symbolic_without_ref_or_desc(common_setup_teardown):
+    sym = Symbolic("calc_1", "sym_str")
+    result = generate_html_for_calc_items([sym])
+    assert sym.name in result
+    assert sym.str_symbolic() in result
+    assert r"\therefore" not in result
+    assert "[]" not in result  # empty reference tag
+
+
+def test_symbolic_error(common_setup_teardown):
+    a = Input("a", 2, "mm")
+    sym = Symbolic("sym", a / 0, "describing text", "refer to code")
+    sym.result()
+    result = generate_html_for_calc_items([sym])
+    assert sym.estimate_display_length() == CalculationLength.SHORT
+    assert sym.description in result
+    assert sym.reference in result
+    assert sym.name in result
+    assert sym.str_symbolic() in result
+    assert r"\therefore" not in result
+    assert "ERROR:" in result
+    assert "could not be calculated because zero was in the denominator." in result
+
+
 def test_comparison_number(common_setup_teardown):
 
     calc = Comparison(5, ">", 2, "good", "nah", "a describer", "the ref")
     result = generate_html_for_calc_items([calc])
     assert calc.description in result
     assert calc.reference in result
     assert ">" in result
```

### Comparing `efficalc-1.1.0/tests/test_math_operations.py` & `efficalc-1.2.0/tests/test_math_operations.py`

 * *Files identical despite different names*

### Comparing `efficalc-1.1.0/tests/test_report_builder.py` & `efficalc-1.2.0/tests/test_report_builder.py`

 * *Files identical despite different names*

