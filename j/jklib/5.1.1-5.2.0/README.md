# Comparing `tmp/jklib-5.1.1.tar.gz` & `tmp/jklib-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jklib-5.1.1.tar", last modified: Sat May  4 16:57:54 2024, max compression
+gzip compressed data, was "jklib-5.2.0.tar", last modified: Wed May 22 13:51:39 2024, max compression
```

## Comparing `jklib-5.1.1.tar` & `jklib-5.2.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-04 16:57:43.000000 jklib-5.1.1/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 16:57:54.144989 jklib-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-04 16:57:43.000000 jklib-5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.136989 jklib-5.1.1/jklib/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4919 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/dj/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/meili/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.140989 jklib-5.1.1/jklib/meili/dj/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5807 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/indexer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7773 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/dj/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/meili/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/jklib/std/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/threads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-04 16:57:43.000000 jklib-5.1.1/jklib/std/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 16:57:54.144989 jklib-5.1.1/jklib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-04 16:57:54.000000 jklib-5.1.1/jklib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 16:57:54.144989 jklib-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-04 16:57:43.000000 jklib-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.269704 jklib-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 13:51:31.000000 jklib-5.2.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 13:51:39.269704 jklib-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-22 13:51:31.000000 jklib-5.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.261704 jklib-5.2.0/jklib/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.265704 jklib-5.2.0/jklib/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4964 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/dj/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.265704 jklib-5.2.0/jklib/meili/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.265704 jklib-5.2.0/jklib/meili/dj/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/dj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/dj/indexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/dj/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7870 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/dj/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/meili/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.269704 jklib-5.2.0/jklib/std/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/threads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-22 13:51:31.000000 jklib-5.2.0/jklib/std/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:51:39.269704 jklib-5.2.0/jklib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-22 13:51:39.000000 jklib-5.2.0/jklib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-22 13:51:39.000000 jklib-5.2.0/jklib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:51:39.000000 jklib-5.2.0/jklib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 13:51:39.000000 jklib-5.2.0/jklib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:51:39.269704 jklib-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-22 13:51:31.000000 jklib-5.2.0/setup.py
```

### Comparing `jklib-5.1.1/LICENCE.txt` & `jklib-5.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `jklib-5.1.1/jklib/dj/admin.py` & `jklib-5.2.0/jklib/dj/admin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Built-in
 from typing import Optional
 
-# Django
 from django.db.models import Model
 from django.http.request import HttpRequest
 
 
 class ReadOnlyAdminMixin:
     """Disables all admin actions for a model."""
```

### Comparing `jklib-5.1.1/jklib/dj/emails.py` & `jklib-5.2.0/jklib/dj/emails.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-# Built-in
 from threading import Thread
 from typing import Any, Dict, List, Optional
 
-# Django
 from django.conf import settings
 from django.core.mail import EmailMessage
 
-# Application
 from jklib.dj.templates import render_template
 
 
 class Email:
     """Sends async/sync emails through Django using templates and contexts."""
 
     def __init__(
```

### Comparing `jklib-5.1.1/jklib/dj/exceptions.py` & `jklib-5.2.0/jklib/dj/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Django
 from django.utils.translation import gettext_lazy as _
 from rest_framework.exceptions import APIException
 from rest_framework.status import HTTP_409_CONFLICT, HTTP_412_PRECONDITION_FAILED
 
 
 class Conflict(APIException):
     """Classic '409 Conflict' HTTP error."""
```

### Comparing `jklib-5.1.1/jklib/dj/files.py` & `jklib-5.2.0/jklib/dj/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Built-in
-import zipfile
 from io import BytesIO
 from urllib.parse import urlparse
+import zipfile
 
-# Django
 from django.core.files.storage import Storage
 from django.http import HttpResponse, StreamingHttpResponse
 
 
 def download_file(path: str, storage: Storage) -> StreamingHttpResponse:
     """Downloads a file from a storage backend."""
     filename = urlparse(path).path.split("/").pop()
```

### Comparing `jklib-5.1.1/jklib/dj/images.py` & `jklib-5.2.0/jklib/dj/images.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-# Built-in
 from io import BytesIO
 from pathlib import Path
 
-# Third-party
-from PIL import Image
-
-# Django
 from django.core.files import File
 from django.db.models import ImageField
 
+# Third-party
+from PIL import Image
+
 IMAGE_TYPES = {
     "jpg": "JPEG",
     "jpeg": "JPEG",
     "png": "PNG",
     "gif": "GIF",
     "tif": "TIFF",
     "tiff": "TIFF",
```

### Comparing `jklib-5.1.1/jklib/dj/managers.py` & `jklib-5.2.0/jklib/dj/managers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# Built-in
 from typing import Iterable, List, Optional, Sequence
 
-# Django
 from django.db.models import Manager, Model, QuerySet
 
 
 class ImprovedManager(Manager):
     def __init__(
         self,
         allow_bulk: bool = True,
         select_related: Optional[Iterable[str]] = None,
         prefetch_related: Optional[Iterable[str]] = None,
     ):
         super().__init__()
         self.allow_bulk = allow_bulk
-        self.select_related = select_related or []
-        self.prefetch_related = prefetch_related or []
+        self.select_related = select_related or []  # type: ignore
+        self.prefetch_related = prefetch_related or []  # type: ignore
 
-    def bulk_create(
+    def bulk_create(  # type: ignore
         self,
         objs: Iterable,
         batch_size: Optional[int] = None,
         ignore_conflicts: bool = False,
     ) -> List:
         if not self.allow_bulk:
             raise NotImplementedError
@@ -33,11 +31,11 @@
         if not self.allow_bulk:
             raise NotImplementedError
         return super().bulk_update(objs, fields, batch_size)
 
     def get_queryset(self) -> QuerySet["Model"]:
         queryset = super().get_queryset()
         if self.select_related:
-            queryset = queryset.select_related(*self.select_related)
+            queryset = queryset.select_related(*self.select_related)  # type: ignore
         if self.prefetch_related:
-            queryset = queryset.prefetch_related(*self.prefetch_related)
+            queryset = queryset.prefetch_related(*self.prefetch_related)  # type: ignore
         return queryset
```

### Comparing `jklib-5.1.1/jklib/dj/models.py` & `jklib-5.2.0/jklib/dj/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Built-in
 import os
-import uuid
 from typing import Any, List, Optional, Type
+import uuid
 
-# Django
 from django import forms
 from django.db import IntegrityError, models
 from django.utils.deconstruct import deconstructible
 
 
 class ImprovedModel(models.Model):
     class Meta:
@@ -53,16 +51,14 @@
             self.full_clean()
         except forms.ValidationError as e:
             raise IntegrityError(e)
         except Exception as e:
             raise e
 
 
-
-
 @deconstructible
 class FileNameWithUUID(object):
     """Generates a unique file name with a UUID."""
 
     def __init__(self, path: str) -> None:
         self.path = os.path.join(path, "%s%s")
```

### Comparing `jklib-5.1.1/jklib/dj/network.py` & `jklib-5.2.0/jklib/dj/network.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Django
 from django.conf import settings
 from django.http import HttpRequest
 
 
 def get_client_ip(request: HttpRequest) -> str:
     """Gets the client IP address from the request."""
     if request.META.get("HTTP_X_FORWARDED_FOR"):
```

### Comparing `jklib-5.1.1/jklib/dj/permissions.py` & `jklib-5.2.0/jklib/dj/permissions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Django
 from rest_framework.permissions import BasePermission, IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.views import APIView
 
 
 class BlockAll(BasePermission):
     """Blocks all requests."""
```

### Comparing `jklib-5.1.1/jklib/dj/serializers.py` & `jklib-5.2.0/jklib/dj/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Built-in
 from typing import Any, Dict
 
-# Django
 from django.conf import settings
 from django.db.models import Model
 from rest_framework import serializers
 
 # Application
 from jklib.std.images import resized_image_to_base64
 
@@ -19,9 +17,9 @@
     def update(self, instance: Model, validated_data: Dict[str, Any]) -> Model:
         raise NotImplementedError
 
 
 class ThumbnailField(serializers.ImageField):
     """A `serializers.ImageField` that returns a thumbnail."""
 
-    def to_representation(self, data: serializers.ImageField) -> bytes:
-        return resized_image_to_base64(data, settings.MAX_THUMBNAIL_SIZE)
+    def to_representation(self, data: serializers.ImageField) -> bytes:  # type: ignore
+        return resized_image_to_base64(data, settings.MAX_THUMBNAIL_SIZE)  # type: ignore
```

### Comparing `jklib-5.1.1/jklib/dj/test_runner.py` & `jklib-5.2.0/jklib/dj/test_runner.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Built-in
 import re
 from time import perf_counter
-from typing import Dict, List, Optional
+from typing import Any, Dict, List, Optional
 from unittest import TestResult, TextTestResult, TextTestRunner
 
-# Django
 from django.test import runner
 
 # Terminal Colors
 ERROR_COLOR = "\033[91m"
 SUCCESS_COLOR = "\033[92m"
 FAILURE_COLOR = "\033[93m"
 ENDC_COLOR = "\033[0m"
@@ -18,17 +17,17 @@
     """Represents a test result with its name, result, and execution time."""
 
     DEFAULT_SYMBOL = "?"
     SUCCESS_SYMBOL = "."
     ERROR_SYMBOL = "E"
     FAILURE_SYMBOL = "F"
 
-    def __init__(self, test) -> None:
+    def __init__(self, test: Any) -> None:
         self.test = test
-        match = re.match("^(.+) \((.+)\)$", str(test))  # noqa: W605
+        match = re.match("^(.+) \((.+)\)$", str(test))  # noqa
         self.app: str = match.group(2).split(".")[0]
         self.case: str = match.group(2).split(".")[-1]
         self.test_name: str = match.group(1)
         self.start: float = perf_counter()
         self.end: Optional[float] = None
         self.symbol: str = self.DEFAULT_SYMBOL
 
@@ -64,34 +63,34 @@
         self.end = perf_counter()
 
 
 class TimedTextTestResult(TextTestResult):
     """Extends TextTestResult to track execution time of each test and print
     them."""
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super(TimedTextTestResult, self).__init__(*args, **kwargs)
         self.clocks: Dict[str, Result] = dict()
         self.unknown_errors: List[Result] = []
 
-    def startTest(self, test) -> None:
+    def startTest(self, test: Any) -> None:
         self.clocks[f"{test}"] = Result(test)
         super().startTest(test)
 
-    def addError(self, test, err) -> None:
+    def addError(self, test: Any, err: Any) -> None:
         result = self._get_result(test)
         result.set_error()
         super().addError(test, err)
 
-    def addFailure(self, test, err) -> None:
+    def addFailure(self, test: Any, err: Any) -> None:
         result = self._get_result(test)
         result.set_failure()
         super().addFailure(test, err)
 
-    def addSuccess(self, test) -> None:
+    def addSuccess(self, test: Any) -> None:
         result = self._get_result(test)
         result.set_success()
         super().addSuccess(test)
 
     def show_execution_times(self) -> None:
         results = self.clocks.values()
         max_app_length = max([len(r.app) for r in results]) + 2
@@ -121,15 +120,15 @@
             f"\n{ERROR_COLOR}"
             f"The test run also encountered some unexpected issues in:"
             f"{ENDC_COLOR}"
         )
         for result in self.unknown_errors:
             print(f"\t{FAILURE_COLOR}{result.test}{ENDC_COLOR}")
 
-    def _get_result(self, test) -> Result:
+    def _get_result(self, test: Any) -> Result:
         """We might end up with an unknown key when crashing in a setUpClass
         method All its tests will be ignored, but to avoid crashing, we create
         a test result on the fly And store that result in the unknown errors
         list."""
         result = self.clocks.get(f"{test}")
         if result is None:
             result = Result(test)
@@ -138,15 +137,15 @@
 
 
 class TimedTextTestRunner(TextTestRunner):
     """Extend TextTestRunner to show the execution times at the end."""
 
     resultclass = TimedTextTestResult
 
-    def run(self, test) -> TestResult:
+    def run(self, test: Any) -> TestResult:
         result = super().run(test)
         result.show_execution_times()
         result.show_unknown_errors()
         print()
         return result
```

### Comparing `jklib-5.1.1/jklib/dj/tests.py` & `jklib-5.2.0/jklib/dj/tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,211 +1,203 @@
-# Built-in
 import datetime
-import json
 from io import BytesIO
+import json
 from typing import (
     TYPE_CHECKING,
     Any,
     ByteString,
     Callable,
     Dict,
     Iterable,
     List,
+    Mapping,
     Optional,
+    OrderedDict,
     Type,
-    Union, OrderedDict,
+    Union,
 )
-from unittest.mock import Mock
 from urllib.parse import urlencode
 from zipfile import ZipFile
 
-# Django
 from django.contrib.sessions.models import Session
 from django.core import mail
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.db import IntegrityError
 from django.db.models import FileField, ImageField, Model, QuerySet
 from django.http import StreamingHttpResponse
 from django.test import RequestFactory, TestCase
 from django.test.client import BOUNDARY, MULTIPART_CONTENT, encode_multipart
 from django.utils import timezone
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.reverse import reverse
 from rest_framework.test import APIClient
 
-# Application
 from jklib.std.images import image_to_base64, resized_image_to_base64
 from jklib.std.transforms import dict_to_flat_dict
 
 if TYPE_CHECKING:
-    # Django
     from django.contrib.auth.models import User as UserType
 
 CONTENT_DISPOSITION = 'attachment; filename="{file_name}"'
 
 
 def assert_logs(logger: str, level: str) -> Callable:
     """Wraps a test into a `self.assertLogs`."""
     level = level.upper()
 
     def decorator(function: Callable) -> Callable:
-        def wrapper(self: TestCase, *args, **kwargs) -> Any:
+        def wrapper(self: TestCase, *args: Any, **kwargs: Any) -> Any:
             with self.assertLogs(logger=logger, level=level) as context:
                 self.logger_context = context
                 return function(self, *args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 class AssertionTestCase(TestCase):
     """A `TestCase` with some assertion methods."""
 
     def assertDictEqual(
-            self,
-            d1: Union[Dict, OrderedDict],
-            d2: Union[Dict, OrderedDict],
-            msg: Optional[str] = None,
-    ):
+        self,
+        d1: Mapping[Any, object],
+        d2: Mapping[Any, object],
+        msg: Optional[str] = None,
+    ) -> None:
         """Overrides `assertDictEqual` to handle `OrderedDict` instances."""
         if isinstance(d1, OrderedDict):
             d1 = dict(d1)
         if isinstance(d2, OrderedDict):
             d2 = dict(d2)
         super().assertDictEqual(d1, d2, msg)
 
     def assertDateEqualsString(
-            self,
-            instance_date: Optional[Union[datetime.datetime, datetime.date]],
-            string_date: Optional[str],
-            format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%fZ",
-    ):
+        self,
+        instance_date: Optional[Union[datetime.datetime, datetime.date]],
+        string_date: Optional[str],
+        format: Optional[str] = "%Y-%m-%dT%H:%M:%S.%fZ",
+    ) -> None:
         if not instance_date:
             self.assertIsNone(string_date)
         else:
             self.assertEqual(instance_date.strftime(format), string_date)
 
     def assertDownloadFile(self, response: Response, file_name: str) -> None:
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             response.get("Content-Disposition"),
             CONTENT_DISPOSITION.format(file_name=file_name),
         )
 
     def assertDownloadZipFile(
-            self, response: Response, file_name: str, zip_content: List[str]
+        self, response: Response, file_name: str, zip_content: List[str]
     ) -> None:
         self.assertEqual(response.status_code, 200)
         self.assertEqual(
             response.get("Content-Disposition"),
             CONTENT_DISPOSITION.format(file_name=file_name),
         )
         # Check the zip content
         myzip = ZipFile(BytesIO(response.getvalue()))
         zipped_files = set(myzip.namelist())
         self.assertSetEqual(set(zip_content), zipped_files)
 
     def assertEmailWasSent(
-            self,
-            subject: str,
-            to: Optional[List[str]] = None,
-            cc: Optional[List[str]] = None,
-            bcc: Optional[List[str]] = None,
+        self,
+        subject: str,
+        to: Optional[List[str]] = None,
+        cc: Optional[List[str]] = None,
+        bcc: Optional[List[str]] = None,
     ) -> None:
         email = mail.outbox[-1]
         self.assertEqual(email.subject, subject)
         if to is not None:
             self.assertEqual(len(to), len(email.to))
             self.assertSetEqual(set(to), set(email.to))
         if cc is not None:
             self.assertEqual(len(cc), len(email.cc))
             self.assertSetEqual(set(cc), set(email.cc))
         if bcc is not None:
             self.assertEqual(len(bcc), len(email.bcc))
             self.assertSetEqual(set(bcc), set(email.bcc))
 
     def assertFieldsHaveError(
-            self,
-            response: Response,
-            key_paths: List[str],
+        self,
+        response: Response,
+        key_paths: List[str],
     ) -> None:
         self.assertEqual(response.status_code, 400)
         for key_path in key_paths:
             # key_path example: "valves.0.description"
             value = response.data
             for key in key_path.split("."):
                 if isinstance(value, list):
                     value = value[int(key)]
                 else:
                     value = value.get(key)
             self.assertIsNotNone(value)
 
     def assertFileEqual(
-            self,
-            file_1: Union[FileField, SimpleUploadedFile],
-            file_2: Union[FileField, SimpleUploadedFile],
+        self,
+        file_1: Union[FileField, SimpleUploadedFile],
+        file_2: Union[FileField, SimpleUploadedFile],
     ) -> None:
         # Reset cursor position to make sure we compare the whole file
-        file_1.seek(0)
-        file_2.seek(0)
+        file_1.seek(0)  # type: ignore
+        file_2.seek(0)  # type: ignore
         # .read() must be stored within variable or it won't work
-        content_1 = file_1.read()
-        content_2 = file_2.read()
+        content_1 = file_1.read()  # type: ignore
+        content_2 = file_2.read()  # type: ignore
         self.assertEqual(content_1, content_2)
 
     def assertFileIsNone(self, file_field: FileField) -> None:
         self.assertFalse(bool(file_field))
 
     def assertImageToBase64(
-            self, img: ImageField, data: ByteString, resize_to: Optional[int] = None
-    ):
+        self, img: ImageField, data: ByteString, resize_to: Optional[int] = None
+    ) -> None:
         converted_image = (
-            resized_image_to_base64(img, resize_to)
+            resized_image_to_base64(img, resize_to)  # type: ignore
             if resize_to is not None
-            else image_to_base64(img)
+            else image_to_base64(img)  # type: ignore
         )
         self.assertEqual(converted_image, data)
 
     def assertIntegrityErrorOnSave(self, instance: Model) -> None:
         with self.assertRaises(IntegrityError):
             instance.save()
 
     def assertQuerySetPks(
-            self, queryset: QuerySet, expected_pks=Iterable[Any], pk="id"
+        self, queryset: QuerySet, expected_pks: Iterable[Any], pk: str = "id"
     ) -> None:
         queryset_pks = {getattr(item, pk) for item in queryset}
         self.assertSetEqual(queryset_pks, set(expected_pks))
 
-    def assertMockCalls(self, mock: Mock, expected_args: List) -> None:
-        self.assertEqual(len(mock.call_args_list), len(expected_args))
-        for (args, _kwargs), expected in zip(mock.call_args_list, expected_args):
-            self.assertEqual(args, expected)
-
 
 class ImprovedTestCase(AssertionTestCase):
     """Base TestCase with additional assertions and methods."""
 
     @staticmethod
     def build_fake_request(
-            method: str = "get", path: str = "/", data: Dict = None
+        method: str = "get", path: str = "/", data: Dict = None
     ) -> Request:
         factory = RequestFactory()
         factory_call = getattr(factory, method.lower())
         return factory_call(path, data=data)
 
     @staticmethod
     def generate_non_existing_id(model: Type[Model]) -> Any:
         instance = model.objects.all().order_by("-id").first()
         return 1 if not instance else instance.id + 1
 
     @staticmethod
     def uploaded_file_from_path(
-            filepath: str, upload_name: Optional[str] = None
+        filepath: str, upload_name: Optional[str] = None
     ) -> SimpleUploadedFile:
         if upload_name is None:
             upload_name = filepath.split("/")[-1]
         with open(filepath, "rb") as f:
             binary_content = f.read()
         return SimpleUploadedFile(
             name=upload_name,
@@ -223,17 +215,17 @@
     @classmethod
     def setUpClass(cls) -> None:
         cls.api_client = cls.api_client_class()
         super().setUpClass()
 
     @staticmethod
     def build_url(
-            name: str,
-            kwargs: Optional[Dict] = None,
-            query_kwargs: Optional[Dict] = None,
+        name: str,
+        kwargs: Optional[Dict] = None,
+        query_kwargs: Optional[Dict] = None,
     ) -> str:
         url = reverse(name, kwargs=kwargs)
         if query_kwargs is not None:
             url += f"?{urlencode(query_kwargs)}"
         return url
 
     @staticmethod
@@ -245,23 +237,23 @@
             if session.get_decoded().get("_auth_user_id") == str(user.pk):
                 user_active_session_ids.append(session.pk)
         if len(user_active_session_ids) > 0:
             Session.objects.filter(pk__in=user_active_session_ids).delete()
 
     @staticmethod
     def parse_streaming_response(response: StreamingHttpResponse) -> Union[Dict, List]:
-        return json.loads(b"".join(response.streaming_content).decode("utf-8"))
+        return json.loads(b"".join(response.streaming_content).decode("utf-8"))  # type: ignore
 
     def multipart_api_call(
-            self,
-            method: str,
-            url: str,
-            payload: Dict[str, Any],
-            *args: Any,
-            **kwargs: Any,
+        self,
+        method: str,
+        url: str,
+        payload: Dict[str, Any],
+        *args: Any,
+        **kwargs: Any,
     ) -> Response:
         """Transforms a JSON payload into a flattened form-data and performs a
         multipart request."""
         flat_dict = dict_to_flat_dict(payload)
         data = encode_multipart(data=flat_dict, boundary=BOUNDARY)
         method = getattr(self.api_client, method.lower())
-        return method(url, data=data, content_type=MULTIPART_CONTENT, *args, **kwargs)
+        return method(url, data=data, content_type=MULTIPART_CONTENT, *args, **kwargs)  # type: ignore
```

### Comparing `jklib-5.1.1/jklib/dj/validators.py` & `jklib-5.2.0/jklib/dj/validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Built-in
 from typing import Optional
 
-# Django
 from django.core.exceptions import ValidationError
 from django.utils.deconstruct import deconstructible
 
 
 @deconstructible
 class LengthValidator:
     """Validates the length of a string."""
```

### Comparing `jklib-5.1.1/jklib/dj/viewsets.py` & `jklib-5.2.0/jklib/dj/viewsets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Built-in
 from typing import Any, Dict, Generator, List, Optional, Sequence, Type
 
-# Django
 from django.db.models import QuerySet
 from rest_framework import mixins
 from rest_framework.permissions import BasePermission
 from rest_framework.renderers import JSONRenderer
 from rest_framework.serializers import BaseSerializer, Serializer
 from rest_framework.settings import api_settings
 from rest_framework.viewsets import GenericViewSet
@@ -32,15 +30,15 @@
     serializer_class_per_action: Dict[str, Type[BaseSerializer]] = {}
 
     def get_permissions(self) -> List[BasePermission]:
         permissions = self.permission_classes_per_action.get(
             self.action, self.default_permission_classes
         )
         if len(permissions) == 0:
-            permissions = api_settings.DEFAULT_PERMISSION_CLASSES
+            permissions = api_settings.DEFAULT_PERMISSION_CLASSES  # type: ignore
         return [permission() for permission in permissions]
 
     def get_serializer_class(self) -> Type[BaseSerializer]:
         return self.serializer_class_per_action.get(
             self.action, self.default_serializer_class
         )
 
@@ -52,15 +50,15 @@
     def generate_json_streaming_content(
         self,
         queryset: QuerySet,
         serializer_class: Optional[Type[Serializer]] = None,
         context: Optional[Dict[str, Any]] = None,
     ) -> Generator[bytes, None, None]:
         """Generates a JSON streaming response as bytes from a queryset."""
-        serializer_class = serializer_class or self.get_serializer_class()
+        serializer_class = serializer_class or self.get_serializer_class()  # type: ignore
         context = context or self.get_serializer_context()
         renderer = JSONRenderer()
         total = queryset.count()
         # Manually adds [] and , to the response to make it a valid JSON array
         for i, item in enumerate(queryset):
             data = b""
             if i == 0:
```

### Comparing `jklib-5.1.1/jklib/meili/dj/indexer.py` & `jklib-5.2.0/jklib/meili/dj/indexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,36 @@
-# Built-in
 from abc import ABC, abstractmethod
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     Generic,
     List,
     Optional,
     Type,
     TypeVar,
     Union,
     Unpack,
 )
 
-# Third-party
-from meilisearch import Client
-
-# Django
 from django.conf import settings
 from django.core.paginator import Paginator
 from django.db.models import Q, QuerySet
+from meilisearch import Client
 
-# Application
 from jklib.meili.search import build_search_filter
 from jklib.meili.types import (
     MeilisearchFilters,
     MeilisearchSearchHits,
     MeilisearchSearchParameters,
     MeilisearchSearchResults,
     MeilisearchSettings,
 )
 
 if TYPE_CHECKING:
-    # Django
     from django.db.models import Model
 
 
 M = TypeVar("M", bound="Model")
 
 
 class MeilisearchModelIndexer(ABC, Generic[M]):
```

### Comparing `jklib-5.1.1/jklib/meili/dj/serializers.py` & `jklib-5.2.0/jklib/meili/dj/serializers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Django
 from rest_framework import serializers
 
 
 class MeilisearchSimpleSearchSerializer(serializers.Serializer):
     query = serializers.CharField(max_length=255, required=True, allow_blank=False)
```

### Comparing `jklib-5.1.1/jklib/meili/dj/test_utils.py` & `jklib-5.2.0/jklib/meili/dj/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,16 @@
-# Built-in
 from time import sleep
-from typing import Generic, Type, TypeVar
+from typing import Dict, Generic, List, Type, TypeVar
 
-# Third-party
-from meilisearch import Client
-
-# Django
 from django.db.models import Model, Q
 from django.test import tag
+from meilisearch import Client
 
-# Application
 from jklib.meili.dj.indexer import MeilisearchModelIndexer
 
-
 M = TypeVar("M", bound=Model)
 
 
 @tag("integration")
 class IndexerBaseTestMixin(Generic[M]):
     """
     Base test mixin for testing MeilisearchModelIndexer subclasses.
@@ -31,22 +25,22 @@
 
     indexer_class: Type[MeilisearchModelIndexer]
     item_1: M
     item_2: M
     search_attribute: str
     sleep_time: float = 0.1
 
-    def setUp(self):
-        super().setUp()
+    def setUp(self) -> None:
+        super().setUp()  # type: ignore
         self.meilisearch_client.delete_index(self.indexer_class.index_name())
         sleep(self.sleep_time)
 
-    def tearDown(self):
+    def tearDown(self) -> None:
         self.meilisearch_client.delete_index(self.indexer_class.index_name())
-        super().tearDown()
+        super().tearDown()  # type: ignore
 
     def test_index_exists(self) -> None:
         self.assertFalse(self.indexer_class.index_exists())
         self.meilisearch_client.create_index(self.indexer_class.index_name())
         sleep(self.sleep_time)
         self.assertTrue(self.indexer_class.index_exists())
 
@@ -170,28 +164,28 @@
         self.assertSearchHits(response, [])
 
     def test_search(self) -> None:
         self.meilisearch_client.create_index(self.indexer_class.index_name())
         search_value = getattr(self.item_1, self.search_attribute)
         sleep(self.sleep_time)
         response = self.indexer_class.search(search_value)
-        self.assertSearchHits(response, [])
+        self.assertSearchHits(response, [])  # type: ignore
         self.indexer_class.index(self.item_1)
         sleep(self.sleep_time)
         response = self.indexer_class.search(search_value)
-        self.assertSearchHits(response, [self.item_1])
+        self.assertSearchHits(response, [self.item_1])  # type: ignore
         self.assertEqual(response.get("limit"), 20)
         response = self.indexer_class.search(search_value, limit=1)
-        self.assertSearchHits(response, [self.item_1])
+        self.assertSearchHits(response, [self.item_1])  # type: ignore
         self.assertEqual(response.get("limit"), 1)
         response = self.indexer_class.search(search_value, only_hits=True, limit=1)
-        self.assertSearchHits(response, [self.item_1])
+        self.assertSearchHits(response, [self.item_1])  # type: ignore
         self.assertNotIn("limit", response)
 
     def test_meilisearch_client(self) -> None:
         self.assertIsInstance(self.indexer_class.meilisearch_client(), Client)
 
-    def assertSearchHits(self, response, items):
+    def assertSearchHits(self, response: Dict, items: List[M]) -> None:
         ids = {hit["id"] for hit in response["hits"]}
         self.assertSetEqual(
             ids, {getattr(item, self.indexer_class.PRIMARY_KEY) for item in items}
         )
```

### Comparing `jklib-5.1.1/jklib/meili/search.py` & `jklib-5.2.0/jklib/meili/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Built-in
 from typing import List, Tuple
 
-# Application
 from jklib.meili.types import MeilisearchFilterValue
 
 
 def build_search_filter(
     is_empty: List[str] = None,
     is_not_empty: List[str] = None,
     is_null: List[str] = None,
```

### Comparing `jklib-5.1.1/jklib/meili/types.py` & `jklib-5.2.0/jklib/meili/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Built-in
 from typing import Any, Dict, List, Literal, Optional, Tuple, TypedDict, Union
 
 
 class Faceting(TypedDict):
     maxValuesPerFacet: int
     sortFacetValuesBy: Dict[str, str]
```

### Comparing `jklib-5.1.1/jklib/std/files.py` & `jklib-5.2.0/jklib/std/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Built-in
 import base64
 import io
 import os
 from typing import Union
 
 
 def convert_size(
```

### Comparing `jklib-5.1.1/jklib/std/images.py` & `jklib-5.2.0/jklib/std/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-# Built-in
 import base64
 from io import BytesIO
 from typing import Optional, Tuple
 
-# Third-party
 from PIL import Image
 
 
 def downsize_image(file_path: str, width: int, height: int) -> None:
     """Downsizes an image to the given dimensions while keeping its ratio."""
     img = Image.open(file_path)
     if (img.height > height) or (img.width > width):
```

### Comparing `jklib-5.1.1/jklib/std/inputs.py` & `jklib-5.2.0/jklib/std/inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Built-in
 import re
 from typing import Dict
 
 
 def choose_from_dict(choices: Dict) -> str:
     """User must choose a value by inputting the associated key."""
     # Displays the initial choices
```

### Comparing `jklib-5.1.1/jklib/std/strings.py` & `jklib-5.2.0/jklib/std/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Built-in
 from typing import List
 
 
 def clean_text(text: str, olds: List[str], new: str = " ") -> str:
     """Replaces all occurrences of 'olds' with 'new' within a text."""
     for old in olds:
         text = text.replace(old, new)
```

### Comparing `jklib-5.1.1/jklib/std/transforms.py` & `jklib-5.2.0/jklib/std/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Built-in
 import json
 from typing import Any, Dict, List, OrderedDict, Union
 
 
 def array2d_to_dict(array2d: List[List], col_index: int) -> Dict[Any, List]:
     """Transforms a 2d array into a dict, with one col as key."""
     new_dict = {}
```

### Comparing `jklib-5.1.1/jklib.egg-info/SOURCES.txt` & `jklib-5.2.0/jklib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jklib-5.1.1/setup.py` & `jklib-5.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Setup file for the PyPi packaging."""
 
-
-# Third-party
-from setuptools import find_packages, setup
+from setuptools import find_packages, setup  # type: ignore
 
 # --------------------------------------------------------------------------------
 # > Variables
 # --------------------------------------------------------------------------------
-VERSION = "5.1.1"
+VERSION = "5.2.0"
 packages = find_packages()
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 # --------------------------------------------------------------------------------
 # > Setup
 # --------------------------------------------------------------------------------
```

