# Comparing `tmp/python_homewizard_energy-5.0.0b1.tar.gz` & `tmp/python_homewizard_energy-6.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_homewizard_energy-5.0.0b1.tar", max compression
+gzip compressed data, was "python_homewizard_energy-6.0.0b1.tar", max compression
```

## Comparing `python_homewizard_energy-5.0.0b1.tar` & `python_homewizard_energy-6.0.0b1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11346 2024-03-19 15:06:22.804876 python_homewizard_energy-5.0.0b1/LICENSE
--rw-r--r--   0        0        0     2105 2024-03-19 15:06:22.804876 python_homewizard_energy-5.0.0b1/README.md
--rw-r--r--   0        0        0      468 2024-03-19 15:06:22.804876 python_homewizard_energy-5.0.0b1/homewizard_energy/__init__.py
--rw-r--r--   0        0        0      185 2024-03-19 15:06:22.804876 python_homewizard_energy-5.0.0b1/homewizard_energy/const.py
--rw-r--r--   0        0        0      765 2024-03-19 15:06:22.808876 python_homewizard_energy-5.0.0b1/homewizard_energy/errors.py
--rw-r--r--   0        0        0     8438 2024-03-19 15:06:22.808876 python_homewizard_energy-5.0.0b1/homewizard_energy/homewizard_energy.py
--rw-r--r--   0        0        0    12926 2024-03-19 15:06:22.808876 python_homewizard_energy-5.0.0b1/homewizard_energy/models.py
--rw-r--r--   0        0        0        0 2024-03-19 15:06:22.808876 python_homewizard_energy-5.0.0b1/homewizard_energy/py.typed
--rw-r--r--   0        0        0     2416 2024-03-19 15:06:45.596989 python_homewizard_energy-5.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 python_homewizard_energy-5.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2105 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/README.md
+-rw-r--r--   0        0        0      439 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/const.py
+-rw-r--r--   0        0        0      765 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/errors.py
+-rw-r--r--   0        0        0     6536 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/homewizard_energy.py
+-rw-r--r--   0        0        0    12486 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/models.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:12:16.247455 python_homewizard_energy-6.0.0b1/homewizard_energy/py.typed
+-rw-r--r--   0        0        0     2415 2024-05-22 19:12:30.971467 python_homewizard_energy-6.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3157 1970-01-01 00:00:00.000000 python_homewizard_energy-6.0.0b1/PKG-INFO
```

### Comparing `python_homewizard_energy-5.0.0b1/LICENSE` & `python_homewizard_energy-6.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-5.0.0b1/README.md` & `python_homewizard_energy-6.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-5.0.0b1/homewizard_energy/errors.py` & `python_homewizard_energy-6.0.0b1/homewizard_energy/errors.py`

 * *Files identical despite different names*

### Comparing `python_homewizard_energy-5.0.0b1/homewizard_energy/homewizard_energy.py` & `python_homewizard_energy-6.0.0b1/homewizard_energy/homewizard_energy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Representation of a HomeWizard Energy device."""
+
 from __future__ import annotations
 
 import asyncio
 import logging
-import string
 from collections.abc import Callable, Coroutine
 from http import HTTPStatus
 from typing import Any, TypeVar
 
 import async_timeout
 from aiohttp.client import ClientError, ClientResponseError, ClientSession
-from aiohttp.hdrs import METH_DELETE, METH_GET, METH_PUT
+from aiohttp.hdrs import METH_GET, METH_PUT
 
 from .const import SUPPORTED_API_VERSION
 from .errors import DisabledError, NotFoundError, RequestError, UnsupportedError
-from .models import Data, Decryption, Device, State, System
+from .models import Data, Device, State, System
 
 _LOGGER = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 def optional_method(
@@ -141,75 +141,14 @@
     async def identify(
         self,
     ) -> bool:
         """Send identify request."""
         await self.request("api/v1/identify", method=METH_PUT)
         return True
 
-    @optional_method
-    async def decryption(self) -> Decryption:
-        """Return the decryption object."""
-        response = await self.request("api/v1/decryption")
-        return Decryption.from_dict(response)
-
-    @optional_method
-    async def decryption_set(
-        self,
-        key: str | None = None,
-        aad: str | None = None,
-    ) -> bool:
-        """Set state of device."""
-        data = {}
-
-        if key is not None:
-            if len(key) != 32:
-                raise ValueError("Key length should be 32 characters long")
-            if not all(c in string.hexdigits for c in key):
-                raise ValueError(
-                    "Key should only contain hexadecimal characters (0-9/a-f)"
-                )
-
-            data["key"] = key
-
-        if aad is not None:
-            if len(aad) != 34:
-
-                hint: str | None = None
-                if len(aad) == 32:
-                    hint = "Hint: Try prefixing AAD with '30', e.g. '30<AAD>'"
-                raise ValueError("AAD length should be 34 characters long", hint)
-            if not all(c in string.hexdigits for c in aad):
-                raise ValueError(
-                    "AAD should only contain hexadecimal characters (0-9/a-f)"
-                )
-
-            data["aad"] = aad
-
-        if not data:
-            _LOGGER.error("At least one decryption key is required")
-            return False
-
-        await self.request("api/v1/decryption", method=METH_PUT, data=data)
-        return True
-
-    @optional_method
-    async def decryption_reset(
-        self,
-        key: bool = False,
-        aad: bool = False,
-    ) -> bool:
-        """Reset decryption keys of device."""
-        data = {
-            "key": key,
-            "aad": aad,
-        }
-
-        await self.request("api/v1/decryption", method=METH_DELETE, data=data)
-        return True
-
     async def request(
         self, path: str, method: str = METH_GET, data: object = None
     ) -> Any:
         """Make a request to the API."""
         if self._session is None:
             self._session = ClientSession()
             self._close_session = True
```

### Comparing `python_homewizard_energy-5.0.0b1/homewizard_energy/models.py` & `python_homewizard_energy-6.0.0b1/homewizard_energy/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,15 +157,17 @@
 
         if external_devices is None:
             return None
 
         for external in external_devices:
             with suppress(ValueError, KeyError):
                 device = ExternalDevice.from_dict(external)
-            devices[device.unique_id] = device
+                type_unique_id = f"{external.get('type')}_{device.unique_id}"
+
+            devices[type_unique_id] = device
 
         return devices
 
     @staticmethod
     def from_dict(data: dict[str, Any]) -> Data:
         """Return State object from API response.
 
@@ -272,15 +274,15 @@
                 return {
                     "gas_meter": ExternalDevice.DeviceType.GAS_METER,
                     "heat_meter": ExternalDevice.DeviceType.HEAT_METER,
                     "warm_water_meter": ExternalDevice.DeviceType.WARM_WATER_METER,
                     "water_meter": ExternalDevice.DeviceType.WATER_METER,
                     "inlet_heat_meter": ExternalDevice.DeviceType.INLET_HEAT_METER,
                 }[value]
-            except (KeyError):
+            except KeyError:
                 return ExternalDevice.DeviceType.UNKNOWN
 
     unique_id: str
     meter_type: DeviceType
     value: float
     unit: str
     timestamp: datetime
@@ -347,30 +349,7 @@
 
         Returns:
             A System object.
         """
         return System(
             cloud_enabled=data.get("cloud_enabled"),
         )
-
-
-@dataclass
-class Decryption:
-    """Represent decryption API."""
-
-    key_set: bool | None
-    aad_set: bool | None
-
-    @staticmethod
-    def from_dict(data: dict[str, Any]) -> Decryption:
-        """Return Decryption object from API response.
-
-        Args:
-            data: The data from the HomeWizard Energy `api/v1/decryption` API.
-
-        Returns:
-            A Decryption object.
-        """
-        return Decryption(
-            key_set=data.get("key"),
-            aad_set=data.get("aad"),
-        )
```

### Comparing `python_homewizard_energy-5.0.0b1/pyproject.toml` & `python_homewizard_energy-6.0.0b1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-homewizard-energy"
-version = "5.0.0-beta-1"
+version = "6.0.0-beta-1"
 description = "Asynchronous Python client for the HomeWizard Energy"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/homewizard/python-homewizard-energy"
 repository = "https://github.com/homewizard/python-homewizard-energy"
@@ -18,27 +18,27 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = ">=3.0.0"
 async-timeout = "^4.0.3"
 
 [tool.poetry.dev-dependencies]
 aresponses = "^3.0.0"
-black = "^22.12"
+black = "^24.4"
 blacken-docs = "^1.16.0"
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.7.0"
 isort = "^5.13.2"
 pre-commit = "^3.6.0"
 pre-commit-hooks = "^4.5.0"
-pylint = "^3.0.3"
+pylint = "^3.1.0"
 pytest = "^7.4.4"
-pytest-asyncio = "^0.23.4"
+pytest-asyncio = "^0.23.6"
 pytest-cov = "^4.1.0"
 yamllint = "^1.33.0"
-pyupgrade = "^3.15.0"
+pyupgrade = "^3.15.2"
 flake8-simplify = "^0.21.0"
 vulture = "^2.11"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
 flake8-builtins = "^2.2.0"
 flake8-comprehensions = "^3.14.0"
 flake8-eradicate = "^1.2.1"
```

### Comparing `python_homewizard_energy-5.0.0b1/PKG-INFO` & `python_homewizard_energy-6.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-homewizard-energy
-Version: 5.0.0b1
+Version: 6.0.0b1
 Summary: Asynchronous Python client for the HomeWizard Energy
 Home-page: https://github.com/homewizard/python-homewizard-energy
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

