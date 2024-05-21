# Comparing `tmp/nora_lib-0.0.5.dev3.tar.gz` & `tmp/nora_lib-0.0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.5.dev3.tar", last modified: Mon May 20 23:36:20 2024, max compression
+gzip compressed data, was "nora_lib-0.0.6.dev0.tar", last modified: Tue May 21 21:31:49 2024, max compression
```

## Comparing `nora_lib-0.0.5.dev3.tar` & `nora_lib-0.0.6.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.480638 nora_lib-0.0.5.dev3/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 23:36:20.480174 nora_lib-0.0.5.dev3/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.469108 nora_lib-0.0.5.dev3/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.472757 nora_lib-0.0.5.dev3/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev3/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.5.dev3/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.474534 nora_lib-0.0.5.dev3/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     8656 2024-05-20 23:35:45.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     4672 2024-05-20 23:33:58.000000 nora_lib-0.0.5.dev3/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.476363 nora_lib-0.0.5.dev3/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1793 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.479012 nora_lib-0.0.5.dev3/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      412 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       64 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-20 23:36:20.000000 nora_lib-0.0.5.dev3/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-20 23:36:20.480734 nora_lib-0.0.5.dev3/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      605 2024-05-20 23:33:58.000000 nora_lib-0.0.5.dev3/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.477162 nora_lib-0.0.5.dev3/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-20 23:36:20.478140 nora_lib-0.0.5.dev3/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.5.dev3/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.757583 nora_lib-0.0.6.dev0/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 21:31:49.757219 nora_lib-0.0.6.dev0/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.745589 nora_lib-0.0.6.dev0/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.749176 nora_lib-0.0.6.dev0/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev0/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev0/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.751650 nora_lib-0.0.6.dev0/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)    11125 2024-05-21 21:30:45.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4659 2024-05-21 21:09:30.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.753562 nora_lib-0.0.6.dev0/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     5553 2024-05-21 21:25:27.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.756246 nora_lib-0.0.6.dev0/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       70 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-21 21:31:49.757718 nora_lib-0.0.6.dev0/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      614 2024-05-21 21:16:46.000000 nora_lib-0.0.6.dev0/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.754205 nora_lib-0.0.6.dev0/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.755416 nora_lib-0.0.6.dev0/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.5.dev3/README.md` & `nora_lib-0.0.6.dev0/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev3/nora_lib/context/context_service.py` & `nora_lib-0.0.6.dev0/nora_lib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev3/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.6.dev0/nora_lib/interactions/interactions_service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime
 import logging
 import requests
 from typing import List, Optional
+import json
 
 from nora_lib.interactions.models import (
     AnnotationBatch,
     Event,
     EventType,
     Message,
     ReturnedMessage,
@@ -27,52 +28,52 @@
     def save_message(self, message: Message) -> None:
         """Save a message to the Interactions API"""
         message_url = f"{self.base_url}/interaction/v1/message"
         response = requests.post(
             message_url,
             json=message.model_dump(),
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
 
     def save_event(self, event: Event) -> None:
         """Save an event to the Interactions API"""
         event_url = f"{self.base_url}/interaction/v1/event"
         response = requests.post(
             event_url,
             json=event.model_dump(),
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
 
     def save_annotation(self, annotation: AnnotationBatch) -> None:
         """Save an annotation to the Interactions API"""
         annotation_url = f"{self.base_url}/interaction/v1/annotation"
         response = requests.post(
             annotation_url,
             json=annotation.model_dump(),
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
 
     def get_message(self, message_id: str) -> ReturnedMessage:
         """Fetch a message from the Interactions API"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
         request_body = {
             "id": message_id,
             "relations": {"thread": {}, "channel": {}, "events": {}, "annotations": {}},
         }
         response = requests.post(
             message_url,
             json=request_body,
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
         res_dict = response.json()["message"]
         res = ReturnedMessage.model_validate(res_dict)
 
         # thread_id and channel_id are for some reason nested in the response
         if not res.thread_id:
@@ -88,15 +89,15 @@
         request_body = self._channel_lookup_request(
             channel_id=channel_id, min_timestamp=min_timestamp
         )
         response = requests.post(
             message_url,
             json=request_body,
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
         return response.json()
 
     def fetch_messages_and_agent_context_events_for_thread(
         self, message_id: str, event_type: str
     ) -> List[ReturnedMessage]:
@@ -110,15 +111,16 @@
             )
         )
         messages_with_events.extend(messages_for_thread.messages)
 
         # Process any thread_fork events
         try:
             for msg in messages_for_thread.messages:
-                for event in msg.events:
+                events = msg.events if msg.events else []
+                for event in events:
                     if event.type == EventType.THREAD_FORK.value:
                         event_data = ThreadForkEventData.model_validate(event.data)
                         forked_thread: ThreadRelationsResponse = (
                             self.fetch_thread_messages_and_events_for_message(
                                 event_data.previous_message_id, [event_type]
                             )
                         )
@@ -139,15 +141,15 @@
         """Fetch messages sorted by timestamp and events for agent context"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
         request_body = self._thread_lookup_request(message_id, event_types=event_types)
         response = requests.post(
             message_url,
             json=request_body,
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
         json_response = response.json()
 
         return ThreadRelationsResponse.model_validate(
             json_response.get("message", {}).get("thread", {})
         )
@@ -172,19 +174,54 @@
             },
         }
 
         response = requests.post(
             thread_search_url,
             json=request_body,
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
         return response.json()
 
+    def fetch_messages_and_events_for_forked_thread(
+        self, message_id: str, event_type: str
+    ) -> List[ReturnedMessage]:
+        """Build a history of messages for a given message including associated events.
+        This includes messages from pre-forked threads."""
+        returned_messages: List[ReturnedMessage] = []
+
+        messages_for_thread: ThreadRelationsResponse = (
+            self.fetch_thread_messages_and_events_for_message(message_id, [event_type])
+        )
+        if messages_for_thread.messages:
+            returned_messages.extend(messages_for_thread.messages)
+
+        # Lookup any thread_fork events (conversation across surfaces)
+        thread_fork_events = self.fetch_messages_and_events_for_thread(
+            messages_for_thread.thread_id, EventType.THREAD_FORK.value
+        )
+        for forked_thread_event in thread_fork_events.get("thread", {}).get(
+            "events", []
+        ):
+            event_data = ThreadForkEventData.model_validate(
+                forked_thread_event.get("data", {})
+            )
+            forked_thread: ThreadRelationsResponse = (
+                self.fetch_thread_messages_and_events_for_message(
+                    event_data.previous_message_id, [event_type]
+                )
+            )
+            if forked_thread.messages:
+                returned_messages.extend(forked_thread.messages)
+
+        returned_messages.sort(key=lambda x: x.ts)
+
+        return returned_messages
+
     def fetch_events_for_message(
         self,
         message_id: str,
         event_type: Optional[str] = None,
     ) -> dict:
         """Fetch messages and events for the thread containing a given message from the Interactions API"""
         message_search_url = f"{self.base_url}/interaction/v1/search/message"
@@ -195,15 +232,15 @@
             },
         }
 
         response = requests.post(
             message_search_url,
             json=request_body,
             headers=self.headers,
-            timeout=int(self.timeout),
+            timeout=self.timeout,
         )
         response.raise_for_status()
         return response.json()
 
     @staticmethod
     def _channel_lookup_request(channel_id: str, min_timestamp: str) -> dict:
         """Interaction service API request to get threads and messages for a channel"""
@@ -233,7 +270,36 @@
                             "relations": {"events": {"filter": {"type": event_types}}},
                             "apply_annotations_from_actors": ["*"],
                         },
                     }
                 }
             },
         }
+
+    @staticmethod
+    def prod() -> "InteractionsService":
+        return InteractionsService(
+            base_url="https://s2ub.prod.s2.allenai.org/service/noraretrieval",
+            timeout=30,
+            token=InteractionsService._fetch_bearer_token(
+                "nora/prod/interaction-bearer-token"
+            ),
+        )
+
+    @staticmethod
+    def dev() -> "InteractionsService":
+        return InteractionsService(
+            base_url="https://s2ub.dev.s2.allenai.org/service/noraretrieval",
+            timeout=30,
+            token=InteractionsService._fetch_bearer_token(
+                "nora/dev/interaction-bearer-token"
+            ),
+        )
+
+    @staticmethod
+    def _fetch_bearer_token(secret_id: str) -> str:
+        import boto3
+
+        secrets_manager = boto3.client("secretsmanager", region_name="us-west-2")
+        return json.loads(
+            secrets_manager.get_secret_value(SecretId=secret_id)["SecretString"]
+        )["token"]
```

### Comparing `nora_lib-0.0.5.dev3/nora_lib/interactions/models.py` & `nora_lib-0.0.6.dev0/nora_lib/interactions/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """Message format returned by interaction service"""
 
     message_id: str
     actor_id: UUID
     text: str
     ts: datetime
     annotated_text: Optional[str] = None
-    events: List[Event] = Field(default_factory=list)
+    events: Optional[List[Event]] = None
     thread_id: Optional[str] = None
     channel_id: Optional[str] = None
     annotations: Optional[List[Annotation]] = None
 
 
 class AgentMessageData(BaseModel):
     """capture requests to and responses from tools within Events"""
```

### Comparing `nora_lib-0.0.5.dev3/nora_lib/tasks/models.py` & `nora_lib-0.0.6.dev0/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev3/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.6.dev0/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.5.dev3/setup.py` & `nora_lib-0.0.6.dev0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
-runtime_requirements = ["pydantic>=2,<3", "requests"]
+runtime_requirements = ["pydantic>=2,<3", "requests", "boto3"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.5.dev3",
+    version="0.0.6.dev0",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.5.dev3/tests/tasks/test_state.py` & `nora_lib-0.0.6.dev0/tests/tasks/test_state.py`

 * *Files identical despite different names*

