# Comparing `tmp/cognite_extractor_utils-7.1.6.tar.gz` & `tmp/cognite_extractor_utils-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_extractor_utils-7.1.6.tar", max compression
+gzip compressed data, was "cognite_extractor_utils-7.2.0.tar", max compression
```

## Comparing `cognite_extractor_utils-7.1.6.tar` & `cognite_extractor_utils-7.2.0.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0    10173 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/LICENSE
--rw-r--r--   0        0        0     4090 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/README.md
--rw-r--r--   0        0        0      739 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/__init__.py
--rw-r--r--   0        0        0     1558 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/_inner_util.py
--rw-r--r--   0        0        0    16391 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/base.py
--rw-r--r--   0        0        0     3059 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/__init__.py
--rw-r--r--   0        0        0     4739 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/_util.py
--rw-r--r--   0        0        0    21564 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/elements.py
--rw-r--r--   0        0        0    16317 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/loaders.py
--rw-r--r--   0        0        0     1084 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/exceptions.py
--rw-r--r--   0        0        0    15509 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/metrics.py
--rw-r--r--   0        0        0        0 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/py.typed
--rw-r--r--   0        0        0    18667 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/statestore.py
--rw-r--r--   0        0        0     3605 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/threading.py
--rw-r--r--   0        0        0     3110 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/__init__.py
--rw-r--r--   0        0        0     5304 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_base.py
--rw-r--r--   0        0        0     3247 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_metrics.py
--rw-r--r--   0        0        0     5628 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/assets.py
--rw-r--r--   0        0        0     5680 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/events.py
--rw-r--r--   0        0        0    18329 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/files.py
--rw-r--r--   0        0        0     6738 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/raw.py
--rw-r--r--   0        0        0    26817 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/time_series.py
--rw-r--r--   0        0        0     7732 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_extractor.py
--rw-r--r--   0        0        0     1020 2024-05-15 10:34:22.112807 cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_types.py
--rw-r--r--   0        0        0    17198 2024-05-15 10:34:22.116807 cognite_extractor_utils-7.1.6/cognite/extractorutils/util.py
--rw-r--r--   0        0        0     2088 2024-05-15 10:34:22.116807 cognite_extractor_utils-7.1.6/pyproject.toml
--rw-r--r--   0        0        0     5446 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.1.6/PKG-INFO
+-rw-r--r--   0        0        0    10173 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/LICENSE
+-rw-r--r--   0        0        0     4090 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/README.md
+-rw-r--r--   0        0        0      739 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/__init__.py
+-rw-r--r--   0        0        0     1558 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/_inner_util.py
+-rw-r--r--   0        0        0    16391 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/base.py
+-rw-r--r--   0        0        0     3059 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/__init__.py
+-rw-r--r--   0        0        0     4739 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/_util.py
+-rw-r--r--   0        0        0    21564 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/elements.py
+-rw-r--r--   0        0        0    16317 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/loaders.py
+-rw-r--r--   0        0        0     1084 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/exceptions.py
+-rw-r--r--   0        0        0    15509 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/metrics.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:37:21.788829 cognite_extractor_utils-7.2.0/cognite/extractorutils/py.typed
+-rw-r--r--   0        0        0      359 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/statestore/__init__.py
+-rw-r--r--   0        0        0     2712 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/statestore/_base.py
+-rw-r--r--   0        0        0     8083 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/statestore/hashing.py
+-rw-r--r--   0        0        0    16755 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/statestore/watermark.py
+-rw-r--r--   0        0        0     3605 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/threading.py
+-rw-r--r--   0        0        0     3110 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/__init__.py
+-rw-r--r--   0        0        0     5304 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/_base.py
+-rw-r--r--   0        0        0     3247 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/_metrics.py
+-rw-r--r--   0        0        0     5628 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/assets.py
+-rw-r--r--   0        0        0     3639 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/data_modeling.py
+-rw-r--r--   0        0        0     5680 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/events.py
+-rw-r--r--   0        0        0    18329 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/files.py
+-rw-r--r--   0        0        0     6738 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/raw.py
+-rw-r--r--   0        0        0    26817 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/time_series.py
+-rw-r--r--   0        0        0     7732 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader_extractor.py
+-rw-r--r--   0        0        0     1020 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader_types.py
+-rw-r--r--   0        0        0    17229 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/cognite/extractorutils/util.py
+-rw-r--r--   0        0        0     2125 2024-05-22 11:37:21.792829 cognite_extractor_utils-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5486 1970-01-01 00:00:00.000000 cognite_extractor_utils-7.2.0/PKG-INFO
```

### Comparing `cognite_extractor_utils-7.1.6/LICENSE` & `cognite_extractor_utils-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/README.md` & `cognite_extractor_utils-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/__init__.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 """
 Cognite extractor utils is a Python package that simplifies the development of new extractors.
 """
 
-__version__ = "7.1.6"
+__version__ = "7.2.0"
 from .base import Extractor
```

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/_inner_util.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/_inner_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/base.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/__init__.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/_util.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/_util.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/elements.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/elements.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/configtools/loaders.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/configtools/loaders.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/exceptions.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/metrics.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/statestore.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/statestore/watermark.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,35 +82,29 @@
     # The state store is now updated automatically!
 
     states.synchronize()
 
 """
 
 import json
-import logging
-import threading
-from abc import ABC, abstractmethod
+from abc import ABC
 from types import TracebackType
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, Union
 
 from cognite.client import CogniteClient
 from cognite.client.exceptions import CogniteAPIError
+from cognite.extractorutils._inner_util import _DecimalDecoder, _DecimalEncoder
 from cognite.extractorutils.threading import CancellationToken
 from cognite.extractorutils.uploader import DataPointList
+from cognite.extractorutils.util import cognite_exceptions, retry
 
-from ._inner_util import _DecimalDecoder, _DecimalEncoder, _resolve_log_level
-from .util import cognite_exceptions, retry
+from ._base import RETRIES, RETRY_BACKOFF_FACTOR, RETRY_DELAY, RETRY_MAX_DELAY, _BaseStateStore
 
-RETRY_BACKOFF_FACTOR = 1.5
-RETRY_MAX_DELAY = 60
-RETRY_DELAY = 1
-RETRIES = 10
 
-
-class AbstractStateStore(ABC):
+class AbstractStateStore(_BaseStateStore, ABC):
     """
     Base class for a state store.
 
     Args:
         save_interval: Automatically trigger synchronize each m seconds when run as a thread (use start/stop
             methods).
         trigger_log_level: Log level to log synchronize triggers to.
@@ -121,77 +115,24 @@
     def __init__(
         self,
         save_interval: Optional[int] = None,
         trigger_log_level: str = "DEBUG",
         thread_name: Optional[str] = None,
         cancellation_token: Optional[CancellationToken] = None,
     ):
-        self._initialized = False
-        self._local_state: Dict[str, Dict[str, Any]] = {}
-        self.save_interval = save_interval
-        self.trigger_log_level = _resolve_log_level(trigger_log_level)
-
-        self.logger = logging.getLogger(__name__)
-
-        self.thread = threading.Thread(target=self._run, daemon=cancellation_token is None, name=thread_name)
-        self.lock = threading.RLock()
-        self.cancellation_token = cancellation_token.create_child_token() if cancellation_token else CancellationToken()
+        super().__init__(
+            save_interval=save_interval,
+            trigger_log_level=trigger_log_level,
+            thread_name=thread_name,
+            cancellation_token=cancellation_token,
+        )
 
+        self._local_state: Dict[str, Dict[str, Any]] = {}
         self._deleted: List[str] = []
 
-    def start(self, initialize: bool = True) -> None:
-        """
-        Start saving state periodically if save_interval is set.
-        This calls the synchronize method every save_interval seconds.
-        """
-        if initialize and not self._initialized:
-            self.initialize()
-        if self.save_interval is not None:
-            self.thread.start()
-
-    def stop(self, ensure_synchronize: bool = True) -> None:
-        """
-        Stop synchronize thread if running, and ensure state is saved if ensure_synchronize is True.
-
-        Args:
-            ensure_synchronize (bool): (Optional). Call synchronize one last time after shutting down thread.
-        """
-        self.cancellation_token.cancel()
-        if ensure_synchronize:
-            self.synchronize()
-
-    def _run(self) -> None:
-        """
-        Internal run method for synchronize thread
-        """
-        self.initialize()
-        while not self.cancellation_token.wait(timeout=self.save_interval):
-            try:
-                self.logger.log(self.trigger_log_level, "Triggering scheduled state store synchronization")
-                self.synchronize()
-            except Exception as e:
-                self.logger.error("Unexpected error while synchronizing state store: %s.", str(e))
-
-        # trigger stop event explicitly to drain the queue
-        self.stop(ensure_synchronize=True)
-
-    @abstractmethod
-    def initialize(self, force: bool = False) -> None:
-        """
-        Get states from remote store
-        """
-        pass
-
-    @abstractmethod
-    def synchronize(self) -> None:
-        """
-        Upload states to remote store
-        """
-        pass
-
     def get_state(self, external_id: Union[str, List[str]]) -> Union[Tuple[Any, Any], List[Tuple[Any, Any]]]:
         """
         Get state(s) for external ID(s)
 
         Args:
             external_id: An external ID or list of external IDs to get states for
```

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/threading.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/threading.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/__init__.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_base.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/_metrics.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/_metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/assets.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/events.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/events.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/files.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/files.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/raw.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader/time_series.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_extractor.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/uploader_types.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/uploader_types.py`

 * *Files identical despite different names*

### Comparing `cognite_extractor_utils-7.1.6/cognite/extractorutils/util.py` & `cognite_extractor_utils-7.2.0/cognite/extractorutils/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,19 +315,22 @@
     delay: float,
     max_delay: Optional[float],
     backoff: float,
     jitter: Union[float, Tuple[float, float]],
 ) -> _T2:
     logger = logging.getLogger(__name__)
 
-    while tries and not cancellation_token.is_cancelled:
+    while tries:
         try:
             return f()
 
         except Exception as e:
+            if cancellation_token.is_cancelled:
+                break
+
             if isinstance(exceptions, tuple):
                 for ex_type in exceptions:
                     if isinstance(e, ex_type):
                         break
                 else:
                     raise e
```

### Comparing `cognite_extractor_utils-7.1.6/pyproject.toml` & `cognite_extractor_utils-7.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-extractor-utils"
-version = "7.1.6"
+version = "7.2.0"
 description = "Utilities for easier development of extractors for CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/python-extractor-utils"
 
 packages = [
@@ -61,14 +61,15 @@
 psutil = "^5.7.0"
 decorator = "^5.1.1"
 more-itertools = "^10.0.0"
 typing-extensions = ">=3.7.4, <5"
 python-dotenv = "^1.0.0"
 azure-identity = "^1.14.0"
 azure-keyvault-secrets = "^4.7.0"
+orjson = "^3.10.3"
 
 [tool.poetry.extras]
 experimental = ["cognite-sdk-experimental"]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.10.0"
 ruff = "^0.4.0"
@@ -80,11 +81,12 @@
 SecretStorage = "^3.1.2"
 twine = "^5.0.0"
 pytest-order = "^1.0.1"
 parameterized = "*"
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240125"
 httpx = "^0.27.0"
+faker = "^25.2.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cognite_extractor_utils-7.1.6/PKG-INFO` & `cognite_extractor_utils-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-extractor-utils
-Version: 7.1.6
+Version: 7.2.0
 Summary: Utilities for easier development of extractors for CDF
 Home-page: https://github.com/cognitedata/python-extractor-utils
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,15 @@
 Requires-Dist: arrow (>=1.0.0,<2.0.0)
 Requires-Dist: azure-identity (>=1.14.0,<2.0.0)
 Requires-Dist: azure-keyvault-secrets (>=4.7.0,<5.0.0)
 Requires-Dist: cognite-sdk (>=7.43.3,<8.0.0)
 Requires-Dist: dacite (>=1.6.0,<2.0.0)
 Requires-Dist: decorator (>=5.1.1,<6.0.0)
 Requires-Dist: more-itertools (>=10.0.0,<11.0.0)
+Requires-Dist: orjson (>=3.10.3,<4.0.0)
 Requires-Dist: prometheus-client (>0.7.0,<=1.0.0)
 Requires-Dist: psutil (>=5.7.0,<6.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: pyyaml (>=5.3.0,<7)
 Requires-Dist: typing-extensions (>=3.7.4,<5)
 Project-URL: Repository, https://github.com/cognitedata/python-extractor-utils
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.1.6 Summary:
+Metadata-Version: 2.1 Name: cognite-extractor-utils Version: 7.2.0 Summary:
 Utilities for easier development of extractors for CDF Home-page: https://
 github.com/cognitedata/python-extractor-utils License: Apache-2.0 Author:
 Mathias Lohne Author-email: mathias.lohne@cognite.com Requires-Python:
 >=3.8.0,<4.0.0 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: experimental Requires-Dist: arrow (>=1.0.0,<2.0.0) Requires-
 Dist: azure-identity (>=1.14.0,<2.0.0) Requires-Dist: azure-keyvault-secrets
 (>=4.7.0,<5.0.0) Requires-Dist: cognite-sdk (>=7.43.3,<8.0.0) Requires-Dist:
 dacite (>=1.6.0,<2.0.0) Requires-Dist: decorator (>=5.1.1,<6.0.0) Requires-
-Dist: more-itertools (>=10.0.0,<11.0.0) Requires-Dist: prometheus-client
-(>0.7.0,<=1.0.0) Requires-Dist: psutil (>=5.7.0,<6.0.0) Requires-Dist: python-
-dotenv (>=1.0.0,<2.0.0) Requires-Dist: pyyaml (>=5.3.0,<7) Requires-Dist:
-typing-extensions (>=3.7.4,<5) Project-URL: Repository, https://github.com/
-cognitedata/python-extractor-utils Description-Content-Type: text/markdown
-_[_C_o_g_n_i_t_e_ _l_o_g_o_]Cognite Python `extractor-utils` ================================
-[![Build Status](https://github.com/cognitedata/python-extractor-utils/
-workflows/release/badge.svg)](https://github.com/cognitedata/python-extractor-
-utils/actions) [![Documentation Status](https://readthedocs.com/projects/
-cognite-extractor-utils/badge/
+Dist: more-itertools (>=10.0.0,<11.0.0) Requires-Dist: orjson (>=3.10.3,<4.0.0)
+Requires-Dist: prometheus-client (>0.7.0,<=1.0.0) Requires-Dist: psutil
+(>=5.7.0,<6.0.0) Requires-Dist: python-dotenv (>=1.0.0,<2.0.0) Requires-Dist:
+pyyaml (>=5.3.0,<7) Requires-Dist: typing-extensions (>=3.7.4,<5) Project-URL:
+Repository, https://github.com/cognitedata/python-extractor-utils Description-
+Content-Type: text/markdown _[_C_o_g_n_i_t_e_ _l_o_g_o_]Cognite Python `extractor-utils`
+================================ [![Build Status](https://github.com/
+cognitedata/python-extractor-utils/workflows/release/badge.svg)](https://
+github.com/cognitedata/python-extractor-utils/actions) [![Documentation Status]
+(https://readthedocs.com/projects/cognite-extractor-utils/badge/
 ?version=latest&token=a9bab88214cbf624706005f6a71bbd77964efc910f8e527c7b3d75edc016397c)]
 (https://cognite-extractor-utils.readthedocs-hosted.com/en/latest/
 ?badge=latest) [![codecov](https://codecov.io/gh/cognitedata/python-extractor-
 utils/branch/master/graph/badge.svg?token=7AmVCpAh7I)](https://codecov.io/gh/
 cognitedata/python-extractor-utils) [![PyPI version](https://badge.fury.io/py/
 cognite-extractor-utils.svg)](https://pypi.org/project/cognite-extractor-utils)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cognite-
```

