# Comparing `tmp/fastapi_mqtt-2.1.1.tar.gz` & `tmp/fastapi_mqtt-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mqtt-2.1.1.tar", max compression
+gzip compressed data, was "fastapi_mqtt-2.2.0.tar", max compression
```

## Comparing `fastapi_mqtt-2.1.1.tar` & `fastapi_mqtt-2.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/LICENSE
--rw-r--r--   0        0        0     4871 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/README.md
--rw-r--r--   0        0        0      377 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/fastapi_mqtt/__init__.py
--rw-r--r--   0        0        0     2276 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/fastapi_mqtt/config.py
--rw-r--r--   0        0        0    11912 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/fastapi_mqtt/fastmqtt.py
--rw-r--r--   0        0        0     2170 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/fastapi_mqtt/handlers.py
--rw-r--r--   0        0        0        0 2024-03-10 09:03:13.962663 fastapi_mqtt-2.1.1/fastapi_mqtt/py.typed
--rw-r--r--   0        0        0     1787 2024-03-10 09:03:22.946549 fastapi_mqtt-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     5963 1970-01-01 00:00:00.000000 fastapi_mqtt-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-22 08:58:55.393524 fastapi_mqtt-2.2.0/LICENSE
+-rw-r--r--   0        0        0     5048 2024-05-22 08:58:55.393524 fastapi_mqtt-2.2.0/README.md
+-rw-r--r--   0        0        0      377 2024-05-22 08:58:55.397524 fastapi_mqtt-2.2.0/fastapi_mqtt/__init__.py
+-rw-r--r--   0        0        0     2310 2024-05-22 08:58:55.397524 fastapi_mqtt-2.2.0/fastapi_mqtt/config.py
+-rw-r--r--   0        0        0    12159 2024-05-22 08:58:55.397524 fastapi_mqtt-2.2.0/fastapi_mqtt/fastmqtt.py
+-rw-r--r--   0        0        0     2459 2024-05-22 08:58:55.397524 fastapi_mqtt-2.2.0/fastapi_mqtt/handlers.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:58:55.397524 fastapi_mqtt-2.2.0/fastapi_mqtt/py.typed
+-rw-r--r--   0        0        0     2120 2024-05-22 08:59:03.273516 fastapi_mqtt-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6023 1970-01-01 00:00:00.000000 fastapi_mqtt-2.2.0/PKG-INFO
```

### Comparing `fastapi_mqtt-2.1.1/LICENSE` & `fastapi_mqtt-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mqtt-2.1.1/README.md` & `fastapi_mqtt-2.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,34 @@
 ```sh
 pip install fastapi-mqtt
 ```
 
 ### 🕹 Guide
 
 ```python
+from contextlib import asynccontextmanager
 from typing import Any
 
 from fastapi import FastAPI
 from gmqtt import Client as MQTTClient
 
 from fastapi_mqtt import FastMQTT, MQTTConfig
 
 mqtt_config = MQTTConfig()
-
 fast_mqtt = FastMQTT(config=mqtt_config)
 
-app = FastAPI()
-fast_mqtt.init_app(app)
+
+@asynccontextmanager
+async def _lifespan(_app: FastAPI):
+    await fast_mqtt.mqtt_startup()
+    yield
+    await fast_mqtt.mqtt_shutdown()
+
+
+app = FastAPI(lifespan=_lifespan)
 
 
 @fast_mqtt.on_connect()
 def connect(client: MQTTClient, flags: int, rc: int, properties: Any):
     client.subscribe("/mqtt")  # subscribing mqtt topic
     print("Connected: ", client, flags, rc, properties)
```

### Comparing `fastapi_mqtt-2.1.1/fastapi_mqtt/config.py` & `fastapi_mqtt-2.2.0/fastapi_mqtt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from ssl import SSLContext
 from typing import Optional, Union
 
 from gmqtt.mqtt.constants import MQTTv50
-from pydantic import BaseModel, ConfigDict
+from pydantic import BaseModel, ConfigDict, Field
 
 
 class MQTTConfig(BaseModel):
     """
     MQTTConfig is main the configuration to be passed client object.
 
     host: To connect MQTT broker, defaults to localhost
@@ -43,15 +43,15 @@
 
     host: str = "localhost"
     port: int = 1883
     ssl: Union[bool, SSLContext] = False
     keepalive: int = 60
     username: Optional[str] = None
     password: Optional[str] = None
-    version: int = MQTTv50
+    version: int = Field(default=MQTTv50, ge=4, le=5)
 
     reconnect_retries: Optional[int] = 1
     reconnect_delay: Optional[int] = 6
 
     will_message_topic: Optional[str] = None
     will_message_payload: Optional[str] = None
     will_delay_interval: Optional[int] = None
```

### Comparing `fastapi_mqtt-2.1.1/fastapi_mqtt/fastmqtt.py` & `fastapi_mqtt-2.2.0/fastapi_mqtt/fastmqtt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 import asyncio
 import logging
 import uuid
 from itertools import zip_longest
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
-from fastapi import FastAPI
 from gmqtt import Client as MQTTClient
 from gmqtt import Message, Subscription
 from gmqtt.mqtt.constants import MQTTv50
 
 from .config import MQTTConfig
-from .handlers import MQTTHandlers
+from .handlers import (
+    MQTTConnectionHandler,
+    MQTTDisconnectHandler,
+    MQTTHandlers,
+    MQTTMessageHandler,
+    MQTTSubscriptionHandler,
+)
 
 try:
     from uvicorn.config import logger as log_info
 except ImportError:
     log_info = logging.getLogger()
 
 
@@ -63,15 +68,15 @@
         self.client._port = config.port
         self.client._keepalive = config.keepalive
         self.client._ssl = config.ssl
         self.client.optimistic_acknowledgement = optimistic_acknowledgement
         self.client._connect_properties = kwargs
         self.client.on_message = self.__on_message
         self.client.on_connect = self.__on_connect
-        self.subscriptions: Dict[str, Tuple[Subscription, List[Callable]]] = {}
+        self.subscriptions: Dict[str, Tuple[Subscription, List[MQTTMessageHandler]]] = {}
         self._logger = mqtt_logger or log_info
         self.mqtt_handlers = MQTTHandlers(self.client, self._logger)
 
         if (
             self.config.will_message_topic
             and self.config.will_message_payload
             and self.config.will_delay_interval
@@ -221,22 +226,22 @@
         """Initial connection for MQTT client, for lifespan startup."""
         await self.connection()
 
     async def mqtt_shutdown(self) -> None:
         """Final disconnection for MQTT client, for lifespan shutdown."""
         await self.client.disconnect()
 
-    def init_app(self, app: FastAPI) -> None:  # pragma: no cover
+    def init_app(self, fastapi_app) -> None:  # pragma: no cover
         """Add startup and shutdown event handlers for app without lifespan."""
 
-        @app.on_event("startup")
+        @fastapi_app.on_event("startup")
         async def startup() -> None:
             await self.mqtt_startup()
 
-        @app.on_event("shutdown")
+        @fastapi_app.on_event("shutdown")
         async def shutdown() -> None:
             await self.mqtt_shutdown()
 
     def subscribe(
         self,
         *topics,
         qos: int = 0,
@@ -245,15 +250,15 @@
         retain_handling_options: int = 0,
         subscription_identifier: Any = None,
     ) -> Callable[..., Any]:
         """
         Decorator method used to subscribe for specific topics.
         """
 
-        def subscribe_handler(handler: Callable) -> Callable:
+        def subscribe_handler(handler: MQTTMessageHandler) -> MQTTMessageHandler:
             self._logger.debug("Subscribe for topics: %s", topics)
             for topic in topics:
                 if topic not in self.subscriptions:
                     subscription = Subscription(
                         topic,
                         qos,
                         no_local,
@@ -286,45 +291,45 @@
         return subscribe_handler
 
     def on_connect(self) -> Callable[..., Any]:
         """
         Decorator method used to handle the connection to MQTT.
         """
 
-        def connect_handler(handler: Callable) -> Callable:
+        def connect_handler(handler: MQTTConnectionHandler) -> MQTTConnectionHandler:
             self._logger.debug("handler accepted")
             return self.mqtt_handlers.on_connect(handler)
 
         return connect_handler
 
     def on_message(self) -> Callable[..., Any]:
         """
         The decorator method is used to subscribe to messages from all topics.
         """
 
-        def message_handler(handler: Callable) -> Callable:
+        def message_handler(handler: MQTTMessageHandler) -> MQTTMessageHandler:
             self._logger.debug("on_message handler accepted")
             return self.mqtt_handlers.on_message(handler)
 
         return message_handler
 
     def on_disconnect(self) -> Callable[..., Any]:
         """
         The Decorator method used wrap disconnect callback.
         """
 
-        def disconnect_handler(handler: Callable) -> Callable:
+        def disconnect_handler(handler: MQTTDisconnectHandler) -> MQTTDisconnectHandler:
             self._logger.debug("on_disconnect handler accepted")
             return self.mqtt_handlers.on_disconnect(handler)
 
         return disconnect_handler
 
     def on_subscribe(self) -> Callable[..., Any]:
         """
         Decorator method is used to obtain subscribed topics and properties.
         """
 
-        def subscribe_handler(handler: Callable):
+        def subscribe_handler(handler: MQTTSubscriptionHandler) -> MQTTSubscriptionHandler:
             self._logger.debug("on_subscribe handler accepted")
             return self.mqtt_handlers.on_subscribe(handler)
 
         return subscribe_handler
```

### Comparing `fastapi_mqtt-2.1.1/fastapi_mqtt/handlers.py` & `fastapi_mqtt-2.2.0/fastapi_mqtt/handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,37 +4,41 @@
 
 from gmqtt import Client as MQTTClient
 
 # client: MQTTClient, topic: str, payload: bytes, qos: int, properties: Any
 MQTTMessageHandler = Callable[[MQTTClient, str, bytes, int, Any], Awaitable[Any]]
 # client: MQTTClient, flags: int, rc: int, properties: Any
 MQTTConnectionHandler = Callable[[MQTTClient, int, int, Any], Any]
+# client: MQTTClient, mid: int, qos: int, properties: Any
+MQTTSubscriptionHandler = Callable[[MQTTClient, int, int, Any], Any]
+# client: MQTTClient, packet: bytes, exc=None
+MQTTDisconnectHandler = Callable[[MQTTClient, bytes, Optional[Exception]], Any]
 
 
 class MQTTHandlers:
     def __init__(self, client: MQTTClient, logger: Logger):
         self._logger = logger
         self.client = client
         self.user_message_handler: Optional[MQTTMessageHandler] = None
         self.user_connect_handler: Optional[MQTTConnectionHandler] = None
 
     def on_message(self, handler: MQTTMessageHandler) -> MQTTMessageHandler:
         self._logger.info("on_message handler accepted")
         self.user_message_handler = handler
         return handler
 
-    def on_subscribe(self, handler: Callable) -> Callable[..., Any]:
+    def on_subscribe(self, handler: MQTTSubscriptionHandler) -> MQTTSubscriptionHandler:
         """
         Decorator method is used to obtain subscribed topics and properties.
         """
         self._logger.info("on_subscribe handler accepted")
         self.client.on_subscribe = handler
         return handler
 
-    def on_disconnect(self, handler: Callable) -> Callable[..., Any]:
+    def on_disconnect(self, handler: MQTTDisconnectHandler) -> MQTTDisconnectHandler:
         self.client.on_disconnect = handler
         return handler
 
     def on_connect(self, handler: MQTTConnectionHandler) -> MQTTConnectionHandler:
         self._logger.info("on_connect handler accepted")
         self.user_connect_handler = handler
         return handler
```

### Comparing `fastapi_mqtt-2.1.1/pyproject.toml` & `fastapi_mqtt-2.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,75 @@
 [tool.poetry]
 name = "fastapi-mqtt"
-version = "2.1.1"
+version = "2.2.0"
 description = "fastapi-mqtt is extension for MQTT protocol"
 authors = ["sabuhish <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mqtt"
 repository = "https://github.com/sabuhish/fastapi-mqtt"
 classifiers = [
     "Intended Audience :: Developers",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [tool.poetry.dependencies]
-python = "^3.7"
-fastapi = ">=0.103"
+python = "^3.8"
 gmqtt = ">=0.6.11"
 pydantic = ">=2.3.0"
-uvicorn = ">=0.19.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = ">=2.9.2,<3"
+fastapi = ">=0.103"
+uvicorn = ">=0.19.0"
 pytest = ">=7.0.0"
 pytest-cov = ">=3.0.0"
 pytest-asyncio = ">=0.16.0"
 async-asgi-testclient = ">=1.4.11"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
-select = ["A", "ASYNC", "B", "BLE", "C", "C4", "E", "F", "FA", "I", "INT", "N", "PIE", "PTH", "RUF", "SIM", "TCH", "W", "YTT"]
 target-version = "py311"
 fix = true
 line-length = 100
 
-[tool.ruff.isort]
+[tool.ruff.lint]
+select = ["A", "ASYNC", "B", "BLE", "C", "C4", "E", "F", "FA", "I", "INT", "N", "PIE", "PTH", "RUF", "SIM", "TCH", "W", "YTT"]
+
+[tool.ruff.lint.isort]
 known-first-party = ["fastapi_mqtt"]
 order-by-type = false
 
+[tool.mypy]
+plugins = ["pydantic.mypy"]
+
+follow_imports = "silent"
+warn_redundant_casts = true
+warn_unused_ignores = true
+disallow_any_generics = true
+check_untyped_defs = true
+no_implicit_reexport = true
+
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+
+
 [tool.pytest.ini_options]
 minversion = 7.0
 asyncio_mode = "auto"
 addopts = "--cov fastapi_mqtt --cov-report term --cov-report html"
 testpaths = "tests"
 log_cli = true
```

### Comparing `fastapi_mqtt-2.1.1/PKG-INFO` & `fastapi_mqtt-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: fastapi-mqtt
-Version: 2.1.1
+Version: 2.2.0
 Summary: fastapi-mqtt is extension for MQTT protocol
 Home-page: https://github.com/sabuhish/fastapi-mqtt
 License: MIT
 Author: sabuhish
 Author-email: sabuhi.shukurov@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: fastapi (>=0.103)
 Requires-Dist: gmqtt (>=0.6.11)
 Requires-Dist: pydantic (>=2.3.0)
-Requires-Dist: uvicorn (>=0.19.0)
 Project-URL: Repository, https://github.com/sabuhish/fastapi-mqtt
 Description-Content-Type: text/markdown
 
 # fastapi-mqtt
 
 MQTT is a lightweight publish/subscribe messaging protocol designed for M2M (machine to machine) telemetry in low bandwidth environments.
 Fastapi-mqtt is the client for working with MQTT.
@@ -65,27 +62,34 @@
 ```sh
 pip install fastapi-mqtt
 ```
 
 ### 🕹 Guide
 
 ```python
+from contextlib import asynccontextmanager
 from typing import Any
 
 from fastapi import FastAPI
 from gmqtt import Client as MQTTClient
 
 from fastapi_mqtt import FastMQTT, MQTTConfig
 
 mqtt_config = MQTTConfig()
-
 fast_mqtt = FastMQTT(config=mqtt_config)
 
-app = FastAPI()
-fast_mqtt.init_app(app)
+
+@asynccontextmanager
+async def _lifespan(_app: FastAPI):
+    await fast_mqtt.mqtt_startup()
+    yield
+    await fast_mqtt.mqtt_shutdown()
+
+
+app = FastAPI(lifespan=_lifespan)
 
 
 @fast_mqtt.on_connect()
 def connect(client: MQTTClient, flags: int, rc: int, properties: Any):
     client.subscribe("/mqtt")  # subscribing mqtt topic
     print("Connected: ", client, flags, rc, properties)
```

