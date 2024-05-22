# Comparing `tmp/pypaperless-3.1.6.tar.gz` & `tmp/pypaperless-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaperless-3.1.6.tar", max compression
+gzip compressed data, was "pypaperless-3.1.7.tar", max compression
```

## Comparing `pypaperless-3.1.6.tar` & `pypaperless-3.1.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1070 2024-05-14 18:44:50.373546 pypaperless-3.1.6/LICENSE.md
--rw-r--r--   0        0        0     2605 2024-05-14 18:44:50.373546 pypaperless-3.1.6/README.md
--rw-r--r--   0        0        0     3720 2024-05-14 18:45:01.245530 pypaperless-3.1.6/pyproject.toml
--rw-r--r--   0        0        0       73 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/__init__.py
--rw-r--r--   0        0        0    11483 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/api.py
--rw-r--r--   0        0        0     3876 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/const.py
--rw-r--r--   0        0        0     1741 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/exceptions.py
--rw-r--r--   0        0        0      899 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/helpers.py
--rw-r--r--   0        0        0     1260 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/__init__.py
--rw-r--r--   0        0        0     3724 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/base.py
--rw-r--r--   0        0        0     6788 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/classifiers.py
--rw-r--r--   0        0        0     5891 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/common.py
--rw-r--r--   0        0        0     1500 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/config.py
--rw-r--r--   0        0        0     1654 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/custom_fields.py
--rw-r--r--   0        0        0    19726 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/documents.py
--rw-r--r--   0        0        0       93 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/generators/__init__.py
--rw-r--r--   0        0        0     2112 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/generators/page.py
--rw-r--r--   0        0        0     3041 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mails.py
--rw-r--r--   0        0        0       37 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/__init__.py
--rw-r--r--   0        0        0      288 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/__init__.py
--rw-r--r--   0        0        0     1009 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/callable.py
--rw-r--r--   0        0        0      916 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/draftable.py
--rw-r--r--   0        0        0     2893 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/iterable.py
--rw-r--r--   0        0        0      765 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/securable.py
--rw-r--r--   0        0        0      413 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/__init__.py
--rw-r--r--   0        0        0     2169 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/creatable.py
--rw-r--r--   0        0        0      382 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/data_fields.py
--rw-r--r--   0        0        0      755 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/deletable.py
--rw-r--r--   0        0        0      742 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/securable.py
--rw-r--r--   0        0        0     2641 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/mixins/models/updatable.py
--rw-r--r--   0        0        0     2660 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/pages.py
--rw-r--r--   0        0        0     2201 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/permissions.py
--rw-r--r--   0        0        0     1390 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/saved_views.py
--rw-r--r--   0        0        0     1856 2024-05-14 18:44:50.373546 pypaperless-3.1.6/src/pypaperless/models/share_links.py
--rw-r--r--   0        0        0     1773 2024-05-14 18:44:50.377546 pypaperless-3.1.6/src/pypaperless/models/status.py
--rw-r--r--   0        0        0     2735 2024-05-14 18:44:50.377546 pypaperless-3.1.6/src/pypaperless/models/tasks.py
--rw-r--r--   0        0        0     7307 2024-05-14 18:44:50.377546 pypaperless-3.1.6/src/pypaperless/models/utils/__init__.py
--rw-r--r--   0        0        0     4564 2024-05-14 18:44:50.377546 pypaperless-3.1.6/src/pypaperless/models/workflows.py
--rw-r--r--   0        0        0        0 2024-05-14 18:44:50.377546 pypaperless-3.1.6/src/pypaperless/py.typed
--rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-22 11:19:26.620070 pypaperless-3.1.7/LICENSE.md
+-rw-r--r--   0        0        0     2605 2024-05-22 11:19:26.620070 pypaperless-3.1.7/README.md
+-rw-r--r--   0        0        0     3720 2024-05-22 11:19:37.891985 pypaperless-3.1.7/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/__init__.py
+-rw-r--r--   0        0        0    11483 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/api.py
+-rw-r--r--   0        0        0     3876 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/const.py
+-rw-r--r--   0        0        0     1741 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/exceptions.py
+-rw-r--r--   0        0        0      899 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/helpers.py
+-rw-r--r--   0        0        0     1260 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/__init__.py
+-rw-r--r--   0        0        0     3797 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/base.py
+-rw-r--r--   0        0        0     6766 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/classifiers.py
+-rw-r--r--   0        0        0     5891 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/common.py
+-rw-r--r--   0        0        0     1500 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/config.py
+-rw-r--r--   0        0        0     1654 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/custom_fields.py
+-rw-r--r--   0        0        0    19769 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/documents.py
+-rw-r--r--   0        0        0       93 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/generators/__init__.py
+-rw-r--r--   0        0        0     2112 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/generators/page.py
+-rw-r--r--   0        0        0     3041 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mails.py
+-rw-r--r--   0        0        0       37 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/__init__.py
+-rw-r--r--   0        0        0     1009 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/callable.py
+-rw-r--r--   0        0        0      916 2024-05-22 11:19:26.620070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/draftable.py
+-rw-r--r--   0        0        0     2893 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/iterable.py
+-rw-r--r--   0        0        0      765 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/securable.py
+-rw-r--r--   0        0        0      413 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/__init__.py
+-rw-r--r--   0        0        0     2169 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/creatable.py
+-rw-r--r--   0        0        0      382 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/data_fields.py
+-rw-r--r--   0        0        0      755 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/deletable.py
+-rw-r--r--   0        0        0      742 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/securable.py
+-rw-r--r--   0        0        0     2641 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/mixins/models/updatable.py
+-rw-r--r--   0        0        0     2660 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/pages.py
+-rw-r--r--   0        0        0     2201 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/permissions.py
+-rw-r--r--   0        0        0     1390 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/saved_views.py
+-rw-r--r--   0        0        0     1856 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/share_links.py
+-rw-r--r--   0        0        0     1802 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/status.py
+-rw-r--r--   0        0        0     2735 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/tasks.py
+-rw-r--r--   0        0        0     7307 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/utils/__init__.py
+-rw-r--r--   0        0        0     4564 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/models/workflows.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:19:26.624070 pypaperless-3.1.7/src/pypaperless/py.typed
+-rw-r--r--   0        0        0     3857 1970-01-01 00:00:00.000000 pypaperless-3.1.7/PKG-INFO
```

### Comparing `pypaperless-3.1.6/LICENSE.md` & `pypaperless-3.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/README.md` & `pypaperless-3.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/pyproject.toml` & `pypaperless-3.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.poetry]
 name = "pypaperless"
-version = "3.1.6"
+version = "3.1.7"
 description = "Little api client for paperless(-ngx)."
 authors = ["Tobias Schulz <public.dev@tbsch.de>"]
 maintainers = ["Tobias Schulz <public.dev@tbsch.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tb1337/paperless-api"
 repository = "https://github.com/tb1337/paperless-api"
```

### Comparing `pypaperless-3.1.6/src/pypaperless/api.py` & `pypaperless-3.1.7/src/pypaperless/api.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/const.py` & `pypaperless-3.1.7/src/pypaperless/const.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/exceptions.py` & `pypaperless-3.1.7/src/pypaperless/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/helpers.py` & `pypaperless-3.1.7/src/pypaperless/helpers.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/__init__.py` & `pypaperless-3.1.7/src/pypaperless/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/base.py` & `pypaperless-3.1.7/src/pypaperless/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,22 @@
     _resource_cls: type[ResourceT]
 
 
 class HelperBase(PaperlessBase, Generic[ResourceT]):
     """Base class for all helpers in PyPaperless."""
 
     _resource: PaperlessResource
+    _resource_public: bool = True
 
     def __init__(self, api: "Paperless") -> None:
         """Initialize a `HelperBase` instance."""
         super().__init__(api)
 
-        self._api.local_resources.add(self._resource)
+        if self._resource_public:
+            self._api.local_resources.add(self._resource)
 
     @property
     def is_available(self) -> bool:
         """Return if the attached endpoint is available, or not."""
         return self._resource in self._api.remote_resources
 
 
@@ -68,14 +70,15 @@
 @dataclass(init=False)
 class PaperlessModel(PaperlessBase):
     """Base class for all models in PyPaperless."""
 
     def __init__(self, api: "Paperless", data: dict[str, Any]) -> None:
         """Initialize a `PaperlessModel` instance."""
         super().__init__(api)
+
         self._data = {}
         self._data.update(data)
         self._fetched = False
         self._params: dict[str, Any] = {}
 
     @final
     @classmethod
```

### Comparing `pypaperless-3.1.6/src/pypaperless/models/classifiers.py` & `pypaperless-3.1.7/src/pypaperless/models/classifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,14 @@
     """Represent a new `Tag`, which is not yet stored in Paperless."""
 
     _api_path = API_PATH["tags"]
 
     _create_required_fields = {
         "name",
         "color",
-        "text_color",
         "is_inbox_tag",
         "match",
         "matching_algorithm",
         "is_insensitive",
     }
 
     name: str | None = None
```

### Comparing `pypaperless-3.1.6/src/pypaperless/models/common.py` & `pypaperless-3.1.7/src/pypaperless/models/common.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/config.py` & `pypaperless-3.1.7/src/pypaperless/models/config.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/custom_fields.py` & `pypaperless-3.1.7/src/pypaperless/models/custom_fields.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/documents.py` & `pypaperless-3.1.7/src/pypaperless/models/documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     title: str | None = None
     created: datetime.datetime | None = None
     correspondent: int | None = None
     document_type: int | None = None
     storage_path: int | None = None
     tags: int | list[int] | None = None
     archive_serial_number: int | None = None
+    custom_fields: list[int] | None = None
 
     def _serialize(self) -> dict[str, Any]:
         """Serialize."""
         data = {
             "form": {
                 field.name: object_to_dict_value(getattr(self, field.name))
                 for field in self._get_dataclass_fields()
```

### Comparing `pypaperless-3.1.6/src/pypaperless/models/generators/page.py` & `pypaperless-3.1.7/src/pypaperless/models/generators/page.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mails.py` & `pypaperless-3.1.7/src/pypaperless/models/mails.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/callable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/callable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/draftable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/draftable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/iterable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/iterable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/helpers/securable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/helpers/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/models/creatable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/models/creatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/models/deletable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/models/deletable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/models/securable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/models/securable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/mixins/models/updatable.py` & `pypaperless-3.1.7/src/pypaperless/models/mixins/models/updatable.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/pages.py` & `pypaperless-3.1.7/src/pypaperless/models/pages.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/permissions.py` & `pypaperless-3.1.7/src/pypaperless/models/permissions.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/saved_views.py` & `pypaperless-3.1.7/src/pypaperless/models/saved_views.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/share_links.py` & `pypaperless-3.1.7/src/pypaperless/models/share_links.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/status.py` & `pypaperless-3.1.7/src/pypaperless/models/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 
 class StatusHelper(HelperBase[Status]):
     """Represent a factory for the Paperless `Status` model."""
 
     _api_path = API_PATH["status"]
     _resource = PaperlessResource.STATUS
+    _resource_public = False
 
     _resource_cls = Status
 
     async def __call__(self) -> Status:
         """Request the `Status` model data."""
         res = await self._api.request_json("get", self._api_path)
         return self._resource_cls.create_with_data(self._api, res, fetched=True)
```

### Comparing `pypaperless-3.1.6/src/pypaperless/models/tasks.py` & `pypaperless-3.1.7/src/pypaperless/models/tasks.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/utils/__init__.py` & `pypaperless-3.1.7/src/pypaperless/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/src/pypaperless/models/workflows.py` & `pypaperless-3.1.7/src/pypaperless/models/workflows.py`

 * *Files identical despite different names*

### Comparing `pypaperless-3.1.6/PKG-INFO` & `pypaperless-3.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypaperless
-Version: 3.1.6
+Version: 3.1.7
 Summary: Little api client for paperless(-ngx).
 Home-page: https://github.com/tb1337/paperless-api
 License: MIT
 Keywords: library,async,api-client,python3,paperless-ngx
 Author: Tobias Schulz
 Author-email: public.dev@tbsch.de
 Maintainer: Tobias Schulz
```

