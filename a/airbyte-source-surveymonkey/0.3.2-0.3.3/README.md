# Comparing `tmp/airbyte_source_surveymonkey-0.3.2.tar.gz` & `tmp/airbyte_source_surveymonkey-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_surveymonkey-0.3.2.tar", max compression
+gzip compressed data, was "airbyte_source_surveymonkey-0.3.3.tar", max compression
```

## Comparing `airbyte_source_surveymonkey-0.3.2.tar` & `airbyte_source_surveymonkey-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4619 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/README.md
--rw-r--r--   0        0        0      822 2024-05-20 18:14:42.339942 airbyte_source_surveymonkey-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1244 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/__init__.py
--rw-r--r--   0        0        0     2164 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/components.py
--rw-r--r--   0        0        0     2620 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/config_migrations.py
--rw-r--r--   0        0        0    15740 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/manifest.yaml
--rw-r--r--   0        0        0      347 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/run.py
--rw-r--r--   0        0        0     3791 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/collectors.json
--rw-r--r--   0        0        0      660 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_collectors.json
--rw-r--r--   0        0        0      588 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_ids.json
--rw-r--r--   0        0        0      815 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_pages.json
--rw-r--r--   0        0        0     4871 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_questions.json
--rw-r--r--   0        0        0     4641 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_responses.json
--rw-r--r--   0        0        0     3390 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/surveys.json
--rw-r--r--   0        0        0     2315 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/source.py
--rw-r--r--   0        0        0     8428 2024-05-20 04:08:55.000000 airbyte_source_surveymonkey-0.3.2/source_surveymonkey/streams.py
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     4619 2024-05-22 20:09:31.791816 airbyte_source_surveymonkey-0.3.3/README.md
+-rw-r--r--   0        0        0      822 2024-05-22 20:13:32.164610 airbyte_source_surveymonkey-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1244 2024-05-22 20:09:31.791816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/__init__.py
+-rw-r--r--   0        0        0     2164 2024-05-22 20:09:31.791816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/components.py
+-rw-r--r--   0        0        0     2620 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/config_migrations.py
+-rw-r--r--   0        0        0    15740 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/manifest.yaml
+-rw-r--r--   0        0        0      347 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/run.py
+-rw-r--r--   0        0        0     3791 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/collectors.json
+-rw-r--r--   0        0        0      660 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_collectors.json
+-rw-r--r--   0        0        0      588 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_ids.json
+-rw-r--r--   0        0        0      815 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_pages.json
+-rw-r--r--   0        0        0     4871 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_questions.json
+-rw-r--r--   0        0        0     4641 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_responses.json
+-rw-r--r--   0        0        0     3390 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/surveys.json
+-rw-r--r--   0        0        0     2331 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/source.py
+-rw-r--r--   0        0        0     8428 2024-05-22 20:09:31.795816 airbyte_source_surveymonkey-0.3.3/source_surveymonkey/streams.py
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 airbyte_source_surveymonkey-0.3.3/PKG-INFO
```

### Comparing `airbyte_source_surveymonkey-0.3.2/README.md` & `airbyte_source_surveymonkey-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/pyproject.toml` & `airbyte_source_surveymonkey-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.2"
+version = "0.3.3"
 name = "airbyte-source-surveymonkey"
 description = "Source implementation for Surveymonkey."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/__init__.py` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/components.py` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/components.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/config_migrations.py` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/manifest.yaml` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/collectors.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/collectors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_collectors.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_collectors.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_ids.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_ids.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_pages.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_questions.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_questions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/survey_responses.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/survey_responses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/schemas/surveys.json` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/schemas/surveys.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/source.py` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 from typing import Any, List, Mapping, Tuple
 
 import pendulum
 import requests
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
-from airbyte_cdk.sources.streams.http.auth import TokenAuthenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth import TokenAuthenticator
 
 from .streams import Surveys
 
 """
 This file provides the necessary constructs to interpret a provided declarative YAML configuration file into
 source connector.
```

### Comparing `airbyte_source_surveymonkey-0.3.2/source_surveymonkey/streams.py` & `airbyte_source_surveymonkey-0.3.3/source_surveymonkey/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     def path(self, stream_slice: Mapping[str, Any] = None, **kwargs) -> str:
         return f"surveys/{stream_slice['survey_id']}/details"
 
     def stream_slices(self, stream_state: Mapping[str, Any] = None, **kwargs):
         if self._survey_ids:
             yield from [{"survey_id": id} for id in self._survey_ids]
         else:
-            survey_stream = SurveyIds(start_date=self._start_date, survey_ids=self._survey_ids, authenticator=self.authenticator)
+            survey_stream = SurveyIds(start_date=self._start_date, survey_ids=self._survey_ids, authenticator=self._session.auth)
             for survey in survey_stream.read_records(sync_mode=SyncMode.full_refresh, stream_state=stream_state):
                 yield {"survey_id": survey["id"]}
 
 
 class Surveys(SurveyIDSliceMixin, IncrementalSurveymonkeyStream):
     """
     Docs: https://developer.surveymonkey.com/api/v3/#surveys
```

### Comparing `airbyte_source_surveymonkey-0.3.2/PKG-INFO` & `airbyte_source_surveymonkey-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-surveymonkey
-Version: 0.3.2
+Version: 0.3.3
 Summary: Source implementation for Surveymonkey.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

