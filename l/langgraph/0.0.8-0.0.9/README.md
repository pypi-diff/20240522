# Comparing `tmp/langgraph-0.0.8.tar.gz` & `tmp/langgraph-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langgraph-0.0.8.tar", max compression
+gzip compressed data, was "langgraph-0.0.9.tar", max compression
```

## Comparing `langgraph-0.0.8.tar` & `langgraph-0.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     3756 2024-01-08 03:37:22.281565 langgraph-0.0.8/LICENSE
--rw-r--r--   0        0        0     5115 2024-01-08 03:38:36.789984 langgraph-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-01-08 03:30:03.961295 langgraph-0.0.8/langgraph/__init__.py
--rw-r--r--   0        0        0      294 2024-01-08 03:38:21.940373 langgraph-0.0.8/langgraph/channels/__init__.py
--rw-r--r--   0        0        0     3996 2024-01-08 03:38:21.639814 langgraph-0.0.8/langgraph/channels/base.py
--rw-r--r--   0        0        0     2004 2024-01-08 03:38:21.640176 langgraph-0.0.8/langgraph/channels/binop.py
--rw-r--r--   0        0        0     3150 2024-01-08 03:38:21.666698 langgraph-0.0.8/langgraph/channels/context.py
--rw-r--r--   0        0        0     1634 2024-01-08 03:38:21.645502 langgraph-0.0.8/langgraph/channels/last_value.py
--rw-r--r--   0        0        0     2528 2024-01-08 03:38:21.640030 langgraph-0.0.8/langgraph/channels/topic.py
--rw-r--r--   0        0        0      205 2024-01-08 03:38:21.972430 langgraph-0.0.8/langgraph/checkpoint/__init__.py
--rw-r--r--   0        0        0     1826 2024-01-08 03:38:21.954522 langgraph-0.0.8/langgraph/checkpoint/base.py
--rw-r--r--   0        0        0      985 2024-01-08 03:38:22.098508 langgraph-0.0.8/langgraph/checkpoint/memory.py
--rw-r--r--   0        0        0       68 2024-01-08 05:14:25.937390 langgraph-0.0.8/langgraph/constants.py
--rw-r--r--   0        0        0     4328 2024-01-08 03:38:21.946537 langgraph-0.0.8/langgraph/graph/__init__.py
--rw-r--r--   0        0        0    25678 2024-01-08 05:12:49.534776 langgraph-0.0.8/langgraph/pregel/__init__.py
--rw-r--r--   0        0        0     1223 2024-01-08 03:38:22.104839 langgraph-0.0.8/langgraph/pregel/debug.py
--rw-r--r--   0        0        0     1409 2024-01-08 03:38:22.252067 langgraph-0.0.8/langgraph/pregel/io.py
--rw-r--r--   0        0        0       53 2023-10-23 09:39:57.968323 langgraph-0.0.8/langgraph/pregel/log.py
--rw-r--r--   0        0        0     6352 2024-01-08 03:38:22.245293 langgraph-0.0.8/langgraph/pregel/read.py
--rw-r--r--   0        0        0      228 2023-11-16 12:37:15.033539 langgraph-0.0.8/langgraph/pregel/reserved.py
--rw-r--r--   0        0        0     2074 2024-01-08 03:38:22.106196 langgraph-0.0.8/langgraph/pregel/validate.py
--rw-r--r--   0        0        0     1950 2024-01-08 03:38:22.261147 langgraph-0.0.8/langgraph/pregel/write.py
--rw-r--r--   0        0        0      133 2023-11-15 14:45:38.048347 langgraph-0.0.8/langgraph/utils.py
--rw-r--r--   0        0        0     2019 2024-01-08 05:13:10.085559 langgraph-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5710 1970-01-01 00:00:00.000000 langgraph-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-01-08 15:57:35.404136 langgraph-0.0.9/LICENSE
+-rw-r--r--   0        0        0    13126 2024-01-08 15:57:35.404684 langgraph-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-08 03:30:03.961295 langgraph-0.0.9/langgraph/__init__.py
+-rw-r--r--   0        0        0      294 2024-01-08 03:38:21.940373 langgraph-0.0.9/langgraph/channels/__init__.py
+-rw-r--r--   0        0        0     3999 2024-01-08 16:19:41.977471 langgraph-0.0.9/langgraph/channels/base.py
+-rw-r--r--   0        0        0     2004 2024-01-08 03:38:21.640176 langgraph-0.0.9/langgraph/channels/binop.py
+-rw-r--r--   0        0        0     3150 2024-01-08 03:38:21.666698 langgraph-0.0.9/langgraph/channels/context.py
+-rw-r--r--   0        0        0     1634 2024-01-08 03:38:21.645502 langgraph-0.0.9/langgraph/channels/last_value.py
+-rw-r--r--   0        0        0     2560 2024-01-08 16:20:30.081641 langgraph-0.0.9/langgraph/channels/topic.py
+-rw-r--r--   0        0        0      205 2024-01-08 03:38:21.972430 langgraph-0.0.9/langgraph/checkpoint/__init__.py
+-rw-r--r--   0        0        0     1842 2024-01-08 16:18:58.069310 langgraph-0.0.9/langgraph/checkpoint/base.py
+-rw-r--r--   0        0        0     1017 2024-01-08 16:19:09.622621 langgraph-0.0.9/langgraph/checkpoint/memory.py
+-rw-r--r--   0        0        0       68 2024-01-08 05:14:25.937390 langgraph-0.0.9/langgraph/constants.py
+-rw-r--r--   0        0        0     4328 2024-01-08 03:38:21.946537 langgraph-0.0.9/langgraph/graph/__init__.py
+-rw-r--r--   0        0        0    26015 2024-01-08 16:27:24.115974 langgraph-0.0.9/langgraph/pregel/__init__.py
+-rw-r--r--   0        0        0     1223 2024-01-08 03:38:22.104839 langgraph-0.0.9/langgraph/pregel/debug.py
+-rw-r--r--   0        0        0     1461 2024-01-08 16:29:26.286688 langgraph-0.0.9/langgraph/pregel/io.py
+-rw-r--r--   0        0        0       53 2023-10-23 09:39:57.968323 langgraph-0.0.9/langgraph/pregel/log.py
+-rw-r--r--   0        0        0     6509 2024-01-08 16:23:21.361058 langgraph-0.0.9/langgraph/pregel/read.py
+-rw-r--r--   0        0        0      239 2024-01-08 15:58:08.106639 langgraph-0.0.9/langgraph/pregel/reserved.py
+-rw-r--r--   0        0        0     2099 2024-01-08 16:24:01.574418 langgraph-0.0.9/langgraph/pregel/validate.py
+-rw-r--r--   0        0        0     1966 2024-01-08 16:24:18.949007 langgraph-0.0.9/langgraph/pregel/write.py
+-rw-r--r--   0        0        0      133 2023-11-15 14:45:38.048347 langgraph-0.0.9/langgraph/utils.py
+-rw-r--r--   0        0        0     2019 2024-01-08 16:30:52.887019 langgraph-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    13721 1970-01-01 00:00:00.000000 langgraph-0.0.9/PKG-INFO
```

### Comparing `langgraph-0.0.8/langgraph/channels/base.py` & `langgraph-0.0.9/langgraph/channels/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     @abstractmethod
     def get(self) -> Value:
         """Return the current value of the channel.
 
         Raises EmptyChannelError if the channel is empty (never updated yet)."""
 
     @abstractmethod
-    def checkpoint(self) -> C | None:
+    def checkpoint(self) -> Optional[C]:
         """Return a string representation of the channel's current state.
 
         Raises EmptyChannelError if the channel is empty (never updated yet),
         or doesn't supportcheckpoints."""
 
 
 @contextmanager
```

### Comparing `langgraph-0.0.8/langgraph/channels/binop.py` & `langgraph-0.0.9/langgraph/channels/binop.py`

 * *Files identical despite different names*

### Comparing `langgraph-0.0.8/langgraph/channels/context.py` & `langgraph-0.0.9/langgraph/channels/context.py`

 * *Files identical despite different names*

### Comparing `langgraph-0.0.8/langgraph/channels/last_value.py` & `langgraph-0.0.9/langgraph/channels/last_value.py`

 * *Files identical despite different names*

### Comparing `langgraph-0.0.8/langgraph/channels/topic.py` & `langgraph-0.0.9/langgraph/channels/topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from typing import Any, Generator, Generic, Iterator, Optional, Sequence, Type, Union
 
 from typing_extensions import Self
 
 from langgraph.channels.base import BaseChannel, Value
 
 
-def flatten(values: Sequence[Value | list[Value]]) -> Iterator[Value]:
+def flatten(values: Sequence[Union[Value, list[Value]]]) -> Iterator[Value]:
     for value in values:
         if isinstance(value, list):
             yield from value
         else:
             yield value
 
 
 class Topic(
     Generic[Value],
-    BaseChannel[Sequence[Value], Value | list[Value], tuple[set[Value], list[Value]]],
+    BaseChannel[
+        Sequence[Value], Union[Value, list[Value]], tuple[set[Value], list[Value]]
+    ],
 ):
     """A configurable PubSub Topic.
 
     Args:
         typ: The type of the value stored in the channel.
         unique: Whether to discard duplicate values.
         accumulate: Whether to accummulate values across steps. If False, the channel will be emptied after each step.
@@ -56,15 +58,15 @@
             empty.seen = checkpoint[0]
             empty.values = checkpoint[1]
         try:
             yield empty
         finally:
             pass
 
-    def update(self, values: Sequence[Value | list[Value]]) -> None:
+    def update(self, values: Sequence[Union[Value, list[Value]]]) -> None:
         if not self.accumulate:
             self.values = list[Value]()
         if flat_values := flatten(values):
             if self.unique:
                 for value in flat_values:
                     if value not in self.seen:
                         self.seen.add(value)
```

### Comparing `langgraph-0.0.8/langgraph/checkpoint/base.py` & `langgraph-0.0.9/langgraph/checkpoint/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from datetime import datetime, timezone
-from typing import Any, TypedDict
+from typing import Any, Optional, TypedDict
 
 from langchain_core.load.serializable import Serializable
 from langchain_core.pydantic_v1 import Field
 from langchain_core.runnables import RunnableConfig
 from langchain_core.runnables.utils import ConfigurableFieldSpec
 
 from langgraph.utils import StrEnum
@@ -39,22 +39,22 @@
     at: CheckpointAt = CheckpointAt.END_OF_RUN
 
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
         return []
 
     @abstractmethod
-    def get(self, config: RunnableConfig) -> Checkpoint | None:
+    def get(self, config: RunnableConfig) -> Optional[Checkpoint]:
         ...
 
     @abstractmethod
     def put(self, config: RunnableConfig, checkpoint: Checkpoint) -> None:
         ...
 
-    async def aget(self, config: RunnableConfig) -> Checkpoint | None:
+    async def aget(self, config: RunnableConfig) -> Optional[Checkpoint]:
         return await asyncio.get_running_loop().run_in_executor(None, self.get, config)
 
     async def aput(self, config: RunnableConfig, checkpoint: Checkpoint) -> None:
         return await asyncio.get_running_loop().run_in_executor(
             None, self.put, config, checkpoint
         )
```

### Comparing `langgraph-0.0.8/langgraph/checkpoint/memory.py` & `langgraph-0.0.9/langgraph/checkpoint/memory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from langchain_core.pydantic_v1 import Field
 from langchain_core.runnables import RunnableConfig
 from langchain_core.runnables.utils import ConfigurableFieldSpec
 
 from langgraph.checkpoint.base import BaseCheckpointSaver, Checkpoint
 
 
@@ -17,12 +19,12 @@
                 name="Thread ID",
                 description=None,
                 default="",
                 is_shared=True,
             ),
         ]
 
-    def get(self, config: RunnableConfig) -> Checkpoint | None:
+    def get(self, config: RunnableConfig) -> Optional[Checkpoint]:
         return self.storage.get(config["configurable"]["thread_id"], None)
 
     def put(self, config: RunnableConfig, checkpoint: Checkpoint) -> None:
         return self.storage.update({config["configurable"]["thread_id"]: checkpoint})
```

### Comparing `langgraph-0.0.8/langgraph/graph/__init__.py` & `langgraph-0.0.9/langgraph/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `langgraph-0.0.8/langgraph/pregel/__init__.py` & `langgraph-0.0.9/langgraph/pregel/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,44 +82,44 @@
 class Channel:
     @overload
     @classmethod
     def subscribe_to(
         cls,
         channels: str,
         key: Optional[str] = None,
-        when: Callable[[Any], bool] | None = None,
+        when: Optional[Callable[[Any], bool]] = None,
     ) -> ChannelInvoke:
         ...
 
     @overload
     @classmethod
     def subscribe_to(
         cls,
         channels: Sequence[str],
         key: None = None,
-        when: Callable[[Any], bool] | None = None,
+        when: Optional[Callable[[Any], bool]] = None,
     ) -> ChannelInvoke:
         ...
 
     @classmethod
     def subscribe_to(
         cls,
-        channels: str | Sequence[str],
+        channels: Union[str, Sequence[str]],
         key: Optional[str] = None,
-        when: Callable[[Any], bool] | None = None,
+        when: Optional[Callable[[Any], bool]] = None,
     ) -> ChannelInvoke:
         """Runs process.invoke() each time channels are updated,
         with a dict of the channel values as input."""
         if not isinstance(channels, str) and key is not None:
             raise ValueError(
                 "Can't specify a key when subscribing to multiple channels"
             )
         return ChannelInvoke(
             channels=cast(
-                Mapping[None, str] | Mapping[str, str],
+                Union[Mapping[None, str], Mapping[str, str]],
                 {key: channels}
                 if isinstance(channels, str)
                 else {chan: chan for chan in channels},
             ),
             triggers=[channels] if isinstance(channels, str) else channels,
             when=when,
         )
@@ -140,22 +140,24 @@
             channels=(
                 [(c, None) for c in channels]
                 + [(k, _coerce_write_value(v)) for k, v in kwargs.items()]
             )
         )
 
 
-class Pregel(RunnableSerializable[dict[str, Any] | Any, dict[str, Any] | Any]):
-    nodes: Mapping[str, ChannelInvoke | ChannelBatch]
+class Pregel(
+    RunnableSerializable[Union[dict[str, Any], Any], Union[dict[str, Any], Any]]
+):
+    nodes: Mapping[str, Union[ChannelInvoke, ChannelBatch]]
 
     channels: Mapping[str, BaseChannel] = Field(default_factory=dict)
 
-    output: str | Sequence[str] = "output"
+    output: Union[str, Sequence[str]] = "output"
 
-    input: str | Sequence[str] = "input"
+    input: Union[str, Sequence[str]] = "input"
 
     step_timeout: Optional[float] = None
 
     debug: bool = Field(default_factory=get_debug)
 
     saver: Optional[BaseCheckpointSaver] = None
 
@@ -209,20 +211,20 @@
             return create_model(  # type: ignore[call-overload]
                 "PregelOutput",
                 **{k: (self.channels[k].ValueType, None) for k in self.output},
             )
 
     def _transform(
         self,
-        input: Iterator[dict[str, Any] | Any],
+        input: Iterator[Union[dict[str, Any], Any]],
         run_manager: CallbackManagerForChainRun,
         config: RunnableConfig,
         *,
-        output: str | Sequence[str] | None = None,
-    ) -> Iterator[tuple[dict[str, Any] | Any, CheckpointView]]:
+        output: Optional[Union[str, Sequence[str]]] = None,
+    ) -> Iterator[tuple[Union[dict[str, Any], Any], CheckpointView]]:
         if config["recursion_limit"] < 1:
             raise ValueError("recursion_limit must be at least 1")
         # assign defaults
         output = output if output is not None else [chan for chan in self.channels]
         # copy nodes to ignore mutations during execution
         processes = {**self.nodes}
         # get checkpoint from saver, or create an empty one
@@ -317,20 +319,20 @@
             # save end of run checkpoint
             if self.saver is not None and self.saver.at == CheckpointAt.END_OF_RUN:
                 checkpoint = create_checkpoint(checkpoint, channels)
                 self.saver.put(config, checkpoint)
 
     async def _atransform(
         self,
-        input: AsyncIterator[dict[str, Any] | Any],
+        input: AsyncIterator[Union[dict[str, Any], Any]],
         run_manager: AsyncCallbackManagerForChainRun,
         config: RunnableConfig,
         *,
-        output: str | Sequence[str] | None = None,
-    ) -> AsyncIterator[tuple[dict[str, Any] | Any, CheckpointView]]:
+        output: Optional[Union[str, Sequence[str]]] = None,
+    ) -> AsyncIterator[tuple[Union[dict[str, Any], Any], CheckpointView]]:
         if config["recursion_limit"] < 1:
             raise ValueError("recursion_limit must be at least 1")
         # if running from astream_log() run each proc with streaming
         do_stream = next(
             (
                 h
                 for h in run_manager.handlers
@@ -437,135 +439,135 @@
             # save end of run checkpoint
             if self.saver is not None and self.saver.at == CheckpointAt.END_OF_RUN:
                 checkpoint = create_checkpoint(checkpoint, channels)
                 await self.saver.aput(config, checkpoint)
 
     def invoke(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> dict[str, Any] | Any:
-        latest: dict[str, Any] | Any = None
+    ) -> Union[dict[str, Any], Any]:
+        latest: Union[dict[str, Any], Any] = None
         for chunk in self.stream(
             input,
             config,
             output=output if output is not None else self.output,
             **kwargs,
         ):
             latest = chunk
         return latest
 
     def stream(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> Iterator[dict[str, Any] | Any]:
+    ) -> Iterator[Union[dict[str, Any], Any]]:
         return self.transform(iter([input]), config, output=output, **kwargs)
 
     def transform(
         self,
-        input: Iterator[dict[str, Any] | Any],
-        config: RunnableConfig | None = None,
+        input: Iterator[Union[dict[str, Any], Any]],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
-        **kwargs: Any | None,
-    ) -> Iterator[dict[str, Any] | Any]:
+        output: Optional[Union[str, Sequence[str]]] = None,
+        **kwargs: Any,
+    ) -> Iterator[Union[dict[str, Any], Any]]:
         for out, _ in self._transform_stream_with_config(
             input, self._transform, config, output=output, **kwargs
         ):
             if out is not None:
-                yield cast(dict[str, Any] | Any, out)
+                yield cast(Union[dict[str, Any], Any], out)
 
     def step(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> Iterator[tuple[dict[str, Any] | Any, CheckpointView]]:
+    ) -> Iterator[tuple[Union[dict[str, Any], Any], CheckpointView]]:
         for tup in self._transform_stream_with_config(
             iter([input]), self._transform, config, output=output, **kwargs
         ):
-            yield cast(tuple[dict[str, Any] | Any, CheckpointView], tup)
+            yield cast(tuple[Union[dict[str, Any], Any], CheckpointView], tup)
 
     async def ainvoke(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> dict[str, Any] | Any:
-        latest: dict[str, Any] | Any = None
+    ) -> Union[dict[str, Any], Any]:
+        latest: Union[dict[str, Any], Any] = None
         async for chunk in self.astream(
             input,
             config,
             output=output if output is not None else self.output,
             **kwargs,
         ):
             latest = chunk
         return latest
 
     async def astream(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> AsyncIterator[dict[str, Any] | Any]:
-        async def input_stream() -> AsyncIterator[dict[str, Any] | Any]:
+    ) -> AsyncIterator[Union[dict[str, Any], Any]]:
+        async def input_stream() -> AsyncIterator[Union[dict[str, Any], Any]]:
             yield input
 
         async for chunk in self.atransform(
             input_stream(), config, output=output, **kwargs
         ):
             yield chunk
 
     async def atransform(
         self,
-        input: AsyncIterator[dict[str, Any] | Any],
-        config: RunnableConfig | None = None,
+        input: AsyncIterator[Union[dict[str, Any], Any]],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
-        **kwargs: Any | None,
-    ) -> AsyncIterator[dict[str, Any] | Any]:
+        output: Optional[Union[str, Sequence[str]]] = None,
+        **kwargs: Any,
+    ) -> AsyncIterator[Union[dict[str, Any], Any]]:
         async for out, _ in self._atransform_stream_with_config(
             input, self._atransform, config, output=output, **kwargs
         ):
             if out is not None:
                 yield out
 
     async def astep(
         self,
-        input: dict[str, Any] | Any,
-        config: RunnableConfig | None = None,
+        input: Union[dict[str, Any], Any],
+        config: Optional[RunnableConfig] = None,
         *,
-        output: str | Sequence[str] | None = None,
+        output: Optional[Union[str, Sequence[str]]] = None,
         **kwargs: Any,
-    ) -> AsyncIterator[tuple[dict[str, Any] | Any, CheckpointView]]:
-        async def input_stream() -> AsyncIterator[dict[str, Any] | Any]:
+    ) -> AsyncIterator[tuple[Union[dict[str, Any], Any], CheckpointView]]:
+        async def input_stream() -> AsyncIterator[Union[dict[str, Any], Any]]:
             yield input
 
         async for tup in self._atransform_stream_with_config(
             input_stream(), self._atransform, config, output=output, **kwargs
         ):
-            yield cast(tuple[dict[str, Any] | Any, CheckpointView], tup)
+            yield cast(tuple[Union[dict[str, Any], Any], CheckpointView], tup)
 
 
 def _interrupt_or_proceed(
-    done: set[concurrent.futures.Future[Any]] | set[asyncio.Task[Any]],
-    inflight: set[concurrent.futures.Future[Any]] | set[asyncio.Task[Any]],
+    done: Union[set[concurrent.futures.Future[Any]], set[asyncio.Task[Any]]],
+    inflight: Union[set[concurrent.futures.Future[Any]], set[asyncio.Task[Any]]],
     step: int,
 ) -> None:
     while done:
         # if any task failed
         if exc := done.pop().exception():
             # cancel all pending tasks
             while inflight:
@@ -641,15 +643,15 @@
         )
         checkpoint["channel_versions"][chan] += 1
         channels[chan].update([view.values[chan]])
 
 
 def _prepare_next_tasks(
     checkpoint: Checkpoint,
-    processes: Mapping[str, ChannelInvoke | ChannelBatch],
+    processes: Mapping[str, Union[ChannelInvoke, ChannelBatch]],
     channels: Mapping[str, BaseChannel],
 ) -> list[tuple[Runnable, Any, str]]:
     tasks: list[tuple[Runnable, Any, str]] = []
     # Check if any processes should be run in next step
     # If so, prepare the values to be passed to them
     for name, proc in processes.items():
         seen = checkpoint["versions_seen"][name]
```

### Comparing `langgraph-0.0.8/langgraph/pregel/debug.py` & `langgraph-0.0.9/langgraph/pregel/debug.py`

 * *Files identical despite different names*

### Comparing `langgraph-0.0.8/langgraph/pregel/io.py` & `langgraph-0.0.9/langgraph/pregel/io.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import Any, Iterator, Mapping, Sequence
+from typing import Any, Iterator, Mapping, Optional, Sequence, Union
 
 from langgraph.channels.base import BaseChannel
 from langgraph.pregel.log import logger
 
 
 def map_input(
-    input_channels: str | Sequence[str], chunk: dict[str, Any] | Any | None
+    input_channels: Union[str, Sequence[str]],
+    chunk: Optional[Union[dict[str, Any], Any]],
 ) -> Iterator[tuple[str, Any]]:
     """Map input chunk to a sequence of pending writes in the form (channel, value)."""
     if chunk is None:
         return
     elif isinstance(input_channels, str):
         yield (input_channels, chunk)
     else:
@@ -19,18 +20,18 @@
             if k in input_channels:
                 yield (k, chunk[k])
             else:
                 logger.warning(f"Input channel {k} not found in {input_channels}")
 
 
 def map_output(
-    output_channels: str | Sequence[str],
+    output_channels: Union[str, Sequence[str]],
     pending_writes: Sequence[tuple[str, Any]],
     channels: Mapping[str, BaseChannel],
-) -> dict[str, Any] | Any | None:
+) -> Optional[Union[dict[str, Any], Any]]:
     """Map pending writes (a sequence of tuples (channel, value)) to output chunk."""
     if isinstance(output_channels, str):
         if any(chan == output_channels for chan, _ in pending_writes):
             return channels[output_channels].get()
     else:
         if updated := {c for c, _ in pending_writes if c in output_channels}:
             return {chan: channels[chan].get() for chan in updated}
```

### Comparing `langgraph-0.0.8/langgraph/pregel/read.py` & `langgraph-0.0.9/langgraph/pregel/read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any, Callable, List, Mapping, Optional, Sequence
+from typing import Any, Callable, Mapping, Optional, Sequence, Union
 
 from langchain_core.pydantic_v1 import Field
 from langchain_core.runnables import (
     Runnable,
     RunnableConfig,
     RunnableLambda,
     RunnablePassthrough,
@@ -63,17 +63,17 @@
         return read(self.channel)
 
 
 default_bound: RunnablePassthrough = RunnablePassthrough()
 
 
 class ChannelInvoke(RunnableBindingBase):
-    channels: Mapping[None, str] | Mapping[str, str]
+    channels: Union[Mapping[None, str], Mapping[str, str]]
 
-    triggers: List[str] = Field(default_factory=list)
+    triggers: list[str] = Field(default_factory=list)
 
     when: Optional[Callable[[Any], bool]] = None
 
     bound: Runnable[Any, Any] = Field(default=default_bound)
 
     kwargs: Mapping[str, Any] = Field(default_factory=dict)
 
@@ -115,17 +115,19 @@
             bound=self.bound,
             kwargs=self.kwargs,
             config=self.config,
         )
 
     def __or__(
         self,
-        other: Runnable[Any, Other]
-        | Callable[[Any], Other]
-        | Mapping[str, Runnable[Any, Other] | Callable[[Any], Other]],
+        other: Union[
+            Runnable[Any, Other],
+            Callable[[Any], Other],
+            Mapping[str, Runnable[Any, Other] | Callable[[Any], Other]],
+        ],
     ) -> ChannelInvoke:
         if self.bound is default_bound:
             return ChannelInvoke(
                 channels=self.channels,
                 triggers=self.triggers,
                 when=self.when,
                 bound=coerce_to_runnable(other),
@@ -141,17 +143,19 @@
                 bound=self.bound | other,
                 kwargs=self.kwargs,
                 config=self.config,
             )
 
     def __ror__(
         self,
-        other: Runnable[Other, Any]
-        | Callable[[Any], Other]
-        | Mapping[str, Runnable[Other, Any] | Callable[[Other], Any]],
+        other: Union[
+            Runnable[Other, Any],
+            Callable[[Any], Other],
+            Mapping[str, Union[Runnable[Other, Any], Callable[[Other], Any]]],
+        ],
     ) -> RunnableSerializable:
         raise NotImplementedError()
 
 
 class ChannelBatch(RunnableEach):
     channel: str
 
@@ -174,28 +178,32 @@
         else:
             return ChannelBatch(
                 channel=self.channel, key=self.key, bound=self.bound | joiner
             )
 
     def __or__(  # type: ignore[override]
         self,
-        other: Runnable[Any, Other]
-        | Callable[[Any], Other]
-        | Mapping[str, Runnable[Any, Other] | Callable[[Any], Other]],
+        other: Union[
+            Runnable[Any, Other],
+            Callable[[Any], Other],
+            Mapping[str, Runnable[Any, Other] | Callable[[Any], Other]],
+        ],
     ) -> ChannelBatch:
         if self.bound is default_bound:
             return ChannelBatch(
                 channel=self.channel, key=self.key, bound=coerce_to_runnable(other)
             )
         else:
             # delegate to __or__ in self.bound
             return ChannelBatch(
                 channel=self.channel, key=self.key, bound=self.bound | other
             )
 
     def __ror__(
         self,
-        other: Runnable[Other, Any]
-        | Callable[[Any], Other]
-        | Mapping[str, Runnable[Other, Any] | Callable[[Other], Any]],
+        other: Union[
+            Runnable[Other, Any],
+            Callable[[Any], Other],
+            Mapping[str, Runnable[Other, Any] | Callable[[Other], Any]],
+        ],
     ) -> RunnableSerializable:
         raise NotImplementedError()
```

### Comparing `langgraph-0.0.8/langgraph/pregel/validate.py` & `langgraph-0.0.9/langgraph/pregel/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Mapping, Sequence
+from typing import Any, Mapping, Sequence, Union
 
 from langgraph.channels.base import BaseChannel
 from langgraph.channels.last_value import LastValue
 from langgraph.pregel.read import ChannelBatch, ChannelInvoke
 from langgraph.pregel.reserved import ReservedChannels
 
 
 def validate_graph(
-    nodes: Mapping[str, ChannelInvoke | ChannelBatch],
+    nodes: Mapping[str, Union[ChannelInvoke, ChannelBatch]],
     channels: dict[str, BaseChannel],
-    input: str | Sequence[str],
-    output: str | Sequence[str],
+    input: Union[str, Sequence[str]],
+    output: Union[str, Sequence[str]],
 ) -> None:
     subscribed_channels = set[str]()
     for node in nodes.values():
         if isinstance(node, ChannelInvoke):
             subscribed_channels.update(node.channels.values())
         elif isinstance(node, ChannelBatch):
             subscribed_channels.add(node.channel)
```

### Comparing `langgraph-0.0.8/langgraph/pregel/write.py` & `langgraph-0.0.9/langgraph/pregel/write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Sequence
+from typing import Any, Callable, Optional, Sequence
 
 from langchain_core.runnables import (
     Runnable,
     RunnableConfig,
     RunnablePassthrough,
 )
 from langchain_core.runnables.utils import ConfigurableFieldSpec
 
 from langgraph.constants import CONFIG_KEY_SEND
 
 TYPE_SEND = Callable[[Sequence[tuple[str, Any]]], None]
 
 
 class ChannelWrite(RunnablePassthrough):
-    channels: Sequence[tuple[str, Runnable | None]]
+    channels: Sequence[tuple[str, Optional[Runnable]]]
     """
     Mapping of write channels to Runnables that return the value to be written,
     or None to skip writing.
     """
 
     class Config:
         arbitrary_types_allowed = True
 
     def __init__(
         self,
         *,
-        channels: Sequence[tuple[str, Runnable | None]],
+        channels: Sequence[tuple[str, Optional[Runnable]]],
     ):
         super().__init__(func=self._write, afunc=self._awrite, channels=channels)
         self.name = f"ChannelWrite<{','.join(chan for chan, _ in self.channels)}>"
 
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
         return [
```

### Comparing `langgraph-0.0.8/pyproject.toml` & `langgraph-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "langgraph"
-version = "0.0.8"
+version = "0.0.9"
 description = "langgraph"
 authors = []
 license = "LangGraph License"
 readme = "README.md"
 repository = "https://www.github.com/langchain-ai/langgraph"
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0"
+python = ">=3.9.0,<4.0"
 langchain-core = "^0.1.8"
 
 
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
```

