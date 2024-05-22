# Comparing `tmp/runzero_sdk-0.8.2.tar.gz` & `tmp/runzero_sdk-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runzero_sdk-0.8.2.tar", max compression
+gzip compressed data, was "runzero_sdk-0.8.3.tar", max compression
```

## Comparing `runzero_sdk-0.8.2.tar` & `runzero_sdk-0.8.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1285 2024-04-01 05:55:36.309520 runzero_sdk-0.8.2/LICENSE
--rw-r--r--   0        0        0     6444 2024-04-01 05:55:36.309520 runzero_sdk-0.8.2/README.md
--rw-r--r--   0        0        0     4930 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      593 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/__init__.py
--rw-r--r--   0        0        0      725 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/__init__.py
--rw-r--r--   0        0        0      496 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/admin/__init__.py
--rw-r--r--   0        0        0    11426 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/admin/_sdk_source_icon.py
--rw-r--r--   0        0        0    14599 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/admin/custom_integrations.py
--rw-r--r--   0        0        0     3427 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/admin/orgs.py
--rw-r--r--   0        0        0     5702 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/admin/tasks.py
--rw-r--r--   0        0        0     2761 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/custom_integrations.py
--rw-r--r--   0        0        0     5037 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/explorers.py
--rw-r--r--   0        0        0     2913 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/hosted_zones.py
--rw-r--r--   0        0        0      274 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/imports/__init__.py
--rw-r--r--   0        0        0     5245 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/imports/assets.py
--rw-r--r--   0        0        0     1385 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/scans.py
--rw-r--r--   0        0        0     4478 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/sites.py
--rw-r--r--   0        0        0     5297 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/api/tasks.py
--rw-r--r--   0        0        0      441 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/__init__.py
--rw-r--r--   0        0        0      318 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/_http/__init__.py
--rw-r--r--   0        0        0     2384 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/_http/auth.py
--rw-r--r--   0        0        0     8121 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/_http/io.py
--rw-r--r--   0        0        0    11337 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/client.py
--rw-r--r--   0        0        0     7081 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/client/errors.py
--rw-r--r--   0        0        0     1077 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/errors.py
--rw-r--r--   0        0        0        0 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/py.typed
--rw-r--r--   0        0        0     1871 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/types/__init__.py
--rw-r--r--   0        0        0    48460 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/types/_data_models_gen.py
--rw-r--r--   0        0        0     2319 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/types/_rate_limit_information.py
--rw-r--r--   0        0        0    22347 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/types/_wrapped.py
--rw-r--r--   0        0        0      302 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/types/errors.py
--rw-r--r--   0        0        0      235 2024-04-01 05:55:36.313520 runzero_sdk-0.8.2/runzero/version.py
--rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 runzero_sdk-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1285 2024-05-22 16:42:19.736649 runzero_sdk-0.8.3/LICENSE
+-rw-r--r--   0        0        0     6444 2024-05-22 16:42:19.736649 runzero_sdk-0.8.3/README.md
+-rw-r--r--   0        0        0     4929 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0      593 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/__init__.py
+-rw-r--r--   0        0        0      725 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/__init__.py
+-rw-r--r--   0        0        0      496 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/admin/__init__.py
+-rw-r--r--   0        0        0    11426 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/admin/_sdk_source_icon.py
+-rw-r--r--   0        0        0    14599 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/admin/custom_integrations.py
+-rw-r--r--   0        0        0     3427 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/admin/orgs.py
+-rw-r--r--   0        0        0     5702 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/admin/tasks.py
+-rw-r--r--   0        0        0     2761 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/custom_integrations.py
+-rw-r--r--   0        0        0     5037 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/explorers.py
+-rw-r--r--   0        0        0     2913 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/hosted_zones.py
+-rw-r--r--   0        0        0      274 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/imports/__init__.py
+-rw-r--r--   0        0        0     5245 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/imports/assets.py
+-rw-r--r--   0        0        0     1385 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/scans.py
+-rw-r--r--   0        0        0     4478 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/sites.py
+-rw-r--r--   0        0        0     5297 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/api/tasks.py
+-rw-r--r--   0        0        0      441 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/__init__.py
+-rw-r--r--   0        0        0      318 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/_http/__init__.py
+-rw-r--r--   0        0        0     2384 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/_http/auth.py
+-rw-r--r--   0        0        0     8121 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/_http/io.py
+-rw-r--r--   0        0        0    11337 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/client.py
+-rw-r--r--   0        0        0     7081 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/client/errors.py
+-rw-r--r--   0        0        0     1077 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/errors.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/py.typed
+-rw-r--r--   0        0        0     1871 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/types/__init__.py
+-rw-r--r--   0        0        0    48467 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/types/_data_models_gen.py
+-rw-r--r--   0        0        0     2319 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/types/_rate_limit_information.py
+-rw-r--r--   0        0        0    22347 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/types/_wrapped.py
+-rw-r--r--   0        0        0      302 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/types/errors.py
+-rw-r--r--   0        0        0      235 2024-05-22 16:42:19.740649 runzero_sdk-0.8.3/runzero/version.py
+-rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 runzero_sdk-0.8.3/PKG-INFO
```

### Comparing `runzero_sdk-0.8.2/LICENSE` & `runzero_sdk-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/README.md` & `runzero_sdk-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/pyproject.toml` & `runzero_sdk-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "runzero-sdk"
-version = "0.8.2"
+version = "0.8.3"
 description = "The runZero platform sdk"
 license = "BSD-2-Clause"
 authors = ["runZero <support@runzero.com>"]
 readme = "README.md"
 homepage = "https://runzero.com/"
 documentation = "https://runzeroinc.github.io/runzero-sdk-py"
 repository = "https://github.com/runZeroInc/runzero-sdk-py"
@@ -61,15 +61,15 @@
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=6.1.3,<8.0.0"
 myst_parser = "^2.0.0"
 pandoc = "^2.3"
 sphinx-codeautolink = ">=0.14.1,<0.16.0"
 sphinx-autoapi = "^3.0.0"
-furo = "2024.1.29"
+furo = "2024.5.6"
 
 [tool.deptry]
 extend_exclude = [
   # necessary until deptry can understand
   # that if TYPE_CHECKING means dev dep
   "runzero/client/_http/io.py"
 ]
```

### Comparing `runzero_sdk-0.8.2/runzero/__init__.py` & `runzero_sdk-0.8.3/runzero/__init__.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/__init__.py` & `runzero_sdk-0.8.3/runzero/api/__init__.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/admin/_sdk_source_icon.py` & `runzero_sdk-0.8.3/runzero/api/admin/_sdk_source_icon.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/admin/custom_integrations.py` & `runzero_sdk-0.8.3/runzero/api/admin/custom_integrations.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/admin/orgs.py` & `runzero_sdk-0.8.3/runzero/api/admin/orgs.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/admin/tasks.py` & `runzero_sdk-0.8.3/runzero/api/admin/tasks.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/custom_integrations.py` & `runzero_sdk-0.8.3/runzero/api/custom_integrations.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/explorers.py` & `runzero_sdk-0.8.3/runzero/api/explorers.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/hosted_zones.py` & `runzero_sdk-0.8.3/runzero/api/hosted_zones.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/imports/assets.py` & `runzero_sdk-0.8.3/runzero/api/imports/assets.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/scans.py` & `runzero_sdk-0.8.3/runzero/api/scans.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/sites.py` & `runzero_sdk-0.8.3/runzero/api/sites.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/api/tasks.py` & `runzero_sdk-0.8.3/runzero/api/tasks.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/client/_http/auth.py` & `runzero_sdk-0.8.3/runzero/client/_http/auth.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/client/_http/io.py` & `runzero_sdk-0.8.3/runzero/client/_http/io.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/client/client.py` & `runzero_sdk-0.8.3/runzero/client/client.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/client/errors.py` & `runzero_sdk-0.8.3/runzero/client/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/errors.py` & `runzero_sdk-0.8.3/runzero/errors.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/types/__init__.py` & `runzero_sdk-0.8.3/runzero/types/__init__.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/types/_data_models_gen.py` & `runzero_sdk-0.8.3/runzero/types/_data_models_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         example="cpe:2.3:a:hp:insight_diagnostics:7.4.0.1570:-:*:*:online:win2003:x64:*",
         max_length=512,
         regex="^cpe:.*",
     )
     """
     The Common Platform Enumeration v2.3 value describing the vulnerable service.
     """
-    cve: Optional[str] = Field(None, example="CVE-2021-31005", max_length=14, regex="^CVE-\\d{4}-\\d{5}$")
+    cve: Optional[str] = Field(None, example="CVE-2021-31005", max_length=14, regex="^CVE-[0-9]{4}-[0-9]{4,19}$")
     """
     CVE represents the common vulnerability ID as assigned by an authority such as NIST and should be in the format of 'CVE-YYYY-NNNNN' where YYYY represents the year of the entry and NNNNN is the vulns unique number.
 
     """
     cvss2_base_score: Optional[float] = Field(None, alias="cvss2BaseScore", example=4.3, ge=0.0, le=10.0)
     """
     The exploit-ability score of the vulnerability as assigned by the CVSS2 system.
```

### Comparing `runzero_sdk-0.8.2/runzero/types/_rate_limit_information.py` & `runzero_sdk-0.8.3/runzero/types/_rate_limit_information.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/runzero/types/_wrapped.py` & `runzero_sdk-0.8.3/runzero/types/_wrapped.py`

 * *Files identical despite different names*

### Comparing `runzero_sdk-0.8.2/PKG-INFO` & `runzero_sdk-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runzero-sdk
-Version: 0.8.2
+Version: 0.8.3
 Summary: The runZero platform sdk
 Home-page: https://runzero.com/
 License: BSD-2-Clause
 Keywords: runzero,api,sdk
 Author: runZero
 Author-email: support@runzero.com
 Requires-Python: >=3.8,<4.0
```

