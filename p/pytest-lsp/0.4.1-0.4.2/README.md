# Comparing `tmp/pytest_lsp-0.4.1.tar.gz` & `tmp/pytest_lsp-0.4.2.tar.gz`

## Comparing `pytest_lsp-0.4.1.tar` & `pytest_lsp-0.4.2.tar`

### file list

```diff
@@ -1,61 +1,63 @@
--rw-r--r--   0        0        0     7970 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/CHANGES.md
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/__init__.py
--rw-r--r--   0        0        0     8274 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/checks.py
--rw-r--r--   0        0        0    13968 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/client.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/plugin.py
--rw-r--r--   0        0        0     3830 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/py.typed
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/__init__.py
--rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/emacs_v29.1.json
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.6.1.json
--rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.7.0.json
--rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.8.0.json
--rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.9.1.json
--rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pytest_lsp/clients/visual_studio_code_v1.65.2.json
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/test_checks.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/test_client.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/test_examples.py
--rw-r--r--   0        0        0     6518 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/test_plugin.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/client-capabilities/server.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/client-capabilities/t_server.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/diagnostics/server.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/diagnostics/t_server.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/fixture-passthrough/server.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/fixture-passthrough/t_server.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/fixture-scope/server.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/fixture-scope/t_server.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/generic-rpc/server.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/generic-rpc/t_server.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/getting-started/server.py
--rw-r--r--   0        0        0     1349 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/getting-started/t_server.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/getting-started-fail/server.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/getting-started-fail/t_server.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/parameterised-clients/server.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/parameterised-clients/t_server.py
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/server-stderr/server.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/server-stderr/t_server.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-create-progress/server.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-create-progress/t_server.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-log-message/server.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-log-message/t_server.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-log-message-fail/server.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-log-message-fail/t_server.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-show-document/server.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-show-document/t_server.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-show-message/server.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/window-show-message/t_server.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/workspace-configuration/server.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/examples/workspace-configuration/t_server.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/servers/capabilities.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/servers/completion_exit.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/servers/crash.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/servers/hello.py
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/tests/servers/invalid_json.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/LICENSE
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/README.md
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/hatch.toml
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pytest_lsp-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     8234 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/CHANGES.md
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/__init__.py
+-rw-r--r--   0        0        0     8269 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/checks.py
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/client.py
+-rw-r--r--   0        0        0     6227 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/plugin.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/py.typed
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/__init__.py
+-rw-r--r--   0        0        0     3820 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/emacs_v29.1.json
+-rw-r--r--   0        0        0     6859 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.10.0.json
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.6.1.json
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.7.0.json
+-rw-r--r--   0        0        0     4851 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.8.0.json
+-rw-r--r--   0        0        0     6021 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.9.1.json
+-rw-r--r--   0        0        0     8458 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pytest_lsp/clients/visual_studio_code_v1.65.2.json
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0     7744 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/test_checks.py
+-rw-r--r--   0        0        0     6813 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/test_client.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/test_examples.py
+-rw-r--r--   0        0        0     6472 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/test_plugin.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/ruff.toml
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/client-capabilities/server.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/client-capabilities/t_server.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/diagnostics/server.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/diagnostics/t_server.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/fixture-passthrough/server.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/fixture-passthrough/t_server.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/fixture-scope/server.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/fixture-scope/t_server.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/generic-rpc/server.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/generic-rpc/t_server.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/getting-started/server.py
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/getting-started/t_server.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/getting-started-fail/server.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/getting-started-fail/t_server.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/parameterised-clients/server.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/parameterised-clients/t_server.py
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/server-stderr/server.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/server-stderr/t_server.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-create-progress/server.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-create-progress/t_server.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-log-message/server.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-log-message/t_server.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-log-message-fail/server.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-log-message-fail/t_server.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-show-document/server.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-show-document/t_server.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-show-message/server.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/window-show-message/t_server.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/workspace-configuration/server.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/examples/workspace-configuration/t_server.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/servers/capabilities.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/servers/completion_exit.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/servers/crash.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/servers/hello.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/tests/servers/invalid_json.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/README.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/hatch.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 pytest_lsp-0.4.2/PKG-INFO
```

### Comparing `pytest_lsp-0.4.1/CHANGES.md` & `pytest_lsp-0.4.2/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+## v0.4.2 - 2024-05-22
+
+
+### Client Capabilities
+
+- Add client capabilities for Neovim v0.10.0 ([#164](https://github.com/swyddfa/lsp-devtools/issues/164))
+
+### Misc
+
+- Start testing against pytest v8 ([#145](https://github.com/swyddfa/lsp-devtools/issues/145))
+
+
 ## v0.4.1 - 2024-02-07
 
 
 ### Enhancements
 
 - When a test fails `pytest-lsp` will now show the server's `stderr` output (if any) ([#143](https://github.com/swyddfa/lsp-devtools/issues/143))
```

### Comparing `pytest_lsp-0.4.1/pytest_lsp/__init__.py` & `pytest_lsp-0.4.2/pytest_lsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/checks.py` & `pytest_lsp-0.4.2/pytest_lsp/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 However, they are also called automatically during end-to-end tests that make use of the
 standard :class:`~pytest_lsp.LanguageClient`. See :ref:`pytest-lsp-spec-checks` for more
 details.
 
 """
 
+# ruff: noqa: S101
 import logging
 import warnings
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import List
 from typing import Optional
@@ -34,28 +35,28 @@
     """Warning raised when encountering results that fall outside the spec."""
 
 
 def check_result_for(*, method: str) -> Callable[[ResultChecker], ResultChecker]:
     """Define a result check."""
 
     def defcheck(fn: ResultChecker):
-        if (existing := RESULT_CHECKS.get(method, None)) is not None:
+        if (existing := RESULT_CHECKS.get(method)) is not None:
             raise ValueError(f"{fn!r} conflicts with existing check {existing!r}")
 
         RESULT_CHECKS[method] = fn
         return fn
 
     return defcheck
 
 
 def check_params_of(*, method: str) -> Callable[[ParamsChecker], ParamsChecker]:
     """Define a params check."""
 
     def defcheck(fn: ParamsChecker):
-        if (existing := PARAMS_CHECKS.get(method, None)) is not None:
+        if (existing := PARAMS_CHECKS.get(method)) is not None:
             raise ValueError(f"{fn!r} conflicts with existing check {existing!r}")
 
         PARAMS_CHECKS[method] = fn
         return fn
 
     return defcheck
 
@@ -82,15 +83,15 @@
     if capabilities is None:
         raise RuntimeError("Client has not been initialized")
 
     # Only run checks if the user provided some capabilities for the client.
     if capabilities == types.ClientCapabilities():
         return
 
-    result_checker = RESULT_CHECKS.get(method, None)
+    result_checker = RESULT_CHECKS.get(method)
     if result_checker is None:
         return
 
     try:
         result_checker(capabilities, result)
     except AssertionError as e:
         warnings.warn(str(e), LspSpecificationWarning, stacklevel=4)
@@ -117,15 +118,15 @@
     if capabilities is None:
         raise RuntimeError("Client has not been initialized")
 
     # Only run checks if the user provided some capabilities for the client.
     if capabilities == types.ClientCapabilities():
         return
 
-    params_checker = PARAMS_CHECKS.get(method, None)
+    params_checker = PARAMS_CHECKS.get(method)
     if params_checker is None:
         return
 
     try:
         params_checker(capabilities, params)
     except AssertionError as e:
         warnings.warn(str(e), LspSpecificationWarning, stacklevel=2)
```

### Comparing `pytest_lsp-0.4.1/pytest_lsp/client.py` & `pytest_lsp-0.4.2/pytest_lsp/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+from __future__ import annotations
+
 import asyncio
 import json
 import logging
 import os
 import pathlib
 import sys
 import traceback
 import typing
 import warnings
-from typing import Any
-from typing import Dict
-from typing import List
-from typing import Optional
-from typing import Type
-from typing import Union
 
 from lsprotocol import types
 from lsprotocol.converters import get_converter
 from packaging.version import parse as parse_version
 from pygls.exceptions import JsonRpcException
 from pygls.exceptions import PyglsError
 from pygls.lsp.client import BaseLanguageClient
 from pygls.protocol import default_converter
 
 from .checks import LspSpecificationWarning
 from .protocol import LanguageClientProtocol
 
-if sys.version_info.minor < 9:
+if sys.version_info < (3, 9):
     import importlib_resources as resources
 else:
-    import importlib.resources as resources  # type: ignore[no-redef]
+    from importlib import resources  # type: ignore[no-redef]
+
+if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import Dict
+    from typing import List
+    from typing import Optional
+    from typing import Type
+    from typing import Union
 
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 logger = logging.getLogger(__name__)
 
 
 class LanguageClient(BaseLanguageClient):
     """Used to drive language servers under test."""
 
     protocol: LanguageClientProtocol
@@ -57,17 +61,17 @@
 
         self.log_messages: List[types.LogMessageParams] = []
         """Holds any received ``window/logMessage`` requests."""
 
         self.diagnostics: Dict[str, List[types.Diagnostic]] = {}
         """Holds any recieved diagnostics."""
 
-        self.progress_reports: Dict[types.ProgressToken, List[types.ProgressParams]] = (
-            {}
-        )
+        self.progress_reports: Dict[
+            types.ProgressToken, List[types.ProgressParams]
+        ] = {}
         """Holds any received progress updates."""
 
         self.error: Optional[Exception] = None
         """Indicates if the client encountered an error."""
 
         config = (configuration or {"": {}}).copy()
         if "" not in config:
@@ -279,15 +283,15 @@
         sys.stderr.buffer.write(line)
 
 
 def cancel_all_tasks(message: str):
     """Called to cancel all awaited tasks."""
 
     for task in asyncio.all_tasks():
-        if sys.version_info.minor < 9:
+        if sys.version_info < (3, 9):
             task.cancel()
         else:
             task.cancel(message)
 
 
 def make_test_lsp_client() -> LanguageClient:
     """Construct a new test client instance with the handlers needed to capture
@@ -314,25 +318,28 @@
     def create_work_done_progress(
         client: LanguageClient, params: types.WorkDoneProgressCreateParams
     ):
         if params.token in client.progress_reports:
             # TODO: Send an error reponse to the client - might require changes
             #       to pygls...
             warnings.warn(
-                f"Duplicate progress token: {params.token!r}", LspSpecificationWarning
+                f"Duplicate progress token: {params.token!r}",
+                LspSpecificationWarning,
+                stacklevel=2,
             )
 
         client.progress_reports.setdefault(params.token, [])
-        return None
 
     @client.feature(types.PROGRESS)
     def progress(client: LanguageClient, params: types.ProgressParams):
         if params.token not in client.progress_reports:
             warnings.warn(
-                f"Unknown progress token: {params.token!r}", LspSpecificationWarning
+                f"Unknown progress token: {params.token!r}",
+                LspSpecificationWarning,
+                stacklevel=2,
             )
 
         if not params.value:
             return
 
         if (kind := params.value.get("kind", None)) == "begin":
             type_: Type[Any] = types.WorkDoneProgressBegin
@@ -408,15 +415,15 @@
         if target_version.startswith("v"):
             target_version = target_version[1:]
 
     for resource in resources.files("pytest_lsp.clients").iterdir():
         filename = typing.cast(pathlib.Path, resource)
 
         # Skip the README or any other files that we don't care about.
-        if not filename.suffix == ".json":
+        if filename.suffix != ".json":
             continue
 
         name, version = filename.stem.split("_v")
         if name == client_spec:
             if version.startswith(target_version) or target_version == "latest":
                 candidates[version] = filename
```

### Comparing `pytest_lsp-0.4.1/pytest_lsp/plugin.py` & `pytest_lsp-0.4.2/pytest_lsp/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+from __future__ import annotations
+
 import inspect
 import logging
 import sys
 import textwrap
 import typing
-from typing import Any
-from typing import Callable
-from typing import Dict
-from typing import List
-from typing import Optional
 
 import attrs
 import pytest
 import pytest_asyncio
 from pygls.client import JsonRPCClient
 
 from pytest_lsp.client import LanguageClient
 from pytest_lsp.client import make_test_lsp_client
 
+if typing.TYPE_CHECKING:
+    from typing import Any
+    from typing import Callable
+    from typing import Dict
+    from typing import List
+    from typing import Optional
+
+
 logger = logging.getLogger("client")
 
 
 @attrs.define
 class ClientServerConfig:
     """Configuration for a Client-Server connection."""
 
@@ -124,17 +129,17 @@
     ]
 
     if len(messages) > 0:
         item.add_report_section(call.when, "window/logMessages", "\n".join(messages))
 
 
 # anext() was added in 3.10
-if sys.version_info.minor < 10:
+if sys.version_info < (3, 10):
 
-    async def anext(it):
+    async def anext(it):  # noqa: A001
         return await it.__anext__()
 
 
 def get_fixture_arguments(
     fn: Callable,
     client: JsonRPCClient,
     request: pytest.FixtureRequest,
```

### Comparing `pytest_lsp-0.4.1/pytest_lsp/protocol.py` & `pytest_lsp-0.4.2/pytest_lsp/protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
            The result
         """
         check_params_against_client_capabilities(
             self._server.capabilities, method, params
         )
         result = await super().send_request_async(method, params)
         check_result_against_client_capabilities(
-            self._server.capabilities, method, result  # type: ignore
+            self._server.capabilities,
+            method,
+            result,  # type: ignore
         )
 
         return result
 
     def wait_for_notification(self, method: str, callback=None) -> Future:
         """Wait for a notification message with the given ``method``.
```

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/README.md` & `pytest_lsp-0.4.2/pytest_lsp/clients/README.md`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/emacs_v29.1.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/emacs_v29.1.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.6.1.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.6.1.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.7.0.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.7.0.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.8.0.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.8.0.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/neovim_v0.9.1.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/neovim_v0.9.1.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pytest_lsp/clients/visual_studio_code_v1.65.2.json` & `pytest_lsp-0.4.2/pytest_lsp/clients/visual_studio_code_v1.65.2.json`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/test_checks.py` & `pytest_lsp-0.4.2/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/test_client.py` & `pytest_lsp-0.4.2/tests/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,16 +21,16 @@
             ["visual_studio_code_v1.65.2.json"],
         ),
         *itertools.product(
             ["neovim@0.6", "neovim@v0.6", "neovim@0.6.1"],
             ["neovim_v0.6.1.json"],
         ),
         *itertools.product(
-            ["neovim", "neovim@latest", "neovim@v0", "neovim@v0.9", "neovim@v0.9.1"],
-            ["neovim_v0.9.1.json"],
+            ["neovim", "neovim@latest", "neovim@v0", "neovim@v0.10", "neovim@v0.10.0"],
+            ["neovim_v0.10.0.json"],
         ),
     ],
 )
 def test_client_capabilities(
     pytester: pytest.Pytester, client_spec: str, capabilities: str
 ):
     """Ensure that the plugin can mimic the requested client's capabilities correctly.
```

### Comparing `pytest_lsp-0.4.1/tests/test_examples.py` & `pytest_lsp-0.4.2/tests/test_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,18 +98,18 @@
     """Ensure that the initial getting started example fails as expected."""
 
     setup_test(pytester, "getting-started-fail")
 
     results = pytester.runpytest()
     results.assert_outcomes(errors=1)
 
-    if sys.version_info.minor < 9:
+    if sys.version_info < (3, 9):
         message = "E*CancelledError"
     else:
-        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"  # noqa: E501
+        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"
 
     results.stdout.fnmatch_lines(message)
 
 
 def test_generic_rpc(pytester: pytest.Pytester):
     """Ensure that the generic rpc example works as expected"""
```

### Comparing `pytest_lsp-0.4.1/tests/test_plugin.py` & `pytest_lsp-0.4.2/tests/test_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,18 +125,18 @@
 """
 
     setup_test(pytester, "hello.py", test_code)
     results = pytester.runpytest("-vv")
 
     results.assert_outcomes(errors=1)
 
-    if sys.version_info.minor < 9:
+    if sys.version_info < (3, 9):
         message = "E*CancelledError"
     else:
-        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"  # noqa: E501
+        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"
 
     results.stdout.fnmatch_lines(message)
 
 
 def test_detect_server_exit_mid_request(pytester: pytest.Pytester):
     """Ensure that the plugin can detect when the server process exits mid request."""
 
@@ -161,18 +161,18 @@
 """
 
     setup_test(pytester, "completion_exit.py", test_code)
     results = pytester.runpytest("-vv")
 
     results.assert_outcomes(failed=1, errors=1)
 
-    if sys.version_info.minor < 9:
+    if sys.version_info < (3, 9):
         message = "E*CancelledError"
     else:
-        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"  # noqa: E501
+        message = "E*asyncio.exceptions.CancelledError: Server process exited with return code: 0"
 
     results.stdout.fnmatch_lines(message)
     results.stdout.fnmatch_lines("E*RuntimeError: Client has been stopped.")
 
 
 def test_detect_server_crash(pytester: pytest.Pytester):
     """Ensure the plugin can detect when the server process crashes on boot."""
@@ -186,19 +186,19 @@
 """
 
     setup_test(pytester, "crash.py", test_code)
     results = pytester.runpytest("-vv")
 
     results.assert_outcomes(errors=1)
 
-    if sys.version_info.minor < 9:
+    if sys.version_info < (3, 9):
         message = "E*CancelledError"
     else:
         message = [
-            "E*asyncio.exceptions.CancelledError: Server process exited with return code: 1",  # noqa: E501
+            "E*asyncio.exceptions.CancelledError: Server process exited with return code: 1",
             "ZeroDivisionError: division by zero",
         ]
 
     results.stdout.fnmatch_lines(message)
 
 
 def test_detect_invalid_json(pytester: pytest.Pytester):
@@ -226,13 +226,13 @@
 """
 
     setup_test(pytester, "invalid_json.py", test_code)
     results = pytester.runpytest("-vv")
 
     results.assert_outcomes(errors=1, failed=1)
 
-    if sys.version_info.minor < 9:
+    if sys.version_info < (3, 9):
         message = "E*CancelledError"
     else:
         message = "E*asyncio.exceptions.CancelledError: JsonRpcInternalError: *"
 
     results.stdout.fnmatch_lines(message)
```

### Comparing `pytest_lsp-0.4.1/tests/examples/client-capabilities/server.py` & `pytest_lsp-0.4.2/tests/examples/client-capabilities/server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from lsprotocol.types import TEXT_DOCUMENT_COMPLETION
-from lsprotocol.types import CompletionItem
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InsertTextFormat
+from lsprotocol.types import (
+    TEXT_DOCUMENT_COMPLETION,
+    CompletionItem,
+    CompletionParams,
+    InsertTextFormat,
+)
 from pygls.server import LanguageServer
 
 server = LanguageServer("hello-world", "v1")
 
 
 @server.feature(TEXT_DOCUMENT_COMPLETION)
 def completion(ls: LanguageServer, params: CompletionParams):
```

### Comparing `pytest_lsp-0.4.1/tests/examples/client-capabilities/t_server.py` & `pytest_lsp-0.4.2/tests/examples/client-capabilities/t_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import sys
 
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
-from pytest_lsp import client_capabilities
+from lsprotocol.types import (
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient, client_capabilities
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/examples/diagnostics/t_server.py` & `pytest_lsp-0.4.2/tests/examples/diagnostics/t_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import sys
 
-from lsprotocol.types import TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import DidOpenTextDocumentParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import TextDocumentItem
-
 import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    TEXT_DOCUMENT_PUBLISH_DIAGNOSTICS,
+    ClientCapabilities,
+    DidOpenTextDocumentParams,
+    InitializeParams,
+    TextDocumentItem,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/examples/fixture-passthrough/t_server.py` & `pytest_lsp-0.4.2/tests/examples/fixture-scope/t_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 import sys
 
 import pytest
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
-from pytest_lsp import client_capabilities
-
-
-@pytest.fixture(scope="module")
-def client_name():
-    return "neovim"
+from lsprotocol import types
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
+    scope="module",
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
-async def client(client_name: str, lsp_client: LanguageClient):
+async def client(lsp_client: LanguageClient):
     # Setup
-    params = InitializeParams(capabilities=client_capabilities(client_name))
+    params = types.InitializeParams(capabilities=types.ClientCapabilities())
     await lsp_client.initialize_session(params)
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
-async def test_completions(client: LanguageClient):
+@pytest.mark.asyncio(scope="module")
+async def test_completion_hello(client: LanguageClient):
+    """Ensure that the server implements completions correctly."""
+
+    results = await client.text_document_completion_async(
+        params=types.CompletionParams(
+            position=types.Position(line=1, character=0),
+            text_document=types.TextDocumentIdentifier(uri="file:///path/to/file.txt"),
+        )
+    )
+    assert results is not None
+
+    if isinstance(results, types.CompletionList):
+        items = results.items
+    else:
+        items = results
+
+    labels = {item.label for item in items}
+    assert "hello" in labels
+
+
+@pytest.mark.asyncio(scope="module")
+async def test_completion_world(client: LanguageClient):
     """Ensure that the server implements completions correctly."""
 
     results = await client.text_document_completion_async(
-        params=CompletionParams(
-            position=Position(line=1, character=0),
-            text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
+        params=types.CompletionParams(
+            position=types.Position(line=1, character=0),
+            text_document=types.TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
     assert results is not None
 
-    if isinstance(results, CompletionList):
+    if isinstance(results, types.CompletionList):
         items = results.items
     else:
         items = results
 
-    labels = [item.label for item in items]
-    assert labels == ["hello", "world"]
+    labels = {item.label for item in items}
+    assert "world" in labels
```

### Comparing `pytest_lsp-0.4.1/tests/examples/fixture-scope/t_server.py` & `pytest_lsp-0.4.2/tests/examples/getting-started/t_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,48 @@
 import sys
 
 import pytest
-from lsprotocol import types
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
-    scope="module",
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
-    params = types.InitializeParams(capabilities=types.ClientCapabilities())
+    params = InitializeParams(capabilities=ClientCapabilities())
     await lsp_client.initialize_session(params)
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
-@pytest.mark.asyncio(scope="module")
-async def test_completion_hello(client: LanguageClient):
-    """Ensure that the server implements completions correctly."""
-
-    results = await client.text_document_completion_async(
-        params=types.CompletionParams(
-            position=types.Position(line=1, character=0),
-            text_document=types.TextDocumentIdentifier(uri="file:///path/to/file.txt"),
-        )
-    )
-    assert results is not None
-
-    if isinstance(results, types.CompletionList):
-        items = results.items
-    else:
-        items = results
-
-    labels = {item.label for item in items}
-    assert "hello" in labels
-
-
-@pytest.mark.asyncio(scope="module")
-async def test_completion_world(client: LanguageClient):
+@pytest.mark.asyncio
+async def test_completions(client: LanguageClient):
     """Ensure that the server implements completions correctly."""
 
     results = await client.text_document_completion_async(
-        params=types.CompletionParams(
-            position=types.Position(line=1, character=0),
-            text_document=types.TextDocumentIdentifier(uri="file:///path/to/file.txt"),
+        params=CompletionParams(
+            position=Position(line=1, character=0),
+            text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
     assert results is not None
 
-    if isinstance(results, types.CompletionList):
+    if isinstance(results, CompletionList):
         items = results.items
     else:
         items = results
 
-    labels = {item.label for item in items}
-    assert "world" in labels
+    labels = [item.label for item in items]
+    assert labels == ["hello", "world"]
```

### Comparing `pytest_lsp-0.4.1/tests/examples/generic-rpc/server.py` & `pytest_lsp-0.4.2/tests/examples/generic-rpc/server.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/examples/generic-rpc/t_server.py` & `pytest_lsp-0.4.2/tests/examples/generic-rpc/t_server.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/examples/getting-started/t_server.py` & `pytest_lsp-0.4.2/tests/examples/server-stderr/t_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
@@ -23,26 +23,25 @@
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
-@pytest.mark.asyncio
 async def test_completions(client: LanguageClient):
-    """Ensure that the server implements completions correctly."""
-
     results = await client.text_document_completion_async(
         params=CompletionParams(
             position=Position(line=1, character=0),
             text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
+
     assert results is not None
 
     if isinstance(results, CompletionList):
         items = results.items
     else:
         items = results
 
     labels = [item.label for item in items]
-    assert labels == ["hello", "world"]
+    assert labels == [f"item-{i}" for i in range(10)]
+    pytest.fail("Failing test!")  # Force the test case to fail.
```

### Comparing `pytest_lsp-0.4.1/tests/examples/getting-started-fail/t_server.py` & `pytest_lsp-0.4.2/tests/examples/window-log-message-fail/t_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import sys
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
+import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
@@ -23,16 +24,14 @@
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
 async def test_completions(client: LanguageClient):
-    """Ensure that the server implements completions correctly."""
-
     results = await client.text_document_completion_async(
         params=CompletionParams(
             position=Position(line=1, character=0),
             text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
 
@@ -40,8 +39,13 @@
 
     if isinstance(results, CompletionList):
         items = results.items
     else:
         items = results
 
     labels = [item.label for item in items]
-    assert labels == ["hello", "world"]
+    assert labels == [f"item-{i}" for i in range(10)]
+
+    for idx, log_message in enumerate(client.log_messages):
+        assert log_message.message == f"Suggesting item {idx}"
+
+    pytest.fail("Failing test!")  # Force the test case to fail.
```

### Comparing `pytest_lsp-0.4.1/tests/examples/parameterised-clients/t_server.py` & `pytest_lsp-0.4.2/tests/examples/window-show-message/t_server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 import sys
 
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
+import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
-from pytest_lsp import client_capabilities
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
-    params=["neovim", "visual_studio_code"],
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
-async def client(request, lsp_client: LanguageClient):
+async def client(lsp_client: LanguageClient):
     # Setup
-    params = InitializeParams(capabilities=client_capabilities(request.param))
+    params = InitializeParams(capabilities=ClientCapabilities())
     await lsp_client.initialize_session(params)
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
+@pytest.mark.asyncio
 async def test_completions(client: LanguageClient):
-    """Ensure that the server implements completions correctly."""
-
     results = await client.text_document_completion_async(
         params=CompletionParams(
             position=Position(line=1, character=0),
             text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
+
     assert results is not None
 
     if isinstance(results, CompletionList):
         items = results.items
     else:
         items = results
 
     labels = [item.label for item in items]
-    assert labels == ["hello", "world"]
+    assert labels == [f"item-{i}" for i in range(10)]
+
+    for idx, shown_message in enumerate(client.messages):
+        assert shown_message.message == f"Suggesting item {idx}"
```

### Comparing `pytest_lsp-0.4.1/tests/examples/server-stderr/t_server.py` & `pytest_lsp-0.4.2/tests/examples/parameterised-clients/t_server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 import sys
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient, client_capabilities
 
 
 @pytest_lsp.fixture(
+    params=["neovim", "visual_studio_code"],
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
-async def client(lsp_client: LanguageClient):
+async def client(request, lsp_client: LanguageClient):
     # Setup
-    params = InitializeParams(capabilities=ClientCapabilities())
+    params = InitializeParams(capabilities=client_capabilities(request.param))
     await lsp_client.initialize_session(params)
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
 async def test_completions(client: LanguageClient):
+    """Ensure that the server implements completions correctly."""
+
     results = await client.text_document_completion_async(
         params=CompletionParams(
             position=Position(line=1, character=0),
             text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
         )
     )
-
     assert results is not None
 
     if isinstance(results, CompletionList):
         items = results.items
     else:
         items = results
 
     labels = [item.label for item in items]
-    assert labels == [f"item-{i}" for i in range(10)]
-    assert False  # Force the test case to fail.
+    assert labels == ["hello", "world"]
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-create-progress/server.py` & `pytest_lsp-0.4.2/tests/examples/window-create-progress/server.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/examples/window-create-progress/t_server.py` & `pytest_lsp-0.4.2/tests/examples/window-create-progress/t_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import sys
 
 import pytest
-from lsprotocol import types
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
-from pytest_lsp import LspSpecificationWarning
+from lsprotocol import types
+from pytest_lsp import ClientServerConfig, LanguageClient, LspSpecificationWarning
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-log-message/server.py` & `pytest_lsp-0.4.2/tests/servers/completion_exit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+# A server that exits mid request.
+import sys
+
 from lsprotocol.types import TEXT_DOCUMENT_COMPLETION
 from lsprotocol.types import CompletionItem
 from lsprotocol.types import CompletionParams
 from pygls.server import LanguageServer
 
-server = LanguageServer("window-log-message", "v1")
 
+class CountingLanguageServer(LanguageServer):
+    count: int = 0
 
-@server.feature(TEXT_DOCUMENT_COMPLETION)
-def completion(ls: LanguageServer, params: CompletionParams):
-    items = []
 
-    for i in range(10):
-        ls.show_message_log(f"Suggesting item {i}")
-        items.append(CompletionItem(label=f"item-{i}"))
+server = CountingLanguageServer(name="completion-exit-server", version="v1.0")
+
+
+@server.feature(TEXT_DOCUMENT_COMPLETION)
+def on_complete(server: CountingLanguageServer, params: CompletionParams):
+    server.count += 1
+    if server.count == 5:
+        sys.exit(0)
 
-    return items
+    return [CompletionItem(label=f"{server.count}")]
 
 
 if __name__ == "__main__":
     server.start_io()
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-log-message/t_server.py` & `pytest_lsp-0.4.2/tests/examples/window-log-message/t_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-log-message-fail/server.py` & `pytest_lsp-0.4.2/tests/examples/window-show-document/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from lsprotocol.types import TEXT_DOCUMENT_COMPLETION
-from lsprotocol.types import CompletionItem
-from lsprotocol.types import CompletionParams
+from lsprotocol.types import (
+    TEXT_DOCUMENT_COMPLETION,
+    CompletionItem,
+    CompletionParams,
+    ShowDocumentParams,
+)
 from pygls.server import LanguageServer
 
-server = LanguageServer("window-log-message", "v1")
+server = LanguageServer("window-show-document", "v1")
 
 
 @server.feature(TEXT_DOCUMENT_COMPLETION)
-def completion(ls: LanguageServer, params: CompletionParams):
+async def completion(ls: LanguageServer, params: CompletionParams):
     items = []
+    await ls.show_document_async(ShowDocumentParams(uri=params.text_document.uri))
 
     for i in range(10):
-        ls.show_message_log(f"Suggesting item {i}")
         items.append(CompletionItem(label=f"item-{i}"))
 
     return items
 
 
 if __name__ == "__main__":
     server.start_io()
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-show-document/t_server.py` & `pytest_lsp-0.4.2/tests/examples/window-show-document/t_server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import sys
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
-
 import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    ClientCapabilities,
+    CompletionList,
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/examples/window-show-message/t_server.py` & `pytest_lsp-0.4.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-import sys
+# pytest-lsp: End-to-end testing of language servers with pytest
+
+`pytest-lsp` is a pytest plugin for writing end-to-end tests for language servers.
+
+It works by running the language server in a subprocess and communicating with it over stdio, just like a real language client.
+This also means `pytest-lsp` can be used to test language servers written in any language - not just Python.
+
+`pytest-lsp` relies on the [`pygls`](https://github.com/openlawlibrary/pygls) library for its language server protocol implementation.
 
-from lsprotocol.types import ClientCapabilities
-from lsprotocol.types import CompletionList
-from lsprotocol.types import CompletionParams
-from lsprotocol.types import InitializeParams
-from lsprotocol.types import Position
-from lsprotocol.types import TextDocumentIdentifier
+See the [documentation](https://lsp-devtools.readthedocs.io/en/latest/) for details on getting started.
+
+```python
+import sys
 
-import pytest
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol.types import (
+    CompletionParams,
+    InitializeParams,
+    Position,
+    TextDocumentIdentifier,
+)
+from pytest_lsp import (
+    ClientServerConfig,
+    LanguageClient,
+    client_capabilities,
+)
 
 
 @pytest_lsp.fixture(
-    config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
+    config=ClientServerConfig(
+        server_command=[sys.executable, "-m", "esbonio"],
+    ),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
-    params = InitializeParams(capabilities=ClientCapabilities())
-    await lsp_client.initialize_session(params)
+    response = await lsp_client.initialize_session(
+        InitializeParams(
+            capabilities=client_capabilities("visual-studio-code"),
+            root_uri="file:///path/to/test/project/root/",
+        )
+    )
 
     yield
 
     # Teardown
     await lsp_client.shutdown_session()
 
 
-@pytest.mark.asyncio
-async def test_completions(client: LanguageClient):
-    results = await client.text_document_completion_async(
+async def test_completion(client: LanguageClient):
+    result = await client.text_document_completion_async(
         params=CompletionParams(
-            position=Position(line=1, character=0),
-            text_document=TextDocumentIdentifier(uri="file:///path/to/file.txt"),
+            position=Position(line=5, character=23),
+            text_document=TextDocumentIdentifier(
+                uri="file:///path/to/test/project/root/test_file.rst"
+            ),
         )
     )
 
-    assert results is not None
-
-    if isinstance(results, CompletionList):
-        items = results.items
-    else:
-        items = results
-
-    labels = [item.label for item in items]
-    assert labels == [f"item-{i}" for i in range(10)]
-
-    for idx, shown_message in enumerate(client.messages):
-        assert shown_message.message == f"Suggesting item {idx}"
+    assert len(result.items) > 0
+```
```

### Comparing `pytest_lsp-0.4.1/tests/examples/workspace-configuration/server.py` & `pytest_lsp-0.4.2/tests/examples/workspace-configuration/server.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/tests/examples/workspace-configuration/t_server.py` & `pytest_lsp-0.4.2/tests/examples/workspace-configuration/t_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import sys
 
 import pytest
-from lsprotocol import types
-
 import pytest_lsp
-from pytest_lsp import ClientServerConfig
-from pytest_lsp import LanguageClient
+from lsprotocol import types
+from pytest_lsp import ClientServerConfig, LanguageClient
 
 
 @pytest_lsp.fixture(
     config=ClientServerConfig(server_command=[sys.executable, "server.py"]),
 )
 async def client(lsp_client: LanguageClient):
     # Setup
```

### Comparing `pytest_lsp-0.4.1/tests/servers/invalid_json.py` & `pytest_lsp-0.4.2/tests/servers/invalid_json.py`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/LICENSE` & `pytest_lsp-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_lsp-0.4.1/pyproject.toml` & `pytest_lsp-0.4.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -43,18 +43,14 @@
 source_pkgs = ["pytest_lsp"]
 
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 sort = "Cover"
 
-[tool.isort]
-force_single_line = true
-profile = "black"
-
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.towncrier]
 filename = "CHANGES.md"
 directory = "changes/"
 title_format = "## v{version} - {project_date}"
```

### Comparing `pytest_lsp-0.4.1/PKG-INFO` & `pytest_lsp-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pytest-lsp
-Version: 0.4.1
+Version: 0.4.2
 Summary: A pytest plugin for end-to-end testing of language servers
 Project-URL: Bug Tracker, https://github.com/swyddfa/lsp-devtools/issues
 Project-URL: Documentation, https://lsp-devtools.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/swyddfa/lsp-devtools
 Author-email: Alex Carney <alcarneyme@gmail.com>
 License: MIT
 License-File: LICENSE
```

