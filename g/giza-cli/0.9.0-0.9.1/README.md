# Comparing `tmp/giza_cli-0.9.0.tar.gz` & `tmp/giza_cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_cli-0.9.0.tar", max compression
+gzip compressed data, was "giza_cli-0.9.1.tar", max compression
```

## Comparing `giza_cli-0.9.0.tar` & `giza_cli-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2024-01-31 14:27:20.257239 giza_cli-0.9.0/LICENSE
--rw-r--r--   0        0        0     4860 2024-01-31 14:27:20.257239 giza_cli-0.9.0/README.md
--rw-r--r--   0        0        0      125 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/__init__.py
--rw-r--r--   0        0        0       77 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/__main__.py
--rw-r--r--   0        0        0     1039 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/callbacks.py
--rw-r--r--   0        0        0     7026 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/cli.py
--rw-r--r--   0        0        0    41238 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/client.py
--rw-r--r--   0        0        0        0 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/__init__.py
--rw-r--r--   0        0        0      687 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/actions.py
--rw-r--r--   0        0        0    12004 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/deployments.py
--rw-r--r--   0        0        0     6384 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/models.py
--rw-r--r--   0        0        0     1208 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/prove.py
--rw-r--r--   0        0        0     3904 2024-01-31 14:27:20.261239 giza_cli-0.9.0/giza/commands/reset_password.py
--rw-r--r--   0        0        0     9566 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/commands/users.py
--rw-r--r--   0        0        0     1331 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/commands/verify.py
--rw-r--r--   0        0        0      669 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/commands/version.py
--rw-r--r--   0        0        0    12396 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/commands/versions.py
--rw-r--r--   0        0        0     6008 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/commands/workspaces.py
--rw-r--r--   0        0        0       41 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/exceptions.py
--rw-r--r--   0        0        0        0 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/frameworks/__init__.py
--rw-r--r--   0        0        0    17555 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/frameworks/cairo.py
--rw-r--r--   0        0        0    12580 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/frameworks/ezkl.py
--rw-r--r--   0        0        0      241 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/options.py
--rw-r--r--   0        0        0      715 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/deployments.py
--rw-r--r--   0        0        0      630 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/jobs.py
--rw-r--r--   0        0        0      112 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/message.py
--rw-r--r--   0        0        0      360 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/models.py
--rw-r--r--   0        0        0      347 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/proofs.py
--rw-r--r--   0        0        0      107 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/token.py
--rw-r--r--   0        0        0      958 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/users.py
--rw-r--r--   0        0        0      645 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/versions.py
--rw-r--r--   0        0        0      136 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/schemas/workspaces.py
--rw-r--r--   0        0        0     1161 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/utils/__init__.py
--rw-r--r--   0        0        0     1358 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/utils/decorators.py
--rw-r--r--   0        0        0     4398 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/utils/echo.py
--rw-r--r--   0        0        0      718 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/utils/enums.py
--rw-r--r--   0        0        0      595 2024-01-31 14:27:20.265239 giza_cli-0.9.0/giza/utils/misc.py
--rw-r--r--   0        0        0     2013 2024-01-31 14:27:20.265239 giza_cli-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5806 1970-01-01 00:00:00.000000 giza_cli-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-02-07 10:12:24.570864 giza_cli-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1531 2024-02-07 10:12:24.570864 giza_cli-0.9.1/README.md
+-rw-r--r--   0        0        0      125 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/__init__.py
+-rw-r--r--   0        0        0       77 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/__main__.py
+-rw-r--r--   0        0        0     1039 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/callbacks.py
+-rw-r--r--   0        0        0     7026 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/cli.py
+-rw-r--r--   0        0        0    41782 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/client.py
+-rw-r--r--   0        0        0        0 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/__init__.py
+-rw-r--r--   0        0        0      687 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/actions.py
+-rw-r--r--   0        0        0    12004 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/deployments.py
+-rw-r--r--   0        0        0     6384 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/models.py
+-rw-r--r--   0        0        0     1208 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/prove.py
+-rw-r--r--   0        0        0     3904 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/reset_password.py
+-rw-r--r--   0        0        0     9566 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/users.py
+-rw-r--r--   0        0        0     1331 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/verify.py
+-rw-r--r--   0        0        0      669 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/version.py
+-rw-r--r--   0        0        0    12396 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/versions.py
+-rw-r--r--   0        0        0     6008 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/commands/workspaces.py
+-rw-r--r--   0        0        0       41 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/frameworks/__init__.py
+-rw-r--r--   0        0        0    17555 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/frameworks/cairo.py
+-rw-r--r--   0        0        0    12580 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/frameworks/ezkl.py
+-rw-r--r--   0        0        0      241 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/options.py
+-rw-r--r--   0        0        0      715 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/deployments.py
+-rw-r--r--   0        0        0      630 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/jobs.py
+-rw-r--r--   0        0        0      112 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/message.py
+-rw-r--r--   0        0        0      360 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/models.py
+-rw-r--r--   0        0        0      347 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/proofs.py
+-rw-r--r--   0        0        0      107 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/token.py
+-rw-r--r--   0        0        0      958 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/users.py
+-rw-r--r--   0        0        0      645 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/versions.py
+-rw-r--r--   0        0        0      136 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/schemas/workspaces.py
+-rw-r--r--   0        0        0     1161 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/utils/__init__.py
+-rw-r--r--   0        0        0     1358 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/utils/decorators.py
+-rw-r--r--   0        0        0     4398 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/utils/echo.py
+-rw-r--r--   0        0        0      718 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/utils/enums.py
+-rw-r--r--   0        0        0      595 2024-02-07 10:12:24.574864 giza_cli-0.9.1/giza/utils/misc.py
+-rw-r--r--   0        0        0     2013 2024-02-07 10:12:24.578864 giza_cli-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 giza_cli-0.9.1/PKG-INFO
```

### Comparing `giza_cli-0.9.0/LICENSE` & `giza_cli-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/callbacks.py` & `giza_cli-0.9.1/giza/callbacks.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/cli.py` & `giza_cli-0.9.1/giza/cli.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/client.py` & `giza_cli-0.9.1/giza/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,21 +460,23 @@
         Returns:
             The recently created deployment information
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.post(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                ]
             ),
             headers=headers,
             params=deployment_create.dict(),
             files={"sierra": f} if f is not None else None,
         )
         self._echo_debug(str(response))
 
@@ -490,21 +492,23 @@
         Returns:
             A list of deployments created by the user
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                ]
             ),
             headers=headers,
         )
         self._echo_debug(str(response))
 
         response.raise_for_status()
 
@@ -522,23 +526,25 @@
         Returns:
             A list of proofs created by the user
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
-                str(deployment_id),
-                "proofs",
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                    str(deployment_id),
+                    "proofs",
+                ]
             ),
             headers=headers,
         )
         self._echo_debug(str(response))
 
         response.raise_for_status()
 
@@ -555,24 +561,26 @@
         Returns:
             A proof created by the user
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
-                str(deployment_id),
-                "proofs",
-                str(proof_id),
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                    str(deployment_id),
+                    "proofs",
+                    str(proof_id),
+                ]
             ),
             headers=headers,
         )
         self._echo_debug(str(response))
 
         response.raise_for_status()
 
@@ -591,24 +599,26 @@
         Returns:
             The proof binary file
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
-                str(deployment_id),
-                "proofs",
-                f"{proof_id}:download",
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                    str(deployment_id),
+                    "proofs",
+                    f"{proof_id}:download",
+                ]
             ),
             headers=headers,
         )
 
         self._echo_debug(str(response))
         response.raise_for_status()
 
@@ -632,22 +642,24 @@
         Returns:
             The deployment information
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.DEPLOYMENTS_ENDPOINT,
-                str(deployment_id),
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.DEPLOYMENTS_ENDPOINT,
+                    str(deployment_id),
+                ]
             ),
             headers=headers,
         )
 
         self._echo_debug(str(response))
         response.raise_for_status()
 
@@ -924,22 +936,24 @@
         Returns:
             Job: job entity with the retrieved information
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.JOBS_ENDPOINT,
-                str(job_id),
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.JOBS_ENDPOINT,
+                    str(job_id),
+                ]
             ),
             headers=headers,
         )
         self._echo_debug(str(response))
 
         response.raise_for_status()
 
@@ -961,21 +975,23 @@
 
         Returns:
             Tuple[Model, str]: the recently created model and a url, used to upload the model.
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
         response = self.session.post(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.JOBS_ENDPOINT,
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.JOBS_ENDPOINT,
+                ]
             ),
             headers=headers,
             params=job_create.dict(),
             files={"file": f},
         )
         self._echo_debug(str(response))
 
@@ -991,21 +1007,23 @@
         Returns:
             A list of jobs created by the user
         """
         headers = copy.deepcopy(self.default_headers)
         headers.update(self._get_auth_header())
 
         response = self.session.get(
-            os.path.join(
-                self.url,
-                self.MODELS_ENDPOINT,
-                str(model_id),
-                self.VERSIONS_ENDPOINT,
-                str(version_id),
-                self.JOBS_ENDPOINT,
+            "/".join(
+                [
+                    self.url,
+                    self.MODELS_ENDPOINT,
+                    str(model_id),
+                    self.VERSIONS_ENDPOINT,
+                    str(version_id),
+                    self.JOBS_ENDPOINT,
+                ]
             ),
             headers=headers,
         )
         self._echo_debug(str(response))
 
         response.raise_for_status()
```

### Comparing `giza_cli-0.9.0/giza/commands/actions.py` & `giza_cli-0.9.1/giza/commands/actions.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/deployments.py` & `giza_cli-0.9.1/giza/commands/deployments.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/models.py` & `giza_cli-0.9.1/giza/commands/models.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/prove.py` & `giza_cli-0.9.1/giza/commands/prove.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/reset_password.py` & `giza_cli-0.9.1/giza/commands/reset_password.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/users.py` & `giza_cli-0.9.1/giza/commands/users.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/verify.py` & `giza_cli-0.9.1/giza/commands/verify.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/version.py` & `giza_cli-0.9.1/giza/commands/version.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/versions.py` & `giza_cli-0.9.1/giza/commands/versions.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/commands/workspaces.py` & `giza_cli-0.9.1/giza/commands/workspaces.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/frameworks/cairo.py` & `giza_cli-0.9.1/giza/frameworks/cairo.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/frameworks/ezkl.py` & `giza_cli-0.9.1/giza/frameworks/ezkl.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/schemas/deployments.py` & `giza_cli-0.9.1/giza/schemas/deployments.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/schemas/jobs.py` & `giza_cli-0.9.1/giza/schemas/jobs.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/schemas/users.py` & `giza_cli-0.9.1/giza/schemas/users.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/schemas/versions.py` & `giza_cli-0.9.1/giza/schemas/versions.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/utils/__init__.py` & `giza_cli-0.9.1/giza/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/utils/decorators.py` & `giza_cli-0.9.1/giza/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/utils/echo.py` & `giza_cli-0.9.1/giza/utils/echo.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/utils/enums.py` & `giza_cli-0.9.1/giza/utils/enums.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/giza/utils/misc.py` & `giza_cli-0.9.1/giza/utils/misc.py`

 * *Files identical despite different names*

### Comparing `giza_cli-0.9.0/pyproject.toml` & `giza_cli-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-cli"
-version = "0.9.0"
+version = "0.9.1"
 description = "CLI for interacting with Giza"
 authors = ["Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
 packages = [{include = "giza"}]
 
 [tool.poetry.scripts]
 giza = "giza.cli:entrypoint"
```

