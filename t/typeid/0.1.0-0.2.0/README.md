# Comparing `tmp/typeid-0.1.0.tar.gz` & `tmp/typeid-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid-0.1.0.tar", max compression
+gzip compressed data, was "typeid-0.2.0.tar", max compression
```

## Comparing `typeid-0.1.0.tar` & `typeid-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 11:53:12.620224 typeid-0.1.0/LICENSE
--rw-r--r--   0        0        0     1336 2024-05-21 11:54:25.460457 typeid-0.1.0/README.md
--rw-r--r--   0        0        0      474 2024-05-21 11:56:28.694103 typeid-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3047 2024-05-21 11:53:49.143679 typeid-0.1.0/typeid/__init__.py
--rw-r--r--   0        0        0     1865 1970-01-01 00:00:00.000000 typeid-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 11:53:12.620224 typeid-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2067 2024-05-22 15:40:19.782174 typeid-0.2.0/README.md
+-rw-r--r--   0        0        0      474 2024-05-22 15:40:49.475427 typeid-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3850 2024-05-22 15:33:55.219867 typeid-0.2.0/typeid/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-22 15:35:58.509544 typeid-0.2.0/typeid/sqla.py
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 typeid-0.2.0/PKG-INFO
```

### Comparing `typeid-0.1.0/LICENSE` & `typeid-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid-0.1.0/typeid/__init__.py` & `typeid-0.2.0/typeid/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,36 +24,37 @@
     >>> UserId("sk_nnv5rr3rfk3hgry6xrygr")
     Traceback (most recent call last):
     ...
     ValueError: Wrong prefix, got sk, expected user
 
 """
 
+from typing import Dict
 from base58 import b58encode, b58decode
 from uuid import UUID
 
 
 class BaseId(UUID):
     """BaseID implementation that does the lifting of a UUID into a typed UUID
     and formats it more nicely.
 
     :param _prefix: The internal _prefix is filled in the generate() method
     """
 
     #: This class variable will be filled in by type() later own
     _prefix: str = ""
 
-    def __init__(self, id: UUID | str | bytes):
+    def __init__(self, id: UUID | str | bytes) -> None:
         if isinstance(id, UUID):
             super().__init__(id.hex)
         elif isinstance(id, bytes):
             super().__init__(id.hex())
         elif isinstance(id, str):
             if id.startswith(self._prefix):
-                prefix_free_id = id[len(self._prefix) + 1:]
+                prefix_free_id = id[len(self._prefix) + 1 :]
                 uid: bytes = b58decode(prefix_free_id)
                 super().__init__(uid.hex())
             elif "_" in id:
                 found_prefix = id[: id.index("_")]
                 raise ValueError(
                     f"Wrong prefix, got {found_prefix}, expected {self._prefix}"
                 )
@@ -70,21 +71,44 @@
         :return: encoded and prefixed id as string
         """
         prefix = str(self._prefix)
         id = b58encode(self.bytes).decode("ascii").lower()
         return f"{prefix}_{id}"
 
 
-def generate(*args: str, suffix: str = "Id"):
+class AttrDict(dict):
+    """This class enables us to access the return values of generate() as
+    attributes."""
+
+    def __init__(self, *args, **kwargs):
+        super(AttrDict, self).__init__(*args, **kwargs)
+        self.__dict__ = self
+
+
+def generate(*args: str, suffix: str = "Id", enable_sqla=False) -> Dict[str, BaseId]:
     """Generate types based on a list of arguments. Each argument will result in
     a new type named after the argument (camel-cased) with the defined suffix at the end.
     """
+    ret = {}
     for _type in args:
         name = f"{_type.capitalize()}{suffix}"
-        globals()[name] = type(name, (BaseId,), dict(_prefix=_type))
+        typeid_class = type(name, (BaseId,), dict(_prefix=_type))
+        globals()[name] = typeid_class
+        ret[name] = typeid_class
+
+        # If the user wants sqla support, these additional classes will be
+        # generated
+        if enable_sqla:
+            from .sqla import GUID
+
+            sqla_name = f"{name}SQLA"
+            sqla_typeid_class = type(name, (GUID,), dict(typeid_class=typeid_class))
+            globals()[sqla_name] = sqla_typeid_class
+            ret[sqla_name] = sqla_typeid_class
+    return AttrDict(ret)
 
 
 if __name__ == "__main__":
     import doctest
 
     generate("sk", "pk", "user", "apikey")
     generate("admin", suffix="IdUseWithCare")
```

### Comparing `typeid-0.1.0/PKG-INFO` & `typeid-0.2.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid
-Version: 0.1.0
+Version: 0.2.0
 Summary: UUID-compatible Typed IDs with prefixes
 License: MIT
 Author: Fabian Schuh
 Author-email: info@chainsquad.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,24 +31,58 @@
 
 First generate the Types using generate(...), then use them like so:
 
 ```python
 from uuid_extensions import uuid7
 from typeid import generate
 
-# Generate a bunch of new id types
-generate("sk", "pk", "user", "apikey")
+typeids = generate("user", enable_sqla=True)
 
 # Now they can be used with SkId, PkId, UserId, and ApikeyId
-assert str(SkId(uuid7().hex)).startswith("sk_")
-assert str(PkId(uuid7().hex)).startswith("pk_")
-assert str(UserId(uuid7().hex)).startswith("user_")
-assert str(ApikeyId(uuid7().hex)).startswith("apikey_")
+assert str(typeids.SkId(uuid7().hex)).startswith("sk_")
+assert str(typeids.PkId(uuid7().hex)).startswith("pk_")
+assert str(typeids.UserId(uuid7().hex)).startswith("user_")
+assert str(typeids.ApikeyId(uuid7().hex)).startswith("apikey_")
 
 # Obviously, loading a prefixed type id in the correct Type works just fine
-assert (UserId("user_nnv5rr3rfk3hgry6xrygr").hex == "0664c4135ed83faabd4bc0dc33839c9f")
+assert (typeids.UserId("user_nnv5rr3rfk3hgry6xrygr").hex == "0664c4135ed83faabd4bc0dc33839c9f")
 
 # Use custom suffixes, just in case you need them
 generate("admin", suffix="IdUseWithCare")
-assert str(AdminIdUseWithCare(uuid7().hex)).startswith("admin_")
+assert str(typeids.AdminIdUseWithCare(uuid7().hex)).startswith("admin_")
+```
+
+## SqlAlchemy Support
+
+The library also allows to create classes specifically for the use with
+sqlalchemy.
+
+#### Example
+
+```python
+from typeid import generate
+
+typeids = generate("user", enable_sqla=True)
+
+class User(Base):
+    __tablename__ = "user"
+
+    # use typeids.UserId in the Mapper[]
+    id: Mapped[typeids.UserId] = mapped_column(
+        # use typeids.UserIdSQLA in the mapped_column!
+        typeids.UserIdSQLA, primary_key=True, default=uuid.uuid4
+    )
+
+    name: str = Column(String(128), unique=True)
+
+user = User(name="John Doe")
+(db,) = get_session()
+db.add(user)
+db.commit()
+db.refresh(user)
+print(type(user.id))
+# <class 'typeid.UserId'>
+
+print((user.id))
+# user_qvnrsem3skqho2hgni2mfk
 ```
```

