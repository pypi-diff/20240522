# Comparing `tmp/synnax_freighter-0.6.9.tar.gz` & `tmp/synnax_freighter-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnax_freighter-0.6.9.tar", max compression
+gzip compressed data, was "synnax_freighter-0.7.1.tar", max compression
```

## Comparing `synnax_freighter-0.6.9.tar` & `synnax_freighter-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1233 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/__init__.py
--rw-r--r--   0        0        0     2101 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/alamos.py
--rw-r--r--   0        0        0     1521 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/context.py
--rw-r--r--   0        0        0     2652 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/encoder.py
--rw-r--r--   0        0        0     4170 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/exceptions.py
--rw-r--r--   0        0        0     4130 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/http.py
--rw-r--r--   0        0        0     6923 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/stream.py
--rw-r--r--   0        0        0     8026 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/sync.py
--rw-r--r--   0        0        0     4649 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/transport.py
--rw-r--r--   0        0        0     2048 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/unary.py
--rw-r--r--   0        0        0     2143 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/url.py
--rw-r--r--   0        0        0      694 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/util/__init__.py
--rw-r--r--   0        0        0     1005 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/util/asyncio.py
--rw-r--r--   0        0        0      969 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/util/threading.py
--rw-r--r--   0        0        0     6349 2024-04-19 14:21:30.862753 synnax_freighter-0.6.9/freighter/websocket.py
--rw-r--r--   0        0        0      846 2024-04-19 14:21:42.018752 synnax_freighter-0.6.9/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 synnax_freighter-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1233 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/__init__.py
+-rw-r--r--   0        0        0     2101 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/alamos.py
+-rw-r--r--   0        0        0     1521 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/context.py
+-rw-r--r--   0        0        0     2652 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/encoder.py
+-rw-r--r--   0        0        0     4650 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/exceptions.py
+-rw-r--r--   0        0        0     4130 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/http.py
+-rw-r--r--   0        0        0     6923 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/stream.py
+-rw-r--r--   0        0        0     8026 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/sync.py
+-rw-r--r--   0        0        0     4649 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/transport.py
+-rw-r--r--   0        0        0     2048 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/unary.py
+-rw-r--r--   0        0        0     2143 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/url.py
+-rw-r--r--   0        0        0      694 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/__init__.py
+-rw-r--r--   0        0        0     1005 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/asyncio.py
+-rw-r--r--   0        0        0      969 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/util/threading.py
+-rw-r--r--   0        0        0     6349 2024-05-21 21:42:40.773337 synnax_freighter-0.7.1/freighter/websocket.py
+-rw-r--r--   0        0        0      847 2024-05-21 21:42:51.541265 synnax_freighter-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 synnax_freighter-0.7.1/PKG-INFO
```

### Comparing `synnax_freighter-0.6.9/freighter/__init__.py` & `synnax_freighter-0.7.1/freighter/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/alamos.py` & `synnax_freighter-0.7.1/freighter/alamos.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/context.py` & `synnax_freighter-0.7.1/freighter/context.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/encoder.py` & `synnax_freighter-0.7.1/freighter/encoder.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/exceptions.py` & `synnax_freighter-0.7.1/freighter/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,156 +3,124 @@
 #  Use of this software is governed by the Business Source License included in the file
 #  licenses/BSL.txt.
 #
 #  As of the Change Date specified in that file, in accordance with the Business Source
 #  License, use of this software will be governed by the Apache License, Version 2.0,
 #  included in the file licenses/APL.txt.
 
-from dataclasses import dataclass
-from typing import Callable
+from __future__ import annotations
 
-from freighter.transport import Payload
+from typing import Type
 
-_TYPE_UNKNOWN = "unknown"
-_TYPE_NONE = "nil"
+import urllib3
+from urllib3 import PoolManager
+from urllib3.exceptions import HTTPError, MaxRetryError
+from urllib3.response import BaseHTTPResponse
+
+from freighter.context import Context, Role
+from freighter.encoder import EncoderDecoder
+from freighter.exceptions import ExceptionPayload, Unreachable, decode_exception
+from freighter.transport import RQ, RS, MiddlewareCollector
+from freighter.unary import UnaryClient
+from freighter.url import URL
+
+
+class HTTPClient(MiddlewareCollector):
+    """HTTPClientFactory provides a factory for creating POST and GET implementation of
+    the UnaryClient protocol.
+    """
+
+    __ERROR_ENCODING_HEADER_KEY = "Error-Encoding"
+    __ERROR_ENCODING_HEADER_VALUE = "freighter"
+    __CONTENT_TYPE_HEADER_KEY = "Content-Type"
+    __pool: PoolManager
+    __endpoint: URL
+    __encoder_decoder: EncoderDecoder
+    __secure: bool
+
+    def __init__(
+        self,
+        url: URL,
+        encoder_decoder: EncoderDecoder,
+        secure: bool = False,
+        **kwargs,
+    ):
+        """
+        :param url: The base URL for the client.
+        :param encoder_decoder: The encoder/decoder to use for the client.
+        :param secure: Whether to use HTTPS.
+        """
+        super().__init__()
+        self.__endpoint = url
+        self.__endpoint.protocol = "https" if secure else "http"
+        self.__encoder_decoder = encoder_decoder
+        self.__secure = secure
+        self.__pool = PoolManager(cert_reqs="CERT_NONE", **kwargs)
+        urllib3.disable_warnings()
+
+    def __(self) -> UnaryClient:
+        return self
+
+    def send(
+        self, target: str, req: RQ, res_t: Type[RS]
+    ) -> tuple[RS, None] | tuple[None, Exception]:
+        """Implements the UnaryClient protocol."""
+        return self.request(
+            "POST",
+            self.__endpoint.child(target).stringify(),
+            "client",
+            req,
+            res_t,
+        )
+
+    @property
+    def __headers(self) -> dict[str, str]:
+        return {
+            self.__CONTENT_TYPE_HEADER_KEY: self.__encoder_decoder.content_type(),
+            self.__ERROR_ENCODING_HEADER_KEY: self.__ERROR_ENCODING_HEADER_VALUE,
+        }
+
+    def request(
+        self,
+        method: str,
+        url: str,
+        role: Role,
+        request: RQ | None = None,
+        res_t: Type[RS] | None = None,
+    ) -> tuple[RS, None] | tuple[None, Exception]:
+        in_ctx = Context(url, self.__endpoint.protocol, role)
+
+        res: RS | None = None
+
+        def finalizer(ctx: Context) -> tuple[Context, Exception | None]:
+            nonlocal res
+            out_meta_data = Context(url, self.__endpoint.protocol, role)
+            data = None
+            if request is not None:
+                data = self.__encoder_decoder.encode(request)
+
+            head = {**self.__headers, **ctx.params}
+
+            http_res: BaseHTTPResponse
+            try:
+                http_res = self.__pool.request(
+                    method=method, url=url, headers=head, body=data
+                )
+            except MaxRetryError as e:
+                return out_meta_data, Unreachable(url, e.url)
+            except HTTPError as e:
+                return out_meta_data, e
+
+            out_meta_data.params = http_res.headers
+
+            if http_res.status < 200 or http_res.status >= 300:
+                err = self.__encoder_decoder.decode(http_res.data, ExceptionPayload)
+                return out_meta_data, decode_exception(err)
 
+            if http_res.data is None:
+                return out_meta_data, None
 
-class ExceptionPayload(Payload):
-    """Error payload is a payload that can be sent between a freighter client and server,
-    so that it can be decoded into a proper exception by the implementing language.
-    """
-
-    type: str | None
-    data: str | None
-
-
-EncoderFunc = Callable[[Exception], ExceptionPayload | None]
-DecoderFunc = Callable[[ExceptionPayload], Exception | None]
-
-
-@dataclass
-class _ExceptionProvider:
-    encode: EncoderFunc
-    decode: DecoderFunc
-
-
-class _Registry:
-    providers: list[_ExceptionProvider]
-
-    def __init__(self):
-        self.providers = list()
-
-    def register(self, provider: _ExceptionProvider) -> None:
-        self.providers.append(provider)
-
-    @staticmethod
-    def encode(error: Exception | None) -> ExceptionPayload:
-        raise NotImplemented
-
-    def decode(self, encoded: ExceptionPayload) -> Exception | None:
-        assert isinstance(encoded, ExceptionPayload)
-        if encoded.type == _TYPE_NONE:
-            return None
-        for provider in self.providers:
-            decoded = provider.decode(encoded)
-            if decoded is not None:
-                return decoded
-        return Exception(encoded.data)
-
-
-REGISTRY = _Registry()
-
-
-def register_exception(_encode: EncoderFunc, _decode: DecoderFunc) -> None:
-    """Registers a custom error encoder and decoder with the freighter error registry,
-    which allows
-    it to be sent over the network.
-
-    :param _encode: A function that takes an exception and returns a string.
-    :param _decode: A function that takes a string and returns an exception.
-    :return: None
-    """
-    REGISTRY.register(_ExceptionProvider(_encode, _decode))
-
-
-def encode_exception(exc: Exception) -> ExceptionPayload:
-    """Encodes an exception into a payload that can be sent between a freighter server
-    and client.
-
-    :param exc: The exception to encode.
-    :return: The encoded error payload.
-    """
-    return REGISTRY.encode(exc)
-
-
-def decode_exception(encoded: ExceptionPayload | None) -> Exception | None:
-    """Decode decodes an error payload into an exception. If a custom decoder can be found
-    for the error type, it will be used. Otherwise, a generic Exception containing the
-    error data is returned.
-
-    :param encoded: The encoded error payload.
-    :return: The decoded exception.
-    """
-    return None if encoded is None else REGISTRY.decode(encoded)
-
-
-class Unreachable(Exception):
-    """
-    Raise when a target is unreachable.
-    """
-
-    target: str
-    message: str
-
-    def __init__(self, target: str = "", message="Unreachable"):
-        self.target = target
-        self.message = message
-        super().__init__(message)
-
-    def __str__(self):
-        return self.message
-
-
-class StreamClosed(Exception):
-    """
-    Raised when a stream is closed.
-    """
-
-    def __str__(self):
-        return "StreamClosed"
-
-
-class EOF(Exception):
-    """
-    Raised when a stream is closed.
-    """
-
-    def __str__(self):
-        return "EOF"
-
-
-_EXCEPTIONS = [
-    Unreachable,
-    StreamClosed,
-    EOF,
-]
-
-_FREIGHTER_EXCEPTION_TYPE = "freighter.exceptions"
-
-
-def _freighter_encode(exc: Exception) -> ExceptionPayload | None:
-    return ExceptionPayload(type=_FREIGHTER_EXCEPTION_TYPE, data=str(exc))
-
-
-def _freighter_decode(exc: ExceptionPayload) -> Exception | None:
-    if exc.type != "freighter":
-        return None
-    if exc.data == "Unreachable":
-        return Unreachable()
-    if exc.data == "StreamClosed":
-        return StreamClosed()
-    if exc.data == "EOF":
-        return EOF()
-    raise ValueError(f"Unknown freighter exception: {exc}")
-
+            res = self.__encoder_decoder.decode(http_res.data, res_t)
+            return out_meta_data, None
 
-register_exception(_freighter_encode, _freighter_decode)
+        _, exc = self.exec(in_ctx, finalizer)
+        return res, exc
```

### Comparing `synnax_freighter-0.6.9/freighter/stream.py` & `synnax_freighter-0.7.1/freighter/stream.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/sync.py` & `synnax_freighter-0.7.1/freighter/sync.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/transport.py` & `synnax_freighter-0.7.1/freighter/transport.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/unary.py` & `synnax_freighter-0.7.1/freighter/unary.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/url.py` & `synnax_freighter-0.7.1/freighter/url.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/util/__init__.py` & `synnax_freighter-0.7.1/freighter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/util/asyncio.py` & `synnax_freighter-0.7.1/freighter/util/asyncio.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/util/threading.py` & `synnax_freighter-0.7.1/freighter/util/threading.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/freighter/websocket.py` & `synnax_freighter-0.7.1/freighter/websocket.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.6.9/pyproject.toml` & `synnax_freighter-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synnax-freighter"
-version = "0.6.9"
+version = "0.7.1"
 description = ""
 authors = ["emiliano bonilla <emilbon99@gmail.com>"]
 packages = [
     { include = "freighter/**/*.py" }
 ]
 
 [tool.mypy]
@@ -17,15 +17,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 websockets = "^11.0.3"
 msgpack = "^1.0.4"
 urllib3 = "^2.0.3"
 janus = "^1.0.0"
 pydantic = "^1.10.0"
-alamos = "^0.3.9"
+alamos = "^0.3.42"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
 mypy = "^1.3.0"
 pytest-cov = "^4.1.0"
```

### Comparing `synnax_freighter-0.6.9/PKG-INFO` & `synnax_freighter-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: synnax-freighter
-Version: 0.6.9
+Version: 0.7.1
 Summary: 
 Author: emiliano bonilla
 Author-email: emilbon99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: alamos (>=0.3.9,<0.4.0)
+Requires-Dist: alamos (>=0.3.42,<0.4.0)
 Requires-Dist: janus (>=1.0.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
```

