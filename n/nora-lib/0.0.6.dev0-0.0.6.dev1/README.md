# Comparing `tmp/nora_lib-0.0.6.dev0.tar.gz` & `tmp/nora_lib-0.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nora_lib-0.0.6.dev0.tar", last modified: Tue May 21 21:31:49 2024, max compression
+gzip compressed data, was "nora_lib-0.0.6.dev1.tar", last modified: Tue May 21 22:28:27 2024, max compression
```

## Comparing `nora_lib-0.0.6.dev0.tar` & `nora_lib-0.0.6.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.757583 nora_lib-0.0.6.dev0/
--rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 21:31:49.757219 nora_lib-0.0.6.dev0/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/README.md
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.745589 nora_lib-0.0.6.dev0/nora_lib/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/__init__.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.749176 nora_lib-0.0.6.dev0/nora_lib/context/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/context/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev0/nora_lib/context/context_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev0/nora_lib/context/models.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.751650 nora_lib-0.0.6.dev0/nora_lib/interactions/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)    11125 2024-05-21 21:30:45.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/interactions_service.py
--rw-r--r--   0 stefanc    (502) staff       (20)     4659 2024-05-21 21:09:30.000000 nora_lib-0.0.6.dev0/nora_lib/interactions/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/py.typed
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.753562 nora_lib-0.0.6.dev0/nora_lib/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/models.py
--rw-r--r--   0 stefanc    (502) staff       (20)     5553 2024-05-21 21:25:27.000000 nora_lib-0.0.6.dev0/nora_lib/tasks/state.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.756246 nora_lib-0.0.6.dev0/nora_lib.egg-info/
--rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/PKG-INFO
--rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/SOURCES.txt
--rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/dependency_links.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       70 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/requires.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-21 21:31:49.000000 nora_lib-0.0.6.dev0/nora_lib.egg-info/top_level.txt
--rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/pyproject.toml
--rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-21 21:31:49.757718 nora_lib-0.0.6.dev0/setup.cfg
--rw-r--r--   0 stefanc    (502) staff       (20)      614 2024-05-21 21:16:46.000000 nora_lib-0.0.6.dev0/setup.py
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.754205 nora_lib-0.0.6.dev0/tests/
-drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 21:31:49.755416 nora_lib-0.0.6.dev0/tests/tasks/
--rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/tasks/__init__.py
--rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/tasks/test_state.py
--rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev0/tests/test_placeholder.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.026868 nora_lib-0.0.6.dev1/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 22:28:27.026165 nora_lib-0.0.6.dev1/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      887 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/README.md
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.013520 nora_lib-0.0.6.dev1/nora_lib/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/__init__.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.017402 nora_lib-0.0.6.dev1/nora_lib/context/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/context/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     1338 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev1/nora_lib/context/context_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      356 2024-05-17 21:59:16.000000 nora_lib-0.0.6.dev1/nora_lib/context/models.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.019632 nora_lib-0.0.6.dev1/nora_lib/interactions/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/interactions/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)    11071 2024-05-21 22:26:47.000000 nora_lib-0.0.6.dev1/nora_lib/interactions/interactions_service.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     4711 2024-05-21 22:26:47.000000 nora_lib-0.0.6.dev1/nora_lib/interactions/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/py.typed
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.021560 nora_lib-0.0.6.dev1/nora_lib/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      925 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/nora_lib/tasks/models.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     5553 2024-05-21 21:25:27.000000 nora_lib-0.0.6.dev1/nora_lib/tasks/state.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.024866 nora_lib-0.0.6.dev1/nora_lib.egg-info/
+-rw-r--r--   0 stefanc    (502) staff       (20)      433 2024-05-21 22:28:26.000000 nora_lib-0.0.6.dev1/nora_lib.egg-info/PKG-INFO
+-rw-r--r--   0 stefanc    (502) staff       (20)      587 2024-05-21 22:28:27.000000 nora_lib-0.0.6.dev1/nora_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)        1 2024-05-21 22:28:26.000000 nora_lib-0.0.6.dev1/nora_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       70 2024-05-21 22:28:26.000000 nora_lib-0.0.6.dev1/nora_lib.egg-info/requires.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       15 2024-05-21 22:28:26.000000 nora_lib-0.0.6.dev1/nora_lib.egg-info/top_level.txt
+-rw-r--r--   0 stefanc    (502) staff       (20)       90 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/pyproject.toml
+-rw-r--r--   0 stefanc    (502) staff       (20)       38 2024-05-21 22:28:27.027006 nora_lib-0.0.6.dev1/setup.cfg
+-rw-r--r--   0 stefanc    (502) staff       (20)      614 2024-05-21 22:27:10.000000 nora_lib-0.0.6.dev1/setup.py
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.022425 nora_lib-0.0.6.dev1/tests/
+drwxr-xr-x   0 stefanc    (502) staff       (20)        0 2024-05-21 22:28:27.023700 nora_lib-0.0.6.dev1/tests/tasks/
+-rw-r--r--   0 stefanc    (502) staff       (20)        0 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/tests/tasks/__init__.py
+-rw-r--r--   0 stefanc    (502) staff       (20)     2670 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/tests/tasks/test_state.py
+-rw-r--r--   0 stefanc    (502) staff       (20)      123 2024-05-15 18:27:33.000000 nora_lib-0.0.6.dev1/tests/test_placeholder.py
```

### Comparing `nora_lib-0.0.6.dev0/README.md` & `nora_lib-0.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.6.dev0/nora_lib/context/context_service.py` & `nora_lib-0.0.6.dev1/nora_lib/context/context_service.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.6.dev0/nora_lib/interactions/interactions_service.py` & `nora_lib-0.0.6.dev1/nora_lib/interactions/interactions_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,16 +111,15 @@
             )
         )
         messages_with_events.extend(messages_for_thread.messages)
 
         # Process any thread_fork events
         try:
             for msg in messages_for_thread.messages:
-                events = msg.events if msg.events else []
-                for event in events:
+                for event in msg.events:
                     if event.type == EventType.THREAD_FORK.value:
                         event_data = ThreadForkEventData.model_validate(event.data)
                         forked_thread: ThreadRelationsResponse = (
                             self.fetch_thread_messages_and_events_for_message(
                                 event_data.previous_message_id, [event_type]
                             )
                         )
```

### Comparing `nora_lib-0.0.6.dev0/nora_lib/interactions/models.py` & `nora_lib-0.0.6.dev1/nora_lib/interactions/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     message_id: str
     actor_id: UUID
     text: str
     thread_id: Optional[str]
     channel_id: str
     surface: Surface
     ts: datetime
-    annotations: Optional[List[Annotation]] = None
+    annotations: List[Annotation] = Field(default_factory=list)
 
     @field_serializer("actor_id")
     def serialize_actor_id(self, actor_id: UUID):
         return str(actor_id)
 
     @field_serializer("ts")
     def serialize_ts(self, ts: datetime):
@@ -90,18 +90,18 @@
     """Message format returned by interaction service"""
 
     message_id: str
     actor_id: UUID
     text: str
     ts: datetime
     annotated_text: Optional[str] = None
-    events: Optional[List[Event]] = None
+    events: List[Event] = Field(default_factory=list)
     thread_id: Optional[str] = None
     channel_id: Optional[str] = None
-    annotations: Optional[List[Annotation]] = None
+    annotations: List[Annotation] = Field(default_factory=list)
 
 
 class AgentMessageData(BaseModel):
     """capture requests to and responses from tools within Events"""
 
     message_data: dict  # dict of agent/tool request/response format
     data_sender_actor_id: Optional[str] = None  # agent sending the data
@@ -123,15 +123,15 @@
     """Message format returned by interaction service for search by thread"""
 
     message_id: str
     actor_id: UUID
     text: str
     ts: str
     annotated_text: Optional[str] = None
-    events: Optional[List[ReturnedAgentContextEvent]] = None
+    events: List[ReturnedAgentContextEvent] = Field(default_factory=list)
 
 
 class ThreadForkEventData(BaseModel):
     """Event data for a thread fork event"""
 
     previous_message_id: str
```

### Comparing `nora_lib-0.0.6.dev0/nora_lib/tasks/models.py` & `nora_lib-0.0.6.dev1/nora_lib/tasks/models.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.6.dev0/nora_lib/tasks/state.py` & `nora_lib-0.0.6.dev1/nora_lib/tasks/state.py`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.6.dev0/nora_lib.egg-info/SOURCES.txt` & `nora_lib-0.0.6.dev1/nora_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nora_lib-0.0.6.dev0/setup.py` & `nora_lib-0.0.6.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 runtime_requirements = ["pydantic>=2,<3", "requests", "boto3"]
 
 # For running tests, linting, etc
 dev_requirements = ["mypy", "pytest", "black", "types-requests"]
 
 setuptools.setup(
     name="nora_lib",
-    version="0.0.6.dev0",
+    version="0.0.6.dev1",
     description="For making and coordinating agents and tools",
     url="https://github.com/allenai/nora_lib",
     packages=setuptools.find_packages(exclude=(["tests"])),
     install_requires=runtime_requirements,
     package_data={
         "nora_lib": ["py.typed"],
     },
```

### Comparing `nora_lib-0.0.6.dev0/tests/tasks/test_state.py` & `nora_lib-0.0.6.dev1/tests/tasks/test_state.py`

 * *Files identical despite different names*

