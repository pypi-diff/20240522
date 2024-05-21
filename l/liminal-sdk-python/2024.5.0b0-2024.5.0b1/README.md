# Comparing `tmp/liminal_sdk_python-2024.5.0b0.tar.gz` & `tmp/liminal_sdk_python-2024.5.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.5.0b0.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.5.0b1.tar", max compression
```

## Comparing `liminal_sdk_python-2024.5.0b0.tar` & `liminal_sdk_python-2024.5.0b1.tar`

### file list

```diff
@@ -1,22 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/LICENSE
--rw-r--r--   0        0        0    12819 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/README.md
--rw-r--r--   0        0        0       82 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/__init__.py
--rw-r--r--   0        0        0      524 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2961 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      873 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0     8055 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/client.py
--rw-r--r--   0        0        0      165 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/const.py
--rw-r--r--   0        0        0       45 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2135 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2090 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0     5463 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3264 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0     2372 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2162 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      400 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-05-02 23:19:50.757433 liminal_sdk_python-2024.5.0b0/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      382 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/liminal/helpers/model.py
--rw-r--r--   0        0        0      109 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/liminal/helpers/typing.py
--rw-r--r--   0        0        0    13901 2024-05-02 23:19:50.761433 liminal_sdk_python-2024.5.0b0/pyproject.toml
--rw-r--r--   0        0        0    13943 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/LICENSE
+-rw-r--r--   0        0        0    12308 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/README.md
+-rw-r--r--   0        0        0       82 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      849 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0    10110 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2064 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0      437 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/llm/schemas.py
+-rw-r--r--   0        0        0     7957 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3322 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0      960 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/prompt/schemas.py
+-rw-r--r--   0        0        0     2562 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2130 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      733 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/endpoints/thread/schemas.py
+-rw-r--r--   0        0        0      400 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      374 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/helpers/model.py
+-rw-r--r--   0        0        0      394 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/helpers/schema.py
+-rw-r--r--   0        0        0      109 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/liminal/helpers/typing.py
+-rw-r--r--   0        0        0    13912 2024-05-21 22:36:57.368243 liminal_sdk_python-2024.5.0b1/pyproject.toml
+-rw-r--r--   0        0        0    13432 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b1/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.5.0b0/LICENSE` & `liminal_sdk_python-2024.5.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b0/README.md` & `liminal_sdk_python-2024.5.0b1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -199,124 +199,96 @@
 
 ## Getting Model Instances
 
 Every LLM instance connected in the Liminal admin dashboard is referred to as a "model
 instance." The SDK provides several methods to interact with model instances:
 
 ```python
-import asyncio
-
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Get all available model instances:
-    model_instances = await liminal.llm.get_available_model_instances()
-    # >>> [ModelInstance(...), ModelInstance(...)]
-
-    # Get a specific model instance (if it exists):
-    model_instance = await liminal.llm.get_model_instance("My Model")
-    # >>> ModelInstance(...)
-
-
-asyncio.run(main())
+# Get all available model instances:
+model_instances = await liminal.llm.get_available_model_instances()
+# >>> [ModelInstance(...), ModelInstance(...)]
+
+# Get a specific model instance (if it exists):
+model_instance = await liminal.llm.get_model_instance("My Model")
+# >>> ModelInstance(...)
 ```
 
 ## Managing Threads
 
 Threads are conversations with an LLM instance:
 
 ```python
-import asyncio
-
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Get all available threads:
-    threads = await liminal.thread.get_available()
-    # >>> [Thread(...), Thread(...)]
-
-    # Get a specific thread by ID:
-    thread = await liminal.thread.get_by_id(123)
-    # >>> Thread(...)
-
-    # Some operations require a model instance:
-    model_instance = await liminal.llm.get_model_instance("My Model")
-
-    # Create a new thread:
-    thread = await liminal.thread.create(model_instance.id, "New Thread")
-    # >>> Thread(...)
-
-
-asyncio.run(main())
+# Get all available threads:
+threads = await liminal.thread.get_available()
+# >>> [Thread(...), Thread(...)]
+
+# Get a specific thread by ID:
+thread = await liminal.thread.get_by_id(123)
+# >>> Thread(...)
+
+# Some operations require a model instance:
+model_instance = await liminal.llm.get_model_instance("My Model")
+
+# Create a new thread:
+thread = await liminal.thread.create(model_instance.id, "New Thread")
+# >>> Thread(...)
 ```
 
 ## Submitting Prompts
 
-Submitting prompts is easy:
-
 ```python
-import asyncio
-
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Prompt operations require a model instance:
-    model_instance = await liminal.llm.get_model_instance(model_instance_name)
-
-    # Prompt operations optionally take an existing thread:
-    thread = await liminal.thread.get_by_id(123)
-    # >>> Thread(...)
-
-    # Analayze a prompt for sensitive info:
-    findings = await liminal.prompt.analyze(
-        model_instance.id, "Here is a sensitive prompt"
-    )
-    # >>> AnalyzeResponse(...)
-
-    # Cleanse input text by applying the policies defined in the Liminal admin
-    # dashboard. You can optionally provide existing analysis finidings; if not
-    # provided, analyze is # called automatically):
-    cleansed = await liminal.prompt.cleanse(
-        model_instance.id,
-        "Here is a sensitive prompt",
-        findings=findings,
-        thread_id=thread.id,
-    )
-    # >>> CleanseResponse(...)
-
-    # Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
-    # findings):
-    response = await liminal.prompt.submit(
-        model_instance.id,
-        "Here is a sensitive prompt",
-        findings=findings,
-        thread_id=thread.id,
-    )
-    # >>> SubmitResponse(...)
-
-    # Rehydrate a response with sensitive data:
-    hydrated = await liminal.prompt.hydrate(
-        model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
-    )
-    # >>> HydrateResponse(...)
-
+# Prompt operations require a model instance:
+model_instance = await liminal.llm.get_model_instance(model_instance_name)
 
-asyncio.run(main())
+# Prompt operations optionally take an existing thread:
+thread = await liminal.thread.get_by_id(123)
+# >>> Thread(...)
+
+# Analayze a prompt for sensitive info:
+findings = await liminal.prompt.analyze(model_instance.id, "Here is a sensitive prompt")
+# >>> AnalyzeResponse(...)
+
+# Cleanse input text by applying the policies defined in the Liminal admin
+# dashboard. You can optionally provide existing analysis finidings; if not
+# provided, analyze is # called automatically):
+cleansed = await liminal.prompt.cleanse(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+# >>> CleanseResponse(...)
+
+# Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
+# findings), and receive the whole response:
+response = await liminal.prompt.submit(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+# >>> SubmitResponse(...)
+
+# Submit a prompt, but this time, stream the response back chunk by chunk:
+response = liminal.prompt.stream(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+async for chunk in resp:
+    # Each chunk is a liminal.endpoints.prompt.models.StreamResponseChunk object:
+    print(chunk.content)
+    print(chunk.finish_reason)
+
+# Rehydrate a response with sensitive data:
+hydrated = await liminal.prompt.hydrate(
+    model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
+)
+# >>> HydrateResponse(...)
 ```
 
 # Connection Pooling
 
 By default, the library creates a new connection to the Liminal API server with each
 coroutine. If you are calling a large number of coroutines (or merely want to squeeze
 out every second of runtime savings possible), an [`httpx`][httpx] `AsyncClient` can be
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/auth/__init__.py` & `liminal_sdk_python-2024.5.0b1/liminal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.5.0b1/liminal/auth/microsoft/device_code_flow.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.5.0b1/liminal/auth/microsoft/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Define models for the auth endpoint."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Literal
 
-from liminal.helpers.model import BaseResponseModel
+from liminal.helpers.model import BaseModel
 
 
 @dataclass(frozen=True, kw_only=True)
-class MSALCacheTokenResponse(BaseResponseModel):
+class MSALCacheTokenResponse(BaseModel):
     """Define an MSAL token response from Entra ID."""
 
     token_type: Literal["Bearer"]
     access_token: str
     expires_in: int
     token_source: Literal["cache"]
 
 
 @dataclass(frozen=True, kw_only=True)
-class MSALIdentityProviderTokenResponse(BaseResponseModel):
+class MSALIdentityProviderTokenResponse(BaseModel):
     """Define an MSAL token response from the local in-memory cache."""
 
     token_type: Literal["Bearer"]
     scope: str
     expires_in: int
     ext_expires_in: int
     access_token: str
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/client.py` & `liminal_sdk_python-2024.5.0b1/liminal/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Define the client module."""
 
 from __future__ import annotations
 
 import asyncio
-from collections.abc import Callable
+from collections.abc import AsyncIterator, Callable
+from contextlib import asynccontextmanager
 from json.decoder import JSONDecodeError
-from typing import Final
+from typing import Any, Final
 
-from httpx import AsyncClient, Cookies, HTTPStatusError, Request, Response
+from httpx import AsyncClient, Cookies, HTTPStatusError, Response
 from mashumaro.codecs.json import json_decode
 from mashumaro.exceptions import (
     MissingField,
     SuitableVariantNotFoundError,
     UnserializableDataError,
 )
 
@@ -53,28 +54,65 @@
         self._refresh_lock = asyncio.Lock()
         self._refreshing = False
         self._session_id: str | None = None
         self._session_id_callbacks: list[Callable[[str], None]] = []
 
         # Define endpoints:
         self.llm = LLMEndpoint(self._request_and_validate)
-        self.prompt = PromptEndpoint(self._request_and_validate)
-        self.thread = ThreadEndpoint(self._request, self._request_and_validate)
+        self.prompt = PromptEndpoint(self._request_and_validate, self._stream)
+        self.thread = ThreadEndpoint(self._request_and_validate)
+
+    def _create_cookie_jar(self, raw_cookies: dict[str, Any] | None) -> Cookies:
+        """Create a cookie jar from raw cookies.
+
+        Args:
+        ----
+            raw_cookies: The raw cookies to use.
+
+        Returns:
+        -------
+            A cookie jar.
+
+        """
+        if not raw_cookies:
+            raw_cookies = {}
+        if self._session_id:
+            raw_cookies["session"] = self._session_id
+        return Cookies(raw_cookies)
+
+    @asynccontextmanager
+    async def _get_httpx_client(self) -> AsyncIterator[AsyncClient]:
+        """Get an HTTPX client.
+
+        Returns
+        -------
+            An HTTPX client.
+
+        """
+        if running_client := self._httpx_client and not self._httpx_client.is_closed:
+            client = self._httpx_client
+        else:
+            client = AsyncClient()
+
+        yield client
+
+        if not running_client:
+            await client.aclose()
 
     async def _request(
         self,
         method: str,
         endpoint: str,
         *,
         headers: dict[str, str] | None = None,
         cookies: dict[str, str] | None = None,
         params: dict[str, str] | None = None,
-        json: dict[str, str] | None = None,
+        json: dict[str, Any] | None = None,
     ) -> Response:
-        """Make a request to the Liminal API server and return a Response.
+        """Make a request to the Liminal API server and return a response.
 
         Args:
         ----
             method: The HTTP method to use.
             endpoint: The endpoint to request.
             headers: The headers to use.
             cookies: The cookies to use.
@@ -87,60 +125,49 @@
 
         Raises:
         ------
             RequestError: If the response fails for any reason.
 
         """
         url = f"{self._api_server_url}{endpoint}"
+        cookie_jar = self._create_cookie_jar(cookies)
 
-        if not cookies:
-            cookies = {}
-        if self._session_id:
-            cookies["session"] = self._session_id
-
-        if running_client := self._httpx_client and not self._httpx_client.is_closed:
-            client = self._httpx_client
-        else:
-            client = AsyncClient()
-
-        request = Request(
-            method,
-            url,
-            headers=headers,
-            cookies=Cookies(cookies),
-            params=params,
-            json=json,
-        )
-        response = await client.send(request)
-
-        try:
-            response.raise_for_status()
-        except HTTPStatusError as err:
-            msg = (
-                f"Error while sending request to {url}: {err.response.content.decode()}"
+        async with self._get_httpx_client() as client:
+            response = await client.request(
+                method,
+                url,
+                headers=headers,
+                cookies=cookie_jar,
+                params=params,
+                json=json,
             )
-            raise RequestError(msg) from err
 
-        if not running_client:
-            await client.aclose()
+            try:
+                response.raise_for_status()
+            except HTTPStatusError as err:
+                msg = (
+                    f"Error while sending request to {url}: "
+                    f"{err.response.content.decode()}"
+                )
+                raise RequestError(msg) from err
 
-        LOGGER.debug("Received data from %s: %s", url, response.content)
+            LOGGER.debug("Received data from %s: %s", url, response.content)
 
-        return response
+            return response
 
     async def _request_and_validate(
         self,
         method: str,
         endpoint: str,
         expected_response_type: type[ValidatedResponseT],
         *,
         headers: dict[str, str] | None = None,
         cookies: dict[str, str] | None = None,
         params: dict[str, str] | None = None,
-        json: dict[str, str] | None = None,
+        json: dict[str, Any] | None = None,
     ) -> ValidatedResponseT:
         """Make a request to the Liminal API server and validate the response.
 
         Args:
         ----
             method: The HTTP method to use.
             endpoint: The endpoint to request.
@@ -185,14 +212,55 @@
         LOGGER.debug("Saving session cookie from auth response")
         self._session_id = auth_response.cookies["session"]
 
         if self._session_id:
             for callback in self._session_id_callbacks:
                 callback(self._session_id)
 
+    async def _stream(
+        self,
+        method: str,
+        endpoint: str,
+        *,
+        headers: dict[str, str] | None = None,
+        cookies: dict[str, str] | None = None,
+        params: dict[str, str] | None = None,
+        json: dict[str, Any] | None = None,
+    ) -> AsyncIterator[bytes]:
+        """Make a request to the Liminal API server and return a streaming response.
+
+        Args:
+        ----
+            method: The HTTP method to use.
+            endpoint: The endpoint to request.
+            headers: The headers to use.
+            cookies: The cookies to use.
+            params: The query parameters to use.
+            json: The JSON body to use.
+
+        Returns:
+        -------
+            An AsyncIterator containing the raw JSON response chunks.
+
+        """
+        url = f"{self._api_server_url}{endpoint}"
+        cookie_jar = self._create_cookie_jar(cookies)
+
+        # pylint: disable=contextmanager-generator-missing-cleanup
+        async with self._get_httpx_client() as client, client.stream(
+            method,
+            url,
+            headers=headers,
+            cookies=cookie_jar,
+            params=params,
+            json=json,
+        ) as resp:
+            async for chunk in resp.aiter_bytes():
+                yield chunk
+
     def add_session_id_callback(
         self, callback: Callable[[str], None]
     ) -> Callable[[], None]:
         """Add a callback to be called when a new session is generated.
 
         The purpose of this is to allow the user to save the session ID to a
         persistent store using their own callback method.
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.5.0b1/liminal/endpoints/llm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from collections.abc import Awaitable, Callable
 from typing import cast
 
 from liminal.endpoints.llm.models import ModelInstance
+from liminal.endpoints.llm.schemas import GetAvailableModelInstancesResponse
 from liminal.errors import ModelInstanceUnknownError
 from liminal.helpers.typing import ValidatedResponseT
 
 
 class LLMEndpoint:
     """Define the LLM endpoint."""
 
@@ -29,20 +30,21 @@
         """Get available model instances.
 
         Returns
         -------
             A list of available model instances.
 
         """
-        return cast(
-            list[ModelInstance],
+        response = cast(
+            GetAvailableModelInstancesResponse,
             await self._request_and_validate(
-                "GET", "/api/v1/model-instances", list[ModelInstance]
+                "GET", "/api/v1/model-instances", GetAvailableModelInstancesResponse
             ),
         )
+        return response.data
 
     async def get_model_instance(self, model_instance_name: str) -> ModelInstance:
         """Get a model instance by name.
 
         Args:
         ----
             model_instance_name: The name of the model instance to retrieve.
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.5.0b1/liminal/endpoints/llm/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from dataclasses import dataclass, field
 from datetime import datetime
 from enum import Enum
 
 from mashumaro import field_options
 
-from liminal.helpers.model import BaseResponseModel
+from liminal.helpers.model import BaseModel
 
 
 # Define enums to use as types:
 class ModelProviderKey(str, Enum):
     """Define the enum for the model provider key."""
 
     ANTHROPIC = "anthropic"
@@ -23,16 +23,16 @@
     HUGGINGFACE = "huggingface"
     MISTRAL = "mistral"
     OLLAMA = "ollama"
     OPENAI = "openai"
 
 
 @dataclass(frozen=True, kw_only=True)
-class ModelConnection(BaseResponseModel):
-    """Define the schema for an LLM model connection."""
+class ModelConnection(BaseModel):
+    """Define the model for an LLM model connection."""
 
     id: int
 
     # References:
     model_instance_id: int = field(metadata=field_options(alias="modelInstanceId"))
 
     # Fields:
@@ -45,16 +45,16 @@
     deleted_at: datetime | None = field(
         default=None, metadata=field_options(alias="deletedAt")
     )
     updated_at: datetime = field(metadata=field_options(alias="updatedAt"))
 
 
 @dataclass(frozen=True, kw_only=True)
-class ModelInstance(BaseResponseModel):
-    """Define the schema for an LLM model instance that Liminal supports."""
+class ModelInstance(BaseModel):
+    """Define the model for an LLM model instance that Liminal supports."""
 
     id: int
 
     # References:
     policy_group_id: int = field(metadata=field_options(alias="policyGroupId"))
 
     # Fields:
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.5.0b1/liminal/endpoints/prompt/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-"""Define models for the LLM endpoint."""
+"""Define models for the prompt endpoint."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 from mashumaro import field_options
 
 from liminal.endpoints.thread.models import DeidentifiedToken
-from liminal.helpers.model import BaseResponseModel
+from liminal.helpers.model import BaseModel
 
 
 @dataclass(frozen=True, kw_only=True)
-class AnalysisFinding(BaseResponseModel):
-    """Define the schema for an analysis finding.
+class AnalysisFinding(BaseModel):
+    """Define a detection analysis finding.
 
     This object stores information about a piece of text from a prompt, what sensitive
     data type was detected, and what the current policy is for this type of data.
     """
 
     start: int
     end: int
@@ -25,67 +25,85 @@
     score_category: str = field(metadata=field_options(alias="scoreCategory"))
     text: str
     type: str
     policy_action: str = field(metadata=field_options(alias="policyAction"))
 
 
 @dataclass(frozen=True, kw_only=True)
-class AnalyzeResponse(BaseResponseModel):
-    """Define the response schema for an analysis request."""
+class AnalysisFindings(BaseModel):
+    """Define consolidated detection analysis findings."""
 
     findings: list[AnalysisFinding]
 
 
 @dataclass(frozen=True, kw_only=True)
-class CleanseResponse(BaseResponseModel):
-    """Define the response schema for a cleanse request."""
+class CleanseData(BaseModel):
+    """Define the result of a cleanse request."""
 
     items: list[CleansedToken]
     # Represents the prompt with the sensitive data replaced with cleansed tokens:
     text: str
     items_hashed: list[CleansedToken]
     # Represents the prompt with the sensitive data replaced with hashed tokens (which
     # are help in mapping):
     text_hashed: str
 
 
 @dataclass(frozen=True, kw_only=True)
-class CleansedToken(BaseResponseModel):
-    """Define the schema for a cleansed token."""
+class CleansedToken(BaseModel):
+    """Define a cleansed token."""
 
     start: int
     end: int
     entity_type: str
 
 
 @dataclass(frozen=True, kw_only=True)
-class HydrateResponse(BaseResponseModel):
-    """Define the response schema for a hydrate request."""
+class HydrateData(BaseModel):
+    """Define the result of a hydration request."""
 
     items: list[HydratedToken]
     text: str
 
 
 @dataclass(frozen=True, kw_only=True)
-class HydratedToken(BaseResponseModel):
-    """Define the schema for a hydrated token."""
+class HydratedToken(BaseModel):
+    """Define a hydrated token."""
 
     end: int
     entity_type: str
     start: int
 
 
 @dataclass(frozen=True, kw_only=True)
-class SubmitResponse(BaseResponseModel):
-    """Define the response schema for a process request."""
+class ReidentifiedToken(BaseModel):
+    """Define a reidentified token."""
+
+    start: int
+    end: int
+    entity_type: str
+    text: str
+
+
+@dataclass(frozen=True, kw_only=True)
+class StreamResponseChunk(BaseModel):
+    """Define a streaming response chunk."""
+
+    content: str
+    finish_reason: str | None = field(metadata=field_options(alias="finishReason"))
+
+
+@dataclass(frozen=True, kw_only=True)
+class SubmitData(BaseModel):
+    """Define the result of a submit request."""
 
     thread_id: int = field(metadata=field_options(alias="threadId"))
     chat_id: int = field(metadata=field_options(alias="chatId"))
     input_text: str = field(metadata=field_options(alias="inputText"))
-    deidentified_input_text_data: CleanseResponse = field(
+    deidentified_input_text_data: CleanseData = field(
         metadata=field_options(alias="deidentifiedInputTextData")
     )
     deidentified_context_history: list[DeidentifiedToken] = field(
         metadata=field_options(alias="deidentifiedContextHistory")
     )
     llm_model: str = field(metadata=field_options(alias="llmModel"))
     raw_llm_response_text: str = field(
@@ -93,17 +111,7 @@
     )
     reidentified_llm_response_text: str = field(
         metadata=field_options(alias="reidentifiedLLMResponseText")
     )
     reidentified_llm_response_items: list[ReidentifiedToken] = field(
         metadata=field_options(alias="reidentifiedLLMResponseItems")
     )
-
-
-@dataclass(frozen=True, kw_only=True)
-class ReidentifiedToken(BaseResponseModel):
-    """Define the schema for a reidentified token."""
-
-    start: int
-    end: int
-    entity_type: str
-    text: str
```

### Comparing `liminal_sdk_python-2024.5.0b0/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.5.0b1/liminal/endpoints/thread/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Literal
 
 from mashumaro import field_options
 
 from liminal.endpoints.llm.models import ModelInstance
-from liminal.helpers.model import BaseResponseModel
+from liminal.helpers.model import BaseModel
 
 
 @dataclass(frozen=True, kw_only=True)
-class DeidentifiedToken(BaseResponseModel):
+class DeidentifiedToken(BaseModel):
     """Define the schema for a deidentified token."""
 
     deid_text: str = field(metadata=field_options(alias="deidText"))
     hash_text: str = field(metadata=field_options(alias="hashText"))
 
 
 @dataclass(frozen=True, kw_only=True)
-class Chat(BaseResponseModel):
+class Chat(BaseModel):
     """Define the schema for a chat."""
 
     id: int
     thread_id: int = field(metadata=field_options(alias="threadId"))
     deidentified_input: str = field(metadata=field_options(alias="deidentifiedInput"))
     dedentified_text: list[DeidentifiedToken] = field(
         metadata=field_options(alias="deidentifiedText")
@@ -41,15 +41,15 @@
     updated_at: datetime | None = field(
         default=None, metadata=field_options(alias="updatedAt")
     )
     deleted_at: datetime = field(metadata=field_options(alias="deletedAt"))
 
 
 @dataclass(frozen=True, kw_only=True)
-class Thread(BaseResponseModel):
+class Thread(BaseModel):
     """Define the schema for a thread."""
 
     id: int
     user_id: int = field(metadata=field_options(alias="userId"))
     model_instance_id: int = field(metadata=field_options(alias="modelInstanceId"))
     name: str
     source: Literal["sdk"]
```

### Comparing `liminal_sdk_python-2024.5.0b0/pyproject.toml` & `liminal_sdk_python-2024.5.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 warn_redundant_casts = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "liminal-sdk-python"
-version = "2024.05.0b0"
+version = "2024.05.0b1"
 description = "The Liminal SDK for Python"
 readme = "README.md"
 authors = ["Aaron Bach <ab@liminal.ai>"]
 license = "Apache-2.0"
 repository = "https://github.com/liminal-ai-security/liminal-sdk-python"
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -54,31 +54,32 @@
     { include="liminal", from="." }
 ]
 
 [tool.poetry.dependencies]
 httpx = "0.27.0"
 msal = "1.28.0"
 python = "^3.11.8"
-mashumaro = "3.12"
+mashumaro = "3.13"
 
 [tool.poetry.group.dev.dependencies]
 blacken-docs = "1.16.0"
 codespell = "2.2.6"
-coverage = {version = "7.5.0", extras = ["toml"]}
+coverage = {version = "7.5.1", extras = ["toml"]}
 darglint = "1.8.1"
 mypy = "1.10.0"
 packaging = "==24.0"
-pre-commit = "3.7.0"
+pre-commit = "3.7.1"
 pre-commit-hooks = "4.6.0"
-pylint = "3.1.0"
+pylint = "3.2.2"
 pytest = "8.2.0"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
 pytest-httpx = "0.30.0"
-ruff = "0.4.2"
+ruff = "0.4.4"
+ruff-lsp = "0.0.53"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/liminal-ai-security/liminal-sdk-python/issues"
 Changelog = "https://github.com/liminal-ai-security/liminal-sdk-python/releases"
 
 [tool.pylint.BASIC]
 class-const-naming-style = "any"
@@ -166,15 +167,14 @@
     "expression-not-assigned",              # B018
     "f-string-without-interpolation",       # F541
     "forgotten-debug-statement",            # T100
     "format-needs-mapping",                 # F502
     "format-string-without-interpolation",  # F
     "function-redefined",                   # F811
     "global-variable-not-assigned",         # PLW0602
-    "if-stmt-min-max",                      # PLR1730, PLR1731
     "implicit-str-concat",                  # ISC001
     "import-self",                          # PLW0406
     "inconsistent-quotes",                  # Q000
     "invalid-all-object",                   # PLE0604
     "invalid-bytes-returned",               # E0308
     "invalid-character-backspace",          # PLE2510
     "invalid-character-esc",                # PLE2513
@@ -236,14 +236,15 @@
     "ungrouped-imports",                    # I001
     "unidiomatic-typecheck",                # E721
     "unnecessary-comprehension",            # C416
     "unnecessary-direct-lambda-call",       # PLC3002
     "unnecessary-lambda-assignment",        # PLC3001
     "unnecessary-pass",                     # PIE790
     "unneeded-not",                         # SIM208
+    "unspecified-encoding",                 # PLW1514
     "unused-argument",                      # ARG001
     "unused-format-string-argument",        # F507
     "unused-format-string-key",             # F504
     "unused-import",                        # F401
     "unused-variable",                      # F841
     "use-a-generator",                      # C417
     "use-dict-literal",                     # C406
```

### Comparing `liminal_sdk_python-2024.5.0b0/PKG-INFO` & `liminal_sdk_python-2024.5.0b1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.5.0b0
+Version: 2024.5.0b1
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: httpx (==0.27.0)
-Requires-Dist: mashumaro (==3.12)
+Requires-Dist: mashumaro (==3.13)
 Requires-Dist: msal (==1.28.0)
 Project-URL: Bug Tracker, https://github.com/liminal-ai-security/liminal-sdk-python/issues
 Project-URL: Changelog, https://github.com/liminal-ai-security/liminal-sdk-python/releases
 Project-URL: Repository, https://github.com/liminal-ai-security/liminal-sdk-python
 Description-Content-Type: text/markdown
 
 # Liminal Python SDK
@@ -224,124 +224,96 @@
 
 ## Getting Model Instances
 
 Every LLM instance connected in the Liminal admin dashboard is referred to as a "model
 instance." The SDK provides several methods to interact with model instances:
 
 ```python
-import asyncio
-
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Get all available model instances:
-    model_instances = await liminal.llm.get_available_model_instances()
-    # >>> [ModelInstance(...), ModelInstance(...)]
-
-    # Get a specific model instance (if it exists):
-    model_instance = await liminal.llm.get_model_instance("My Model")
-    # >>> ModelInstance(...)
-
-
-asyncio.run(main())
+# Get all available model instances:
+model_instances = await liminal.llm.get_available_model_instances()
+# >>> [ModelInstance(...), ModelInstance(...)]
+
+# Get a specific model instance (if it exists):
+model_instance = await liminal.llm.get_model_instance("My Model")
+# >>> ModelInstance(...)
 ```
 
 ## Managing Threads
 
 Threads are conversations with an LLM instance:
 
 ```python
-import asyncio
-
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Get all available threads:
-    threads = await liminal.thread.get_available()
-    # >>> [Thread(...), Thread(...)]
-
-    # Get a specific thread by ID:
-    thread = await liminal.thread.get_by_id(123)
-    # >>> Thread(...)
-
-    # Some operations require a model instance:
-    model_instance = await liminal.llm.get_model_instance("My Model")
-
-    # Create a new thread:
-    thread = await liminal.thread.create(model_instance.id, "New Thread")
-    # >>> Thread(...)
-
-
-asyncio.run(main())
+# Get all available threads:
+threads = await liminal.thread.get_available()
+# >>> [Thread(...), Thread(...)]
+
+# Get a specific thread by ID:
+thread = await liminal.thread.get_by_id(123)
+# >>> Thread(...)
+
+# Some operations require a model instance:
+model_instance = await liminal.llm.get_model_instance("My Model")
+
+# Create a new thread:
+thread = await liminal.thread.create(model_instance.id, "New Thread")
+# >>> Thread(...)
 ```
 
 ## Submitting Prompts
 
-Submitting prompts is easy:
-
 ```python
-import asyncio
+# Prompt operations require a model instance:
+model_instance = await liminal.llm.get_model_instance(model_instance_name)
 
-from liminal import Client
-from liminal.auth.microsoft.device_code_flow import DeviceCodeFlowProvider
-
-
-async def main() -> None:
-    # Assuming you have an authenticated `liminal` object:
-
-    # Prompt operations require a model instance:
-    model_instance = await liminal.llm.get_model_instance(model_instance_name)
-
-    # Prompt operations optionally take an existing thread:
-    thread = await liminal.thread.get_by_id(123)
-    # >>> Thread(...)
-
-    # Analayze a prompt for sensitive info:
-    findings = await liminal.prompt.analyze(
-        model_instance.id, "Here is a sensitive prompt"
-    )
-    # >>> AnalyzeResponse(...)
-
-    # Cleanse input text by applying the policies defined in the Liminal admin
-    # dashboard. You can optionally provide existing analysis finidings; if not
-    # provided, analyze is # called automatically):
-    cleansed = await liminal.prompt.cleanse(
-        model_instance.id,
-        "Here is a sensitive prompt",
-        findings=findings,
-        thread_id=thread.id,
-    )
-    # >>> CleanseResponse(...)
-
-    # Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
-    # findings):
-    response = await liminal.prompt.submit(
-        model_instance.id,
-        "Here is a sensitive prompt",
-        findings=findings,
-        thread_id=thread.id,
-    )
-    # >>> SubmitResponse(...)
-
-    # Rehydrate a response with sensitive data:
-    hydrated = await liminal.prompt.hydrate(
-        model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
-    )
-    # >>> HydrateResponse(...)
-
-
-asyncio.run(main())
+# Prompt operations optionally take an existing thread:
+thread = await liminal.thread.get_by_id(123)
+# >>> Thread(...)
+
+# Analayze a prompt for sensitive info:
+findings = await liminal.prompt.analyze(model_instance.id, "Here is a sensitive prompt")
+# >>> AnalyzeResponse(...)
+
+# Cleanse input text by applying the policies defined in the Liminal admin
+# dashboard. You can optionally provide existing analysis finidings; if not
+# provided, analyze is # called automatically):
+cleansed = await liminal.prompt.cleanse(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+# >>> CleanseResponse(...)
+
+# Submit a prompt to an LLM, cleansing it in the process (once again, providing optional
+# findings), and receive the whole response:
+response = await liminal.prompt.submit(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+# >>> SubmitResponse(...)
+
+# Submit a prompt, but this time, stream the response back chunk by chunk:
+response = liminal.prompt.stream(
+    model_instance.id,
+    "Here is a sensitive prompt",
+    findings=findings,
+    thread_id=thread.id,
+)
+async for chunk in resp:
+    # Each chunk is a liminal.endpoints.prompt.models.StreamResponseChunk object:
+    print(chunk.content)
+    print(chunk.finish_reason)
+
+# Rehydrate a response with sensitive data:
+hydrated = await liminal.prompt.hydrate(
+    model_instance.id, "Here is a response to rehdyrate", thread_id=thread.id
+)
+# >>> HydrateResponse(...)
 ```
 
 # Connection Pooling
 
 By default, the library creates a new connection to the Liminal API server with each
 coroutine. If you are calling a large number of coroutines (or merely want to squeeze
 out every second of runtime savings possible), an [`httpx`][httpx] `AsyncClient` can be
```

