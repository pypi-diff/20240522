# Comparing `tmp/karp_lex_types-0.7.1.tar.gz` & `tmp/karp_lex_types-0.7.2.tar.gz`

## Comparing `karp_lex_types-0.7.1.tar` & `karp_lex_types-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/.bumpversion.toml
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/Makefile
--rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/cliff.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/mypy.ini
--rw-r--r--   0        0        0    38495 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/pdm.lock
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/ruff.toml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/alias_generators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/py.typed
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/__init__.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/base.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_commands.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_repo_commands.py
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/commands/resource_commands.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/dtos/__init__.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/dtos/entry_dto.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/value_objects/__init__.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/src/karp_lex_types/value_objects/unique_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/entry_dto_unit_test.py
--rw-r--r--   0        0        0    15784 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/requirements-testing.lock
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_entry_commands.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_entry_repo_commands.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_resource_commands.py
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/tests/test_unique_id.py
--rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/LICENSE
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/README.md
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/.bumpversion.toml
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/Makefile
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/cliff.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/mypy.ini
+-rw-r--r--   0        0        0    38495 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/pdm.lock
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/ruff.toml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/alias_generators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/py.typed
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/commands/__init__.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/commands/base.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/commands/entry_commands.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/commands/entry_repo_commands.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/commands/resource_commands.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/dtos/__init__.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/dtos/entry_dto.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/value_objects/__init__.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/src/karp_lex_types/value_objects/unique_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/entry_dto_unit_test.py
+-rw-r--r--   0        0        0    15784 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/requirements-testing.lock
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/test_entry_commands.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/test_entry_repo_commands.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/test_resource_commands.py
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/tests/test_unique_id.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/LICENSE
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/README.md
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 karp_lex_types-0.7.2/PKG-INFO
```

### Comparing `karp_lex_types-0.7.1/.bumpversion.toml` & `karp_lex_types-0.7.2/.bumpversion.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.7.1"
+current_version = "0.7.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 commit = true
 tag = true
 sign_tag = true
 allow_dirty = false
 message = "chore(release): Bump version: {current_version} → {new_version}"
```

### Comparing `karp_lex_types-0.7.1/CHANGELOG.md` & `karp_lex_types-0.7.2/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.7.2] - 2024-05-22
+
+### Fixed
+
+- Serialize field with UniqueIds as string
+
 ## [0.7.1] - 2024-05-22
 
 ### Fixed
 
 - Use str to serialize UniqueId
 
 ## [0.7.0] - 2024-05-22
```

### Comparing `karp_lex_types-0.7.1/Makefile` & `karp_lex_types-0.7.2/Makefile`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/cliff.toml` & `karp_lex_types-0.7.2/cliff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/pdm.lock` & `karp_lex_types-0.7.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/ruff.toml` & `karp_lex_types-0.7.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/commands/__init__.py` & `karp_lex_types-0.7.2/src/karp_lex_types/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/commands/base.py` & `karp_lex_types-0.7.2/src/karp_lex_types/commands/base.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/commands/entry_commands.py` & `karp_lex_types-0.7.2/src/karp_lex_types/commands/entry_commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 class GenericAddEntry(Command, Generic[T]):  # noqa: D101
     id: UniqueId = pydantic.Field(default_factory=make_unique_id)
     resource_id: str
     entry: T
     message: str
     cmdtype: Literal["add_entry"] = "add_entry"
 
+    @pydantic.field_serializer("id")
+    def serialize_id(self, id: UniqueId, _info) -> str:  # noqa: PLR6301, A002
+        """Serialize id as string."""
+        return str(id)
+
 
 class AddEntry(GenericAddEntry[dict]):
     """Command to add an entry."""
 
 
 class AddEntries(Command):  # noqa: D101
     resource_id: str
@@ -43,14 +48,19 @@
 class DeleteEntry(Command):  # noqa: D101
     resource_id: str
     id: UniqueId
     version: int
     message: str | None = None
     cmdtype: Literal["delete_entry"] = "delete_entry"
 
+    @pydantic.field_serializer("id")
+    def serialize_id(self, id: UniqueId, _info) -> str:  # noqa: PLR6301, A002
+        """Serialize id as string."""
+        return str(id)
+
 
 class ImportEntries(AddEntries):  # noqa: D101
     pass
 
 
 class ImportEntriesInChunks(AddEntriesInChunks):  # noqa: D101
     pass
@@ -61,14 +71,19 @@
     id: UniqueId
     version: int
     entry: T
     message: str
     force: bool = False
     cmdtype: Literal["update_entry"] = "update_entry"
 
+    @pydantic.field_serializer("id")
+    def serialize_id(self, id: UniqueId, _info) -> str:  # noqa: PLR6301, A002
+        """Serialize id as string."""
+        return str(id)
+
 
 class UpdateEntry(GenericUpdateEntry[dict]):  # noqa: D101
     ...
 
 
 EntryCommandType = Annotated[
     AddEntry | DeleteEntry | UpdateEntry, pydantic.Field(discriminator="cmdtype")
```

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/commands/resource_commands.py` & `karp_lex_types-0.7.2/src/karp_lex_types/commands/resource_commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 T = TypeVar("T")
 
 
 class EntityOrResourceIdMixin(Command):  # noqa: D101
     resource_id: str | None = None
     id: UniqueId | None = None
 
+    @pydantic.field_serializer("id")
+    def serialize_id(self, id: UniqueId, _info) -> str:  # noqa: PLR6301, A002
+        """Serialize id as string."""
+        return str(id)
+
     @pydantic.model_validator(mode="before")
     @classmethod
     def resource_id_or_id(cls, values) -> dict:  # noqa: D102
         resource_id = values.get("resourceId", None)
         if "id" in values and resource_id:
             raise ValueError("Can't give both 'id' and 'resourceId'")
 
@@ -42,14 +47,24 @@
     id: UniqueId = pydantic.Field(default_factory=make_unique_id)
     resource_id: str
     name: str
     config: T
     entry_repo_id: UniqueId
     cmdtype: Literal["create_resource"] = "create_resource"
 
+    @pydantic.field_serializer("id")
+    def serialize_id(self, id: UniqueId, _info) -> str:  # noqa: PLR6301, A002
+        """Serialize id as string."""
+        return str(id)
+
+    @pydantic.field_serializer("entry_repo_id")
+    def serialize_entry_repo_id(self, entry_repo_id: UniqueId, _info) -> str:  # noqa: PLR6301
+        """Serialize id as string."""
+        return str(entry_repo_id)
+
 
 class CreateResource(GenericCreateResource[dict]):
     """Command to create a resource."""
 
     @classmethod
     def from_dict(  # noqa: D102
         cls,
@@ -100,7 +115,12 @@
     cmdtype: Literal["delete_resource"] = "delete_resource"
 
 
 class SetEntryRepoId(EntityOrResourceIdMixin, Command):  # noqa: D101
     entry_repo_id: UniqueId
     version: int
     cmdtype: Literal["set_entry_repo_id"] = "set_entry_repo_id"
+
+    @pydantic.field_serializer("entry_repo_id")
+    def serialize_entry_repo_id(self, entry_repo_id: UniqueId, _info) -> str:  # noqa: PLR6301
+        """Serialize id as string."""
+        return str(entry_repo_id)
```

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/dtos/entry_dto.py` & `karp_lex_types-0.7.2/src/karp_lex_types/dtos/entry_dto.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/src/karp_lex_types/value_objects/unique_id.py` & `karp_lex_types-0.7.2/src/karp_lex_types/value_objects/unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/tests/entry_dto_unit_test.py` & `karp_lex_types-0.7.2/tests/entry_dto_unit_test.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/tests/requirements-testing.lock` & `karp_lex_types-0.7.2/tests/requirements-testing.lock`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/tests/test_entry_commands.py` & `karp_lex_types-0.7.2/tests/test_entry_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/tests/test_resource_commands.py` & `karp_lex_types-0.7.2/tests/test_resource_commands.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/tests/test_unique_id.py` & `karp_lex_types-0.7.2/tests/test_unique_id.py`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/.gitignore` & `karp_lex_types-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/LICENSE` & `karp_lex_types-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/README.md` & `karp_lex_types-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `karp_lex_types-0.7.1/pyproject.toml` & `karp_lex_types-0.7.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
 ]
 license = { text = "MIT" }
 requires-python = ">=3.10"
 dependencies = ["pydantic>=2.5.3", "ulid-py>=1.1.0"]
 name = "karp-lex-types"
-version = "0.7.1"
+version = "0.7.2"
 description = "The types of karp-lex"
 readme = "README.md"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/spraakbanken/karp-lex-types/issues"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/karp-lex-types"
```

### Comparing `karp_lex_types-0.7.1/PKG-INFO` & `karp_lex_types-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: karp-lex-types
-Version: 0.7.1
+Version: 0.7.2
 Summary: The types of karp-lex
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-lex-types/issues
 Project-URL: homepage, https://spraakbanken.gu.se
 Project-URL: repository, https://github.com/spraakbanken/karp-lex-types
 Project-URL: documentation, https://github.com/spraakbanken/karp-lex-types
 Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
```

