# Comparing `tmp/skipy-0.1.4.tar.gz` & `tmp/skipy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skipy-0.1.4.tar", max compression
+gzip compressed data, was "skipy-0.1.5.tar", max compression
```

## Comparing `skipy-0.1.4.tar` & `skipy-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      119 2024-05-22 09:59:41.090950 skipy-0.1.4/README.md
--rw-r--r--   0        0        0     1152 2024-05-22 09:59:41.090950 skipy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       64 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/AWS/__init__.py
--rw-r--r--   0        0        0      599 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/AWS/utils.py
--rw-r--r--   0        0        0       56 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Chatwork/__init__.py
--rw-r--r--   0        0        0     5722 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Chatwork/__wrapper.py
--rw-r--r--   0        0        0      108 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/GCP/__init__.py
--rw-r--r--   0        0        0     5944 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/GCP/drive.py
--rw-r--r--   0        0        0     3633 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/GCP/sheet.py
--rw-r--r--   0        0        0       64 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Selenium/__init__.py
--rw-r--r--   0        0        0     1117 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Selenium/__wrapper.py
--rw-r--r--   0        0        0       50 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Slack/__init__.py
--rw-r--r--   0        0        0      483 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/Slack/__wrapper.py
--rw-r--r--   0        0        0       50 2024-05-22 09:59:41.090950 skipy-0.1.4/skipy/__init__.py
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 skipy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      119 2024-05-22 10:46:35.720830 skipy-0.1.5/README.md
+-rw-r--r--   0        0        0     1152 2024-05-22 10:46:35.720830 skipy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/AWS/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/AWS/utils.py
+-rw-r--r--   0        0        0       56 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/Chatwork/__init__.py
+-rw-r--r--   0        0        0     5722 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/Chatwork/__wrapper.py
+-rw-r--r--   0        0        0      108 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/GCP/__init__.py
+-rw-r--r--   0        0        0     5944 2024-05-22 10:46:35.720830 skipy-0.1.5/skipy/GCP/drive.py
+-rw-r--r--   0        0        0     3633 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/GCP/sheet.py
+-rw-r--r--   0        0        0       64 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/Selenium/__init__.py
+-rw-r--r--   0        0        0     1164 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/Selenium/__wrapper.py
+-rw-r--r--   0        0        0       50 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/Slack/__init__.py
+-rw-r--r--   0        0        0      483 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/Slack/__wrapper.py
+-rw-r--r--   0        0        0       50 2024-05-22 10:46:35.724830 skipy-0.1.5/skipy/__init__.py
+-rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 skipy-0.1.5/PKG-INFO
```

### Comparing `skipy-0.1.4/pyproject.toml` & `skipy-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skipy-0.1.4/skipy/AWS/utils.py` & `skipy-0.1.5/skipy/AWS/utils.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.4/skipy/Chatwork/__wrapper.py` & `skipy-0.1.5/skipy/Chatwork/__wrapper.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.4/skipy/GCP/drive.py` & `skipy-0.1.5/skipy/GCP/drive.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.4/skipy/GCP/sheet.py` & `skipy-0.1.5/skipy/GCP/sheet.py`

 * *Files identical despite different names*

### Comparing `skipy-0.1.4/skipy/Selenium/__wrapper.py` & `skipy-0.1.5/skipy/Selenium/__wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     os.makedirs(dl_path, exist_ok=True)
     options.add_experimental_option(
         "prefs",
         {"download.default_directory": dl_path, "download.prompt_for_download": False},
     )
     if is_lambda:
         chrome = webdriver.Chrome(
-            service=Service("/opt/chromedriver-linux64"),
+            service=Service("/opt/chromedriver"),
             options=options,
         )
+        options.binary_location = "/opt/chrome/chrome"
     else:
         chrome = webdriver.Chrome(options=options)
 
     chrome.implicitly_wait(15)
     return chrome
```

### Comparing `skipy-0.1.4/PKG-INFO` & `skipy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skipy
-Version: 0.1.4
+Version: 0.1.5
 Summary: Skip-tac python modules
 License: MIT
 Author: syamaguc
 Author-email: programmer2844@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

