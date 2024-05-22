# Comparing `tmp/sipmessage-0.2.1.tar.gz` & `tmp/sipmessage-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sipmessage-0.2.1.tar", last modified: Tue May 21 11:05:35 2024, max compression
+gzip compressed data, was "sipmessage-0.2.2.tar", last modified: Wed May 22 21:13:34 2024, max compression
```

## Comparing `sipmessage-0.2.1.tar` & `sipmessage-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.550305 sipmessage-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-21 11:05:26.000000 sipmessage-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-21 11:05:26.000000 sipmessage-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-21 11:05:26.000000 sipmessage-0.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-21 11:05:35.550305 sipmessage-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-21 11:05:26.000000 sipmessage-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 11:05:26.000000 sipmessage-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-21 11:05:26.000000 sipmessage-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:05:35.550305 sipmessage-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:05:26.000000 sipmessage-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.542305 sipmessage-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/src/sipmessage/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/address.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-21 11:05:26.000000 sipmessage-0.2.1/src/sipmessage/via.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.550305 sipmessage-0.2.1/src/sipmessage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 11:05:35.000000 sipmessage-0.2.1/src/sipmessage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:35.546305 sipmessage-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 11:05:26.000000 sipmessage-0.2.1/tests/test_via.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.705148 sipmessage-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 21:13:30.000000 sipmessage-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-22 21:13:30.000000 sipmessage-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-22 21:13:30.000000 sipmessage-0.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-22 21:13:34.701148 sipmessage-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-22 21:13:30.000000 sipmessage-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.697148 sipmessage-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 21:13:30.000000 sipmessage-0.2.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-22 21:13:30.000000 sipmessage-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 21:13:30.000000 sipmessage-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-22 21:13:30.000000 sipmessage-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:13:34.705148 sipmessage-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:13:30.000000 sipmessage-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.697148 sipmessage-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.701148 sipmessage-0.2.2/src/sipmessage/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-22 21:13:30.000000 sipmessage-0.2.2/src/sipmessage/via.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.701148 sipmessage-0.2.2/src/sipmessage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-22 21:13:34.000000 sipmessage-0.2.2/src/sipmessage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-22 21:13:34.000000 sipmessage-0.2.2/src/sipmessage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:13:34.000000 sipmessage-0.2.2/src/sipmessage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 21:13:34.000000 sipmessage-0.2.2/src/sipmessage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 21:13:34.000000 sipmessage-0.2.2/src/sipmessage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:34.701148 sipmessage-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/test_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-22 21:13:30.000000 sipmessage-0.2.2/tests/test_via.py
```

### Comparing `sipmessage-0.2.1/LICENSE` & `sipmessage-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/Makefile` & `sipmessage-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/PKG-INFO` & `sipmessage-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
```

### Comparing `sipmessage-0.2.1/README.rst` & `sipmessage-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/docs/Makefile` & `sipmessage-0.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/docs/conf.py` & `sipmessage-0.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/docs/index.rst` & `sipmessage-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/pyproject.toml` & `sipmessage-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 # Version
 name = "sipmessage"
-version = "0.2.1"
+version = "0.2.2"
 
 # Dependencies
 dependencies = []
 requires-python = ">= 3.10"
 
 # Development
 authors = [
```

### Comparing `sipmessage-0.2.1/src/sipmessage/address.py` & `sipmessage-0.2.2/src/sipmessage/address.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     parameters: Parameters = dataclasses.field(default_factory=Parameters)
     "The parameters of the address."
 
     @classmethod
     def parse(cls, value: str) -> "Address":
         """
         Parse the given string into an :class:`Address` instance.
+
+        If parsing fails, a :class:`ValueError` is raised.
         """
         for pattern in ADDRESS_PATTERNS:
             m = pattern.match(value)
             if m:
                 return cls(
                     uri=URI.parse(m.group("uri")),
                     name=m.group("name"),
```

### Comparing `sipmessage-0.2.1/src/sipmessage/parameters.py` & `sipmessage-0.2.2/src/sipmessage/parameters.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/src/sipmessage/uri.py` & `sipmessage-0.2.2/src/sipmessage/uri.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,30 +33,40 @@
     parameters: Parameters = dataclasses.field(default_factory=Parameters)
     "Parameters affecting a request constructed from the URI."
 
     @classmethod
     def parse(cls, value: str) -> "URI":
         """
         Parse the given string into a :class:`URI` instance.
+
+        If parsing fails, a :class:`ValueError` is raised.
         """
         parsed = urllib.parse.urlparse(value)
+
+        # Check the URI scheme is valid.
+        if parsed.scheme not in ("sip", "sips"):
+            raise ValueError("URI scheme must be 'sip' or 'sips'")
+
         if "@" in parsed.path:
             user_password, host_port = parsed.path.split("@")
             if ":" in user_password:
                 user, password = user_password.split(":")
             else:
                 user = user_password
                 password = None
         else:
             host_port = parsed.path
             user = None
             password = None
         if ":" in host_port:
             host, port_ = host_port.split(":")
-            port = int(port_)
+            try:
+                port = int(port_)
+            except ValueError:
+                raise ValueError("URI port must be an integer")
         else:
             host = host_port
             port = None
         return cls(
             scheme=parsed.scheme,
             host=host,
             port=port,
```

### Comparing `sipmessage-0.2.1/src/sipmessage/via.py` & `sipmessage-0.2.2/src/sipmessage/via.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,16 @@
     parameters: Parameters = dataclasses.field(default_factory=Parameters)
     "The parameters of the address."
 
     @classmethod
     def parse(cls, value: str) -> "Via":
         """
         Parse the given string into a :class:`Via` instance.
+
+        If parsing fails, a :class:`ValueError` is raised.
         """
         m = re.match(r"SIP/2\.0/([A-Z]+) (.+)", value)
         if m is None:
             raise ValueError("Malformed Via header")
 
         transport = m.group(1)
         address, _, rest = m.group(2).partition(";")
```

### Comparing `sipmessage-0.2.1/src/sipmessage.egg-info/PKG-INFO` & `sipmessage-0.2.2/src/sipmessage.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sipmessage
-Version: 0.2.1
+Version: 0.2.2
 Summary: Pure python parsing of SIP messages and headers
 Author-email: Spacinov Engineering <opensource@spacinov.com>
 License: BSD License
 Project-URL: Homepage, https://sipmessage.readthedocs.io/
 Project-URL: Documentation, https://sipmessage.readthedocs.io/
 Project-URL: Repository, https://github.com/spacinov/sipmessage
 Project-URL: Issues, https://github.com/spacinov/sipmessage/issues
```

### Comparing `sipmessage-0.2.1/src/sipmessage.egg-info/SOURCES.txt` & `sipmessage-0.2.2/src/sipmessage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/tests/test_address.py` & `sipmessage-0.2.2/tests/test_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,19 @@
 
 class AddressTest(unittest.TestCase):
     def test_empty(self) -> None:
         with self.assertRaises(ValueError) as cm:
             Address.parse("")
         self.assertEqual(str(cm.exception), "Not a valid address")
 
+    def test_invalid_uri(self) -> None:
+        with self.assertRaises(ValueError) as cm:
+            Address.parse("atlanta.com")
+        self.assertEqual(str(cm.exception), "URI scheme must be 'sip' or 'sips'")
+
     def test_no_brackets(self) -> None:
         contact = Address.parse("sip:+12125551212@phone2net.com;tag=887s")
         self.assertEqual(contact.name, "")
         self.assertEqual(str(contact.uri), "sip:+12125551212@phone2net.com")
         self.assertEqual(contact.parameters, {"tag": "887s"})
         self.assertEqual(str(contact), "<sip:+12125551212@phone2net.com>;tag=887s")
```

### Comparing `sipmessage-0.2.1/tests/test_parameters.py` & `sipmessage-0.2.2/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `sipmessage-0.2.1/tests/test_uri.py` & `sipmessage-0.2.2/tests/test_uri.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,36 @@
 
 import unittest
 
 from sipmessage import URI
 
 
 class URITest(unittest.TestCase):
+    def test_invalid_port(self) -> None:
+        # No port.
+        with self.assertRaises(ValueError) as cm:
+            URI.parse("sip:atlanta.com:")
+        self.assertEqual(str(cm.exception), "URI port must be an integer")
+
+        # Invalid port.
+        with self.assertRaises(ValueError) as cm:
+            URI.parse("sip:atlanta.com:bob")
+        self.assertEqual(str(cm.exception), "URI port must be an integer")
+
+    def test_invalid_scheme(self) -> None:
+        # No scheme.
+        with self.assertRaises(ValueError) as cm:
+            URI.parse("atlanta.com")
+        self.assertEqual(str(cm.exception), "URI scheme must be 'sip' or 'sips'")
+
+        # Invalid scheme.
+        with self.assertRaises(ValueError) as cm:
+            URI.parse("bogus:atlanta.com")
+        self.assertEqual(str(cm.exception), "URI scheme must be 'sip' or 'sips'")
+
     def test_host(self) -> None:
         uri = URI.parse("sip:atlanta.com")
 
         self.assertEqual(uri.host, "atlanta.com")
         self.assertEqual(uri.port, None)
         self.assertEqual(uri.user, None)
         self.assertEqual(uri.password, None)
```

### Comparing `sipmessage-0.2.1/tests/test_via.py` & `sipmessage-0.2.2/tests/test_via.py`

 * *Files identical despite different names*

