# Comparing `tmp/karp_lex_types-0.7.0.tar.gz` & `tmp/karp_lex_types-0.7.1.tar.gz`

## Comparing `karp_lex_types-0.7.0.tar` & `karp_lex_types-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/.bumpversion.toml
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/Makefile
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/cliff.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/mypy.ini
--rw-r--r--   0        0        0    38495 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/pdm.lock
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/ruff.toml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/alias_generators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/py.typed
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/base.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_commands.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_repo_commands.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/commands/resource_commands.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/dtos/__init__.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/dtos/entry_dto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/value_objects/__init__.py
--rw-r--r--   0        0        0     4127 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/src/karp_lex_types/value_objects/unique_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/entry_dto_unit_test.py
--rw-r--r--   0        0        0    15784 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/requirements-testing.lock
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_entry_commands.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_entry_repo_commands.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_resource_commands.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/tests/test_unique_id.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/LICENSE
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/README.md
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/.bumpversion.toml
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/Makefile
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/cliff.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/mypy.ini
+-rw-r--r--   0        0        0    38495 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/pdm.lock
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/ruff.toml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/alias_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/py.typed
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/base.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_commands.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_repo_commands.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/resource_commands.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/dtos/__init__.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/dtos/entry_dto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/value_objects/__init__.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/value_objects/unique_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/entry_dto_unit_test.py
+-rw-r--r--   0        0        0    15784 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_entry_commands.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_entry_repo_commands.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_resource_commands.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_unique_id.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/README.md
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/PKG-INFO
```

### Comparing `karp_lex_types-0.7.0/.bumpversion.toml` & `karp_lex_types-0.7.1/.bumpversion.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.7.0"
+current_version = "0.7.1"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 commit = true
 tag = true
 sign_tag = true
 allow_dirty = false
 message = "chore(release): Bump version: {current_version} → {new_version}"
```

### Comparing `karp_lex_types-0.7.0/CHANGELOG.md` & `karp_lex_types-0.7.1/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.7.1] - 2024-05-22
+
+### Fixed
+
+- Use str to serialize UniqueId
+
 ## [0.7.0] - 2024-05-22
 
 ### Fixed
 
 - Serialize UniuqeId as str
 
 ## [0.6.5] - 2024-05-15
```

### Comparing `karp_lex_types-0.7.0/Makefile` & `karp_lex_types-0.7.1/Makefile`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/cliff.toml` & `karp_lex_types-0.7.1/cliff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/pdm.lock` & `karp_lex_types-0.7.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/ruff.toml` & `karp_lex_types-0.7.1/ruff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/commands/__init__.py` & `karp_lex_types-0.7.1/src/karp_lex_types/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/commands/base.py` & `karp_lex_types-0.7.1/src/karp_lex_types/commands/base.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_commands.py` & `karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/commands/entry_repo_commands.py` & `karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_repo_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/commands/resource_commands.py` & `karp_lex_types-0.7.1/src/karp_lex_types/commands/resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/dtos/entry_dto.py` & `karp_lex_types-0.7.1/src/karp_lex_types/dtos/entry_dto.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/src/karp_lex_types/value_objects/unique_id.py` & `karp_lex_types-0.7.1/src/karp_lex_types/value_objects/unique_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         return json_schema
 
     @classmethod
     def __get_pydantic_core_schema__(  # noqa: D105, PLW3201
         cls, source: typing.Any, handler: GetCoreSchemaHandler
     ) -> core_schema.CoreSchema:
         def _serialize(instance: typing.Any, info: typing.Any) -> typing.Any:
-            return instance.to_string() if info.mode == "json" else instance
+            return str(instance) if info.mode == "json" else instance
 
         from_any_schema = core_schema.chain_schema(
             [
                 core_schema.any_schema(),
                 core_schema.no_info_plain_validator_function(cls.validate),
             ]
         )
```

### Comparing `karp_lex_types-0.7.0/tests/entry_dto_unit_test.py` & `karp_lex_types-0.7.1/tests/entry_dto_unit_test.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/tests/requirements-testing.lock` & `karp_lex_types-0.7.1/tests/requirements-testing.lock`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/tests/test_entry_commands.py` & `karp_lex_types-0.7.1/tests/test_entry_commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -46,7 +46,60 @@
                 "user": "alice@example.com",
             }
         }
 
         cmd = EntryCommand(**data)
 
         assert isinstance(cmd.cmd, UpdateEntry)
+
+
+class TestSerializeEntryCommand:
+    def test_can_serialize_add_entry(self) -> None:  # noqa: PLR6301
+        data = {
+            "cmd": {
+                "cmdtype": "add_entry",
+                "resourceId": "resource_a",
+                "entry": {"baseform": "sko"},
+                "message": "add sko",
+                "user": "alice@example.com",
+            }
+        }
+
+        cmd = EntryCommand(**data)
+
+        assert isinstance(cmd.cmd, AddEntry)
+        cmd.model_dump_json()
+
+    def test_can_serialize_delete_entry(self) -> None:  # noqa: PLR6301
+        data = {
+            "cmd": {
+                "cmdtype": "delete_entry",
+                "resourceId": "resource_a",
+                "id": make_unique_id(),
+                "version": 1,
+                "message": "add sko",
+                "user": "alice@example.com",
+            }
+        }
+
+        cmd = EntryCommand(**data)
+
+        assert isinstance(cmd.cmd, DeleteEntry)
+        cmd.model_dump_json()
+
+    def test_can_serialize_update_entry(self) -> None:  # noqa: PLR6301
+        data = {
+            "cmd": {
+                "cmdtype": "update_entry",
+                "resourceId": "resource_a",
+                "id": make_unique_id(),
+                "entry": {"baseform": "sko"},
+                "version": 1,
+                "message": "add sko",
+                "user": "alice@example.com",
+            }
+        }
+
+        cmd = EntryCommand(**data)
+
+        assert isinstance(cmd.cmd, UpdateEntry)
+        cmd.model_dump_json()
```

### Comparing `karp_lex_types-0.7.0/tests/test_resource_commands.py` & `karp_lex_types-0.7.1/tests/test_resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/tests/test_unique_id.py` & `karp_lex_types-0.7.1/tests/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/.gitignore` & `karp_lex_types-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/LICENSE` & `karp_lex_types-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/README.md` & `karp_lex_types-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.0/pyproject.toml` & `karp_lex_types-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = ["pydantic>=2.5.3", "ulid-py>=1.1.0"]
 name = "karp-lex-types"
-version = "0.7.0"
+version = "0.7.1"
 description = "The types of karp-lex"
 readme = "README.md"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/spraakbanken/karp-lex-types/issues"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/karp-lex-types"
```

### Comparing `karp_lex_types-0.7.0/PKG-INFO` & `karp_lex_types-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: karp-lex-types
-Version: 0.7.0
+Version: 0.7.1
 Summary: The types of karp-lex
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-lex-types/issues
 Project-URL: homepage, https://spraakbanken.gu.se
 Project-URL: repository, https://github.com/spraakbanken/karp-lex-types
 Project-URL: documentation, https://github.com/spraakbanken/karp-lex-types
 Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
```

