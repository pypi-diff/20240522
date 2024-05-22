# Comparing `tmp/aioamazondevices-0.1.0.tar.gz` & `tmp/aioamazondevices-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioamazondevices-0.1.0.tar", max compression
+gzip compressed data, was "aioamazondevices-0.1.1.tar", max compression
```

## Comparing `aioamazondevices-0.1.0.tar` & `aioamazondevices-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11346 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/LICENSE
--rw-r--r--   0        0        0     3588 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/README.md
--rw-r--r--   0        0        0     2296 2024-05-07 20:46:52.609484 aioamazondevices-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      276 2024-05-07 20:46:52.617484 aioamazondevices-0.1.0/src/aioamazondevices/__init__.py
--rw-r--r--   0        0        0     8856 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/api.py
--rw-r--r--   0        0        0     1089 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/const.py
--rw-r--r--   0        0        0      444 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-07 20:46:51.825465 aioamazondevices-0.1.0/src/aioamazondevices/py.typed
--rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 aioamazondevices-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-05-22 07:21:37.363623 aioamazondevices-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3588 2024-05-22 07:21:37.363623 aioamazondevices-0.1.1/README.md
+-rw-r--r--   0        0        0     2296 2024-05-22 07:21:38.763634 aioamazondevices-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      276 2024-05-22 07:21:38.767634 aioamazondevices-0.1.1/src/aioamazondevices/__init__.py
+-rw-r--r--   0        0        0     8934 2024-05-22 07:21:37.367622 aioamazondevices-0.1.1/src/aioamazondevices/api.py
+-rw-r--r--   0        0        0     1089 2024-05-22 07:21:37.367622 aioamazondevices-0.1.1/src/aioamazondevices/const.py
+-rw-r--r--   0        0        0      444 2024-05-22 07:21:37.367622 aioamazondevices-0.1.1/src/aioamazondevices/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-22 07:21:37.367622 aioamazondevices-0.1.1/src/aioamazondevices/py.typed
+-rw-r--r--   0        0        0     4680 1970-01-01 00:00:00.000000 aioamazondevices-0.1.1/PKG-INFO
```

### Comparing `aioamazondevices-0.1.0/LICENSE` & `aioamazondevices-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioamazondevices-0.1.0/README.md` & `aioamazondevices-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aioamazondevices-0.1.0/pyproject.toml` & `aioamazondevices-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioamazondevices"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python library to control Amazon devices"
 authors = ["Simone Chemelli <simone.chemelli@gmail.com>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/chemelli74/aioamazondevices"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

### Comparing `aioamazondevices-0.1.0/src/aioamazondevices/api.py` & `aioamazondevices-0.1.1/src/aioamazondevices/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,20 +66,23 @@
     def __init__(
         self,
         login_country_code: str,
         login_email: str,
         login_password: str,
     ) -> None:
         """Initialize the scanner."""
-        locale = DOMAIN_BY_COUNTRY.get(login_country_code)
-        domain = locale["domain"] if locale else login_country_code
+        # Force country digits as lower case
+        country_code = login_country_code.lower()
+
+        locale = DOMAIN_BY_COUNTRY.get(country_code)
+        domain = locale["domain"] if locale else country_code
 
         assoc_handle = "amzn_dp_project_dee_ios"
         if not locale:
-            assoc_handle += f"_{login_country_code}"
+            assoc_handle += f"_{country_code}"
         self._assoc_handle = assoc_handle
 
         self._login_email = login_email
         self._login_password = login_password
         self._domain = domain
         self._url = f"https://www.amazon.{domain}"
         self._cookies = _build_init_cookies()
```

### Comparing `aioamazondevices-0.1.0/src/aioamazondevices/const.py` & `aioamazondevices-0.1.1/src/aioamazondevices/const.py`

 * *Files identical despite different names*

### Comparing `aioamazondevices-0.1.0/PKG-INFO` & `aioamazondevices-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioamazondevices
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python library to control Amazon devices
 Home-page: https://github.com/chemelli74/aioamazondevices
 License: Apache Software License 2.0
 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioamazondevices Version: 0.1.0 Summary: Python
+Metadata-Version: 2.1 Name: aioamazondevices Version: 0.1.1 Summary: Python
 library to control Amazon devices Home-page: https://github.com/chemelli74/
 aioamazondevices License: Apache Software License 2.0 Author: Simone Chemelli
 Author-email: simone.chemelli@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

