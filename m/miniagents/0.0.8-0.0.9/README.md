# Comparing `tmp/miniagents-0.0.8.tar.gz` & `tmp/miniagents-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniagents-0.0.8.tar", max compression
+gzip compressed data, was "miniagents-0.0.9.tar", max compression
```

## Comparing `miniagents-0.0.8.tar` & `miniagents-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.8/LICENSE
--rw-r--r--   0        0        0       19 2024-04-03 21:42:22.424193 miniagents-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.8/miniagents/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.8/miniagents/ext/__init__.py
--rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725975 miniagents-0.0.8/miniagents/ext/llms/__init__.py
--rw-r--r--   0        0        0     4307 2024-04-29 06:06:00.887264 miniagents-0.0.8/miniagents/ext/llms/anthropic.py
--rw-r--r--   0        0        0     8301 2024-05-05 14:27:35.144467 miniagents-0.0.8/miniagents/messages.py
--rw-r--r--   0        0        0    16169 2024-05-05 14:47:49.141620 miniagents-0.0.8/miniagents/miniagents.py
--rw-r--r--   0        0        0        0 2024-04-27 10:16:52.343384 miniagents-0.0.8/miniagents/promising/__init__.py
--rw-r--r--   0        0        0      548 2024-04-28 10:26:42.580105 miniagents-0.0.8/miniagents/promising/errors.py
--rw-r--r--   0        0        0     6122 2024-05-05 14:27:35.146244 miniagents-0.0.8/miniagents/promising/node.py
--rw-r--r--   0        0        0    20940 2024-05-05 14:27:35.146955 miniagents-0.0.8/miniagents/promising/promising.py
--rw-r--r--   0        0        0      453 2024-04-27 10:16:52.345574 miniagents-0.0.8/miniagents/promising/sentinels.py
--rw-r--r--   0        0        0     1881 2024-04-28 10:27:04.793246 miniagents-0.0.8/miniagents/promising/sequence.py
--rw-r--r--   0        0        0     2474 2024-04-28 10:26:42.582714 miniagents-0.0.8/miniagents/promising/typing.py
--rw-r--r--   0        0        0     2302 2024-04-29 06:06:00.889297 miniagents-0.0.8/miniagents/utils.py
--rw-r--r--   0        0        0      694 2024-04-23 16:40:25.878553 miniagents-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 miniagents-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-03-27 07:32:21.725211 miniagents-0.0.9/LICENSE
+-rw-r--r--   0        0        0      829 2024-05-22 20:44:51.677911 miniagents-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725673 miniagents-0.0.9/miniagents/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 07:32:21.725814 miniagents-0.0.9/miniagents/ext/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 06:47:04.188664 miniagents-0.0.9/miniagents/ext/llm/__init__.py
+-rw-r--r--   0        0        0     6783 2024-05-22 20:44:51.678826 miniagents-0.0.9/miniagents/ext/llm/anthropic.py
+-rw-r--r--   0        0        0      577 2024-05-19 14:33:20.444960 miniagents-0.0.9/miniagents/ext/llm/llm_common.py
+-rw-r--r--   0        0        0     5736 2024-05-19 14:33:20.446007 miniagents-0.0.9/miniagents/ext/llm/openai.py
+-rw-r--r--   0        0        0     8288 2024-05-19 14:33:20.447056 miniagents-0.0.9/miniagents/messages.py
+-rw-r--r--   0        0        0    16823 2024-05-22 20:44:51.679370 miniagents-0.0.9/miniagents/miniagents.py
+-rw-r--r--   0        0        0        0 2024-04-27 10:16:52.343384 miniagents-0.0.9/miniagents/promising/__init__.py
+-rw-r--r--   0        0        0      548 2024-04-28 10:26:42.580105 miniagents-0.0.9/miniagents/promising/errors.py
+-rw-r--r--   0        0        0     6122 2024-05-05 14:27:35.146244 miniagents-0.0.9/miniagents/promising/node.py
+-rw-r--r--   0        0        0    21701 2024-05-22 20:44:51.679946 miniagents-0.0.9/miniagents/promising/promising.py
+-rw-r--r--   0        0        0      465 2024-05-22 20:44:51.680771 miniagents-0.0.9/miniagents/promising/sentinels.py
+-rw-r--r--   0        0        0     1881 2024-04-28 10:27:04.793246 miniagents-0.0.9/miniagents/promising/sequence.py
+-rw-r--r--   0        0        0     2474 2024-05-09 17:35:27.336242 miniagents-0.0.9/miniagents/promising/typing.py
+-rw-r--r--   0        0        0     9520 2024-05-22 20:44:51.681515 miniagents-0.0.9/miniagents/utils.py
+-rw-r--r--   0        0        0      707 2024-05-14 20:49:36.136330 miniagents-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 miniagents-0.0.9/PKG-INFO
```

### Comparing `miniagents-0.0.8/LICENSE` & `miniagents-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.8/miniagents/messages.py` & `miniagents-0.0.9/miniagents/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             return self.text
         if self.text_template is not None:
             return self.text_template.format(**self.model_dump())
         return super()._as_string()
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
-        self._serialize_message_event_triggered = False
+        self._persist_message_event_triggered = False
 
 
 class MessagePromise(StreamedPromise[str, Message]):
     """
     A promise of a message that can be streamed token by token.
     """
 
@@ -188,15 +188,15 @@
     """
 
     async def acollect_messages(self) -> tuple[Message, ...]:
         """
         Collect all messages from the sequence and return them as a tuple of Message objects.
         """
         # pylint: disable=consider-using-generator
-        return tuple([await message_promise.acollect() async for message_promise in self])
+        return tuple([await message_promise async for message_promise in self])
 
     def __aiter__(self) -> AsyncIterator[MessagePromise]:
         # PyCharm fails to see that MessageSequencePromise inherits AsyncIterable protocol from StreamedPromise,
         # hence the need to explicitly declare the __aiter__ method here
         return super().__aiter__()
```

### Comparing `miniagents-0.0.8/miniagents/miniagents.py` & `miniagents-0.0.9/miniagents/miniagents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,128 +1,131 @@
 """
 "Core" classes of the MiniAgents framework.
 """
 
+from functools import partial
 from typing import Protocol, AsyncIterator, Any, Union, Optional, Callable, Iterable
 
 from pydantic import BaseModel
 
 from miniagents.messages import MessageType, MessagePromise, MessageSequencePromise, Message
 from miniagents.promising.node import Node
 from miniagents.promising.promising import AppendProducer, Promise, PromisingContext
 from miniagents.promising.sentinels import Sentinel, DEFAULT
 from miniagents.promising.sequence import FlatSequence
-from miniagents.promising.typing import StreamedPieceProducer, NodeCollectedEventHandler
+from miniagents.promising.typing import StreamedPieceProducer, NodeCollectedEventHandler, PromiseBound
 
 
-class SerializeMessageEventHandler(Protocol):
+class PersistMessageEventHandler(Protocol):
     """
     TODO Oleksandr: docstring
     """
 
-    async def __call__(self, promise: MessagePromise, message: Message) -> None: ...
+    async def __call__(self, promise: PromiseBound, message: Message) -> None: ...
 
 
 class MiniAgents(PromisingContext):
     """
     TODO Oleksandr: docstring
     """
 
     def __init__(
         self,
         stream_llm_tokens_by_default: bool = True,
         on_node_collected: Union[NodeCollectedEventHandler, Iterable[NodeCollectedEventHandler]] = (),
-        on_serialize_message: Union[SerializeMessageEventHandler, Iterable[SerializeMessageEventHandler]] = (),
+        on_persist_message: Union[PersistMessageEventHandler, Iterable[PersistMessageEventHandler]] = (),
         **kwargs,
     ) -> None:
         on_node_collected = (
-            [self._schedule_serialize_message_event, on_node_collected]
+            [self._schedule_persist_message_event, on_node_collected]
             if callable(on_node_collected)
-            else [self._schedule_serialize_message_event, *on_node_collected]
+            else [self._schedule_persist_message_event, *on_node_collected]
         )
         super().__init__(on_node_collected=on_node_collected, **kwargs)
         self.stream_llm_tokens_by_default = stream_llm_tokens_by_default
-        self.on_serialize_message_handlers: list[SerializeMessageEventHandler] = (
-            [on_serialize_message] if callable(on_serialize_message) else list(on_serialize_message)
+        self.on_persist_message_handlers: list[PersistMessageEventHandler] = (
+            [on_persist_message] if callable(on_persist_message) else list(on_persist_message)
         )
 
     @classmethod
     def get_current(cls) -> "MiniAgents":
         """
         TODO Oleksandr: docstring
         """
         # noinspection PyTypeChecker
         return super().get_current()
 
-    def on_serialize_message(self, handler: SerializeMessageEventHandler) -> SerializeMessageEventHandler:
+    def on_persist_message(self, handler: PersistMessageEventHandler) -> PersistMessageEventHandler:
         """
-        Add a handler that will be called every time a Message needs to be serialized.
+        Add a handler that will be called every time a Message needs to be persisted.
         """
-        self.on_serialize_message_handlers.append(handler)
+        self.on_persist_message_handlers.append(handler)
         return handler
 
     # noinspection PyProtectedMember
-    async def _schedule_serialize_message_event(self, _, node: Node) -> None:
+    async def _schedule_persist_message_event(self, _, node: Node) -> None:
         """
         TODO Oleksandr: docstring
         """
         # pylint: disable=protected-access
         if not isinstance(node, Message):
             return
 
         for sub_message in node.sub_messages():
-            if sub_message._serialize_message_event_triggered:
+            if sub_message._persist_message_event_triggered:
                 continue
 
-            for handler in self.on_serialize_message_handlers:
+            for handler in self.on_persist_message_handlers:
                 self.schedule_task(handler(_, sub_message))
-            sub_message._serialize_message_event_triggered = True
+            sub_message._persist_message_event_triggered = True
 
-        if node._serialize_message_event_triggered:
+        if node._persist_message_event_triggered:
             return
 
-        for handler in self.on_serialize_message_handlers:
+        for handler in self.on_persist_message_handlers:
             self.schedule_task(handler(_, node))
-        node._serialize_message_event_triggered = True
+        node._persist_message_event_triggered = True
 
 
 def miniagent(
     func: Optional["AgentFunction"] = None,
-    /,  # TODO Oleksandr: do I really need to enforce positional-only upon `func` ?
     alias: Optional[str] = None,
     description: Optional[str] = None,
     uppercase_func_name: bool = True,
     normalize_spaces_in_docstring: bool = True,
     interaction_metadata: Optional[dict[str, Any]] = None,
+    **partial_kwargs,
 ) -> Union["MiniAgent", Callable[["AgentFunction"], "MiniAgent"]]:
     """
     A decorator that converts an agent function into an agent.
     """
     if func is None:
         # the decorator `@miniagent(...)` was used with arguments
         def _decorator(f: "AgentFunction") -> "MiniAgent":
             return MiniAgent(
                 f,
                 alias=alias,
                 description=description,
                 uppercase_func_name=uppercase_func_name,
                 normalize_spaces_in_docstring=normalize_spaces_in_docstring,
                 interaction_metadata=interaction_metadata,
+                **partial_kwargs,
             )
 
         return _decorator
 
     # the decorator `@miniagent` was used either without arguments or as a direct function call
     return MiniAgent(
         func,
         alias=alias,
         description=description,
         uppercase_func_name=uppercase_func_name,
         normalize_spaces_in_docstring=normalize_spaces_in_docstring,
         interaction_metadata=interaction_metadata,
+        **partial_kwargs,
     )
 
 
 class AgentFunction(Protocol):
     """
     A protocol for agent functions.
     """
@@ -146,16 +149,28 @@
         """
         TODO Oleksandr: docstring
         """
         # TODO Oleksandr: add a warning that iterators, async iterators and generators, if passed as `messages` will
         #  not be iterated over immediately, which means that if two agent calls are passed as a generator, those
         #  agent calls will not be scheduled for parallel execution, unless the generator is wrapped into a list (to
         #  guarantee that it will be iterated over immediately)
+        # TODO Oleksandr: implement a utility in MiniAgents that deep-copies/freezes mutable data containers
+        #  while keeping objects of other types intact and use it in AppendProducer to freeze the state of those
+        #  objects upon their submission (this way the user will not have to worry about things like `history[:]`
+        #  in the code below)
         self._reply_producer.append(messages)
 
+    def finish_early(self) -> None:
+        """
+        TODO Oleksandr: docstring
+        TODO Oleksandr: is this a good name for this method ?
+        TODO Oleksandr: what to do with exceptions in agent function that may happen after this method was called ?
+        """
+        self._reply_producer.close()
+
 
 class AgentCall:
     """
     TODO Oleksandr: docstring
     TODO Oleksandr: turn this into a context manager ?
     """
 
@@ -206,19 +221,21 @@
         func: AgentFunction,
         alias: Optional[str] = None,
         description: Optional[str] = None,
         # TODO Oleksandr: use DEFAULT for the following two arguments (and put them into MiniAgents class)
         uppercase_func_name: bool = True,
         normalize_spaces_in_docstring: bool = True,
         interaction_metadata: Optional[dict[str, Any]] = None,
-        # TODO Oleksandr: turn MiniAgent into a Node object so arbitrary agent level metadata can be stored in it ?
+        **partial_kwargs,
     ) -> None:
         self._func = func
         # TODO Oleksandr: do deep copy ? freeze with Node ? yoo need to start putting these things down into the
         #  "Philosophy" section of README
+        if partial_kwargs:
+            self._func = partial(func, **partial_kwargs)
         self.interaction_metadata = interaction_metadata or {}
 
         self.alias = alias
         if self.alias is None:
             self.alias = func.__name__
             if uppercase_func_name:
                 self.alias = self.alias.upper()
@@ -426,15 +443,15 @@
         async for reply_promise in super()._producer(_):
             yield reply_promise  # at this point all MessageType items are "flattened" into MessagePromise items
 
         async def create_agent_reply_node(_) -> AgentReplyNode:
             return AgentReplyNode(
                 replies=await self.sequence_promise.acollect_messages(),
                 agent_alias=self._mini_agent.alias,
-                agent_call=await agent_call_promise.acollect(),
+                agent_call=await agent_call_promise,
                 **self._mini_agent.interaction_metadata,
             )
 
         Promise[AgentReplyNode](
             schedule_immediately=True,  # use a separate async task to avoid deadlock upon AgentReplyNode "collection"
             fulfiller=create_agent_reply_node,
         )
```

### Comparing `miniagents-0.0.8/miniagents/promising/errors.py` & `miniagents-0.0.9/miniagents/promising/errors.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.8/miniagents/promising/node.py` & `miniagents-0.0.9/miniagents/promising/node.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.8/miniagents/promising/promising.py` & `miniagents-0.0.9/miniagents/promising/promising.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,17 +119,20 @@
         """
 
         async def awaitable_wrapper() -> Any:
             # noinspection PyBroadException
             try:
                 return await awaitable
             except BaseException:  # pylint: disable=broad-except
-                if suppress_errors:
-                    logger.debug("AN ERROR OCCURRED IN A SCHEDULED TASK BUT WAS SUPPRESSED", exc_info=True)
-                else:
+                logger.debug(
+                    "An error occurred in a scheduled task (suppress_errors=%s)",
+                    suppress_errors,
+                    exc_info=True,
+                )
+                if not suppress_errors:
                     raise
             finally:
                 self.child_tasks.remove(task)
 
         task = asyncio.create_task(awaitable_wrapper())
         self.child_tasks.add(task)
         return task
@@ -199,15 +202,15 @@
         else:
             self._result = prefill_result
             self._schedule_collected_event_handlers()
 
         self._fulfiller_lock = asyncio.Lock()
 
         if schedule_immediately and prefill_result is NO_VALUE:
-            promising_context.schedule_task(self.acollect())
+            promising_context.schedule_task(self)
 
     async def acollect(self) -> T:
         """
         TODO Oleksandr: update this docstring
         "Accumulates" all the pieces of the stream and returns the "whole" value. Will return the exact
         same object (the exact same instance) if called multiple times on the same instance of `StreamedPromise`.
         """
@@ -215,22 +218,26 @@
         #  `acollect()` from within the `fulfiller` function
         if self._result is NO_VALUE:
             async with self._fulfiller_lock:
                 if self._result is NO_VALUE:
                     try:
                         self._result = await self.__fulfiller(self)
                     except BaseException as exc:  # pylint: disable=broad-except
+                        logger.debug("An error occurred while fulfilling a Promise", exc_info=True)
                         self._result = exc
 
                     self._schedule_collected_event_handlers()
 
         if isinstance(self._result, BaseException):
             raise self._result
         return self._result
 
+    def __await__(self):
+        return self.acollect().__await__()
+
     def _schedule_collected_event_handlers(self):
         promising_context = PromisingContext.get_current()
         while promising_context:
             for handler in promising_context.on_promise_collected_handlers:
                 promising_context.schedule_task(handler(self, self._result))
             promising_context = promising_context.parent
 
@@ -314,24 +321,30 @@
         # pylint: disable=broad-except
         if self._producer_iterator is None:
             try:
                 self._producer_iterator = self.__producer(self)
                 if not callable(self._producer_iterator.__anext__):
                     raise TypeError("The producer must return an async iterator")
             except BaseException as exc:
+                logger.debug("An error occurred while instantiating a producer for a StreamedPromise", exc_info=True)
                 self._producer_iterator = FAILED
                 return exc
 
         elif self._producer_iterator is FAILED:
             # we were not able to instantiate the producer iterator at all - stopping the stream
             return StopAsyncIteration()
 
         try:
             return await self._producer_iterator.__anext__()
         except BaseException as exc:
+            if not isinstance(exc, StopAsyncIteration):
+                logger.debug(
+                    'An error occurred while fetching a single "piece" of a StreamedPromise from its pieces producer.',
+                    exc_info=True,
+                )
             # Any exception, apart from `StopAsyncIteration`, will always be stored in the `_pieces_so_far` list
             # before the `StopAsyncIteration` and will not conclude the list (in other words, `StopAsyncIteration`
             # will always conclude the `_pieces_so_far` list). This is because if you keep iterating over an
             # iterator/generator past any other exception that it might raise, it is still supposed to raise
             # `StopAsyncIteration` at the end.
             return exc
 
@@ -408,20 +421,24 @@
     def __exit__(
         self,
         exc_type: Optional[type[BaseException]],
         exc_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> bool:
         is_append_closed_error = isinstance(exc_value, AppendClosedError)
-        if exc_value and not is_append_closed_error and self._capture_errors:
+        error_should_not_propagate = self._capture_errors and not is_append_closed_error
+
+        if exc_value and error_should_not_propagate:
+            logger.debug("An error occurred while appending pieces to an AppendProducer", exc_info=exc_value)
             self.append(exc_value)
         self.close()
-        # if `_capture_errors` is True, then we also return True, so that the exception is not propagated outside
+
+        # if `capture_errors` is True, then we also return True, so that the exception is not propagated outside
         # the `with` block (except if the error is an `AppendClosedError` - in this case, we do not suppress it)
-        return self._capture_errors and not is_append_closed_error
+        return error_should_not_propagate
 
     def append(self, piece: PIECE) -> "AppendProducer":
         """
         Append a `piece` to the producer. This method can only be called when the producer is open for appending (and
         also not closed yet). Consequently, the `piece` is delivered to the `StreamedPromise` that is consuming from
         this producer.
         """
```

### Comparing `miniagents-0.0.8/miniagents/promising/sequence.py` & `miniagents-0.0.9/miniagents/promising/sequence.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.8/miniagents/promising/typing.py` & `miniagents-0.0.9/miniagents/promising/typing.py`

 * *Files identical despite different names*

### Comparing `miniagents-0.0.8/pyproject.toml` & `miniagents-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 line-length = 119
 
 [tool.coverage.run]
 branch = true
 
 [tool.poetry]
 name = "miniagents"
-version = "0.0.8"
+version = "0.0.9"
 description = """\
 TODO Oleksandr\
 """
 authors = ["Oleksandr Tereshchenko <toporok@gmail.com>"]
 homepage = "https://github.com/teremterem/MiniAgents"
 readme = "README.md"
 license = "MIT"
@@ -21,14 +21,15 @@
 
 [tool.poetry.dev-dependencies]
 anthropic = "*"
 black = "*"
 ipython = "*"
 jupyterlab = "*"
 notebook = "*"
+openai = "*"
 pre-commit = "*"
 promptlayer = "*"
 pylint = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
 python-dotenv = "*"
```

