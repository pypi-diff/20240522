# Comparing `tmp/apiiif-0.2.5.tar.gz` & `tmp/apiiif-0.3.0.tar.gz`

## Comparing `apiiif-0.2.5.tar` & `apiiif-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.2.5/.vscode/settings.json
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.2.5/src/apiiif/__about__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.2.5/src/apiiif/__init__.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 apiiif-0.2.5/src/apiiif/factory.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 apiiif-0.2.5/src/apiiif/resource_properties.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 apiiif-0.2.5/src/apiiif/resource_types.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.2.5/.gitignore
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.2.5/LICENSE.txt
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.2.5/README.md
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 apiiif-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 apiiif-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 apiiif-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/log.txt
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/apiiif/__about__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/apiiif/__init__.py
+-rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/apiiif/factory.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/apiiif/resource_properties.py
+-rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 apiiif-0.3.0/src/apiiif/resource_types.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 apiiif-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 apiiif-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 apiiif-0.3.0/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 apiiif-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 apiiif-0.3.0/PKG-INFO
```

### Comparing `apiiif-0.2.5/src/apiiif/factory.py` & `apiiif-0.3.0/src/apiiif/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from apiiif.resource_properties import (
+from ..apiiif.resource_properties import (
     LanguageString,
     LabelValue,
     Thumbnail,
     Logo,
     Homepage,
     PartOf,
     Provider,
     Choice,
     ImageService,
     ExternalAuthService,
 )
-from apiiif.resource_types import (
+from ..apiiif.resource_types import (
     Collection,
     Manifest,
     Canvas,
     Annotation,
     IIIFImage,
     AnnotationPage,
 )
@@ -137,21 +137,21 @@
             width=width,
             height=height,
             service=[self.imageService(iiif_root_url, additional_services)],
         )
 
     def external_auth_service(
         self,
-        _id: str,
+        iiif_id: str,
         label: str,
         failure_header: str,
         failure_description: str,
     ):
         return ExternalAuthService(
-            _id=_id,
+            iiif_id=iiif_id,
             label=self.langugae_string(label),
             failureHeader=self.langugae_string(failure_header),
             failureDescription=self.langugae_string(failure_description),
         )
 
     def annotation_page(
         self,
```

### Comparing `apiiif-0.2.5/src/apiiif/resource_properties.py` & `apiiif-0.3.0/src/apiiif/resource_properties.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from multiprocessing import context
-from pydantic import BaseModel, AnyUrl, root_validator, validator, Field
+from pydantic import field_validator, model_validator, BaseModel, AnyUrl, Field
 
 
 class BaseID(BaseModel):
 
-    @validator("id", pre=True)
+    @field_validator("id", mode="before")
     def slugify(s):
         if isinstance(s, str):
             return s.replace(" ", "%20")
         return s
 
     id: AnyUrl
 
 
 class LanguageString(BaseModel):
     """A language string is a dictionary with language codes as keys and
     strings as values. The language codes are ISO 2-character codes.
     Add additional languages as needed, but once more than one exists,
     logic is needed to enable all to be optional, but one must be declared."""
 
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def check_language_string(cls, values):
         if len(values) == 0:
             raise ValueError("At least one language string must be provided.")
         return values
 
-    en: list[str] | None
-    fr: list[str] | None
-    de: list[str] | None
-    it: list[str] | None
-    es: list[str] | None
+    en: list[str] | None = None
+    fr: list[str] | None = None
+    de: list[str] | None = None
+    it: list[str] | None = None
+    es: list[str] | None = None
 
 
 class LabelValue(BaseModel):
     """Used as the value of the requiredStatement and metadata items."""
 
     label: LanguageString
     value: LanguageString
 
 
 class Image(BaseID):
     type: str = "Image"
-    width: int | None
-    height: int | None
+    width: int | None = None
+    height: int | None = None
 
 
 class Thumbnail(Image):
     format: str = "image/jpeg"
 
 
 class Logo(Image):
@@ -63,27 +63,27 @@
 class PartOf(BaseID):
     type: str = "Collection"
 
 
 class Provider(BaseID):
     type: str = "Agent"
     label: LanguageString
-    homepage: list[Homepage] | None
-    logo: list[Logo] | None
+    homepage: list[Homepage] | None = None
+    logo: list[Logo] | None = None
 
 
 class Choice(BaseModel):
     type: str = "Choice"
     items: list = []
 
 
 class ExternalAuthService(BaseModel):
-    _id: AnyUrl = Field(alias="@id")
+    iiif_id: AnyUrl = Field(serialization_alias="@id")
     context: str = Field(
-        default="http://iiif.io/api/auth/1/context.json", alias="@context"
+        default="http://iiif.io/api/auth/1/context.json", serialization_alias="@context"
     )
     profile: str = "http://iiif.io/api/auth/1/external"
     label: LanguageString
     failureHeader: LanguageString
     failureDescription: LanguageString
```

### Comparing `apiiif-0.2.5/src/apiiif/resource_types.py` & `apiiif-0.3.0/src/apiiif/resource_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pydantic import BaseModel, AnyUrl, Field
 
-from apiiif.resource_properties import (
+from ..apiiif.resource_properties import (
     LanguageString,
     LabelValue,
     Provider,
     Thumbnail,
     Homepage,
     PartOf,
     Image,
@@ -51,15 +51,15 @@
 
 
 class Canvas(BaseID):
     type: str = "Canvas"
     label: LanguageString
     height: int
     width: int
-    behavior: list[str] | None  # ['paged'], ['facing-pages'], ['non-paged']
+    behavior: list[str] | None = None  # ['paged'], ['facing-pages'], ['non-paged']
     items: list = []
 
     def add_annotation_page(self, annotation_page: AnnotationPage):
         self.items.append(annotation_page)
 
 
 # Range should be defined here, but the collections site does not yet support it.
@@ -71,34 +71,34 @@
 class Manifest(BaseID):
     context: str = Field(
         default="http://iiif.io/api/presentation/3/context.json", alias="@context"
     )
     type: str = "Manifest"
     label: LanguageString
     metadata: list[LabelValue] = []
-    summary: LanguageString | None
-    thumbnail: Thumbnail | None
+    summary: LanguageString | None = None
+    thumbnail: Thumbnail | None = None
     viewingDirection: str = "left-to-right"
     behavior: list[str] = ["paged"]
-    rights: AnyUrl | str | None
-    requiredStatement: LabelValue | None
-    provider: list[Provider] | None
-    homepage: Homepage | None
-    partOf: PartOf | None
+    rights: AnyUrl | str | None = None
+    requiredStatement: LabelValue | None = None
+    provider: list[Provider] | None = None
+    homepage: Homepage | None = None
+    partOf: PartOf | None = None
     items: list = []
     services: list[ExternalAuthService] = []
 
     def add_canvas(self, canvas: Canvas):
         self.items.append(canvas)
 
 
 class Collection(BaseID):
     context: str = Field(
         default="http://iiif.io/api/presentation/3/context.json", alias="@context"
     )
     type: str = "Collection"
     label: LanguageString
-    requiredStatement: LabelValue | None
+    requiredStatement: LabelValue | None = None
     items: list = []
 
     def add_manifest(self, manifest: Manifest):
         self.items.append(manifest)
```

### Comparing `apiiif-0.2.5/.gitignore` & `apiiif-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.5/LICENSE.txt` & `apiiif-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.5/README.md` & `apiiif-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `apiiif-0.2.5/pyproject.toml` & `apiiif-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "pydantic==1.10.8",
+  "pydantic==2.7.1",
 ]
 description = ''
 dynamic = ["version"]
 keywords = []
 license = "MIT"
 name = "apiiif"
 readme = "README.md"
```

### Comparing `apiiif-0.2.5/PKG-INFO` & `apiiif-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: apiiif
-Version: 0.2.5
+Version: 0.3.0
 Project-URL: Documentation, https://github.com/d-flood/apiiif#readme
 Project-URL: Issues, https://github.com/d-flood/apiiif/issues
 Project-URL: Source, https://github.com/d-flood/apiiif
 Author-email: David Flood <d-flood@users.noreply.github.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
-Requires-Dist: pydantic==1.10.8
+Requires-Dist: pydantic==2.7.1
 Description-Content-Type: text/markdown
 
 # apiiif
 
 [![PyPI - Version](https://img.shields.io/pypi/v/apiiif.svg)](https://pypi.org/project/apiiif)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/apiiif.svg)](https://pypi.org/project/apiiif)
```

