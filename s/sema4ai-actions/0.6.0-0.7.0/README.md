# Comparing `tmp/sema4ai_actions-0.6.0.tar.gz` & `tmp/sema4ai_actions-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sema4ai_actions-0.6.0.tar", max compression
+gzip compressed data, was "sema4ai_actions-0.7.0.tar", max compression
```

## Comparing `sema4ai_actions-0.6.0.tar` & `sema4ai_actions-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2971 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/README.md
--rw-r--r--   0        0        0      971 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5508 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/__init__.py
--rw-r--r--   0        0        0       80 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/__main__.py
--rw-r--r--   0        0        0    15553 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_action.py
--rw-r--r--   0        0        0     7567 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_action_context.py
--rw-r--r--   0        0        0    11151 2024-05-16 19:14:01.084860 sema4ai_actions-0.6.0/src/sema4ai/actions/_args_dispatcher.py
--rw-r--r--   0        0        0     1494 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_callback.py
--rw-r--r--   0        0        0     8339 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_collect_actions.py
--rw-r--r--   0        0        0    32316 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_commands.py
--rw-r--r--   0        0        0     2276 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_config.py
--rw-r--r--   0        0        0      336 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_constants.py
--rw-r--r--   0        0        0        0 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/__init__.py
--rw-r--r--   0        0        0     2722 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_extension_points.py
--rw-r--r--   0        0        0     9922 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_plugin_manager.py
--rw-r--r--   0        0        0      220 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_exceptions.py
--rw-r--r--   0        0        0     5638 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_fixtures.py
--rw-r--r--   0        0        0     2500 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_hooks.py
--rw-r--r--   0        0        0     7491 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_interrupts.py
--rw-r--r--   0        0        0     1367 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_lifecycle.py
--rw-r--r--   0        0        0    13368 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_lint_action.py
--rw-r--r--   0        0        0     1082 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_log_auto_setup.py
--rw-r--r--   0        0        0     3074 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_log_output_setup.py
--rw-r--r--   0        0        0     6342 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_managed_parameters.py
--rw-r--r--   0        0        0     6023 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_protocols.py
--rw-r--r--   0        0        0    13813 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_remove_refs.py
--rw-r--r--   0        0        0     2906 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_request.py
--rw-r--r--   0        0        0     1023 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_request_impl.py
--rw-r--r--   0        0        0     6615 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/__init__.py
--rw-r--r--   0        0        0     5153 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_oauth2_secret.py
--rw-r--r--   0        0        0     2678 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_secret.py
--rw-r--r--   0        0        0     3134 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/api.py
--rw-r--r--   0        0        0     2277 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/cli.py
--rw-r--r--   0        0        0        0 2024-05-16 19:14:01.088860 sema4ai_actions-0.6.0/src/sema4ai/actions/py.typed
--rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2971 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/README.md
+-rw-r--r--   0        0        0      971 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     5508 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/__main__.py
+-rw-r--r--   0        0        0    16339 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_action.py
+-rw-r--r--   0        0        0     7567 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_action_context.py
+-rw-r--r--   0        0        0    11652 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_args_dispatcher.py
+-rw-r--r--   0        0        0     1494 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_callback.py
+-rw-r--r--   0        0        0     8339 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_collect_actions.py
+-rw-r--r--   0        0        0    33643 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_commands.py
+-rw-r--r--   0        0        0     2276 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_config.py
+-rw-r--r--   0        0        0      336 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_constants.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/__init__.py
+-rw-r--r--   0        0        0     2722 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_extension_points.py
+-rw-r--r--   0        0        0     9922 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_plugin_manager.py
+-rw-r--r--   0        0        0      220 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_exceptions.py
+-rw-r--r--   0        0        0     5638 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_fixtures.py
+-rw-r--r--   0        0        0     2500 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_hooks.py
+-rw-r--r--   0        0        0     7491 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_interrupts.py
+-rw-r--r--   0        0        0     1367 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_lifecycle.py
+-rw-r--r--   0        0        0    13368 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_lint_action.py
+-rw-r--r--   0        0        0     1082 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_log_auto_setup.py
+-rw-r--r--   0        0        0     3074 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_log_output_setup.py
+-rw-r--r--   0        0        0     6342 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_managed_parameters.py
+-rw-r--r--   0        0        0     6023 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_protocols.py
+-rw-r--r--   0        0        0    13813 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_remove_refs.py
+-rw-r--r--   0        0        0     2906 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_request.py
+-rw-r--r--   0        0        0     1023 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_request_impl.py
+-rw-r--r--   0        0        0     6615 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/__init__.py
+-rw-r--r--   0        0        0     5153 2024-05-22 11:54:50.419717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_oauth2_secret.py
+-rw-r--r--   0        0        0     2678 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_secret.py
+-rw-r--r--   0        0        0     3134 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/api.py
+-rw-r--r--   0        0        0     2277 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 11:54:50.423717 sema4ai_actions-0.7.0/src/sema4ai/actions/py.typed
+-rw-r--r--   0        0        0     3788 1970-01-01 00:00:00.000000 sema4ai_actions-0.7.0/PKG-INFO
```

### Comparing `sema4ai_actions-0.6.0/README.md` & `sema4ai_actions-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/pyproject.toml` & `sema4ai_actions-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sema4ai-actions"
-version = "0.6.0"
+version = "0.7.0"
 description = "Sema4AI Actions"
 authors = [
 	"Fabio Z. <fabio@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/Sema4AI/actions/"
 license = "Apache-2.0"
```

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/__init__.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from typing import Callable, Optional, overload
 
 from ._fixtures import setup, teardown
 from ._protocols import IAction, Status
 from ._request import Request
 from ._secret import OAuth2Secret, Secret
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 
 @overload
 def action(func: Callable) -> Callable:
     ...
```

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_action.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_action.py`

 * *Files 6% similar despite different names*

```diff
@@ -331,16 +331,17 @@
 
     # Some user message which was being sent to the stdout.
     KIND_STDOUT = ConsoleMessageKind.STDOUT
 
     # Some user message which was being sent to the stderr.
     KIND_STDERR = ConsoleMessageKind.STDERR
 
-    def __init__(self):
+    def __init__(self, print_result: bool = False):
         self._msg_len_target = 80
+        self._print_result = print_result
 
     def _show_header(self, parts: List[Tuple[str, str]]) -> int:
         """
         Returns:
             The final number of chars used in the full header.
         """
         if not parts:
@@ -396,28 +397,33 @@
     def _before_action_run(self, action: IAction):
         self._msg_len_target = 80
         self._msg_len_target = self._show_header(
             [("Running: ", self.KIND_REGULAR), (action.name, self.KIND_TASK_NAME)]
         )
 
     def _after_action_run(self, action: IAction):
+        import json
         import traceback
 
         msg = ""
         if action.message:
             msg = f"\n{action.message}"
 
         status_kind = self.KIND_REGULAR
         if action.status == Status.FAIL:
             status_kind = self.KIND_ERROR
 
         show = self.show
+
+        result = action.result
+
         show(f"{action.name}", end="", kind=self.KIND_TASK_NAME)
         show(" status: ", end="")
         show(f"{action.status.value}", kind=status_kind)
+
         if msg:
             show(f"{msg}", kind=status_kind)
 
             if action.exc_info and action.exc_info[0]:
                 self._show_header(
                     [
                         ("Full Traceback (running ", self.KIND_REGULAR),
@@ -427,14 +433,32 @@
                 )
 
                 self.show(
                     "".join(traceback.format_exception(*action.exc_info)),
                     kind=self.KIND_TRACEBACK,
                 )
 
+        if self._print_result and action.status == Status.PASS:
+            show("result:", kind=self.KIND_IMPORTANT)
+            try:
+                if hasattr(result, "model_dump_json"):
+                    # Support for pydantic
+                    result_as_json_str = result.model_dump_json(indent=4)
+                else:
+                    result_as_json_str = json.dumps(result, indent=4)
+            except Exception:
+                raise RuntimeError(
+                    "The resulting value: {result} cannot be converted to JSON."
+                )
+
+            show(
+                result_as_json_str,
+                flush=True,
+            )
+
         self._show_header([])
 
     @contextmanager
     def register_lifecycle_prints(self):
         from sema4ai.actions._hooks import after_action_run, before_action_run
 
         with before_action_run.register(
```

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_action_context.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_action_context.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_args_dispatcher.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_args_dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,28 @@
         run_parser.add_argument(
             "--os-exit",
             dest="os_exit",
             type=str,
             choices=["no", "before-teardown", "after-teardown"],
             help="Can be used to do an early os._exit to avoid the actions session teardown or the interpreter teardown. Not recommended in general.",
         )
+        run_parser.add_argument(
+            "--print-input",
+            dest="print_input",
+            action="store_true",
+            default=False,
+            help="Can be used to see the input of the actions run in the terminal.",
+        )
+        run_parser.add_argument(
+            "--print-result",
+            dest="print_result",
+            action="store_true",
+            default=False,
+            help="Can be used to see the result of the actions run in the terminal.",
+        )
 
         return run_parser
 
     def _create_list_actions_parser(self, main_parser):
         # List actions
         list_parser = main_parser.add_parser(
             "list",
```

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_callback.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_callback.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_collect_actions.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_collect_actions.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_commands.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,21 +164,23 @@
     teardown_interrupt_timeout: Optional[float] = None,
     os_exit: Optional[str] = None,
     additional_arguments: Optional[List[str]] = None,
     preload_module: Optional[List[str]] = None,
     glob: Optional[str] = None,
     json_input: Optional[str] = None,
     pm: Optional[PluginManager] = None,
+    print_input: bool = False,
+    print_result: bool = False,
 ) -> int:
     """
     Runs an action.
 
     Args:
         output_dir: The directory where output should be put.
-        path: The path (file or directory where the actions should be collected from.
+        path: The file or directory where the actions should be collected from.
         action_name: The name(s) of the action to run.
         max_log_files: The maximum number of log files to be created (if more would
             be needed the oldest one is deleted).
         max_log_file_size: The maximum size for the created log files.
         console_colors:
             "auto": uses the default console
             "plain": disables colors
@@ -213,22 +215,32 @@
             'after-teardown' means that the process will exit right after the
                 actions session teardown takes place.
         additional_arguments: The arguments passed to the action.
         preload_module: The modules which should be pre-loaded (i.e.: loaded
             after the logging is in place but before any other action is collected).
         glob: A glob to define from which module names the actions should be loaded.
         json_input: The path to a json file to be loaded to get the arguments.
+        print_input: If set the input passed to an @action will be shown
+            in the console (note that even if false it should be also added to the
+            `log.html`).
+        print_result: If set the result generated by running an @action will be shown
+            in the console (note that even if false it should be also added to the
+            `log.html`).
 
     Returns:
         0 if everything went well.
         1 if there was some error running the action.
     """
+    # If it's set it'll only consider files under the ROBOT_ROOT to contain user code
+    # we leave it unset so that it considers all files under lib or site-packages as
+    # lib code and everything else is user code.
+    os.environ.pop("ROBOT_ROOT", None)
     import copy
 
-    from robocorp.log import console, redirect
+    from robocorp.log import ConsoleMessageKind, console, redirect
     from robocorp.log.pyproject_config import (
         read_pyproject_toml,
         read_robocorp_auto_log_config,
     )
 
     from sema4ai.actions._action import Context, set_current_action
     from sema4ai.actions._collect_actions import collect_actions
@@ -261,15 +273,15 @@
 
     # Don't show internal machinery on tracebacks:
     # setting __tracebackhide__ will make it so that robocorp-log
     # won't show this frame onwards in the logging.
     __tracebackhide__ = 1
 
     p = Path(path).absolute()
-    context = Context()
+    context = Context(print_result=print_result)
     if not p.exists():
         context.show_error(f"Path: {path} does not exist")
         return 1
 
     if teardown_dump_threads_timeout is None:
         v = os.getenv("RC_TEARDOWN_DUMP_THREADS_TIMEOUT", "5")
 
@@ -448,14 +460,25 @@
                 before_all_actions_run(actions)
 
                 try:
                     for action in actions:
                         set_current_action(action)
                         before_action_run(action)
                         try:
+                            if print_input and json_loaded_arguments is not None:
+                                input_as_json_str = json.dumps(
+                                    json_loaded_arguments, indent=4
+                                )
+                                context.show(
+                                    "input:", kind=ConsoleMessageKind.IMPORTANT
+                                )
+                                context.show(
+                                    input_as_json_str,
+                                    flush=True,
+                                )
                             if json_loaded_arguments is not None:
                                 kwargs = copy.deepcopy(json_loaded_arguments)
                                 kwargs = _validate_and_convert_kwargs(
                                     pm, action, kwargs
                                 )
 
                             else:
```

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_config.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_config.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_extension_points.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_extension_points.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_customization/_plugin_manager.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_customization/_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_fixtures.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_fixtures.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_hooks.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_hooks.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_interrupts.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_interrupts.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_lifecycle.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_lifecycle.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_lint_action.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_lint_action.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_log_auto_setup.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_log_auto_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_log_output_setup.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_managed_parameters.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_managed_parameters.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_protocols.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_protocols.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_remove_refs.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_remove_refs.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_request.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_request.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_request_impl.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_request_impl.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/__init__.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/__init__.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_oauth2_secret.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_oauth2_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/_secret/_secret.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/_secret/_secret.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/api.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/api.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/src/sema4ai/actions/cli.py` & `sema4ai_actions-0.7.0/src/sema4ai/actions/cli.py`

 * *Files identical despite different names*

### Comparing `sema4ai_actions-0.6.0/PKG-INFO` & `sema4ai_actions-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sema4ai-actions
-Version: 0.6.0
+Version: 0.7.0
 Summary: Sema4AI Actions
 Home-page: https://github.com/Sema4AI/actions/
 License: Apache-2.0
 Author: Fabio Z.
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

