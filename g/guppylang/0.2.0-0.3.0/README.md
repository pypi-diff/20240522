# Comparing `tmp/guppylang-0.2.0.tar.gz` & `tmp/guppylang-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guppylang-0.2.0.tar", max compression
+gzip compressed data, was "guppylang-0.3.0.tar", max compression
```

## Comparing `guppylang-0.2.0.tar` & `guppylang-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0      240 2024-03-06 14:35:45.141750 guppylang-0.2.0/guppylang/__init__.py
--rw-r--r--   0        0        0    10848 2024-03-19 17:26:38.074513 guppylang-0.2.0/guppylang/ast_util.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.099571 guppylang-0.2.0/guppylang/cfg/__init__.py
--rw-r--r--   0        0        0     6805 2024-01-18 13:08:34.099799 guppylang-0.2.0/guppylang/cfg/analysis.py
--rw-r--r--   0        0        0     5600 2024-01-18 13:08:34.099944 guppylang-0.2.0/guppylang/cfg/bb.py
--rw-r--r--   0        0        0    20103 2024-03-19 17:26:38.075014 guppylang-0.2.0/guppylang/cfg/builder.py
--rw-r--r--   0        0        0     2034 2024-01-18 13:08:34.100296 guppylang-0.2.0/guppylang/cfg/cfg.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.100352 guppylang-0.2.0/guppylang/checker/__init__.py
--rw-r--r--   0        0        0     9281 2024-04-10 12:30:34.670288 guppylang-0.2.0/guppylang/checker/cfg_checker.py
--rw-r--r--   0        0        0     6958 2024-04-10 12:30:34.670754 guppylang-0.2.0/guppylang/checker/core.py
--rw-r--r--   0        0        0    40940 2024-04-10 12:30:34.671870 guppylang-0.2.0/guppylang/checker/expr_checker.py
--rw-r--r--   0        0        0     7887 2024-04-10 12:30:34.672400 guppylang-0.2.0/guppylang/checker/func_checker.py
--rw-r--r--   0        0        0     6466 2024-03-19 17:26:38.077637 guppylang-0.2.0/guppylang/checker/stmt_checker.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.101552 guppylang-0.2.0/guppylang/compiler/__init__.py
--rw-r--r--   0        0        0     6881 2024-04-10 12:30:34.672984 guppylang-0.2.0/guppylang/compiler/cfg_compiler.py
--rw-r--r--   0        0        0     3592 2024-04-10 12:30:34.673508 guppylang-0.2.0/guppylang/compiler/core.py
--rw-r--r--   0        0        0    13938 2024-04-10 12:34:58.734322 guppylang-0.2.0/guppylang/compiler/expr_compiler.py
--rw-r--r--   0        0        0     4497 2024-04-10 12:30:34.675115 guppylang-0.2.0/guppylang/compiler/func_compiler.py
--rw-r--r--   0        0        0     3501 2024-03-19 17:26:38.078950 guppylang-0.2.0/guppylang/compiler/stmt_compiler.py
--rw-r--r--   0        0        0     9000 2024-04-10 12:30:34.675423 guppylang-0.2.0/guppylang/custom.py
--rw-r--r--   0        0        0     3066 2024-04-10 12:30:34.675833 guppylang-0.2.0/guppylang/declared.py
--rw-r--r--   0        0        0     8741 2024-04-10 12:30:34.676264 guppylang-0.2.0/guppylang/decorator.py
--rw-r--r--   0        0        0     6043 2024-03-19 17:26:38.079877 guppylang-0.2.0/guppylang/error.py
--rw-r--r--   0        0        0        0 2024-01-30 13:18:23.816770 guppylang-0.2.0/guppylang/graph.hugr
--rw-r--r--   0        0        0     2903 2024-04-09 09:34:36.229984 guppylang-0.2.0/guppylang/graph.json
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.102977 guppylang-0.2.0/guppylang/hugr/__init__.py
--rw-r--r--   0        0        0    28695 2024-03-19 17:26:38.080208 guppylang-0.2.0/guppylang/hugr/hugr.py
--rw-r--r--   0        0        0    14938 2024-03-19 17:26:38.080533 guppylang-0.2.0/guppylang/hugr/ops.py
--rw-r--r--   0        0        0      567 2024-01-30 09:26:54.831969 guppylang-0.2.0/guppylang/hugr/raw.py
--rw-r--r--   0        0        0     7476 2024-04-09 09:42:13.717116 guppylang-0.2.0/guppylang/hugr/tys.py
--rw-r--r--   0        0        0     1340 2024-01-18 13:08:34.103710 guppylang-0.2.0/guppylang/hugr/val.py
--rw-r--r--   0        0        0     8182 2024-03-19 14:02:30.181552 guppylang-0.2.0/guppylang/hugr/visualise.py
--rw-r--r--   0        0        0    11390 2024-04-10 12:30:34.676681 guppylang-0.2.0/guppylang/module.py
--rw-r--r--   0        0        0     3773 2024-04-10 12:30:34.677122 guppylang-0.2.0/guppylang/nodes.py
--rw-r--r--   0        0        0        0 2024-01-18 13:08:34.104139 guppylang-0.2.0/guppylang/prelude/__init__.py
--rw-r--r--   0        0        0    11676 2024-04-10 12:34:58.734743 guppylang-0.2.0/guppylang/prelude/_internal.py
--rw-r--r--   0        0        0    22151 2024-04-10 12:30:34.677590 guppylang-0.2.0/guppylang/prelude/builtins.py
--rw-r--r--   0        0        0     2566 2024-04-11 09:51:54.533323 guppylang-0.2.0/guppylang/prelude/quantum.py
--rw-r--r--   0        0        0        0 2024-03-04 15:19:40.627545 guppylang-0.2.0/guppylang/py.typed
--rw-r--r--   0        0        0    10347 2024-04-09 09:34:36.108313 guppylang-0.2.0/guppylang/test
--rw-r--r--   0        0        0    20574 2024-04-09 09:34:36.224964 guppylang-0.2.0/guppylang/test.svg
--rw-r--r--   0        0        0        0 2024-03-19 17:26:38.082129 guppylang-0.2.0/guppylang/tys/__init__.py
--rw-r--r--   0        0        0     2934 2024-03-19 17:26:38.082454 guppylang-0.2.0/guppylang/tys/arg.py
--rw-r--r--   0        0        0     1835 2024-03-19 17:26:38.082672 guppylang-0.2.0/guppylang/tys/common.py
--rw-r--r--   0        0        0     1860 2024-03-19 17:26:38.082879 guppylang-0.2.0/guppylang/tys/const.py
--rw-r--r--   0        0        0     6593 2024-04-10 12:30:34.679407 guppylang-0.2.0/guppylang/tys/definition.py
--rw-r--r--   0        0        0     5826 2024-03-19 17:26:38.083313 guppylang-0.2.0/guppylang/tys/param.py
--rw-r--r--   0        0        0     4447 2024-04-10 12:30:34.680034 guppylang-0.2.0/guppylang/tys/parsing.py
--rw-r--r--   0        0        0     4390 2024-03-19 17:26:38.083753 guppylang-0.2.0/guppylang/tys/printing.py
--rw-r--r--   0        0        0     2209 2024-03-19 17:26:38.083922 guppylang-0.2.0/guppylang/tys/subst.py
--rw-r--r--   0        0        0    18580 2024-04-10 12:30:34.680493 guppylang-0.2.0/guppylang/tys/ty.py
--rw-r--r--   0        0        0     1174 2024-03-19 17:26:38.084390 guppylang-0.2.0/guppylang/tys/var.py
--rw-r--r--   0        0        0     1173 2024-04-11 09:51:54.533542 guppylang-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      646 2024-03-06 14:35:45.146062 guppylang-0.2.0/quickstart.md
--rw-r--r--   0        0        0     1441 1970-01-01 00:00:00.000000 guppylang-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-16 13:03:20.692812 guppylang-0.3.0/LICENCE
+-rw-r--r--   0        0        0      240 2024-03-06 14:35:45.141750 guppylang-0.3.0/guppylang/__init__.py
+-rw-r--r--   0        0        0    11717 2024-05-16 08:19:39.071491 guppylang-0.3.0/guppylang/ast_util.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.099571 guppylang-0.3.0/guppylang/cfg/__init__.py
+-rw-r--r--   0        0        0     6805 2024-04-11 15:37:05.443728 guppylang-0.3.0/guppylang/cfg/analysis.py
+-rw-r--r--   0        0        0     5600 2024-01-18 13:08:34.099944 guppylang-0.3.0/guppylang/cfg/bb.py
+-rw-r--r--   0        0        0    20103 2024-03-19 17:26:38.075014 guppylang-0.3.0/guppylang/cfg/builder.py
+-rw-r--r--   0        0        0     2034 2024-01-18 13:08:34.100296 guppylang-0.3.0/guppylang/cfg/cfg.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.100352 guppylang-0.3.0/guppylang/checker/__init__.py
+-rw-r--r--   0        0        0     9267 2024-04-16 10:39:14.815309 guppylang-0.3.0/guppylang/checker/cfg_checker.py
+-rw-r--r--   0        0        0     7303 2024-05-21 08:25:07.488971 guppylang-0.3.0/guppylang/checker/core.py
+-rw-r--r--   0        0        0    43253 2024-05-15 11:05:11.494825 guppylang-0.3.0/guppylang/checker/expr_checker.py
+-rw-r--r--   0        0        0     6515 2024-05-16 08:19:39.072106 guppylang-0.3.0/guppylang/checker/func_checker.py
+-rw-r--r--   0        0        0     6466 2024-03-19 17:26:38.077637 guppylang-0.3.0/guppylang/checker/stmt_checker.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.101552 guppylang-0.3.0/guppylang/compiler/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-16 08:39:58.377179 guppylang-0.3.0/guppylang/compiler/cfg_compiler.py
+-rw-r--r--   0        0        0     2774 2024-05-16 08:39:58.377318 guppylang-0.3.0/guppylang/compiler/core.py
+-rw-r--r--   0        0        0    16773 2024-05-22 14:23:20.915219 guppylang-0.3.0/guppylang/compiler/expr_compiler.py
+-rw-r--r--   0        0        0     3433 2024-05-16 08:39:58.377812 guppylang-0.3.0/guppylang/compiler/func_compiler.py
+-rw-r--r--   0        0        0     3509 2024-05-16 08:39:58.377937 guppylang-0.3.0/guppylang/compiler/stmt_compiler.py
+-rw-r--r--   0        0        0     9397 2024-05-16 08:39:58.378210 guppylang-0.3.0/guppylang/decorator.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:39:14.818760 guppylang-0.3.0/guppylang/definition/__init__.py
+-rw-r--r--   0        0        0     4063 2024-05-16 08:39:58.378467 guppylang-0.3.0/guppylang/definition/common.py
+-rw-r--r--   0        0        0    10028 2024-05-16 08:39:58.378624 guppylang-0.3.0/guppylang/definition/custom.py
+-rw-r--r--   0        0        0     4153 2024-05-16 08:39:58.378758 guppylang-0.3.0/guppylang/definition/declaration.py
+-rw-r--r--   0        0        0     6560 2024-05-16 08:39:58.378889 guppylang-0.3.0/guppylang/definition/function.py
+-rw-r--r--   0        0        0      768 2024-04-16 10:39:14.820919 guppylang-0.3.0/guppylang/definition/parameter.py
+-rw-r--r--   0        0        0    10623 2024-05-16 08:19:39.074117 guppylang-0.3.0/guppylang/definition/struct.py
+-rw-r--r--   0        0        0     1745 2024-05-16 08:39:58.379178 guppylang-0.3.0/guppylang/definition/ty.py
+-rw-r--r--   0        0        0     2880 2024-05-16 08:39:58.379286 guppylang-0.3.0/guppylang/definition/value.py
+-rw-r--r--   0        0        0     6043 2024-03-19 17:26:38.079877 guppylang-0.3.0/guppylang/error.py
+-rw-r--r--   0        0        0        0 2024-01-30 13:18:23.816770 guppylang-0.3.0/guppylang/graph.hugr
+-rw-r--r--   0        0        0    17256 2024-05-14 08:36:03.085334 guppylang-0.3.0/guppylang/graph.json
+-rw-r--r--   0        0        0        0 2024-05-16 08:39:58.379321 guppylang-0.3.0/guppylang/hugr_builder/__init__.py
+-rw-r--r--   0        0        0    30252 2024-05-16 08:39:58.379625 guppylang-0.3.0/guppylang/hugr_builder/hugr.py
+-rw-r--r--   0        0        0     8223 2024-05-16 08:39:58.379735 guppylang-0.3.0/guppylang/hugr_builder/visualise.py
+-rw-r--r--   0        0        0     9099 2024-05-16 08:39:58.379946 guppylang-0.3.0/guppylang/module.py
+-rw-r--r--   0        0        0     4173 2024-05-15 11:05:11.496569 guppylang-0.3.0/guppylang/nodes.py
+-rw-r--r--   0        0        0        0 2024-01-18 13:08:34.104139 guppylang-0.3.0/guppylang/prelude/__init__.py
+-rw-r--r--   0        0        0    12756 2024-05-21 08:31:14.534985 guppylang-0.3.0/guppylang/prelude/_internal.py
+-rw-r--r--   0        0        0    21940 2024-05-21 08:25:07.490151 guppylang-0.3.0/guppylang/prelude/builtins.py
+-rw-r--r--   0        0        0     2695 2024-05-16 08:39:58.380535 guppylang-0.3.0/guppylang/prelude/quantum.py
+-rw-r--r--   0        0        0        0 2024-03-04 15:19:40.627545 guppylang-0.3.0/guppylang/py.typed
+-rw-r--r--   0        0        0    57008 2024-05-14 08:36:02.964537 guppylang-0.3.0/guppylang/test
+-rw-r--r--   0        0        0   110258 2024-05-14 08:36:03.079698 guppylang-0.3.0/guppylang/test.svg
+-rw-r--r--   0        0        0        0 2024-03-19 17:26:38.082129 guppylang-0.3.0/guppylang/tys/__init__.py
+-rw-r--r--   0        0        0     2952 2024-05-16 15:53:50.323816 guppylang-0.3.0/guppylang/tys/arg.py
+-rw-r--r--   0        0        0     5348 2024-05-21 08:25:07.490527 guppylang-0.3.0/guppylang/tys/builtin.py
+-rw-r--r--   0        0        0     1835 2024-05-08 13:56:29.603685 guppylang-0.3.0/guppylang/tys/common.py
+-rw-r--r--   0        0        0     1865 2024-05-16 10:25:22.563789 guppylang-0.3.0/guppylang/tys/const.py
+-rw-r--r--   0        0        0     6818 2024-05-16 15:53:50.324510 guppylang-0.3.0/guppylang/tys/param.py
+-rw-r--r--   0        0        0     5232 2024-05-16 08:19:39.075330 guppylang-0.3.0/guppylang/tys/parsing.py
+-rw-r--r--   0        0        0     4489 2024-05-21 08:25:07.490807 guppylang-0.3.0/guppylang/tys/printing.py
+-rw-r--r--   0        0        0     2209 2024-05-15 14:51:55.689897 guppylang-0.3.0/guppylang/tys/subst.py
+-rw-r--r--   0        0        0    22318 2024-05-21 08:25:07.491323 guppylang-0.3.0/guppylang/tys/ty.py
+-rw-r--r--   0        0        0     1174 2024-03-19 17:26:38.084390 guppylang-0.3.0/guppylang/tys/var.py
+-rw-r--r--   0        0        0     1226 2024-05-22 14:23:20.916921 guppylang-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      646 2024-03-06 14:35:45.146062 guppylang-0.3.0/quickstart.md
+-rw-r--r--   0        0        0     1478 1970-01-01 00:00:00.000000 guppylang-0.3.0/PKG-INFO
```

### Comparing `guppylang-0.2.0/guppylang/ast_util.py` & `guppylang-0.3.0/guppylang/ast_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -246,14 +246,33 @@
                 for item in value:
                     if isinstance(item, ast.AST):
                         annotate_location(item, source, file, line_offset, recurse)
             elif isinstance(value, ast.AST):
                 annotate_location(value, source, file, line_offset, recurse)
 
 
+def shift_loc(node: ast.AST, delta_lineno: int, delta_col_offset: int) -> None:
+    """Shifts all line and column number in the AST node by the given amount."""
+    if hasattr(node, "lineno"):
+        node.lineno += delta_lineno
+    if hasattr(node, "end_lineno") and node.end_lineno is not None:
+        node.end_lineno += delta_lineno
+    if hasattr(node, "col_offset"):
+        node.col_offset += delta_col_offset
+    if hasattr(node, "end_col_offset") and node.end_col_offset is not None:
+        node.end_col_offset += delta_col_offset
+    for _, value in ast.iter_fields(node):
+        if isinstance(value, list):
+            for item in value:
+                if isinstance(item, ast.AST):
+                    shift_loc(item, delta_lineno, delta_col_offset)
+        elif isinstance(value, ast.AST):
+            shift_loc(value, delta_lineno, delta_col_offset)
+
+
 def get_file(node: AstNode) -> str | None:
     """Tries to retrieve a file annotation from an AST node."""
     try:
         file = node.file  # type: ignore[union-attr]
         return file if isinstance(file, str) else None
     except AttributeError:
         return None
```

### Comparing `guppylang-0.2.0/guppylang/cfg/analysis.py` & `guppylang-0.3.0/guppylang/cfg/analysis.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/cfg/bb.py` & `guppylang-0.3.0/guppylang/cfg/bb.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/cfg/builder.py` & `guppylang-0.3.0/guppylang/cfg/builder.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/cfg/cfg.py` & `guppylang-0.3.0/guppylang/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/checker/cfg_checker.py` & `guppylang-0.3.0/guppylang/checker/cfg_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     cfg = bb.containing_cfg
 
     # For the entry BB we have to separately check that all used variables are
     # defined. For all other BBs, this will be checked when compiling a predecessor.
     if bb == cfg.entry_bb:
         assert len(bb.predecessors) == 0
         for x, use in bb.vars.used.items():
-            if x not in cfg.ass_before[bb] and x not in globals.values:
+            if x not in cfg.ass_before[bb] and x not in globals:
                 raise GuppyError(f"Variable `{x}` is not defined", use)
 
     # Check the basic block
     ctx = Context(globals, Locals({v.name: v for v in inputs}))
     checked_stmts = StmtChecker(ctx, bb, return_ty).check_stmts(bb.statements)
 
     # If we branch, we also have to check the branch predicate
@@ -143,15 +143,15 @@
         assert bb.branch_pred is not None
         bb.branch_pred, ty = ExprSynthesizer(ctx).synthesize(bb.branch_pred)
         bb.branch_pred, _ = to_bool(bb.branch_pred, ty, ctx)
 
     for succ in bb.successors:
         for x, use_bb in cfg.live_before[succ].items():
             # Check that the variables requested by the successor are defined
-            if x not in ctx.locals and x not in ctx.globals.values:
+            if x not in ctx.locals and x not in ctx.globals:
                 # If the variable is defined on *some* paths, we can give a more
                 # informative error message
                 if x in cfg.maybe_ass_before[use_bb]:
                     # TODO: This should be "Variable x is not defined when coming
                     #  from {bb}". But for this we need a way to associate BBs with
                     #  source locations.
                     raise GuppyError(
```

### Comparing `guppylang-0.2.0/guppylang/checker/core.py` & `guppylang-0.3.0/guppylang/checker/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,146 +1,151 @@
 import ast
 import copy
 import itertools
-from abc import ABC, abstractmethod
-from collections.abc import Iterable, Iterator
+from collections.abc import Iterable, Iterator, Mapping
 from dataclasses import dataclass
 from typing import Any, NamedTuple
 
 from typing_extensions import assert_never
 
 from guppylang.ast_util import AstNode, name_nodes_in_ast
-from guppylang.tys.definition import (
-    TypeDef,
+from guppylang.definition.common import DefId, Definition
+from guppylang.definition.ty import TypeDef
+from guppylang.definition.value import CallableDef
+from guppylang.tys.builtin import (
     bool_type_def,
     callable_type_def,
     linst_type_def,
     list_type_def,
     none_type_def,
     tuple_type_def,
 )
-from guppylang.tys.param import Parameter
-from guppylang.tys.subst import Subst
 from guppylang.tys.ty import (
     BoundTypeVar,
     ExistentialTypeVar,
     FunctionType,
     NoneType,
     OpaqueType,
+    StructType,
     SumType,
     TupleType,
     Type,
 )
 
 
 @dataclass
 class Variable:
-    """Class holding data associated with a variable."""
+    """Class holding data associated with a local variable."""
 
     name: str
     ty: Type
     defined_at: AstNode | None
     used: AstNode | None
 
 
-@dataclass
-class CallableVariable(ABC, Variable):
-    """Abstract base class for global variables that can be called."""
-
-    ty: FunctionType
-
-    @abstractmethod
-    def check_call(
-        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: "Context"
-    ) -> tuple[ast.expr, Subst]:
-        """Checks the return type of a function call against a given type."""
-
-    @abstractmethod
-    def synthesize_call(
-        self, args: list[ast.expr], node: AstNode, ctx: "Context"
-    ) -> tuple[ast.expr, Type]:
-        """Synthesizes the return type of a function call."""
-
-
-@dataclass
-class TypeVarDecl:
-    """A declared type variable."""
-
-    name: str
-    linear: bool
-
-
 PyScope = dict[str, Any]
 
 
-class Globals(NamedTuple):
-    """Collection of names that are available on module-level.
+@dataclass(frozen=True)
+class Globals:
+    """Collection of definitions that are available on module-level.
 
-    Separately stores names that are bound to values (i.e. module-level functions or
-    constants), to types, or to instance functions belonging to types.
+    Stores a mapping from global ids to their definition together with a mapping of
+    user names to definition id and instance implementation id.
     """
 
-    values: dict[str, Variable]
-    type_defs: dict[str, TypeDef]
-    param_vars: dict[str, Parameter]
+    defs: Mapping[DefId, Definition]
+
+    names: dict[str, DefId]
+    impls: dict[DefId, dict[str, DefId]]
     python_scope: PyScope
 
     @staticmethod
     def default() -> "Globals":
         """Generates a `Globals` instance that is populated with all core types"""
-        type_defs = {
-            "Callable": callable_type_def,
-            "tuple": tuple_type_def,
-            "None": none_type_def,
-            "bool": bool_type_def,
-            "list": list_type_def,
-            "linst": linst_type_def,
-        }
-        return Globals({}, type_defs, {}, {})
+        builtins: list[Definition] = [
+            callable_type_def,
+            tuple_type_def,
+            none_type_def,
+            bool_type_def,
+            list_type_def,
+            linst_type_def,
+        ]
+        defs = {defn.id: defn for defn in builtins}
+        names = {defn.name: defn.id for defn in builtins}
+        return Globals(defs, names, {}, {})
 
-    def get_instance_func(self, ty: Type, name: str) -> CallableVariable | None:
+    def get_instance_func(self, ty: Type | TypeDef, name: str) -> CallableDef | None:
         """Looks up an instance function with a given name for a type.
 
         Returns `None` if the name doesn't exist or isn't a function.
         """
-        defn: TypeDef
+        type_defn: TypeDef
         match ty:
+            case TypeDef() as type_defn:
+                pass
             case BoundTypeVar() | ExistentialTypeVar() | SumType():
                 return None
             case FunctionType():
-                defn = callable_type_def
+                type_defn = callable_type_def
             case OpaqueType() as ty:
-                defn = ty.defn
+                type_defn = ty.defn
+            case StructType() as ty:
+                type_defn = ty.defn
             case TupleType():
-                defn = tuple_type_def
+                type_defn = tuple_type_def
             case NoneType():
-                defn = none_type_def
+                type_defn = none_type_def
             case _:
-                assert_never(ty)
+                return assert_never(ty)
 
-        qualname = qualified_name(defn.name, name)
-        if qualname in self.values:
-            val = self.values[qualname]
-            if isinstance(val, CallableVariable):
-                return val
+        if type_defn.id in self.impls and name in self.impls[type_defn.id]:
+            def_id = self.impls[type_defn.id][name]
+            defn = self.defs[def_id]
+            if isinstance(defn, CallableDef):
+                return defn
         return None
 
+    def update_defs(self, defs: Mapping[DefId, Definition]) -> "Globals":
+        """Returns a new `Globals` instance with updated definitions.
+
+        This method is needed since in-place definition updates are impossible as the
+        definition map is immutable.
+        """
+        return Globals({**self.defs, **defs}, self.names, self.impls, self.python_scope)
+
     def __or__(self, other: "Globals") -> "Globals":
+        impls = {
+            def_id: self.impls.get(def_id, {}) | other.impls.get(def_id, {})
+            for def_id in self.impls.keys() | other.impls.keys()
+        }
         return Globals(
-            self.values | other.values,
-            self.type_defs | other.type_defs,
-            self.param_vars | other.param_vars,
+            {**self.defs, **other.defs},  # Can't use `|` since it's a Mapping
+            self.names | other.names,
+            impls,
             self.python_scope | other.python_scope,
         )
 
-    def __ior__(self, other: "Globals") -> "Globals":  # noqa: PYI034
-        self.values.update(other.values)
-        self.type_defs.update(other.type_defs)
-        self.param_vars.update(other.param_vars)
-        return self
+    def __contains__(self, item: DefId | str) -> bool:
+        match item:
+            case DefId() as def_id:
+                return def_id in self.defs
+            case str(name):
+                return name in self.names
+            case x:
+                return assert_never(x)
+
+    def __getitem__(self, item: DefId | str) -> Definition:
+        match item:
+            case DefId() as def_id:
+                return self.defs[def_id]
+            case str(name):
+                return self.defs[self.names[name]]
+            case x:
+                return assert_never(x)
 
 
 @dataclass
 class Locals:
     """Scoped mapping from names to variables"""
 
     vars: dict[str, Variable]
@@ -223,13 +228,7 @@
         self._check_item(key)
         super().__delitem__(key)
 
     def __contains__(self, key: object) -> bool:
         if isinstance(key, str) and key in self.ctx.locals:
             return True
         return super().__contains__(key)
-
-
-def qualified_name(ty: TypeDef | str, name: str) -> str:
-    """Returns a qualified name for an instance function on a type."""
-    ty_name = ty if isinstance(ty, str) else ty.name
-    return f"{ty_name}.{name}"
```

### Comparing `guppylang-0.2.0/guppylang/checker/expr_checker.py` & `guppylang-0.3.0/guppylang/checker/expr_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,21 @@
     get_type_opt,
     name_nodes_in_ast,
     return_nodes_in_ast,
     with_loc,
     with_type,
 )
 from guppylang.checker.core import (
-    CallableVariable,
     Context,
     DummyEvalDict,
     Globals,
     Locals,
 )
+from guppylang.definition.ty import TypeDef
+from guppylang.definition.value import CallableDef, ValueDef
 from guppylang.error import (
     GuppyError,
     GuppyTypeError,
     GuppyTypeInferenceError,
     InternalGuppyError,
 )
 from guppylang.nodes import (
@@ -56,18 +57,19 @@
     IterEnd,
     IterHasNext,
     IterNext,
     LocalCall,
     LocalName,
     MakeIter,
     PyExpr,
+    TensorCall,
     TypeApply,
 )
 from guppylang.tys.arg import TypeArg
-from guppylang.tys.definition import (
+from guppylang.tys.builtin import (
     bool_type,
     get_element_type,
     is_bool_type,
     is_linst_type,
     is_list_type,
     linst_type,
     list_type,
@@ -78,14 +80,16 @@
     ExistentialTypeVar,
     FunctionType,
     NoneType,
     OpaqueType,
     TupleType,
     Type,
     TypeBase,
+    function_tensor_signature,
+    parse_function_tensor,
     row_to_type,
     unify,
 )
 
 # Mapping from unary AST op to dunder method and display name
 unary_table: dict[type[ast.unaryop], tuple[str, str]] = {
     ast.UAdd:   ("__pos__",    "+"),
@@ -221,27 +225,50 @@
         if len(node.keywords) > 0:
             raise GuppyError(
                 "Argument passing by keyword is not supported", node.keywords[0]
             )
         node.func, func_ty = self._synthesize(node.func, allow_free_vars=False)
 
         # First handle direct calls of user-defined functions and extension functions
-        if isinstance(node.func, GlobalName) and isinstance(
-            node.func.value, CallableVariable
-        ):
-            return node.func.value.check_call(node.args, ty, node, self.ctx)
+        if isinstance(node.func, GlobalName):
+            defn = self.ctx.globals[node.func.def_id]
+            if isinstance(defn, CallableDef):
+                return defn.check_call(node.args, ty, node, self.ctx)
 
-        # Otherwise, it must be a function as a higher-order value
+        # Otherwise, it must be a function as a higher-order value - something
+        # whose type is either a FunctionType or a Tuple of FunctionTypes
         if isinstance(func_ty, FunctionType):
             args, return_ty, inst = check_call(func_ty, node.args, ty, node, self.ctx)
             check_inst(func_ty, inst, node)
             node.func = instantiate_poly(node.func, func_ty, inst)
             return with_loc(node, LocalCall(func=node.func, args=args)), return_ty
-        elif f := self.ctx.globals.get_instance_func(func_ty, "__call__"):
-            return f.check_call(node.args, ty, node, self.ctx)
+
+        if isinstance(func_ty, TupleType) and (
+            function_elements := parse_function_tensor(func_ty)
+        ):
+            if any(f.parametrized for f in function_elements):
+                raise GuppyTypeError(
+                    "Polymorphic functions in tuples are not supported", node.func
+                )
+
+            tensor_ty = function_tensor_signature(function_elements)
+
+            processed_args, subst, inst = check_call(
+                tensor_ty, node.args, ty, node, self.ctx
+            )
+            assert len(inst) == 0
+            return with_loc(
+                node,
+                TensorCall(
+                    func=node.func, args=processed_args, out_tys=tensor_ty.output
+                ),
+            ), subst
+
+        elif callee := self.ctx.globals.get_instance_func(func_ty, "__call__"):
+            return callee.check_call(node.args, ty, node, self.ctx)
         else:
             raise GuppyTypeError(f"Expected function type, got `{func_ty}`", node.func)
 
     def visit_PyExpr(self, node: PyExpr, ty: Type) -> tuple[ast.expr, Subst]:
         python_val = eval_py_expr(node, self.ctx)
         if act := python_value_to_guppy_type(python_val, node, self.ctx.globals):
             subst = unify(ty, act, {})
@@ -311,25 +338,36 @@
                     f"Variable `{x}` with linear type `{var.ty}` was "
                     "already used (at {0})",
                     node,
                     [var.used],
                 )
             var.used = node
             return with_loc(node, LocalName(id=x)), var.ty
-        elif x in self.ctx.globals.values:
-            # Cache value in the AST
-            value = self.ctx.globals.values[x]
-            return with_loc(node, GlobalName(id=x, value=value)), value.ty
+        elif x in self.ctx.globals:
+            # Look-up what kind of definition it is
+            match self.ctx.globals[x]:
+                case ValueDef() as defn:
+                    return with_loc(node, GlobalName(id=x, def_id=defn.id)), defn.ty
+                # For types, we return their `__new__` constructor
+                case TypeDef() as defn if constr := self.ctx.globals.get_instance_func(
+                    defn, "__new__"
+                ):
+                    return with_loc(node, GlobalName(id=x, def_id=constr.id)), constr.ty
+                case defn:
+                    raise GuppyError(
+                        f"Expected a value, got {defn.description} `{x}`", node
+                    )
         raise InternalGuppyError(
             f"Variable `{x}` is not defined in `TypeSynthesiser`. This should have "
-            f"been caught by program analysis!"
+            "been caught by program analysis!"
         )
 
     def visit_Tuple(self, node: ast.Tuple) -> tuple[ast.expr, Type]:
         elems = [self.synthesize(elem) for elem in node.elts]
+
         node.elts = [n for n, _ in elems]
         return node, TupleType([ty for _, ty in elems])
 
     def visit_List(self, node: ast.List) -> tuple[ast.expr, Type]:
         if len(node.elts) == 0:
             raise GuppyTypeInferenceError(
                 "Cannot infer type variable in expression of type `list[?T]`", node
@@ -450,24 +488,42 @@
 
     def visit_Call(self, node: ast.Call) -> tuple[ast.expr, Type]:
         if len(node.keywords) > 0:
             raise GuppyError("Keyword arguments are not supported", node.keywords[0])
         node.func, ty = self.synthesize(node.func)
 
         # First handle direct calls of user-defined functions and extension functions
-        if isinstance(node.func, GlobalName) and isinstance(
-            node.func.value, CallableVariable
-        ):
-            return node.func.value.synthesize_call(node.args, node, self.ctx)
+        if isinstance(node.func, GlobalName):
+            defn = self.ctx.globals[node.func.def_id]
+            if isinstance(defn, CallableDef):
+                return defn.synthesize_call(node.args, node, self.ctx)
 
-        # Otherwise, it must be a function as a higher-order value
+        # Otherwise, it must be a function as a higher-order value, or a tensor
         if isinstance(ty, FunctionType):
             args, return_ty, inst = synthesize_call(ty, node.args, node, self.ctx)
             node.func = instantiate_poly(node.func, ty, inst)
             return with_loc(node, LocalCall(func=node.func, args=args)), return_ty
+        elif isinstance(ty, TupleType) and (
+            function_elems := parse_function_tensor(ty)
+        ):
+            if any(f.parametrized for f in function_elems):
+                raise GuppyTypeError(
+                    "Polymorphic functions in tuples are not supported", node.func
+                )
+
+            tensor_ty = function_tensor_signature(function_elems)
+            args, return_ty, inst = synthesize_call(
+                tensor_ty, node.args, node, self.ctx
+            )
+            assert len(inst) == 0
+
+            return with_loc(
+                node, TensorCall(func=node.func, args=args, out_tys=tensor_ty.output)
+            ), return_ty
+
         elif f := self.ctx.globals.get_instance_func(ty, "__call__"):
             return f.synthesize_call(node.args, node, self.ctx)
         else:
             raise GuppyTypeError(f"Expected function type, got `{ty}`", node.func)
 
     def visit_MakeIter(self, node: MakeIter) -> tuple[ast.expr, Type]:
         node.value, ty = self.synthesize(node.value)
@@ -782,15 +838,15 @@
 
 def instantiate_poly(node: ast.expr, ty: FunctionType, inst: Inst) -> ast.expr:
     """Instantiates quantified type arguments in a function."""
     assert len(ty.params) == len(inst)
     if len(inst) > 0:
         node = with_loc(node, TypeApply(value=with_type(ty, node), inst=inst))
         return with_type(ty.instantiate(inst), node)
-    return node
+    return with_type(ty, node)
 
 
 def to_bool(node: ast.expr, node_ty: Type, ctx: Context) -> tuple[ast.expr, Type]:
     """Tries to turn a node into a bool"""
     if is_bool_type(node_ty):
         return node, node_ty
 
@@ -918,15 +974,15 @@
         )
     except DummyEvalDict.GuppyVarUsedError as e:
         raise GuppyError(
             f"Guppy variable `{e.var}` cannot be accessed in a compile-time "
             "`py(...)` expression",
             e.node or node,
         ) from None
-    except Exception as e:  # noqa: BLE001
+    except Exception as e:
         # Remove the top frame pointing to the `eval` call from the stack trace
         tb = e.__traceback__.tb_next if e.__traceback__ else None
         raise GuppyError(
             "Error occurred while evaluating Python expression:\n\n"
             + "".join(traceback.format_exception(type(e), e, tb)),
             node,
         ) from e
@@ -936,19 +992,19 @@
 def python_value_to_guppy_type(v: Any, node: ast.expr, globals: Globals) -> Type | None:
     """Turns a primitive Python value into a Guppy type.
 
     Returns `None` if the Python value cannot be represented in Guppy.
     """
     match v:
         case bool():
-            return globals.type_defs["bool"].check_instantiate([])
+            return bool_type()
         case int():
-            return globals.type_defs["int"].check_instantiate([])
+            return cast(TypeDef, globals["int"]).check_instantiate([], globals)
         case float():
-            return globals.type_defs["float"].check_instantiate([])
+            return cast(TypeDef, globals["float"]).check_instantiate([], globals)
         case tuple(elts):
             tys = [python_value_to_guppy_type(elt, node, globals) for elt in elts]
             if any(ty is None for ty in tys):
                 return None
             return TupleType(cast(list[Type], tys))
         case list():
             return _python_list_to_guppy_type(v, node, globals)
@@ -958,15 +1014,17 @@
                 import pytket
 
                 if isinstance(v, pytket.circuit.Circuit):
                     # We also need tket2 installed
                     try:
                         import tket2  # type: ignore[import-untyped, import-not-found, unused-ignore]  # noqa: F401
 
-                        qubit = globals.type_defs["qubit"].check_instantiate([])
+                        qubit = cast(TypeDef, globals["qubit"]).check_instantiate(
+                            [], globals
+                        )
                         return FunctionType(
                             [qubit] * v.n_qubits,
                             row_to_type(
                                 [qubit] * v.n_qubits + [bool_type()] * v.n_bits
                             ),
                         )
                     except ImportError:
```

### Comparing `guppylang-0.2.0/guppylang/checker/func_checker.py` & `guppylang-0.3.0/guppylang/checker/func_checker.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,87 +2,45 @@
 
 For top-level functions, we take the `DefinedFunction` containing the `ast.FunctionDef`
 node straight from the Python AST. We build a CFG, check it, and return a
 `CheckedFunction` containing a `CheckedCFG` with type annotations.
 """
 
 import ast
-from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
-from guppylang.ast_util import AstNode, return_nodes_in_ast, with_loc
+from guppylang.ast_util import return_nodes_in_ast, with_loc
 from guppylang.cfg.bb import BB
 from guppylang.cfg.builder import CFGBuilder
 from guppylang.checker.cfg_checker import CheckedCFG, check_cfg
-from guppylang.checker.core import CallableVariable, Context, Globals, Variable
-from guppylang.checker.expr_checker import check_call, synthesize_call
+from guppylang.checker.core import Context, Globals, Variable
+from guppylang.definition.common import DefId
 from guppylang.error import GuppyError
-from guppylang.nodes import CheckedNestedFunctionDef, GlobalCall, NestedFunctionDef
+from guppylang.nodes import CheckedNestedFunctionDef, NestedFunctionDef
 from guppylang.tys.parsing import type_from_ast
-from guppylang.tys.subst import Subst
-from guppylang.tys.ty import FunctionType, NoneType, Type
+from guppylang.tys.ty import FunctionType, NoneType
 
 if TYPE_CHECKING:
     from guppylang.tys.param import Parameter
 
 
-@dataclass
-class DefinedFunction(CallableVariable):
-    """A user-defined function"""
-
-    ty: FunctionType
-    defined_at: ast.FunctionDef
-
-    @staticmethod
-    def from_ast(
-        func_def: ast.FunctionDef, name: str, globals: Globals
-    ) -> "DefinedFunction":
-        ty = check_signature(func_def, globals)
-        if ty.parametrized:
-            raise GuppyError(
-                "Generic function definitions are not supported yet", func_def
-            )
-        return DefinedFunction(name, ty, func_def, None)
-
-    def check_call(
-        self, args: list[ast.expr], ty: Type, node: AstNode, ctx: Context
-    ) -> tuple[ast.expr, Subst]:
-        # Use default implementation from the expression checker
-        args, subst, inst = check_call(self.ty, args, ty, node, ctx)
-        return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), subst
-
-    def synthesize_call(
-        self, args: list[ast.expr], node: AstNode, ctx: Context
-    ) -> tuple[GlobalCall, Type]:
-        # Use default implementation from the expression checker
-        args, ty, inst = synthesize_call(self.ty, args, node, ctx)
-        return with_loc(node, GlobalCall(func=self, args=args, type_args=inst)), ty
-
-
-@dataclass
-class CheckedFunction(DefinedFunction):
-    """Type checked version of a user-defined function"""
-
-    cfg: CheckedCFG
-
-
-def check_global_func_def(func: DefinedFunction, globals: Globals) -> CheckedFunction:
+def check_global_func_def(
+    func_def: ast.FunctionDef, ty: FunctionType, globals: Globals
+) -> CheckedCFG:
     """Type checks a top-level function definition."""
-    func_def = func.defined_at
     args = func_def.args.args
-    returns_none = isinstance(func.ty.output, NoneType)
-    assert func.ty.input_names is not None
+    returns_none = isinstance(ty.output, NoneType)
+    assert ty.input_names is not None
 
     cfg = CFGBuilder().build(func_def.body, returns_none, globals)
     inputs = [
         Variable(x, ty, loc, None)
-        for x, ty, loc in zip(func.ty.input_names, func.ty.inputs, args)
+        for x, ty, loc in zip(ty.input_names, ty.inputs, args)
     ]
-    cfg = check_cfg(cfg, inputs, func.ty.output, globals)
-    return CheckedFunction(func_def.name, func.ty, func_def, None, cfg)
+    return check_cfg(cfg, inputs, ty.output, globals)
 
 
 def check_nested_func_def(
     func_def: NestedFunctionDef, bb: BB, ctx: Context
 ) -> CheckedNestedFunctionDef:
     """Type checks a local (nested) function definition."""
     func_ty = check_signature(func_def, ctx.globals)
@@ -128,31 +86,38 @@
                 )
 
     # Construct inputs for checking the body CFG
     inputs = list(captured.values()) + [
         Variable(x, ty, func_def.args.args[i], None)
         for i, (x, ty) in enumerate(zip(func_ty.input_names, func_ty.inputs))
     ]
+    def_id = DefId.fresh()
     globals = ctx.globals
 
     # Check if the body contains a free (recursive) occurrence of the function name.
     # By checking if the name is free at the entry BB, we avoid false positives when
     # a user shadows the name with a local variable
     if func_def.name in cfg.live_before[cfg.entry_bb]:
         if not captured:
             # If there are no captured vars, we treat the function like a global name
-            func = DefinedFunction(func_def.name, func_ty, func_def, None)
-            globals = ctx.globals | Globals({func_def.name: func}, {}, {}, {})
+            from guppylang.definition.function import ParsedFunctionDef
 
+            func = ParsedFunctionDef(
+                def_id, func_def.name, func_def, func_ty, globals.python_scope
+            )
+            globals = ctx.globals | Globals(
+                {func.id: func}, {func_def.name: func.id}, {}, {}
+            )
         else:
             # Otherwise, we treat it like a local name
             inputs.append(Variable(func_def.name, func_def.ty, func_def, None))
 
     checked_cfg = check_cfg(cfg, inputs, func_ty.output, globals)
     checked_def = CheckedNestedFunctionDef(
+        def_id,
         checked_cfg,
         func_ty,
         captured,
         name=func_def.name,
         args=func_def.args,
         body=func_def.body,
         decorator_list=func_def.decorator_list,
@@ -183,24 +148,24 @@
             raise GuppyError(
                 "Return type must be annotated. Try adding a `-> None` annotation.",
                 func_def,
             )
         raise GuppyError("Return type must be annotated", func_def)
 
     # TODO: Prepopulate mapping when using Python 3.12 style generic functions
-    type_var_mapping: dict[str, "Parameter"] = {}
+    param_var_mapping: dict[str, "Parameter"] = {}
     input_tys = []
     input_names = []
     for inp in func_def.args.args:
         if inp.annotation is None:
             raise GuppyError("Argument type must be annotated", inp)
-        ty = type_from_ast(inp.annotation, globals, type_var_mapping)
+        ty = type_from_ast(inp.annotation, globals, param_var_mapping)
         input_tys.append(ty)
         input_names.append(inp.arg)
-    ret_type = type_from_ast(func_def.returns, globals, type_var_mapping)
+    ret_type = type_from_ast(func_def.returns, globals, param_var_mapping)
 
     return FunctionType(
         input_tys,
         ret_type,
         input_names,
-        sorted(type_var_mapping.values(), key=lambda v: v.idx),
+        sorted(param_var_mapping.values(), key=lambda v: v.idx),
     )
```

### Comparing `guppylang-0.2.0/guppylang/checker/stmt_checker.py` & `guppylang-0.3.0/guppylang/checker/stmt_checker.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/compiler/cfg_compiler.py` & `guppylang-0.3.0/guppylang/compiler/cfg_compiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     DFContainer,
     PortVariable,
     is_return_var,
     return_var,
 )
 from guppylang.compiler.expr_compiler import ExprCompiler
 from guppylang.compiler.stmt_compiler import StmtCompiler
-from guppylang.hugr.hugr import CFNode, Hugr, Node, OutPortV
-from guppylang.tys.definition import is_bool_type
-from guppylang.tys.ty import SumType, TupleType, type_to_row
+from guppylang.hugr_builder.hugr import CFNode, Hugr, Node, OutPortV
+from guppylang.tys.builtin import is_bool_type
+from guppylang.tys.ty import SumType, row_to_type, type_to_row
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
 
 def compile_cfg(
     cfg: CheckedCFG, graph: Hugr, parent: Node, globals: CompiledGlobals
@@ -61,17 +61,16 @@
 
     # If we branch, we also have to compile the branch predicate
     if len(bb.successors) > 1:
         assert bb.branch_pred is not None
         branch_port = ExprCompiler(graph, globals).compile(bb.branch_pred, dfg)
     else:
         # Even if we don't branch, we still have to add a `Sum(())` predicates
-        unit = graph.add_make_tuple([], parent=block).out_port(0)
         branch_port = graph.add_tag(
-            variants=[TupleType([])], tag=0, inp=unit, parent=block
+            variants=[[]], tag=0, inputs=[], parent=block
         ).out_port(0)
 
     # Finally, we have to add the block output.
     outputs: Sequence[Variable]
     if len(bb.successors) == 1:
         # The easy case is if we don't branch: We just output all variables that are
         # specified by the signature
@@ -88,15 +87,19 @@
             # (since they are shared between all successors). This is in line with the
             # ordering on variables which puts linear variables at the end. The only
             # exception are return vars which must be outputted in order.
             branch_port = choose_vars_for_tuple_sum(
                 graph=graph,
                 unit_sum=branch_port,
                 output_vars=[
-                    [v for v in row if not v.ty.linear or is_return_var(v.name)]
+                    [
+                        v
+                        for v in sort_vars(row)
+                        if not v.ty.linear or is_return_var(v.name)
+                    ]
                     for row in bb.sig.output_rows
                 ],
                 dfg=dfg,
             )
             outputs = [v for v in first if v.ty.linear and not is_return_var(v.name)]
 
     graph.add_output(
@@ -129,38 +132,31 @@
 
 
 def choose_vars_for_tuple_sum(
     graph: Hugr, unit_sum: OutPortV, output_vars: list[VarRow], dfg: DFContainer
 ) -> OutPortV:
     """Selects an output based on a TupleSum.
 
-    Given `unit_sum: Sum((), (), ...)` and output variable sets `#s1, #s2, ...`,
-    constructs a TupleSum value of type `Sum(Tuple(#s1), Tuple(#s2), ...)`.
+    Given `unit_sum: Sum(*(), *(), ...)` and output variable rows `#s1, #s2, ...`,
+    constructs a TupleSum value of type `Sum(#s1, #s2, ...)`.
     """
     assert isinstance(unit_sum.ty, SumType) or is_bool_type(unit_sum.ty)
     assert len(output_vars) == (
         len(unit_sum.ty.element_types) if isinstance(unit_sum.ty, SumType) else 2
     )
-    tuples = [
-        graph.add_make_tuple(
-            inputs=[dfg[v.name].port for v in sort_vars(vs) if v.name in dfg],
-            parent=dfg.node,
-        ).out_port(0)
-        for vs in output_vars
-    ]
-    tys = [t.ty for t in tuples]
-    conditional = graph.add_conditional(
-        cond_input=unit_sum, inputs=tuples, parent=dfg.node
-    )
-    for i, _ty in enumerate(tys):
+    assert all(not v.ty.linear for var_row in output_vars for v in var_row)
+    conditional = graph.add_conditional(cond_input=unit_sum, inputs=[], parent=dfg.node)
+    tys = [[v.ty for v in var_row] for var_row in output_vars]
+    for i, var_row in enumerate(output_vars):
         case = graph.add_case(conditional)
-        inp = graph.add_input(output_tys=tys, parent=case).out_port(i)
-        tag = graph.add_tag(variants=tys, tag=i, inp=inp, parent=case).out_port(0)
+        graph.add_input(output_tys=[], parent=case)
+        inputs = [dfg[v.name].port for v in var_row]
+        tag = graph.add_tag(variants=tys, tag=i, inputs=inputs, parent=case).out_port(0)
         graph.add_output(inputs=[tag], parent=case)
-    return conditional.add_out_port(SumType(tys))
+    return conditional.add_out_port(SumType([row_to_type(row) for row in tys]))
 
 
 def compare_var(x: Variable, y: Variable) -> int:
     """Defines a `<` order on variables.
 
     We use this to determine in which order variables are outputted from basic blocks.
     We need to output linear variables at the end, so we do a lexicographic ordering of
```

### Comparing `guppylang-0.2.0/guppylang/compiler/core.py` & `guppylang-0.3.0/guppylang/compiler/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from abc import ABC, abstractmethod
+from abc import ABC
 from collections.abc import Iterator
 from dataclasses import dataclass
 
 from guppylang.ast_util import AstNode
-from guppylang.checker.core import CallableVariable, Variable
-from guppylang.hugr.hugr import DFContainingNode, Hugr, OutPortV
-from guppylang.tys.subst import Inst
-from guppylang.tys.ty import FunctionType
+from guppylang.checker.core import Variable
+from guppylang.definition.common import CompiledDef, DefId
+from guppylang.hugr_builder.hugr import DFContainingNode, Hugr, OutPortV
 
 
 @dataclass
 class PortVariable(Variable):
     """Represents a local variable in a dataflow graph.
 
     Local variables are associated with a port in the Hugr.
@@ -25,43 +24,15 @@
         defined_at: AstNode | None,
         used: AstNode | None = None,
     ) -> None:
         super().__init__(name, port.ty, defined_at, used)
         object.__setattr__(self, "port", port)
 
 
-class CompiledVariable(ABC, Variable):
-    """Abstract base class for compiled global module-level variables."""
-
-    @abstractmethod
-    def load(
-        self, dfg: "DFContainer", graph: Hugr, globals: "CompiledGlobals", node: AstNode
-    ) -> OutPortV:
-        """Loads the variable as a value into a local dataflow graph."""
-
-
-class CompiledFunction(CompiledVariable, CallableVariable):
-    """Abstract base class a global module-level function."""
-
-    ty: FunctionType
-
-    @abstractmethod
-    def compile_call(
-        self,
-        args: list[OutPortV],
-        type_args: Inst,
-        dfg: "DFContainer",
-        graph: Hugr,
-        globals: "CompiledGlobals",
-        node: AstNode,
-    ) -> list[OutPortV]:
-        """Compiles a call to the function."""
-
-
-CompiledGlobals = dict[str, CompiledVariable]
+CompiledGlobals = dict[DefId, CompiledDef]
 CompiledLocals = dict[str, PortVariable]
 
 
 @dataclass
 class DFContainer:
     """A dataflow graph under construction.
```

### Comparing `guppylang-0.2.0/guppylang/compiler/expr_compiler.py` & `guppylang-0.3.0/guppylang/compiler/expr_compiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 import ast
 import json
 from collections.abc import Iterator
 from contextlib import contextmanager
-from typing import Any
+from typing import Any, TypeGuard, TypeVar
+
+from hugr.serialization import ops
 
 from guppylang.ast_util import AstVisitor, get_type, with_loc, with_type
 from guppylang.cfg.builder import tmp_vars
 from guppylang.compiler.core import (
-    CompiledFunction,
     CompilerBase,
     DFContainer,
     PortVariable,
 )
+from guppylang.definition.value import CompiledCallableDef, CompiledValueDef
 from guppylang.error import GuppyError, InternalGuppyError
-from guppylang.hugr import ops, val
-from guppylang.hugr.hugr import DFContainingNode, OutPortV, VNode
+from guppylang.hugr_builder.hugr import (
+    UNDEFINED,
+    DFContainingNode,
+    DummyOp,
+    OutPortV,
+    VNode,
+)
 from guppylang.nodes import (
     DesugaredGenerator,
     DesugaredListComp,
     GlobalCall,
     GlobalName,
     LocalCall,
     LocalName,
+    TensorCall,
     TypeApply,
 )
-from guppylang.tys.definition import bool_type, get_element_type, is_list_type
+from guppylang.tys.builtin import bool_type, get_element_type, is_list_type
 from guppylang.tys.subst import Inst
 from guppylang.tys.ty import (
     BoundTypeVar,
     FunctionType,
     NoneType,
     TupleType,
     Type,
@@ -142,109 +150,171 @@
             return self.graph.add_load_constant(const).out_port(0)
         raise InternalGuppyError("Unsupported constant expression in compiler")
 
     def visit_LocalName(self, node: LocalName) -> OutPortV:
         return self.dfg[node.id].port
 
     def visit_GlobalName(self, node: GlobalName) -> OutPortV:
-        return self.globals[node.id].load(self.dfg, self.graph, self.globals, node)
+        defn = self.globals[node.def_id]
+        assert isinstance(defn, CompiledValueDef)
+        if isinstance(defn, CompiledCallableDef) and defn.ty.parametrized:
+            raise GuppyError(
+                "Usage of polymorphic functions as dynamic higher-order values is not "
+                "supported yet",
+                node,
+            )
+        return defn.load(self.dfg, self.graph, self.globals, node)
 
     def visit_Name(self, node: ast.Name) -> OutPortV:
         raise InternalGuppyError("Node should have been removed during type checking.")
 
     def visit_Tuple(self, node: ast.Tuple) -> OutPortV:
         return self.graph.add_make_tuple(
             inputs=[self.visit(e) for e in node.elts]
         ).out_port(0)
 
     def visit_List(self, node: ast.List) -> OutPortV:
         # Note that this is a list literal (i.e. `[e1, e2, ...]`), not a comprehension
         return self.graph.add_node(
-            ops.DummyOp(name="MakeList"), inputs=[self.visit(e) for e in node.elts]
+            DummyOp("MakeList"), inputs=[self.visit(e) for e in node.elts]
         ).add_out_port(get_type(node))
 
-    def _pack_returns(self, returns: list[OutPortV]) -> OutPortV:
+    def _unpack_tuple(self, wire: OutPortV) -> list[OutPortV]:
+        unpack_node = self.graph.add_unpack_tuple(wire, self.dfg.node)
+        return list(unpack_node.out_ports)
+
+    def _pack_returns(self, returns: list[OutPortV], return_ty: Type) -> OutPortV:
         """Groups function return values into a tuple"""
-        if len(returns) != 1:
+        if isinstance(return_ty, TupleType | NoneType) and not return_ty.preserve:
+            assert len(returns) == (
+                len(return_ty.element_types) if isinstance(return_ty, TupleType) else 0
+            )
             return self.graph.add_make_tuple(inputs=returns).out_port(0)
+        assert len(returns) == 1
         return returns[0]
 
     def visit_LocalCall(self, node: LocalCall) -> OutPortV:
         func = self.visit(node.func)
         assert isinstance(func.ty, FunctionType)
 
         args = [self.visit(arg) for arg in node.args]
         call = self.graph.add_indirect_call(func, args)
         rets = [call.out_port(i) for i in range(len(type_to_row(func.ty.output)))]
-        return self._pack_returns(rets)
+        return self._pack_returns(rets, func.ty.output)
+
+    def visit_TensorCall(self, node: TensorCall) -> OutPortV:
+        func = self.visit(node.func)
+        args = [self.visit(arg) for arg in node.args]
+
+        assert isinstance(func.ty, TupleType)
+
+        rets: list[OutPortV] = []
+        remaining_args = args
+        for elem in self._unpack_tuple(func):
+            outs, remaining_args = self._compile_tensor_with_leftovers(
+                elem, remaining_args
+            )
+            rets.extend(outs)
+        assert remaining_args == []
+
+        return self._pack_returns(rets, node.out_tys)
+
+    def _compile_tensor_with_leftovers(
+        self, func: OutPortV, args: list[OutPortV]
+    ) -> tuple[
+        list[OutPortV],  # Compiled outputs
+        list[OutPortV],
+    ]:  # Leftover args
+        if isinstance(func.ty, TupleType):
+            remaining_args = args
+            all_outs = []
+            for elem in self._unpack_tuple(func):
+                outs, remaining_args = self._compile_tensor_with_leftovers(
+                    elem, remaining_args
+                )
+                all_outs.extend(outs)
+            return all_outs, remaining_args
+
+        elif isinstance(func.ty, FunctionType):
+            input_len = len(func.ty.inputs)
+            call = self.graph.add_indirect_call(func, args[0:input_len])
+
+            return list(call.out_ports), args[input_len:]
+        else:
+            raise InternalGuppyError("Tensor element wasn't function or tuple")
 
     def visit_GlobalCall(self, node: GlobalCall) -> OutPortV:
-        func = self.globals[node.func.name]
-        assert isinstance(func, CompiledFunction)
+        func = self.globals[node.def_id]
+        assert isinstance(func, CompiledCallableDef)
 
         args = [self.visit(arg) for arg in node.args]
         rets = func.compile_call(
             args, list(node.type_args), self.dfg, self.graph, self.globals, node
         )
-        return self._pack_returns(rets)
+        return self._pack_returns(rets, func.ty.output)
 
     def visit_Call(self, node: ast.Call) -> OutPortV:
         raise InternalGuppyError("Node should have been removed during type checking.")
 
     def visit_TypeApply(self, node: TypeApply) -> OutPortV:
-        func = self.visit(node.value)
-        assert isinstance(func.ty, FunctionType)
-        ta = self.graph.add_type_apply(func, node.inst, self.dfg.node).out_port(0)
+        # For now, we can only TypeApply global FunctionDefs/Decls.
+        if not isinstance(node.value, GlobalName):
+            raise InternalGuppyError("Dynamic TypeApply not supported yet!")
+        defn = self.globals[node.value.def_id]
+        assert isinstance(defn, CompiledCallableDef)
 
         # We have to be very careful here: If we instantiate `foo: forall T. T -> T`
         # with a tuple type `tuple[A, B]`, we get the type `tuple[A, B] -> tuple[A, B]`.
         # Normally, this would be represented in Hugr as a function with two output
         # ports types A and B. However, when TypeApplying `foo`, we actually get a
         # function with a single output port typed `tuple[A, B]`.
         # TODO: We would need to do manual monomorphisation in that case to obtain a
         #  function that returns two ports as expected
-        if instantiation_needs_unpacking(func.ty, node.inst):
+        if instantiation_needs_unpacking(defn.ty, node.inst):
             raise GuppyError(
                 "Generic function instantiations returning rows are not supported yet",
                 node,
             )
 
-        return ta
+        return defn.load_with_args(node.inst, self.dfg, self.graph, self.globals, node)
 
     def visit_UnaryOp(self, node: ast.UnaryOp) -> OutPortV:
         # The only case that is not desugared by the type checker is the `not` operation
         # since it is not implemented via a dunder method
         if isinstance(node.op, ast.Not):
             arg = self.visit(node.operand)
-            return self.graph.add_node(
-                ops.CustomOp(extension="logic", op_name="Not", args=[]), inputs=[arg]
-            ).add_out_port(bool_type())
+            op = ops.CustomOp(
+                extension="logic", op_name="Not", args=[], parent=UNDEFINED
+            )
+            return self.graph.add_node(ops.OpType(op), inputs=[arg]).add_out_port(
+                bool_type()
+            )
 
         raise InternalGuppyError("Node should have been removed during type checking.")
 
     def visit_DesugaredListComp(self, node: DesugaredListComp) -> OutPortV:
         from guppylang.compiler.stmt_compiler import StmtCompiler
 
         compiler = StmtCompiler(self.graph, self.globals)
 
         # Make up a name for the list under construction and bind it to an empty list
         list_ty = get_type(node)
         list_name = with_type(list_ty, with_loc(node, LocalName(id=next(tmp_vars))))
-        empty_list = self.graph.add_node(ops.DummyOp(name="MakeList"))
+        empty_list = self.graph.add_node(DummyOp("MakeList"))
         self.dfg[list_name.id] = PortVariable(
             list_name.id, empty_list.add_out_port(list_ty), node, None
         )
 
         def compile_generators(elt: ast.expr, gens: list[DesugaredGenerator]) -> None:
             """Helper function to generate nested TailLoop nodes for generators"""
             # If there are no more generators left, just append the element to the list
             if not gens:
                 list_port, elt_port = self.visit(list_name), self.visit(elt)
                 push = self.graph.add_node(
-                    ops.DummyOp(name="Push"), inputs=[list_port, elt_port]
+                    DummyOp("Push"), inputs=[list_port, elt_port]
                 )
                 self.dfg[list_name.id].port = push.add_out_port(list_port.ty)
                 return
 
             # Otherwise, compile the first iterator and construct a TailLoop
             gen, *gens = gens
             compiler.compile_stmts([gen.iter_assign], self.dfg)
@@ -292,15 +362,15 @@
     """Checks if instantiating a polymorphic makes it return a row."""
     if isinstance(func_ty.output, BoundTypeVar):
         return_ty = inst[func_ty.output.idx]
         return isinstance(return_ty, TupleType | NoneType)
     return False
 
 
-def python_value_to_hugr(v: Any, exp_ty: Type) -> val.Value | None:
+def python_value_to_hugr(v: Any, exp_ty: Type) -> ops.Value | None:
     """Turns a Python value into a Hugr value.
 
     Returns None if the Python value cannot be represented in Guppy.
     """
     from guppylang.prelude._internal import (
         bool_value,
         float_value,
@@ -317,31 +387,37 @@
             return float_value(v)
         case tuple(elts):
             assert isinstance(exp_ty, TupleType)
             vs = [
                 python_value_to_hugr(elt, ty)
                 for elt, ty in zip(elts, exp_ty.element_types)
             ]
-            if any(value is None for value in vs):
-                return None
-            return val.Tuple(vs=vs)
+            if doesnt_contain_none(vs):
+                return ops.Value(ops.TupleValue(vs=vs))
         case list(elts):
             assert is_list_type(exp_ty)
-            return list_value(
-                [python_value_to_hugr(elt, get_element_type(exp_ty)) for elt in elts],
-                get_element_type(exp_ty).to_hugr(),
-            )
+            vs = [python_value_to_hugr(elt, get_element_type(exp_ty)) for elt in elts]
+            if doesnt_contain_none(vs):
+                return list_value(vs, get_element_type(exp_ty))
         case _:
             # Pytket conversion is an optional feature
             try:
                 import pytket
 
                 if isinstance(v, pytket.circuit.Circuit):
                     from tket2.circuit import (  # type: ignore[import-untyped, import-not-found, unused-ignore]
                         Tk2Circuit,
                     )
 
-                    hugr = json.loads(Tk2Circuit(v).to_hugr_json())
-                    return val.FunctionVal(hugr=hugr)
+                    hugr = json.loads(Tk2Circuit(v).to_hugr_json())  # type: ignore[attr-defined, unused-ignore]
+                    return ops.Value(ops.FunctionValue(hugr=hugr))
             except ImportError:
                 pass
-            return None
+    return None
+
+
+T = TypeVar("T")
+
+
+def doesnt_contain_none(xs: list[T | None]) -> TypeGuard[list[T]]:
+    """Checks if a list contains `None`."""
+    return all(x is not None for x in xs)
```

### Comparing `guppylang-0.2.0/guppylang/compiler/func_compiler.py` & `guppylang-0.3.0/guppylang/compiler/func_compiler.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,72 +1,40 @@
-from dataclasses import dataclass
+from typing import TYPE_CHECKING
 
-from guppylang.ast_util import AstNode
-from guppylang.checker.func_checker import CheckedFunction, DefinedFunction
 from guppylang.compiler.cfg_compiler import compile_cfg
 from guppylang.compiler.core import (
-    CompiledFunction,
     CompiledGlobals,
     DFContainer,
     PortVariable,
 )
-from guppylang.hugr.hugr import DFContainingVNode, Hugr, OutPortV
+from guppylang.hugr_builder.hugr import DFContainingVNode, Hugr
 from guppylang.nodes import CheckedNestedFunctionDef
-from guppylang.tys.subst import Inst
 from guppylang.tys.ty import FunctionType, type_to_row
 
-
-@dataclass
-class CompiledFunctionDef(DefinedFunction, CompiledFunction):
-    node: DFContainingVNode
-
-    def load(
-        self, dfg: DFContainer, graph: Hugr, globals: CompiledGlobals, node: AstNode
-    ) -> OutPortV:
-        return graph.add_load_constant(self.node.out_port(0), dfg.node).out_port(0)
-
-    def compile_call(
-        self,
-        args: list[OutPortV],
-        type_args: Inst,
-        dfg: DFContainer,
-        graph: Hugr,
-        globals: CompiledGlobals,
-        node: AstNode,
-    ) -> list[OutPortV]:
-        # TODO: Hugr should probably allow us to pass type args to `Call`, so we can
-        #   avoid loading the function to manually add a `TypeApply`
-        if type_args:
-            func = graph.add_load_constant(self.node.out_port(0), dfg.node)
-            func = graph.add_type_apply(func.out_port(0), type_args, dfg.node)
-            call = graph.add_indirect_call(func.out_port(0), args, dfg.node)
-        else:
-            call = graph.add_call(self.node.out_port(0), args, dfg.node)
-        return [call.out_port(i) for i in range(len(type_to_row(self.ty.output)))]
+if TYPE_CHECKING:
+    from guppylang.definition.function import CheckedFunctionDef
 
 
 def compile_global_func_def(
-    func: CheckedFunction,
+    func: "CheckedFunctionDef",
     def_node: DFContainingVNode,
     graph: Hugr,
     globals: CompiledGlobals,
-) -> CompiledFunctionDef:
+) -> None:
     """Compiles a top-level function definition to Hugr."""
     _, ports = graph.add_input_with_ports(list(func.ty.inputs), def_node)
     cfg_node = graph.add_cfg(def_node, ports)
     compile_cfg(func.cfg, graph, cfg_node, globals)
 
     # Add output node for the cfg
     graph.add_output(
         inputs=[cfg_node.add_out_port(ty) for ty in type_to_row(func.cfg.output_ty)],
         parent=def_node,
     )
 
-    return CompiledFunctionDef(func.name, func.ty, func.defined_at, None, def_node)
-
 
 def compile_local_func_def(
     func: CheckedNestedFunctionDef,
     dfg: DFContainer,
     graph: Hugr,
     globals: CompiledGlobals,
 ) -> PortVariable:
@@ -88,37 +56,47 @@
         list(closure_ty.inputs), def_node
     )
 
     # If we have captured variables and the body contains a recursive occurrence of
     # the function itself, then we provide the partially applied function as a local
     # variable
     if len(captured) > 0 and func.name in func.cfg.live_before[func.cfg.entry_bb]:
-        loaded = graph.add_load_constant(def_node.out_port(0), def_node).out_port(0)
+        loaded = graph.add_load_function(def_node.out_port(0), [], def_node).out_port(0)
         partial = graph.add_partial(
             loaded, [def_input.out_port(i) for i in range(len(captured))], def_node
         )
         input_ports.append(partial.out_port(0))
         func.cfg.input_tys.append(func.ty)
     else:
         # Otherwise, we treat the function like a normal global variable
+        from guppylang.definition.function import CompiledFunctionDef
+
         globals = globals | {
-            func.name: CompiledFunctionDef(func.name, func.ty, func, None, def_node)
+            func.def_id: CompiledFunctionDef(
+                func.def_id,
+                func.name,
+                func,
+                func.ty,
+                {},
+                func.cfg,
+                def_node,
+            )
         }
 
     # Compile the CFG
     cfg_node = graph.add_cfg(def_node, inputs=input_ports)
     compile_cfg(func.cfg, graph, cfg_node, globals)
 
     # Add output node for the cfg
     graph.add_output(
         inputs=[cfg_node.add_out_port(ty) for ty in type_to_row(func.cfg.output_ty)],
         parent=def_node,
     )
 
     # Finally, load the function into the local data-flow graph
-    loaded = graph.add_load_constant(def_node.out_port(0), dfg.node).out_port(0)
+    loaded = graph.add_load_function(def_node.out_port(0), [], dfg.node).out_port(0)
     if len(captured) > 0:
         loaded = graph.add_partial(
             loaded, [dfg[v.name].port for v in captured], dfg.node
         ).out_port(0)
 
     return PortVariable(func.name, loaded, func)
```

### Comparing `guppylang-0.2.0/guppylang/compiler/stmt_compiler.py` & `guppylang-0.3.0/guppylang/compiler/stmt_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     CompilerBase,
     DFContainer,
     PortVariable,
     return_var,
 )
 from guppylang.compiler.expr_compiler import ExprCompiler
 from guppylang.error import InternalGuppyError
-from guppylang.hugr.hugr import Hugr, OutPortV
+from guppylang.hugr_builder.hugr import Hugr, OutPortV
 from guppylang.nodes import CheckedNestedFunctionDef
 from guppylang.tys.ty import TupleType
 
 
 class StmtCompiler(CompilerBase, AstVisitor[None]):
     """A compiler for Guppy statements to Hugr"""
```

### Comparing `guppylang-0.2.0/guppylang/custom.py` & `guppylang-0.3.0/guppylang/definition/custom.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,173 +1,185 @@
 import ast
 from abc import ABC, abstractmethod
+from dataclasses import dataclass, field
+
+from hugr.serialization import ops
 
 from guppylang.ast_util import AstNode, get_type, with_loc, with_type
 from guppylang.checker.core import Context, Globals
 from guppylang.checker.expr_checker import check_call, synthesize_call
 from guppylang.checker.func_checker import check_signature
-from guppylang.compiler.core import CompiledFunction, CompiledGlobals, DFContainer
+from guppylang.compiler.core import CompiledGlobals, DFContainer
+from guppylang.definition.common import ParsableDef
+from guppylang.definition.value import CompiledCallableDef
 from guppylang.error import GuppyError, InternalGuppyError
-from guppylang.hugr import ops
-from guppylang.hugr.hugr import DFContainingVNode, Hugr, Node, OutPortV
+from guppylang.hugr_builder.hugr import Hugr, Node, OutPortV
 from guppylang.nodes import GlobalCall
 from guppylang.tys.subst import Inst, Subst
 from guppylang.tys.ty import FunctionType, NoneType, Type, type_to_row
 
 
-class CustomFunction(CompiledFunction):
-    """A function whose type checking and compilation behaviour can be customised."""
+@dataclass(frozen=True)
+class RawCustomFunctionDef(ParsableDef):
+    """A raw custom function definition provided by the user.
+
+    Custom functions provide their own checking and compilation logic using a
+    `CustomCallChecker` and a `CustomCallCompiler`.
+
+    The raw definition stores exactly what the user has written (i.e. the AST together
+    with the provided checker and compiler), without inspecting the signature.
+    """
 
-    defined_at: ast.FunctionDef | None
+    defined_at: ast.FunctionDef
+    call_checker: "CustomCallChecker"
+    call_compiler: "CustomCallCompiler"
 
     # Whether the function may be used as a higher-order value. This is only possible
     # if a static type for the function is provided.
     higher_order_value: bool
 
-    call_checker: "CustomCallChecker"
-    call_compiler: "CustomCallCompiler"
+    description: str = field(default="function", init=False)
+
+    def parse(self, globals: "Globals") -> "CustomFunctionDef":
+        """Parses and checks the user-provided signature of the custom function.
 
-    _ty: FunctionType | None = None
-    _defined: dict[Node, DFContainingVNode] = {}  # noqa: RUF012
+        The signature is optional if custom type checking logic is provided by the user.
+        However, note that the signature annotation is required, if we want to use the
+        function as a higher-order value.
+
+        If no signature is provided, we fill in the dummy signature `() -> ()`. This
+        type will never be inspected, since we rely on the provided custom checking
+        code. The only information we need to access is that it's a function type and
+        that there are no unsolved existential vars.
+        """
+        # Type annotations are needed if we rely on the default call checker or want
+        # to allow the usage of the function as a higher-order value
+        requires_type_annotation = (
+            isinstance(self.call_checker, DefaultCallChecker) or self.higher_order_value
+        )
+        has_type_annotation = self.defined_at.returns or any(
+            arg.annotation for arg in self.defined_at.args.args
+        )
+
+        if requires_type_annotation and not has_type_annotation:
+            raise GuppyError(
+                f"Type signature for function `{self.name}` is required. "
+                "Alternatively, try passing `higher_order_value=False` on definition.",
+                self.defined_at,
+            )
 
-    def __init__(
+        ty = (
+            check_signature(self.defined_at, globals)
+            if requires_type_annotation
+            else FunctionType([], NoneType())
+        )
+        return CustomFunctionDef(
+            self.id,
+            self.name,
+            self.defined_at,
+            ty,
+            self.call_checker,
+            self.call_compiler,
+            self.higher_order_value,
+        )
+
+    def compile_call(
         self,
-        name: str,
-        defined_at: ast.FunctionDef | None,
-        compiler: "CustomCallCompiler",
-        checker: "CustomCallChecker",
-        higher_order_value: bool = True,
-        ty: FunctionType | None = None,
-    ):
-        self.name = name
-        self.defined_at = defined_at
-        self.higher_order_value = higher_order_value
-        self.call_compiler = compiler
-        self.call_checker = checker
-        self.used = None
-        self._ty = ty
-        self._defined = {}
-
-    @property  # type: ignore[override]
-    def ty(self) -> FunctionType:
-        if self._ty is None:
-            # If we don't have a specified type, then the extension writer has to
-            # provide their own type-checking code. Therefore, it doesn't matter which
-            # type we return here since it will never be inspected.
-            return FunctionType([], NoneType())
-        return self._ty
-
-    @ty.setter
-    def ty(self, ty: FunctionType) -> None:
-        self._ty = ty
-
-    def check_type(self, globals: Globals) -> None:
-        """Checks the type annotation on the signature declaration if provided."""
-        if self._ty is not None:
-            return
-
-        if self.defined_at is None:
-            if self.higher_order_value:
-                raise GuppyError(
-                    f"Type signature for function `{self.name}` is required. "
-                    "Alternatively, try passing `higher_order_value=False` on "
-                    "definition."
-                )
-            return
+        args: list[OutPortV],
+        type_args: Inst,
+        dfg: DFContainer,
+        graph: Hugr,
+        globals: CompiledGlobals,
+        node: AstNode,
+    ) -> list[OutPortV]:
+        """Compiles a call to the function."""
+        self.call_compiler._setup(type_args, dfg, graph, globals, node)
+        return self.call_compiler.compile(args)
 
-        try:
-            self._ty = check_signature(self.defined_at, globals)
-        except GuppyError:
-            # We can ignore the error if a custom call checker is provided and the
-            # function may not be used as a higher-order value
-            if self.call_checker is None or self.higher_order_value:
-                raise
+
+@dataclass(frozen=True)
+class CustomFunctionDef(RawCustomFunctionDef, CompiledCallableDef):
+    """A custom function with parsed and checked signature."""
+
+    ty: FunctionType
 
     def check_call(
         self, args: list[ast.expr], ty: Type, node: AstNode, ctx: Context
     ) -> tuple[ast.expr, Subst]:
+        """Checks the return type of a function call against a given type.
+
+        This is done by invoking the provided `CustomCallChecker`.
+        """
         self.call_checker._setup(ctx, node, self)
         new_node, subst = self.call_checker.check(args, ty)
         return with_type(ty, with_loc(node, new_node)), subst
 
     def synthesize_call(
         self, args: list[ast.expr], node: AstNode, ctx: "Context"
     ) -> tuple[ast.expr, Type]:
+        """Synthesizes the return type of a function call.
+
+        This is done by invoking the provided `CustomCallChecker`.
+        """
         self.call_checker._setup(ctx, node, self)
         new_node, ty = self.call_checker.synthesize(args)
         return with_type(ty, with_loc(node, new_node)), ty
 
-    def compile_call(
+    def load_with_args(
         self,
-        args: list[OutPortV],
         type_args: Inst,
-        dfg: DFContainer,
+        dfg: "DFContainer",
         graph: Hugr,
         globals: CompiledGlobals,
         node: AstNode,
-    ) -> list[OutPortV]:
-        self.call_compiler._setup(type_args, dfg, graph, globals, node)
-        return self.call_compiler.compile(args)
-
-    def load(
-        self, dfg: "DFContainer", graph: Hugr, globals: CompiledGlobals, node: AstNode
     ) -> OutPortV:
         """Loads the custom function as a value into a local dataflow graph.
 
-        This will place a `FunctionDef` node into the Hugr module if one for this
-        function doesn't already exist and loads it into the DFG. This operation will
-        fail if no function type has been specified.
+        This will place a `FunctionDef` node into the Hugr module and loads it into the
+        DFG. This operation will fail the function is not allowed to be used as a
+        higher-order value.
         """
-        if self._ty is None:
+        # TODO: This should be raised during checking, not compilation!
+        if not self.higher_order_value:
             raise GuppyError(
                 "This function does not support usage in a higher-order context",
                 node,
             )
-
-        if self._ty.parametrized:
-            raise InternalGuppyError(
-                "Can't yet generate higher-order versions of custom functions. This "
-                "requires generic function *definitions*"
-            )
+        assert len(self.ty.params) == len(type_args)
 
         # Find the module node by walking up the hierarchy
         module: Node = dfg.node
         while not isinstance(module.op, ops.Module):
             if module.parent is None:
                 raise InternalGuppyError(
                     "Encountered node that is not contained in a module."
                 )
             module = module.parent
 
-        # If the function has not yet been loaded in this module, we first have to
-        # define it. We create a `FunctionDef` that takes some inputs, compiles a call
-        # to the function, and returns the results.
-        if module not in self._defined:
-            def_node = graph.add_def(self.ty, module, self.name)
-            _, inp_ports = graph.add_input_with_ports(list(self.ty.inputs), def_node)
-            returns = self.compile_call(
-                inp_ports, [], DFContainer(def_node, {}), graph, globals, node
-            )
-            graph.add_output(returns, parent=def_node)
-            self._defined[module] = def_node
+        # We create a `FunctionDef` that takes some inputs, compiles a call to the
+        # function, and returns the results.
+        def_node = graph.add_def(self.ty, module, self.name)
+        _, inp_ports = graph.add_input_with_ports(list(self.ty.inputs), def_node)
+        returns = self.compile_call(
+            inp_ports, type_args, DFContainer(def_node, {}), graph, globals, node
+        )
+        graph.add_output(returns, parent=def_node)
 
         # Finally, load the function into the local DFG
-        return graph.add_load_constant(
-            self._defined[module].out_port(0), dfg.node
-        ).out_port(0)
+        return graph.add_load_constant(def_node.out_port(0), dfg.node).out_port(0)
 
 
 class CustomCallChecker(ABC):
-    """Protocol for custom function call type checkers."""
+    """Abstract base class for custom function call type checkers."""
 
     ctx: Context
     node: AstNode
-    func: CustomFunction
+    func: CustomFunctionDef
 
-    def _setup(self, ctx: Context, node: AstNode, func: CustomFunction) -> None:
+    def _setup(self, ctx: Context, node: AstNode, func: CustomFunctionDef) -> None:
         self.ctx = ctx
         self.node = node
         self.func = func
 
     @abstractmethod
     def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         """Checks the return value against a given type.
@@ -180,15 +192,15 @@
         """Synthesizes a type for the return value of a call.
 
         Also returns a (possibly) transformed and annotated argument list.
         """
 
 
 class CustomCallCompiler(ABC):
-    """Protocol for custom function call compilers."""
+    """Abstract base class for custom function call compilers."""
 
     type_args: Inst
     dfg: DFContainer
     graph: Hugr
     globals: CompiledGlobals
     node: AstNode
 
@@ -213,39 +225,48 @@
 
 class DefaultCallChecker(CustomCallChecker):
     """Checks function calls by comparing to a type signature."""
 
     def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         # Use default implementation from the expression checker
         args, subst, inst = check_call(self.func.ty, args, ty, self.node, self.ctx)
-        return GlobalCall(func=self.func, args=args, type_args=inst), subst
+        return GlobalCall(def_id=self.func.id, args=args, type_args=inst), subst
 
     def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         # Use default implementation from the expression checker
         args, ty, inst = synthesize_call(self.func.ty, args, self.node, self.ctx)
-        return GlobalCall(func=self.func, args=args, type_args=inst), ty
+        return GlobalCall(def_id=self.func.id, args=args, type_args=inst), ty
+
 
+class NotImplementedCallCompiler(CustomCallCompiler):
+    """Call compiler for custom functions that are already lowered during checking.
 
-class DefaultCallCompiler(CustomCallCompiler):
-    """Call compiler that invokes the regular expression compiler."""
+    For example, the custom checker could replace the call with a series of calls to
+    other functions. In that case, the original function will no longer be present and
+    thus doesn't need to be compiled.
+    """
 
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
-        raise NotImplementedError
+        raise InternalGuppyError("Function should have been removed during checking")
 
 
 class OpCompiler(CustomCallCompiler):
-    op: ops.BaseOp
+    """Call compiler for functions that are directly implemented via Hugr ops."""
 
-    def __init__(self, op: ops.BaseOp) -> None:
+    op: ops.OpType
+
+    def __init__(self, op: ops.OpType) -> None:
         self.op = op
 
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
         node = self.graph.add_node(
-            self.op.model_copy(), inputs=args, parent=self.dfg.node
+            self.op.model_copy(deep=True), inputs=args, parent=self.dfg.node
         )
         return_ty = get_type(self.node)
         return [node.add_out_port(ty) for ty in type_to_row(return_ty)]
 
 
 class NoopCompiler(CustomCallCompiler):
+    """Call compiler for functions that are noops."""
+
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
         return args
```

### Comparing `guppylang-0.2.0/guppylang/decorator.py` & `guppylang-0.3.0/guppylang/decorator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,87 @@
-import functools
 import inspect
 from collections.abc import Callable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 from types import ModuleType
 from typing import Any, TypeVar
 
+from hugr.serialization import ops, tys
+
 from guppylang.ast_util import has_empty_body
-from guppylang.custom import (
+from guppylang.definition.common import DefId
+from guppylang.definition.custom import (
     CustomCallChecker,
     CustomCallCompiler,
-    CustomFunction,
     DefaultCallChecker,
-    DefaultCallCompiler,
+    NotImplementedCallCompiler,
     OpCompiler,
+    RawCustomFunctionDef,
 )
+from guppylang.definition.declaration import RawFunctionDecl
+from guppylang.definition.function import RawFunctionDef, parse_py_func
+from guppylang.definition.parameter import TypeVarDef
+from guppylang.definition.struct import RawStructDef
+from guppylang.definition.ty import OpaqueTypeDef, TypeDef
 from guppylang.error import GuppyError, MissingModuleError, pretty_errors
-from guppylang.hugr import ops, tys
-from guppylang.hugr.hugr import Hugr
-from guppylang.module import GuppyModule, PyFunc, parse_py_func
-from guppylang.tys.definition import OpaqueTypeDef, TypeDef
+from guppylang.hugr_builder.hugr import Hugr
+from guppylang.module import GuppyModule, PyFunc
 
-FuncDecorator = Callable[[PyFunc], PyFunc | Hugr]
-CustomFuncDecorator = Callable[[PyFunc], CustomFunction]
+FuncDefDecorator = Callable[[PyFunc], RawFunctionDef]
+FuncDeclDecorator = Callable[[PyFunc], RawFunctionDecl]
+CustomFuncDecorator = Callable[[PyFunc], RawCustomFunctionDef]
 ClassDecorator = Callable[[type], type]
+StructDecorator = Callable[[type], RawStructDef]
 
 
 @dataclass(frozen=True)
 class ModuleIdentifier:
     """Identifier for the Python file/module that called the decorator."""
 
     filename: Path
-    module: ModuleType | None
-
-    @property
-    def name(self) -> str:
-        """Returns a user-friendly name for the caller.
 
-        If the called is not a function, uses the file name.
-        """
-        if self.module is not None:
-            return str(self.module.__name__)
-        return self.filename.name
+    #: The name of the module. We only store this to have nice name to report back to
+    #: the user. When determining whether two `ModuleIdentifier`s correspond to the same
+    #: module, we only take the module path into account.
+    name: str = field(compare=False)
 
 
 class _Guppy:
     """Class for the `@guppy` decorator."""
 
     # The currently-alive GuppyModules, associated with a Python file/module.
     #
     # Only contains **uncompiled** modules.
     _modules: dict[ModuleIdentifier, GuppyModule]
 
     def __init__(self) -> None:
         self._modules = {}
 
     @pretty_errors
-    def __call__(self, arg: PyFunc | GuppyModule) -> FuncDecorator:
+    def __call__(self, arg: PyFunc | GuppyModule) -> FuncDefDecorator | RawFunctionDef:
         """Decorator to annotate Python functions as Guppy code.
 
         Optionally, the `GuppyModule` in which the function should be placed can
         be passed to the decorator.
         """
-
-        def make_dummy(wraps: PyFunc) -> Callable[..., Any]:
-            @functools.wraps(wraps)
-            def dummy(*args: Any, **kwargs: Any) -> Any:
-                raise GuppyError(
-                    "Guppy functions can only be called in a Guppy context"
-                )
-
-            return dummy
-
         if not isinstance(arg, GuppyModule):
             # Decorator used without any arguments.
             # We default to a module associated with the caller of the decorator.
             f = arg
 
             caller = self._get_python_caller(f)
             if caller not in self._modules:
                 self._modules[caller] = GuppyModule(caller.name)
             module = self._modules[caller]
-            module.register_func_def(f)
-            return make_dummy(f)
+            return module.register_func_def(f)
 
         if isinstance(arg, GuppyModule):
             # Module passed.
-            def dec(f: Callable[..., Any]) -> Callable[..., Any]:
-                arg.register_func_def(f)
-                return make_dummy(f)
+            def dec(f: Callable[..., Any]) -> RawFunctionDef:
+                return arg.register_func_def(f)
 
             return dec
 
         raise ValueError(f"Invalid arguments to `@guppy` decorator: {arg}")
 
     def _get_python_caller(self, fn: PyFunc | None = None) -> ModuleIdentifier:
         """Returns an identifier for the Python file/module that called the decorator.
@@ -106,15 +95,18 @@
             for s in inspect.stack():
                 if s.filename != __file__:
                     filename = s.filename
                     module = inspect.getmodule(s.frame)
                     break
             else:
                 raise GuppyError("Could not find a caller for the `@guppy` decorator")
-        return ModuleIdentifier(Path(filename), module)
+        module_path = Path(filename)
+        return ModuleIdentifier(
+            module_path, module.__name__ if module else module_path.name
+        )
 
     @pretty_errors
     def extend_type(self, module: GuppyModule, defn: TypeDef) -> ClassDecorator:
         """Decorator to add new instance functions to a type."""
         module._instance_func_buffer = {}
 
         def dec(c: type) -> type:
@@ -137,26 +129,49 @@
         Requires the static Hugr translation of the type. Additionally, the type can be
         marked as linear. All `@guppy` annotated functions on the class are turned into
         instance functions.
         """
         module._instance_func_buffer = {}
 
         def dec(c: type) -> type:
-            _name = name or c.__name__
-            defn = OpaqueTypeDef(_name, [], linear, lambda _: hugr_ty, bound)
-            module.register_type(_name, defn)
+            defn = OpaqueTypeDef(
+                DefId.fresh(module),
+                name or c.__name__,
+                None,
+                [],
+                linear,
+                lambda _: hugr_ty,
+                bound,
+            )
+            module.register_def(defn)
             module._register_buffered_instance_funcs(defn)
             return c
 
         return dec
 
     @pretty_errors
+    def struct(self, module: GuppyModule) -> StructDecorator:
+        """Decorator to define a new struct."""
+        module._instance_func_buffer = {}
+
+        def dec(cls: type) -> RawStructDef:
+            defn = RawStructDef(DefId.fresh(module), cls.__name__, None, cls)
+            module.register_def(defn)
+            module._register_buffered_instance_funcs(defn)
+            return defn
+
+        return dec
+
+    @pretty_errors
     def type_var(self, module: GuppyModule, name: str, linear: bool = False) -> TypeVar:
         """Creates a new type variable in a module."""
-        module.register_type_var(name, linear)
+        defn = TypeVarDef(DefId.fresh(module), name, None, linear)
+        module.register_def(defn)
+        # Return an actual Python `TypeVar` so it can be used as an actual type in code
+        # that is executed by interpreter before handing it to Guppy.
         return TypeVar(name)
 
     @pretty_errors
     def custom(
         self,
         module: GuppyModule,
         compiler: CustomCallCompiler | None = None,
@@ -167,31 +182,31 @@
         """Decorator to add custom typing or compilation behaviour to function decls.
 
         Optionally, usage of the function as a higher-order value can be disabled. In
         that case, the function signature can be omitted if a custom call compiler is
         provided.
         """
 
-        def dec(f: PyFunc) -> CustomFunction:
+        def dec(f: PyFunc) -> RawCustomFunctionDef:
             func_ast = parse_py_func(f)
             if not has_empty_body(func_ast):
                 raise GuppyError(
                     "Body of custom function declaration must be empty",
                     func_ast.body[0],
                 )
             call_checker = checker or DefaultCallChecker()
-            func = CustomFunction(
+            func = RawCustomFunctionDef(
+                DefId.fresh(module),
                 name or func_ast.name,
                 func_ast,
-                compiler or DefaultCallCompiler(),
                 call_checker,
+                compiler or NotImplementedCallCompiler(),
                 higher_order_value,
             )
-            call_checker.func = func
-            module.register_custom_func(func)
+            module.register_def(func)
             return func
 
         return dec
 
     def hugr_op(
         self,
         module: GuppyModule,
@@ -199,27 +214,19 @@
         checker: CustomCallChecker | None = None,
         higher_order_value: bool = True,
         name: str = "",
     ) -> CustomFuncDecorator:
         """Decorator to annotate function declarations as HUGR ops."""
         return self.custom(module, OpCompiler(op), checker, higher_order_value, name)
 
-    def declare(self, module: GuppyModule) -> FuncDecorator:
+    def declare(self, module: GuppyModule) -> FuncDeclDecorator:
         """Decorator to declare functions"""
 
-        def dec(f: Callable[..., Any]) -> Callable[..., Any]:
-            module.register_func_decl(f)
-
-            @functools.wraps(f)
-            def dummy(*args: Any, **kwargs: Any) -> Any:
-                raise GuppyError(
-                    "Guppy functions can only be called in a Guppy context"
-                )
-
-            return dummy
+        def dec(f: Callable[..., Any]) -> RawFunctionDecl:
+            return module.register_func_decl(f)
 
         return dec
 
     def load(self, m: ModuleType | GuppyModule) -> None:
         caller = self._get_python_caller()
         if caller not in self._modules:
             self._modules[caller] = GuppyModule(caller.name)
```

### Comparing `guppylang-0.2.0/guppylang/error.py` & `guppylang-0.3.0/guppylang/error.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/hugr/hugr.py` & `guppylang-0.3.0/guppylang/hugr_builder/hugr.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 from abc import ABC, abstractmethod
 from collections.abc import Iterator, Sequence
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import Any, Optional
 
 import networkx as nx  # type: ignore[import-untyped]
+from hugr.serialization import SerialHugr, ops, tys
+from hugr.serialization import serial_hugr as raw
+from hugr.serialization.ops import OpType
 
-import guppylang.hugr.ops as ops
-import guppylang.hugr.raw as raw
-from guppylang.hugr import val
 from guppylang.tys.subst import Inst
 from guppylang.tys.ty import (
     FunctionType,
     SumType,
     TupleType,
     Type,
+    TypeRow,
     row_to_type,
+    rows_to_hugr,
     type_to_row,
 )
 
 NodeIdx = int
 PortOffset = int
 
 
@@ -64,28 +66,43 @@
     offset: None = field(default=None, init=False)
 
 
 class OutPortCF(OutPort):
     """A control-flow output port."""
 
 
+class DummyOp(OpType):
+    """A dummy Hugr op that is replaced with a call to a dummy function declaration
+    during serialisation.
+
+    This is a placeholder for ops that aren't yet available in Hugr.
+    """
+
+    root: str  # type: ignore[assignment]
+
+    @property
+    def name(self) -> str:
+        """The name of the dummy op."""
+        return self.root
+
+
 Edge = tuple[OutPort, InPort]
 
 TypeList = list[Type]
 
 
 @dataclass
 class Node(ABC):
     """Base class for a node in the graph.
 
     Has a number of input and output ports and an associated op type.
     """
 
     idx: NodeIdx
-    op: ops.BaseOp
+    op: ops.OpType
     parent: Optional["Node"]
     meta_data: dict[str, Any]
 
     @property
     @abstractmethod
     def num_in_ports(self) -> int:
         """The number of input ports on this node."""
@@ -99,16 +116,15 @@
     def in_port(self, offset: PortOffset | None) -> InPort:
         """Returns the input port at the given offset."""
 
     @abstractmethod
     def out_port(self, offset: PortOffset | None) -> OutPort:
         """Returns the output port at the given offset."""
 
-    @abstractmethod
-    def update_op(self) -> None:
+    def update_op(self) -> None:  # noqa: B027
         """Updates the op type associated with this node with additional information.
 
         This should be called before serialisation.
         """
 
     @property
     def in_ports(self) -> Iterator[InPort]:
@@ -176,17 +192,23 @@
 
     def update_op(self) -> None:
         """Updates the operation associated with this node with type information.
 
         Feeds type information from the in- and out-ports to the operation class to
         update signature information. This function must be called before serialisation.
         """
-        in_types = [t.to_hugr() for t in self.in_port_types]
-        out_types = [t.to_hugr() for t in self.out_port_types]
-        self.op.insert_port_types(in_types, out_types)
+        # We can't call `to_hugr()` on polymorphic function types, so we have to skip
+        # ops that have connected `Function` edges.
+        has_poly_func_edge = isinstance(
+            self.op.root, ops.FuncDecl | ops.FuncDefn | ops.Call | ops.LoadFunction
+        )
+        if isinstance(self.op.root, ops.BaseOp) and not has_poly_func_edge:
+            in_types = [t.to_hugr() for t in self.in_port_types]
+            out_types = [t.to_hugr() for t in self.out_port_types]
+            self.op.root.insert_port_types(in_types, out_types)
         super().update_op()
 
 
 class CFNode(Node):
     """A node in a control-flow graph.
 
     Compared to value nodes, the ports on this node are not typed since they correspond
@@ -239,33 +261,36 @@
         """Updates the operation associated with this node with type information.
 
         Feeds type information from the signature of the contained dataflow graph to
         the operation class to. This function must be called before serialisation.
         """
         assert self.input_child is not None
         assert self.output_child is not None
+        assert isinstance(self.op.root, ops.BaseOp)
         # Input and output node may have extra order edges connected, so we filter
         # `None`s here
         ins = [ty.to_hugr() for ty in self.input_child.out_port_types]
         outs = [ty.to_hugr() for ty in self.output_child.in_port_types]
-        self.op.insert_child_dfg_signature(inputs=ins, outputs=outs)
+        self.op.root.insert_child_dfg_signature(inputs=ins, outputs=outs)
         super().update_op()
 
 
 class DFContainingVNode(VNode, DFContainingNode):
     """A value node whose children form a dataflow graph"""
 
 
 class BlockNode(DFContainingNode, CFNode):
     """A `Block` node representing a basic block."""
 
 
 OrderEdge = tuple["Node", "Node"]
 ORDER_EDGE_KEY = (-1, -1)
 
+UNDEFINED: ops.NodeID = -1
+
 
 class Hugr:
     """Hierarchical unified graph representation."""
 
     name: str
     root: VNode
     _graph: nx.MultiDiGraph  # TODO: We probably don't need networkx.
@@ -275,15 +300,17 @@
     def __init__(self, name: str | None = None) -> None:
         """Creates a new Hugr."""
         self.name = name or "Unnamed"
         self._default_parent = None
         self._graph = nx.MultiDiGraph()
         self._children = {-1: []}
         self.root = self.add_node(
-            op=ops.Module(), meta_data={"name": name}, parent=None
+            op=ops.OpType(ops.Module(parent=UNDEFINED)),
+            meta_data={"name": name},
+            parent=None,
         )
 
     @contextmanager
     def parent(self, parent: Node) -> Iterator[None]:
         """Context manager to set a default parent for adding new nodes."""
         old_default = self._default_parent
         self._default_parent = parent
@@ -297,15 +324,15 @@
         self._children[node.parent.idx if node.parent else -1].append(node)
         if inputs is not None:
             for i, port in enumerate(inputs):
                 self.add_edge(port, node.in_port(i))
 
     def add_node(
         self,
-        op: ops.BaseOp,
+        op: ops.OpType,
         input_types: TypeList | None = None,
         output_types: TypeList | None = None,
         parent: Node | None = None,
         inputs: list[OutPortV] | None = None,
         meta_data: dict[str, Any] | None = None,
     ) -> VNode:
         """Helper method to add a generic value node to the graph."""
@@ -350,27 +377,29 @@
 
     def set_root_name(self, name: str) -> VNode:
         """Sets the name of the root node."""
         self.root.meta_data["name"] = name
         return self.root
 
     def add_constant(
-        self, value: val.Value, ty: Type, parent: Node | None = None
+        self, value: ops.Value, ty: Type, parent: Node | None = None
     ) -> VNode:
         """Adds a constant node holding a given value to the graph."""
         return self.add_node(
-            ops.Const(value=value, typ=ty.to_hugr()), [], [ty], parent, None
+            ops.OpType(ops.Const(v=value, parent=UNDEFINED)), [], [ty], parent, None
         )
 
     def add_input(
         self, output_tys: TypeList | None = None, parent: Node | None = None
     ) -> VNode:
         """Adds an `Input` node to the graph."""
         parent = parent or self._default_parent
-        node = self.add_node(ops.Input(), [], output_tys, parent)
+        node = self.add_node(
+            ops.OpType(ops.Input(parent=UNDEFINED)), [], output_tys, parent
+        )
         if isinstance(parent, DFContainingNode):
             parent.input_child = node
         return node
 
     def add_input_with_ports(
         self, output_tys: Sequence[Type], parent: Node | None = None
     ) -> tuple[VNode, list[OutPortV]]:
@@ -383,134 +412,188 @@
         self,
         inputs: list[OutPortV] | None = None,
         input_tys: TypeList | None = None,
         parent: Node | None = None,
     ) -> VNode:
         """Adds an `Output` node to the graph."""
         parent = parent or self._default_parent
-        node = self.add_node(ops.Output(), input_tys, [], parent, inputs)
+        node = self.add_node(
+            ops.OpType(ops.Output(parent=UNDEFINED)), input_tys, [], parent, inputs
+        )
         if isinstance(parent, DFContainingNode):
             parent.output_child = node
         return node
 
     def add_block(self, parent: Node | None, num_successors: int = 0) -> BlockNode:
         """Adds a `Block` node to the graph."""
         node = BlockNode(
             idx=self._graph.number_of_nodes(),
-            op=ops.DataflowBlock(),
+            op=ops.OpType(ops.DataflowBlock(parent=UNDEFINED, sum_rows=[])),
             parent=parent,
             meta_data={},
         )
         self._insert_node(node)
         for _ in range(num_successors):
             node.add_out_port()
         return node
 
     def add_exit(self, output_tys: TypeList, parent: Node) -> CFNode:
         """Adds an `Exit` node to the graph."""
         outputs = [ty.to_hugr() for ty in output_tys]
         node = CFNode(
             idx=self._graph.number_of_nodes(),
-            op=ops.ExitBlock(cfg_outputs=outputs),
+            op=ops.OpType(ops.ExitBlock(cfg_outputs=outputs, parent=UNDEFINED)),
             parent=parent,
             meta_data={},
         )
         self._insert_node(node)
         return node
 
     def add_dfg(self, parent: Node) -> DFContainingVNode:
         """Adds a nested dataflow `DFG` node to the graph."""
-        return self._add_dfg_node(ops.DFG(), [], [], parent)
+        return self._add_dfg_node(ops.OpType(ops.DFG(parent=UNDEFINED)), [], [], parent)
 
     def add_case(self, parent: Node) -> DFContainingVNode:
         """Adds a `Case` node to the graph."""
-        return self._add_dfg_node(ops.Case(), [], [], parent)
+        return self._add_dfg_node(
+            ops.OpType(ops.Case(parent=UNDEFINED)), [], [], parent
+        )
 
     def add_cfg(self, parent: Node, inputs: list[OutPortV]) -> VNode:
         """Adds a nested control-flow `CFG` node to the graph."""
-        return self.add_node(ops.CFG(), [], [], parent, inputs)
+        return self.add_node(
+            ops.OpType(ops.CFG(parent=UNDEFINED)), [], [], parent, inputs
+        )
 
     def add_conditional(
         self,
         cond_input: OutPortV,
         inputs: list[OutPortV],
         parent: Node | None = None,
     ) -> VNode:
         """Adds a `Conditional` node to the graph."""
         inputs = [cond_input, *inputs]
-        return self.add_node(ops.Conditional(), None, None, parent, inputs)
+        return self.add_node(
+            ops.OpType(ops.Conditional(sum_rows=[], parent=UNDEFINED)),
+            None,
+            None,
+            parent,
+            inputs,
+        )
 
     def add_tail_loop(
         self, inputs: list[OutPortV], parent: Node | None = None
     ) -> DFContainingVNode:
         """Adds a `TailLoop` node to the graph."""
-        return self._add_dfg_node(ops.TailLoop(), None, None, parent, inputs)
+        return self._add_dfg_node(
+            ops.OpType(ops.TailLoop(parent=UNDEFINED)), None, None, parent, inputs
+        )
 
     def add_make_tuple(
         self, inputs: list[OutPortV], parent: Node | None = None
     ) -> VNode:
         """Adds a `MakeTuple` node to the graph."""
         ty = TupleType([port.ty for port in inputs])
-        return self.add_node(ops.MakeTuple(), None, [ty], parent, inputs)
+        return self.add_node(
+            ops.OpType(ops.MakeTuple(parent=UNDEFINED)), None, [ty], parent, inputs
+        )
 
     def add_unpack_tuple(
         self, input_tuple: OutPortV, parent: Node | None = None
     ) -> VNode:
         """Adds an `UnpackTuple` node to the graph."""
         assert isinstance(input_tuple.ty, TupleType)
         return self.add_node(
-            ops.UnpackTuple(),
+            ops.OpType(ops.UnpackTuple(parent=UNDEFINED)),
             None,
             list(input_tuple.ty.element_types),
             parent,
             [input_tuple],
         )
 
     def add_tag(
-        self, variants: TypeList, tag: int, inp: OutPortV, parent: Node | None = None
+        self,
+        variants: Sequence[TypeRow],
+        tag: int,
+        inputs: list[OutPortV],
+        parent: Node | None = None,
     ) -> VNode:
         """Adds a `Tag` node to the graph."""
-        types = [ty.to_hugr() for ty in variants]
-        assert inp.ty == variants[tag]
+        assert all(inp.ty == ty for inp, ty in zip(inputs, variants[tag]))
+        hugr_variants = rows_to_hugr(variants)
+        out_ty = SumType([row_to_type(row) for row in variants])
         return self.add_node(
-            ops.Tag(tag=tag, variants=types), None, [SumType(variants)], parent, [inp]
+            ops.OpType(ops.Tag(tag=tag, variants=hugr_variants, parent=UNDEFINED)),
+            None,
+            [out_ty],
+            parent,
+            inputs,
         )
 
     def add_load_constant(
         self, const_port: OutPortV, parent: Node | None = None
     ) -> VNode:
         """Adds a `LoadConstant` node to the graph."""
         return self.add_node(
-            ops.LoadConstant(datatype=const_port.ty.to_hugr()),
+            ops.OpType(
+                ops.LoadConstant(datatype=const_port.ty.to_hugr(), parent=UNDEFINED)
+            ),
             None,
             [const_port.ty],
             parent,
             [const_port],
         )
 
+    def add_load_function(
+        self, def_port: OutPortV, inst: Inst, parent: Node | None = None
+    ) -> VNode:
+        """Adds a `LoadFunction` node to the graph."""
+        assert isinstance(def_port.ty, FunctionType)
+        assert len(def_port.ty.params) == len(inst)
+        instantiation = def_port.ty.instantiate(inst)
+        op = ops.LoadFunction(
+            func_sig=def_port.ty.to_hugr_poly(),
+            type_args=[arg.to_hugr() for arg in inst],
+            signature=tys.FunctionType(input=[], output=[instantiation.to_hugr()]),
+            parent=UNDEFINED,
+        )
+        return self.add_node(ops.OpType(op), None, [instantiation], parent, [def_port])
+
     def add_call(
-        self, def_port: OutPortV, args: list[OutPortV], parent: Node | None = None
+        self,
+        def_port: OutPortV,
+        args: list[OutPortV],
+        inst: Inst,
+        parent: Node | None = None,
     ) -> VNode:
         """Adds a `Call` node to the graph."""
         assert isinstance(def_port.ty, FunctionType)
+        instantiation = def_port.ty.instantiate(inst)
+        op = ops.Call(
+            func_sig=def_port.ty.to_hugr_poly(),
+            type_args=[arg.to_hugr() for arg in inst],
+            instantiation=instantiation.to_hugr().root,
+            parent=UNDEFINED,
+        )
         return self.add_node(
-            ops.Call(),
+            ops.OpType(op),
             None,
-            list(type_to_row(def_port.ty.output)),
+            list(type_to_row(instantiation.output)),
             parent,
             [*args, def_port],
         )
 
     def add_indirect_call(
         self, fun_port: OutPortV, args: list[OutPortV], parent: Node | None = None
     ) -> VNode:
         """Adds an `IndirectCall` node to the graph."""
         assert isinstance(fun_port.ty, FunctionType)
+
         return self.add_node(
-            ops.CallIndirect(),
+            ops.OpType(ops.CallIndirect(parent=UNDEFINED)),
             None,
             list(type_to_row(fun_port.ty.output)),
             parent,
             [fun_port, *args],
         )
 
     def add_partial(
@@ -524,45 +607,28 @@
             def_port.ty.inputs[len(inputs) :],
             def_port.ty.output,
             def_port.ty.input_names[len(inputs) :]
             if def_port.ty.input_names is not None
             else None,
         )
         return self.add_node(
-            ops.DummyOp(name="partial"), None, [new_ty], parent, [*inputs, def_port]
-        )
-
-    def add_type_apply(
-        self, func_port: OutPortV, args: Inst, parent: Node | None = None
-    ) -> VNode:
-        """Adds a `TypeApply` node to the graph."""
-        assert isinstance(func_port.ty, FunctionType)
-        assert len(func_port.ty.params) == len(args)
-        result_ty = func_port.ty.instantiate(args)
-        ta = ops.TypeApplication(
-            input=func_port.ty.to_hugr(),
-            args=[arg.to_hugr() for arg in args],
-            output=result_ty.to_hugr(),
-        )
-        return self.add_node(
-            ops.TypeApply(ta=ta),
-            inputs=[func_port],
-            output_types=[result_ty],
-            parent=parent,
+            DummyOp("partial"), None, [new_ty], parent, [*inputs, def_port]
         )
 
     def add_def(
         self, fun_ty: FunctionType, parent: Node | None, name: str
     ) -> DFContainingVNode:
-        """Adds a `Def` node to the graph."""
-        return self._add_dfg_node(ops.FuncDefn(name=name), [], [fun_ty], parent, None)
+        """Adds a `FucnDefn` node to the graph."""
+        op = ops.FuncDefn(name=name, signature=fun_ty.to_hugr_poly(), parent=UNDEFINED)
+        return self._add_dfg_node(ops.OpType(op), [], [fun_ty], parent, None)
 
     def add_declare(self, fun_ty: FunctionType, parent: Node, name: str) -> VNode:
-        """Adds a `Declare` node to the graph."""
-        return self.add_node(ops.FuncDecl(name=name), [], [fun_ty], parent, None)
+        """Adds a `FuncDecl` node to the graph."""
+        op = ops.FuncDecl(name=name, signature=fun_ty.to_hugr_poly(), parent=UNDEFINED)
+        return self.add_node(ops.OpType(op), [], [fun_ty], parent, None)
 
     def add_edge(self, src_port: OutPort, tgt_port: InPort) -> None:
         """Adds an edge between two ports."""
         if isinstance(src_port, OutPortV) or isinstance(tgt_port, InPortV):
             assert isinstance(src_port, OutPortV)
             assert isinstance(tgt_port, InPortV)
             assert src_port.ty == tgt_port.ty
@@ -658,65 +724,46 @@
 
     def remove_dummy_nodes(self) -> "Hugr":
         """Replaces dummy ops with external function calls."""
         if self.root is None:
             raise ValueError("Dummy node removal requires a module root node")
         used_names: dict[str, int] = {}
         for n in list(self.nodes()):
-            if isinstance(n, VNode) and isinstance(n.op, ops.DummyOp):
+            if isinstance(n, VNode) and isinstance(n.op, DummyOp):
                 name = n.op.name
                 fun_ty = FunctionType(
                     list(n.in_port_types), row_to_type(n.out_port_types)
                 )
                 if name in used_names:
                     used_names[name] += 1
                     name = f"{name}${used_names[name]}"
                 else:
                     used_names[name] = 0
                 decl = self.add_declare(fun_ty, self.root, name)
-                n.op = ops.Call()
+                n.op = ops.OpType(
+                    ops.Call(
+                        func_sig=fun_ty.to_hugr_poly(),
+                        type_args=[],
+                        instantiation=fun_ty.to_hugr().root,
+                        parent=UNDEFINED,
+                    )
+                )
                 self.add_edge(decl.out_port(0), n.add_in_port(fun_ty))
         return self
 
     def insert_order_edges(self) -> "Hugr":
-        """Adds state edges to all dataflow ops without inputs outputs.
+        """Adds order edges to the source and target inter-graph edges.
 
-        We add state edges connecting them to the input or output node of the DFG.
-        This action must be performed before serialisation.
+        This ensures that the source is executed before the target. This action must be
+        performed before serialisation.
         """
-        for n in self.nodes():
-            if isinstance(n.op, ops.DataflowOp) and isinstance(
-                n.parent, DFContainingNode
-            ):
-                if all(
-                    next(self.in_edges(p), None) is None for p in n.in_ports
-                ) and not isinstance(n.op, ops.Input):
-                    assert n.parent.input_child is not None
-                    self.add_order_edge(n.parent.input_child, n)
-                if all(
-                    next(self.out_edges(p), None) is None for p in n.out_ports
-                ) and not isinstance(n.op, ops.Output):
-                    assert n.parent.output_child is not None
-                    self.add_order_edge(n, n.parent.output_child)
-                # Special case: Call ops for functions without any arguments are
-                # only connected to the top-level def/declare and also need an
-                # order edge
-                if isinstance(n.op, ops.Call) and n.num_in_ports == 1:  # noqa: SIM114
-                    assert n.parent.input_child is not None
-                    self.add_order_edge(n.parent.input_child, n)
-                # Special case: Load constant ops always need an order edge
-                elif isinstance(n.op, ops.LoadConstant):
-                    assert n.parent.input_child is not None
-                    self.add_order_edge(n.parent.input_child, n)
-
-        # Also add order edges for non-local edges
         for src, tgt in list(self.edges()):
             # Exclude CF and constant edges
             if isinstance(src, OutPortCF) or isinstance(
-                src.node.op, ops.FuncDecl | ops.FuncDefn | ops.Const
+                src.node.op.root, ops.FuncDecl | ops.FuncDefn | ops.Const
             ):
                 continue
 
             if src.node.parent != tgt.node.parent:
                 # Walk up the hierarchy from the tgt until we hit a node at the same
                 # level as src
                 node = tgt.node
@@ -724,76 +771,85 @@
                     if node.parent is None:
                         raise ValueError("Invalid non-local edge!")
                     node = node.parent
                 # Add order edge to make sure that the src is executed first
                 self.add_order_edge(src.node, node)
         return self
 
-    def to_raw(self) -> raw.RawHugr:
+    def to_raw(self) -> SerialHugr:
         """Returns the raw representation of this HUGR for serialisation."""
+        if self.root is None:
+            raise ValueError("Serial Hugr requires a root node")
+
         self.remove_dummy_nodes()
         self.insert_order_edges()
         # Hugr requires that Input/Output nodes are the first/second children in a DFG.
         # Furthermore, exit nodes must be the second children of CFGs. We're going to
         # satisfy this trivially by first serialising all inputs, outputs, entry and
         # exit nodes
         input_nodes: list[Node] = []
         output_nodes: list[Node] = []
         entry_nodes: list[Node] = []
         exit_nodes: list[Node] = []
         remaining_nodes: list[Node] = []
         indices = itertools.count()
         raw_index: dict[int, ops.NodeID] = {}
         all_nodes = self.nodes()
-        root_node = next(all_nodes)
         for n in all_nodes:
-            if isinstance(n.op, ops.Input):
-                input_nodes.append(n)
-            elif isinstance(n.op, ops.Output):
-                output_nodes.append(n)
-            elif (
-                isinstance(n.op, ops.DataflowBlock)
-                and next(self.in_edges(n.in_port(None)), None) is None
-            ):
-                entry_nodes.append(n)
-            elif isinstance(n.op, ops.ExitBlock):
-                exit_nodes.append(n)
-            else:
-                remaining_nodes.append(n)
+            if n is self.root:
+                continue
+            match n.op.root:
+                case ops.Input():
+                    input_nodes.append(n)
+                case ops.Output():
+                    output_nodes.append(n)
+                # We can detect entry BBs by looking for BBs without incoming edges
+                # since Guppy will never generate an edge pointing back to the entry.
+                # Also, Guppy errors on unreachable code, so we will never generate
+                # interior BBs without incoming edges. Hence, there are also no false
+                # positives.
+                case ops.DataflowBlock() if next(
+                    self.in_edges(n.in_port(None)), None
+                ) is None:
+                    entry_nodes.append(n)
+                case ops.ExitBlock():
+                    exit_nodes.append(n)
+                case _:
+                    remaining_nodes.append(n)
         for n in itertools.chain(
-            iter([root_node]),
+            iter([self.root]),
             iter(entry_nodes),
             iter(exit_nodes),
             iter(input_nodes),
             iter(output_nodes),
             iter(remaining_nodes),
         ):
             raw_index[n.idx] = next(indices)
 
-        nodes: list[ops.OpType] = [ops.Module()] * self._graph.number_of_nodes()
+        nodes: list[ops.OpType] = [
+            ops.OpType(ops.Module(parent=UNDEFINED))
+        ] * self._graph.number_of_nodes()
         for n in self.nodes():
             idx = raw_index[n.idx]
             # Nodes without parent have themselves as parent in the serialised format
             parent = n.parent or n
             n.update_op()
-            n.op.parent = raw_index[parent.idx]
+            n.op.root.parent = raw_index[parent.idx]
             nodes[idx] = n.op
 
         edges: list[raw.Edge] = []
         for src, tgt in self.edges():
             edges.append(
                 (
                     (raw_index[src.node.idx], src.offset),
                     (raw_index[tgt.node.idx], tgt.offset),
                 )
             )
 
         for src, tgt in self.order_edges():
             edges.append(((raw_index[src.idx], None), (raw_index[tgt.idx], None)))
 
-        if self.root is None:
-            raise ValueError("Raw Hugr requires a root node")
-        return raw.RawHugr(nodes=nodes, edges=edges)
+        return SerialHugr(nodes=nodes, edges=edges)
 
     def serialize(self) -> str:
         """Serialize this Hugr in JSON format."""
         return self.to_raw().to_json()
```

### Comparing `guppylang-0.2.0/guppylang/hugr/visualise.py` & `guppylang-0.3.0/guppylang/hugr_builder/visualise.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from guppylang.cfg.analysis import (
     DefAssignmentDomain,
     LivenessDomain,
     MaybeAssignmentDomain,
 )
 from guppylang.cfg.bb import BB
-from guppylang.hugr.hugr import Hugr, InPort, Node, OutPort, OutPortV
+from guppylang.hugr_builder.hugr import DummyOp, Hugr, InPort, Node, OutPort, OutPortV
 
 if TYPE_CHECKING:
     from guppylang.cfg.cfg import CFG
 
 # old palettte: https://colorhunt.co/palette/343a407952b3ffc107e1e8eb
 # _COLOURS = {
 #     "background": "white",
@@ -59,21 +59,16 @@
 _HTML_LABEL_TEMPLATE = """
 <TABLE BORDER="{border_width}" CELLBORDER="0" CELLSPACING="1" CELLPADDING="1"
        BGCOLOR="{node_back_color}" COLOR="{border_colour}">
   {inputs_row}
   <TR>
     <TD>
       <TABLE BORDER="0" CELLBORDER="0">
-        <TR>
-          <TD>
-            <FONT POINT-SIZE="{fontsize}" FACE="{fontface}" COLOR="{label_color}">
-              <B>{node_label}</B>{node_data}
-            </FONT>
-          </TD>
-        </TR>
+        <TR><TD><FONT POINT-SIZE="{fontsize}" FACE="{fontface}"
+            COLOR="{label_color}"><B>{node_label}</B>{node_data}</FONT></TD></TR>
       </TABLE>
     </TD>
   </TR>
   {outputs_row}
 </TABLE>
 """
 
@@ -168,30 +163,32 @@
         data = ""
     if len(hugr.children(node)) > 0:
         with graph.subgraph(name=f"cluster{node.idx}") as sub:
             for child in hugr.children(node):
                 viz_node(child, hugr, sub)
             html_label = _format_html_label(
                 node_back_color=_COLOURS["edge"],
-                node_label=node.op.display_name(),
+                node_label=node.op.root.display_name(),
                 node_data=data,
                 border_colour=_COLOURS["port_border"],
                 inputs_row=_html_ports(in_ports, _INPUT_PREFIX)
                 if len(in_ports) > 0
                 else "",
                 outputs_row=_html_ports(out_ports, _OUTPUT_PREFIX)
                 if len(out_ports) > 0
                 else "",
             )
             sub.node(f"{node.idx}", shape="plain", label=f"<{html_label}>")
             sub.attr(label="", margin="10", color=_COLOURS["edge"])
     else:
         html_label = _format_html_label(
             node_back_color=_COLOURS["node"],
-            node_label=node.op.display_name(),
+            node_label=node.op.name
+            if isinstance(node.op, DummyOp)
+            else node.op.root.display_name(),
             node_data=data,
             inputs_row=_html_ports(in_ports, _INPUT_PREFIX)
             if len(in_ports) > 0
             else "",
             outputs_row=_html_ports(out_ports, _OUTPUT_PREFIX)
             if len(out_ports) > 0
             else "",
```

### Comparing `guppylang-0.2.0/guppylang/module.py` & `guppylang-0.3.0/guppylang/module.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-import ast
 import inspect
+import itertools
 import sys
-import textwrap
-from collections.abc import Callable
+from collections.abc import Callable, Mapping
 from types import ModuleType
 from typing import Any, Union
 
-from guppylang.ast_util import AstNode, annotate_location
-from guppylang.checker.core import Globals, PyScope, qualified_name
-from guppylang.checker.func_checker import DefinedFunction, check_global_func_def
+from guppylang.ast_util import AstNode
+from guppylang.checker.core import Globals, PyScope
 from guppylang.compiler.core import CompiledGlobals
-from guppylang.compiler.func_compiler import (
-    CompiledFunctionDef,
-    compile_global_func_def,
+from guppylang.definition.common import (
+    CheckableDef,
+    CheckedDef,
+    CompilableDef,
+    DefId,
+    ParsableDef,
+    RawDef,
 )
-from guppylang.custom import CustomFunction
-from guppylang.declared import DeclaredFunction
+from guppylang.definition.custom import CustomFunctionDef
+from guppylang.definition.declaration import RawFunctionDecl
+from guppylang.definition.function import RawFunctionDef
+from guppylang.definition.parameter import TypeVarDef
+from guppylang.definition.ty import TypeDef
 from guppylang.error import GuppyError, pretty_errors
-from guppylang.hugr.hugr import Hugr
-from guppylang.tys.definition import TypeDef
-from guppylang.tys.param import TypeParam
+from guppylang.hugr_builder.hugr import Hugr
 
 PyFunc = Callable[..., Any]
 PyFuncDefOrDecl = tuple[bool, PyFunc]
 
 
 class GuppyModule:
     """A Guppy module that may contain function and type definitions."""
 
     name: str
 
     # Whether the module has already been compiled
     _compiled: bool
 
+    # Map of raw definitions in this module
+    _raw_defs: dict[DefId, RawDef]
+    _raw_type_defs: dict[DefId, RawDef]
+
     # Globals from imported modules
     _imported_globals: Globals
     _imported_compiled_globals: CompiledGlobals
 
     # Globals for functions and types defined in this module. Only gets populated during
     # compilation
     _globals: Globals
     _compiled_globals: CompiledGlobals
 
-    # Mappings of functions defined in this module
-    _func_defs: dict[str, tuple[ast.FunctionDef, PyScope]]
-    _func_decls: dict[str, ast.FunctionDef]
-    _custom_funcs: dict[str, CustomFunction]
-
     # When `_instance_buffer` is not `None`, then all registered functions will be
     # buffered in this list. They only get properly registered, once
     # `_register_buffered_instance_funcs` is called. This way, we can associate
-    _instance_func_buffer: dict[str, PyFuncDefOrDecl | CustomFunction] | None
+    _instance_func_buffer: dict[str, RawDef] | None
 
     def __init__(self, name: str, import_builtins: bool = True):
         self.name = name
         self._globals = Globals({}, {}, {}, {})
         self._compiled_globals = {}
         self._imported_globals = Globals.default()
         self._imported_compiled_globals = {}
-        self._func_defs = {}
-        self._func_decls = {}
-        self._custom_funcs = {}
         self._compiled = False
         self._instance_func_buffer = None
+        self._raw_defs = {}
+        self._raw_type_defs = {}
 
         # Import builtin module
         if import_builtins:
             import guppylang.prelude.builtins as builtins
 
             self.load(builtins)
 
@@ -76,205 +77,151 @@
         if isinstance(m, GuppyModule):
             # Compile module if it isn't compiled yet
             if not m.compiled:
                 m.compile()
 
             # For now, we can only import custom functions
             if any(
-                not isinstance(v, CustomFunction) for v in m._compiled_globals.values()
+                not isinstance(v, CustomFunctionDef | TypeDef | TypeVarDef)
+                for v in m._compiled_globals.values()
             ):
                 raise GuppyError(
                     "Importing modules with defined functions is not supported yet"
                 )
 
             self._imported_globals |= m._globals
             self._imported_compiled_globals |= m._compiled_globals
         else:
             for val in m.__dict__.values():
                 if isinstance(val, GuppyModule):
                     self.load(val)
 
-    def register_func_def(self, f: PyFunc, instance: TypeDef | None = None) -> None:
-        """Registers a Python function definition as belonging to this Guppy module."""
-        self._check_not_yet_compiled()
-        func_ast = parse_py_func(f)
-        if self._instance_func_buffer is not None:
-            self._instance_func_buffer[func_ast.name] = (True, f)
-        else:
-            name = (
-                qualified_name(instance, func_ast.name) if instance else func_ast.name
-            )
-            self._check_name_available(name, func_ast)
-            self._func_defs[name] = func_ast, get_py_scope(f)
-
-    def register_func_decl(self, f: PyFunc, instance: TypeDef | None = None) -> None:
-        """Registers a Python function declaration as belonging to this Guppy module."""
-        self._check_not_yet_compiled()
-        func_ast = parse_py_func(f)
-        if self._instance_func_buffer is not None:
-            self._instance_func_buffer[func_ast.name] = (False, f)
-        else:
-            name = (
-                qualified_name(instance, func_ast.name) if instance else func_ast.name
-            )
-            self._check_name_available(name, func_ast)
-            self._func_decls[name] = func_ast
+    def register_def(self, defn: RawDef, instance: TypeDef | None = None) -> None:
+        """Registers a definition with this module.
 
-    def register_custom_func(
-        self, func: CustomFunction, instance: TypeDef | None = None
-    ) -> None:
-        """Registers a custom function as belonging to this Guppy module."""
+        Optionally, the definition can be marked as an instance method by passing the
+        corresponding instance type definition.
+        """
         self._check_not_yet_compiled()
-        if self._instance_func_buffer is not None:
-            self._instance_func_buffer[func.name] = func
+        if self._instance_func_buffer is not None and not isinstance(defn, TypeDef):
+            self._instance_func_buffer[defn.name] = defn
         else:
-            if instance:
-                func.name = qualified_name(instance, func.name)
-            self._check_name_available(func.name, func.defined_at)
-            self._custom_funcs[func.name] = func
-
-    def register_type(self, name: str, defn: TypeDef) -> None:
-        """Registers an existing Guppy type as belonging to this Guppy module."""
-        self._check_not_yet_compiled()
-        self._check_type_name_available(name, None)
-        self._globals.type_defs[name] = defn
+            self._check_name_available(defn.name, defn.defined_at)
+            if isinstance(defn, TypeDef | TypeVarDef):
+                self._raw_type_defs[defn.id] = defn
+            else:
+                self._raw_defs[defn.id] = defn
+            if instance is not None:
+                self._globals.impls.setdefault(instance.id, {})
+                self._globals.impls[instance.id][defn.name] = defn.id
+            else:
+                self._globals.names[defn.name] = defn.id
 
-    def register_type_var(self, name: str, linear: bool) -> None:
-        """Registers a new type variable"""
-        self._check_not_yet_compiled()
-        self._check_type_name_available(name, None)
-        self._globals.param_vars[name] = TypeParam(
-            len(self._globals.param_vars), name, linear
-        )
+    def register_func_def(
+        self, f: PyFunc, instance: TypeDef | None = None
+    ) -> RawFunctionDef:
+        """Registers a Python function definition as belonging to this Guppy module."""
+        defn = RawFunctionDef(DefId.fresh(self), f.__name__, None, f, get_py_scope(f))
+        self.register_def(defn, instance)
+        return defn
+
+    def register_func_decl(
+        self, f: PyFunc, instance: TypeDef | None = None
+    ) -> RawFunctionDecl:
+        """Registers a Python function declaration as belonging to this Guppy module."""
+        decl = RawFunctionDecl(DefId.fresh(self), f.__name__, None, f)
+        self.register_def(decl, instance)
+        return decl
 
-    def _register_buffered_instance_funcs(self, defn: TypeDef) -> None:
+    def _register_buffered_instance_funcs(self, instance: TypeDef) -> None:
         assert self._instance_func_buffer is not None
         buffer = self._instance_func_buffer
         self._instance_func_buffer = None
-        for f in buffer.values():
-            if isinstance(f, CustomFunction):
-                self.register_custom_func(f, defn)
-            else:
-                is_def, pyfunc = f
-                if is_def:
-                    self.register_func_def(pyfunc, defn)
-                else:
-                    self.register_func_decl(pyfunc, defn)
+        for defn in buffer.values():
+            self.register_def(defn, instance)
 
     @property
     def compiled(self) -> bool:
         return self._compiled
 
+    @staticmethod
+    def _check_defs(
+        raw_defs: Mapping[DefId, RawDef], globals: Globals
+    ) -> dict[DefId, CheckedDef]:
+        """Helper method to parse and check raw definitions."""
+        raw_globals = globals | Globals(raw_defs, {}, {}, {})
+        parsed = {
+            def_id: defn.parse(raw_globals) if isinstance(defn, ParsableDef) else defn
+            for def_id, defn in raw_defs.items()
+        }
+        parsed_globals = globals | Globals(parsed, {}, {}, {})
+        return {
+            def_id: (
+                defn.check(parsed_globals) if isinstance(defn, CheckableDef) else defn
+            )
+            for def_id, defn in parsed.items()
+        }
+
     @pretty_errors
     def compile(self) -> Hugr | None:
         """Compiles the module and returns the final Hugr."""
         if self.compiled:
             raise GuppyError("Module has already been compiled")
 
-        # Prepare globals for type checking
-        for func in self._custom_funcs.values():
-            func.check_type(self._imported_globals | self._globals)
-        defined_funcs = {
-            x: DefinedFunction.from_ast(f, x, self._imported_globals | self._globals)
-            for x, (f, _) in self._func_defs.items()
-        }
-        declared_funcs = {
-            x: DeclaredFunction.from_ast(f, x, self._imported_globals | self._globals)
-            for x, f in self._func_decls.items()
-        }
-        self._globals.values.update(self._custom_funcs)
-        self._globals.values.update(declared_funcs)
-        self._globals.values.update(defined_funcs)
-
-        # Type check function definitions
-        checked = {
-            x: check_global_func_def(
-                f,
-                self._imported_globals
-                | self._globals
-                | Globals({}, {}, {}, self._func_defs[x][1]),
-            )
-            for x, f in defined_funcs.items()
-        }
+        # Type definitions need to be checked first so that we can use them when parsing
+        # function signatures etc.
+        type_defs = self._check_defs(
+            self._raw_type_defs, self._imported_globals | self._globals
+        )
+        self._globals = self._globals.update_defs(type_defs)
 
-        # Add declared functions to the graph
+        # Now, we can check all other definitions
+        other_defs = self._check_defs(
+            self._raw_defs, self._imported_globals | self._globals
+        )
+        self._globals = self._globals.update_defs(other_defs)
+
+        # Prepare Hugr for this module
         graph = Hugr(self.name)
         module_node = graph.set_root_name(self.name)
-        for f in declared_funcs.values():
-            f.add_to_graph(graph, module_node)
 
-        # Prepare `FunctionDef` nodes for all function definitions
-        def_nodes = {x: graph.add_def(f.ty, module_node, x) for x, f in checked.items()}
-        self._compiled_globals |= (
-            self._custom_funcs
-            | declared_funcs
-            | {
-                x: CompiledFunctionDef(x, f.ty, f.defined_at, None, def_nodes[x])
-                for x, f in checked.items()
-            }
-        )
-
-        # Compile function definitions to Hugr
-        for x, f in checked.items():
-            compile_global_func_def(
-                f,
-                def_nodes[x],
-                graph,
-                self._imported_compiled_globals | self._compiled_globals,
+        # Compile definitions to Hugr
+        self._compiled_globals = {
+            defn.id: (
+                defn.compile_outer(graph, module_node)
+                if isinstance(defn, CompilableDef)
+                else defn
             )
+            for defn in itertools.chain(type_defs.values(), other_defs.values())
+        }
+        all_compiled_globals = self._compiled_globals | self._imported_compiled_globals
+
+        # Finally, compile the definition contents to Hugr. For example, this compiles
+        # the bodies of functions.
+        for defn in self._compiled_globals.values():
+            defn.compile_inner(graph, all_compiled_globals)
 
         self._compiled = True
         return graph
 
-    def contains_function(self, name: str) -> bool:
-        """Returns 'True' if the module contains a function with the given name."""
-        return name in self._func_defs or name in self._custom_funcs
-
-    def contains_type(self, name: str) -> bool:
-        """Returns 'True' if the module contains a type with the given name."""
-        return name in self._globals.type_defs or name in self._globals.param_vars
+    def contains(self, name: str) -> bool:
+        """Returns 'True' if the module contains an object with the given name."""
+        return name in self._globals.names
 
     def _check_not_yet_compiled(self) -> None:
         if self._compiled:
             raise GuppyError(f"The module `{self.name}` has already been compiled")
 
     def _check_name_available(self, name: str, node: AstNode | None) -> None:
-        if self.contains_function(name):
-            raise GuppyError(
-                f"Module `{self.name}` already contains a function named `{name}`",
-                node,
-            )
-
-    def _check_type_name_available(self, name: str, node: AstNode | None) -> None:
-        if name in self._globals.type_defs:
+        if self.contains(name):
             raise GuppyError(
-                f"Module `{self.name}` already contains a type `{name}`",
+                f"Module `{self.name}` already contains a definition named `{name}`",
                 node,
             )
 
-        if name in self._globals.param_vars:
-            raise GuppyError(
-                f"Module `{self.name}` already contains a type variable `{name}`",
-                node,
-            )
-
-
-def parse_py_func(f: PyFunc) -> ast.FunctionDef:
-    source_lines, line_offset = inspect.getsourcelines(f)
-    source = "".join(source_lines)  # Lines already have trailing \n's
-    source = textwrap.dedent(source)
-    func_ast = ast.parse(source).body[0]
-    file = inspect.getsourcefile(f)
-    if file is None:
-        raise GuppyError("Couldn't determine source file for function")
-    annotate_location(func_ast, source, file, line_offset)
-    if not isinstance(func_ast, ast.FunctionDef):
-        raise GuppyError("Expected a function definition", func_ast)
-    return func_ast
-
 
 def get_py_scope(f: PyFunc) -> PyScope:
     """Returns a mapping of all variables captured by a Python function.
 
     Note that this function only works in CPython. On other platforms, an empty
     dictionary is returned.
```

### Comparing `guppylang-0.2.0/guppylang/nodes.py` & `guppylang-0.3.0/guppylang/nodes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,60 +1,76 @@
 """Custom AST nodes used by Guppy"""
 
 import ast
 from collections.abc import Mapping
 from typing import TYPE_CHECKING, Any
 
 from guppylang.tys.subst import Inst
-from guppylang.tys.ty import FunctionType
+from guppylang.tys.ty import FunctionType, Type
 
 if TYPE_CHECKING:
     from guppylang.cfg.cfg import CFG
     from guppylang.checker.cfg_checker import CheckedCFG
-    from guppylang.checker.core import CallableVariable, Variable
+    from guppylang.checker.core import Variable
+    from guppylang.definition.common import DefId
 
 
 class LocalName(ast.Name):
     id: str
 
     _fields = ("id",)
 
 
 class GlobalName(ast.Name):
     id: str
-    value: "Variable"
+    def_id: "DefId"
 
     _fields = (
         "id",
-        "value",
+        "def_id",
     )
 
 
 class LocalCall(ast.expr):
     func: ast.expr
     args: list[ast.expr]
 
     _fields = (
         "func",
         "args",
     )
 
 
 class GlobalCall(ast.expr):
-    func: "CallableVariable"
+    def_id: "DefId"
     args: list[ast.expr]
     type_args: Inst  # Inferred type arguments
 
     _fields = (
-        "func",
+        "def_id",
         "args",
         "type_args",
     )
 
 
+class TensorCall(ast.expr):
+    """A call to a tuple of functions. Behaves like a local call, but more
+    unpacking of tuples is required at compilation"""
+
+    func: ast.expr
+    args: list[ast.expr]
+    out_tys: Type
+
+    _fields = (
+        "func",
+        "args",
+        "out_tys",
+    )
+
+
 class TypeApply(ast.expr):
     value: ast.expr
     inst: Inst
 
     _fields = (
         "value",
         "inst",
@@ -163,23 +179,26 @@
     def __init__(self, cfg: "CFG", ty: FunctionType, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.cfg = cfg
         self.ty = ty
 
 
 class CheckedNestedFunctionDef(ast.FunctionDef):
+    def_id: "DefId"
     cfg: "CheckedCFG"
     ty: FunctionType
     captured: Mapping[str, "Variable"]
 
     def __init__(
         self,
+        def_id: "DefId",
         cfg: "CheckedCFG",
         ty: FunctionType,
         captured: Mapping[str, "Variable"],
         *args: Any,
         **kwargs: Any,
     ) -> None:
         super().__init__(*args, **kwargs)
+        self.def_id = def_id
         self.cfg = cfg
         self.ty = ty
         self.captured = captured
```

### Comparing `guppylang-0.2.0/guppylang/prelude/_internal.py` & `guppylang-0.3.0/guppylang/prelude/_internal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,142 +1,176 @@
 import ast
-from typing import Any, Literal
 
+from hugr.serialization import ops, tys
 from pydantic import BaseModel
 
 from guppylang.ast_util import AstNode, get_type, with_loc, with_type
-from guppylang.checker.core import CallableVariable, Context
+from guppylang.checker.core import Context
 from guppylang.checker.expr_checker import ExprSynthesizer, check_num_args
-from guppylang.custom import (
+from guppylang.definition.custom import (
     CustomCallChecker,
     CustomCallCompiler,
-    CustomFunction,
+    CustomFunctionDef,
     DefaultCallChecker,
 )
+from guppylang.definition.ty import TypeDef
+from guppylang.definition.value import CallableDef
 from guppylang.error import GuppyError, GuppyTypeError
-from guppylang.hugr import ops, tys, val
-from guppylang.hugr.hugr import OutPortV
+from guppylang.hugr_builder.hugr import UNDEFINED, OutPortV
 from guppylang.nodes import GlobalCall
-from guppylang.tys.definition import bool_type
+from guppylang.tys.builtin import bool_type, list_type
 from guppylang.tys.subst import Subst
 from guppylang.tys.ty import FunctionType, OpaqueType, Type, unify
 
 INT_WIDTH = 6  # 2^6 = 64 bit
 
 
-hugr_int_type = tys.Opaque(
-    extension="arithmetic.int.types",
-    id="int",
-    args=[tys.BoundedNatArg(n=INT_WIDTH)],
-    bound=tys.TypeBound.Eq,
+hugr_int_type = tys.Type(
+    tys.Opaque(
+        extension="arithmetic.int.types",
+        id="int",
+        args=[tys.TypeArg(tys.BoundedNatArg(n=INT_WIDTH))],
+        bound=tys.TypeBound.Eq,
+    )
 )
 
 
-hugr_float_type = tys.Opaque(
-    extension="arithmetic.float.types",
-    id="float64",
-    args=[],
-    bound=tys.TypeBound.Copyable,
+hugr_float_type = tys.Type(
+    tys.Opaque(
+        extension="arithmetic.float.types",
+        id="float64",
+        args=[],
+        bound=tys.TypeBound.Copyable,
+    )
 )
 
 
-class ConstIntS(BaseModel):
-    """Hugr representation of signed integers in the arithmetic extension."""
+class ConstInt(BaseModel):
+    """Hugr representation of signed and unsigned integers in the arithmetic extension.
+
+    Hugr always uses a u64 for the value. The interpretation is:
+      - as an unsigned integer, (value mod `2^N`);
+      - as a signed integer, (value mod `2^(N-1) - 2^(N-1)*a`)
+    where `N = 2^log_width` and `a` is the (N-1)th bit of `x` (counting from 0 = least
+    significant bit).
+    """
 
-    c: Literal["ConstIntS"] = "ConstIntS"
     log_width: int
     value: int
 
 
 class ConstF64(BaseModel):
-    """Hugr representation of floats in the arithmetic extension."""
+    """Hugr representation of float values."""
 
-    c: Literal["ConstF64"] = "ConstF64"
     value: float
 
 
-class ListValue(BaseModel):
-    """Hugr representation of floats in the arithmetic extension."""
-
-    c: Literal["ListValue"] = "ListValue"
-    value: tuple[list[Any], tys.Type]
-
-
-def bool_value(b: bool) -> val.Value:
+def bool_value(b: bool) -> ops.Value:
     """Returns the Hugr representation of a boolean value."""
-    return val.Sum(tag=int(b), value=val.Tuple(vs=[]))
+    unit = ops.Value(ops.TupleValue(vs=[]))
+    return ops.Value(
+        ops.SumValue(tag=int(b), typ=tys.SumType(tys.UnitSum(size=2)), vs=[unit])
+    )
 
 
-def int_value(i: int) -> val.Value:
+def int_value(i: int) -> ops.Value:
     """Returns the Hugr representation of an integer value."""
-    return val.ExtensionVal(c=(ConstIntS(log_width=INT_WIDTH, value=i),))
+    return ops.Value(
+        ops.ExtensionValue(
+            extensions=["arithmetic.int.types"],
+            typ=hugr_int_type,
+            value=ops.CustomConst(
+                c="ConstInt", v=ConstInt(log_width=INT_WIDTH, value=i)
+            ),
+        )
+    )
 
 
-def float_value(f: float) -> val.Value:
+def float_value(f: float) -> ops.Value:
     """Returns the Hugr representation of a float value."""
-    return val.ExtensionVal(c=(ConstF64(value=f),))
+    return ops.Value(
+        ops.ExtensionValue(
+            extensions=["arithmetic.float.types"],
+            typ=hugr_float_type,
+            value=ops.CustomConst(c="ConstF64", v=ConstF64(value=f)),
+        )
+    )
 
 
-def list_value(v: list[val.Value], ty: tys.Type) -> val.Value:
+def list_value(v: list[ops.Value], ty: Type) -> ops.Value:
     """Returns the Hugr representation of a list value."""
-    return val.ExtensionVal(c=(ListValue(value=(v, ty)),))
+    return ops.Value(
+        ops.ExtensionValue(
+            extensions=["Collections"],
+            typ=list_type(ty).to_hugr(),
+            value=ops.CustomConst(c="ListValue", v=(v, ty.to_hugr())),
+        )
+    )
 
 
 def logic_op(op_name: str, args: list[tys.TypeArg] | None = None) -> ops.OpType:
     """Utility method to create Hugr logic ops."""
-    return ops.CustomOp(extension="logic", op_name=op_name, args=args or [])
+    return ops.OpType(
+        ops.CustomOp(
+            extension="logic", op_name=op_name, args=args or [], parent=UNDEFINED
+        )
+    )
 
 
 def int_op(
     op_name: str, ext: str = "arithmetic.int", num_params: int = 1
 ) -> ops.OpType:
     """Utility method to create Hugr integer arithmetic ops."""
-    return ops.CustomOp(
-        extension=ext,
-        op_name=op_name,
-        args=num_params * [tys.BoundedNatArg(n=INT_WIDTH)],
+    return ops.OpType(
+        ops.CustomOp(
+            extension=ext,
+            op_name=op_name,
+            args=num_params * [tys.TypeArg(tys.BoundedNatArg(n=INT_WIDTH))],
+            parent=UNDEFINED,
+        )
     )
 
 
 def float_op(op_name: str, ext: str = "arithmetic.float") -> ops.OpType:
     """Utility method to create Hugr integer arithmetic ops."""
-    return ops.CustomOp(extension=ext, op_name=op_name, args=[])
+    return ops.OpType(
+        ops.CustomOp(extension=ext, op_name=op_name, args=[], parent=UNDEFINED)
+    )
 
 
 class CoercingChecker(DefaultCallChecker):
     """Function call type checker that automatically coerces arguments to float."""
 
     def synthesize(self, args: list[ast.expr]) -> tuple[ast.expr, Type]:
         from .builtins import Int
 
         for i in range(len(args)):
             args[i], ty = ExprSynthesizer(self.ctx).synthesize(args[i])
-            if (
-                isinstance(ty, OpaqueType)
-                and ty.defn == self.ctx.globals.type_defs["int"]
-            ):
+            if isinstance(ty, OpaqueType) and ty.defn == self.ctx.globals["int"]:
                 call = with_loc(
                     self.node,
-                    GlobalCall(func=Int.__float__, args=[args[i]], type_args=[]),
+                    GlobalCall(def_id=Int.__float__.id, args=[args[i]], type_args=[]),
                 )
+                float_defn = self.ctx.globals["float"]
+                assert isinstance(float_defn, TypeDef)
                 args[i] = with_type(
-                    self.ctx.globals.type_defs["float"].check_instantiate([]), call
+                    float_defn.check_instantiate([], self.ctx.globals), call
                 )
         return super().synthesize(args)
 
 
 class ReversingChecker(CustomCallChecker):
     """Call checker that reverses the arguments after checking."""
 
     base_checker: CustomCallChecker
 
     def __init__(self, base_checker: CustomCallChecker | None = None):
         self.base_checker = base_checker or DefaultCallChecker()
 
-    def _setup(self, ctx: Context, node: AstNode, func: CustomFunction) -> None:
+    def _setup(self, ctx: Context, node: AstNode, func: CustomFunctionDef) -> None:
         super()._setup(ctx, node, func)
         self.base_checker._setup(ctx, node, func)
 
     def check(self, args: list[ast.expr], ty: Type) -> tuple[ast.expr, Subst]:
         expr, subst = self.base_checker.check(args, ty)
         if isinstance(expr, GlobalCall):
             expr.args = list(reversed(args))
@@ -189,17 +223,15 @@
     num_args: int
 
     def __init__(self, dunder_name: str, num_args: int = 1):
         assert num_args > 0
         self.dunder_name = dunder_name
         self.num_args = num_args
 
-    def _get_func(
-        self, args: list[ast.expr]
-    ) -> tuple[list[ast.expr], CallableVariable]:
+    def _get_func(self, args: list[ast.expr]) -> tuple[list[ast.expr], CallableDef]:
         check_num_args(self.num_args, len(args), self.node)
         fst, *rest = args
         fst, ty = ExprSynthesizer(self.ctx).synthesize(fst)
         func = self.ctx.globals.get_instance_func(ty, self.dunder_name)
         if func is None:
             raise GuppyTypeError(
                 f"Builtin function `{self.func.name}` is not defined for argument of "
@@ -251,38 +283,40 @@
         [left, right] = args
         [left] = Int.__float__.compile_call(
             [left], [], self.dfg, self.graph, self.globals, self.node
         )
         [right] = Int.__float__.compile_call(
             [right], [], self.dfg, self.graph, self.globals, self.node
         )
-        return Float.__truediv__.compile_call(
+        [out] = Float.__truediv__.compile_call(
             [left, right], [], self.dfg, self.graph, self.globals, self.node
         )
+        return [out]
 
 
 class FloatBoolCompiler(CustomCallCompiler):
     """Compiler for the `float.__bool__` method."""
 
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
         from .builtins import Float
 
         # We have: bool(x) = (x != 0.0)
         zero_const = self.graph.add_constant(
             float_value(0.0), get_type(self.node), self.dfg.node
         )
         zero = self.graph.add_load_constant(zero_const.out_port(0), self.dfg.node)
-        return Float.__ne__.compile_call(
+        [out] = Float.__ne__.compile_call(
             [args[0], zero.out_port(0)],
             [],
             self.dfg,
             self.graph,
             self.globals,
             self.node,
         )
+        return [out]
 
 
 class FloatFloordivCompiler(CustomCallCompiler):
     """Compiler for the `float.__floordiv__` method."""
 
     def compile(self, args: list[OutPortV]) -> list[OutPortV]:
         from .builtins import Float
```

### Comparing `guppylang-0.2.0/guppylang/prelude/builtins.py` & `guppylang-0.3.0/guppylang/prelude/builtins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Guppy module for builtin types and operations."""
 
 # mypy: disable-error-code="empty-body, misc, override, valid-type, no-untyped-def"
 
-from guppylang.custom import DefaultCallChecker, NoopCompiler
+from hugr.serialization import tys
+
 from guppylang.decorator import guppy
-from guppylang.hugr import ops, tys
+from guppylang.definition.custom import DefaultCallChecker, NoopCompiler
+from guppylang.hugr_builder.hugr import DummyOp
 from guppylang.module import GuppyModule
 from guppylang.prelude._internal import (
     CallableChecker,
     CoercingChecker,
     DunderChecker,
     FailingChecker,
     FloatBoolCompiler,
@@ -20,34 +22,37 @@
     UnsupportedChecker,
     float_op,
     hugr_float_type,
     hugr_int_type,
     int_op,
     logic_op,
 )
-from guppylang.tys.definition import bool_type_def, linst_type_def, list_type_def
+from guppylang.tys.builtin import bool_type_def, linst_type_def, list_type_def
 
 builtins = GuppyModule("builtins", import_builtins=False)
 
 T = guppy.type_var(builtins, "T")
 L = guppy.type_var(builtins, "L", linear=True)
 
 
 @guppy.extend_type(builtins, bool_type_def)
 class Bool:
-    @guppy.hugr_op(builtins, logic_op("And", [tys.BoundedNatArg(n=2)]))
+    @guppy.hugr_op(builtins, logic_op("And", [tys.TypeArg(tys.BoundedNatArg(n=2))]))
     def __and__(self: bool, other: bool) -> bool: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __bool__(self: bool) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ifrombool"))
     def __int__(self: bool) -> int: ...
 
-    @guppy.hugr_op(builtins, logic_op("Or", [tys.BoundedNatArg(n=2)]))
+    @guppy.custom(builtins, checker=DunderChecker("__bool__"), higher_order_value=False)
+    def __new__(x): ...
+
+    @guppy.hugr_op(builtins, logic_op("Or", [tys.TypeArg(tys.BoundedNatArg(n=2))]))
     def __or__(self: bool, other: bool) -> bool: ...
 
 
 @guppy.type(builtins, hugr_int_type, name="int")
 class Int:
     @guppy.hugr_op(builtins, int_op("iabs"))  # TODO: Maybe wrong? (signed vs unsigned!)
     def __abs__(self: int) -> int: ...
@@ -108,21 +113,24 @@
 
     @guppy.hugr_op(builtins, int_op("ine"))
     def __ne__(self: int, other: int) -> bool: ...
 
     @guppy.hugr_op(builtins, int_op("ineg"))
     def __neg__(self: int) -> int: ...
 
+    @guppy.custom(builtins, checker=DunderChecker("__int__"), higher_order_value=False)
+    def __new__(x): ...
+
     @guppy.hugr_op(builtins, int_op("ior"))
     def __or__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __pos__(self: int) -> int: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="ipow"))  # TODO
+    @guppy.hugr_op(builtins, DummyOp("ipow"))  # TODO
     def __pow__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("iadd"), ReversingChecker())
     def __radd__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(builtins, int_op("rand"), ReversingChecker())
     def __rand__(self: int, other: int) -> int: ...
@@ -146,15 +154,15 @@
 
     @guppy.hugr_op(builtins, int_op("ior"), ReversingChecker())
     def __ror__(self: int, other: int) -> int: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __round__(self: int) -> int: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="ipow"), ReversingChecker())  # TODO
+    @guppy.hugr_op(builtins, DummyOp("ipow"), ReversingChecker())  # TODO
     def __rpow__(self: int, other: int) -> int: ...
 
     @guppy.hugr_op(
         builtins, int_op("ishr", num_params=2), ReversingChecker()
     )  # TODO: RHS is unsigned
     def __rrshift__(self: int, other: int) -> int: ...
 
@@ -237,18 +245,23 @@
 
     @guppy.hugr_op(builtins, float_op("fne"), CoercingChecker())
     def __ne__(self: float, other: float) -> bool: ...
 
     @guppy.hugr_op(builtins, float_op("fneg"), CoercingChecker())
     def __neg__(self: float, other: float) -> float: ...
 
+    @guppy.custom(
+        builtins, checker=DunderChecker("__float__"), higher_order_value=False
+    )
+    def __new__(x): ...
+
     @guppy.custom(builtins, NoopCompiler(), CoercingChecker())
     def __pos__(self: float) -> float: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="fpow"))  # TODO
+    @guppy.hugr_op(builtins, DummyOp("fpow"))  # TODO
     def __pow__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fadd"), ReversingChecker(CoercingChecker()))
     def __radd__(self: float, other: float) -> float: ...
 
     @guppy.custom(builtins, FloatDivmodCompiler(), ReversingChecker(CoercingChecker()))
     def __rdivmod__(self: float, other: float) -> tuple[float, float]: ...
@@ -260,19 +273,19 @@
 
     @guppy.custom(builtins, FloatModCompiler(), ReversingChecker(CoercingChecker()))
     def __rmod__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fmul"), ReversingChecker(CoercingChecker()))
     def __rmul__(self: float, other: float) -> float: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="fround"))  # TODO
+    @guppy.hugr_op(builtins, DummyOp("fround"))  # TODO
     def __round__(self: float) -> float: ...
 
     @guppy.hugr_op(
-        builtins, ops.DummyOp(name="fpow"), ReversingChecker(DefaultCallChecker())
+        builtins, DummyOp("fpow"), ReversingChecker(DefaultCallChecker())
     )  # TODO
     def __rpow__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fsub"), ReversingChecker(CoercingChecker()))
     def __rsub__(self: float, other: float) -> float: ...
 
     @guppy.hugr_op(builtins, float_op("fdiv"), ReversingChecker(CoercingChecker()))
@@ -288,69 +301,72 @@
         builtins, float_op("trunc_s", "arithmetic.conversions"), CoercingChecker()
     )
     def __trunc__(self: float) -> float: ...
 
 
 @guppy.extend_type(builtins, list_type_def)
 class List:
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Concat"))
+    @guppy.hugr_op(builtins, DummyOp("Concat"))
     def __add__(self: list[T], other: list[T]) -> list[T]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="IsEmpty"))
+    @guppy.hugr_op(builtins, DummyOp("IsEmpty"))
     def __bool__(self: list[T]) -> bool: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Contains"))
+    @guppy.hugr_op(builtins, DummyOp("Contains"))
     def __contains__(self: list[T], el: T) -> bool: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="AssertEmpty"))
+    @guppy.hugr_op(builtins, DummyOp("AssertEmpty"))
     def __end__(self: list[T]) -> None: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Lookup"))
+    @guppy.hugr_op(builtins, DummyOp("Lookup"))
     def __getitem__(self: list[T], idx: int) -> T: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="IsNonEmpty"))
+    @guppy.hugr_op(builtins, DummyOp("IsNonEmpty"))
     def __hasnext__(self: list[T]) -> tuple[bool, list[T]]: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __iter__(self: list[T]) -> list[T]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Length"))
+    @guppy.hugr_op(builtins, DummyOp("Length"))
     def __len__(self: list[T]) -> int: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"))
+    @guppy.hugr_op(builtins, DummyOp("Repeat"))
     def __mul__(self: list[T], other: int) -> list[T]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Pop"))
+    @guppy.hugr_op(builtins, DummyOp("Pop"))
     def __next__(self: list[T]) -> tuple[T, list[T]]: ...
 
+    @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
+    def __new__(x): ...
+
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def __setitem__(self: list[T], idx: int, value: T) -> None: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Append"), ReversingChecker())
+    @guppy.hugr_op(builtins, DummyOp("Append"), ReversingChecker())
     def __radd__(self: list[T], other: list[T]) -> list[T]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"), ReversingChecker())
+    @guppy.hugr_op(builtins, DummyOp("Repeat"), ReversingChecker())
     def __rmul__(self: list[T], other: int) -> list[T]: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def append(self: list[T], elt: T) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def clear(self: list[T]) -> None: ...
 
     @guppy.custom(builtins, NoopCompiler())  # Can be noop since lists are immutable
     def copy(self: list[T]) -> list[T]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Count"))
+    @guppy.hugr_op(builtins, DummyOp("Count"))
     def count(self: list[T], elt: T) -> int: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def extend(self: list[T], seq: None) -> None: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Find"))
+    @guppy.hugr_op(builtins, DummyOp("Find"))
     def index(self: list[T], elt: T) -> int: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def pop(self: list[T], idx: int) -> None: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def remove(self: list[T], elt: T) -> None: ...
@@ -363,83 +379,68 @@
 
 
 linst = list
 
 
 @guppy.extend_type(builtins, linst_type_def)
 class Linst:
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Append"))
+    @guppy.hugr_op(builtins, DummyOp("Append"))
     def __add__(self: linst[L], other: linst[L]) -> linst[L]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="AssertEmpty"))
+    @guppy.hugr_op(builtins, DummyOp("AssertEmpty"))
     def __end__(self: linst[L]) -> None: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="IsNonempty"))
+    @guppy.hugr_op(builtins, DummyOp("IsNonempty"))
     def __hasnext__(self: linst[L]) -> tuple[bool, linst[L]]: ...
 
     @guppy.custom(builtins, NoopCompiler())
     def __iter__(self: linst[L]) -> linst[L]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Length"))
+    @guppy.hugr_op(builtins, DummyOp("Length"))
     def __len__(self: linst[L]) -> tuple[int, linst[L]]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Pop"))
+    @guppy.hugr_op(builtins, DummyOp("Pop"))
     def __next__(self: linst[L]) -> tuple[L, linst[L]]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Append"), ReversingChecker())
+    @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
+    def __new__(x): ...
+
+    @guppy.hugr_op(builtins, DummyOp("Append"), ReversingChecker())
     def __radd__(self: linst[L], other: linst[L]) -> linst[L]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Repeat"), ReversingChecker())
+    @guppy.hugr_op(builtins, DummyOp("Repeat"), ReversingChecker())
     def __rmul__(self: linst[L], other: int) -> linst[L]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Push"))
+    @guppy.hugr_op(builtins, DummyOp("Push"))
     def append(self: linst[L], elt: L) -> linst[L]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="PopAt"))
+    @guppy.hugr_op(builtins, DummyOp("PopAt"))
     def pop(self: linst[L], idx: int) -> tuple[L, linst[L]]: ...
 
-    @guppy.hugr_op(builtins, ops.DummyOp(name="Reverse"))
+    @guppy.hugr_op(builtins, DummyOp("Reverse"))
     def reverse(self: linst[L]) -> linst[L]: ...
 
     @guppy.custom(builtins, checker=FailingChecker("Guppy lists are immutable"))
     def sort(self: list[T]) -> None: ...
 
 
 @guppy.custom(builtins, checker=DunderChecker("__abs__"), higher_order_value=False)
 def abs(x): ...
 
 
-@guppy.custom(
-    builtins, name="bool", checker=DunderChecker("__bool__"), higher_order_value=False
-)
-def _bool(x): ...
-
-
 @guppy.custom(builtins, checker=CallableChecker(), higher_order_value=False)
 def callable(x): ...
 
 
 @guppy.custom(
     builtins, checker=DunderChecker("__divmod__", num_args=2), higher_order_value=False
 )
 def divmod(x, y): ...
 
 
-@guppy.custom(
-    builtins, name="float", checker=DunderChecker("__float__"), higher_order_value=False
-)
-def _float(x, y): ...
-
-
-@guppy.custom(
-    builtins, name="int", checker=DunderChecker("__int__"), higher_order_value=False
-)
-def _int(x): ...
-
-
 @guppy.custom(builtins, checker=DunderChecker("__len__"), higher_order_value=False)
 def len(x): ...
 
 
 @guppy.custom(
     builtins, checker=DunderChecker("__pow__", num_args=2), higher_order_value=False
 )
@@ -577,20 +578,14 @@
 def issubclass(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def iter(x): ...
 
 
-@guppy.custom(
-    builtins, checker=UnsupportedChecker(), name="list", higher_order_value=False
-)
-def _list(x): ...
-
-
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def locals(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def map(x): ...
 
@@ -675,20 +670,14 @@
 def sum(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def super(x): ...
 
 
-@guppy.custom(
-    builtins, name="tuple", checker=UnsupportedChecker(), higher_order_value=False
-)
-def _tuple(x): ...
-
-
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def type(x): ...
 
 
 @guppy.custom(builtins, checker=UnsupportedChecker(), higher_order_value=False)
 def vars(x): ...
```

### Comparing `guppylang-0.2.0/guppylang/prelude/quantum.py` & `guppylang-0.3.0/guppylang/prelude/quantum.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 """Guppy standard module for quantum operations."""
 
-# mypy: disable-error-code=empty-body
+# mypy: disable-error-code="empty-body, misc"
+
+from hugr.serialization import ops, tys
+from hugr.serialization.tys import TypeBound
 
 from guppylang.decorator import guppy
-from guppylang.hugr import ops, tys
-from guppylang.hugr.tys import TypeBound
+from guppylang.hugr_builder.hugr import UNDEFINED
 from guppylang.module import GuppyModule
 from guppylang.prelude._internal import MeasureCompiler
 
 quantum = GuppyModule("quantum")
 
 
 def quantum_op(op_name: str) -> ops.OpType:
     """Utility method to create Hugr quantum ops."""
-    return ops.CustomOp(extension="quantum.tket2", op_name=op_name, args=[])
+    return ops.OpType(
+        ops.CustomOp(
+            extension="quantum.tket2", op_name=op_name, args=[], parent=UNDEFINED
+        )
+    )
 
 
 @guppy.type(
     quantum,
-    tys.Opaque(extension="prelude", id="qubit", args=[], bound=TypeBound.Any),
+    tys.Type(tys.Opaque(extension="prelude", id="qubit", args=[], bound=TypeBound.Any)),
     linear=True,
 )
 class qubit:
-    pass
+    @guppy.hugr_op(quantum, quantum_op("QAlloc"))
+    def __new__() -> "qubit": ...
 
 
 @guppy.hugr_op(quantum, quantum_op("H"))
 def h(q: qubit) -> qubit: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("CZ"))
@@ -89,18 +96,14 @@
 def zz_phase(q1: qubit, q2: qubit, angle: float) -> tuple[qubit, qubit]: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("TK1"))
 def tk1(q: qubit, angle1: float, angle2: float, angle3: float) -> qubit: ...
 
 
-@guppy.hugr_op(quantum, quantum_op("QAlloc"), name="qubit")
-def _qubit() -> qubit: ...
-
-
 @guppy.hugr_op(quantum, quantum_op("QFree"))
 def discard(q: qubit) -> None: ...
 
 
 @guppy.hugr_op(quantum, quantum_op("Reset"))
 def reset(q: qubit) -> qubit: ...
```

### Comparing `guppylang-0.2.0/guppylang/tys/arg.py` & `guppylang-0.3.0/guppylang/tys/arg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, TypeAlias
 
-from guppylang.hugr import tys
+from hugr.serialization import tys
+
 from guppylang.tys.common import ToHugr, Transformable, Transformer, Visitor
 from guppylang.tys.const import Const
 from guppylang.tys.var import ExistentialVar
 
 if TYPE_CHECKING:
     from guppylang.tys.ty import Type
 
@@ -43,15 +44,15 @@
     @property
     def unsolved_vars(self) -> set[ExistentialVar]:
         """The existential type variables contained in this argument."""
         return self.ty.unsolved_vars
 
     def to_hugr(self) -> tys.TypeArg:
         """Computes the Hugr representation of the argument."""
-        return tys.TypeTypeArg(ty=self.ty.to_hugr())
+        return tys.TypeArg(tys.TypeTypeArg(ty=self.ty.to_hugr()))
 
     def visit(self, visitor: Visitor) -> None:
         """Accepts a visitor on this argument."""
         if not visitor.visit(self):
             self.ty.visit(visitor)
 
     def transform(self, transformer: Transformer) -> Argument:
```

### Comparing `guppylang-0.2.0/guppylang/tys/common.py` & `guppylang-0.3.0/guppylang/tys/common.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/tys/const.py` & `guppylang-0.3.0/guppylang/tys/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABC
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
+from hugr.serialization import ops
+
 from guppylang.error import InternalGuppyError
-from guppylang.hugr import val
 from guppylang.tys.var import BoundVar, ExistentialVar
 
 if TYPE_CHECKING:
     from guppylang.tys.ty import Type
 
 
 @dataclass(frozen=True)
@@ -32,15 +33,15 @@
 
     For example, in the type `array[int, 5]` the second argument is a `ConstArg`  that
     contains a `ConstValue(5)`.
     """
 
     # Hugr encoding of the value
     # TODO: We might need a Guppy representation of this...
-    value: val.Value
+    value: ops.Value
 
 
 @dataclass(frozen=True)
 class BoundConstVar(BoundVar, Const):
     """Bound variable referencing a `ConstParam`.
 
     For example, in the function type `forall n: int. array[float, n] -> array[int, n]`,
```

### Comparing `guppylang-0.2.0/guppylang/tys/definition.py` & `guppylang-0.3.0/guppylang/tys/builtin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,81 +1,36 @@
-from abc import ABC, abstractmethod
-from collections.abc import Callable, Sequence
+from collections.abc import Sequence
 from dataclasses import dataclass, field
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
+
+from hugr.serialization import tys
 
 from guppylang.ast_util import AstNode
+from guppylang.definition.common import DefId
+from guppylang.definition.ty import OpaqueTypeDef, TypeDef
 from guppylang.error import GuppyError
-from guppylang.hugr import tys
 from guppylang.tys.arg import Argument, TypeArg
-from guppylang.tys.param import Parameter, TypeParam
+from guppylang.tys.param import TypeParam
 from guppylang.tys.ty import FunctionType, NoneType, OpaqueType, TupleType, Type
 
-
-@dataclass(frozen=True)
-class TypeDef(ABC):
-    """Abstract base class for type definitions."""
-
-    name: str
-
-    @abstractmethod
-    def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
-    ) -> Type:
-        """Checks if the type definition can be instantiated with the given arguments.
-
-        Returns the resulting concrete type or raises a user error if the arguments are
-        invalid.
-        """
-
-
-@dataclass(frozen=True)
-class OpaqueTypeDef(TypeDef):
-    """An opaque type definition that is backed by some Hugr type."""
-
-    params: Sequence[Parameter]
-    always_linear: bool
-    to_hugr: Callable[[Sequence[Argument]], tys.Type]
-    bound: tys.TypeBound | None = None
-
-    def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
-    ) -> OpaqueType:
-        """Checks if the type definition can be instantiated with the given arguments.
-
-        Returns the resulting concrete type or raises a user error if the arguments are
-        invalid.
-        """
-        exp, act = len(self.params), len(args)
-        if exp > act:
-            raise GuppyError(f"Missing parameter for type `{self.name}`", loc)
-        elif 0 == exp < act:
-            raise GuppyError(f"Type `{self.name}` is not parameterized", loc)
-        elif 0 < exp < act:
-            raise GuppyError(f"Too many parameters for type `{self.name}`", loc)
-
-        # Now check that the kinds match up
-        for param, arg in zip(self.params, args, strict=True):
-            # TODO: The error location is bad. We want the location of `arg`, not of the
-            #  whole thing.
-            param.check_arg(arg, loc)
-        return OpaqueType(args, self)
+if TYPE_CHECKING:
+    from guppylang.checker.core import Globals
 
 
 @dataclass(frozen=True)
 class _CallableTypeDef(TypeDef):
     """Type definition associated with the builtin `Callable` type.
 
     Any impls on functions can be registered with this definition.
     """
 
     name: Literal["Callable"] = field(default="Callable", init=False)
 
     def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
+        self, args: Sequence[Argument], globals: "Globals", loc: AstNode | None = None
     ) -> FunctionType:
         # We get the inputs/output as a flattened list: `args = [*inputs, output]`.
         if not args:
             raise GuppyError(f"Missing parameter for type `{self.name}`", loc)
         args = [
             # TODO: Better error location
             TypeParam(0, f"T{i}", can_be_linear=True).check_arg(arg, loc).ty
@@ -91,15 +46,15 @@
 
     Any impls on tuples can be registered with this definition.
     """
 
     name: Literal["tuple"] = field(default="tuple", init=False)
 
     def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
+        self, args: Sequence[Argument], globals: "Globals", loc: AstNode | None = None
     ) -> TupleType:
         # We accept any number of arguments. If users just write `tuple`, we give them
         # the empty tuple type. We just have to make sure that the args are of kind type
         args = [
             # TODO: Better error location
             TypeParam(0, f"T{i}", can_be_linear=True).check_arg(arg, loc).ty
             for i, arg in enumerate(args)
@@ -113,15 +68,15 @@
 
     Any impls on None can be registered with this definition.
     """
 
     name: Literal["None"] = field(default="None", init=False)
 
     def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
+        self, args: Sequence[Argument], globals: "Globals", loc: AstNode | None = None
     ) -> NoneType:
         if args:
             raise GuppyError("Type `None` is not parameterized", loc)
         return NoneType()
 
 
 @dataclass(frozen=True)
@@ -129,53 +84,61 @@
     """Type definition associated with the builtin `list` type.
 
     We have a custom definition to give a nicer error message if the user tries to put
     linear data into a regular list.
     """
 
     def check_instantiate(
-        self, args: Sequence[Argument], loc: AstNode | None = None
+        self, args: Sequence[Argument], globals: "Globals", loc: AstNode | None = None
     ) -> OpaqueType:
         if len(args) == 1:
             [arg] = args
             if isinstance(arg, TypeArg) and arg.ty.linear:
                 raise GuppyError(
                     "Type `list` cannot store linear data, use `linst` instead", loc
                 )
-        return super().check_instantiate(args, loc)
+        return super().check_instantiate(args, globals, loc)
 
 
-def _list_to_hugr(args: Sequence[Argument]) -> tys.Opaque:
-    return tys.Opaque(
+def _list_to_hugr(args: Sequence[Argument]) -> tys.Type:
+    # Type checker ensures that we get a single arg of kind type
+    [arg] = args
+    assert isinstance(arg, TypeArg)
+    ty = tys.Opaque(
         extension="Collections",
         id="List",
-        args=[arg.to_hugr() for arg in args],
-        bound=tys.TypeBound.join(
-            *(arg.ty.hugr_bound for arg in args if isinstance(arg, TypeArg))
-        ),
+        args=[arg.to_hugr()],
+        bound=arg.ty.hugr_bound,
     )
+    return tys.Type(ty)
 
 
-callable_type_def = _CallableTypeDef()
-tuple_type_def = _TupleTypeDef()
-none_type_def = _NoneTypeDef()
+callable_type_def = _CallableTypeDef(DefId.fresh(), None)
+tuple_type_def = _TupleTypeDef(DefId.fresh(), None)
+none_type_def = _NoneTypeDef(DefId.fresh(), None)
 bool_type_def = OpaqueTypeDef(
+    id=DefId.fresh(),
     name="bool",
+    defined_at=None,
     params=[],
     always_linear=False,
-    to_hugr=lambda _: tys.UnitSum(size=2),
+    to_hugr=lambda _: tys.Type(tys.SumType(tys.UnitSum(size=2))),
 )
 linst_type_def = OpaqueTypeDef(
+    id=DefId.fresh(),
     name="linst",
+    defined_at=None,
     params=[TypeParam(0, "T", can_be_linear=True)],
     always_linear=False,
     to_hugr=_list_to_hugr,
 )
 list_type_def = _ListTypeDef(
+    id=DefId.fresh(),
     name="list",
+    defined_at=None,
     params=[TypeParam(0, "T", can_be_linear=False)],
     always_linear=False,
     to_hugr=_list_to_hugr,
 )
 
 
 def bool_type() -> OpaqueType:
```

### Comparing `guppylang-0.2.0/guppylang/tys/param.py` & `guppylang-0.3.0/guppylang/tys/param.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from abc import ABC, abstractmethod
+from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, TypeAlias
 
+from hugr.serialization import tys
+from hugr.serialization.tys import TypeBound
 from typing_extensions import Self
 
 from guppylang.ast_util import AstNode
-from guppylang.error import GuppyTypeError, InternalGuppyError
-from guppylang.hugr import tys
-from guppylang.hugr.tys import TypeBound
+from guppylang.error import GuppyError, GuppyTypeError, InternalGuppyError
 from guppylang.tys.arg import Argument, ConstArg, TypeArg
 from guppylang.tys.common import ToHugr
 from guppylang.tys.var import ExistentialVar
 
 if TYPE_CHECKING:
     from guppylang.tys.ty import Type
 
@@ -117,16 +118,18 @@
 
         if idx is None:
             idx = self.idx
         return TypeArg(BoundTypeVar(self.name, idx, self.can_be_linear))
 
     def to_hugr(self) -> tys.TypeParam:
         """Computes the Hugr representation of the parameter."""
-        return tys.TypeTypeParam(
-            b=tys.TypeBound.Any if self.can_be_linear else TypeBound.Copyable
+        return tys.TypeParam(
+            tys.TypeTypeParam(
+                b=tys.TypeBound.Any if self.can_be_linear else TypeBound.Copyable
+            )
         )
 
 
 @dataclass(frozen=True)
 class ConstParam(ParameterBase):
     """A parameter of kind constant. Used to define fixed-size arrays etc.
 
@@ -165,7 +168,33 @@
         parameter.
         """
         raise NotImplementedError
 
     def to_hugr(self) -> tys.TypeParam:
         """Computes the Hugr representation of the parameter."""
         raise NotImplementedError
+
+
+def check_all_args(
+    params: Sequence[Parameter],
+    args: Sequence[Argument],
+    type_name: str,
+    loc: AstNode | None = None,
+) -> None:
+    """Checks a list of arguments against the given parameters.
+
+    Raises a user error if number of arguments doesn't match or one of the argument is
+    invalid.
+    """
+    exp, act = len(params), len(args)
+    if exp > act:
+        raise GuppyError(f"Missing parameter for type `{type_name}`", loc)
+    elif 0 == exp < act:
+        raise GuppyError(f"Type `{type_name}` is not parameterized", loc)
+    elif 0 < exp < act:
+        raise GuppyError(f"Too many parameters for type `{type_name}`", loc)
+
+    # Now check that the kinds match up
+    for param, arg in zip(params, args, strict=True):
+        # TODO: The error location is bad. We want the location of `arg`, not of the
+        #  whole thing.
+        param.check_arg(arg, loc)
```

### Comparing `guppylang-0.2.0/guppylang/tys/parsing.py` & `guppylang-0.3.0/guppylang/tys/parsing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 import ast
 from collections.abc import Sequence
 
-from guppylang.ast_util import AstNode
+from guppylang.ast_util import (
+    AstNode,
+    set_location_from,
+    shift_loc,
+)
 from guppylang.checker.core import Globals
+from guppylang.definition.parameter import ParamDef
+from guppylang.definition.ty import TypeDef
 from guppylang.error import GuppyError
 from guppylang.tys.arg import Argument, TypeArg
 from guppylang.tys.param import Parameter, TypeParam
 from guppylang.tys.ty import NoneType, TupleType, Type
 
 
 def arg_from_ast(
@@ -14,58 +20,67 @@
     globals: Globals,
     param_var_mapping: dict[str, Parameter] | None = None,
 ) -> Argument:
     """Turns an AST expression into an argument."""
     # A single identifier
     if isinstance(node, ast.Name):
         x = node.id
-        # Either a defined type (e.g. `int`, `bool`, ...)
-        if x in globals.type_defs:
-            ty = globals.type_defs[x].check_instantiate([], node)
-            return TypeArg(ty)
-        # Or a parameter (e.g. `T`, `n`, ...)
-        if x in globals.param_vars:
-            if param_var_mapping is None:
+        if x not in globals:
+            raise GuppyError("Unknown identifier", node)
+        match globals[x]:
+            # Either a defined type (e.g. `int`, `bool`, ...)
+            case TypeDef() as defn:
+                return TypeArg(defn.check_instantiate([], globals, node))
+            # Or a parameter (e.g. `T`, `n`, ...)
+            case ParamDef() as defn:
+                if param_var_mapping is None:
+                    raise GuppyError(
+                        "Free type variable. Only function types can be generic", node
+                    )
+                if x not in param_var_mapping:
+                    param_var_mapping[x] = defn.to_param(len(param_var_mapping))
+                return param_var_mapping[x].to_bound()
+            case defn:
                 raise GuppyError(
-                    "Free type variable. Only function types can be generic", node
+                    f"Expected a type, got {defn.description} `{defn.name}`", node
                 )
-            var = globals.param_vars[x]
-            if var.name not in param_var_mapping:
-                param_var_mapping[var.name] = var.with_idx(len(param_var_mapping))
-            return param_var_mapping[var.name].to_bound()
-        raise GuppyError("Unknown identifier", node)
 
     # A parametrised type, e.g. `list[??]`
     if isinstance(node, ast.Subscript) and isinstance(node.value, ast.Name):
         x = node.value.id
-        if x in globals.type_defs:
-            arg_nodes = (
-                node.slice.elts if isinstance(node.slice, ast.Tuple) else [node.slice]
-            )
-            # Hack: Flatten argument lists to support the `Callable` type. For example,
-            # we turn `Callable[[int, int], bool]` into `Callable[int, int, bool]`.
-            # TODO: We can get rid of this once we added support for variadic params
-            arg_nodes = [
-                n
-                for arg in arg_nodes
-                for n in (arg.elts if isinstance(arg, ast.List) else (arg,))
-            ]
-            args = [
-                arg_from_ast(arg_node, globals, param_var_mapping)
-                for arg_node in arg_nodes
-            ]
-            ty = globals.type_defs[x].check_instantiate(args, node)
-            return TypeArg(ty)
-        # We don't allow parametrised variables like `T[int]`
-        if x in globals.param_vars:
-            raise GuppyError(
-                f"Variable `{x}` is not parameterized. Higher-kinded types are not "
-                f"supported",
-                node,
-            )
+        if x in globals:
+            defn = globals[x]
+            if isinstance(defn, TypeDef):
+                arg_nodes = (
+                    node.slice.elts
+                    if isinstance(node.slice, ast.Tuple)
+                    else [node.slice]
+                )
+                # Hack: Flatten argument lists to support the `Callable` type. For
+                # example, we turn `Callable[[int, int], bool]` into
+                # `Callable[int, int, bool]`.
+                # TODO: We can get rid of this once we added support for variadic params
+                arg_nodes = [
+                    n
+                    for arg in arg_nodes
+                    for n in (arg.elts if isinstance(arg, ast.List) else (arg,))
+                ]
+                args = [
+                    arg_from_ast(arg_node, globals, param_var_mapping)
+                    for arg_node in arg_nodes
+                ]
+                ty = defn.check_instantiate(args, globals, node)
+                return TypeArg(ty)
+            # We don't allow parametrised variables like `T[int]`
+            if isinstance(defn, ParamDef):
+                raise GuppyError(
+                    f"Variable `{x}` is not parameterized. Higher-kinded types are not "
+                    f"supported",
+                    node,
+                )
 
     # We allow tuple types to be written as `(int, bool)`
     if isinstance(node, ast.Tuple):
         ty = TupleType(
             [type_from_ast(el, globals, param_var_mapping) for el in node.elts]
         )
         return TypeArg(ty)
@@ -76,14 +91,20 @@
 
     # Finally, we also support delayed annotations in strings
     if isinstance(node, ast.Constant) and isinstance(node.value, str):
         try:
             [stmt] = ast.parse(node.value).body
             if not isinstance(stmt, ast.Expr):
                 raise GuppyError("Invalid Guppy type", node)
+            set_location_from(stmt, loc=node)
+            shift_loc(
+                stmt,
+                delta_lineno=node.lineno - 1,  # -1 since lines start at 1
+                delta_col_offset=node.col_offset + 1,  # +1 to remove the `"`
+            )
             return arg_from_ast(stmt.value, globals, param_var_mapping)
         except (SyntaxError, ValueError):
             raise GuppyError("Invalid Guppy type", node) from None
 
     raise GuppyError("Not a valid type argument", node)
```

### Comparing `guppylang-0.2.0/guppylang/tys/printing.py` & `guppylang-0.3.0/guppylang/tys/printing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from guppylang.error import InternalGuppyError
 from guppylang.tys.arg import ConstArg, TypeArg
 from guppylang.tys.param import ConstParam, TypeParam
 from guppylang.tys.ty import (
     FunctionType,
     NoneType,
     OpaqueType,
+    StructType,
     SumType,
     TupleType,
     Type,
 )
 from guppylang.tys.var import BoundVar, ExistentialVar, UniqueId
 
 
@@ -77,16 +78,19 @@
         output = self._visit(ty.output, True)
         if ty.parametrized:
             quantified = ", ".join([self._visit(param, False) for param in ty.params])
             del self.bound_names[: -len(ty.params)]
             return _wrap(f"forall {quantified}. {inputs} -> {output}", inside_row)
         return _wrap(f"{inputs} -> {output}", inside_row)
 
-    @_visit.register
-    def _visit_OpaqueType(self, ty: OpaqueType, inside_row: bool) -> str:
+    @_visit.register(OpaqueType)
+    @_visit.register(StructType)
+    def _visit_OpaqueType_StructType(
+        self, ty: OpaqueType | StructType, inside_row: bool
+    ) -> str:
         if ty.args:
             args = ", ".join(self._visit(arg, True) for arg in ty.args)
             return f"{ty.defn.name}[{args}]"
         return ty.defn.name
 
     @_visit.register
     def _visit_TupleType(self, ty: TupleType, inside_row: bool) -> str:
```

### Comparing `guppylang-0.2.0/guppylang/tys/subst.py` & `guppylang-0.3.0/guppylang/tys/subst.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/guppylang/tys/ty.py` & `guppylang-0.3.0/guppylang/tys/ty.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import ABC, abstractmethod
 from collections.abc import Sequence
 from dataclasses import dataclass, field
 from functools import cached_property
 from typing import TYPE_CHECKING, TypeAlias, cast
 
+from hugr.serialization import tys
+from hugr.serialization.tys import TypeBound
+
 from guppylang.error import InternalGuppyError
-from guppylang.hugr import tys
-from guppylang.hugr.tys import TypeBound
 from guppylang.tys.arg import Argument, ConstArg, TypeArg
 from guppylang.tys.common import ToHugr, Transformable, Transformer, Visitor
 from guppylang.tys.const import ExistentialConstVar
 from guppylang.tys.param import Parameter
 from guppylang.tys.var import BoundVar, ExistentialVar
 
 if TYPE_CHECKING:
-    from guppylang.tys.definition import OpaqueTypeDef
+    from guppylang.definition.struct import CheckedStructDef, StructField
+    from guppylang.definition.ty import OpaqueTypeDef
     from guppylang.tys.subst import Inst, Subst
 
 
 @dataclass(frozen=True)
 class TypeBase(ToHugr[tys.Type], Transformable["Type"], ABC):
     """Abstract base class for all Guppy types.
 
@@ -144,15 +146,15 @@
             return TypeBound.Any
         # We're conservative and don't require equatability for non-linear variables.
         # This is fine since Guppy doesn't use the equatable feature anyways.
         return TypeBound.Copyable
 
     def to_hugr(self) -> tys.Type:
         """Computes the Hugr representation of the type."""
-        return tys.Variable(i=self.idx, b=self.hugr_bound)
+        return tys.Type(tys.Variable(i=self.idx, b=self.hugr_bound))
 
     def visit(self, visitor: Visitor) -> None:
         """Accepts a visitor on this type."""
         visitor.visit(self)
 
     def transform(self, transformer: Transformer) -> "Type":
         """Accepts a transformer on this type."""
@@ -217,15 +219,15 @@
     # Flag to avoid turning the type into a row when calling `type_to_row()`. This is
     # used to make sure that type vars instantiated to Nones are not broken up into
     # empty rows when generating a Hugr
     preserve: bool = field(default=False, compare=False)
 
     def to_hugr(self) -> tys.Type:
         """Computes the Hugr representation of the type."""
-        return tys.TupleType(inner=[])
+        return TupleType([]).to_hugr()
 
     def visit(self, visitor: Visitor) -> None:
         """Accepts a visitor on this type."""
         visitor.visit(self)
 
     def transform(self, transformer: Transformer) -> "Type":
         """Accepts a transformer on this type."""
@@ -265,18 +267,35 @@
     @property
     def parametrized(self) -> bool:
         """Whether the function is parametrized."""
         return len(self.params) > 0
 
     def to_hugr(self) -> tys.Type:
         """Computes the Hugr representation of the type."""
+        if self.parametrized:
+            raise InternalGuppyError(
+                "Tried to convert parametrised function type to Hugr. Use "
+                "`to_hugr_poly` instead"
+            )
+        return tys.Type(self._to_hugr_function_type())
+
+    def to_hugr_poly(self) -> tys.PolyFuncType:
+        """Computes the Hugr `PolyFuncType` representation of the type."""
+        func_ty = self._to_hugr_function_type()
+        return tys.PolyFuncType(params=[p.to_hugr() for p in self.params], body=func_ty)
+
+    def _to_hugr_function_type(self) -> tys.FunctionType:
+        """Helper method to compute the Hugr `FunctionType` representation of the type.
+
+        The resulting `FunctionType` can then be embedded into a Hugr `Type` or a Hugr
+        `PolyFuncType`.
+        """
         ins = [t.to_hugr() for t in self.inputs]
         outs = [t.to_hugr() for t in type_to_row(self.output)]
-        func_ty = tys.FunctionType(input=ins, output=outs, extension_reqs=[])
-        return tys.PolyFuncType(params=[p.to_hugr() for p in self.params], body=func_ty)
+        return tys.FunctionType(input=ins, output=outs)
 
     def visit(self, visitor: Visitor) -> None:
         """Accepts a visitor on this type."""
         if not visitor.visit(self):
             for inp in self.inputs:
                 visitor.visit(inp)
             visitor.visit(self.output)
@@ -341,15 +360,20 @@
 
     @property
     def intrinsically_linear(self) -> bool:
         return False
 
     def to_hugr(self) -> tys.Type:
         """Computes the Hugr representation of the type."""
-        return tys.TupleType(inner=[ty.to_hugr() for ty in self.element_types])
+        # Tuples are encoded as a unary sum. Note that we need to make a copy of this
+        # tuple with `preserve=False` to ensure that it can be broken up into a row (if
+        # this tuple was created by instantiating a type variable, it is still
+        # represented as a *row* sum).
+        tuple_ty = TupleType(self.element_types, preserve=False)
+        return SumType([tuple_ty]).to_hugr()
 
     def transform(self, transformer: Transformer) -> "Type":
         """Accepts a transformer on this type."""
         return transformer.transform(self) or TupleType(
             [ty.transform(transformer) for ty in self.element_types], self.preserve
         )
 
@@ -372,20 +396,21 @@
 
     @property
     def intrinsically_linear(self) -> bool:
         return False
 
     def to_hugr(self) -> tys.Type:
         """Computes the Hugr representation of the type."""
-        if all(
-            isinstance(e, TupleType) and len(e.element_types) == 0
-            for e in self.element_types
-        ):
-            return tys.UnitSum(size=len(self.element_types))
-        return tys.GeneralSum(row=[t.to_hugr() for t in self.element_types])
+        rows = [type_to_row(ty) for ty in self.element_types]
+        sum_inner: tys.UnitSum | tys.GeneralSum
+        if all(len(row) == 0 for row in rows):
+            sum_inner = tys.UnitSum(size=len(rows))
+        else:
+            sum_inner = tys.GeneralSum(rows=rows_to_hugr(rows))
+        return tys.Type(tys.SumType(sum_inner))
 
     def transform(self, transformer: Transformer) -> "Type":
         """Accepts a transformer on this type."""
         return transformer.transform(self) or SumType(
             [ty.transform(transformer) for ty in self.element_types]
         )
 
@@ -419,23 +444,62 @@
     def transform(self, transformer: Transformer) -> "Type":
         """Accepts a transformer on this type."""
         return transformer.transform(self) or OpaqueType(
             [arg.transform(transformer) for arg in self.args], self.defn
         )
 
 
-# We define the `Type` type as a union of all `TypeBase` subclasses defined above. This
-# models an algebraic data type and enables exhaustiveness checking in pattern matches
-# etc.
-# Note that this might become obsolete in case the `@sealed` decorator is added:
-#  * https://peps.python.org/pep-0622/#sealed-classes-as-algebraic-data-types
-#  * https://github.com/johnthagen/sealed-typing-pep
-ParametrizedType: TypeAlias = FunctionType | TupleType | SumType | OpaqueType
+@dataclass(frozen=True)
+class StructType(ParametrizedTypeBase):
+    """A struct type."""
+
+    defn: "CheckedStructDef"
+
+    @cached_property
+    def fields(self) -> list["StructField"]:
+        """The fields of this struct type."""
+        from guppylang.definition.struct import StructField
+        from guppylang.tys.subst import Instantiator
+
+        inst = Instantiator(self.args)
+        return [StructField(f.name, f.ty.transform(inst)) for f in self.defn.fields]
+
+    @cached_property
+    def intrinsically_linear(self) -> bool:
+        """Whether this type is linear, independent of the arguments."""
+        return any(f.ty.linear for f in self.defn.fields)
+
+    def to_hugr(self) -> tys.Type:
+        """Computes the Hugr representation of the type."""
+        return TupleType([f.ty for f in self.fields]).to_hugr()
+
+    def transform(self, transformer: Transformer) -> "Type":
+        """Accepts a transformer on this type."""
+        return transformer.transform(self) or StructType(
+            [arg.transform(transformer) for arg in self.args], self.defn
+        )
+
+
+#: The type of parametrized Guppy types.
+ParametrizedType: TypeAlias = (
+    FunctionType | TupleType | SumType | OpaqueType | StructType
+)
+
+#: The type of Guppy types.
+#:
+#: This is a type alias for a union of all Guppy types defined in this module. This
+#: models an algebraic data type and enables exhaustiveness checking in pattern matches
+#: etc.
+#:
+#: This might become obsolete in case the @sealed decorator is added:
+#:   * https://peps.python.org/pep-0622/#sealed-classes-as-algebraic-data-types
+#:   * https://github.com/johnthagen/sealed-typing-pep
 Type: TypeAlias = BoundTypeVar | ExistentialTypeVar | NoneType | ParametrizedType
 
+#: An immutable row of Guppy types.
 TypeRow: TypeAlias = Sequence[Type]
 
 
 def row_to_type(row: TypeRow) -> Type:
     """Turns a row of types into a single type by packing into a tuple."""
     if len(row) == 0:
         return NoneType()
@@ -450,14 +514,24 @@
     if isinstance(ty, NoneType) and not ty.preserve:
         return []
     if isinstance(ty, TupleType) and not ty.preserve:
         return ty.element_types
     return [ty]
 
 
+def row_to_hugr(row: TypeRow) -> tys.TypeRow:
+    """Computes the Hugr representation of a type row."""
+    return [ty.to_hugr() for ty in row]
+
+
+def rows_to_hugr(rows: Sequence[TypeRow]) -> list[tys.TypeRow]:
+    """Computes the Hugr representation of a sequence of rows."""
+    return [row_to_hugr(row) for row in rows]
+
+
 def unify(s: Type, t: Type, subst: "Subst | None") -> "Subst | None":
     """Computes a most general unifier for two types.
 
     Return a substitutions `subst` such that `s[subst] == t[subst]` or `None` if this
     not possible.
     """
     if subst is None:
@@ -477,14 +551,16 @@
             return _unify_args(s, t, subst)
         case TupleType() as s, TupleType() as t:
             return _unify_args(s, t, subst)
         case SumType() as s, SumType() as t:
             return _unify_args(s, t, subst)
         case OpaqueType() as s, OpaqueType() as t if s.defn == t.defn:
             return _unify_args(s, t, subst)
+        case StructType() as s, StructType() as t if s.defn == t.defn:
+            return _unify_args(s, t, subst)
         case _:
             return None
 
 
 def _unify_var(var: ExistentialTypeVar, t: Type, subst: "Subst") -> "Subst | None":
     """Helper function for unification of type variables."""
     if var in subst:
@@ -510,7 +586,36 @@
                     return None
                 subst = res
             case ConstArg(), ConstArg():
                 raise NotImplementedError
             case _:
                 return None
     return subst
+
+
+### Helpers for working with tuples of functions
+
+
+def parse_function_tensor(ty: TupleType) -> list[FunctionType] | None:
+    """Parses a nested tuple of function types into a flat list of functions."""
+    result = []
+    for el in ty.element_types:
+        if isinstance(el, FunctionType):
+            result.append(el)
+        elif isinstance(el, TupleType):
+            funcs = parse_function_tensor(el)
+            if funcs:
+                result.extend(funcs)
+            else:
+                return None
+    return result
+
+
+def function_tensor_signature(tys: list[FunctionType]) -> FunctionType:
+    """Compute the combined function signature of a list of functions"""
+    inputs: list[Type] = []
+    outputs: list[Type] = []
+    for fun_ty in tys:
+        assert not fun_ty.parametrized
+        inputs.extend(fun_ty.inputs)
+        outputs.extend(type_to_row(fun_ty.output))
+    return FunctionType(inputs, row_to_type(outputs))
```

### Comparing `guppylang-0.2.0/guppylang/tys/var.py` & `guppylang-0.3.0/guppylang/tys/var.py`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/pyproject.toml` & `guppylang-0.3.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 [tool.poetry]
 name = "guppylang"
-version = "0.2.0"
+version = "0.3.0"
 description = "Pythonic quantum-classical programming language"
 authors = ["Mark Koch <mark.koch@quantinuum.com>"]
 license = "Apache-2.0"
 readme = "quickstart.md"
 repository = "https://github.com/CQCL/guppy"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 graphviz = "^0.20.1"
 networkx = "^3.2.1"
 pydantic = "^2.7.0b1"
 typing-extensions = "^4.9.0"
+hugr = "~0.2.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.4"
 pytest-cov = "^4.1.0"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
-ruff = ">=0.3"
+ruff = ">=0.4.2"
 maturin = "^1.4.0"
 pytket = "*"
 
 [tool.poetry.group.validation]
 optional = true
 
 [tool.poetry.group.validation.dependencies]
@@ -31,21 +32,26 @@
 
 
 [tool.poetry.group.pytket]
 optional = true
 
 [tool.poetry.group.pytket.dependencies]
 pytket = { version = "^1.24.0" }
-tket2-py = { git = "https://github.com/CQCL/tket2.git", rev = "9e941f3" }
+tket2-py = { git = "https://github.com/CQCL/tket2.git", rev = "8aff57a65d42aae631c89ee86f6f1fc7bb1b4da8" }
+
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^7.2.6"
+sphinx-book-theme = "^1.1.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 plugins = ["pydantic.mypy"]
 strict = true
 allow_redefinition = true
-# mypy doesn't support TypeAliasType fully yet
-# https://github.com/python/mypy/issues/16614
-disable_error_code = "valid-type"
```

### Comparing `guppylang-0.2.0/quickstart.md` & `guppylang-0.3.0/quickstart.md`

 * *Files identical despite different names*

### Comparing `guppylang-0.2.0/PKG-INFO` & `guppylang-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: guppylang
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pythonic quantum-classical programming language
 Home-page: https://github.com/CQCL/guppy
 License: Apache-2.0
 Author: Mark Koch
 Author-email: mark.koch@quantinuum.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: graphviz (>=0.20.1,<0.21.0)
+Requires-Dist: hugr (>=0.2.1,<0.3.0)
 Requires-Dist: networkx (>=3.2.1,<4.0.0)
 Requires-Dist: pydantic (>=2.7.0b1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Project-URL: Repository, https://github.com/CQCL/guppy
 Description-Content-Type: text/markdown
 
 Guppy is a quantum programming language that is fully embedded into Python. It
```

