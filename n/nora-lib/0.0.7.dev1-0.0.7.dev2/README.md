# Comparing `tmp/nora_lib-0.0.7.dev1.tar.gz` & `tmp/nora_lib-0.0.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.7.dev1.tar", last modified: Wed May 22 17:48:47 2024, max compression
+gzip compressed data, was "nora_lib-0.0.7.dev2.tar", last modified: Wed May 22 20:20:37 2024, max compression
```

## Comparing `nora_lib-0.0.7.dev1.tar` & `nora_lib-0.0.7.dev2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.440015 nora_lib-0.0.7.dev1/
--rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-22 17:48:47.439474 nora_lib-0.0.7.dev1/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.424694 nora_lib-0.0.7.dev1/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.429818 nora_lib-0.0.7.dev1/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.7.dev1/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.7.dev1/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.432124 nora_lib-0.0.7.dev1/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)    11071 2024-05-21 22:33:10.000000 nora_lib-0.0.7.dev1/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     5055 2024-05-22 17:48:35.000000 nora_lib-0.0.7.dev1/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.434404 nora_lib-0.0.7.dev1/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     5553 2024-05-21 22:33:10.000000 nora_lib-0.0.7.dev1/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.437661 nora_lib-0.0.7.dev1/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-22 17:48:47.000000 nora_lib-0.0.7.dev1/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-22 17:48:47.000000 nora_lib-0.0.7.dev1/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-22 17:48:47.000000 nora_lib-0.0.7.dev1/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       70 2024-05-22 17:48:47.000000 nora_lib-0.0.7.dev1/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-22 17:48:47.000000 nora_lib-0.0.7.dev1/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-22 17:48:47.440152 nora_lib-0.0.7.dev1/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      614 2024-05-22 17:48:40.000000 nora_lib-0.0.7.dev1/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.435386 nora_lib-0.0.7.dev1/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 17:48:47.436479 nora_lib-0.0.7.dev1/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev1/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.126165 nora_lib-0.0.7.dev2/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-22 20:20:37.125697 nora_lib-0.0.7.dev2/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.114203 nora_lib-0.0.7.dev2/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.118472 nora_lib-0.0.7.dev2/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1095 2024-05-22 20:19:40.000000 nora_lib-0.0.7.dev2/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.7.dev2/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.120305 nora_lib-0.0.7.dev2/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     7906 2024-05-22 20:18:24.000000 nora_lib-0.0.7.dev2/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4708 2024-05-22 20:18:24.000000 nora_lib-0.0.7.dev2/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.121900 nora_lib-0.0.7.dev2/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     5553 2024-05-21 22:33:10.000000 nora_lib-0.0.7.dev2/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.124533 nora_lib-0.0.7.dev2/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-22 20:20:37.000000 nora_lib-0.0.7.dev2/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-22 20:20:37.000000 nora_lib-0.0.7.dev2/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-22 20:20:37.000000 nora_lib-0.0.7.dev2/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       70 2024-05-22 20:20:37.000000 nora_lib-0.0.7.dev2/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-22 20:20:37.000000 nora_lib-0.0.7.dev2/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-22 20:20:37.126258 nora_lib-0.0.7.dev2/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      614 2024-05-22 20:15:41.000000 nora_lib-0.0.7.dev2/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.122452 nora_lib-0.0.7.dev2/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-22 20:20:37.123548 nora_lib-0.0.7.dev2/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.7.dev2/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.7.dev1/README.md` & `nora_lib-0.0.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.7.dev1/nora_lib/context/context_service.py` & `nora_lib-0.0.7.dev2/nora_lib/context/context_service.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-from datetime import datetime, timezone
-from typing import List, Optional
-from uuid import UUID
+from typing import Optional
 
 from nora_lib.interactions.interactions_service import InteractionsService
-from nora_lib.interactions.models import (
-    ReturnedMessage,
-    ReturnedAgentContextMessage,
-    ReturnedAgentContextEvent,
-    EventType,
-    AgentMessageData,
-    Event,
-)
-from nora_lib.context.models import WrappedTaskObject
+from nora_lib.interactions.models import ReturnedMessage
 
 
 class ContextService:
     """
     Save and retrieve task agent context from interaction store
     """
```

### Comparing `nora_lib-0.0.7.dev1/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.7.dev2/nora_lib/interactions/interactions_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,17 @@
-from datetime import datetime
-import logging
 import requests
-from typing import List, Optional
+from typing import Optional
 import json
 
 from nora_lib.interactions.models import (
     AnnotationBatch,
     Event,
-    EventType,
     Message,
     ReturnedMessage,
     ThreadRelationsResponse,
-    ThreadForkEventData,
 )
 
 
 class InteractionsService:
     """
     Service which saves interactions to the Interactions API
     """
@@ -94,50 +90,14 @@
             json=request_body,
             headers=self.headers,
             timeout=self.timeout,
         )
         response.raise_for_status()
         return response.json()
 
-    def fetch_messages_and_agent_context_events_for_thread(
-        self, message_id: str, event_type: str
-    ) -> List[ReturnedMessage]:
-        """Build a history of messages for a given message including associated events.
-        This includes messages from pre-forked threads."""
-        messages_with_events: List[ReturnedMessage] = []
-
-        messages_for_thread: ThreadRelationsResponse = (
-            self.fetch_thread_messages_and_events_for_message(
-                message_id, [event_type, EventType.THREAD_FORK.value]
-            )
-        )
-        messages_with_events.extend(messages_for_thread.messages)
-
-        # Process any thread_fork events
-        try:
-            for msg in messages_for_thread.messages:
-                for event in msg.events:
-                    if event.type == EventType.THREAD_FORK.value:
-                        event_data = ThreadForkEventData.model_validate(event.data)
-                        forked_thread: ThreadRelationsResponse = (
-                            self.fetch_thread_messages_and_events_for_message(
-                                event_data.previous_message_id, [event_type]
-                            )
-                        )
-                        messages_with_events.extend(forked_thread.messages)
-        except Exception as e:  # pylint: disable=broad-except
-            logging.exception(
-                "Failed to fetch forked thread messages for message %s: %s",
-                message_id,
-                e,
-            )
-
-        messages_with_events.sort(key=lambda x: x.ts)
-        return messages_with_events
-
     def fetch_thread_messages_and_events_for_message(
         self, message_id: str, event_types: list[str]
     ) -> ThreadRelationsResponse:
         """Fetch messages sorted by timestamp and events for agent context"""
         message_url = f"{self.base_url}/interaction/v1/search/message"
         request_body = self._thread_lookup_request(message_id, event_types=event_types)
         response = requests.post(
@@ -178,49 +138,14 @@
             json=request_body,
             headers=self.headers,
             timeout=self.timeout,
         )
         response.raise_for_status()
         return response.json()
 
-    def fetch_messages_and_events_for_forked_thread(
-        self, message_id: str, event_type: str
-    ) -> List[ReturnedMessage]:
-        """Build a history of messages for a given message including associated events.
-        This includes messages from pre-forked threads."""
-        returned_messages: List[ReturnedMessage] = []
-
-        messages_for_thread: ThreadRelationsResponse = (
-            self.fetch_thread_messages_and_events_for_message(message_id, [event_type])
-        )
-        if messages_for_thread.messages:
-            returned_messages.extend(messages_for_thread.messages)
-
-        # Lookup any thread_fork events (conversation across surfaces)
-        thread_fork_events = self.fetch_messages_and_events_for_thread(
-            messages_for_thread.thread_id, EventType.THREAD_FORK.value
-        )
-        for forked_thread_event in thread_fork_events.get("thread", {}).get(
-            "events", []
-        ):
-            event_data = ThreadForkEventData.model_validate(
-                forked_thread_event.get("data", {})
-            )
-            forked_thread: ThreadRelationsResponse = (
-                self.fetch_thread_messages_and_events_for_message(
-                    event_data.previous_message_id, [event_type]
-                )
-            )
-            if forked_thread.messages:
-                returned_messages.extend(forked_thread.messages)
-
-        returned_messages.sort(key=lambda x: x.ts)
-
-        return returned_messages
-
     def fetch_events_for_message(
         self,
         message_id: str,
         event_type: Optional[str] = None,
     ) -> dict:
         """Fetch messages and events for the thread containing a given message from the Interactions API"""
         message_search_url = f"{self.base_url}/interaction/v1/search/message"
```

### Comparing `nora_lib-0.0.7.dev1/nora_lib/interactions/models.py` & `nora_lib-0.0.7.dev2/nora_lib/interactions/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,23 +51,14 @@
         return str(actor_id)
 
     @field_serializer("ts")
     def serialize_ts(self, ts: datetime):
         return ts.isoformat()
 
 
-class EventType(str, Enum):
-    """Event types for the interactions service"""
-
-    AGENT_CONTEXT = "agent:message_context"
-    S2_ANNOTATION = "s2_annotation"
-    THREAD_FORK = "thread_fork"
-    UI_INTERACTION = "ui_interaction"
-
-
 class Event(BaseModel):
     """event object to be sent to the interactions service; requires association with a message, thread or channel id"""
 
     type: str
     actor_id: UUID = Field(
         description="identifies actor writing the event to the interaction service"
     )
@@ -137,20 +128,14 @@
     actor_id: UUID
     text: str
     ts: str
     annotated_text: Optional[str] = None
     events: List[ReturnedAgentContextEvent] = Field(default_factory=list)
 
 
-class ThreadForkEventData(BaseModel):
-    """Event data for a thread fork event"""
-
-    previous_message_id: str
-
-
 class ThreadRelationsResponse(BaseModel):
     """Thread format returned by interaction service for thread relations in a search response"""
 
     thread_id: str
     events: List[Event] = Field(
         default_factory=list
     )  # events associated only with the thread
```

### Comparing `nora_lib-0.0.7.dev1/nora_lib/tasks/models.py` & `nora_lib-0.0.7.dev2/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.7.dev1/nora_lib/tasks/state.py` & `nora_lib-0.0.7.dev2/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.7.dev1/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.7.dev2/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.7.dev1/setup.py` & `nora_lib-0.0.7.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests", "boto3"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.7.dev1",
+    version="0.0.7.dev2",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.7.dev1/tests/tasks/test_state.py` & `nora_lib-0.0.7.dev2/tests/tasks/test_state.py`

 * *Files identical despite different names*

