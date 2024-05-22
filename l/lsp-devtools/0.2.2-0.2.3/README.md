# Comparing `tmp/lsp_devtools-0.2.2.tar.gz` & `tmp/lsp_devtools-0.2.3.tar.gz`

## Comparing `lsp_devtools-0.2.2.tar` & `lsp_devtools-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/CHANGES.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/__main__.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/cli.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/database.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/py.typed
--rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/agent/__init__.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/agent/agent.py
--rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/agent/client.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/agent/protocol.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/agent/server.py
--rw-r--r--   0        0        0     5162 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/__init__.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/app.css
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/lsp.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/editor/__init__.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/editor/completion.py
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/client/editor/text_editor.py
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/handlers/__init__.py
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/handlers/dbinit.sql
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/handlers/sql.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/inspector/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/inspector/app.css
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/record/__init__.py
--rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/record/filters.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/record/formatters.py
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/lsp_devtools/record/visualize.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/tests/test_agent.py
--rw-r--r--   0        0        0    13024 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/tests/record/test_filters.py
--rw-r--r--   0        0        0     5298 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/tests/record/test_formatters.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/tests/record/test_record.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/tests/servers/simple.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/LICENSE
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/README.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/hatch.toml
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 lsp_devtools-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/CHANGES.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/__main__.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/cli.py
+-rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/database.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/py.typed
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/agent/__init__.py
+-rw-r--r--   0        0        0     7223 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/agent/agent.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/agent/client.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/agent/protocol.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/agent/server.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/__init__.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/app.css
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/lsp.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/editor/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/editor/completion.py
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/client/editor/text_editor.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/handlers/__init__.py
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/handlers/dbinit.sql
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/handlers/sql.py
+-rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/inspector/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/inspector/app.css
+-rw-r--r--   0        0        0    10410 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/record/__init__.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/record/filters.py
+-rw-r--r--   0        0        0     4957 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/record/formatters.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/lsp_devtools/record/visualize.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/tests/test_agent.py
+-rw-r--r--   0        0        0    13112 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/tests/record/test_filters.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/tests/record/test_formatters.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/tests/record/test_record.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/tests/servers/simple.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/README.md
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/hatch.toml
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 lsp_devtools-0.2.3/PKG-INFO
```

### Comparing `lsp_devtools-0.2.2/CHANGES.md` & `lsp_devtools-0.2.3/CHANGES.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+## v0.2.3 - 2024-05-22
+
+
+### Enhancements
+
+- The `lsp-devtools agent` now forwards the server's `stderr` channel ([#165](https://github.com/swyddfa/lsp-devtools/issues/165))
+
+### Fixes
+
+- All `lsp-devtools` commands should no longer crash when encountering messages containing unicode characters ([#157](https://github.com/swyddfa/lsp-devtools/issues/157))
+- Commands like `lsp-devtools record` should now continue to function after encountering an error ([#158](https://github.com/swyddfa/lsp-devtools/issues/158))
+
+
 ## v0.2.2 - 2024-01-29
 
 
 ### Enhancements
 
 - Added formatters `json` and `json-compact` that can be used within format strings. ([#130](https://github.com/swyddfa/lsp-devtools/issues/130))
 - When not printing messages to stdout, the `lsp-devtools record` command now displays a nice visualisation of the traffic between client and server - so that you can see that it's doing something ([#134](https://github.com/swyddfa/lsp-devtools/issues/134))
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/cli.py` & `lsp_devtools-0.2.3/lsp_devtools/cli.py`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/lsp_devtools/database.py` & `lsp_devtools-0.2.3/lsp_devtools/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 import sys
 from contextlib import asynccontextmanager
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Set
-from uuid import uuid4
 
 import aiosqlite
 from textual.app import App
 from textual.message import Message
 
 from lsp_devtools.handlers import LspMessage
 
-if sys.version_info.minor < 9:
+if sys.version_info < (3, 9):
     import importlib_resources as resources
 else:
-    import importlib.resources as resources  # type: ignore[no-redef]
+    from importlib import resources  # type: ignore[no-redef]
 
 
 class Database:
     """Controls access to the backing sqlite database."""
 
     class Update(Message):
         """Sent when there are updates to the database"""
@@ -58,22 +57,22 @@
             await self.db.commit()
 
         cursor = await self.db.cursor()
         yield cursor
 
         await self.db.commit()
 
-    async def add_message(self, session: str, timestamp: float, source: str, rpc: dict):
+    async def add_message(self, session: str, timestamp: str, source: str, rpc: dict):
         """Add a new rpc message to the database."""
 
-        msg_id = rpc.get("id", None)
-        method = rpc.get("method", None)
-        params = rpc.get("params", None)
-        result = rpc.get("result", None)
-        error = rpc.get("error", None)
+        msg_id = rpc.get("id")
+        method = rpc.get("method")
+        params = rpc.get("params")
+        result = rpc.get("result")
+        error = rpc.get("error")
 
         async with self.cursor() as cursor:
             await cursor.execute(
                 "INSERT INTO protocol VALUES (?, ?, ?, ?, ?, ?, ?, ?)",
                 (
                     session,
                     timestamp,
@@ -145,23 +144,25 @@
 
             return results
 
 
 class DatabaseLogHandler(logging.Handler):
     """A logging handler that records messages in the given database."""
 
-    def __init__(self, db: Database, *args, session=None, **kwargs):
+    def __init__(self, db: Database, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.db = db
-        self.session = session or str(uuid4())
         self._tasks: Set[asyncio.Task] = set()
 
     def emit(self, record: logging.LogRecord):
         body = json.loads(record.args[0])  # type: ignore
         task = asyncio.create_task(
             self.db.add_message(
-                self.session, record.created, record.__dict__["source"], body
+                record.__dict__["Message-Session"],
+                record.__dict__["Message-Timestamp"],
+                record.__dict__["Message-Source"],
+                body,
             )
         )
 
         self._tasks.add(task)
         task.add_done_callback(self._tasks.discard)
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/agent/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/agent/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,89 +1,60 @@
 import argparse
 import asyncio
-import logging
 import subprocess
 import sys
 from typing import List
-from uuid import uuid4
 
 from .agent import Agent
+from .agent import RPCMessage
 from .agent import logger
+from .agent import parse_rpc_message
 from .client import AgentClient
-from .protocol import MESSAGE_TEXT_NOTIFICATION
-from .protocol import MessageText
 from .server import AgentServer
-from .server import parse_rpc_message
 
 __all__ = [
     "Agent",
     "AgentClient",
     "AgentServer",
+    "RPCMessage",
     "logger",
-    "MESSAGE_TEXT_NOTIFICATION",
-    "MessageText",
     "parse_rpc_message",
 ]
 
 
-class MessageHandler(logging.Handler):
-    """Logging handler that forwards captured JSON-RPC messages through to the
-    ``AgentServer`` instance."""
-
-    def __init__(self, client: AgentClient, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.client = client
-        self.session = str(uuid4())
-        self._buffer: List[MessageText] = []
-
-    def emit(self, record: logging.LogRecord):
-        message = MessageText(
-            text=record.args[0],  # type: ignore
-            session=self.session,
-            timestamp=record.created,
-            source=record.__dict__["source"],
-        )
-
-        if not self.client.connected:
-            self._buffer.append(message)
-            return
-
-        # Send any buffered messages
-        while len(self._buffer) > 0:
-            self.client.protocol.message_text_notification(self._buffer.pop(0))
-
-        self.client.protocol.message_text_notification(message)
+async def forward_stderr(server: asyncio.subprocess.Process):
+    """Forward the server's stderr to the agent's stderr."""
+    if server.stderr is None:
+        return
+
+    # EOF is signalled with an empty bytestring
+    while (line := await server.stderr.readline()) != b"":
+        sys.stderr.buffer.write(line)
 
 
 async def main(args, extra: List[str]):
     if extra is None:
         print("Missing server start command", file=sys.stderr)
         return 1
 
     command, *arguments = extra
-
     server = await asyncio.create_subprocess_exec(
         command,
         *arguments,
         stdin=subprocess.PIPE,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
     )
-    agent = Agent(server, sys.stdin.buffer, sys.stdout.buffer)
-
     client = AgentClient()
-    handler = MessageHandler(client)
-    handler.setLevel(logging.INFO)
-
-    logger.setLevel(logging.INFO)
-    logger.addHandler(handler)
+    agent = Agent(server, sys.stdin.buffer, sys.stdout.buffer, client.forward_message)
 
     await asyncio.gather(
         client.start_tcp(args.host, args.port),
         agent.start(),
+        forward_stderr(server),
     )
 
 
 def run_agent(args, extra: List[str]):
     asyncio.run(main(args, extra))
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/agent/client.py` & `lsp_devtools-0.2.3/lsp_devtools/agent/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+from __future__ import annotations
+
 import asyncio
-from typing import Any
-from typing import Optional
+import typing
 
 import stamina
 from pygls.client import JsonRPCClient
 from pygls.client import aio_readline
 from pygls.protocol import default_converter
 
 from lsp_devtools.agent.protocol import AgentProtocol
 
+if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import List
+    from typing import Optional
+
 # from websockets.client import WebSocketClientProtocol
 
 
 # class WebSocketClientTransportAdapter:
 #     """Protocol adapter for the WebSocket client interface."""
 
 #     def __init__(self, ws: WebSocketClientProtocol, loop: asyncio.AbstractEventLoop):
@@ -35,14 +41,15 @@
     protocol: AgentProtocol
 
     def __init__(self):
         super().__init__(
             protocol_cls=AgentProtocol, converter_factory=default_converter
         )
         self.connected = False
+        self._buffer: List[bytes] = []
 
     def _report_server_error(self, error, source):
         # Bail on error
         # TODO: Report the actual error somehow
         self._stop_event.set()
 
     def feature(self, feature_name: str, options: Optional[Any] = None):
@@ -67,14 +74,30 @@
         self.protocol.connection_made(writer)  # type: ignore[arg-type]
         connection = asyncio.create_task(
             aio_readline(self._stop_event, reader, self.protocol.data_received)
         )
         self.connected = True
         self._async_tasks.append(connection)
 
+    def forward_message(self, message: bytes):
+        """Forward the given message to the server instance."""
+
+        if not self.connected:
+            self._buffer.append(message)
+            return
+
+        if self.protocol.transport is None:
+            return
+
+        # Send any buffered messages
+        while len(self._buffer) > 0:
+            self.protocol.transport.write(self._buffer.pop(0))
+
+        self.protocol.transport.write(message)
+
     # TODO: Upstream this... or at least something equivalent.
     # def start_ws(self, host: str, port: int):
     #     self.protocol._send_only_body = True  # Don't send headers within the payload
 
     #     async def client_connection(host: str, port: int):
     #         """Create and run a client connection."""
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/client/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,17 @@
         self.server_command = server_command
         self.lsp_client = LanguageClient()
 
         self._async_tasks: List[asyncio.Task] = []
 
     def compose(self) -> ComposeResult:
         message_viewer = MessageViewer("")
-        messages_table = MessagesTable(self.db, message_viewer, session=self.session)
+        messages_table = MessagesTable(
+            self.db, message_viewer, session=self.lsp_client.session_id
+        )
 
         yield Header()
         yield Explorer(".")
         yield EditorView(self.lsp_client)
         devtools = Devtools(ScrollableContainer(messages_table), message_viewer)
         devtools.add_class("-hidden")
         yield devtools
@@ -141,15 +143,15 @@
 def client(args, extra: List[str]):
     if len(extra) == 0:
         raise ValueError("Missing server command.")
 
     db = Database(args.dbpath)
 
     session = str(uuid4())
-    dbhandler = DatabaseLogHandler(db, session=session)
+    dbhandler = DatabaseLogHandler(db)
     dbhandler.setLevel(logging.INFO)
 
     logger.setLevel(logging.INFO)
     logger.addHandler(dbhandler)
 
     app = LSPClient(db, session=session, server_command=extra)
     app.run()
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/client/lsp.py` & `lsp_devtools-0.2.3/lsp_devtools/client/lsp.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import importlib.metadata
 import json
+from datetime import datetime
+from datetime import timezone
 from typing import Optional
+from uuid import uuid4
 
 from lsprotocol import types
 from pygls.lsp.client import BaseLanguageClient
 from pygls.protocol import LanguageServerProtocol
 
 from lsp_devtools.agent import logger
 
+UTC = timezone.utc
 VERSION = importlib.metadata.version("lsp-devtools")
 
 
 class RecordingLSProtocol(LanguageServerProtocol):
     """A version of the LanguageServerProtocol that also records all the traffic."""
 
     def __init__(self, server, converter):
         super().__init__(server, converter)
+        self.session_id = ""
 
     def _procedure_handler(self, message):
         logger.info(
             "%s",
             json.dumps(message, default=self._serialize_message),
-            extra={"source": "server"},
+            extra={
+                "Message-Source": "server",
+                "Message-Session": self.session_id,
+                "Message-Timestamp": datetime.now(tz=UTC).isoformat(),
+            },
         )
         return super()._procedure_handler(message)
 
     def _send_data(self, data):
         logger.info(
             "%s",
             json.dumps(data, default=self._serialize_message),
-            extra={"source": "client"},
+            extra={
+                "Message-Source": "client",
+                "Message-Session": self.session_id,
+                "Message-Timestamp": datetime.now(tz=UTC).isoformat(),
+            },
         )
         return super()._send_data(data)
 
 
 class LanguageClient(BaseLanguageClient):
     """A language client for integrating with a textual text edit."""
 
     def __init__(self):
         super().__init__("lsp-devtools", VERSION, protocol_cls=RecordingLSProtocol)
 
+        self.session_id = str(uuid4())
+        self.protocol.session_id = self.session_id  # type: ignore[attr-defined]
         self._server_capabilities: Optional[types.ServerCapabilities] = None
 
     @property
     def server_capabilities(self) -> types.ServerCapabilities:
         if self._server_capabilities is None:
             raise RuntimeError(
                 "sever_capabilities is None - has the server been initialized?"
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/client/editor/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/client/editor/__init__.py`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/lsp_devtools/client/editor/completion.py` & `lsp_devtools-0.2.3/lsp_devtools/client/editor/completion.py`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/lsp_devtools/client/editor/text_editor.py` & `lsp_devtools-0.2.3/lsp_devtools/client/editor/text_editor.py`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/lsp_devtools/handlers/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/handlers/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+from __future__ import annotations
+
 import json
 import logging
-from typing import Any
-from typing import Literal
-from typing import Mapping
-from typing import Optional
-from uuid import uuid4
+import typing
+from datetime import datetime
 
 import attrs
 
-MessageSource = Literal["client", "server"]
+if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import Literal
+    from typing import Mapping
+    from typing import Optional
+
+    MessageSource = Literal["client", "server"]
 
 
 def maybe_json(value):
     try:
         return json.loads(value)
     except Exception:
         return value
 
 
 @attrs.define
 class LspMessage:
     """A container that holds a message from the LSP protocol, with some additional
     metadata."""
 
-    Source = MessageSource
-
     session: str
     """An id representing the session the message is a part of."""
 
-    timestamp: float
+    timestamp: datetime
     """When the message was sent."""
 
     source: MessageSource
     """Indicates if the message was sent by the client or the server."""
 
     id: Optional[str]
     """The ``id`` field, if it exists."""
@@ -47,20 +50,20 @@
     """The ``result`` field, if it exists."""
 
     error: Optional[Any] = attrs.field(converter=maybe_json)
     """The ``error`` field, if it exists."""
 
     @classmethod
     def from_rpc(
-        cls, session: str, timestamp: float, source: str, message: Mapping[str, Any]
+        cls, session: str, timestamp: str, source: str, message: Mapping[str, Any]
     ):
         """Create an instance from a JSON-RPC message."""
         return cls(
             session=session,
-            timestamp=timestamp,
+            timestamp=datetime.fromisoformat(timestamp),
             source=source,  # type: ignore
             id=message.get("id", None),
             method=message.get("method", None),
             params=message.get("params", None),
             result=message.get("result", None),
             error=message.get("error", None),
         )
@@ -80,28 +83,26 @@
 
 
 class LspHandler(logging.Handler):
     """Base class for lsp log handlers."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.session_id = str(uuid4())
 
     def handle_message(self, message: LspMessage):
         """Called each time a message is processed."""
 
     def emit(self, record: logging.LogRecord):
         if not isinstance(record.args, dict):
             return
 
         message = record.args
-        timestamp = record.created
-        source = record.__dict__["source"]
+        source = record.__dict__["Message-Source"]
 
         self.handle_message(
             LspMessage.from_rpc(
-                session=self.session_id,
-                timestamp=timestamp,
+                session=record.__dict__["Message-Session"],
+                timestamp=record.__dict__["Message-Timestamp"],
                 source=source,
                 message=message,
             )
         )
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/handlers/dbinit.sql` & `lsp_devtools-0.2.3/lsp_devtools/handlers/dbinit.sql`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/lsp_devtools/handlers/sql.py` & `lsp_devtools-0.2.3/lsp_devtools/handlers/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sqlite3
 import sys
 from contextlib import closing
 
 from lsp_devtools.handlers import LspHandler
 from lsp_devtools.handlers import LspMessage
 
-if sys.version_info.minor < 9:
+if sys.version_info < (3, 9):
     import importlib_resources as resources
 else:
-    import importlib.resources as resources  # type: ignore[no-redef]
+    from importlib import resources  # type: ignore[no-redef]
 
 
 class SqlHandler(LspHandler):
     """A logging handler that sends log records to a SQL database"""
 
     def __init__(self, dbpath: pathlib.Path, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/inspector/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/inspector/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import argparse
 import asyncio
-import json
 import logging
 import pathlib
-import re
-from datetime import datetime
+from functools import partial
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 
 import platformdirs
 from rich.highlighter import ReprHighlighter
@@ -21,17 +19,16 @@
 from textual.events import Ready
 from textual.widgets import DataTable
 from textual.widgets import Footer
 from textual.widgets import Header
 from textual.widgets import Tree
 from textual.widgets.tree import TreeNode
 
-from lsp_devtools.agent import MESSAGE_TEXT_NOTIFICATION
 from lsp_devtools.agent import AgentServer
-from lsp_devtools.agent import MessageText
+from lsp_devtools.agent import parse_rpc_message
 from lsp_devtools.database import Database
 from lsp_devtools.handlers import LspMessage
 
 logger = logging.getLogger(__name__)
 
 
 class MessageViewer(Tree):
@@ -128,19 +125,15 @@
 
         query_params = self._get_query_params()
         messages = await self.db.get_messages(**query_params)
         for idx, message in messages:
             self.max_row = idx
             self.rpcdata[idx] = message
 
-            # Surely there's a more direct way to do this?
-            dt = datetime.fromtimestamp(message.timestamp)
-            time = dt.isoformat(timespec="milliseconds")
-            time = time[time.find("T") + 1 :]
-
+            time = message.timestamp[message.timestamp.find("T") + 1 :]
             self.add_row(str(idx), time, message.source, message.id, message.method)
 
         self.move_cursor(row=self.row_count, animate=True)
 
 
 class Sidebar(Container):
     pass
@@ -197,72 +190,38 @@
 
     @on(Database.Update)
     async def update_table(self, event: Database.Update):
         table = self.query_one(MessagesTable)
         await table.update()
 
     async def action_quit(self):
-        await self.server.stop()
+        self.server.stop()
         await self.db.close()
         await super().action_quit()
 
 
-MESSAGE_PATTERN = re.compile(
-    r"^(?:[^\r\n]+\r\n)*"
-    + r"Content-Length: (?P<length>\d+)\r\n"
-    + r"(?:[^\r\n]+\r\n)*\r\n"
-    + r"(?P<body>{.*)",
-    re.DOTALL,
-)
-
-
-async def handle_message(ls: AgentServer, message: MessageText):
+async def handle_message(db: Database, data: bytes):
     """Handle messages received from the connected lsp server."""
 
-    data = message.text
-    message_buf = ls._client_buffer if message.source == "client" else ls._server_buffer
-
-    while len(data):
-        # Append the incoming chunk to the message buffer
-        message_buf.append(data)
-
-        # Look for the body of the message
-        msg = "".join(message_buf)
-        found = MESSAGE_PATTERN.fullmatch(msg)
-
-        body = found.group("body") if found else ""
-        length = int(found.group("length")) if found else 1
-
-        if len(body) < length:
-            # Message is incomplete; bail until more data arrives
-            return
+    try:
+        rpc = parse_rpc_message(data)
+    except ValueError:
+        # TODO: error reporting
+        return
+
+    session = rpc["Message-Session"]
+    timestamp = rpc["Message-Timestamp"]
+    source = rpc["Message-Source"]
 
-        # Message is complete;
-        # extract the body and any remaining data,
-        # and reset the buffer for the next message
-        body, data = body[:length], body[length:]
-        message_buf.clear()
-
-        rpc = json.loads(body)
-        if ls.db is not None:
-            await ls.db.add_message(
-                message.session, message.timestamp, message.source, rpc
-            )
-
-
-def setup_server(db: Database):
-    server = AgentServer()
-    server.db = db
-    server.feature(MESSAGE_TEXT_NOTIFICATION)(handle_message)
-    return server
+    await db.add_message(session, timestamp, source, rpc.body)
 
 
 def inspector(args, extra: List[str]):
     db = Database(args.dbpath)
-    server = setup_server(db)
+    server = AgentServer(handler=partial(handle_message, db))
 
     app = LSPInspector(db, server)
     app.run()
 
 
 def cli(commands: argparse._SubParsersAction):
     cmd: argparse.ArgumentParser = commands.add_parser(
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/record/__init__.py` & `lsp_devtools-0.2.3/lsp_devtools/record/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,29 +9,26 @@
 from typing import Optional
 
 from rich.console import Console
 from rich.console import ConsoleRenderable
 from rich.logging import RichHandler
 from rich.traceback import Traceback
 
-from lsp_devtools.agent import MESSAGE_TEXT_NOTIFICATION
 from lsp_devtools.agent import AgentServer
-from lsp_devtools.agent import MessageText
 from lsp_devtools.agent import parse_rpc_message
 from lsp_devtools.handlers.sql import SqlHandler
 
 from .filters import LSPFilter
 from .visualize import SpinnerHandler
 
 EXPORTERS = {
     ".html": ("save_html", {}),
     ".svg": ("save_svg", {"title": ""}),
     ".txt": ("save_text", {}),
 }
-logger = logging.getLogger(__name__)
 
 
 class RichLSPHandler(RichHandler):
     def __init__(self, level: int, log_time_format="%X", **kwargs):
         super().__init__(
             level=level,
             show_path=False,
@@ -49,38 +46,40 @@
     ) -> "ConsoleRenderable":
         # Delegate most of the rendering to the base RichHandler class.
         res = super().render(
             record=record, traceback=traceback, message_renderable=message_renderable
         )
 
         # Abuse the log level column to display the source of the message,
-        source = record.__dict__["source"]
+        source = record.__dict__["Message-Source"]
         color = "red" if source == "client" else "blue"
         message_source = f"[bold][{color}]{source.upper()}[/{color}][/bold]"
         res.columns[1]._cells[0] = message_source  # type: ignore
 
         return res
 
     def format(self, record: LogRecord) -> str:
         # Pretty print json messages
         if isinstance(record.args, dict):
             record.args = (json.dumps(record.args, indent=2),)
         return super().format(record)
 
 
-def log_raw_message(ls: AgentServer, message: MessageText):
-    """Push raw messages through the logging system."""
-    logger.info(message.text, extra={"source": message.source})
+def setup_logging(logger: logging.Logger, console: Console):
+    """Setup logging of messages from other loggers."""
 
+    # Suppress pygls logging
+    pygls_logger = logging.getLogger("pygls")
+    pygls_logger.setLevel(logging.CRITICAL)
 
-def log_rpc_message(ls: AgentServer, message: MessageText):
-    """Push parsed json-rpc messages through the logging system"""
+    handler = RichHandler(console=console)
+    handler.setLevel(logging.ERROR)
 
-    logfn = partial(logger.info, "%s", extra={"source": message.source})
-    parse_rpc_message(ls, message, logfn)
+    logger.setLevel(logging.ERROR)
+    logger.addHandler(handler)
 
 
 def setup_stdout_output(args, logger: logging.Logger, console: Console):
     """Log messages to stdout."""
 
     handler = RichLSPHandler(level=logging.INFO, console=console)
     handler.addFilter(
@@ -91,14 +90,15 @@
             include_methods=args.include_methods,
             exclude_methods=args.exclude_methods,
             formatter=args.format_message or "{.|json}",
         )
     )
 
     logger.addHandler(handler)
+    logger.propagate = False
 
 
 def setup_file_output(args, logger: logging.Logger, console: Optional[Console] = None):
     """Log messages to a file."""
     handler = logging.FileHandler(filename=str(args.to_file))
     handler.setLevel(logging.INFO)
     handler.addFilter(
@@ -115,14 +115,15 @@
     if console:
         spinner = SpinnerHandler(console)
         spinner.setLevel(logging.INFO)
         logger.addHandler(spinner)
 
     # This must come last!
     logger.addHandler(handler)
+    logger.propagate = False
 
 
 def setup_sqlite_output(
     args, logger: logging.Logger, console: Optional[Console] = None
 ):
     """Log messages to SQLite."""
     handler = SqlHandler(args.to_sqlite)
@@ -140,32 +141,47 @@
     if console:
         spinner = SpinnerHandler(console)
         spinner.setLevel(logging.INFO)
         logger.addHandler(spinner)
 
     # This must come last!
     logger.addHandler(handler)
+    logger.propagate = False
+
+
+def log_message(logger: logging.Logger, message: bytes):
+    try:
+        rpc = parse_rpc_message(message)
+    except ValueError:
+        # TODO: report the error.
+        return
+
+    logger.info("%s", rpc.body, extra=rpc.headers)
 
 
 def start_recording(args, extra: List[str]):
-    server = AgentServer()
-    log_func = log_raw_message if args.capture_raw_output else log_rpc_message
-    logger.setLevel(logging.INFO)
-    server.feature(MESSAGE_TEXT_NOTIFICATION)(log_func)
+    logger = logging.getLogger("lsp_devtools")
+
+    rpc_logger = logging.getLogger(__name__)
+    rpc_logger.setLevel(logging.INFO)
+
+    handler = partial(log_message, rpc_logger)
+    server = AgentServer(logger=logger, handler=handler)
 
     console = Console(record=args.save_output is not None)
+    setup_logging(logger, console)
 
     if args.to_file:
-        setup_file_output(args, logger, console)
+        setup_file_output(args, rpc_logger, console)
 
     elif args.to_sqlite:
-        setup_sqlite_output(args, logger, console)
+        setup_sqlite_output(args, rpc_logger, console)
 
     else:
-        setup_stdout_output(args, logger, console)
+        setup_stdout_output(args, rpc_logger, console)
 
     try:
         host = args.host
         port = args.port
 
         print(f"Waiting for connection on {host}:{port}...", end="\r", flush=True)
         asyncio.run(server.start_tcp(host, port))
@@ -187,52 +203,52 @@
             exporter = getattr(console, exporter_name)
             exporter(str(destination), **kwargs)
 
 
 def setup_filter_args(cmd: argparse.ArgumentParser):
     """Add arguments that can be used to filter messages."""
 
-    filter = cmd.add_argument_group(
+    filter_ = cmd.add_argument_group(
         title="filter options",
         description=(
             "select which messages to record, mutliple options will be ANDed together. "
             "Does not apply to raw message capture"
         ),
     )
-    filter.add_argument(
+    filter_.add_argument(
         "--message-source",
         default="both",
         choices=["client", "server", "both"],
         help="only include messages from the given source",
     )
-    filter.add_argument(
+    filter_.add_argument(
         "--include-message-type",
         action="append",
         default=[],
         dest="include_message_types",
         choices=["request", "response", "result", "error", "notification"],
         help="only include the given message type(s)",
     )
-    filter.add_argument(
+    filter_.add_argument(
         "--exclude-message-type",
         action="append",
         dest="exclude_message_types",
         default=[],
         choices=["request", "response", "result", "error", "notification"],
         help="omit the given message type(s)",
     )
-    filter.add_argument(
+    filter_.add_argument(
         "--include-method",
         action="append",
         dest="include_methods",
         default=[],
         metavar="METHOD",
         help="only include the given messages for the given method(s)",
     )
-    filter.add_argument(
+    filter_.add_argument(
         "--exclude-method",
         action="append",
         dest="exclude_methods",
         default=[],
         metavar="METHOD",
         help="omit messages for the given method(s)",
     )
@@ -271,22 +287,22 @@
         "--capture-rpc-output",
         default=True,
         action="store_true",
         help="capture the rpc messages sent between client and server.",
     )
 
     setup_filter_args(cmd)
-    format = cmd.add_argument_group(
+    format_ = cmd.add_argument_group(
         title="formatting options",
         description=(
             "control how the recorded messages are formatted "
             "(does not apply to SQLite output or raw message capture)"
         ),
     )
-    format.add_argument(
+    format_.add_argument(
         "-f",
         "--format-message",
         default=None,
         help=(
             "format messages according to given format string, "
             "see example commands above for syntax. "
             "Messages which fail to format will be excluded"
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/record/filters.py` & `lsp_devtools-0.2.3/lsp_devtools/record/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,19 @@
     """Used to determine the method for response messages"""
 
     def filter(self, record: logging.LogRecord) -> bool:
         message = record.args
         if not isinstance(message, dict):
             return False
 
-        source = record.__dict__["source"]
+        source = record.__dict__["Message-Source"]
         message_type = get_message_type(message)
         message_method = self._get_message_method(message_type, message)
 
-        if self.message_source != "both" and source != self.message_source:
+        if self.message_source not in {"both", source}:
             return False
 
         if self.include_message_types and not message_matches_type(
             message_type, self.include_message_types
         ):
             return False
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/record/formatters.py` & `lsp_devtools-0.2.3/lsp_devtools/record/formatters.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
                 obj = obj[match.group(1)]
                 remainder = accessor[idx + 1 :]
                 sep, index = get_separator_index(match.group(2))
 
                 if isinstance(index, int):
                     obj = obj[index]
                     continue
-                elif isinstance(index, slice):
+
+                if isinstance(index, slice):
                     obj = obj[index]
 
                 return sep.join([self.format(o, remainder) for o in obj])
 
             obj = obj[field]
 
         return self.formatter(obj)
```

### Comparing `lsp_devtools-0.2.2/lsp_devtools/record/visualize.py` & `lsp_devtools-0.2.3/lsp_devtools/record/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
         if not isinstance(message, dict):
             return
 
         self.progress.start()
 
         method = message.get("method", None)
-        source = record.__dict__["source"]
+        source = record.__dict__["Message-Source"]
         args = {}
 
         if method:
             args[f"{source}_method"] = method
             count = getattr(self, f"{source}_count") + 1
 
             setattr(self, f"{source}_count", count)
```

### Comparing `lsp_devtools-0.2.2/tests/test_agent.py` & `lsp_devtools-0.2.3/tests/test_agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,19 @@
             "\r\n",
             f"{content}",
         ]
     )
     return message.encode()
 
 
+def echo_handler(d: bytes):
+    sys.stdout.buffer.write(d)
+    sys.stdout.flush()
+
+
 @pytest.mark.asyncio
 async def test_agent_exits():
     """Ensure that when the client closes down the lsp session and the server process
     exits, the agent does also."""
 
     (stdin_read, stdin_write) = os.pipe()
     (stdout_read, stdout_write) = os.pipe()
@@ -40,14 +45,15 @@
         stderr=subprocess.PIPE,
     )
 
     agent = Agent(
         server,
         os.fdopen(stdin_read, mode="rb"),
         os.fdopen(stdout_write, mode="wb"),
+        echo_handler,
     )
 
     os.write(
         stdin_write,
         format_message(
             dict(jsonrpc="2.0", id=1, method="initialize", params=dict(capabilities={}))
         ),
@@ -71,11 +77,10 @@
         )
     except asyncio.CancelledError:
         pass  # The agent's tasks should be cancelled
 
     except TimeoutError as exc:
         # Make sure this timed out for the right reason.
         if server.returncode is None:
-            raise RuntimeError("Server process did not exit")
-        else:
-            exc.add_note("lsp-devtools agent did not stop")
-            raise
+            raise RuntimeError("Server process did not exit") from exc
+
+        exc.add_note("lsp-devtools agent did not stop")
```

### Comparing `lsp_devtools-0.2.2/tests/record/test_filters.py` & `lsp_devtools-0.2.3/tests/record/test_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 def test_filter_message_source(filter_source: str, message_source: str, expected: bool):
     """Ensure that we can filter messages by their source correctly."""
 
     lsp = LSPFilter(message_source=filter_source)
     message = dict(id="1", method="initialize", params={})
 
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", message, None)
-    record.__dict__["source"] = message_source
+    record.__dict__["Message-Source"] = message_source
 
     assert lsp.filter(record) is expected
 
 
 @pytest.mark.parametrize(
     "message,setup",
     [
@@ -92,15 +92,15 @@
     ],
 )
 def test_filter_included_message_types(message: dict, setup: Tuple[List[str], bool]):
     """Ensure that we can filter messages by listing the types we DO want to see."""
 
     message_types, expected = setup
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", message, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp = LSPFilter(include_message_types=message_types)
     lsp._response_method_map["1"] = ""
 
     assert lsp.filter(record) is expected
 
 
@@ -165,15 +165,15 @@
     ],
 )
 def test_filter_excluded_message_types(message: dict, setup: Tuple[List[str], bool]):
     """Ensure that we can filter messages by listing the types we DO NOT want to see."""
 
     message_types, expected = setup
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", message, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp = LSPFilter(exclude_message_types=message_types)
     lsp._response_method_map["1"] = ""
 
     assert lsp.filter(record) is expected
 
 
@@ -203,15 +203,15 @@
     ],
 )
 def test_filter_included_method(message: dict, setup: Tuple[List[str], bool]):
     """Ensure that we can filter messages by listing the methods we wish to see."""
 
     methods, expected = setup
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", message, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp = LSPFilter(include_methods=methods)
     assert lsp.filter(record) is expected
 
 
 @pytest.mark.parametrize(
     "response,setup",
@@ -253,20 +253,20 @@
     to see."""
 
     methods, method, expected = setup
     lsp = LSPFilter(include_methods=methods)
 
     request = dict(id="1", method=method, params={})
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", request, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp.filter(record)
 
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", response, None)
-    record.__dict__["source"] = "server"
+    record.__dict__["Message-Source"] = "server"
 
     assert lsp.filter(record) is expected
 
 
 @pytest.mark.parametrize(
     "message,setup",
     [
@@ -294,15 +294,15 @@
 )
 def test_filter_excluded_method(message: dict, setup: Tuple[List[str], bool]):
     """Ensure that we can filter messages by listing the methods we don't wish to
     see."""
 
     methods, expected = setup
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", message, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp = LSPFilter(exclude_methods=methods)
     assert lsp.filter(record) is expected
 
 
 @pytest.mark.parametrize(
     "response,setup",
@@ -344,32 +344,32 @@
     to see."""
 
     methods, method, expected = setup
     lsp = LSPFilter(exclude_methods=methods)
 
     request = dict(id="1", method=method, params={})
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", request, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp.filter(record)
 
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", response, None)
-    record.__dict__["source"] = "server"
+    record.__dict__["Message-Source"] = "server"
 
     assert lsp.filter(record) is expected
 
 
 def test_filter_skip_unformattable_message():
     """Ensure that if a message cannot be formatted it is skipped."""
 
     lsp = LSPFilter(formatter="{.xxx}")
 
     request = dict(id="1", method="textDocument/completion", params={})
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", request, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     lsp.filter(record)
     assert lsp.filter(record) is False
 
 
 def test_filter_format_message():
     """Ensure that we can format a message according to some string."""
@@ -378,11 +378,11 @@
 
     request = dict(
         id="1",
         method="textDocument/completion",
         params=dict(textDocument=dict(uri="file:///path/to/file.txt")),
     )
     record = logging.LogRecord("example", logging.INFO, "", 0, "%s", request, None)
-    record.__dict__["source"] = "client"
+    record.__dict__["Message-Source"] = "client"
 
     assert lsp.filter(record) is True
     assert record.msg == "file:///path/to/file.txt"
```

### Comparing `lsp_devtools-0.2.2/tests/record/test_formatters.py` & `lsp_devtools-0.2.3/tests/record/test_formatters.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             {
                 "method": "textDocument/completion",
                 "params": {
                     "position": {"line": 1, "character": 2},
                     "textDocument": {"uri": "file:///path/to/file.txt"},
                 },
             },
-            'textDocument/completion file:///path/to/file.txt:{\n  "line": 1,\n  "character": 2\n}',  # noqa: E501
+            'textDocument/completion file:///path/to/file.txt:{\n  "line": 1,\n  "character": 2\n}',
         ),
         (
             "{.method} {.params.textDocument.uri}:{.params.position|Position}",
             {
                 "method": "textDocument/completion",
                 "params": {
                     "position": {"line": 1, "character": 2},
```

### Comparing `lsp_devtools-0.2.2/tests/record/test_record.py` & `lsp_devtools-0.2.3/tests/record/test_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     parser = argparse.ArgumentParser(description="for testing purposes")
     commands = parser.add_subparsers()
     cli(commands)
 
     return parser
 
 
-@pytest.fixture()
+@pytest.fixture
 def logger():
     """Return the logger instance to use."""
 
     log = logging.getLogger(__name__)
     log.setLevel(logging.INFO)
 
     for handler in log.handlers:
@@ -114,10 +114,10 @@
     """
     log = tmp_path / "log.json"
     parsed_args = record.parse_args(["record", "--to-file", str(log), *args])
 
     setup_file_output(parsed_args, logger)
 
     for message in messages:
-        logger.info("%s", message, extra={"source": "client"})
+        logger.info("%s", message, extra={"Message-Source": "client"})
 
     assert log.read_text() == expected
```

### Comparing `lsp_devtools-0.2.2/LICENSE` & `lsp_devtools-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/README.md` & `lsp_devtools-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `lsp_devtools-0.2.2/pyproject.toml` & `lsp_devtools-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,32 +30,28 @@
   "stamina",
   "textual>=0.41.0",
   "typing-extensions; python_version<\"3.8\"",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/swyddfa/lsp-devtools/issues"
-"Documentation" = "https://swyddfa.github.io/lsp-devtools/"
+"Documentation" = "https://lsp-devtools.readthedocs.io/en/latest/"
 "Source Code" = "https://github.com/swyddfa/lsp-devtools"
 
 [project.scripts]
 lsp-devtools = "lsp_devtools.cli:main"
 
 [tool.coverage.run]
 source_pkgs = ["lsp_devtools"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 sort = "Cover"
 
-[tool.isort]
-force_single_line = true
-profile = "black"
-
 [tool.pyright]
 venv = ".env"
 include = ["lsp_devtools"]
 pythonVersion = "3.8"
 
 [tool.towncrier]
 filename = "CHANGES.md"
```

### Comparing `lsp_devtools-0.2.2/PKG-INFO` & `lsp_devtools-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lsp-devtools
-Version: 0.2.2
+Version: 0.2.3
 Summary: Developer tooling for language servers
 Project-URL: Bug Tracker, https://github.com/swyddfa/lsp-devtools/issues
-Project-URL: Documentation, https://swyddfa.github.io/lsp-devtools/
+Project-URL: Documentation, https://lsp-devtools.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/swyddfa/lsp-devtools
 Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

