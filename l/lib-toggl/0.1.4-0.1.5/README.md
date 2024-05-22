# Comparing `tmp/lib_toggl-0.1.4.tar.gz` & `tmp/lib_toggl-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_toggl-0.1.4.tar", max compression
+gzip compressed data, was "lib_toggl-0.1.5.tar", max compression
```

## Comparing `lib_toggl-0.1.4.tar` & `lib_toggl-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.4/LICENSE
--rw-r--r--   0        0        0     3112 2023-12-28 19:42:25.168562 lib_toggl-0.1.4/README.md
--rw-r--r--   0        0        0       87 2023-12-28 19:53:02.130478 lib_toggl-0.1.4/lib_toggl/__init__.py
--rw-r--r--   0        0        0      943 2023-12-28 19:50:29.575332 lib_toggl-0.1.4/lib_toggl/account.py
--rw-r--r--   0        0        0    11631 2023-12-28 19:42:25.168562 lib_toggl-0.1.4/lib_toggl/client.py
--rw-r--r--   0        0        0      371 2023-12-26 19:39:10.972800 lib_toggl-0.1.4/lib_toggl/const.py
--rw-r--r--   0        0        0     6666 2023-12-28 19:50:04.662608 lib_toggl-0.1.4/lib_toggl/time_entries.py
--rw-r--r--   0        0        0     5687 2023-12-28 19:52:58.827141 lib_toggl-0.1.4/lib_toggl/workspace.py
--rw-r--r--   0        0        0      606 2023-12-28 19:48:50.511366 lib_toggl-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 lib_toggl-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-12-26 19:39:10.972800 lib_toggl-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3112 2024-05-22 17:50:45.128033 lib_toggl-0.1.5/README.md
+-rw-r--r--   0        0        0       87 2024-01-18 17:19:23.942907 lib_toggl-0.1.5/lib_toggl/__init__.py
+-rw-r--r--   0        0        0      758 2024-01-18 17:13:20.299494 lib_toggl-0.1.5/lib_toggl/account.py
+-rw-r--r--   0        0        0    29959 2024-05-22 17:50:44.804704 lib_toggl-0.1.5/lib_toggl/client.py
+-rw-r--r--   0        0        0      371 2023-12-26 19:39:10.972800 lib_toggl-0.1.5/lib_toggl/const.py
+-rw-r--r--   0        0        0      559 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/organization.py
+-rw-r--r--   0        0        0     1621 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/tags.py
+-rw-r--r--   0        0        0     9195 2024-05-22 17:25:32.613801 lib_toggl-0.1.5/lib_toggl/time_entries.py
+-rw-r--r--   0        0        0     5688 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/lib_toggl/workspace.py
+-rw-r--r--   0        0        0      628 2024-05-22 02:03:37.351411 lib_toggl-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3658 1970-01-01 00:00:00.000000 lib_toggl-0.1.5/PKG-INFO
```

### Comparing `lib_toggl-0.1.4/LICENSE` & `lib_toggl-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.4/README.md` & `lib_toggl-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lib_toggl-0.1.4/lib_toggl/account.py` & `lib_toggl-0.1.5/lib_toggl/account.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 """Account Information
 Parse/Coercion done by Pydantic
 """
 from datetime import datetime
 from typing import Optional
 
-# Pydantic v2 includes v1 so try importing that first
-# See: https://github.com/kquinsland/lib-toggl/issues/3
-try:
-    from pydantic.v1 import BaseModel, SecretStr
-except ImportError:
-    from pydantic import BaseModel, SecretStr
+from pydantic.v1 import BaseModel, SecretStr
 
 from .const import BASE
 
 ENDPOINT = f"{BASE}/me"
 
 
 class Account(BaseModel):
```

### Comparing `lib_toggl-0.1.4/lib_toggl/time_entries.py` & `lib_toggl-0.1.5/lib_toggl/time_entries.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,85 @@
 """Various type/class definitions for the Organizations bit of the Toggle API
 Parse/Coercion done by Pydantic
 """
+
 import logging
 from datetime import datetime
-from typing import List, Optional
-
-# Pydantic v2 includes v1 so try importing that first
-# See: https://github.com/kquinsland/lib-toggl/issues/3
-try:
-    from pydantic.v1 import BaseModel, Field
-except ImportError:
-    from pydantic import BaseModel, Field
+from typing import Any, List, Optional
 
+from pydantic.v1 import BaseModel, Field, validator
 from pyrfc3339 import generate
 
 from .const import BASE, DEFAULT_CREATED_BY
 
 log = logging.getLogger(__name__)
 
 ENDPOINT = f"{BASE}/me/time_entries"
 
 
 @staticmethod
-# pylint: disable=invalid-name
-def CREATE_ENDPOINT(workspace_id: int = None) -> str:
-    """Returns the endpoint for creating a new time entry in the specified workspace"""
+def validate_time_entry_id(time_entry_id: Any) -> None:
+    """Raises Value Error if time_entry_id is not a positive integer.
+    Allow for `Any` as the type to allow for None to be passed in as a value
+    """
+    if not time_entry_id:
+        raise ValueError("time_entry_id must be specified")
+    if not isinstance(time_entry_id, int):
+        raise TypeError("time_entry_id must be an integer")
+    if time_entry_id <= 0:
+        raise ValueError("time_entry_id must be positive.")
+
+
+@staticmethod
+def validate_workspace_id(workspace_id: Any) -> None:
+    """Raises Value Error if workspace_id is not a positive integer
+    Allow for `Any` as the type to allow for None to be passed in as a value
+    """
     if not workspace_id:
         raise ValueError("workspace_id must be specified")
+    if not isinstance(workspace_id, int):
+        raise TypeError("workspace_id must be an integer")
+    if workspace_id <= 0:
+        raise ValueError("workspace_id must be positive.")
+
+
+@staticmethod
+# pylint: disable=invalid-name
+def CREATE_ENDPOINT(workspace_id: int) -> str:
+    """Returns the endpoint for creating a new time entry in the specified workspace"""
+    validate_workspace_id(workspace_id)
     return f"{BASE}/workspaces/{workspace_id}/time_entries"
 
 
 @staticmethod
 # pylint: disable=invalid-name
-def STOP_ENDPOINT(workspace_id: int = None, time_entry_id: int = None) -> str:
+def STOP_ENDPOINT(workspace_id: int, time_entry_id: int) -> str:
     """Returns the endpoint for creating a new time entry in the specified workspace"""
-    if not workspace_id:
-        raise ValueError("workspace_id must be specified")
-    if not time_entry_id:
-        raise ValueError("time_entry_id must be specified")
+    validate_workspace_id(workspace_id)
+    validate_time_entry_id(time_entry_id)
     return f"{BASE}/workspaces/{workspace_id}/time_entries/{time_entry_id}/stop"
 
 
+@staticmethod
+# pylint: disable=invalid-name
+def EDIT_ENDPOINT(workspace_id: int, time_entry_id: int) -> str:
+    """Returns the endpoint for editing specific time entry in the specified workspace"""
+    validate_workspace_id(workspace_id)
+    validate_time_entry_id(time_entry_id)
+    return f"{BASE}/workspaces/{workspace_id}/time_entries/{time_entry_id}"
+
+
+@staticmethod
+# pylint: disable=invalid-name
+def EXPLICIT_ENDPOINT(time_entry_id: int) -> str:
+    """Returns the endpoint for editing specific time entry in the specified workspace"""
+    validate_time_entry_id(time_entry_id)
+    return f"{BASE}/me/time_entries/{time_entry_id}"
+
+
 class TimeEntry(BaseModel):
     """Class representing the Toggl organization object.
     Leverages dataclass to cut down on boilerplate code.
     See: https://developers.track.toggl.com/docs/api/time_entries#200
     """
 
     # For Pydantic v1, a sub `config` class holds the custom serialization config.
@@ -62,18 +97,20 @@
 
     # When user creates a TimeEntry, this will not be known; it is set by server when successful CREATE request
     id: Optional[int] = Field(default=None)
     # Toggle API has a few fields that are "legacy" and "should not be used" but are still
     #   returned by the API. We store the new/current/correct field value and set up aliases
     #   so the old field names still work.
     ##
-    # TODO: do I want to frozen everything? May want to support updating a TE in the future...?
     workspace_id: int = Field(description="Workspace ID, required.", default=None)
+
     project_id: Optional[int] = Field(description="Project ID, optional.", default=None)
+
     task_id: Optional[int] = Field(alias="tid", default=None)
+
     user_id: int = Field(
         default=None,
         description="Time Entry creator ID, if omitted will use the requester user ID",
     )
 
     billable: bool = Field(
         default=False,
@@ -83,57 +120,68 @@
     created_with: str = Field(
         description="Must be provided when creating a time entry and should identify the service/application used to create it",
         # value will NOT be provided when making a "get current" call so we default to None
         default=DEFAULT_CREATED_BY,
     )
 
     # Toggl API wants everything in RFC3339 format which is just a specific flavor of ISO8601
-    # Internally, just store everything as a datetime with UTC timezone and only convert to
+    # Internally, just store everything as a TZ aware datetime with UTC timezone and only convert to
     #   RFC3339 when we need to send it to the API.
-    start: datetime = Field(default_factory=datetime.utcnow)
+    ##
+    # Note that Toggle API **requires** that a start datetime be provided when creating a new Time Entry.
+    # No longer going to enforce this / default to now() in model creation as there are some valid use cases for
+    #   a model that does not have a start time set.
+    # As a convenience, the API client will check for start of None and automatically set to now() during the create() calls.
+    start: Optional[datetime] = Field(
+        default=None,
+        # pylint: disable=line-too-long
+        description="Start `datetime` in UTC, required when creating a new Time Entry, optional when updating an existing one.",
+    )
+
     stop: Optional[datetime] = Field(
         default=None,
         # pylint: disable=line-too-long
-        description="Stop time in UTC, can be omitted if it's still running or created with 'duration'. If 'stop' and 'duration' are provided, values must be consistent (start + duration == stop)",
+        description="Stop `datetime` in UTC, can be omitted if it's still running or created with 'duration'. If 'stop' and 'duration' are provided, values must be consistent (start + duration == stop)",
     )
 
     # Duration in seconds
     # Should be -1 for something that's on-going but should be correct for creating an "already-done" TE
     # e.g. start + duration = stop
     # TODO: better validation around this field with the After validation
     # https://docs.pydantic.dev/2.5/concepts/validators/#before-after-wrap-and-plain-validators
     duration: int = Field(
         default=-1,
-        description="Time entry duration. For running entries should be negative, preferable -1",
+        description="Time entry duration. For running entries should be negative, preferable `-1`",
     )
 
     # Description is required when CREATING, but not required when deleting.
     description: Optional[str] = Field(
         default=None, description="Time entry description, optional"
     )
-    # Can be "add" or "delete". Used when updating an existing time entry
+
     tag_action: Optional[str] = Field(pattern=r"^(add|delete)$", default="add")
 
-    tags: List[str] = Field(
-        default=None,
-        description="Tag names, None if tags were not provided or were later deleted",
+    tags: Optional[List[str]] = Field(
+        default=[],
+        description="Tag names",
     )
 
-    tag_ids: List[int] = Field(
-        default=None,
-        description="Tag IDs, None if tags were not provided or were later deleted",
+    tag_ids: Optional[List[int]] = Field(
+        default=[],
+        description="Tag IDs.",
     )
 
     # This field is deprecated for GET endpoints where the value will always be true.
     duronly: Optional[bool] = Field(
         exclude=True,
         default=False,
         repr=False,
         description="Deprecated: Used to create a time entry with a duration but without a stop time. This parameter can be ignored.",
     )
+
     # This appears to be the datetime server got/fulfilled request
     # Isn't something user will supply when creating a Time Entry and doesn't really serve a useful
     #   purpose so we exclude it from the model.
     at: Optional[datetime] = Field(
         exclude=True, default=None, description="When was last updated", repr=False
     )
 
@@ -143,21 +191,45 @@
 
     uid: Optional[int] = Field(
         exclude=True,
         default=None,
         repr=False,
         description="Time Entry creator ID, legacy field",
     )
+
     wid: Optional[int] = Field(
         exclude=True, default=None, repr=False, description="Workspace ID, legacy field"
     )
+
     pid: Optional[int] = Field(
         exclude=True, default=None, repr=False, description="Project ID, legacy field"
     )
+
     tid: Optional[int] = Field(
         exclude=True, default=None, repr=False, description="Task ID, legacy field"
     )
 
-
-# TODO: general logic implementation around what fields are required / should be validated
-#   when user is creating a new TE versus updating one versus getting current from API.
-# TODO: fix: TypeError: 'TimeEntry' object is not subscriptable
+    # The Toggl API continues to "amaze".
+    # It is absolutely possible to get a reply that looks like this:
+    #       "tags":null,"tag_ids":[]
+    # Which when parsed as json results in tags = None, tag_ids = []
+    # Internally, Pydantic's Optional[] is a Union of the type and None.
+    # This means that we technically are allowed to pass None as a value for tags and tag_ids.
+    # This makes things simple if the user wants to create a TimeEntry with no tags, for example.
+    # But internally, we do not want to expose `None` to the user as a valid value for tags.
+    # The list of tags/tags_ids should always be a list, even if it's an empty list.
+    ##
+    # pylint: disable=no-self-argument
+    @validator("tags", "tag_ids", always=True)
+    def tags_must_not_be_null(cls, v):
+        """Ensures that tag/tag_ids is always an empty list not None
+
+        Args:
+            v (_type_): Value of the field to be validated
+
+        Returns:
+            _type_: `v` if `v` is not None, else an empty list
+        """
+        if v is None:
+            return []
+        else:
+            return v
```

### Comparing `lib_toggl-0.1.4/lib_toggl/workspace.py` & `lib_toggl-0.1.5/lib_toggl/workspace.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Various type/class definitions for the Workspaces bit of the Toggle API
 Parse/Coercion done by Pydantic
 """
+
 import logging
 from datetime import datetime
 from typing import Any, Optional
 
-try:
-    from pydantic.v1 import BaseModel, Field, SecretStr
-except ImportError:
-    from pydantic import BaseModel, Field, SecretStr
+from pydantic import BaseModel, Field, SecretStr
 
 from .const import BASE
 
 log = logging.getLogger(__name__)
 
 ENDPOINT = f"{BASE}/workspaces"
 
@@ -196,7 +194,9 @@
         exclude=True, default=None, description="When was deleted, null if not deleted"
     )
 
     working_hours_in_minutes: Optional[int] = Field(
         default=None,
         description="TODO (unconfirmed)",
     )
+
+    # TODO: tags seem to belong to a workspace, so move the get_tags() method here?
```

### Comparing `lib_toggl-0.1.4/pyproject.toml` & `lib_toggl-0.1.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-toggl"
-version = "0.1.4"
+version = "0.1.5"
 description = "Asynchronous Python library for the Toggl API."
 authors = ["Karl Quinsalnd <karl@karlquinsland.com>"]
 readme = "README.md"
 packages = [{ include = "lib_toggl" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -17,11 +17,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.0.3"
 isort = "^5.13.2"
 black = "^23.12.0"
 pytest = "^7.4.3"
 pytest-asyncio = "^0.23.2"
+structlog = "^24.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lib_toggl-0.1.4/PKG-INFO` & `lib_toggl-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-toggl
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous Python library for the Toggl API.
 Author: Karl Quinsalnd
 Author-email: karl@karlquinsland.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodns (>=3.1.1,<4.0.0)
```

