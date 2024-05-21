# Comparing `tmp/cs.resources-20240519.tar.gz` & `tmp/cs.resources-20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.resources-20240519.tar", last modified: Sun May 19 02:20:34 2024, max compression
+gzip compressed data, was "cs.resources-20240522.tar", last modified: Tue May 21 23:32:01 2024, max compression
```

## Comparing `cs.resources-20240519.tar` & `cs.resources-20240522.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.072875 cs.resources-20240519/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-19 02:20:02.000000 cs.resources-20240519/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    17728 2024-05-19 02:20:34.072564 cs.resources-20240519/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    16971 2024-05-19 02:20:12.000000 cs.resources-20240519/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.068001 cs.resources-20240519/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.068329 cs.resources-20240519/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.069930 cs.resources-20240519/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    27607 2024-05-19 02:19:49.000000 cs.resources-20240519/lib/python/cs/resources.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-19 02:20:34.072014 cs.resources-20240519/lib/python/cs.resources.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    17728 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-05-19 02:20:34.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      206 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-19 02:20:33.000000 cs.resources-20240519/lib/python/cs.resources.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    18338 2024-05-19 02:20:32.000000 cs.resources-20240519/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-19 02:20:34.072975 cs.resources-20240519/setup.cfg
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:32:01.531860 cs.resources-20240522/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2024-05-21 23:31:29.000000 cs.resources-20240522/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18506 2024-05-21 23:32:01.531543 cs.resources-20240522/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    17749 2024-05-21 23:31:40.000000 cs.resources-20240522/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:32:01.527538 cs.resources-20240522/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:32:01.527846 cs.resources-20240522/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:32:01.529242 cs.resources-20240522/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    28175 2024-05-21 23:31:16.000000 cs.resources-20240522/lib/python/cs/resources.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2024-05-21 23:32:01.531077 cs.resources-20240522/lib/python/cs.resources.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    18506 2024-05-21 23:32:00.000000 cs.resources-20240522/lib/python/cs.resources.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      297 2024-05-21 23:32:01.000000 cs.resources-20240522/lib/python/cs.resources.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2024-05-21 23:32:01.000000 cs.resources-20240522/lib/python/cs.resources.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      227 2024-05-21 23:32:01.000000 cs.resources-20240522/lib/python/cs.resources.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2024-05-21 23:32:01.000000 cs.resources-20240522/lib/python/cs.resources.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    19144 2024-05-21 23:31:59.000000 cs.resources-20240522/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)       38 2024-05-21 23:32:01.531962 cs.resources-20240522/setup.cfg
```

### Comparing `cs.resources-20240519/PKG-INFO` & `cs.resources-20240522/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,55 @@
-Metadata-Version: 2.1
-Name: cs.resources
-Version: 20240519
-Summary: Resource management classes and functions.
-Author-email: Cameron Simpson <cs@cskk.id.au>
-License: GNU General Public License v3 or later (GPLv3+)
-Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
-Keywords: python2,python3
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Description-Content-Type: text/markdown
+[project]
+name = "cs.resources"
+description = "Resource management classes and functions."
+authors = [
+    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
+]
+keywords = [
+    "python2",
+    "python3",
+]
+dependencies = [
+    "cs.context>=20240412",
+    "cs.deco>=20240412",
+    "cs.fsm>=20240519",
+    "cs.gimmicks>=20240316",
+    "cs.obj>=20220918",
+    "cs.pfx>=20240412",
+    "cs.psutils>=20240316",
+    "cs.py.func>=20230331",
+    "cs.py.stack>=20240519",
+    "cs.result>=20240412",
+    "cs.threads>=20240422",
+    "typeguard",
+]
+classifiers = [
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Python Modules",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+]
+version = "20240522"
 
+[project.license]
+text = "GNU General Public License v3 or later (GPLv3+)"
+
+[project.urls]
+URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
+
+[project.readme]
+text = """
 Resource management classes and functions.
 
-*Latest release 20240519*:
-RunState now subclasses cs.fsm.FSM.
+*Latest release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -78,15 +104,15 @@
         def startup_shutdown(self):
             with open_the_database() as db:
                 self._db = db
                 yield
 
 Why not just write a plain context manager class? Because in
 multithreaded or async code one wants to keep the instance
-"open" while any thread is still using it.
+\"open\" while any thread is still using it.
 This mixin lets threads use an instance in overlapping fashion:
 
     db_thing = DatabaseThing(...)
     with db_thing:
         ... kick off threads with access to the db ...
     ...
     thread 1:
@@ -271,15 +297,15 @@
 * stop
 
 Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
-in the "running" state.
+in the \"running\" state.
 
 *Method `RunState.__nonzero__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.cancel(self)`*:
 Set the cancelled flag; the associated process should notice and stop.
 
@@ -351,15 +377,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function uses_runstate.<locals>.<lambda> at 0x10424b250>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -374,18 +400,36 @@
 
 *Property `RunStateMixin.stopped`*:
 Test .runstate.stopped.
 
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
+## Function `uses_runstate(*da, **dkw)`
+
+A wrapper for `@default_params` which makes a new thread wide
+`RunState` parameter `runstate` if missing.
+The optional decorator parameter `name` may be used to specify
+a name for the new `RunState` if one is made. The default
+comes from the wrapped function's name.
+
+Example:
+
+    @uses_runstate
+    def do_something(blah, *, runstate:RunState):
+        ... do something, polling the runstate as approriate ...
+
 # Release Log
 
 
 
+*Release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
+
 *Release 20240519*:
 RunState now subclasses cs.fsm.FSM.
 
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
@@ -449,15 +493,15 @@
 * MultiOpenMixin.startup_shutdown: fix up shutdown logic, was not using a finally clause.
 * MultiOpenMixin: use ContextManagerMixin __enter_exit__ generator method instead of __enter__ and __exit__.
 
 *Release 20210906*:
 MultiOpenMixin: make startup and shutdown optional.
 
 *Release 20210731*:
-RunState: tune the sanity checks around whether the state is "running".
+RunState: tune the sanity checks around whether the state is \"running\".
 
 *Release 20210420*:
 MultiOpenMixin: run startup/shutdown entirely via the new default method @contextmanager(startup_shutdown), paving the way for subclasses to just define their own startup_shutdown context manager methods instead of distinct startup/shutdown methods.
 
 *Release 20201025*:
 MultiOpenMixin.__mo_getstate: dereference self.__dict__ because using AttributeError was pulling a state object from another instance, utterly weird.
 
@@ -483,17 +527,33 @@
 * RunState improvements.
 
 *Release 20171024*:
 * bugfix MultiOpenMixin finalise logic and other small logic fixes and checs
 * new class RunState for tracking or controlling a running task
 
 *Release 20160828*:
-Use "install_requires" instead of "requires" in DISTINFO.
+Use \"install_requires\" instead of \"requires\" in DISTINFO.
 
 *Release 20160827*:
 * BREAKING CHANGE: rename NestingOpenCloseMixin to MultiOpenMixin.
 * New Pool class for generic object reuse.
 * Assorted minor improvements.
 
 *Release 20150115*:
-First PyPI release.
+First PyPI release."""
+content-type = "text/markdown"
+
+[build-system]
+build-backend = "setuptools.build_meta"
+requires = [
+    "setuptools >= 61.2",
+    "trove-classifiers",
+    "wheel",
+]
+
+[tool.setuptools]
+py-modules = [
+    "cs.resources",
+]
 
+[tool.setuptools.package-dir]
+"" = "lib/python"
```

### Comparing `cs.resources-20240519/README.md` & `cs.resources-20240522/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Resource management classes and functions.
 
-*Latest release 20240519*:
-RunState now subclasses cs.fsm.FSM.
+*Latest release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -333,15 +334,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function uses_runstate.<locals>.<lambda> at 0x10424b250>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -356,18 +357,36 @@
 
 *Property `RunStateMixin.stopped`*:
 Test .runstate.stopped.
 
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
+## Function `uses_runstate(*da, **dkw)`
+
+A wrapper for `@default_params` which makes a new thread wide
+`RunState` parameter `runstate` if missing.
+The optional decorator parameter `name` may be used to specify
+a name for the new `RunState` if one is made. The default
+comes from the wrapped function's name.
+
+Example:
+
+    @uses_runstate
+    def do_something(blah, *, runstate:RunState):
+        ... do something, polling the runstate as approriate ...
+
 # Release Log
 
 
 
+*Release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
+
 *Release 20240519*:
 RunState now subclasses cs.fsm.FSM.
 
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
```

### Comparing `cs.resources-20240519/lib/python/cs/resources.py` & `cs.resources-20240522/lib/python/cs/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,26 @@
 from threading import Lock, current_thread, main_thread
 import time
 from typing import Any, Callable, Mapping, Optional, Tuple, Union
 
 from typeguard import typechecked
 
 from cs.context import contextif, stackattrs, setup_cmgr, ContextManagerMixin
-from cs.deco import default_params, OBSOLETE
+from cs.deco import decorator, default_params, OBSOLETE
 from cs.fsm import FSM
 from cs.gimmicks import error, warning, nullcontext
 from cs.obj import Proxy
 from cs.pfx import pfx_call, pfx_method
 from cs.psutils import signal_handlers
+from cs.py.func import funccite
 from cs.py.stack import caller, frames as stack_frames, StackSummary
 from cs.result import CancellationError
 from cs.threads import ThreadState, HasThreadState, NRLock
 
-__version__ = '20240519'
+__version__ = '20240522'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
@@ -41,14 +42,15 @@
         'cs.context',
         'cs.deco',
         'cs.fsm',
         'cs.gimmicks',
         'cs.obj',
         'cs.pfx',
         'cs.psutils',
+        'cs.py.func',
         'cs.py.stack',
         'cs.result',
         'cs.threads',
         'typeguard',
     ],
 }
 
@@ -687,15 +689,18 @@
 
         On `'cancel'` set the cancelled flag.
         On `'start'` clear the cancelled flag and set `.start_time`.
         On `'stop'`set `.stop_time`.
     '''
     new_state = super().fsm_event(event, **extra)
     if event == 'cancel':
-      self._canceled = True
+      self._cancelled = True
+      # TODO: use the main FSM callback mechanism
+      for notify in self.notify_cancel:
+        notify(self)
     elif event == 'start':
       self._cancelled = False
       self.start_time = time.time()
       self._started_from = stack_frames()
     elif event == 'stop':
       self.stop_time = time.time()
     return new_state
@@ -742,20 +747,14 @@
       return True
     if self.poll_cancel:
       if self.poll_cancel():
         self._cancelled = True
         return True
     return False
 
-  @cancelled.setter
-  def cancelled(self, cancel_status):
-    ''' Set the .cancelled attribute.
-    '''
-    self._cancelled = cancel_status
-
   def raiseif(self, msg=None, *a):
     ''' Raise `CancellationError` if cancelled.
         This is the concise way to terminate an operation which honour
         `.cancelled` if you're prepared to handle the exception.
 
         Example:
 
@@ -783,27 +782,25 @@
     '''
     return self.fsm_state == 'STOPPING'
 
   def cancel(self):
     ''' Set the cancelled flag; the associated process should notice and stop.
     '''
     self.fsm_event('cancel')
-    for notify in self.notify_cancel:
-      notify(self)
 
   @property
   def run_time(self):
     ''' Property returning most recent run time (`stop_time-start_time`).
         If still running, use now as the stop time.
         If not started, return `0.0`.
     '''
     start_time = self.start_time
     if start_time is None:
       return 0.0
-    if self.is_running:
+    if self.is_running or self.stop_time is None:
       stop_time = time.time()
     else:
       stop_time = self.stop_time
     return max(0, stop_time - start_time)
 
   def iter(self, it):
     ''' Iterate over `it` while not `self.cancelled`.
@@ -847,19 +844,37 @@
         Warn if `self.verbose`.
       '''
     # pylint: disable=expression-not-assigned
     if self.verbose:
       warning("%s: received signal %s, cancelling", self, sig)
     self.cancel()
 
-# default to the current RunState or make one
-uses_runstate = default_params(
-    runstate=lambda:
-    (RunState.default(factory=partial(RunState, thread_wide=True)))
-)
+@decorator
+def uses_runstate(func, name=None):
+  ''' A wrapper for `@default_params` which makes a new thread wide
+      `RunState` parameter `runstate` if missing.
+      The optional decorator parameter `name` may be used to specify
+      a name for the new `RunState` if one is made. The default
+      comes from the wrapped function's name.
+
+      Example:
+
+          @uses_runstate
+          def do_something(blah, *, runstate:RunState):
+              ... do something, polling the runstate as approriate ...
+  '''
+  if name is None:
+    name = funccite(func)
+  return default_params(
+      func,
+      runstate=lambda: (
+          RunState.
+          default(factory=partial(RunState, name=name, thread_wide=True))
+      )
+  )
 
 class RunStateMixin(object):
   ''' Mixin to provide convenient access to a `RunState`.
 
       Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
   '''
```

### Comparing `cs.resources-20240519/lib/python/cs.resources.egg-info/PKG-INFO` & `cs.resources-20240522/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.resources
-Version: 20240519
+Version: 20240522
 Summary: Resource management classes and functions.
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
@@ -14,16 +14,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 Resource management classes and functions.
 
-*Latest release 20240519*:
-RunState now subclasses cs.fsm.FSM.
+*Latest release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -351,15 +352,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function uses_runstate.<locals>.<lambda> at 0x10424b250>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -374,18 +375,36 @@
 
 *Property `RunStateMixin.stopped`*:
 Test .runstate.stopped.
 
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
+## Function `uses_runstate(*da, **dkw)`
+
+A wrapper for `@default_params` which makes a new thread wide
+`RunState` parameter `runstate` if missing.
+The optional decorator parameter `name` may be used to specify
+a name for the new `RunState` if one is made. The default
+comes from the wrapped function's name.
+
+Example:
+
+    @uses_runstate
+    def do_something(blah, *, runstate:RunState):
+        ... do something, polling the runstate as approriate ...
+
 # Release Log
 
 
 
+*Release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
+
 *Release 20240519*:
 RunState now subclasses cs.fsm.FSM.
 
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
```

### Comparing `cs.resources-20240519/pyproject.toml` & `cs.resources-20240522/lib/python/cs.resources.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,30 @@
-[project]
-name = "cs.resources"
-description = "Resource management classes and functions."
-authors = [
-    { name = "Cameron Simpson", email = "cs@cskk.id.au" },
-]
-keywords = [
-    "python2",
-    "python3",
-]
-dependencies = [
-    "cs.context>=20240412",
-    "cs.deco>=20240412",
-    "cs.fsm>=20240519",
-    "cs.gimmicks>=20240316",
-    "cs.obj>=20220918",
-    "cs.pfx>=20240412",
-    "cs.psutils>=20240316",
-    "cs.py.stack>=20240519",
-    "cs.result>=20240412",
-    "cs.threads>=20240422",
-    "typeguard",
-]
-classifiers = [
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Development Status :: 4 - Beta",
-    "Intended Audience :: Developers",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
-version = "20240519"
+Metadata-Version: 2.1
+Name: cs.resources
+Version: 20240522
+Summary: Resource management classes and functions.
+Author-email: Cameron Simpson <cs@cskk.id.au>
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
+Keywords: python2,python3
+Platform: UNKNOWN
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Description-Content-Type: text/markdown
 
-[project.license]
-text = "GNU General Public License v3 or later (GPLv3+)"
-
-[project.urls]
-URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
-
-[project.readme]
-text = """
 Resource management classes and functions.
 
-*Latest release 20240519*:
-RunState now subclasses cs.fsm.FSM.
+*Latest release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
 
 ## Class `ClosedError(builtins.Exception)`
 
 Exception for operations invalid when something is closed.
 
 ## Class `MultiOpen(MultiOpenMixin)`
 
@@ -102,15 +79,15 @@
         def startup_shutdown(self):
             with open_the_database() as db:
                 self._db = db
                 yield
 
 Why not just write a plain context manager class? Because in
 multithreaded or async code one wants to keep the instance
-\"open\" while any thread is still using it.
+"open" while any thread is still using it.
 This mixin lets threads use an instance in overlapping fashion:
 
     db_thing = DatabaseThing(...)
     with db_thing:
         ... kick off threads with access to the db ...
     ...
     thread 1:
@@ -295,15 +272,15 @@
 * stop
 
 Note that if the `RunState` is already running we do not
 do any of that stuff apart from the `yield self` because
 we assume whatever setup should have been done has already
 been done.
 In particular, the `HasThreadState.Thread` factory calls this
-in the \"running\" state.
+in the "running" state.
 
 *Method `RunState.__nonzero__(self)`*:
 Return true if the task is running.
 
 *Method `RunState.cancel(self)`*:
 Set the cancelled flag; the associated process should notice and stop.
 
@@ -375,15 +352,15 @@
 
 ## Class `RunStateMixin`
 
 Mixin to provide convenient access to a `RunState`.
 
 Provides: `.runstate`, `.cancelled`, `.running`, `.stopping`, `.stopped`.
 
-*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function <lambda> at 0x10ecf9f30>)`*:
+*Method `RunStateMixin.__init__(self, *, runstate: Union[cs.resources.RunState, str, NoneType] = <function uses_runstate.<locals>.<lambda> at 0x10424b250>)`*:
 Initialise the `RunStateMixin`; sets the `.runstate` attribute.
 
 Parameters:
 * `runstate`: optional `RunState` instance or name.
   If a `str`, a new `RunState` with that name is allocated.
   If omitted, the default `RunState` is used.
 
@@ -398,18 +375,36 @@
 
 *Property `RunStateMixin.stopped`*:
 Test .runstate.stopped.
 
 *Property `RunStateMixin.stopping`*:
 Test .runstate.stopping.
 
+## Function `uses_runstate(*da, **dkw)`
+
+A wrapper for `@default_params` which makes a new thread wide
+`RunState` parameter `runstate` if missing.
+The optional decorator parameter `name` may be used to specify
+a name for the new `RunState` if one is made. The default
+comes from the wrapped function's name.
+
+Example:
+
+    @uses_runstate
+    def do_something(blah, *, runstate:RunState):
+        ... do something, polling the runstate as approriate ...
+
 # Release Log
 
 
 
+*Release 20240522*:
+* @uses_runstate: if we make a new RunState, get the default name from the wrapped function.
+* RunState: bug fixes from the recent subclassing of cs.fsm.FSM.
+
 *Release 20240519*:
 RunState now subclasses cs.fsm.FSM.
 
 *Release 20240423*:
 RunStateMixin: make the optional runstate parameter keyword only.
 
 *Release 20240422*:
@@ -473,15 +468,15 @@
 * MultiOpenMixin.startup_shutdown: fix up shutdown logic, was not using a finally clause.
 * MultiOpenMixin: use ContextManagerMixin __enter_exit__ generator method instead of __enter__ and __exit__.
 
 *Release 20210906*:
 MultiOpenMixin: make startup and shutdown optional.
 
 *Release 20210731*:
-RunState: tune the sanity checks around whether the state is \"running\".
+RunState: tune the sanity checks around whether the state is "running".
 
 *Release 20210420*:
 MultiOpenMixin: run startup/shutdown entirely via the new default method @contextmanager(startup_shutdown), paving the way for subclasses to just define their own startup_shutdown context manager methods instead of distinct startup/shutdown methods.
 
 *Release 20201025*:
 MultiOpenMixin.__mo_getstate: dereference self.__dict__ because using AttributeError was pulling a state object from another instance, utterly weird.
 
@@ -507,33 +502,17 @@
 * RunState improvements.
 
 *Release 20171024*:
 * bugfix MultiOpenMixin finalise logic and other small logic fixes and checs
 * new class RunState for tracking or controlling a running task
 
 *Release 20160828*:
-Use \"install_requires\" instead of \"requires\" in DISTINFO.
+Use "install_requires" instead of "requires" in DISTINFO.
 
 *Release 20160827*:
 * BREAKING CHANGE: rename NestingOpenCloseMixin to MultiOpenMixin.
 * New Pool class for generic object reuse.
 * Assorted minor improvements.
 
 *Release 20150115*:
-First PyPI release."""
-content-type = "text/markdown"
-
-[build-system]
-build-backend = "setuptools.build_meta"
-requires = [
-    "setuptools >= 61.2",
-    "trove-classifiers",
-    "wheel",
-]
-
-[tool.setuptools]
-py-modules = [
-    "cs.resources",
-]
+First PyPI release.
 
-[tool.setuptools.package-dir]
-"" = "lib/python"
```

