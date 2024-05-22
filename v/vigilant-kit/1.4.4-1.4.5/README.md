# Comparing `tmp/vigilant_kit-1.4.4.tar.gz` & `tmp/vigilant_kit-1.4.5.tar.gz`

## Comparing `vigilant_kit-1.4.4.tar` & `vigilant_kit-1.4.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/CHANGELOG.md
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/vgl_config.yaml.example
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/bin/doc_generator.py
--rw-r--r--   0        0        0    31729 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/actions.md
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/browser_options.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/changelog_logic.md
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/configuration.md
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/native_selenium.md
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/docs/vigilant_unittest.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/data_saver.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/vigilant_pdf.py
--rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/LICENSE
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/pyproject.toml
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 vigilant_kit-1.4.4/PKG-INFO
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/CHANGELOG.md
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/vgl_config.yaml.example
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/bin/doc_generator.py
+-rw-r--r--   0        0        0    31729 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/actions.md
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/browser_options.md
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/changelog_logic.md
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/configuration.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/data_saver.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0    15142 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/vigilant_pdf.py
+-rw-r--r--   0        0        0     5064 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/LICENSE
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/README.md
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 vigilant_kit-1.4.5/PKG-INFO
```

### Comparing `vigilant_kit-1.4.4/CHANGELOG.md` & `vigilant_kit-1.4.5/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog for Vigilant Kit
 
 ### [Logic behind Changelog](docs/changelog_logic.md)
 
+## Version 1.4.5
+
+### Code refactor 
+
+- Refactored class `VigilantDriver()`, refactored methods for creating driver sessions, added docstrings.
+
 ## Version 1.4.4
 
 ### Code refactor & New features
 
 - Added new class that allows to test PDF files `VigilantPDF`
 - Added new method `find_pdf_file()` - find PDF files that match a given regex pattern within the specified directory.
 - Added new method `assert_strings_are_in_file()` - assert that all strings in the list are found in the specified PDF files.
```

### Comparing `vigilant_kit-1.4.4/bin/doc_generator.py` & `vigilant_kit-1.4.5/bin/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/actions.md` & `vigilant_kit-1.4.5/docs/actions.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/browser_options.md` & `vigilant_kit-1.4.5/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/changelog_logic.md` & `vigilant_kit-1.4.5/docs/changelog_logic.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/configuration.md` & `vigilant_kit-1.4.5/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/native_selenium.md` & `vigilant_kit-1.4.5/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/selenium_install.md` & `vigilant_kit-1.4.5/docs/selenium_install.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/tutorial_pytest.md` & `vigilant_kit-1.4.5/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/vigilant_pytest.md` & `vigilant_kit-1.4.5/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/docs/vigilant_unittest.md` & `vigilant_kit-1.4.5/docs/vigilant_unittest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/actions/assertions.py` & `vigilant_kit-1.4.5/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/actions/finder.py` & `vigilant_kit-1.4.5/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.4.5/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/actions/vigilant_pdf.py` & `vigilant_kit-1.4.5/src/vigilant/actions/vigilant_pdf.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/actions/waiter.py` & `vigilant_kit-1.4.5/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/src/vigilant/driver/__init__.py` & `vigilant_kit-1.4.5/src/vigilant/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/.gitignore` & `vigilant_kit-1.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/LICENSE` & `vigilant_kit-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/README.md` & `vigilant_kit-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.4.4/pyproject.toml` & `vigilant_kit-1.4.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.4.4"
+version = "1.4.5"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `vigilant_kit-1.4.4/PKG-INFO` & `vigilant_kit-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vigilant_kit
-Version: 1.4.4
+Version: 1.4.5
 Summary: Library that makes functional testing with Selenium WebDriver fast and easy. 
 Project-URL: Homepage, https://github.com/ivpel/vigilant
 Project-URL: Bug Tracker, https://github.com/ivpel/vigilant/issues
 Author-email: Pelykh Ivan <ivan.pelykh@protonmail.com>
 License-File: LICENSE
 Keywords: bdd,functional,functional-testing,pytest,selenium,tdd,testing,unittest,webdriver
 Requires-Python: >=3.7
```

