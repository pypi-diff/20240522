# Comparing `tmp/rfc9457-0.0.4.tar.gz` & `tmp/rfc9457-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc9457-0.0.4.tar", max compression
+gzip compressed data, was "rfc9457-0.0.5.tar", max compression
```

## Comparing `rfc9457-0.0.4.tar` & `rfc9457-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11307 2024-05-17 08:47:51.051562 rfc9457-0.0.4/LICENSE
--rw-r--r--   0        0        0     1789 2024-05-17 08:47:51.055562 rfc9457-0.0.4/README.md
--rw-r--r--   0        0        0     2021 2024-05-17 08:47:51.055562 rfc9457-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2723 2024-05-17 08:47:51.055562 rfc9457-0.0.4/src/rfc9457/__init__.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11307 2024-05-21 16:54:09.801519 rfc9457-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1789 2024-05-21 16:54:09.801519 rfc9457-0.0.5/README.md
+-rw-r--r--   0        0        0     2021 2024-05-21 16:54:09.801519 rfc9457-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2777 2024-05-21 16:54:09.801519 rfc9457-0.0.5/src/rfc9457/__init__.py
+-rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 rfc9457-0.0.5/PKG-INFO
```

### Comparing `rfc9457-0.0.4/LICENSE` & `rfc9457-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.4/README.md` & `rfc9457-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `rfc9457-0.0.4/pyproject.toml` & `rfc9457-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rfc9457"
-version = "0.0.4"
+version = "0.0.5"
 description = "Implementation of RFC9457 problems."
 authors = ["Daniel Edgecombe <daniel@nrwl.co>"]
 license = "Apache-2.0"
 repository="https://github.com/NRWLDev/rfc9457/"
 homepage="https://github.com/NRWLDev/rfc9457/"
 readme = "README.md"
 
@@ -19,15 +19,15 @@
 pytest-random-order = "^1.0"
 
 # Style
 ruff = "^0.3"
 pre-commit = "^3.0.2"
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `rfc9457-0.0.4/src/rfc9457/__init__.py` & `rfc9457-0.0.5/src/rfc9457/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,24 @@
         self: t.Self,
         title: str,
         type_: str | None = None,
         details: str | None = None,
         status: int = 500,
         **kwargs,
     ) -> None:
-        super().__init__(title)
         self._type = type_
         self.title = title
         self.details = details
         self.status = status
         self.status_code = status  # work around for sentry integrations that expect status_code attr
         self.extras = kwargs
 
+    def __str__(self: t.Self) -> str:
+        return f"{self.title}: {self.details}"
+
     @property
     def type(self: t.Self) -> str:
         type_ = error_class_to_type(self)
         return self._type if self._type else type_
 
     def marshal(self: t.Self, *, strip_debug: bool = False) -> dict[str, t.Any]:
         """Generate a JSON compatible representation.
```

### Comparing `rfc9457-0.0.4/PKG-INFO` & `rfc9457-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc9457
-Version: 0.0.4
+Version: 0.0.5
 Summary: Implementation of RFC9457 problems.
 Home-page: https://github.com/NRWLDev/rfc9457/
 License: Apache-2.0
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

