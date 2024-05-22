# Comparing `tmp/galileo_core-0.9.3.tar.gz` & `tmp/galileo_core-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.9.3.tar", max compression
+gzip compressed data, was "galileo_core-1.0.0.tar", max compression
```

## Comparing `galileo_core-0.9.3.tar` & `galileo_core-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,35 @@
--rw-r--r--   0        0        0    10946 2024-04-08 05:10:36.721013 galileo_core-0.9.3/LICENSE
--rw-r--r--   0        0        0       80 2024-04-08 05:10:36.721013 galileo_core-0.9.3/README.md
--rw-r--r--   0        0        0     2323 2024-04-08 05:10:38.125014 galileo_core-0.9.3/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-08 05:10:38.129014 galileo_core-0.9.3/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     6123 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/py.typed
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      890 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      902 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     3905 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0     1934 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0      831 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0     1124 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      149 2024-04-08 05:10:36.721013 galileo_core-0.9.3/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-05-21 23:28:30.890934 galileo_core-1.0.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-05-21 23:28:30.890934 galileo_core-1.0.0/README.md
+-rw-r--r--   0        0        0     2389 2024-05-21 23:28:32.170933 galileo_core-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-21 23:28:32.170933 galileo_core-1.0.0/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      190 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/constants/request_method.py
+-rw-r--r--   0        0        0      424 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     2977 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     6398 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0      369 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/dependencies.py
+-rw-r--r--   0        0        0     1291 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/execution.py
+-rw-r--r--   0        0        0       60 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0     2146 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/helpers/project.py
+-rw-r--r--   0        0        0       60 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/logger.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/py.typed
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/core/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/core/project.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      246 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/execution_status.py
+-rw-r--r--   0        0        0      890 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      795 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     3905 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0      521 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/response.py
+-rw-r--r--   0        0        0     2886 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0      831 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0      840 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/utils/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-21 23:28:30.894934 galileo_core-1.0.0/src/galileo_core/utils/name.py
+-rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 galileo_core-1.0.0/PKG-INFO
```

### Comparing `galileo_core-0.9.3/LICENSE` & `galileo_core-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/pyproject.toml` & `galileo_core-1.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.9.3"
+version = "1.0.0"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
 pydantic = "^2.6.0"
 pydantic-settings = "^2.2.1"
-requests = "^2.31.0"
 pyjwt = "^2.8.0"
+importlib-metadata = "^7.1.0"
+httpx = "^0.27.0"
+typing-extensions = "^4.11.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.1.1"
 coverage = "^7.3.4"
 pytest-cov = "^5.0.0"
 pytest-xdist = "^3.5.0"
 pytest-socket = "^0.7.0"
-requests-mock = "^1.11.0"
+respx = "^0.21.1"
+pytest-asyncio = "^0.23.7"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.8.0"
 pre-commit = "^3.5.0"
 invoke = "^2.2.0"
-types-requests = "^2.31.0.20240311"
 types-jwt = "^0.1.3"
 pydantic = { extras = ["mypy"], version = "^2.6.0" }
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -45,20 +47,20 @@
     "-n",
     "auto",
     # Show local variables in tracebacks.
     "--showlocals",
     # Show extra test summary info as specified by chars.
     "-o",
     "console_output_style=progress",
-    # Disable warnings.
-    "--disable-warnings",
     # Show slowest 10 test durations.
     "--durations=10",
     # Disable internet access.
     "--disable-socket",
+    # Enable Unix socket access for async tests.
+    "--allow-unix-socket",
 ]
 
 # Formatters.
 [tool.black]
 line-length = 120
 
 [tool.isort]
```

### Comparing `galileo_core-0.9.3/src/galileo_core/constants/http_headers.py` & `galileo_core-1.0.0/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/src/galileo_core/helpers/config.py` & `galileo_core-1.0.0/src/galileo_core/helpers/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     computed_field,
     field_serializer,
     field_validator,
     model_validator,
 )
 from pydantic_core import Url
 from pydantic_settings import BaseSettings, SettingsConfigDict
-from requests import get, post
 
+from galileo_core.constants.request_method import RequestMethod
 from galileo_core.constants.routes import Routes
 from galileo_core.helpers.api_client import ApiClient
+from galileo_core.helpers.execution import async_run
 from galileo_core.helpers.logger import logger
 
 AGalileoConfig = TypeVar("AGalileoConfig", bound="GalileoConfig")
 
 
 class GalileoConfig(BaseSettings):
     console_url: HttpUrl
@@ -67,37 +68,41 @@
             print(f"Go to {token_url} to generate a new token.")
             return getpass("🔐 Enter your token:")
 
     def login(self) -> None:
         token_data = {}
         if self.api_key:
             logger.debug("Logging in with API key.")
-            token_data = ApiClient.make_request(
-                post,
-                base_url=str(self.api_url),
-                endpoint=Routes.api_key_login,
-                json=dict(api_key=self.api_key.get_secret_value()),
+            token_data = async_run(
+                ApiClient.make_request(
+                    RequestMethod.POST,
+                    base_url=str(self.api_url),
+                    endpoint=Routes.api_key_login,
+                    json=dict(api_key=self.api_key.get_secret_value()),
+                )
             )
         elif self.username and self.password:
             logger.debug("Logging in with username and password.")
-            token_data = ApiClient.make_request(
-                post,
-                base_url=str(self.api_url),
-                endpoint=Routes.username_login,
-                data=dict(username=self.username, password=self.password.get_secret_value(), auth_method="email"),
+            token_data = async_run(
+                ApiClient.make_request(
+                    RequestMethod.POST,
+                    base_url=str(self.api_url),
+                    endpoint=Routes.username_login,
+                    data=dict(username=self.username, password=self.password.get_secret_value(), auth_method="email"),
+                )
             )
         else:
             logger.debug("No credentials found. Attempting to log in with token.")
 
         if (jwt_token := token_data.get("access_token")) is None:
             logger.debug("No credentials found. Attempting to log in with token.")
             jwt_token = self.get_token_from_ui()
         self.jwt_token = SecretStr(jwt_token)
         logger.debug("Logged in successfully.")
-        self.current_user = self.api_client.request(get, path=Routes.current_user).get("email")
+        self.current_user = self.api_client.request(RequestMethod.GET, path=Routes.current_user).get("email")
         self.write()
         print(f"👋 You have logged into 🔭 Galileo ({self.console_url}) as {self.current_user}.")
 
     def refresh_jwt_token(self) -> None:
         """Refresh token if not present or expired."""
         # Check to see if our token is expired before making a request and refresh token if it's expired.
         if self.jwt_token:
@@ -132,15 +137,15 @@
     def http_url(cls, value: str) -> str:
         if value and not (value.startswith("https") or value.startswith("http")):
             value = f"https://{value}"
         return value
 
     @model_validator(mode="after")
     def validate_api_url(self) -> "GalileoConfig":
-        ApiClient.make_request(get, base_url=str(self.api_url), endpoint=Routes.healthcheck)
+        async_run(ApiClient.make_request(RequestMethod.GET, base_url=str(self.api_url), endpoint=Routes.healthcheck))
         return self
 
     @field_serializer("password", "jwt_token", "api_key", when_used="json-unless-none")
     def serialize_secrets(self, value: SecretStr) -> str:
         return value.get_secret_value()
 
     def write(self) -> None:
```

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/action.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/metric.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/metric.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/payload.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/payload.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from functools import cached_property
 from typing import Optional
 
-from pydantic import BaseModel, Field, computed_field, model_validator
+from pydantic import BaseModel, Field, model_validator
 
 
 class Payload(BaseModel):
     input: Optional[str] = Field(default=None, description="Input text to be processed.")
     output: Optional[str] = Field(default=None, description="Output text to be processed.")
 
     @model_validator(mode="after")
     def ensure_input_or_output(self) -> "Payload":
         if not self.input and not self.output:
             raise ValueError("Either input or output must be set.")
         return self
 
-    # https://github.com/python/mypy/issues/1362
-    @computed_field  # type: ignore[misc]
     @cached_property
     def text(self) -> str:
         if self.output:
             return self.output
         elif self.input:
             return self.input
         else:
```

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/request.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/request.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/rule.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,26 @@
     gt = "gt"
     lt = "lt"
     gte = "gte"
     lte = "lte"
     eq = "eq"
     neq = "neq"
     contains = "contains"
+    all = "all"
+    any = "any"
+    empty = "empty"
+    not_empty = "not_empty"
 
 
 class Rule(BaseModel):
     metric: str = Field(description="Name of the metric.")
     operator: RuleOperator = Field(description="Operator to use for comparison.")
-    target_value: Union[str, float, int] = Field(description="Value to compare with for this metric (right hand side).")
+    target_value: Union[str, float, int, list, None] = Field(
+        description="Value to compare with for this metric (right hand side)."
+    )
 
     def evaluate(self, value: MetricValueType) -> bool:
         if value is not None:
             if isinstance(value, (float, int)) and isinstance(self.target_value, (float, int)):
                 if self.operator == RuleOperator.gt:
                     return value > self.target_value
                 elif self.operator == RuleOperator.lt:
@@ -32,16 +38,32 @@
                     return value >= self.target_value
                 elif self.operator == RuleOperator.lte:
                     return value <= self.target_value
                 elif self.operator == RuleOperator.eq:
                     return value == self.target_value
                 elif self.operator == RuleOperator.neq:
                     return value != self.target_value
-            elif isinstance(value, str) and isinstance(self.target_value, str):
-                if self.operator == RuleOperator.eq:
-                    return value == self.target_value
-                elif self.operator == RuleOperator.neq:
-                    return value != self.target_value
-            elif isinstance(value, list) and isinstance(self.target_value, str):
-                if self.operator == RuleOperator.contains:
-                    return self.target_value in value
+            elif isinstance(value, str):
+                if isinstance(self.target_value, (str)):
+                    if self.operator == RuleOperator.eq:
+                        return value == self.target_value
+                    elif self.operator == RuleOperator.neq:
+                        return value != self.target_value
+                elif isinstance(self.target_value, list):
+                    if self.operator == RuleOperator.any:
+                        return any([t == value for t in self.target_value])
+            elif isinstance(value, list):
+                if isinstance(self.target_value, str):
+                    if self.operator == RuleOperator.contains:
+                        return self.target_value in value
+                elif isinstance(self.target_value, list):
+                    if self.operator == RuleOperator.all:
+                        return all([v in value for v in self.target_value])
+                    elif self.operator == RuleOperator.any:
+                        return any([v in value for v in self.target_value])
+                elif self.target_value is None:
+                    if self.operator == RuleOperator.empty:
+                        return len(value) == 0
+                    elif self.operator == RuleOperator.not_empty:
+                        return len(value) > 0
+
         return False
```

### Comparing `galileo_core-0.9.3/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-1.0.0/src/galileo_core/schemas/protect/ruleset.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.9.3/PKG-INFO` & `galileo_core-1.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.9.3
+Version: 1.0.0
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: importlib-metadata (>=7.1.0,<8.0.0)
 Requires-Dist: pydantic (>=2.6.0,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # galileo-core
 
 Shared schemas and configuration for Galileo's Python packages.
```

