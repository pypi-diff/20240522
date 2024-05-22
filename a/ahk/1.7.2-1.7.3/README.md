# Comparing `tmp/ahk-1.7.2.tar.gz` & `tmp/ahk-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ahk-1.7.2.tar", last modified: Fri May 10 07:59:38 2024, max compression
+gzip compressed data, was "ahk-1.7.3.tar", last modified: Wed May 22 01:10:23 2024, max compression
```

## Comparing `ahk-1.7.2.tar` & `ahk-1.7.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.646675 ahk-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-10 07:59:31.000000 ahk-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-10 07:59:31.000000 ahk-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-10 07:59:38.646675 ahk-1.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.638675 ahk-1.7.2/ahk/
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/_async/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   206949 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    47647 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_async/window.py
--rw-r--r--   0 runner    (1001) docker     (127)   171011 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_hotkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/_sync/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   200233 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    42697 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_sync/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/message.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    80096 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/daemon-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)    80517 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/daemon.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/hotkeys-v2.ahk
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-10 07:59:31.000000 ahk-1.7.2/ahk/templates/hotkeys.ahk
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/ahk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-10 07:59:38.000000 ahk-1.7.2/ahk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-10 07:59:31.000000 ahk-1.7.2/buildunasync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 07:59:38.642675 ahk-1.7.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-05-10 07:59:31.000000 ahk-1.7.2/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-10 07:59:31.000000 ahk-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-10 07:59:38.646675 ahk-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 07:59:31.000000 ahk-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.302622 ahk-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-22 01:10:13.000000 ahk-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 01:10:13.000000 ahk-1.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-22 01:10:23.302622 ahk-1.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.294622 ahk-1.7.3/ahk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.298622 ahk-1.7.3/ahk/_async/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210809 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_async/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48128 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_async/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30507 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_async/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172200 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17219 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.298622 ahk-1.7.3/ahk/_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   203991 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_sync/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43146 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_sync/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_sync/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7404 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10999 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.298622 ahk-1.7.3/ahk/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    80688 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/templates/daemon-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)    81114 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/templates/daemon.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/templates/hotkeys-v2.ahk
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-22 01:10:13.000000 ahk-1.7.3/ahk/templates/hotkeys.ahk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.298622 ahk-1.7.3/ahk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28092 2024-05-22 01:10:23.000000 ahk-1.7.3/ahk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-22 01:10:23.000000 ahk-1.7.3/ahk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:10:23.000000 ahk-1.7.3/ahk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 01:10:23.000000 ahk-1.7.3/ahk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 01:10:23.000000 ahk-1.7.3/ahk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-22 01:10:13.000000 ahk-1.7.3/buildunasync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:10:23.298622 ahk-1.7.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    26719 2024-05-22 01:10:13.000000 ahk-1.7.3/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 01:10:13.000000 ahk-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-22 01:10:23.302622 ahk-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:10:13.000000 ahk-1.7.3/setup.py
```

### Comparing `ahk-1.7.2/LICENSE` & `ahk-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/PKG-INFO` & `ahk-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.2
+Version: 1.7.3
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.2/ahk/__init__.py` & `ahk-1.7.3/ahk/__init__.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/_async/engine.py` & `ahk-1.7.3/ahk/_async/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1281,41 +1281,125 @@
             args.append('')
 
         resp = await self._transport.function_call('AHKSendPlay', args=args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    async def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
     @overload
-    async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    async def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
     @overload
-    async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
+    async def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
-    async def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    async def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
     # fmt: on
     async def set_capslock_state(
-        self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
     ) -> Union[None, AsyncFutureResult[None]]:
         """
         Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
         """
         args: List[str] = []
         if state is not None:
             if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
                 raise ValueError(
                     f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
                 )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
             args.append(str(state))
+        else:
+            args.append('')
 
         resp = await self._transport.function_call('AHKSetCapsLockState', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
+    async def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    @overload
+    async def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    @overload
+    async def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
+    @overload
+    async def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    # fmt: on
+    async def set_numlock_state(
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
+        args: List[str] = []
+        if state is not None:
+            if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
+                raise ValueError(
+                    f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
+                )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
+            args.append(str(state))
+        else:
+            args.append('')
+
+        resp = await self._transport.function_call('AHKSetNumLockState', args, blocking=blocking)
+        return resp
+
+    # fmt: off
+    @overload
+    async def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    @overload
+    async def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    @overload
+    async def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
+    @overload
+    async def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
+    # fmt: on
+    async def set_scroll_lock_state(
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, AsyncFutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
+        args: List[str] = []
+        if state is not None:
+            if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
+                raise ValueError(
+                    f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
+                )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
+            args.append(str(state))
+        else:
+            args.append('')
+
+        resp = await self._transport.function_call('AHKSetScrollLockState', args, blocking=blocking)
+        return resp
+
+    # fmt: off
+    @overload
     async def set_volume(self, value: int, device_number: int = 1) -> None: ...
     @overload
     async def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[False]) -> AsyncFutureResult[None]: ...
     @overload
     async def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[True]) -> None: ...
     @overload
     async def set_volume(self, value: int, device_number: int = 1, *, blocking: bool = True) -> Union[None, AsyncFutureResult[None]]: ...
```

### Comparing `ahk-1.7.2/ahk/_async/transport.py` & `ahk-1.7.3/ahk/_async/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,18 @@
     @overload
     async def function_call(self, function_name: Literal['AHKSendEvent'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKSendPlay'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKSetCapsLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
     @overload
+    async def function_call(self, function_name: Literal['AHKSetNumLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
+    @overload
+    async def function_call(self, function_name: Literal['AHKSetScrollLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
+    @overload
     async def function_call(self, function_name: Literal['AHKWinGetTitle'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[str, AsyncFutureResult[str]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKWinGetClass'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[str, AsyncFutureResult[str]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKWinGetText'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[str, AsyncFutureResult[str]]: ...
     @overload
     async def function_call(self, function_name: Literal['AHKWinActivate'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AsyncAHK[Any]] = None) -> Union[None, AsyncFutureResult[None]]: ...
```

### Comparing `ahk-1.7.2/ahk/_async/window.py` & `ahk-1.7.3/ahk/_async/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/_constants.py` & `ahk-1.7.3/ahk/_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -2054,14 +2054,39 @@
     } else {
         SetCapsLockState, %state%
     }
     return FormatNoValueResponse()
     {% endblock AHKSetCapsLockState %}
 }
 
+
+AHKSetNumLockState(args*) {
+    {% block AHKSetNumLockState %}
+    state := args[1]
+    if (state = "") {
+        SetNumLockState % !GetKeyState("NumLock", "T")
+    } else {
+        SetNumLockState, %state%
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetNumLockState %}
+}
+
+AHKSetScrollLockState(args*) {
+    {% block AHKSetScrollLockState %}
+    state := args[1]
+    if (state = "") {
+        SetScrollLockState % !GetKeyState("ScrollLock", "T")
+    } else {
+        SetScrollLockState, %state%
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetScrollLockState %}
+}
+
 HideTrayTip(args*) {
     {% block HideTrayTip %}
     TrayTip ; Attempt to hide it the normal way.
     if SubStr(A_OSVersion,1,3) = "10." {
         Menu Tray, NoIcon
         Sleep 200 ; It may be necessary to adjust this sleep.
         Menu Tray, Icon
@@ -5143,14 +5168,40 @@
     } else {
         SetCapsLockState(state)
     }
     return FormatNoValueResponse()
     {% endblock AHKSetCapsLockState %}
 }
 
+
+AHKSetNumLockState(args*) {
+    {% block AHKSetNumLockState %}
+    state := args[1]
+    if (state = "") {
+        SetNumLockState(!GetKeyState("NumLock", "T"))
+    } else {
+        SetNumLockState(state)
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetNumLockState %}
+}
+
+
+AHKSetScrollLockState(args*) {
+    {% block AHKSetScrollLockState %}
+    state := args[1]
+    if (state = "") {
+        SetScrollLockState(!GetKeyState("ScrollLock", "T"))
+    } else {
+        SetScrollLockState(state)
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetScrollLockState %}
+}
+
 HideTrayTip(args*) {
     {% block HideTrayTip %}
     TrayTip ; Attempt to hide it the normal way.
     if SubStr(A_OSVersion,1,3) = "10." {
         A_IconHidden := true
         Sleep 200 ; It may be necessary to adjust this sleep.
         A_IconHidden := false
```

### Comparing `ahk-1.7.2/ahk/_hotkey.py` & `ahk-1.7.3/ahk/_hotkey.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/_sync/engine.py` & `ahk-1.7.3/ahk/_sync/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1269,41 +1269,125 @@
             args.append('')
 
         resp = self._transport.function_call('AHKSendPlay', args=args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
-    def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
     @overload
-    def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
     @overload
-    def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> FutureResult[None]: ...
+    def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
-    def set_capslock_state(self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    def set_capslock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
     # fmt: on
     def set_capslock_state(
-        self, state: Optional[Literal[0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
     ) -> Union[None, FutureResult[None]]:
         """
         Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
         """
         args: List[str] = []
         if state is not None:
             if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
                 raise ValueError(
                     f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
                 )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
             args.append(str(state))
+        else:
+            args.append('')
 
         resp = self._transport.function_call('AHKSetCapsLockState', args, blocking=blocking)
         return resp
 
     # fmt: off
     @overload
+    def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    @overload
+    def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    @overload
+    def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> FutureResult[None]: ...
+    @overload
+    def set_numlock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    # fmt: on
+    def set_numlock_state(
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
+        args: List[str] = []
+        if state is not None:
+            if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
+                raise ValueError(
+                    f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
+                )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
+            args.append(str(state))
+        else:
+            args.append('')
+
+        resp = self._transport.function_call('AHKSetNumLockState', args, blocking=blocking)
+        return resp
+
+    # fmt: off
+    @overload
+    def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None) -> None: ...
+    @overload
+    def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[True]) -> None: ...
+    @overload
+    def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: Literal[False]) -> FutureResult[None]: ...
+    @overload
+    def set_scroll_lock_state(self, state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
+    # fmt: on
+    def set_scroll_lock_state(
+        self,
+        state: Optional[Literal[True, False, 0, 1, 'On', 'Off', 'AlwaysOn', 'AlwaysOff']] = None,
+        *,
+        blocking: bool = True,
+    ) -> Union[None, FutureResult[None]]:
+        """
+        Analog for `SetCapsLockState <https://www.autohotkey.com/docs/commands/SetNumScrollCapsLockState.htm>`_
+        """
+        args: List[str] = []
+        if state is not None:
+            if str(state).lower() not in ('1', '0', 'on', 'off', 'alwayson', 'alwaysoff'):
+                raise ValueError(
+                    f'Invalid value for state. Must be one of On, Off, AlwaysOn, AlwaysOff or None. Got {state!r}'
+                )
+            if state is True:
+                state = 'On'
+            elif state is False:
+                state = 'Off'
+
+            args.append(str(state))
+        else:
+            args.append('')
+
+        resp = self._transport.function_call('AHKSetScrollLockState', args, blocking=blocking)
+        return resp
+
+    # fmt: off
+    @overload
     def set_volume(self, value: int, device_number: int = 1) -> None: ...
     @overload
     def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[False]) -> FutureResult[None]: ...
     @overload
     def set_volume(self, value: int, device_number: int = 1, *, blocking: Literal[True]) -> None: ...
     @overload
     def set_volume(self, value: int, device_number: int = 1, *, blocking: bool = True) -> Union[None, FutureResult[None]]: ...
```

### Comparing `ahk-1.7.2/ahk/_sync/transport.py` & `ahk-1.7.3/ahk/_sync/transport.py`

 * *Files 0% similar despite different names*

```diff
@@ -306,14 +306,18 @@
     @overload
     def function_call(self, function_name: Literal['AHKSendEvent'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKSendPlay'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKSetCapsLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
     @overload
+    def function_call(self, function_name: Literal['AHKSetNumLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
+    @overload
+    def function_call(self, function_name: Literal['AHKSetScrollLockState'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
+    @overload
     def function_call(self, function_name: Literal['AHKWinGetTitle'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[str, FutureResult[str]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKWinGetClass'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[str, FutureResult[str]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKWinGetText'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[str, FutureResult[str]]: ...
     @overload
     def function_call(self, function_name: Literal['AHKWinActivate'], args: Optional[List[str]] = None, *, blocking: bool = True, engine: Optional[AHK[Any]] = None) -> Union[None, FutureResult[None]]: ...
```

### Comparing `ahk-1.7.2/ahk/_sync/window.py` & `ahk-1.7.3/ahk/_sync/window.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/_types.py` & `ahk-1.7.3/ahk/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,16 @@
     'AHKWindowList',
     'AHKWinWait',
     'AHKWinWaitActive',
     'AHKWinWaitClose',
     'AHKWinWaitNotActive',
     'AHKClick',
     'AHKSetCapsLockState',
+    'AHKSetNumLockState',
+    'AHKSetScrollLockState',
     'SetKeyDelay',
     'WinActivateBottom',
     'AHKWinGetClass',
     'AHKWinKill',
     'AHKWinMaximize',
     'AHKWinMinimize',
     'AHKWinRestore',
```

### Comparing `ahk-1.7.2/ahk/_utils.py` & `ahk-1.7.3/ahk/_utils.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/directives.py` & `ahk-1.7.3/ahk/directives.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/extensions.py` & `ahk-1.7.3/ahk/extensions.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/keys.py` & `ahk-1.7.3/ahk/keys.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/message.py` & `ahk-1.7.3/ahk/message.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/templates/daemon-v2.ahk` & `ahk-1.7.3/ahk/templates/daemon-v2.ahk`

 * *Files 0% similar despite different names*

```diff
@@ -2153,14 +2153,40 @@
     } else {
         SetCapsLockState(state)
     }
     return FormatNoValueResponse()
     {% endblock AHKSetCapsLockState %}
 }
 
+
+AHKSetNumLockState(args*) {
+    {% block AHKSetNumLockState %}
+    state := args[1]
+    if (state = "") {
+        SetNumLockState(!GetKeyState("NumLock", "T"))
+    } else {
+        SetNumLockState(state)
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetNumLockState %}
+}
+
+
+AHKSetScrollLockState(args*) {
+    {% block AHKSetScrollLockState %}
+    state := args[1]
+    if (state = "") {
+        SetScrollLockState(!GetKeyState("ScrollLock", "T"))
+    } else {
+        SetScrollLockState(state)
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetScrollLockState %}
+}
+
 HideTrayTip(args*) {
     {% block HideTrayTip %}
     TrayTip ; Attempt to hide it the normal way.
     if SubStr(A_OSVersion,1,3) = "10." {
         A_IconHidden := true
         Sleep 200 ; It may be necessary to adjust this sleep.
         A_IconHidden := false
```

### Comparing `ahk-1.7.2/ahk/templates/daemon.ahk` & `ahk-1.7.3/ahk/templates/daemon.ahk`

 * *Files 1% similar despite different names*

```diff
@@ -2051,14 +2051,39 @@
     } else {
         SetCapsLockState, %state%
     }
     return FormatNoValueResponse()
     {% endblock AHKSetCapsLockState %}
 }
 
+
+AHKSetNumLockState(args*) {
+    {% block AHKSetNumLockState %}
+    state := args[1]
+    if (state = "") {
+        SetNumLockState % !GetKeyState("NumLock", "T")
+    } else {
+        SetNumLockState, %state%
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetNumLockState %}
+}
+
+AHKSetScrollLockState(args*) {
+    {% block AHKSetScrollLockState %}
+    state := args[1]
+    if (state = "") {
+        SetScrollLockState % !GetKeyState("ScrollLock", "T")
+    } else {
+        SetScrollLockState, %state%
+    }
+    return FormatNoValueResponse()
+    {% endblock AHKSetScrollLockState %}
+}
+
 HideTrayTip(args*) {
     {% block HideTrayTip %}
     TrayTip ; Attempt to hide it the normal way.
     if SubStr(A_OSVersion,1,3) = "10." {
         Menu Tray, NoIcon
         Sleep 200 ; It may be necessary to adjust this sleep.
         Menu Tray, Icon
```

### Comparing `ahk-1.7.2/ahk/templates/hotkeys-v2.ahk` & `ahk-1.7.3/ahk/templates/hotkeys-v2.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk/templates/hotkeys.ahk` & `ahk-1.7.3/ahk/templates/hotkeys.ahk`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/ahk.egg-info/PKG-INFO` & `ahk-1.7.3/ahk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ahk
-Version: 1.7.2
+Version: 1.7.3
 Summary: A Python wrapper for AHK
 Home-page: https://github.com/spyoungtech/ahk
 Author: Spencer Young
 Author-email: spencer.young@spyoung.com
 Project-URL: Documentation, https://ahk.readthedocs.io/en/latest/
 Project-URL: Funding, https://github.com/sponsors/spyoungtech/
 Project-URL: Source, https://github.com/spyoungtech/ahk
```

### Comparing `ahk-1.7.2/ahk.egg-info/SOURCES.txt` & `ahk-1.7.3/ahk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/buildunasync.py` & `ahk-1.7.3/buildunasync.py`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/docs/README.md` & `ahk-1.7.3/docs/README.md`

 * *Files identical despite different names*

### Comparing `ahk-1.7.2/setup.cfg` & `ahk-1.7.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ahk
-version = 1.7.2
+version = 1.7.3
 author_email = spencer.young@spyoung.com
 author = Spencer Young
 description = A Python wrapper for AHK
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 url = https://github.com/spyoungtech/ahk
 project_urls =
```

