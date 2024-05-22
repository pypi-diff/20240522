# Comparing `tmp/di_service_locator-1.1.0.tar.gz` & `tmp/di_service_locator-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "di_service_locator-1.1.0.tar", max compression
+gzip compressed data, was "di_service_locator-1.2.0.tar", max compression
```

## Comparing `di_service_locator-1.1.0.tar` & `di_service_locator-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1072 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/LICENSE
--rw-r--r--   0        0        0     6138 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/README.md
--rw-r--r--   0        0        0      185 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/__init__.py
--rw-r--r--   0        0        0     8177 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/config.py
--rw-r--r--   0        0        0     1736 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/definitions.py
--rw-r--r--   0        0        0      552 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/exceptions.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/__init__.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/aws/__init__.py
--rw-r--r--   0        0        0     8016 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/aws/blob_storage.py
--rw-r--r--   0        0        0     6290 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/blob_storage.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/gcp/__init__.py
--rw-r--r--   0        0        0     6781 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/gcp/blob_storage.py
--rw-r--r--   0        0        0     6596 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/instrumentation.py
--rw-r--r--   0        0        0    10079 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/feature_defs/interfaces.py
--rw-r--r--   0        0        0     6350 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/features.py
--rw-r--r--   0        0        0     1482 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/files.py
--rw-r--r--   0        0        0     1325 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/instantiator.py
--rw-r--r--   0        0        0        1 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/py.typed
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/utils/__init__.py
--rw-r--r--   0        0        0      468 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/utils/helpers.py
--rw-r--r--   0        0        0     1355 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/di_service_locator/utils/transcoding.py
--rw-r--r--   0        0        0     3396 2024-02-28 16:01:31.747384 di_service_locator-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1793 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/__init__.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/aws/__init__.py
--rw-r--r--   0        0        0     7636 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/aws/test_blob_storage.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/gcp/__init__.py
--rw-r--r--   0        0        0     5414 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/gcp/test_blob_storage.py
--rw-r--r--   0        0        0     7889 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/test_blobstorage.py
--rw-r--r--   0        0        0    14176 2024-02-28 16:01:22.515298 di_service_locator-1.1.0/tests/feature_defs/test_instrumentation.py
--rw-r--r--   0        0        0     2765 2024-02-28 16:01:22.519298 di_service_locator-1.1.0/tests/test_config.py
--rw-r--r--   0        0        0      259 2024-02-28 16:01:22.519298 di_service_locator-1.1.0/tests/test_features.json
--rw-r--r--   0        0        0     3653 2024-02-28 16:01:22.519298 di_service_locator-1.1.0/tests/test_features.py
--rw-r--r--   0        0        0       94 2024-02-28 16:01:22.519298 di_service_locator-1.1.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     1352 2024-02-28 16:01:22.519298 di_service_locator-1.1.0/tests/utils/test_transcoding.py
--rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 di_service_locator-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/LICENSE
+-rw-r--r--   0        0        0     6138 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/README.md
+-rw-r--r--   0        0        0      186 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/__init__.py
+-rw-r--r--   0        0        0     9180 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/config.py
+-rw-r--r--   0        0        0     1749 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/definitions.py
+-rw-r--r--   0        0        0      552 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/exceptions.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/aws/__init__.py
+-rw-r--r--   0        0        0     8017 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/aws/blob_storage.py
+-rw-r--r--   0        0        0     6291 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/blob_storage.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/gcp/__init__.py
+-rw-r--r--   0        0        0     6782 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/gcp/blob_storage.py
+-rw-r--r--   0        0        0     6597 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/instrumentation.py
+-rw-r--r--   0        0        0    10080 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/feature_defs/interfaces.py
+-rw-r--r--   0        0        0     6351 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/features.py
+-rw-r--r--   0        0        0     1483 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/files.py
+-rw-r--r--   0        0        0     1326 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/instantiator.py
+-rw-r--r--   0        0        0        1 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/py.typed
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/utils/__init__.py
+-rw-r--r--   0        0        0      468 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/utils/helpers.py
+-rw-r--r--   0        0        0     1356 2024-05-22 09:48:55.108867 di_service_locator-1.2.0/di_service_locator/utils/transcoding.py
+-rw-r--r--   0        0        0     3423 2024-05-22 09:49:04.840985 di_service_locator-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1793 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/__init__.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/aws/__init__.py
+-rw-r--r--   0        0        0     7639 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/aws/test_blob_storage.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/gcp/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/gcp/test_blob_storage.py
+-rw-r--r--   0        0        0     7890 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/test_blobstorage.py
+-rw-r--r--   0        0        0    14176 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/feature_defs/test_instrumentation.py
+-rw-r--r--   0        0        0     3062 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/test_config.py
+-rw-r--r--   0        0        0      259 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/test_features.json
+-rw-r--r--   0        0        0     3653 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/test_features.py
+-rw-r--r--   0        0        0       94 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-22 09:48:55.112867 di_service_locator-1.2.0/tests/utils/test_transcoding.py
+-rw-r--r--   0        0        0     7056 1970-01-01 00:00:00.000000 di_service_locator-1.2.0/PKG-INFO
```

### Comparing `di_service_locator-1.1.0/LICENSE` & `di_service_locator-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/README.md` & `di_service_locator-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/di_service_locator/config.py` & `di_service_locator-1.2.0/di_service_locator/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Classes and functions to create factory maps from config."""
+
 import json
 import os
 import pathlib
 import sys
 from typing import Callable, Dict, Mapping, Optional, Sequence, Tuple
 
 from di_service_locator import logger
@@ -84,31 +85,55 @@
 
     @staticmethod
     def _is_property(property_value: str) -> bool:
         return isinstance(property_value, str) and property_value.startswith(
             PROPERTY_IDENTIFIER
         )
 
-    def _resolve_property(self, property_value: str) -> str:
+    def _resolve_property(self, property_value: str) -> Optional[str]:
+        """
+        Resolves properties into values.
+
+        The initial value could be one of the following:
+            value            a hardcoded value
+            $VALUE           a property to resolve (mandatory)
+            $VALUE=default   a property to resolve with a default
+            $VALUE=          a property to resolve with a default of None
+
+        :param property_value: the intial property value from the config
+        :type property_value: str
+        :raises FeatureConfigError: if a manadatory property can't be resolved and there is
+            no default
+        :return: the resolved value
+        :rtype: Optional[str]
+        """
+        ret: Optional[str] = property_value
         if PropertyResolver._is_property(property_value):
-            property_name = property_value[len(PROPERTY_IDENTIFIER) :]
+            property_value = property_value.lstrip(PROPERTY_IDENTIFIER)
             property_default = None
-            if PROPERTY_DEFAULT_SEPARATOR in property_name:
-                property_name, property_default = property_name.split(
+            property_default_found = False
+            if PROPERTY_DEFAULT_SEPARATOR in property_value:
+                property_value, property_default = property_value.split(
                     PROPERTY_DEFAULT_SEPARATOR, maxsplit=1
                 )
+                property_default_found = True
+                if not property_default:
+                    property_default = None
             for resolver in self._providers:
-                value = resolver(property_name)
+                value = resolver(property_value)
                 if value:
+                    # early return if we've resolved a property
                     return value
-            if property_default:
-                property_value = property_default
+            if property_default_found:
+                ret = property_default
             else:
-                raise FeatureConfigError(f"No property value found for {property_value}")
-        return property_value
+                raise FeatureConfigError(
+                    f"No property value found for {PROPERTY_IDENTIFIER}{property_value}"
+                )
+        return ret
 
     def resolve(self, factory_definition: FactoryDefinition) -> FactoryDefinition:
         """
         Take a `FactoryDefinition` and resolve any args or kwargs that are properties.
 
         Properties are values of the form $<property name>
         Note that property resolution is done in place and the factory definition is mutated
```

### Comparing `di_service_locator-1.1.0/di_service_locator/definitions.py` & `di_service_locator-1.2.0/di_service_locator/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Feature dataclasses and types."""
+
 import abc
 import dataclasses
 from typing import Collection, Mapping, Sequence, Tuple, Union
 
-Primitives = Union[str, bool, int, float, Collection[str], Collection[int], Collection[float]]
+Primitives = Union[
+    str, bool, int, float, Collection[str], Collection[int], Collection[float], None
+]
 # Type def for supported primitives
 # TODO: dates? timestamps?
 
 
 @dataclasses.dataclass
 class FactoryDefinition:
     """
```

### Comparing `di_service_locator-1.1.0/di_service_locator/exceptions.py` & `di_service_locator-1.2.0/di_service_locator/exceptions.py`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/di_service_locator/feature_defs/aws/blob_storage.py` & `di_service_locator-1.2.0/di_service_locator/feature_defs/aws/blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 """
 Module for aws s3 bucket blob storage implementation.
 
 Sadly the python API doesn't support streaming so we occasionally have to buffer data
 in memory.
 """
+
 import contextlib
 import io
 import os
 from typing import IO, TYPE_CHECKING, Generator, Optional
 
 import boto3
 import botocore.exceptions
```

### Comparing `di_service_locator-1.1.0/di_service_locator/feature_defs/blob_storage.py` & `di_service_locator-1.2.0/di_service_locator/feature_defs/blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Module for basic blob storage implementations."""
+
 import contextlib
 from pathlib import Path
 from typing import IO, Generator, Tuple
 
 from typing_extensions import Self
 
 from di_service_locator.feature_defs.instrumentation import instrument_timer
```

### Comparing `di_service_locator-1.1.0/di_service_locator/feature_defs/gcp/blob_storage.py` & `di_service_locator-1.2.0/di_service_locator/feature_defs/gcp/blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 """
 Google cloud bucket blob storage implementation of BlobStorage.
 
 Sadly the python API doesn't support streaming so we occasionally have to buffer data
 in memory.
 """
+
 import contextlib
 import io
 import os
 from typing import IO, Generator, Optional
 
 import google.api_core.exceptions as google_exceptions
 from google.auth.credentials import AnonymousCredentials
```

### Comparing `di_service_locator-1.1.0/di_service_locator/feature_defs/instrumentation.py` & `di_service_locator-1.2.0/di_service_locator/feature_defs/instrumentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Contains concrete instrumentation implementations."""
+
 import functools
 from collections import defaultdict
 from contextlib import contextmanager
 from datetime import datetime
 from typing import Callable, Dict, Generator, Optional, TypeVar
 
 from typing_extensions import ParamSpec
```

### Comparing `di_service_locator-1.1.0/di_service_locator/feature_defs/interfaces.py` & `di_service_locator-1.2.0/di_service_locator/feature_defs/interfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 """
 Contains common, simple service interface definitions.
 
 It is not a requirement that all service definitions go in here, but it is a useful place
 for most of them.
 """
+
 import abc
 from datetime import datetime
 from typing import IO, ContextManager, Generator, Iterable
 
 from typing_extensions import Self
```

### Comparing `di_service_locator-1.1.0/di_service_locator/features.py` & `di_service_locator-1.2.0/di_service_locator/features.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Features injector and service locator module."""
+
 import os
 import threading
 from typing import Any, Optional, Type, TypeVar
 
 from di_service_locator import logger
 from di_service_locator.config import factory_map_from_json_file
 from di_service_locator.definitions import FactoryDefinition, FactoryMap
```

### Comparing `di_service_locator-1.1.0/di_service_locator/files.py` & `di_service_locator-1.2.0/di_service_locator/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Some file utilities."""
+
 from pathlib import Path
 from typing import Sequence
 
 DI_CONFIG_DIR = ".di"
 HOME_DIR = Path.home() / DI_CONFIG_DIR
 CURRENT_DIR = Path().absolute()
 CURRENT_OR_HOME = [CURRENT_DIR, HOME_DIR]
```

### Comparing `di_service_locator-1.1.0/di_service_locator/instantiator.py` & `di_service_locator-1.2.0/di_service_locator/instantiator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Reusable functions for dynamically loading and instantiating classes."""
+
 import importlib
 from typing import Type, TypeVar
 
 InstanceT = TypeVar("InstanceT")
 
 
 def load_class(fqn: str) -> Type:
```

### Comparing `di_service_locator-1.1.0/di_service_locator/utils/transcoding.py` & `di_service_locator-1.2.0/di_service_locator/utils/transcoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Module containing useful utility functions to transcode streams on the fly."""
+
 import codecs
 from typing import IO, cast
 
 
 def text_to_bytes_writer(byte_stream: IO[bytes], encoding: str = "utf-8") -> IO[str]:
     """
     Transcode text to bytes whilst writing.
```

### Comparing `di_service_locator-1.1.0/pyproject.toml` & `di_service_locator-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "di-service-locator"
-version = "1.1.0"
+version = "1.2.0"
 description = "Injection utilities to obtain instances of dynamically created features from config"
 authors = []
 license = "MIT"
 readme = "README.md"
 homepage = "https://deeperinsights.com"
 repository = "https://github.com/skimit/di-service-locator"
 include = [
@@ -20,20 +20,20 @@
 botocore = {version = "^1.23.24", optional = true}
 google-cloud-storage = {version = "^2.5.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 boto3-stubs = {extras = ["s3"], version = "^1.20.45"}
 gcp-storage-emulator = "2022.6.11"
 google-cloud-storage = "^2.5.0"
-moto = "4.2.6"
+moto = "5.0.5"
 pyright = "^1.1.349"
 pytest = "^8.0.0"
 pytest-cov = "^4.0.0"
 pytest-ruff = "^0.2.1"
-ruff = "^0.1.14"
+ruff = ">=0.1.14,<0.5.0"
 taskipy = "^1.2.0"
 typing-extensions = "^4.9.0"
 urllib3 = "1.26.18"  # Ugly hack to work around poetry bug
 
 [tool.poetry.extras]
 gcp = ["google-cloud-storage"]
 aws = ["boto3", "botocore"]
@@ -43,15 +43,15 @@
 coverage = "pyright . && pytest --ruff --ruff-format -ra -v --cov=. --cov-report=xml:test-coverage.xml --cov-fail-under=70 --maxfail=3 --junitxml=test-results.xml"
 debug = "python -m debugpy --listen 0.0.0.0:5678 --wait-for-client /usr/local/bin/pytest"
 format = "ruff format -n . && ruff check -n --fix ."
 test = "pytest --ruff --ruff-format --cache-clear -ra -v"
 typecheck = "pyright ."
 
 [tool.pyright]
-include = ["di_service_locator"]
+include = ["di_service_locator", "tests"]
 exclude = [  # Do not process these files
     "**/node_modules",
     "**/__pycache__",
     ".venv/**",
 ]
 defineConstant = { DEBUG = true }
 ignore = ["tests"]  # Process these files, but ignore errors
@@ -59,15 +59,15 @@
 reportMissingImports = true
 reportMissingTypeStubs = false
 pythonVersion = "3.9"
 pythonPlatform = "Linux"
 executionEnvironments = [{ root = "di_service_locator" }]
 
 [tool.ruff]
-select = ["E", "F", "D", "I"]
+lint.select = ["E", "F", "D", "I"]
 # Docstring Ignores:
 # D100 - Missing docstring in public module
 # D102 - Missing docstring in public method
 # D103 - Missing docstring in public function
 # D104 - Missing docstring in public package
 # D105 - Missing docstring in magic method
 # D107 - Missing docstring in __init__
@@ -76,15 +76,15 @@
 # D213 - Multi-line docstring summary should start at the first line
 # D400 - First line should end with a period
 # D401 - First line should be in imperative mood
 # D406 - Section name should end with a newline
 # D407 - Missing dashed underline after section
 # D413 - Missing blank line after last section
 # D415 - First line should end with a period, question mark, or exclamation point
-ignore = ["D100", "D102", "D103", "D104", "D105", "D107", "D202", "D203", "D212", "D400", "D401", "D406", "D407", "D413", "D415"]
+lint.ignore = ["D100", "D102", "D103", "D104", "D105", "D107", "D202", "D203", "D212", "D400", "D401", "D406", "D407", "D413", "D415"]
 line-length = 95
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
 line-ending = "auto"
```

### Comparing `di_service_locator-1.1.0/tests/conftest.py` & `di_service_locator-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/tests/feature_defs/aws/test_blob_storage.py` & `di_service_locator-1.2.0/tests/feature_defs/aws/test_blob_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Tests for aws blob storage implementation."""
+
 import io
 import os
 import re
 from typing import Type
 
 import boto3
 import pytest
-from moto import mock_s3
+from moto import mock_aws
 
 from di_service_locator.feature_defs.aws.blob_storage import (
     AwsBucketBlobStorage,
     DeletableAwsBucketBlobStorage,
 )
 from di_service_locator.feature_defs.interfaces import (
     BlobNotFoundError,
@@ -28,15 +29,15 @@
     """Mocked AWS Credentials for moto."""
     os.environ["AWS_ACCESS_KEY_ID"] = "testing"
     os.environ["AWS_SECRET_ACCESS_KEY"] = "testing"
     os.environ["AWS_SECURITY_TOKEN"] = "testing"
     os.environ["AWS_SESSION_TOKEN"] = "testing"
 
     try:
-        mock = mock_s3()
+        mock = mock_aws()
         mock.start()
 
         try:
             conn = boto3.resource("s3", region_name="us-east-1")
             conn.create_bucket(Bucket="test_bucket")
             yield conn
         finally:
```

### Comparing `di_service_locator-1.1.0/tests/feature_defs/gcp/test_blob_storage.py` & `di_service_locator-1.2.0/tests/feature_defs/gcp/test_blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Tests for google blob storage implementation."""
+
 import io
 import os
 import re
 
 import pytest
 from gcp_storage_emulator.server import create_server
```

### Comparing `di_service_locator-1.1.0/tests/feature_defs/test_blobstorage.py` & `di_service_locator-1.2.0/tests/feature_defs/test_blobstorage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Explicit tests for `FileBlobStorage` implementation."""
+
 import dataclasses
 import io
 import json
 import tempfile
 from pathlib import Path
 from typing import Generator, Type
```

### Comparing `di_service_locator-1.1.0/tests/feature_defs/test_instrumentation.py` & `di_service_locator-1.2.0/tests/feature_defs/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/tests/test_config.py` & `di_service_locator-1.2.0/tests/test_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Tests for config functions and property resolution."""
+
 import os
 import sys
 from unittest.mock import patch
 
 import pytest
 
 from di_service_locator.config import STANDARD_PROPERTY_RESOLVER, FeatureConfigError
@@ -15,42 +16,55 @@
 
 @pytest.fixture(name="mock_factory_definition")
 def _mock_factory_definition():
     return FactoryDefinition(
         fqn_impl_factory="dummy",
         fqn_interface="dummy",
         args=[1, "$PROPERTY1", 3],
-        kwargs={"key": "value", "key2": "$PROPERTY2", "key3": "$PROPERTY3=default_value"},
+        kwargs={
+            "key": "value",
+            "key2": "$PROPERTY2",
+            "key3": "$PROPERTY3=default_value",
+            "key4": "$PROPERTY4=",
+        },
     )
 
 
 def test_property_resolver__args(mock_factory_definition):
     """Test that properties can be extracted from command line args."""
     testargs = ["--PROPERTY1=testvalue1", "--PROPERTY2=testvalue2"]
     with patch.object(sys, "argv", testargs):
         result = STANDARD_PROPERTY_RESOLVER.resolve(mock_factory_definition)
         assert result.args == [1, "testvalue1", 3]
-        assert result.kwargs == {"key": "value", "key2": "testvalue2", "key3": "default_value"}
+        assert result.kwargs == {
+            "key": "value",
+            "key2": "testvalue2",
+            "key3": "default_value",
+            "key4": None,
+        }
 
 
 def test_property_resolver__env(mock_factory_definition):
     """Test that properties can be extracted from environment variables."""
     os.environ["PROPERTY1"] = "envtestvalue1"
     os.environ["PROPERTY2"] = "envtestvalue2"
+    os.environ["PROPERTY4"] = "hasavalue"
     try:
         result = STANDARD_PROPERTY_RESOLVER.resolve(mock_factory_definition)
         assert result.args == [1, "envtestvalue1", 3]
         assert result.kwargs == {
             "key": "value",
             "key2": "envtestvalue2",
             "key3": "default_value",
+            "key4": "hasavalue",
         }
     finally:
         del os.environ["PROPERTY1"]
         del os.environ["PROPERTY2"]
+        del os.environ["PROPERTY4"]
 
 
 def test_property_resolver__precedence(mock_factory_definition):
     """Test the properties are resolved in the correct order."""
     os.environ["PROPERTY1"] = "notused1"
     os.environ["PROPERTY2"] = "envtestvalue2"
     try:
@@ -58,14 +72,15 @@
         with patch.object(sys, "argv", testargs):
             result = STANDARD_PROPERTY_RESOLVER.resolve(mock_factory_definition)
             assert result.args == [1, "testvalue1", 3]
             assert result.kwargs == {
                 "key": "value",
                 "key2": "envtestvalue2",
                 "key3": "default_value",
+                "key4": None,
             }
     finally:
         del os.environ["PROPERTY1"]
         del os.environ["PROPERTY2"]
 
 
 def test_property_resolver__not_found(mock_factory_definition):
```

### Comparing `di_service_locator-1.1.0/tests/test_features.py` & `di_service_locator-1.2.0/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `di_service_locator-1.1.0/tests/utils/test_transcoding.py` & `di_service_locator-1.2.0/tests/utils/test_transcoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -=- encoding: utf-8 -=-
 #
 # Copyright (c) 2024 Deeper Insights. Subject to the MIT license.
 
 """Tests for transcoding functions."""
+
 import json
 import tempfile
 from pathlib import Path
 
 from di_service_locator.utils.transcoding import bytes_to_text_reader, text_to_bytes_writer
```

### Comparing `di_service_locator-1.1.0/PKG-INFO` & `di_service_locator-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: di-service-locator
-Version: 1.1.0
+Version: 1.2.0
 Summary: Injection utilities to obtain instances of dynamically created features from config
 Home-page: https://deeperinsights.com
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

