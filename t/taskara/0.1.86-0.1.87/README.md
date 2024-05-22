# Comparing `tmp/taskara-0.1.86.tar.gz` & `tmp/taskara-0.1.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.86.tar", max compression
+gzip compressed data, was "taskara-0.1.87.tar", max compression
```

## Comparing `taskara-0.1.86.tar` & `taskara-0.1.87.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.86/LICENSE
--rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.86/README.md
--rw-r--r--   0        0        0     1149 2024-05-21 03:10:20.213972 taskara-0.1.86/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.86/taskara/__init__.py
--rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.86/taskara/agent.py
--rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.86/taskara/auth/default.py
--rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.86/taskara/auth/key.py
--rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.86/taskara/auth/provider.py
--rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.86/taskara/auth/transport.py
--rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.86/taskara/cli/main.py
--rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.86/taskara/config.py
--rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.86/taskara/db/conn.py
--rw-r--r--   0        0        0     1639 2024-05-18 03:15:36.180173 taskara-0.1.86/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.86/taskara/env.py
--rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.86/taskara/metrics.py
--rw-r--r--   0        0        0    11573 2024-05-18 03:15:36.180417 taskara-0.1.86/taskara/runtime/base.py
--rw-r--r--   0        0        0    11912 2024-05-20 19:30:07.725603 taskara-0.1.86/taskara/runtime/docker.py
--rw-r--r--   0        0        0    28338 2024-05-18 03:15:36.180876 taskara-0.1.86/taskara/runtime/kube.py
--rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.86/taskara/runtime/load.py
--rw-r--r--   0        0        0    13524 2024-05-18 03:15:36.181232 taskara-0.1.86/taskara/runtime/process.py
--rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.86/taskara/server/app.py
--rw-r--r--   0        0        0     2747 2024-05-20 20:35:44.826563 taskara-0.1.86/taskara/server/models.py
--rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.86/taskara/server/router/tasks.py
--rw-r--r--   0        0        0    35236 2024-05-20 20:35:50.306485 taskara-0.1.86/taskara/task.py
--rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.86/taskara/util.py
--rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.86/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-17 17:09:32.374116 taskara-0.1.87/LICENSE
+-rw-r--r--   0        0        0     2060 2024-05-18 03:15:36.175112 taskara-0.1.87/README.md
+-rw-r--r--   0        0        0     1149 2024-05-22 02:10:01.421342 taskara-0.1.87/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-30 21:36:12.359132 taskara-0.1.87/taskara/__init__.py
+-rw-r--r--   0        0        0     1725 2024-04-30 21:35:45.162984 taskara-0.1.87/taskara/agent.py
+-rw-r--r--   0        0        0       23 2024-04-25 16:52:45.140876 taskara-0.1.87/taskara/auth/default.py
+-rw-r--r--   0        0        0     2548 2024-05-18 03:15:36.178446 taskara-0.1.87/taskara/auth/key.py
+-rw-r--r--   0        0        0     3106 2024-05-18 03:15:36.178774 taskara-0.1.87/taskara/auth/provider.py
+-rw-r--r--   0        0        0     1446 2024-05-18 03:15:36.179051 taskara-0.1.87/taskara/auth/transport.py
+-rw-r--r--   0        0        0     3250 2024-05-18 03:15:36.179410 taskara-0.1.87/taskara/cli/main.py
+-rw-r--r--   0        0        0      672 2024-05-18 03:15:36.179529 taskara-0.1.87/taskara/config.py
+-rw-r--r--   0        0        0     2517 2024-05-18 03:15:36.179872 taskara-0.1.87/taskara/db/conn.py
+-rw-r--r--   0        0        0     1682 2024-05-22 02:05:59.304348 taskara-0.1.87/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-30 21:35:42.361364 taskara-0.1.87/taskara/env.py
+-rw-r--r--   0        0        0     1520 2024-04-30 21:35:40.978077 taskara-0.1.87/taskara/metrics.py
+-rw-r--r--   0        0        0    11823 2024-05-22 02:05:59.304732 taskara-0.1.87/taskara/runtime/base.py
+-rw-r--r--   0        0        0    14256 2024-05-22 02:05:59.305169 taskara-0.1.87/taskara/runtime/docker.py
+-rw-r--r--   0        0        0    30487 2024-05-22 02:05:59.305538 taskara-0.1.87/taskara/runtime/kube.py
+-rw-r--r--   0        0        0     1983 2024-05-18 03:15:36.181027 taskara-0.1.87/taskara/runtime/load.py
+-rw-r--r--   0        0        0    16251 2024-05-22 02:05:59.305817 taskara-0.1.87/taskara/runtime/process.py
+-rw-r--r--   0        0        0     2243 2024-05-18 03:15:36.181763 taskara-0.1.87/taskara/server/app.py
+-rw-r--r--   0        0        0     2798 2024-05-22 02:05:59.306098 taskara-0.1.87/taskara/server/models.py
+-rw-r--r--   0        0        0     8468 2024-05-18 03:15:36.182433 taskara-0.1.87/taskara/server/router/tasks.py
+-rw-r--r--   0        0        0    36114 2024-05-22 02:09:57.737020 taskara-0.1.87/taskara/task.py
+-rw-r--r--   0        0        0     1822 2024-05-20 20:35:44.827574 taskara-0.1.87/taskara/util.py
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 taskara-0.1.87/PKG-INFO
```

### Comparing `taskara-0.1.86/LICENSE` & `taskara-0.1.87/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/README.md` & `taskara-0.1.87/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/pyproject.toml` & `taskara-0.1.87/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskara"
-version = "0.1.86"
+version = "0.1.87"
 description = "Task management for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `taskara-0.1.86/taskara/agent.py` & `taskara-0.1.87/taskara/agent.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/auth/key.py` & `taskara-0.1.87/taskara/auth/key.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/auth/provider.py` & `taskara-0.1.87/taskara/auth/provider.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/auth/transport.py` & `taskara-0.1.87/taskara/auth/transport.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/cli/main.py` & `taskara-0.1.87/taskara/cli/main.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/config.py` & `taskara-0.1.87/taskara/config.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/db/conn.py` & `taskara-0.1.87/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/db/models.py` & `taskara-0.1.87/taskara/db/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
     id = Column(String, primary_key=True)
     owner_id = Column(String, nullable=True)
     description = Column(String, nullable=False)
     max_steps = Column(Integer, nullable=False, default=30)
     device = Column(String, nullable=True)
     device_type = Column(String, nullable=True)
+    expect = Column(String, nullable=True)
     assigned_to = Column(String, nullable=True)
     assigned_type = Column(String, nullable=True)
     status = Column(String, nullable=False)
     created = Column(Float, nullable=False)
     started = Column(Float, nullable=False, default=0.0)
     completed = Column(Float, nullable=False, default=0.0)
     error = Column(String, nullable=True)
```

### Comparing `taskara-0.1.86/taskara/metrics.py` & `taskara-0.1.87/taskara/metrics.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/runtime/base.py` & `taskara-0.1.87/taskara/runtime/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,7 +394,17 @@
             data (Optional[dict], optional): Body data. Defaults to None.
             headers (Optional[dict], optional): Headers. Defaults to None.
 
         Returns:
             Tuple[int, str]: Status code and response text
         """
         pass
+
+    
+    @abstractmethod
+    def refresh(self, owner_id: Optional[str] = None) -> None:
+        """Refresh the runtime
+
+        Args:
+            owner_id (Optional[str], optional): Owner id to scope it to. Defaults to None.
+        """
+        pass
```

### Comparing `taskara-0.1.86/taskara/runtime/docker.py` & `taskara-0.1.87/taskara/runtime/docker.py`

 * *Files 18% similar despite different names*

```diff
@@ -349,7 +349,67 @@
                 return container.logs().decode("utf-8")  # type: ignore
         except NotFound:
             print(f"Container '{name}' does not exist.")
             raise
         except Exception as e:
             print(f"Failed to fetch logs for container '{name}': {e}")
             raise
+
+    def refresh(self, owner_id: Optional[str] = None) -> None:
+        """
+        Reconciles the database against the Docker containers running.
+
+        Parameters:
+            owner_id (Optional[str]): The owner ID to filter the trackers. If None, refreshes for all owners.
+        """
+        # List all Docker containers with the specific label
+        label_filter = {"label": "provisioner=taskara"}
+        running_containers = self.client.containers.list(filters=label_filter, all=True)
+        running_container_names = {container.name for container in running_containers}  # type: ignore
+
+        # List all trackers in the database
+        if owner_id:
+            db_trackers = Tracker.find(owner_id=owner_id, runtime_name=self.name())
+        else:
+            db_trackers = Tracker.find(runtime_name=self.name())
+
+        db_tracker_names = {tracker.name for tracker in db_trackers}
+
+        # Determine trackers to add or remove from the database
+        containers_to_add = running_container_names - db_tracker_names
+        containers_to_remove = db_tracker_names - running_container_names
+
+        # Add new containers to the database
+        for container_name in containers_to_add:
+            container = self.client.containers.get(container_name)
+            env_vars = container.attrs.get("Config", {}).get("Env", [])
+            port = next(
+                (
+                    int(var.split("=")[1])
+                    for var in env_vars
+                    if var.startswith("TASK_SERVER_PORT=")
+                ),
+                9070,
+            )
+            new_tracker = Tracker(
+                name=container_name,
+                runtime=self,
+                port=port,
+                status="running",
+                owner_id=owner_id,
+            )
+            new_tracker.save()
+
+        # Remove containers from the database that are no longer running
+        for tracker_name in containers_to_remove:
+            trackers = Tracker.find(
+                name=tracker_name, owner_id=owner_id, runtime_name=self.name()
+            )
+            if not trackers:
+                continue
+
+            tracker = trackers[0]
+            tracker.delete()
+
+        print(
+            f"Refresh completed: added {len(containers_to_add)} trackers, removed {len(containers_to_remove)} trackers."
+        )
```

### Comparing `taskara-0.1.86/taskara/runtime/kube.py` & `taskara-0.1.87/taskara/runtime/kube.py`

 * *Files 4% similar despite different names*

```diff
@@ -753,7 +753,66 @@
             print(
                 f"Signal {signum} received, stopping and deleting pod '{server_name}'"
             )
             self.delete(server_name)
             sys.exit(1)
 
         return handle_signal
+
+    def refresh(self, owner_id: Optional[str] = None) -> None:
+        """
+        Reconciles the database against the Kubernetes pods running.
+
+        Parameters:
+            owner_id (Optional[str]): The owner ID to filter the trackers. If None, refreshes for all owners.
+        """
+        # List all Kubernetes pods with the specific label
+        label_selector = "provisioner=surfkit"
+        try:
+            running_pods = self.core_api.list_namespaced_pod(
+                namespace=self.namespace, label_selector=label_selector
+            )
+        except ApiException as e:
+            print(f"Failed to list pods: {e}")
+            raise
+
+        running_pod_names = {pod.metadata.name for pod in running_pods.items}
+
+        # List all trackers in the database
+        if owner_id:
+            db_trackers = Tracker.find(owner_id=owner_id, runtime_name=self.name())
+        else:
+            db_trackers = Tracker.find(runtime_name=self.name())
+
+        db_tracker_names = {tracker.name for tracker in db_trackers}
+
+        # Determine trackers to add or remove from the database
+        pods_to_add = running_pod_names - db_tracker_names
+        pods_to_remove = db_tracker_names - running_pod_names
+
+        # Add new pods to the database
+        for pod_name in pods_to_add:
+            pod = self.core_api.read_namespaced_pod(
+                name=pod_name, namespace=self.namespace
+            )
+            new_tracker = Tracker(
+                name=pod_name,
+                runtime=self,
+                port=9070,
+                status="running",
+                owner_id=owner_id,
+            )
+            new_tracker.save()
+
+        # Remove pods from the database that are no longer running
+        for tracker_name in pods_to_remove:
+            trackers = Tracker.find(
+                name=tracker_name, owner_id=owner_id, runtime_name=self.name()
+            )
+            if not trackers:
+                continue
+            tracker = trackers[0]
+            tracker.delete()
+
+        print(
+            f"Refresh completed: added {len(pods_to_add)} trackers, removed {len(pods_to_remove)} trackers."
+        )
```

### Comparing `taskara-0.1.86/taskara/runtime/load.py` & `taskara-0.1.87/taskara/runtime/load.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/runtime/process.py` & `taskara-0.1.87/taskara/runtime/process.py`

 * *Files 11% similar despite different names*

```diff
@@ -383,7 +383,78 @@
                         yield line
 
             return follow_logs()
         else:
             # If not following, return all logs as a single string
             with open(log_path, "r") as log_file:
                 return log_file.read()
+
+    def refresh(self, owner_id: Optional[str] = None) -> None:
+        """
+        Reconciles the database against the running processes.
+
+        Parameters:
+            owner_id (Optional[str]): The owner ID to filter the trackers. If None, refreshes for all owners.
+        """
+        # List all running processes with the specific environment variable
+        all_processes = subprocess.check_output(
+            "ps ax -o pid,command", shell=True, text=True
+        )
+        running_processes = {}
+        for line in all_processes.splitlines():
+            if "TASK_SERVER=" in line:
+                pid, command = line.split(maxsplit=1)
+                server_name = next(
+                    (
+                        part.split("=")[1]
+                        for part in command.split()
+                        if part.startswith("TASK_SERVER=")
+                    ),
+                    None,
+                )
+                if server_name:
+                    running_processes[server_name] = pid
+
+        running_process_names = set(running_processes.keys())
+
+        # List all trackers in the database
+        if owner_id:
+            db_trackers = Tracker.find(owner_id=owner_id, runtime_name=self.name())
+        else:
+            db_trackers = Tracker.find(runtime_name=self.name())
+
+        db_tracker_names = {tracker.name for tracker in db_trackers}
+
+        # Determine trackers to add or remove from the database
+        processes_to_add = running_process_names - db_tracker_names
+        processes_to_remove = db_tracker_names - running_process_names
+
+        # Add new processes to the database
+        for process_name in processes_to_add:
+            try:
+                with open(f".data/proc/{process_name}.json", "r") as f:
+                    metadata = json.load(f)
+
+                new_tracker = Tracker(
+                    name=metadata["name"],
+                    runtime=self,
+                    port=metadata["port"],
+                    status="running",
+                    owner_id=owner_id,
+                )
+                new_tracker.save()
+            except FileNotFoundError:
+                logger.warning(f"No metadata found for process {process_name}")
+
+        # Remove processes from the database that are no longer running
+        for tracker_name in processes_to_remove:
+            trackers = Tracker.find(
+                name=tracker_name, owner_id=owner_id, runtime_name=self.name()
+            )
+            if not trackers:
+                continue
+            tracker = trackers[0]
+            tracker.delete()
+
+        print(
+            f"Refresh completed: added {len(processes_to_add)} trackers, removed {len(processes_to_remove)} trackers."
+        )
```

### Comparing `taskara-0.1.86/taskara/server/app.py` & `taskara-0.1.87/taskara/server/app.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/server/models.py` & `taskara-0.1.87/taskara/server/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 class V1Task(BaseModel):
     id: str = Field(default_factory=lambda: str(uuid.uuid4()))
     description: str
     max_steps: int = 30
     device: Optional[V1Device] = None
     device_type: Optional[V1DeviceType] = None
+    expect_schema: Optional[Dict[str, Any]] = None
     status: Optional[str] = None
     threads: Optional[List[V1RoleThread]] = None
     prompts: Optional[List[str]] = None
     assigned_to: Optional[str] = None
     assigned_type: Optional[str] = None
     created: float = Field(default_factory=time.time)
     started: float = 0.0
```

### Comparing `taskara-0.1.86/taskara/server/router/tasks.py` & `taskara-0.1.87/taskara/server/router/tasks.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/taskara/task.py` & `taskara-0.1.87/taskara/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import uuid
 import time
-from typing import List, Optional, TypeVar, Any, Dict
+from typing import List, Optional, TypeVar, Any, Dict, Type
 import requests
 import os
 import json
 import hashlib
 import logging
 import copy
 
@@ -29,14 +29,15 @@
     def __init__(
         self,
         description: Optional[str] = None,
         max_steps: int = 30,
         owner_id: Optional[str] = None,
         device: Optional[V1Device] = None,
         device_type: Optional[V1DeviceType] = None,
+        expect: Optional[Type[BaseModel]] = None,
         id: Optional[str] = None,
         status: str = "defined",
         created: Optional[float] = None,
         started: float = 0.0,
         completed: float = 0.0,
         threads: List[RoleThread] = [],
         prompts: List[Prompt] = [],
@@ -67,14 +68,15 @@
         self._output = output
         self._parameters = parameters
         self._remote = remote
         self._prompts = prompts
         self._labels = labels
         self._tags = tags
         self._episode = episode
+        self._expect_schema = expect.model_json_schema() if expect else None
 
         self._threads = []
         if threads:
             self._threads.extend(threads)
 
         self._version = version if version is not None else self.generate_version_hash()
 
@@ -131,14 +133,22 @@
         return self._device_type
 
     @device_type.setter
     def device_type(self, value: Optional[V1DeviceType]):
         self._device_type = value
 
     @property
+    def expect(self) -> Optional[Dict[str, Any]]:
+        return self._expect_schema
+
+    @expect.setter
+    def expect(self, value: Optional[Type[BaseModel]]):
+        self._expect_schema = value.model_json_schema() if value else None
+
+    @property
     def owner_id(self) -> Optional[str]:
         return self._owner_id
 
     @owner_id.setter
     def owner_id(self, value: Optional[str]):
         self._owner_id = value
 
@@ -260,24 +270,29 @@
         if self._device:
             device = self._device.model_dump_json()
 
         device_type = None
         if self._device_type:
             device_type = self._device_type.model_dump_json()
 
+        expect = None
+        if self._expect_schema:
+            expect = json.dumps(self._expect_schema)
+
         if not hasattr(self, "_episode") or not self._episode:
             raise ValueError("episode not set")
 
         return TaskRecord(
             id=self._id,
             owner_id=self._owner_id,
             description=self._description,
             max_steps=self._max_steps,
             device=device,
             device_type=device_type,
+            expect=expect,
             status=self._status,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
             assigned_type=self._assigned_type,
             error=self._error,
@@ -308,21 +323,26 @@
         if record.device:  # type: ignore
             device = V1Device.model_validate_json(str(record.device))
 
         device_type = None
         if record.device_type:  # type: ignore
             device_type = V1DeviceType.model_validate_json(str(record.device_type))
 
+        expect = None
+        if record.expect:  # type: ignore
+            expect = json.loads(str(record.expect))
+
         obj = cls.__new__(cls)
         obj._id = record.id
         obj._owner_id = record.owner_id
         obj._description = record.description
         obj._max_steps = record.max_steps
         obj._device = device
         obj._device_type = device_type
+        obj._expect_schema = expect
         obj._status = record.status
         obj._created = record.created
         obj._started = record.started
         obj._completed = record.completed
         obj._assigned_to = record.assigned_to
         obj._assigned_type = record.assigned_type
         obj._error = record.error
@@ -845,14 +865,15 @@
 
         return V1Task(
             id=self._id,
             description=self._description if self._description else "",
             max_steps=self._max_steps,
             device=self._device,
             device_type=self.device_type,
+            expect_schema=self._expect_schema,
             threads=[t.to_v1() for t in self._threads],
             prompts=[p.id for p in self._prompts],
             status=self._status,
             created=self._created,
             started=self._started,
             completed=self._completed,
             assigned_to=self._assigned_to,
@@ -891,14 +912,15 @@
         # Manually set attributes on the object
         obj._id = v1.id if v1.id else str(uuid.uuid4())
         obj._owner_id = owner_id
         obj._description = v1.description
         obj._max_steps = v1.max_steps
         obj._device = v1.device
         obj._device_type = v1.device_type
+        obj._expect_schema = v1.expect_schema
         obj._status = v1.status if v1.status else "defined"
         obj._created = v1.created
         obj._started = v1.started
         obj._completed = v1.completed
         obj._assigned_to = v1.assigned_to
         obj._assigned_type = v1.assigned_type
         obj._error = v1.error
@@ -941,14 +963,15 @@
                 logger.debug(f"found remote task {remote_task}")
                 if remote_task:
                     v1 = V1Task(**remote_task)
                     self._description = v1.description
                     self._max_steps = v1.max_steps
                     self._device = v1.device
                     self._device_type = v1.device_type
+                    self._expect_schema = v1.expect_schema
                     self._status = v1.status if v1.status else "defined"
                     self._created = v1.created
                     self._started = v1.started
                     self._completed = v1.completed
                     self._assigned_to = v1.assigned_to
                     self._assigned_type = v1.assigned_type
                     self._error = v1.error
@@ -972,14 +995,15 @@
         else:
             tasks = self.find(id=self._id)
             task = tasks[0]
             self._description = task._description
             self._max_steps = task._max_steps
             self._device = task._device
             self._device_type = task._device_type
+            self._expect_schema = task._expect_schema
             self._status = task._status
             self._created = task._created
             self._started = task._started
             self._completed = task._completed
             self._assigned_to = task._assigned_to
             self._assigned_type = task._assigned_type
             self._error = task._error
```

### Comparing `taskara-0.1.86/taskara/util.py` & `taskara-0.1.87/taskara/util.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.86/PKG-INFO` & `taskara-0.1.87/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.86
+Version: 0.1.87
 Summary: Task management for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskara Version: 0.1.86 Summary: Task management
+Metadata-Version: 2.1 Name: taskara Version: 0.1.87 Summary: Task management
 for AI agents License: MIT Author: Patrick Barker Author-email:
 patrickbarkerco@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: all Provides-Extra: cli Provides-
 Extra: runtime Requires-Dist: devicebay (>=0.1.24,<0.2.0) Requires-Dist: docker
 (>=7.0.0,<8.0.0) ; extra == "runtime" or extra == "all" Requires-Dist: google-
```

