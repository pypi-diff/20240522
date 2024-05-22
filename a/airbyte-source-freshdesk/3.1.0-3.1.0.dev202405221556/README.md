# Comparing `tmp/airbyte_source_freshdesk-3.1.0.tar.gz` & `tmp/airbyte_source_freshdesk-3.1.0.dev202405221556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_freshdesk-3.1.0.tar", max compression
+gzip compressed data, was "airbyte_source_freshdesk-3.1.0.dev202405221556.tar", max compression
```

## Comparing `airbyte_source_freshdesk-3.1.0.tar` & `airbyte_source_freshdesk-3.1.0.dev202405221556.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4578 2024-03-26 18:32:53.961272 airbyte_source_freshdesk-3.1.0/README.md
--rw-r--r--   0        0        0      777 2024-03-26 18:36:11.815135 airbyte_source_freshdesk-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       67 2024-03-26 18:32:53.961272 airbyte_source_freshdesk-3.1.0/source_freshdesk/__init__.py
--rw-r--r--   0        0        0     6344 2024-03-26 18:32:53.961272 airbyte_source_freshdesk-3.1.0/source_freshdesk/components.py
--rw-r--r--   0        0        0    14902 2024-03-26 18:32:53.961272 airbyte_source_freshdesk-3.1.0/source_freshdesk/manifest.yaml
--rw-r--r--   0        0        0      239 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/run.py
--rw-r--r--   0        0        0     1555 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/agents.json
--rw-r--r--   0        0        0     2514 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/business_hours.json
--rw-r--r--   0        0        0      453 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/canned_response_folders.json
--rw-r--r--   0        0        0     1274 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/canned_responses.json
--rw-r--r--   0        0        0      867 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/companies.json
--rw-r--r--   0        0        0     1287 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/contacts.json
--rw-r--r--   0        0        0     1168 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/conversations.json
--rw-r--r--   0        0        0      389 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_categories.json
--rw-r--r--   0        0        0      732 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_comments.json
--rw-r--r--   0        0        0      771 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_forums.json
--rw-r--r--   0        0        0      983 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_topics.json
--rw-r--r--   0        0        0      687 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/email_configs.json
--rw-r--r--   0        0        0     1129 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/email_mailboxes.json
--rw-r--r--   0        0        0      711 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/groups.json
--rw-r--r--   0        0        0      389 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/products.json
--rw-r--r--   0        0        0      447 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/roles.json
--rw-r--r--   0        0        0      685 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/satisfaction_ratings.json
--rw-r--r--   0        0        0      743 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/scenario_automations.json
--rw-r--r--   0        0        0      422 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/settings.json
--rw-r--r--   0        0        0     1214 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/skills.json
--rw-r--r--   0        0        0     5479 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/sla_policies.json
--rw-r--r--   0        0        0     1370 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_articles.json
--rw-r--r--   0        0        0      518 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_categories.json
--rw-r--r--   0        0        0      832 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_folders.json
--rw-r--r--   0        0        0      921 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/surveys.json
--rw-r--r--   0        0        0     1991 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/ticket_fields.json
--rw-r--r--   0        0        0     2213 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/tickets.json
--rw-r--r--   0        0        0      812 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/time_entries.json
--rw-r--r--   0        0        0      287 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/source.py
--rw-r--r--   0        0        0     1111 2024-03-26 18:32:53.965272 airbyte_source_freshdesk-3.1.0/source_freshdesk/utils.py
--rw-r--r--   0        0        0     5323 1970-01-01 00:00:00.000000 airbyte_source_freshdesk-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4578 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/README.md
+-rw-r--r--   0        0        0      793 2024-05-22 15:56:55.176110 airbyte_source_freshdesk-3.1.0.dev202405221556/pyproject.toml
+-rw-r--r--   0        0        0       67 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/__init__.py
+-rw-r--r--   0        0        0     6385 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/components.py
+-rw-r--r--   0        0        0    14900 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/manifest.yaml
+-rw-r--r--   0        0        0      239 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/run.py
+-rw-r--r--   0        0        0     1555 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/agents.json
+-rw-r--r--   0        0        0     2514 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/business_hours.json
+-rw-r--r--   0        0        0      453 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/canned_response_folders.json
+-rw-r--r--   0        0        0     1274 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/canned_responses.json
+-rw-r--r--   0        0        0      867 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/companies.json
+-rw-r--r--   0        0        0     1287 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/contacts.json
+-rw-r--r--   0        0        0     1168 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/conversations.json
+-rw-r--r--   0        0        0      389 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_categories.json
+-rw-r--r--   0        0        0      732 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_comments.json
+-rw-r--r--   0        0        0      771 2024-05-22 15:52:57.791352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_forums.json
+-rw-r--r--   0        0        0      983 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_topics.json
+-rw-r--r--   0        0        0      687 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/email_configs.json
+-rw-r--r--   0        0        0     1129 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/email_mailboxes.json
+-rw-r--r--   0        0        0      711 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/groups.json
+-rw-r--r--   0        0        0      389 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/products.json
+-rw-r--r--   0        0        0      447 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/roles.json
+-rw-r--r--   0        0        0      685 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/satisfaction_ratings.json
+-rw-r--r--   0        0        0      743 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/scenario_automations.json
+-rw-r--r--   0        0        0      422 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/settings.json
+-rw-r--r--   0        0        0     1214 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/skills.json
+-rw-r--r--   0        0        0     5479 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/sla_policies.json
+-rw-r--r--   0        0        0     1370 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_articles.json
+-rw-r--r--   0        0        0      518 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_categories.json
+-rw-r--r--   0        0        0      832 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_folders.json
+-rw-r--r--   0        0        0      921 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/surveys.json
+-rw-r--r--   0        0        0     1991 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/ticket_fields.json
+-rw-r--r--   0        0        0     2213 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/tickets.json
+-rw-r--r--   0        0        0      812 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/time_entries.json
+-rw-r--r--   0        0        0      287 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/source.py
+-rw-r--r--   0        0        0     1111 2024-05-22 15:52:57.795352 airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/utils.py
+-rw-r--r--   0        0        0     5339 1970-01-01 00:00:00.000000 airbyte_source_freshdesk-3.1.0.dev202405221556/PKG-INFO
```

### Comparing `airbyte_source_freshdesk-3.1.0/README.md` & `airbyte_source_freshdesk-3.1.0.dev202405221556/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/pyproject.toml` & `airbyte_source_freshdesk-3.1.0.dev202405221556/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "3.1.0"
+version = "3.1.0.dev202405221556"
 name = "airbyte-source-freshdesk"
 description = "Source implementation for Freshdesk."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/components.py` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 
 from dataclasses import dataclass
-from typing import Any, List, Mapping, MutableMapping, Optional
+from typing import Any, Mapping, MutableMapping, Optional
 
 import requests
 from airbyte_cdk.sources.declarative.incremental import DatetimeBasedCursor
 from airbyte_cdk.sources.declarative.requesters.http_requester import HttpRequester
 from airbyte_cdk.sources.declarative.requesters.paginators.strategies.page_increment import PageIncrement
 from airbyte_cdk.sources.declarative.requesters.request_option import RequestOptionType
 from airbyte_cdk.sources.declarative.requesters.request_options.interpolated_request_options_provider import (
     InterpolatedRequestOptionsProvider,
     RequestInput,
 )
 from airbyte_cdk.sources.declarative.types import StreamSlice, StreamState
+from airbyte_cdk.sources.types import Record
 from source_freshdesk.utils import CallCredit
 
 
 @dataclass
 class FreshdeskRequester(HttpRequester):
     """
     This class is created to add call throttling using the optional requests_per_minute parameter
@@ -117,21 +118,21 @@
 class FreshdeskTicketsPaginationStrategy(PageIncrement):
     """
     This pagination strategy will return latest record cursor for the next_page_token after hitting page count limit
     """
 
     PAGE_LIMIT = 300
 
-    def next_page_token(self, response: requests.Response, last_records: List[Mapping[str, Any]]) -> Optional[Any]:
+    def next_page_token(self, response: requests.Response, last_page_size: int, last_record: Optional[Record]) -> Optional[Any]:
         # Stop paginating when there are fewer records than the page size or the current page has no records, or maximum page number is hit
-        if (self._page_size and len(last_records) < self._page_size) or len(last_records) == 0:
+        if (self._page_size and last_page_size < self._page_size) or last_page_size == 0:
             return None
         elif self._page >= self.PAGE_LIMIT:
             # reset page count as cursor parameter will be updated in the stream slicer
             self.reset()
             # get last_record from latest batch, pos. -1, because of ACS order of records
-            last_record_updated_at = last_records[-1]["updated_at"]
+            last_record_updated_at = last_record["updated_at"]
             # updating slicer request parameters with last_record state
             return last_record_updated_at
         else:
             self._page += 1
             return self._page
```

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/manifest.yaml` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/manifest.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
   paginator:
     type: DefaultPaginator
     pagination_strategy:
       type: CursorPagination
       cursor_value: "{{ headers['link']['next']['url'] }}"
       stop_condition: "{{ 'next' not in headers['link'] }}"
-      page_size: 100
+      page_size: 2
     page_size_option:
       field_name: "per_page"
       inject_into: "request_parameter"
     page_token_option:
       type: RequestPath
 
   error_handler:
```

#### html2text {}

```diff
@@ -17,15 +17,15 @@
 lookback window for the stream Satisfaction Ratings additionalProperties: true
 definitions: schema_loader: type: JsonFileSchemaLoader file_path: "./
 source_freshdesk/schemas/{{ parameters['name'] }}.json" basic_authenticator:
 type: BasicHttpAuthenticator username: "{{ config.get('api_key')}}"
 record_selector: type: RecordSelector extractor: type: DpathExtractor
 field_path: [] paginator: type: DefaultPaginator pagination_strategy: type:
 CursorPagination cursor_value: "{{ headers['link']['next']['url'] }}"
-stop_condition: "{{ 'next' not in headers['link'] }}" page_size: 100
+stop_condition: "{{ 'next' not in headers['link'] }}" page_size: 2
 page_size_option: field_name: "per_page" inject_into: "request_parameter"
 page_token_option: type: RequestPath error_handler: type: CompositeErrorHandler
 error_handlers: - type: DefaultErrorHandler response_filters: - http_codes:
 [401] action: FAIL error_message: "The endpoint to access stream '{{ parameters
 ['name'] }}' returned 401: Unauthorized. This is most likely due to wrong
 credentials." - type: DefaultErrorHandler backoff_strategies: - type:
 WaitTimeFromHeader header: Retry-After requester: # This requester is used to
```

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/agents.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/agents.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/business_hours.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/business_hours.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/canned_responses.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/canned_responses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/companies.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/companies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/contacts.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/conversations.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/conversations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_comments.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_forums.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_forums.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/discussion_topics.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/discussion_topics.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/email_configs.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/email_configs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/email_mailboxes.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/email_mailboxes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/groups.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/satisfaction_ratings.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/satisfaction_ratings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/scenario_automations.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/scenario_automations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/skills.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/skills.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/sla_policies.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/sla_policies.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_articles.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_categories.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/solution_folders.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/solution_folders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/surveys.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/surveys.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/ticket_fields.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/ticket_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/tickets.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/tickets.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/schemas/time_entries.json` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/schemas/time_entries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/source_freshdesk/utils.py` & `airbyte_source_freshdesk-3.1.0.dev202405221556/source_freshdesk/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_freshdesk-3.1.0/PKG-INFO` & `airbyte_source_freshdesk-3.1.0.dev202405221556/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-freshdesk
-Version: 3.1.0
+Version: 3.1.0.dev202405221556
 Summary: Source implementation for Freshdesk.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

