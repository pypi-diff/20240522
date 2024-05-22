# Comparing `tmp/typeshed_stats-23.2.1.tar.gz` & `tmp/typeshed_stats-24.5.21.tar.gz`

## Comparing `typeshed_stats-23.2.1.tar` & `typeshed_stats-24.5.21.tar`

### file list

```diff
@@ -1,56 +1,50 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.editorconfig
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.flake8
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.gitattributes
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.markdownlint.yaml
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/mkdocs.yml
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/website_macros.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/renovate.json
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/check-requirements.yml
--rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/regen-examples-and-docs.yml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/test-website.yml
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0    19907 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/examples/example.csv
--rw-r--r--   0        0        0   137928 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/examples/example.json
--rw-r--r--   0        0        0   239577 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/examples/example.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/docs.txt
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/flake8.txt
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/misc-lint.txt
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/mypy.txt
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/pytest.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/requirements/rich.txt
--rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/scripts/regenerate.py
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/scripts/runtests.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/__init__.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/__main__.py
--rw-r--r--   0        0        0    10916 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/_cli.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/_markdown_template.md.jinja
--rw-r--r--   0        0        0    44887 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/gather.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/py.typed
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/src/typeshed_stats/serialize.py
--rw-r--r--   0        0        0  1796956 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/big_logo.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/cli.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/gather.md
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/index.md
--rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/logo.png
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/serialize.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/stats-csv.md
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/stats.md
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/.snippets/links.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/.snippets/refs.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/javascripts/filtertable.js
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/stats_website/javascripts/tablesort.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/__init__.py
--rw-r--r--   0        0        0     8935 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/conftest.py
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/test___all__.py
--rw-r--r--   0        0        0    21873 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/test__cli.py
--rw-r--r--   0        0        0    36603 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/test_gather.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/test_running_from_command_line.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/tests/test_serialize.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/LICENSE
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/README.md
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/pyproject.toml
--rw-r--r--   0        0        0     8329 2020-02-02 00:00:00.000000 typeshed_stats-23.2.1/PKG-INFO
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.editorconfig
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.gitattributes
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.markdownlint.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/mkdocs.yml
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/website_macros.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/renovate.json5
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/check-requirements.yml
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/regen-examples-and-docs.yml
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/test-website.yml
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.github/workflows/typecheck.yml
+-rw-r--r--   0        0        0    31439 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.csv
+-rw-r--r--   0        0        0   170878 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.json
+-rw-r--r--   0        0        0   286068 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/examples/example.md
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/scripts/regenerate.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/scripts/runtests.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/__init__.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/__main__.py
+-rw-r--r--   0        0        0    10933 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_cli.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_markdown_template.md.jinja
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/_version.py
+-rw-r--r--   0        0        0    50756 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/gather.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/py.typed
+-rw-r--r--   0        0        0     7855 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/src/typeshed_stats/serialize.py
+-rw-r--r--   0        0        0   791271 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/big_logo.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/cli.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/gather.md
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/index.md
+-rw-r--r--   0        0        0   111209 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/logo.png
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/serialize.md
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/stats-csv.md
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/stats.md
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/.snippets/links.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/.snippets/refs.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/javascripts/filtertable.js
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/stats_website/javascripts/tablesort.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/__init__.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/conftest.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test___all__.py
+-rw-r--r--   0        0        0    22122 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test__cli.py
+-rw-r--r--   0        0        0    42127 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_gather.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_running_from_command_line.py
+-rw-r--r--   0        0        0     5135 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/tests/test_serialize.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/LICENSE
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/README.md
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/pyproject.toml
+-rw-r--r--   0        0        0     8708 2020-02-02 00:00:00.000000 typeshed_stats-24.5.21/PKG-INFO
```

### Comparing `typeshed_stats-23.2.1/.pre-commit-config.yaml` & `typeshed_stats-24.5.21/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,47 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0 # must match requirements/misc-lint.txt
+    rev: v4.5.0 # must match pyproject.toml
     hooks:
       - id: trailing-whitespace
-      - id: requirements-txt-fixer
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-toml
       - id: check-json
       - id: check-merge-conflict
-      - id: mixed-line-ending
       - id: check-case-conflict
       - id: name-tests-test
         args: [--pytest-test-first]
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.3.5 # must match pyproject.toml
     hooks:
-      - id: python-check-mock-methods
-  - repo: https://github.com/hadialqattan/pycln
-    rev: v2.1.2 # must match requirements/misc-lint.txt
-    hooks:
-      - id: pycln
-        args: [--config=pyproject.toml, .]
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1 # must match requirements/misc-lint.txt
-    hooks:
-      - id: pyupgrade
-        args: [--py310-plus]
-  - repo: https://github.com/psf/black
-    rev: 23.1.0 # must match requirements/misc-lint.txt AND the black used by blacken-docs
-    hooks:
-      - id: black
+      - id: ruff
+      - id: ruff-format
   - repo: https://github.com/adamchainz/blacken-docs
-    rev: v1.12.1 # must match requirements/misc-lint.txt
+    rev: 1.16.0 # must match pyproject.toml
     hooks:
       - id: blacken-docs
-        additional_dependencies: [black==23.1.0]
-  - repo: https://github.com/pycqa/isort
-    rev: 5.12.0 # must match requirements/misc-lint.txt
-    hooks:
-      - id: isort
+        additional_dependencies: [black==24.3.0]
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.6
     hooks:
       - id: codespell
   - repo: https://github.com/alan-turing-institute/CleverCSV-pre-commit
-    rev: v0.7.5
+    rev: v0.8.2
     hooks:
       - id: clevercsv-standardize
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.32.2
+    rev: v0.39.0
     hooks:
       - id: markdownlint-fix
         args: ["--ignore", "stats_website/.snippets"]
       - id: markdownlint
         args: ["--ignore", "stats_website/.snippets"]
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         exclude: "^examples/.*"
         exclude_types: ["markdown"]
   - repo: meta
     hooks:
       - id: check-hooks-apply
```

### Comparing `typeshed_stats-23.2.1/mkdocs.yml` & `typeshed_stats-24.5.21/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/website_macros.py` & `typeshed_stats-24.5.21/website_macros.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+# pyright: reportUnusedFunction=false
 """Macros and variables for the mkdocs-macros plugin."""
 
 import builtins
 import csv
 import datetime as dt
 import shutil
 import subprocess
 import types
+from abc import abstractmethod
 from collections.abc import Callable
 from enum import Enum
 from pathlib import Path
 from typing import Any, Protocol, TypeGuard, TypeVar, get_args, get_origin
 
 import attrs
 import markdown
@@ -22,14 +24,15 @@
 
 class Env(Protocol):
     """Protocol representing the `mkdocs_macros.MacrosPlugin` object."""
 
     variables: dict[str, Any]
     conf: dict[str, Any]
 
+    @abstractmethod
     def macro(self, /, func: CF) -> CF:
         """Register a function as a macro."""
 
 
 def define_env(env: Env) -> None:
     """Define environment variables."""
     # Variables needed for cli.md
@@ -65,28 +68,34 @@
             typ_name = typ.__name__
             if typ_name in typeshed_stats.gather.__all__:
                 return f"[`{typ_name}`][typeshed_stats.gather.{typ_name}]"
             if typ_name in dir(builtins):
                 return f"[`{typ_name}`][{typ_name}]"
             if typ is Path:
                 return "[`Path`][pathlib.Path]"
-            if typ is types.NoneType:  # noqa: E721
+            if typ is types.NoneType:
                 return "[`None`][None]"
             return f"`{typ_name}`"
         return f"`{typ}`"
 
     env.variables.update(gather=typeshed_stats.gather, attrs=attrs)
 
     # Variables needed for stats.md and stats-csv.md
     stats_as_csv: list[dict[str, str | int]] = []
     with Path("examples", "example.csv").open(newline="", encoding="utf-8") as csvfile:
         for line in csv.DictReader(csvfile):
-            stats_as_csv.append(
-                {key: int(val) if val.isdigit() else val for key, val in line.items()}
-            )
+            row: dict[str, str | int] = {}
+            for key, val in line.items():
+                if val.isdigit():
+                    row[key] = int(val)
+                elif key == "upstream_url":
+                    row[key] = "(unknown)" if val == "-" else f"[{val}]({val})"
+                else:
+                    row[key] = val
+            stats_as_csv.append(row)
 
     @env.macro
     def is_int(x: object) -> TypeGuard[int]:
         return isinstance(x, int)
 
     env.variables.update(
         last_update_time=dt.datetime.utcnow().strftime("%H:%M UTC on %Y-%m-%d"),
```

### Comparing `typeshed_stats-23.2.1/.github/workflows/check-requirements.yml` & `typeshed_stats-24.5.21/.github/workflows/check-requirements.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 name: Check requirements
 
 on:
   push:
     branches: main
     paths:
       - ".github/workflows/check-requirements.yml"
-      - "requirements/**.txt"
       - "pyproject.toml"
   pull_request:
     paths:
       - ".github/workflows/check-requirements.yml"
-      - "requirements/**.txt"
       - "pyproject.toml"
   workflow_dispatch:
   schedule:
     - cron: "0 0 * * *"
 
 permissions:
   contents: read
 
 env:
   FORCE_COLOR: 1 # Request colored output from CLI tools supporting it
-  PIP_DISABLE_PIP_VERSION_CHECK: 1
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
   check-requirements:
     name: Check requirements can all be installed together
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
+      - name: Install uv
+        run: curl -LsSf https://astral.sh/uv/install.sh | sh
       - name: Check requirements can all be installed together
-        run: pip install -e .[dev]
+        run: uv pip install -e '.[dev]' --system
 
   create-issue-on-failure:
     name: Create an issue if daily requirements check failed
     runs-on: ubuntu-latest
     needs: check-requirements
-    if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && github.event_name == 'schedule' && needs.check-requirements.result == 'failure' }}
+    if: >-
+      ${{
+        github.repository == 'AlexWaygood/typeshed-stats'
+        && always()
+        && github.event_name == 'schedule'
+        && needs.check-requirements.result == 'failure'
+      }}
     permissions:
       issues: write
     steps:
-      - uses: actions/github-script@v6
+      - uses: actions/github-script@v7
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           script: |
             await github.rest.issues.create({
               owner: "AlexWaygood",
               repo: "typeshed-stats",
               title: `Daily requirements check failed on ${new Date().toDateString()}`,
```

### Comparing `typeshed_stats-23.2.1/.github/workflows/lint.yml` & `typeshed_stats-24.5.21/.github/workflows/typecheck.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: lint
+name: Typecheck
 
 on:
   push:
     branches: main
     paths-ignore:
       - "**.json"
       - "**.md"
@@ -19,76 +19,70 @@
     - cron: "0 0 * * *"
 
 permissions:
   contents: read
 
 env:
   FORCE_COLOR: 1 # Request colored output from CLI tools supporting it
-  PIP_DISABLE_PIP_VERSION_CHECK: 1
   TERM: xterm-256color # needed for FORCE_COLOR to work on mypy on Ubuntu, see https://github.com/python/mypy/issues/13817
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
   mypy:
     name: Check code with mypy
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
-          cache: "pip"
-          cache-dependency-path: "requirements/mypy.txt"
-          python-version: "3.10"
-      - name: Install wheel
-        run: pip install "wheel<1"
-      - name: Install mypy requirements only
-        # Install the minimal requirements for a PR run, so that it's fast
-        if: ${{ github.event_name != 'schedule' }}
-        run: pip install -r requirements/mypy.txt
-      - name: Install all requirements for daily run
-        # Install all requirements for the daily run,
-        # so we detect if any of the dependencies has added a py.typed file recently
-        if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && github.event_name == 'schedule' }}
-        run: pip install -e .[dev]
-      - run: pip freeze --all
-      - name: Run mypy on the project
-        run: mypy
+          python-version: "3.11"
+      - uses: hynek/setup-cached-uv@v1
+      - run: uv pip install -e ".[typecheck]" --system
+      - run: uv pip freeze
+      - run: mypy
 
-  flake8:
-    name: Lint code with flake8
+  pyright:
+    name: Run pyright on the codebase
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
-          cache: "pip"
-          cache-dependency-path: "requirements/flake8.txt"
           python-version: "3.10"
-      - name: Install wheel
-        run: pip install "wheel<1"
-      - name: Install requirements
-        run: pip install -r requirements/flake8.txt
-      - run: pip freeze --all
-      - name: lint the project
-        run: flake8 --color always
+      - uses: hynek/setup-cached-uv@v1
+      - run: uv pip install -e ".[typecheck]" --system
+      - run: uv pip freeze
+      - name: Run pyright
+        uses: jakebailey/pyright-action@v2
+        with:
+          version: "1.1.331"
 
   create-issue-on-failure:
-    name: Create an issue if daily lint failed
+    name: Create an issue if daily typecheck failed
     runs-on: ubuntu-latest
-    needs: [mypy, flake8]
-    if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && github.event_name == 'schedule' && (needs.mypy.result == 'failure' || needs.flake8.result == 'failure') }}
+    needs: [mypy, pyright]
+    if: >-
+      ${{
+        github.repository == 'AlexWaygood/typeshed-stats'
+        && always()
+        && github.event_name == 'schedule'
+        && (
+          needs.mypy.result == 'failure'
+          || needs.pyright.result == 'failure'
+        )
+      }}
     permissions:
       issues: write
     steps:
-      - uses: actions/github-script@v6
+      - uses: actions/github-script@v7
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           script: |
             await github.rest.issues.create({
               owner: "AlexWaygood",
               repo: "typeshed-stats",
-              title: `Daily lint failed on ${new Date().toDateString()}`,
-              body: "Runs are listed here: https://github.com/AlexWaygood/typeshed-stats/actions/workflows/lint.yml",
+              title: `Daily typecheck failed on ${new Date().toDateString()}`,
+              body: "Runs are listed here: https://github.com/AlexWaygood/typeshed-stats/actions/workflows/typecheck.yml",
             })
```

### Comparing `typeshed_stats-23.2.1/.github/workflows/regen-examples-and-docs.yml` & `typeshed_stats-24.5.21/.github/workflows/regen-examples-and-docs.yml`

 * *Files 16% similar despite different names*

```diff
@@ -10,62 +10,74 @@
       - "tests/**"
       - "examples/**"
       - "**.json"
       - "**.csv"
       - "**.html"
   workflow_dispatch:
 
-env:
-  PIP_DISABLE_PIP_VERSION_CHECK: 1
-
 jobs:
   regen_examples_and_docs:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: git config
         run: |
           git config --global user.name statsabot
           git config --global user.email ''
-      - uses: actions/setup-python@v4
+      - uses: actions/setup-python@v5
         with:
-          cache: "pip"
-          cache-dependency-path: |
-            requirements/docs.txt
-            pyproject.toml
-          python-version: "3.10"
-      - run: pip install "wheel<1"
-      - run: pip install -e .[docs]
-      - run: pip freeze --all
+          python-version: "3.11"
+      - uses: hynek/setup-cached-uv@v1
+      - run: uv pip install -e .[docs] --system
+      - run: uv pip freeze
       - name: Regenerate examples and docs
         id: regen
         run: python scripts/regenerate.py --download-typeshed
       - name: Check the generated files with pre-commit
         id: lint
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
       - name: Commit and push the changes
         id: commit
-        if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && steps.regen.outcome == 'success' && steps.lint.outcome == 'success' }}
+        if: >-
+          ${{
+            github.repository == 'AlexWaygood/typeshed-stats'
+            && always()
+            && steps.regen.outcome == 'success'
+            && steps.lint.outcome == 'success'
+          }}
         run: |
           git add .
           git diff --staged --quiet || git commit -m "👷 Automated regeneration of examples and docs"
           git push
       - name: Deploy docs
-        if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && steps.regen.outcome == 'success' && steps.lint.outcome == 'success' && steps.commit.outcome == 'success' }}
+        if: >-
+          ${{
+            github.repository == 'AlexWaygood/typeshed-stats'
+            && always()
+            && steps.regen.outcome == 'success'
+            && steps.lint.outcome == 'success'
+            && steps.commit.outcome == 'success'
+          }}
         run: mkdocs gh-deploy -m "🚀 Deploying {sha} with MkDocs {version}" --force
 
   create-issue-on-failure:
     name: Create an issue if the automated regeneration failed
     runs-on: ubuntu-latest
     needs: [regen_examples_and_docs]
-    if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && needs.regen_examples_and_docs.result == 'failure' }}
+    if: >-
+      ${{
+        github.repository == 'AlexWaygood/typeshed-stats'
+        && always()
+        && github.event_name == 'schedule'
+        && needs.regen_examples_and_docs.result == 'failure'
+      }}
     permissions:
       issues: write
     steps:
-      - uses: actions/github-script@v6
+      - uses: actions/github-script@v7
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           script: |
             await github.rest.issues.create({
               owner: "AlexWaygood",
               repo: "typeshed-stats",
               title: `Automated regeneration of examples failed on ${new Date().toDateString()}`,
```

### Comparing `typeshed_stats-23.2.1/.github/workflows/test-website.yml` & `typeshed_stats-24.5.21/.github/workflows/test-website.yml`

 * *Files 20% similar despite different names*

```diff
@@ -6,40 +6,33 @@
     paths-ignore:
       - "tests/**"
       - "examples/**"
       - "**.json"
       - "**.csv"
       - "**.html"
 
-env:
-  PIP_DISABLE_PIP_VERSION_CHECK: 1
-
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
   test-website:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
-          cache: "pip"
-          cache-dependency-path: |
-            requirements/docs.txt
-            pyproject.toml
-          python-version: "3.10"
-      - run: pip install "wheel<1"
-      - run: pip install -e .[docs]
-      - run: pip freeze --all
+          python-version: "3.11"
+      - uses: hynek/setup-cached-uv@v1
+      - run: uv pip install -e .[docs] --system
+      - run: uv pip freeze
       - name: Regenerate examples and docs
         run: python scripts/regenerate.py --download-typeshed
       - name: Check the generated files with pre-commit
-        uses: pre-commit/action@v3.0.0
+        uses: pre-commit/action@v3.0.1
       - name: Build docs
         run: mkdocs build --strict
       - name: Upload docs
-        uses: actions/upload-artifact@v3
+        uses: actions/upload-artifact@v4
         with:
           name: doc-html
           path: site
```

### Comparing `typeshed_stats-23.2.1/.github/workflows/test.yml` & `typeshed_stats-24.5.21/.github/workflows/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -25,77 +25,66 @@
     - cron: "0 0 * * *"
 
 permissions:
   contents: read
 
 env:
   FORCE_COLOR: 1 # Request colored output from CLI tools supporting it
-  PIP_DISABLE_PIP_VERSION_CHECK: 1
   PY_COLORS: 1 # Recognized by the `py` package, dependency of `pytest`
-  TERM: xterm-256color # needed for FORCE_COLOR to work on mypy on Ubuntu, see https://github.com/python/mypy/issues/13817
+  # TERM is needed for FORCE_COLOR to work on mypy on Ubuntu,
+  # see https://github.com/python/mypy/issues/13817
+  TERM: xterm-256color
   GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-  COVERALLS_PARALLEL: true
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.head_ref || github.run_id }}
   cancel-in-progress: true
 
 jobs:
   pytest-tests:
     name: Run tests with pytest
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: ["ubuntu-latest", "windows-latest", "macos-latest"]
-        python-version: ["3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12", "3.13"]
       fail-fast: false
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }} on ${{ matrix.os }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
-          cache: "pip"
-          cache-dependency-path: |
-            requirements/pytest.txt
-            pyproject.toml
           python-version: ${{ matrix.python-version }}
-      - run: pip install "wheel<1"
-      - run: pip install "coveralls==3.3.*" -e .[pytest]
-      - run: pip freeze --all
+          allow-prereleases: true
+      - uses: hynek/setup-cached-uv@v1
+      - name: Install dependencies
+        run: uv pip install -e ".[pytest]" --system
+      - run: uv pip freeze
       - name: Run tests under coverage
+        shell: bash
         run: |
           coverage run -m pytest --doctest-modules
           coverage report --no-skip-covered
-      - name: Upload coverage to coveralls
-        if: github.repository == 'AlexWaygood/typeshed-stats'
-        env:
-          COVERALLS_FLAG_NAME: ${{ matrix.os }}-${{ matrix.python-version }}
-        run: coveralls --service=github
-
-  coveralls-finish:
-    name: Indicate completion to coveralls.io
-    needs: pytest-tests
-    if: github.repository == 'AlexWaygood/typeshed-stats'
-    runs-on: ubuntu-latest
-    container: python:3-slim
-    steps:
-      - run: |
-          pip install "coveralls==3.3.*"
-          coveralls --service=github --finish
 
   create-issue-on-failure:
     name: Create an issue if daily test failed
     runs-on: ubuntu-latest
     needs: pytest-tests
-    if: ${{ github.repository == 'AlexWaygood/typeshed-stats' && always() && github.event_name == 'schedule' && needs.pytest-tests.result == 'failure' }}
+    if: >-
+      ${{
+        github.repository == 'AlexWaygood/typeshed-stats'
+        && always()
+        && github.event_name == 'schedule'
+        && needs.pytest-tests.result == 'failure'
+      }}
     permissions:
       issues: write
     steps:
-      - uses: actions/github-script@v6
+      - uses: actions/github-script@v7
         with:
           github-token: ${{ secrets.GITHUB_TOKEN }}
           script: |
             await github.rest.issues.create({
               owner: "AlexWaygood",
               repo: "typeshed-stats",
               title: `Daily test failed on ${new Date().toDateString()}`,
```

### Comparing `typeshed_stats-23.2.1/examples/example.md` & `typeshed_stats-24.5.21/examples/example.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,120 +1,20 @@
-## Info on typeshed's stubs for `D3DShot`
-
-### Stub distribution name
-
-`types-D3DShot`
-
-### Number of lines
-
-585 (excluding blank lines)
-
-### Package status: *up to date*
-
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *skipped*
-
-Stubtest is skipped in typeshed's CI for this package.
-
-Typeshed currently has 0 allowlist entries for `D3DShot` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `D3DShot`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 127
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 255
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 100
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 43
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
-
----
-
-## Info on typeshed's stubs for `DateTimeRange`
-
-### Stub distribution name
-
-`types-DateTimeRange`
-
-### Number of lines
-
-64 (excluding blank lines)
-
-### Package status: *obsolete*
-
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *error on missing stub*
-
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 0 allowlist entries for `DateTimeRange` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `DateTimeRange`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 30
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 28
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 10
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 1
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
+## Info on typeshed's stubs for `Deprecated`
 
----
+### Upstream repo URL
 
-## Info on typeshed's stubs for `Deprecated`
+[https://github.com/tantale/deprecated](https://github.com/tantale/deprecated)
 
 ### Stub distribution name
 
 `types-Deprecated`
 
 ### Number of lines
 
-56 (excluding blank lines)
+55 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -153,21 +53,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `ExifRead`
 
+### Upstream repo URL
+
+[https://github.com/ianare/exif-py](https://github.com/ianare/exif-py)
+
 ### Stub distribution name
 
 `types-ExifRead`
 
 ### Number of lines
 
-218 (excluding blank lines)
+217 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -175,15 +79,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `ExifRead` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `ExifRead` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `ExifRead`
 
@@ -206,21 +110,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Flask-Cors`
 
+### Upstream repo URL
+
+[https://github.com/corydolphin/flask-cors](https://github.com/corydolphin/flask-cors)
+
 ### Stub distribution name
 
 `types-Flask-Cors`
 
 ### Number of lines
 
-124 (excluding blank lines)
+126 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -237,20 +145,20 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `Flask-Cors`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 62
+    - Annotated parameters: 63
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 7
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 23
+    - Annotated returns: 24
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 30
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
@@ -259,141 +167,153 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Flask-Migrate`
 
+### Upstream repo URL
+
+[https://github.com/miguelgrinberg/Flask-Migrate](https://github.com/miguelgrinberg/Flask-Migrate)
+
 ### Stub distribution name
 
 `types-Flask-Migrate`
 
 ### Number of lines
 
-100 (excluding blank lines)
+130 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `Flask-Migrate` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `Flask-Migrate` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `Flask-Migrate`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 74
-    - Unannotated parameters: 4
+    - Annotated parameters: 86
+    - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 20
-    - Unannotated returns: 2
+    - Annotated returns: 24
+    - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 7
-    - Explicit `Any` variables: 1
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 2
+    - Total class definitions: 3
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `Flask-SQLAlchemy`
+## Info on typeshed's stubs for `Flask-SocketIO`
+
+### Upstream repo URL
+
+[https://github.com/miguelgrinberg/flask-socketio](https://github.com/miguelgrinberg/flask-socketio)
 
 ### Stub distribution name
 
-`types-Flask-SQLAlchemy`
+`types-Flask-SocketIO`
 
 ### Number of lines
 
-106 (excluding blank lines)
+233 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `Flask-SQLAlchemy` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `Flask-SocketIO` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `Flask-SQLAlchemy`
+### Statistics on the annotations in typeshed's stubs for `Flask-SocketIO`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 54
-    - Unannotated parameters: 21
+    - Annotated parameters: 138
+    - Unannotated parameters: 36
     - Explicit `Any` parameters: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 23
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 17
 - Returns:
-    - Annotated returns: 24
-    - Unannotated returns: 19
-    - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 37
+    - Unannotated returns: 15
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
 - Variables:
-    - Annotated variables: 16
-    - Explicit `Any` variables: 9
+    - Annotated variables: 3
+    - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 9
+    - Total class definitions: 8
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `JACK-Client`
 
+### Upstream repo URL
+
+[https://github.com/spatialaudio/jackclient-python](https://github.com/spatialaudio/jackclient-python)
+
 ### Stub distribution name
 
 `types-JACK-Client`
 
 ### Number of lines
 
-309 (excluding blank lines)
+311 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `darwin` and `linux`.
+In CI, stubtest is run on `linux` only.
 
 Typeshed currently has 0 allowlist entries for `JACK-Client` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
@@ -401,15 +321,15 @@
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 107
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 151
+    - Annotated returns: 152
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 46
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
@@ -418,21 +338,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Markdown`
 
+### Upstream repo URL
+
+[https://github.com/Python-Markdown/markdown](https://github.com/Python-Markdown/markdown)
+
 ### Stub distribution name
 
 `types-Markdown`
 
 ### Number of lines
 
-641 (excluding blank lines)
+695 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -440,105 +364,113 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 12 allowlist entries for `Markdown` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `Markdown` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `Markdown`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 115
-    - Unannotated parameters: 143
-    - Explicit `Any` parameters: 12
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 5
+    - Annotated parameters: 256
+    - Unannotated parameters: 30
+    - Explicit `Any` parameters: 15
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 114
-    - Unannotated returns: 64
-    - Explicit `Any` returns: 5
+    - Annotated returns: 198
+    - Unannotated returns: 2
+    - Explicit `Any` returns: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 215
-    - Explicit `Any` variables: 83
+    - Annotated variables: 217
+    - Explicit `Any` variables: 15
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 99
+    - Total class definitions: 102
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Pillow`
 
+### Upstream repo URL
+
+[https://github.com/python-pillow/Pillow](https://github.com/python-pillow/Pillow)
+
 ### Stub distribution name
 
 `types-Pillow`
 
 ### Number of lines
 
-2,537 (excluding blank lines)
+3,266 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *obsolete*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+The runtime package has added inline type hints; these typeshed stubs are now obsolete.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 1 allowlist entry for `Pillow` when running stubtest in CI.
+Typeshed currently has 18 unique allowlist entries for `Pillow` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `Pillow`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 653
-    - Unannotated parameters: 613
-    - Explicit `Any` parameters: 5
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 60
+    - Annotated parameters: 777
+    - Unannotated parameters: 584
+    - Explicit `Any` parameters: 7
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 55
 - Returns:
-    - Annotated returns: 466
-    - Unannotated returns: 340
-    - Explicit `Any` returns: 4
+    - Annotated returns: 588
+    - Unannotated returns: 319
+    - Explicit `Any` returns: 5
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 847
-    - Explicit `Any` variables: 323
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 8
+    - Annotated variables: 766
+    - Explicit `Any` variables: 5
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 305
 - Class definitions:
-    - Total class definitions: 204
-    - Class definitions with `Any`: 4
-    - Class definitions marked as at least partially `Incomplete`: 0
+    - Total class definitions: 226
+    - Class definitions with `Any`: 3
+    - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
 ## Info on typeshed's stubs for `PyAutoGUI`
 
+### Upstream repo URL
+
+[https://github.com/asweigart/pyautogui](https://github.com/asweigart/pyautogui)
+
 ### Stub distribution name
 
 `types-PyAutoGUI`
 
 ### Number of lines
 
-229 (excluding blank lines)
+234 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -546,15 +478,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `PyAutoGUI` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `PyAutoGUI` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `PyAutoGUI`
 
@@ -577,21 +509,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `PyMySQL`
 
+### Upstream repo URL
+
+[https://github.com/PyMySQL/PyMySQL](https://github.com/PyMySQL/PyMySQL)
+
 ### Stub distribution name
 
 `types-PyMySQL`
 
 ### Number of lines
 
-1,041 (excluding blank lines)
+1,045 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -599,105 +535,113 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 11 allowlist entries for `PyMySQL` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `PyMySQL` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `PyMySQL`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 139
-    - Unannotated parameters: 53
+    - Annotated parameters: 142
+    - Unannotated parameters: 52
     - Explicit `Any` parameters: 10
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 28
 - Returns:
-    - Annotated returns: 98
-    - Unannotated returns: 40
+    - Annotated returns: 101
+    - Unannotated returns: 37
     - Explicit `Any` returns: 18
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 733
-    - Explicit `Any` variables: 62
+    - Annotated variables: 734
+    - Explicit `Any` variables: 60
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 24
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `PyScreeze`
 
+### Upstream repo URL
+
+[https://github.com/asweigart/pyscreeze](https://github.com/asweigart/pyscreeze)
+
 ### Stub distribution name
 
 `types-PyScreeze`
 
 ### Number of lines
 
-183 (excluding blank lines)
+193 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 1 allowlist entry for `PyScreeze` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `PyScreeze` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `PyScreeze`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 93
+    - Annotated parameters: 102
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 18
+    - Annotated returns: 21
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 14
+    - Annotated variables: 17
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 5
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `PyYAML`
 
+### Upstream repo URL
+
+[https://github.com/yaml/pyyaml](https://github.com/yaml/pyyaml)
+
 ### Stub distribution name
 
 `types-PyYAML`
 
 ### Number of lines
 
-1,177 (excluding blank lines)
+1,298 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -705,52 +649,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `PyYAML` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `PyYAML` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `PyYAML`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 395
-    - Unannotated parameters: 315
-    - Explicit `Any` parameters: 40
+    - Annotated parameters: 516
+    - Unannotated parameters: 282
+    - Explicit `Any` parameters: 44
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 12
 - Returns:
-    - Annotated returns: 158
-    - Unannotated returns: 230
+    - Annotated returns: 222
+    - Unannotated returns: 172
     - Explicit `Any` returns: 12
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 220
-    - Explicit `Any` variables: 189
+    - Explicit `Any` variables: 160
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
     - Total class definitions: 91
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Pygments`
 
+### Upstream repo URL
+
+[https://github.com/pygments/pygments](https://github.com/pygments/pygments)
+
 ### Stub distribution name
 
 `types-Pygments`
 
 ### Number of lines
 
-687 (excluding blank lines)
+845 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -758,125 +706,127 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 4 allowlist entries for `Pygments` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `Pygments` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `Pygments`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 108
-    - Unannotated parameters: 157
+    - Annotated parameters: 116
+    - Unannotated parameters: 156
     - Explicit `Any` parameters: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 17
 - Returns:
-    - Annotated returns: 96
-    - Unannotated returns: 79
+    - Annotated returns: 108
+    - Unannotated returns: 75
     - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 5
 - Variables:
-    - Annotated variables: 313
-    - Explicit `Any` variables: 193
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 376
+    - Explicit `Any` variables: 169
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 24
 - Class definitions:
-    - Total class definitions: 62
-    - Class definitions with `Any`: 1
-    - Class definitions marked as at least partially `Incomplete`: 0
+    - Total class definitions: 94
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
-## Info on typeshed's stubs for `SQLAlchemy`
+## Info on typeshed's stubs for `RPi.GPIO`
 
-### Extra description
+### Upstream repo URL
 
-The `sqlalchemy-stubs` package is an alternative to this package and also includes a mypy plugin for more precise types.
+[https://sourceforge.net/p/raspberry-gpio-python/code/](https://sourceforge.net/p/raspberry-gpio-python/code/)
 
 ### Stub distribution name
 
-`types-SQLAlchemy`
+`types-RPi.GPIO`
 
 ### Number of lines
 
-14,666 (excluding blank lines)
+56 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
-
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+### Stubtest settings in CI: *skipped*
 
-In CI, stubtest is run on `linux` only.
+Stubtest is skipped in typeshed's CI for this package.
 
-Typeshed currently has 1,153 allowlist entries for `SQLAlchemy` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `RPi.GPIO` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `SQLAlchemy`
+### Statistics on the annotations in typeshed's stubs for `RPi.GPIO`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 2,117
-    - Unannotated parameters: 7,007
-    - Explicit `Any` parameters: 67
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1,141
+    - Annotated parameters: 28
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 2,115
-    - Unannotated returns: 3,317
-    - Explicit `Any` returns: 23
+    - Annotated returns: 18
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 3,089
-    - Explicit `Any` variables: 1,859
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 197
+    - Annotated variables: 26
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1,329
-    - Class definitions with `Any`: 62
-    - Class definitions marked as at least partially `Incomplete`: 2
+    - Total class definitions: 2
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `Send2Trash`
 
+### Upstream repo URL
+
+[https://github.com/arsenetar/send2trash](https://github.com/arsenetar/send2trash)
+
 ### Stub distribution name
 
 `types-Send2Trash`
 
 ### Number of lines
 
-21 (excluding blank lines)
+15 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `Send2Trash` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `Send2Trash` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `Send2Trash`
 
@@ -885,88 +835,96 @@
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 4
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 2
-    - Explicit `Any` variables: 1
+    - Annotated variables: 0
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `aiofiles`
+## Info on typeshed's stubs for `WTForms`
+
+### Upstream repo URL
+
+[https://github.com/wtforms/wtforms](https://github.com/wtforms/wtforms)
 
 ### Stub distribution name
 
-`types-aiofiles`
+`types-WTForms`
 
 ### Number of lines
 
-590 (excluding blank lines)
+1,069 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` and `win32`.
+In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 57 allowlist entries for `aiofiles` when running stubtest in CI.
+Typeshed currently has 21 unique allowlist entries for `WTForms` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `aiofiles`
+### Statistics on the annotations in typeshed's stubs for `WTForms`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 342
+    - Annotated parameters: 531
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 24
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 26
+    - Explicit `Any` parameters: 71
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 136
+    - Annotated returns: 185
     - Unannotated returns: 0
-    - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
+    - Explicit `Any` returns: 15
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 0
-    - Explicit `Any` variables: 0
+    - Annotated variables: 139
+    - Explicit `Any` variables: 28
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 10
+    - Total class definitions: 100
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `annoy`
+## Info on typeshed's stubs for `WebOb`
+
+### Upstream repo URL
+
+[https://github.com/Pylons/webob](https://github.com/Pylons/webob)
 
 ### Stub distribution name
 
-`types-annoy`
+`types-WebOb`
 
 ### Number of lines
 
-45 (excluding blank lines)
+1,796 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -974,264 +932,284 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `annoy` when running stubtest in CI.
+Typeshed currently has 100 unique allowlist entries for `WebOb` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `annoy`
+### Statistics on the annotations in typeshed's stubs for `WebOb`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 40
+    - Annotated parameters: 808
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
+    - Explicit `Any` parameters: 91
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 20
+    - Annotated returns: 606
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Explicit `Any` returns: 13
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 1
-    - Explicit `Any` variables: 0
+    - Annotated variables: 246
+    - Explicit `Any` variables: 15
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 149
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `appdirs`
+## Info on typeshed's stubs for `aiofiles`
+
+### Upstream repo URL
+
+[https://github.com/Tinche/aiofiles](https://github.com/Tinche/aiofiles)
 
 ### Stub distribution name
 
-`types-appdirs`
+`types-aiofiles`
 
 ### Number of lines
 
-54 (excluding blank lines)
+681 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 0 allowlist entries for `appdirs` when running stubtest in CI.
+Typeshed currently has 90 unique allowlist entries for `aiofiles` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *strict on some files*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
-### Statistics on the annotations in typeshed's stubs for `appdirs`
+### Statistics on the annotations in typeshed's stubs for `aiofiles`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 33
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+    - Annotated parameters: 390
+    - Unannotated parameters: 1
+    - Explicit `Any` parameters: 34
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 25
 - Returns:
-    - Annotated returns: 15
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 151
+    - Unannotated returns: 3
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 3
 - Variables:
-    - Annotated variables: 8
+    - Annotated variables: 6
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 16
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `aws-xray-sdk`
+## Info on typeshed's stubs for `antlr4-python3-runtime`
+
+### Upstream repo URL
+
+[https://github.com/antlr/antlr4](https://github.com/antlr/antlr4)
 
 ### Stub distribution name
 
-`types-aws-xray-sdk`
+`types-antlr4-python3-runtime`
 
 ### Number of lines
 
-711 (excluding blank lines)
+1,781 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 4 allowlist entries for `aws-xray-sdk` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `antlr4-python3-runtime` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `aws-xray-sdk`
+### Statistics on the annotations in typeshed's stubs for `antlr4-python3-runtime`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 127
-    - Unannotated parameters: 166
-    - Explicit `Any` parameters: 12
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 21
+    - Annotated parameters: 777
+    - Unannotated parameters: 222
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 27
 - Returns:
-    - Annotated returns: 180
-    - Unannotated returns: 94
-    - Explicit `Any` returns: 3
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 208
+    - Unannotated returns: 485
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 141
-    - Explicit `Any` variables: 46
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 395
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 269
 - Class definitions:
-    - Total class definitions: 45
+    - Total class definitions: 142
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `babel`
+## Info on typeshed's stubs for `assertpy`
+
+### Upstream repo URL
+
+[https://github.com/assertpy/assertpy](https://github.com/assertpy/assertpy)
 
 ### Stub distribution name
 
-`types-babel`
+`types-assertpy`
 
 ### Number of lines
 
-1,134 (excluding blank lines)
+208 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `babel` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `assertpy` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `babel`
+### Statistics on the annotations in typeshed's stubs for `assertpy`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 497
-    - Unannotated parameters: 136
-    - Explicit `Any` parameters: 19
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 15
+    - Annotated parameters: 84
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 29
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 300
-    - Unannotated returns: 79
-    - Explicit `Any` returns: 5
+    - Annotated returns: 87
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 257
-    - Explicit `Any` variables: 100
+    - Annotated variables: 21
+    - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 45
-    - Class definitions with `Any`: 1
+    - Total class definitions: 15
+    - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `backports.ssl_match_hostname`
+## Info on typeshed's stubs for `aws-xray-sdk`
+
+### Upstream repo URL
+
+[https://github.com/aws/aws-xray-sdk-python](https://github.com/aws/aws-xray-sdk-python)
 
 ### Stub distribution name
 
-`types-backports.ssl_match_hostname`
+`types-aws-xray-sdk`
 
 ### Number of lines
 
-6 (excluding blank lines)
+675 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *error on missing stub*
+### Stubtest settings in CI: *missing stubs ignored*
 
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `backports.ssl_match_hostname` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `aws-xray-sdk` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `backports.ssl_match_hostname`
+### Statistics on the annotations in typeshed's stubs for `aws-xray-sdk`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 3
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+    - Annotated parameters: 139
+    - Unannotated parameters: 154
+    - Explicit `Any` parameters: 12
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 21
 - Returns:
-    - Annotated returns: 2
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Annotated returns: 182
+    - Unannotated returns: 92
+    - Explicit `Any` returns: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 0
-    - Explicit `Any` variables: 0
+    - Annotated variables: 136
+    - Explicit `Any` variables: 46
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 45
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `beautifulsoup4`
 
+### Upstream repo URL
+
+[https://git.launchpad.net/beautifulsoup/tree](https://git.launchpad.net/beautifulsoup/tree)
+
 ### Stub distribution name
 
 `types-beautifulsoup4`
 
 ### Number of lines
 
-795 (excluding blank lines)
+822 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1248,96 +1226,161 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `beautifulsoup4`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 239
+    - Annotated parameters: 245
     - Unannotated parameters: 137
     - Explicit `Any` parameters: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 31
 - Returns:
     - Annotated returns: 192
     - Unannotated returns: 49
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 177
-    - Explicit `Any` variables: 69
+    - Explicit `Any` variables: 70
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
     - Total class definitions: 47
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `bleach`
 
+### Upstream repo URL
+
+[https://github.com/mozilla/bleach](https://github.com/mozilla/bleach)
+
 ### Stub distribution name
 
 `types-bleach`
 
 ### Number of lines
 
-187 (excluding blank lines)
+239 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `bleach` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `bleach` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict on some files*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for `bleach`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 64
-    - Unannotated parameters: 21
-    - Explicit `Any` parameters: 0
+    - Annotated parameters: 91
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 26
-    - Unannotated returns: 16
+    - Annotated returns: 49
+    - Unannotated returns: 1
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
 - Variables:
-    - Annotated variables: 45
-    - Explicit `Any` variables: 0
+    - Annotated variables: 60
+    - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 13
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `boltons`
+
+### Upstream repo URL
+
+[https://github.com/mahmoud/boltons](https://github.com/mahmoud/boltons)
+
+### Stub distribution name
+
+`types-boltons`
+
+### Number of lines
+
+1,212 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 5 unique allowlist entries for `boltons` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `boltons`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 634
+    - Unannotated parameters: 263
+    - Explicit `Any` parameters: 61
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 72
+- Returns:
+    - Annotated returns: 456
+    - Unannotated returns: 172
+    - Explicit `Any` returns: 34
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 8
+- Variables:
+    - Annotated variables: 234
+    - Explicit `Any` variables: 7
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 69
+- Class definitions:
+    - Total class definitions: 81
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 3
+
+---
+
 ## Info on typeshed's stubs for `boto`
 
+### Upstream repo URL
+
+[https://github.com/boto/boto](https://github.com/boto/boto)
+
 ### Stub distribution name
 
 `types-boto`
 
 ### Number of lines
 
-1,891 (excluding blank lines)
+1,916 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1345,15 +1388,15 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 9 allowlist entries for `boto` when running stubtest in CI.
+Typeshed currently has 9 unique allowlist entries for `boto` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `boto`
 
@@ -1376,67 +1419,75 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `braintree`
 
+### Upstream repo URL
+
+[https://github.com/braintree/braintree_python](https://github.com/braintree/braintree_python)
+
 ### Stub distribution name
 
 `types-braintree`
 
 ### Number of lines
 
-2,859 (excluding blank lines)
+2,932 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `braintree` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `braintree` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `braintree`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 80
-    - Unannotated parameters: 394
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 75
+    - Annotated parameters: 91
+    - Unannotated parameters: 429
+    - Explicit `Any` parameters: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 80
 - Returns:
-    - Annotated returns: 113
-    - Unannotated returns: 304
-    - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 142
+    - Unannotated returns: 324
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 1,301
-    - Explicit `Any` variables: 432
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 1,504
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 131
 - Class definitions:
-    - Total class definitions: 234
+    - Total class definitions: 267
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `cachetools`
 
+### Upstream repo URL
+
+[https://github.com/tkem/cachetools](https://github.com/tkem/cachetools)
+
 ### Stub distribution name
 
 `types-cachetools`
 
 ### Number of lines
 
 119 (excluding blank lines)
@@ -1451,15 +1502,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 20 allowlist entries for `cachetools` when running stubtest in CI.
+Typeshed currently has 20 unique allowlist entries for `cachetools` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `cachetools`
 
@@ -1482,74 +1533,139 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `caldav`
 
+### Upstream repo URL
+
+[https://github.com/python-caldav/caldav](https://github.com/python-caldav/caldav)
+
 ### Stub distribution name
 
 `types-caldav`
 
 ### Number of lines
 
-499 (excluding blank lines)
+526 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 9 allowlist entries for `caldav` when running stubtest in CI.
+Typeshed currently has 9 unique allowlist entries for `caldav` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `caldav`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 205
-    - Unannotated parameters: 30
-    - Explicit `Any` parameters: 9
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 17
+    - Annotated parameters: 214
+    - Unannotated parameters: 35
+    - Explicit `Any` parameters: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 21
 - Returns:
-    - Annotated returns: 116
+    - Annotated returns: 117
     - Unannotated returns: 8
-    - Explicit `Any` returns: 5
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 5
+- Variables:
+    - Annotated variables: 94
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 6
+- Class definitions:
+    - Total class definitions: 86
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `capturer`
+
+### Upstream repo URL
+
+[https://github.com/xolox/python-capturer](https://github.com/xolox/python-capturer)
+
+### Stub distribution name
+
+`types-capturer`
+
+### Number of lines
+
+114 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 1 unique allowlist entry for `capturer` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `capturer`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 50
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 42
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 92
+    - Annotated variables: 38
     - Explicit `Any` variables: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 86
+    - Total class definitions: 6
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `cffi`
 
+### Upstream repo URL
+
+[https://foss.heptapod.net/pypy/cffi](https://foss.heptapod.net/pypy/cffi)
+
 ### Stub distribution name
 
 `types-cffi`
 
 ### Number of lines
 
-820 (excluding blank lines)
+827 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1557,101 +1673,109 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 5 allowlist entries for `cffi` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `cffi` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `cffi`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 295
-    - Unannotated parameters: 251
+    - Annotated parameters: 302
+    - Unannotated parameters: 246
     - Explicit `Any` parameters: 32
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 21
 - Returns:
-    - Annotated returns: 191
-    - Unannotated returns: 132
+    - Annotated returns: 194
+    - Unannotated returns: 130
     - Explicit `Any` returns: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
     - Annotated variables: 252
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 115
 - Class definitions:
     - Total class definitions: 52
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `chardet`
+## Info on typeshed's stubs for `chevron`
+
+### Upstream repo URL
+
+[https://github.com/noahmorrison/chevron](https://github.com/noahmorrison/chevron)
 
 ### Stub distribution name
 
-`types-chardet`
+`types-chevron`
 
 ### Number of lines
 
-122 (excluding blank lines)
+38 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 25 allowlist entries for `chardet` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `chevron` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `chardet`
+### Statistics on the annotations in typeshed's stubs for `chevron`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 5
+    - Annotated parameters: 29
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
+    - Explicit `Any` parameters: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 7
+    - Annotated returns: 9
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 86
+    - Annotated variables: 3
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 10
+    - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `chevron`
+## Info on typeshed's stubs for `click-default-group`
+
+### Upstream repo URL
+
+[https://github.com/click-contrib/click-default-group](https://github.com/click-contrib/click-default-group)
 
 ### Stub distribution name
 
-`types-chevron`
+`types-click-default-group`
 
 ### Number of lines
 
 37 (excluding blank lines)
 
 ### Package status: *up to date*
 
@@ -1663,45 +1787,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `chevron` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `click-default-group` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `chevron`
+### Statistics on the annotations in typeshed's stubs for `click-default-group`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 29
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 2
+    - Annotated parameters: 16
+    - Unannotated parameters: 4
+    - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 9
+    - Annotated returns: 10
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
 - Variables:
-    - Annotated variables: 3
+    - Annotated variables: 7
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 2
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `click-spinner`
 
+### Upstream repo URL
+
+[https://github.com/click-contrib/click-spinner](https://github.com/click-contrib/click-spinner)
+
 ### Stub distribution name
 
 `types-click-spinner`
 
 ### Number of lines
 
 30 (excluding blank lines)
@@ -1747,21 +1875,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `colorama`
 
+### Upstream repo URL
+
+[https://github.com/tartley/colorama](https://github.com/tartley/colorama)
+
 ### Stub distribution name
 
 `types-colorama`
 
 ### Number of lines
 
-198 (excluding blank lines)
+201 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1769,15 +1901,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 45 allowlist entries for `colorama` when running stubtest in CI.
+Typeshed currently has 44 unique allowlist entries for `colorama` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `colorama`
 
@@ -1800,14 +1932,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `commonmark`
 
+### Upstream repo URL
+
+[https://github.com/rtfd/commonmark.py](https://github.com/rtfd/commonmark.py)
+
 ### Stub distribution name
 
 `types-commonmark`
 
 ### Number of lines
 
 370 (excluding blank lines)
@@ -1853,21 +1989,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `console-menu`
 
+### Upstream repo URL
+
+[https://github.com/aegirhall/console-menu](https://github.com/aegirhall/console-menu)
+
 ### Stub distribution name
 
 `types-console-menu`
 
 ### Number of lines
 
-687 (excluding blank lines)
+711 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1884,96 +2024,47 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `console-menu`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 210
+    - Annotated parameters: 217
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 278
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 57
+    - Annotated variables: 58
     - Explicit `Any` variables: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
     - Total class definitions: 39
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `contextvars`
-
-### Stub distribution name
-
-`types-contextvars`
-
-### Number of lines
-
-41 (excluding blank lines)
-
-### Package status: *up to date*
-
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *error on missing stub*
-
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 4 allowlist entries for `contextvars` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `contextvars`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 12
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 17
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 1
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 3
-    - Class definitions with `Any`: 1
-    - Class definitions marked as at least partially `Incomplete`: 0
+## Info on typeshed's stubs for `croniter`
 
----
+### Upstream repo URL
 
-## Info on typeshed's stubs for `croniter`
+[https://github.com/kiorky/croniter](https://github.com/kiorky/croniter)
 
 ### Stub distribution name
 
 `types-croniter`
 
 ### Number of lines
 
-136 (excluding blank lines)
+151 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -1990,43 +2081,47 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `croniter`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 63
+    - Annotated parameters: 69
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 23
+    - Annotated returns: 24
     - Unannotated returns: 0
-    - Explicit `Any` returns: 9
+    - Explicit `Any` returns: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 21
-    - Explicit `Any` variables: 3
+    - Annotated variables: 29
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 8
     - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `dateparser`
 
+### Upstream repo URL
+
+[https://github.com/scrapinghub/dateparser](https://github.com/scrapinghub/dateparser)
+
 ### Stub distribution name
 
 `types-dateparser`
 
 ### Number of lines
 
-468 (excluding blank lines)
+473 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2034,45 +2129,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 6 allowlist entries for `dateparser` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `dateparser` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `dateparser`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 126
-    - Unannotated parameters: 127
+    - Unannotated parameters: 130
     - Explicit `Any` parameters: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 21
 - Returns:
-    - Annotated returns: 75
-    - Unannotated returns: 67
+    - Annotated returns: 74
+    - Unannotated returns: 69
     - Explicit `Any` returns: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 135
     - Explicit `Any` variables: 76
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 34
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `decorator`
 
+### Upstream repo URL
+
+[https://github.com/micheles/decorator](https://github.com/micheles/decorator)
+
 ### Stub distribution name
 
 `types-decorator`
 
 ### Number of lines
 
 66 (excluding blank lines)
@@ -2087,15 +2186,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 9 allowlist entries for `decorator` when running stubtest in CI.
+Typeshed currently has 10 unique allowlist entries for `decorator` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `decorator`
 
@@ -2116,76 +2215,141 @@
 - Class definitions:
     - Total class definitions: 2
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `dj-database-url`
+## Info on typeshed's stubs for `defusedxml`
+
+### Upstream repo URL
+
+[https://github.com/tiran/defusedxml](https://github.com/tiran/defusedxml)
 
 ### Stub distribution name
 
-`types-dj-database-url`
+`types-defusedxml`
 
 ### Number of lines
 
-37 (excluding blank lines)
+234 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *error on missing stub*
+### Stubtest settings in CI: *missing stubs ignored*
 
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `dj-database-url` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `defusedxml` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `dj-database-url`
+### Statistics on the annotations in typeshed's stubs for `defusedxml`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 13
-    - Unannotated parameters: 0
+    - Annotated parameters: 81
+    - Unannotated parameters: 97
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 13
 - Returns:
-    - Annotated returns: 2
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Annotated returns: 38
+    - Unannotated returns: 13
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 15
-    - Explicit `Any` variables: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 37
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 19
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 12
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `docker`
+
+### Upstream repo URL
+
+[https://github.com/docker/docker-py](https://github.com/docker/docker-py)
+
+### Stub distribution name
+
+`types-docker`
+
+### Number of lines
+
+1,886 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 7 unique allowlist entries for `docker` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `docker`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 775
+    - Unannotated parameters: 379
+    - Explicit `Any` parameters: 19
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 315
+- Returns:
+    - Annotated returns: 290
+    - Unannotated returns: 270
+    - Explicit `Any` returns: 25
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
+- Variables:
+    - Annotated variables: 206
+    - Explicit `Any` variables: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 83
+- Class definitions:
+    - Total class definitions: 127
+    - Class definitions with `Any`: 2
+    - Class definitions marked as at least partially `Incomplete`: 24
+
+---
+
 ## Info on typeshed's stubs for `dockerfile-parse`
 
+### Upstream repo URL
+
+[https://github.com/containerbuildsystem/dockerfile-parse](https://github.com/containerbuildsystem/dockerfile-parse)
+
 ### Stub distribution name
 
 `types-dockerfile-parse`
 
 ### Number of lines
 
-111 (excluding blank lines)
+113 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2224,21 +2388,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `docopt`
 
+### Upstream repo URL
+
+[https://github.com/docopt/docopt](https://github.com/docopt/docopt)
+
 ### Stub distribution name
 
 `types-docopt`
 
 ### Number of lines
 
-10 (excluding blank lines)
+14 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2255,43 +2423,47 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `docopt`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 6
+    - Annotated parameters: 7
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
-    - Annotated returns: 2
+    - Annotated returns: 3
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 1
+    - Annotated variables: 2
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 0
+    - Total class definitions: 2
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `docutils`
 
+### Upstream repo URL
+
+[https://sourceforge.net/p/docutils/code](https://sourceforge.net/p/docutils/code)
+
 ### Stub distribution name
 
 `types-docutils`
 
 ### Number of lines
 
-502 (excluding blank lines)
+1,493 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2299,52 +2471,56 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 19 allowlist entries for `docutils` when running stubtest in CI.
+Typeshed currently has 18 unique allowlist entries for `docutils` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `docutils`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 213
-    - Unannotated parameters: 60
-    - Explicit `Any` parameters: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 30
+    - Annotated parameters: 762
+    - Unannotated parameters: 51
+    - Explicit `Any` parameters: 39
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 51
 - Returns:
-    - Annotated returns: 148
-    - Unannotated returns: 10
-    - Explicit `Any` returns: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 45
+    - Annotated returns: 448
+    - Unannotated returns: 7
+    - Explicit `Any` returns: 19
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 33
 - Variables:
-    - Annotated variables: 80
-    - Explicit `Any` variables: 11
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 250
+    - Explicit `Any` variables: 20
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 46
-    - Class definitions with `Any`: 0
+    - Total class definitions: 222
+    - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `editdistance`
 
+### Upstream repo URL
+
+[https://github.com/roy-ht/editdistance](https://github.com/roy-ht/editdistance)
+
 ### Stub distribution name
 
 `types-editdistance`
 
 ### Number of lines
 
-3 (excluding blank lines)
+5 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2352,105 +2528,113 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `editdistance` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `editdistance` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `editdistance`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 4
+    - Annotated parameters: 10
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 2
+    - Annotated returns: 4
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 0
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 0
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `emoji`
+## Info on typeshed's stubs for `entrypoints`
+
+### Upstream repo URL
+
+[https://github.com/takluyver/entrypoints](https://github.com/takluyver/entrypoints)
 
 ### Stub distribution name
 
-`types-emoji`
+`types-entrypoints`
 
 ### Number of lines
 
-66 (excluding blank lines)
+41 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `emoji` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `entrypoints` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `emoji`
+### Statistics on the annotations in typeshed's stubs for `entrypoints`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 21
+    - Annotated parameters: 23
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 10
+    - Annotated returns: 12
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 12
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 5
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `entrypoints`
+## Info on typeshed's stubs for `fanstatic`
+
+### Upstream repo URL
+
+[https://github.com/zopefoundation/fanstatic](https://github.com/zopefoundation/fanstatic)
 
 ### Stub distribution name
 
-`types-entrypoints`
+`types-fanstatic`
 
 ### Number of lines
 
-45 (excluding blank lines)
+530 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2458,45 +2642,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `entrypoints` when running stubtest in CI.
+Typeshed currently has 40 unique allowlist entries for `fanstatic` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `entrypoints`
+### Statistics on the annotations in typeshed's stubs for `fanstatic`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 23
+    - Annotated parameters: 167
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
+    - Explicit `Any` parameters: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 12
+    - Annotated returns: 133
     - Unannotated returns: 0
-    - Explicit `Any` returns: 1
+    - Explicit `Any` returns: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 12
+    - Annotated variables: 128
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 5
+    - Total class definitions: 49
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `first`
 
+### Upstream repo URL
+
+[https://github.com/hynek/first](https://github.com/hynek/first)
+
 ### Stub distribution name
 
 `types-first`
 
 ### Number of lines
 
 14 (excluding blank lines)
@@ -2540,16 +2728,77 @@
 - Class definitions:
     - Total class definitions: 0
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `flake8`
+
+### Upstream repo URL
+
+[https://github.com/pycqa/flake8](https://github.com/pycqa/flake8)
+
+### Stub distribution name
+
+`types-flake8`
+
+### Number of lines
+
+570 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 2 unique allowlist entries for `flake8` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `flake8`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 221
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 35
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 163
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 8
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 182
+    - Explicit `Any` variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 94
+- Class definitions:
+    - Total class definitions: 39
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `flake8-2020`
 
+### Upstream repo URL
+
+[https://github.com/asottile/flake8-2020](https://github.com/asottile/flake8-2020)
+
 ### Stub distribution name
 
 `types-flake8-2020`
 
 ### Number of lines
 
 22 (excluding blank lines)
@@ -2595,14 +2844,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `flake8-bugbear`
 
+### Upstream repo URL
+
+[https://github.com/PyCQA/flake8-bugbear](https://github.com/PyCQA/flake8-bugbear)
+
 ### Stub distribution name
 
 `types-flake8-bugbear`
 
 ### Number of lines
 
 27 (excluding blank lines)
@@ -2617,15 +2870,15 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `flake8-bugbear` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `flake8-bugbear` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `flake8-bugbear`
 
@@ -2648,21 +2901,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `flake8-builtins`
 
+### Upstream repo URL
+
+[https://github.com/gforcada/flake8-builtins](https://github.com/gforcada/flake8-builtins)
+
 ### Stub distribution name
 
 `types-flake8-builtins`
 
 ### Number of lines
 
-10 (excluding blank lines)
+39 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2679,36 +2936,40 @@
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `flake8-builtins`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 3
+    - Annotated parameters: 17
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 3
+    - Annotated returns: 15
     - Unannotated returns: 0
-    - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 2
+    - Annotated variables: 11
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `flake8-docstrings`
 
+### Upstream repo URL
+
+[https://github.com/pycqa/flake8-docstrings](https://github.com/pycqa/flake8-docstrings)
+
 ### Stub distribution name
 
 `types-flake8-docstrings`
 
 ### Number of lines
 
 19 (excluding blank lines)
@@ -2752,68 +3013,19 @@
 - Class definitions:
     - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `flake8-plugin-utils`
-
-### Stub distribution name
-
-`types-flake8-plugin-utils`
-
-### Number of lines
-
-61 (excluding blank lines)
-
-### Package status: *up to date*
-
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *missing stubs ignored*
-
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 6 allowlist entries for `flake8-plugin-utils` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `flake8-plugin-utils`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 30
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 17
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 9
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 3
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
+## Info on typeshed's stubs for `flake8-rst-docstrings`
 
----
+### Upstream repo URL
 
-## Info on typeshed's stubs for `flake8-rst-docstrings`
+[https://github.com/peterjc/flake8-rst-docstrings](https://github.com/peterjc/flake8-rst-docstrings)
 
 ### Stub distribution name
 
 `types-flake8-rst-docstrings`
 
 ### Number of lines
 
@@ -2860,14 +3072,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `flake8-simplify`
 
+### Upstream repo URL
+
+[https://github.com/MartinThoma/flake8-simplify](https://github.com/MartinThoma/flake8-simplify)
+
 ### Stub distribution name
 
 `types-flake8-simplify`
 
 ### Number of lines
 
 8 (excluding blank lines)
@@ -2913,14 +3129,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `flake8-typing-imports`
 
+### Upstream repo URL
+
+[https://github.com/asottile/flake8-typing-imports](https://github.com/asottile/flake8-typing-imports)
+
 ### Stub distribution name
 
 `types-flake8-typing-imports`
 
 ### Number of lines
 
 15 (excluding blank lines)
@@ -2966,21 +3186,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `fpdf2`
 
+### Upstream repo URL
+
+[https://github.com/PyFPDF/fpdf2](https://github.com/PyFPDF/fpdf2)
+
 ### Stub distribution name
 
 `types-fpdf2`
 
 ### Number of lines
 
-2,185 (excluding blank lines)
+2,987 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -2988,107 +3212,174 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 7 allowlist entries for `fpdf2` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `fpdf2` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `fpdf2`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 642
-    - Unannotated parameters: 528
-    - Explicit `Any` parameters: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 67
+    - Annotated parameters: 969
+    - Unannotated parameters: 591
+    - Explicit `Any` parameters: 7
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 86
 - Returns:
-    - Annotated returns: 417
-    - Unannotated returns: 194
-    - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
+    - Annotated returns: 566
+    - Unannotated returns: 206
+    - Explicit `Any` returns: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
 - Variables:
-    - Annotated variables: 676
+    - Annotated variables: 681
     - Explicit `Any` variables: 14
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 160
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 166
 - Class definitions:
-    - Total class definitions: 156
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
+    - Total class definitions: 204
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
 ## Info on typeshed's stubs for `gdb`
 
 ### Extra description
 
-Type hints for GDB's [Python API](https://sourceware.org/gdb/onlinedocs/gdb/Python-API.html). Note that this API is available only when running Python scripts under GDB: is is not possible to install the `gdb` package separately, for instance using `pip`.
+Type hints for GDB's [Python API](https://sourceware.org/gdb/onlinedocs/gdb/Python-API.html). Note that this API is available only when running Python scripts under GDB: it is not possible to install the `gdb` package separately, for instance using `pip`.
+
+### Upstream repo URL
+
+[https://sourceware.org/git/gitweb.cgi?p=binutils-gdb.git;a=tree](https://sourceware.org/git/gitweb.cgi?p=binutils-gdb.git;a=tree)
 
 ### Stub distribution name
 
 `types-gdb`
 
 ### Number of lines
 
-733 (excluding blank lines)
+824 (excluding blank lines)
 
 ### Package status: *not on pypi*
 
 The runtime package that these stubs are for doesn't exist on PyPI, so whether or not these stubs are up to date or not is unknown.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *skipped*
+### Stubtest settings in CI: *error on missing stub*
 
-Stubtest is skipped in typeshed's CI for this package.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `gdb` when running stubtest in CI.
+Typeshed currently has 50 unique allowlist entries for `gdb` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `gdb`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 233
+    - Annotated parameters: 237
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
+    - Explicit `Any` parameters: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 257
+    - Annotated returns: 263
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 290
+    - Annotated variables: 318
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 87
+    - Total class definitions: 82
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `gevent`
+
+### Upstream repo URL
+
+[https://github.com/gevent/gevent](https://github.com/gevent/gevent)
+
+### Stub distribution name
+
+`types-gevent`
+
+### Number of lines
+
+3,018 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `darwin`, `linux` and `win32`.
+
+Typeshed currently has 150 unique allowlist entries for `gevent` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `gevent`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,346
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 65
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 5
+- Returns:
+    - Annotated returns: 824
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 21
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 359
+    - Explicit `Any` variables: 26
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 207
+    - Class definitions with `Any`: 2
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `google-cloud-ndb`
 
+### Upstream repo URL
+
+[https://github.com/googleapis/python-ndb](https://github.com/googleapis/python-ndb)
+
 ### Stub distribution name
 
 `types-google-cloud-ndb`
 
 ### Number of lines
 
-1,415 (excluding blank lines)
+1,536 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3096,52 +3387,56 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 3 allowlist entries for `google-cloud-ndb` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `google-cloud-ndb` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `google-cloud-ndb`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 479
+    - Annotated parameters: 486
     - Unannotated parameters: 368
     - Explicit `Any` parameters: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 123
 - Returns:
-    - Annotated returns: 234
+    - Annotated returns: 236
     - Unannotated returns: 203
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 190
+    - Annotated variables: 194
     - Explicit `Any` variables: 132
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
     - Total class definitions: 143
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `hdbcli`
+## Info on typeshed's stubs for `greenlet`
+
+### Upstream repo URL
+
+[https://github.com/python-greenlet/greenlet](https://github.com/python-greenlet/greenlet)
 
 ### Stub distribution name
 
-`types-hdbcli`
+`types-greenlet`
 
 ### Number of lines
 
-129 (excluding blank lines)
+79 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3149,52 +3444,109 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 5 allowlist entries for `hdbcli` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `greenlet` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `hdbcli`
+### Statistics on the annotations in typeshed's stubs for `greenlet`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 77
+    - Annotated parameters: 21
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 12
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 6
+    - Explicit `Any` parameters: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 62
+    - Annotated returns: 25
     - Unannotated returns: 0
-    - Explicit `Any` returns: 7
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
+    - Explicit `Any` returns: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 11
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 5
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `hdbcli`
+
+### Stub distribution name
+
+`types-hdbcli`
+
+### Number of lines
+
+138 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 8 unique allowlist entries for `hdbcli` when running stubtest in CI.
+
+### Pyright settings in CI: *strict on some files*
+
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
+
+### Statistics on the annotations in typeshed's stubs for `hdbcli`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 75
+    - Unannotated parameters: 6
+    - Explicit `Any` parameters: 12
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 64
+    - Unannotated returns: 3
+    - Explicit `Any` returns: 10
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 21
     - Explicit `Any` variables: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
     - Total class definitions: 16
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `html5lib`
 
+### Upstream repo URL
+
+[https://github.com/html5lib/html5lib-python](https://github.com/html5lib/html5lib-python)
+
 ### Stub distribution name
 
 `types-html5lib`
 
 ### Number of lines
 
-673 (excluding blank lines)
+696 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3211,43 +3563,47 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `html5lib`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 67
-    - Unannotated parameters: 207
+    - Annotated parameters: 87
+    - Unannotated parameters: 195
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 27
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 23
 - Returns:
-    - Annotated returns: 100
-    - Unannotated returns: 208
+    - Annotated returns: 133
+    - Unannotated returns: 177
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 220
-    - Explicit `Any` variables: 180
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 224
+    - Explicit `Any` variables: 175
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 40
+    - Total class definitions: 41
     - Class definitions with `Any`: 4
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `httplib2`
 
+### Upstream repo URL
+
+[https://github.com/httplib2/httplib2](https://github.com/httplib2/httplib2)
+
 ### Stub distribution name
 
 `types-httplib2`
 
 ### Number of lines
 
-253 (excluding blank lines)
+254 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3255,15 +3611,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `httplib2` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `httplib2` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `httplib2`
 
@@ -3274,26 +3630,30 @@
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 37
 - Returns:
     - Annotated returns: 39
     - Unannotated returns: 25
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 86
-    - Explicit `Any` variables: 57
+    - Annotated variables: 87
+    - Explicit `Any` variables: 58
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 33
     - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `humanfriendly`
 
+### Upstream repo URL
+
+[https://github.com/xolox/python-humanfriendly](https://github.com/xolox/python-humanfriendly)
+
 ### Stub distribution name
 
 `types-humanfriendly`
 
 ### Number of lines
 
 340 (excluding blank lines)
@@ -3308,25 +3668,25 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 7 allowlist entries for `humanfriendly` when running stubtest in CI.
+Typeshed currently has 7 unique allowlist entries for `humanfriendly` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `humanfriendly`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 79
-    - Unannotated parameters: 181
+    - Annotated parameters: 81
+    - Unannotated parameters: 179
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 22
 - Returns:
     - Annotated returns: 82
     - Unannotated returns: 95
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
@@ -3337,23 +3697,84 @@
 - Class definitions:
     - Total class definitions: 25
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `hvac`
+
+### Upstream repo URL
+
+[https://github.com/hvac/hvac](https://github.com/hvac/hvac)
+
+### Stub distribution name
+
+`types-hvac`
+
+### Number of lines
+
+2,125 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 2 unique allowlist entries for `hvac` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `hvac`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,028
+    - Unannotated parameters: 694
+    - Explicit `Any` parameters: 27
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 530
+- Returns:
+    - Annotated returns: 77
+    - Unannotated returns: 490
+    - Explicit `Any` returns: 19
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 94
+    - Explicit `Any` variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 15
+- Class definitions:
+    - Total class definitions: 75
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `ibm-db`
 
+### Upstream repo URL
+
+[https://github.com/ibmdb/python-ibmdb](https://github.com/ibmdb/python-ibmdb)
+
 ### Stub distribution name
 
 `types-ibm-db`
 
 ### Number of lines
 
-252 (excluding blank lines)
+336 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3380,33 +3801,98 @@
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 65
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 110
+    - Annotated variables: 196
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 4
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `icalendar`
+
+### Upstream repo URL
+
+[https://github.com/collective/icalendar](https://github.com/collective/icalendar)
+
+### Stub distribution name
+
+`types-icalendar`
+
+### Number of lines
+
+417 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 4 unique allowlist entries for `icalendar` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `icalendar`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 109
+    - Unannotated parameters: 85
+    - Explicit `Any` parameters: 5
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 6
+- Returns:
+    - Annotated returns: 87
+    - Unannotated returns: 73
+    - Explicit `Any` returns: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+- Variables:
+    - Annotated variables: 89
+    - Explicit `Any` variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 41
+- Class definitions:
+    - Total class definitions: 41
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 3
+
+---
+
 ## Info on typeshed's stubs for `influxdb-client`
 
+### Extra description
+
+Note: `types-influxdb-client` has required `urllib3>=2` since v1.37.0.1. If you need to install `types-influxdb-client` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-influxdb-client<1.37.0.1`.
+
+### Upstream repo URL
+
+[https://github.com/influxdata/influxdb-client-python](https://github.com/influxdata/influxdb-client-python)
+
 ### Stub distribution name
 
 `types-influxdb-client`
 
 ### Number of lines
 
-13,317 (excluding blank lines)
+13,460 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3414,98 +3900,106 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `influxdb-client` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `influxdb-client` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `influxdb-client`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 2,269
-    - Unannotated parameters: 3,800
+    - Annotated parameters: 2,353
+    - Unannotated parameters: 3,778
     - Explicit `Any` parameters: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1,979
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1,957
 - Returns:
-    - Annotated returns: 1,857
-    - Unannotated returns: 3,446
-    - Explicit `Any` returns: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Annotated returns: 1,864
+    - Unannotated returns: 3,423
+    - Explicit `Any` returns: 5
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 1,178
+    - Annotated variables: 1,195
     - Explicit `Any` variables: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1,076
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1,063
 - Class definitions:
     - Total class definitions: 423
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `invoke`
+## Info on typeshed's stubs for `inifile`
+
+### Upstream repo URL
+
+[https://github.com/mitsuhiko/python-inifile](https://github.com/mitsuhiko/python-inifile)
 
 ### Stub distribution name
 
-`types-invoke`
+`types-inifile`
 
 ### Number of lines
 
-741 (excluding blank lines)
+122 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `invoke` when running stubtest in CI.
+Typeshed currently has 20 unique allowlist entries for `inifile` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `invoke`
+### Statistics on the annotations in typeshed's stubs for `inifile`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 243
-    - Unannotated parameters: 171
-    - Explicit `Any` parameters: 28
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
+    - Annotated parameters: 57
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 174
-    - Unannotated returns: 73
-    - Explicit `Any` returns: 8
+    - Annotated returns: 58
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 128
-    - Explicit `Any` variables: 70
+    - Annotated variables: 1
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 43
+    - Total class definitions: 4
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `jmespath`
 
+### Upstream repo URL
+
+[https://github.com/jmespath/jmespath.py](https://github.com/jmespath/jmespath.py)
+
 ### Stub distribution name
 
 `types-jmespath`
 
 ### Number of lines
 
 172 (excluding blank lines)
@@ -3551,21 +4045,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `jsonschema`
 
+### Upstream repo URL
+
+[https://github.com/python-jsonschema/jsonschema](https://github.com/python-jsonschema/jsonschema)
+
 ### Stub distribution name
 
 `types-jsonschema`
 
 ### Number of lines
 
-389 (excluding blank lines)
+422 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3582,43 +4080,47 @@
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `jsonschema`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 108
-    - Unannotated parameters: 295
-    - Explicit `Any` parameters: 10
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 12
+    - Annotated parameters: 117
+    - Unannotated parameters: 307
+    - Explicit `Any` parameters: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 19
 - Returns:
-    - Annotated returns: 145
-    - Unannotated returns: 31
-    - Explicit `Any` returns: 9
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Annotated returns: 153
+    - Unannotated returns: 29
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 11
 - Variables:
-    - Annotated variables: 54
-    - Explicit `Any` variables: 23
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 52
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 19
 - Class definitions:
-    - Total class definitions: 25
+    - Total class definitions: 26
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `keyboard`
 
+### Upstream repo URL
+
+[https://github.com/boppreh/keyboard](https://github.com/boppreh/keyboard)
+
 ### Stub distribution name
 
 `types-keyboard`
 
 ### Number of lines
 
-240 (excluding blank lines)
+246 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3626,15 +4128,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 6 allowlist entries for `keyboard` when running stubtest in CI.
+Typeshed currently has 7 unique allowlist entries for `keyboard` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `keyboard`
 
@@ -3657,21 +4159,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `ldap3`
 
+### Upstream repo URL
+
+[https://github.com/cannatag/ldap3](https://github.com/cannatag/ldap3)
+
 ### Stub distribution name
 
 `types-ldap3`
 
 ### Number of lines
 
-2,648 (excluding blank lines)
+2,659 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3708,23 +4214,141 @@
 - Class definitions:
     - Total class definitions: 316
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `libsass`
+
+### Upstream repo URL
+
+[https://github.com/sass/libsass-python](https://github.com/sass/libsass-python)
+
+### Stub distribution name
+
+`types-libsass`
+
+### Number of lines
+
+230 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 2 unique allowlist entries for `libsass` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `libsass`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 109
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 41
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 36
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 17
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `lzstring`
+
+### Upstream repo URL
+
+[https://github.com/gkovacs/lz-string-python](https://github.com/gkovacs/lz-string-python)
+
+### Stub distribution name
+
+`types-lzstring`
+
+### Number of lines
+
+17 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 5 unique allowlist entries for `lzstring` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `lzstring`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 8
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 8
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 0
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 1
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `mock`
 
+### Upstream repo URL
+
+[https://github.com/testing-cabal/mock](https://github.com/testing-cabal/mock)
+
 ### Stub distribution name
 
 `types-mock`
 
 ### Number of lines
 
-359 (excluding blank lines)
+390 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3732,52 +4356,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `mock` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `mock` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `mock`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 204
+    - Annotated parameters: 217
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 76
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 47
+    - Explicit `Any` parameters: 86
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 45
 - Returns:
-    - Annotated returns: 85
+    - Annotated returns: 90
     - Unannotated returns: 0
     - Explicit `Any` returns: 15
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 56
+    - Annotated variables: 58
     - Explicit `Any` variables: 34
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 23
+    - Total class definitions: 24
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `mypy-extensions`
 
+### Upstream repo URL
+
+[https://github.com/python/mypy_extensions](https://github.com/python/mypy_extensions)
+
 ### Stub distribution name
 
 `types-mypy-extensions`
 
 ### Number of lines
 
-71 (excluding blank lines)
+79 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3785,29 +4413,29 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 6 allowlist entries for `mypy-extensions` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `mypy-extensions` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `mypy-extensions`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 28
+    - Annotated parameters: 31
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 1
+    - Explicit `Any` parameters: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 25
+    - Annotated returns: 28
     - Unannotated returns: 0
     - Explicit `Any` returns: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 1
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
@@ -3816,21 +4444,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `mysqlclient`
 
+### Upstream repo URL
+
+[https://github.com/PyMySQL/mysqlclient](https://github.com/PyMySQL/mysqlclient)
+
 ### Stub distribution name
 
 `types-mysqlclient`
 
 ### Number of lines
 
-1,215 (excluding blank lines)
+1,228 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3838,52 +4470,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `mysqlclient` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `mysqlclient` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `mysqlclient`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 28
-    - Unannotated parameters: 128
-    - Explicit `Any` parameters: 1
+    - Annotated parameters: 35
+    - Unannotated parameters: 124
+    - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
 - Returns:
-    - Annotated returns: 83
-    - Unannotated returns: 30
-    - Explicit `Any` returns: 51
+    - Annotated returns: 37
+    - Unannotated returns: 79
+    - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 972
-    - Explicit `Any` variables: 31
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 971
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 28
 - Class definitions:
     - Total class definitions: 35
-    - Class definitions with `Any`: 1
-    - Class definitions marked as at least partially `Incomplete`: 0
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
 ## Info on typeshed's stubs for `netaddr`
 
+### Upstream repo URL
+
+[https://github.com/drkjam/netaddr](https://github.com/drkjam/netaddr)
+
 ### Stub distribution name
 
 `types-netaddr`
 
 ### Number of lines
 
-659 (excluding blank lines)
+696 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3891,52 +4527,113 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `netaddr` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `netaddr` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *strict on some files*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for `netaddr`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 292
-    - Unannotated parameters: 0
+    - Annotated parameters: 286
+    - Unannotated parameters: 4
     - Explicit `Any` parameters: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 5
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
-    - Annotated returns: 310
+    - Annotated returns: 308
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 103
-    - Explicit `Any` variables: 0
+    - Annotated variables: 101
+    - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
     - Total class definitions: 43
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `networkx`
+
+### Upstream repo URL
+
+[https://github.com/networkx/networkx](https://github.com/networkx/networkx)
+
+### Stub distribution name
+
+`types-networkx`
+
+### Number of lines
+
+4,781 (excluding blank lines)
+
+### Package status: *out of date*
+
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *missing stubs ignored*
+
+The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 13 unique allowlist entries for `networkx` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `networkx`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,959
+    - Unannotated parameters: 1,511
+    - Explicit `Any` parameters: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 763
+- Returns:
+    - Annotated returns: 503
+    - Unannotated returns: 808
+    - Explicit `Any` returns: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 102
+- Variables:
+    - Annotated variables: 320
+    - Explicit `Any` variables: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 249
+- Class definitions:
+    - Total class definitions: 126
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 2
+
+---
+
 ## Info on typeshed's stubs for `oauthlib`
 
+### Upstream repo URL
+
+[https://github.com/oauthlib/oauthlib](https://github.com/oauthlib/oauthlib)
+
 ### Stub distribution name
 
 `types-oauthlib`
 
 ### Number of lines
 
-1,385 (excluding blank lines)
+1,444 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -3944,105 +4641,170 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `oauthlib` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `oauthlib` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `oauthlib`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 274
-    - Unannotated parameters: 541
+    - Annotated parameters: 406
+    - Unannotated parameters: 414
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 185
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 182
 - Returns:
-    - Annotated returns: 139
-    - Unannotated returns: 211
+    - Annotated returns: 161
+    - Unannotated returns: 191
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 318
+    - Annotated variables: 329
     - Explicit `Any` variables: 207
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
-    - Total class definitions: 106
+    - Total class definitions: 109
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `olefile`
+
+### Upstream repo URL
+
+[https://github.com/decalage2/olefile](https://github.com/decalage2/olefile)
+
+### Stub distribution name
+
+`types-olefile`
+
+### Number of lines
+
+214 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 1 unique allowlist entry for `olefile` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `olefile`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 103
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 66
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 73
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 7
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `openpyxl`
 
+### Upstream repo URL
+
+[https://foss.heptapod.net/openpyxl/openpyxl](https://foss.heptapod.net/openpyxl/openpyxl)
+
 ### Stub distribution name
 
 `types-openpyxl`
 
 ### Number of lines
 
-9,276 (excluding blank lines)
+13,238 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `openpyxl` when running stubtest in CI.
+Typeshed currently has 183 unique allowlist entries for `openpyxl` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `openpyxl`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 2,690
-    - Unannotated parameters: 607
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 2,186
+    - Annotated parameters: 3,902
+    - Unannotated parameters: 341
+    - Explicit `Any` parameters: 12
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 211
 - Returns:
-    - Annotated returns: 819
-    - Unannotated returns: 356
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 18
+    - Annotated returns: 1,315
+    - Unannotated returns: 91
+    - Explicit `Any` returns: 13
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 8
 - Variables:
-    - Annotated variables: 4,197
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 3,559
+    - Annotated variables: 4,048
+    - Explicit `Any` variables: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 352
 - Class definitions:
-    - Total class definitions: 566
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 5
+    - Total class definitions: 609
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 21
 
 ---
 
 ## Info on typeshed's stubs for `opentracing`
 
+### Upstream repo URL
+
+[https://github.com/opentracing/opentracing-python](https://github.com/opentracing/opentracing-python)
+
 ### Stub distribution name
 
 `types-opentracing`
 
 ### Number of lines
 
-329 (excluding blank lines)
+331 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4050,15 +4812,15 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 4 allowlist entries for `opentracing` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `opentracing` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `opentracing`
 
@@ -4081,25 +4843,29 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `paho-mqtt`
 
+### Upstream repo URL
+
+[https://github.com/eclipse/paho.mqtt.python](https://github.com/eclipse/paho.mqtt.python)
+
 ### Stub distribution name
 
 `types-paho-mqtt`
 
 ### Number of lines
 
-503 (excluding blank lines)
+513 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *obsolete*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+The runtime package has added inline type hints; these typeshed stubs are now obsolete.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
@@ -4134,21 +4900,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `paramiko`
 
+### Upstream repo URL
+
+[https://github.com/paramiko/paramiko](https://github.com/paramiko/paramiko)
+
 ### Stub distribution name
 
 `types-paramiko`
 
 ### Number of lines
 
-1,724 (excluding blank lines)
+1,840 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4156,52 +4926,56 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 14 allowlist entries for `paramiko` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `paramiko` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `paramiko`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 738
+    - Annotated parameters: 770
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 20
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
 - Returns:
-    - Annotated returns: 623
+    - Annotated returns: 642
     - Unannotated returns: 0
     - Explicit `Any` returns: 9
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 529
-    - Explicit `Any` variables: 17
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 545
+    - Explicit `Any` variables: 14
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 3
 - Class definitions:
-    - Total class definitions: 113
+    - Total class definitions: 124
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `parsimonious`
 
+### Upstream repo URL
+
+[https://github.com/erikrose/parsimonious](https://github.com/erikrose/parsimonious)
+
 ### Stub distribution name
 
 `types-parsimonious`
 
 ### Number of lines
 
-181 (excluding blank lines)
+187 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4209,52 +4983,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 4 allowlist entries for `parsimonious` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `parsimonious` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *strict on some files*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for `parsimonious`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 114
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 23
+    - Explicit `Any` parameters: 22
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 60
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 4
+    - Annotated returns: 59
+    - Unannotated returns: 1
+    - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 34
     - Explicit `Any` variables: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2
 - Class definitions:
     - Total class definitions: 27
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `passlib`
 
+### Upstream repo URL
+
+[https://foss.heptapod.net/python-libs/passlib](https://foss.heptapod.net/python-libs/passlib)
+
 ### Stub distribution name
 
 `types-passlib`
 
 ### Number of lines
 
-1,778 (excluding blank lines)
+1,798 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4262,45 +5040,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 31 allowlist entries for `passlib` when running stubtest in CI.
+Typeshed currently has 31 unique allowlist entries for `passlib` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `passlib`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 382
-    - Unannotated parameters: 466
-    - Explicit `Any` parameters: 18
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 156
+    - Annotated parameters: 410
+    - Unannotated parameters: 442
+    - Explicit `Any` parameters: 27
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 132
 - Returns:
-    - Annotated returns: 155
-    - Unannotated returns: 329
-    - Explicit `Any` returns: 10
+    - Annotated returns: 187
+    - Unannotated returns: 297
+    - Explicit `Any` returns: 13
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 576
-    - Explicit `Any` variables: 101
+    - Explicit `Any` variables: 92
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 3
 - Class definitions:
     - Total class definitions: 143
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `passpy`
 
+### Upstream repo URL
+
+[https://github.com/bfrascher/passpy](https://github.com/bfrascher/passpy)
+
 ### Stub distribution name
 
 `types-passpy`
 
 ### Number of lines
 
 47 (excluding blank lines)
@@ -4315,15 +5097,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 3 allowlist entries for `passpy` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `passpy` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `passpy`
 
@@ -4346,74 +5128,82 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `peewee`
 
+### Upstream repo URL
+
+[https://github.com/coleifer/peewee](https://github.com/coleifer/peewee)
+
 ### Stub distribution name
 
 `types-peewee`
 
 ### Number of lines
 
-1,609 (excluding blank lines)
+1,693 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 25 allowlist entries for `peewee` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `peewee` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `peewee`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 370
-    - Unannotated parameters: 704
+    - Annotated parameters: 425
+    - Unannotated parameters: 669
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 244
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 216
 - Returns:
-    - Annotated returns: 298
-    - Unannotated returns: 448
+    - Annotated returns: 346
+    - Unannotated returns: 438
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 5
 - Variables:
-    - Annotated variables: 437
+    - Annotated variables: 420
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 368
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 348
 - Class definitions:
-    - Total class definitions: 166
+    - Total class definitions: 168
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pep8-naming`
 
+### Upstream repo URL
+
+[https://github.com/PyCQA/pep8-naming](https://github.com/PyCQA/pep8-naming)
+
 ### Stub distribution name
 
 `types-pep8-naming`
 
 ### Number of lines
 
-27 (excluding blank lines)
+26 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4421,15 +5211,15 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `pep8-naming` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `pep8-naming` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pep8-naming`
 
@@ -4440,37 +5230,98 @@
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 8
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 11
+    - Annotated variables: 10
     - Explicit `Any` variables: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `pexpect`
+
+### Upstream repo URL
+
+[https://github.com/pexpect/pexpect](https://github.com/pexpect/pexpect)
+
+### Stub distribution name
+
+`types-pexpect`
+
+### Number of lines
+
+673 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 1 unique allowlist entry for `pexpect` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `pexpect`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 234
+    - Unannotated parameters: 120
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 8
+- Returns:
+    - Annotated returns: 181
+    - Unannotated returns: 33
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 160
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 24
+- Class definitions:
+    - Total class definitions: 22
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `pika`
 
 ### Extra description
 
 The `types-pika` package contains alternate, more complete type stubs, that are maintained outside of typeshed.
 
+### Upstream repo URL
+
+[https://github.com/pika/pika](https://github.com/pika/pika)
+
 ### Stub distribution name
 
 `types-pika-ts`
 
 ### Number of lines
 
-2,187 (excluding blank lines)
+2,235 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4478,45 +5329,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 20 allowlist entries for `pika` when running stubtest in CI.
+Typeshed currently has 9 unique allowlist entries for `pika` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `pika`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 604
-    - Unannotated parameters: 397
+    - Annotated parameters: 618
+    - Unannotated parameters: 383
     - Explicit `Any` parameters: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 141
 - Returns:
-    - Annotated returns: 390
-    - Unannotated returns: 370
+    - Annotated returns: 413
+    - Unannotated returns: 347
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 24
 - Variables:
-    - Annotated variables: 470
+    - Annotated variables: 464
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 261
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 258
 - Class definitions:
     - Total class definitions: 222
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `playsound`
 
+### Upstream repo URL
+
+[https://github.com/TaylorSMarks/playsound](https://github.com/TaylorSMarks/playsound)
+
 ### Stub distribution name
 
 `types-playsound`
 
 ### Number of lines
 
 5 (excluding blank lines)
@@ -4562,21 +5417,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `polib`
 
+### Upstream repo URL
+
+[https://github.com/izimobil/polib](https://github.com/izimobil/polib)
+
 ### Stub distribution name
 
 `types-polib`
 
 ### Number of lines
 
-144 (excluding blank lines)
+143 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4613,133 +5472,145 @@
 - Class definitions:
     - Total class definitions: 8
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `prettytable`
+## Info on typeshed's stubs for `portpicker`
+
+### Upstream repo URL
+
+[https://github.com/google/python_portpicker](https://github.com/google/python_portpicker)
 
 ### Stub distribution name
 
-`types-prettytable`
+`types-portpicker`
 
 ### Number of lines
 
-294 (excluding blank lines)
+16 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `prettytable` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `portpicker` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `prettytable`
+### Statistics on the annotations in typeshed's stubs for `portpicker`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 18
-    - Unannotated parameters: 77
+    - Annotated parameters: 10
+    - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 70
-    - Unannotated returns: 56
+    - Annotated returns: 6
+    - Unannotated returns: 0
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 34
-    - Explicit `Any` variables: 6
+    - Annotated variables: 0
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 5
+    - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `protobuf`
 
 ### Extra description
 
-Generated with aid from mypy-protobuf v3.4.0
+Generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on [protobuf v26.1](https://github.com/protocolbuffers/protobuf/releases/tag/v26.1) (python protobuf==5.26.1)
+
+### Upstream repo URL
+
+[https://github.com/protocolbuffers/protobuf](https://github.com/protocolbuffers/protobuf)
 
 ### Stub distribution name
 
 `types-protobuf`
 
 ### Number of lines
 
-4,281 (excluding blank lines)
+4,825 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *up to date*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 14 allowlist entries for `protobuf` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `protobuf` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `protobuf`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 726
-    - Unannotated parameters: 248
-    - Explicit `Any` parameters: 15
+    - Annotated parameters: 785
+    - Unannotated parameters: 254
+    - Explicit `Any` parameters: 17
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 14
 - Returns:
-    - Annotated returns: 494
-    - Unannotated returns: 79
+    - Annotated returns: 530
+    - Unannotated returns: 75
     - Explicit `Any` returns: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 738
-    - Explicit `Any` variables: 126
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 921
+    - Explicit `Any` variables: 123
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 147
+    - Total class definitions: 185
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `psutil`
 
+### Upstream repo URL
+
+[https://github.com/giampaolo/psutil](https://github.com/giampaolo/psutil)
+
 ### Stub distribution name
 
 `types-psutil`
 
 ### Number of lines
 
-1,546 (excluding blank lines)
+1,565 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4747,105 +5618,113 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 20 allowlist entries for `psutil` when running stubtest in CI.
+Typeshed currently has 14 unique allowlist entries for `psutil` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `psutil`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 117
+    - Annotated parameters: 125
     - Unannotated parameters: 310
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 28
 - Returns:
-    - Annotated returns: 185
-    - Unannotated returns: 358
+    - Annotated returns: 194
+    - Unannotated returns: 355
     - Explicit `Any` returns: 47
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 610
-    - Explicit `Any` variables: 203
+    - Annotated variables: 592
+    - Explicit `Any` variables: 198
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 99
 - Class definitions:
-    - Total class definitions: 90
+    - Total class definitions: 89
     - Class definitions with `Any`: 3
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `psycopg2`
 
+### Upstream repo URL
+
+[https://github.com/psycopg/psycopg2](https://github.com/psycopg/psycopg2)
+
 ### Stub distribution name
 
 `types-psycopg2`
 
 ### Number of lines
 
-1,563 (excluding blank lines)
+1,731 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 5 allowlist entries for `psycopg2` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `psycopg2` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `psycopg2`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 171
-    - Unannotated parameters: 328
-    - Explicit `Any` parameters: 4
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 52
+    - Annotated parameters: 337
+    - Unannotated parameters: 152
+    - Explicit `Any` parameters: 14
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 29
 - Returns:
-    - Annotated returns: 189
-    - Unannotated returns: 169
-    - Explicit `Any` returns: 7
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+    - Annotated returns: 314
+    - Unannotated returns: 75
+    - Explicit `Any` returns: 21
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 5
 - Variables:
-    - Annotated variables: 532
-    - Explicit `Any` variables: 168
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 517
+    - Explicit `Any` variables: 60
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 3
 - Class definitions:
-    - Total class definitions: 335
+    - Total class definitions: 331
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyOpenSSL`
 
+### Upstream repo URL
+
+[https://github.com/pyca/pyopenssl](https://github.com/pyca/pyopenssl)
+
 ### Stub distribution name
 
 `types-pyOpenSSL`
 
 ### Number of lines
 
-374 (excluding blank lines)
+363 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4853,45 +5732,49 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `pyOpenSSL` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `pyOpenSSL` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pyOpenSSL`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 163
+    - Annotated parameters: 148
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
-    - Annotated returns: 198
+    - Annotated returns: 179
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
 - Variables:
-    - Annotated variables: 120
+    - Annotated variables: 125
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 25
+    - Total class definitions: 22
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyRFC3339`
 
+### Upstream repo URL
+
+[https://github.com/kurtraschke/pyRFC3339](https://github.com/kurtraschke/pyRFC3339)
+
 ### Stub distribution name
 
 `types-pyRFC3339`
 
 ### Number of lines
 
 17 (excluding blank lines)
@@ -4937,21 +5820,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyasn1`
 
+### Upstream repo URL
+
+[https://github.com/pyasn1/pyasn1](https://github.com/pyasn1/pyasn1)
+
 ### Stub distribution name
 
 `types-pyasn1`
 
 ### Number of lines
 
-1,316 (excluding blank lines)
+1,502 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -4959,38 +5846,38 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 5 allowlist entries for `pyasn1` when running stubtest in CI.
+Typeshed currently has 8 unique allowlist entries for `pyasn1` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `pyasn1`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 196
-    - Unannotated parameters: 501
+    - Annotated parameters: 209
+    - Unannotated parameters: 533
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 38
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 39
 - Returns:
-    - Annotated returns: 111
-    - Unannotated returns: 411
+    - Annotated returns: 118
+    - Unannotated returns: 425
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 6
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 9
 - Variables:
-    - Annotated variables: 207
+    - Annotated variables: 251
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 164
+    - Total class definitions: 178
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyaudio`
 
@@ -5043,21 +5930,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pycocotools`
 
+### Upstream repo URL
+
+[https://github.com/ppwwyyxx/cocoapi](https://github.com/ppwwyyxx/cocoapi)
+
 ### Stub distribution name
 
 `types-pycocotools`
 
 ### Number of lines
 
-172 (excluding blank lines)
+183 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5084,79 +5975,87 @@
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 35
     - Unannotated returns: 0
     - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 64
+    - Annotated variables: 70
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 11
+    - Total class definitions: 12
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pycurl`
 
+### Upstream repo URL
+
+[https://github.com/pycurl/pycurl](https://github.com/pycurl/pycurl)
+
 ### Stub distribution name
 
 `types-pycurl`
 
 ### Number of lines
 
-674 (excluding blank lines)
+706 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
 Typeshed currently has 0 allowlist entries for `pycurl` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `pycurl`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 22
-    - Unannotated parameters: 0
+    - Annotated parameters: 15
+    - Unannotated parameters: 7
     - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 7
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 32
-    - Unannotated returns: 0
+    - Annotated returns: 26
+    - Unannotated returns: 6
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 10
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
 - Variables:
-    - Annotated variables: 629
+    - Annotated variables: 659
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 4
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyfarmhash`
 
+### Upstream repo URL
+
+[https://github.com/veelion/python-farmhash](https://github.com/veelion/python-farmhash)
+
 ### Stub distribution name
 
 `types-pyfarmhash`
 
 ### Number of lines
 
 9 (excluding blank lines)
@@ -5202,21 +6101,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyflakes`
 
+### Upstream repo URL
+
+[https://github.com/PyCQA/pyflakes](https://github.com/PyCQA/pyflakes)
+
 ### Stub distribution name
 
 `types-pyflakes`
 
 ### Number of lines
 
-428 (excluding blank lines)
+434 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5224,52 +6127,113 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 24 allowlist entries for `pyflakes` when running stubtest in CI.
+Typeshed currently has 24 unique allowlist entries for `pyflakes` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `pyflakes`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 267
+    - Annotated parameters: 265
     - Unannotated parameters: 69
     - Explicit `Any` parameters: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 210
+    - Annotated returns: 206
     - Unannotated returns: 2
     - Explicit `Any` returns: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 76
+    - Annotated variables: 75
     - Explicit `Any` variables: 33
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 74
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
+## Info on typeshed's stubs for `pygit2`
+
+### Upstream repo URL
+
+[https://github.com/libgit2/pygit2](https://github.com/libgit2/pygit2)
+
+### Stub distribution name
+
+`types-pygit2`
+
+### Number of lines
+
+1,928 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `darwin`, `linux` and `win32`.
+
+Typeshed currently has 11 unique allowlist entries for `pygit2` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `pygit2`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 674
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 503
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 474
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+- Class definitions:
+    - Total class definitions: 119
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
 ## Info on typeshed's stubs for `pyinstaller`
 
+### Upstream repo URL
+
+[https://github.com/pyinstaller/pyinstaller](https://github.com/pyinstaller/pyinstaller)
+
 ### Stub distribution name
 
 `types-pyinstaller`
 
 ### Number of lines
 
-429 (excluding blank lines)
+703 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5277,68 +6241,129 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 33 allowlist entries for `pyinstaller` when running stubtest in CI.
+Typeshed currently has 49 unique allowlist entries for `pyinstaller` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pyinstaller`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 188
+    - Annotated parameters: 274
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 9
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 6
 - Returns:
-    - Annotated returns: 117
+    - Annotated returns: 149
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 98
+    - Annotated variables: 195
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 15
+- Class definitions:
+    - Total class definitions: 26
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `pyjks`
+
+### Upstream repo URL
+
+[https://github.com/kurtbrose/pyjks](https://github.com/kurtbrose/pyjks)
+
+### Stub distribution name
+
+`types-pyjks`
+
+### Number of lines
+
+377 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 38 unique allowlist entries for `pyjks` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `pyjks`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 132
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 59
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 73
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 18
+    - Total class definitions: 31
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pynput`
 
+### Upstream repo URL
+
+[https://github.com/moses-palmer/pynput](https://github.com/moses-palmer/pynput)
+
 ### Stub distribution name
 
 `types-pynput`
 
 ### Number of lines
 
 324 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 14 allowlist entries for `pynput` when running stubtest in CI.
+Typeshed currently has 12 unique allowlist entries for `pynput` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pynput`
 
@@ -5349,33 +6374,37 @@
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 71
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 155
+    - Annotated variables: 58
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 24
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pyserial`
 
+### Upstream repo URL
+
+[https://github.com/pyserial/pyserial](https://github.com/pyserial/pyserial)
+
 ### Stub distribution name
 
 `types-pyserial`
 
 ### Number of lines
 
-1,033 (excluding blank lines)
+1,079 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5383,52 +6412,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 84 allowlist entries for `pyserial` when running stubtest in CI.
+Typeshed currently has 64 unique allowlist entries for `pyserial` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pyserial`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 205
+    - Annotated parameters: 223
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 251
+    - Annotated returns: 270
     - Unannotated returns: 0
     - Explicit `Any` returns: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 466
     - Explicit `Any` variables: 7
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 65
 - Class definitions:
     - Total class definitions: 66
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pysftp`
 
+### Upstream repo URL
+
+[https://bitbucket.org/dundeemt/pysftp](https://bitbucket.org/dundeemt/pysftp)
+
 ### Stub distribution name
 
 `types-pysftp`
 
 ### Number of lines
 
-161 (excluding blank lines)
+166 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5467,14 +6500,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pytest-lazy-fixture`
 
+### Upstream repo URL
+
+[https://github.com/tvorog/pytest-lazy-fixture](https://github.com/tvorog/pytest-lazy-fixture)
+
 ### Stub distribution name
 
 `types-pytest-lazy-fixture`
 
 ### Number of lines
 
 12 (excluding blank lines)
@@ -5489,15 +6526,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 7 allowlist entries for `pytest-lazy-fixture` when running stubtest in CI.
+Typeshed currently has 8 unique allowlist entries for `pytest-lazy-fixture` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pytest-lazy-fixture`
 
@@ -5520,21 +6557,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-crontab`
 
+### Upstream repo URL
+
+[https://gitlab.com/doctormo/python-crontab](https://gitlab.com/doctormo/python-crontab)
+
 ### Stub distribution name
 
 `types-python-crontab`
 
 ### Number of lines
 
-292 (excluding blank lines)
+328 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5542,45 +6583,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `python-crontab` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `python-crontab` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `python-crontab`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 137
-    - Unannotated parameters: 0
+    - Annotated parameters: 174
+    - Unannotated parameters: 2
     - Explicit `Any` parameters: 17
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 1
 - Returns:
-    - Annotated returns: 133
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
+    - Annotated returns: 146
+    - Unannotated returns: 4
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 66
+    - Annotated variables: 72
     - Explicit `Any` variables: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
 - Class definitions:
-    - Total class definitions: 17
+    - Total class definitions: 18
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 1
 
 ---
 
 ## Info on typeshed's stubs for `python-datemath`
 
+### Upstream repo URL
+
+[https://github.com/nickmaccarthy/python-datemath](https://github.com/nickmaccarthy/python-datemath)
+
 ### Stub distribution name
 
 `types-python-datemath`
 
 ### Number of lines
 
 16 (excluding blank lines)
@@ -5626,21 +6671,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-dateutil`
 
+### Upstream repo URL
+
+[https://github.com/dateutil/dateutil](https://github.com/dateutil/dateutil)
+
 ### Stub distribution name
 
 `types-python-dateutil`
 
 ### Number of lines
 
-440 (excluding blank lines)
+439 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5648,45 +6697,49 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 11 allowlist entries for `python-dateutil` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `python-dateutil` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `python-dateutil`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 171
-    - Unannotated parameters: 66
+    - Annotated parameters: 172
+    - Unannotated parameters: 65
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 5
 - Returns:
-    - Annotated returns: 106
-    - Unannotated returns: 48
+    - Annotated returns: 112
+    - Unannotated returns: 42
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 90
-    - Explicit `Any` variables: 13
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+    - Annotated variables: 89
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 4
 - Class definitions:
     - Total class definitions: 29
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-gflags`
 
+### Upstream repo URL
+
+[https://github.com/google/python-gflags](https://github.com/google/python-gflags)
+
 ### Stub distribution name
 
 `types-python-gflags`
 
 ### Number of lines
 
 251 (excluding blank lines)
@@ -5701,15 +6754,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `python-gflags` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `python-gflags` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `python-gflags`
 
@@ -5732,21 +6785,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-jose`
 
+### Upstream repo URL
+
+[https://github.com/mpdavis/python-jose](https://github.com/mpdavis/python-jose)
+
 ### Stub distribution name
 
 `types-python-jose`
 
 ### Number of lines
 
-356 (excluding blank lines)
+357 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5754,15 +6811,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 6 allowlist entries for `python-jose` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `python-jose` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `python-jose`
 
@@ -5785,21 +6842,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-nmap`
 
+### Upstream repo URL
+
+[https://bitbucket.org/xael/python-nmap](https://bitbucket.org/xael/python-nmap)
+
 ### Stub distribution name
 
 `types-python-nmap`
 
 ### Number of lines
 
-116 (excluding blank lines)
+119 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5807,15 +6868,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `python-nmap` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `python-nmap` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `python-nmap`
 
@@ -5838,37 +6899,41 @@
     - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-slugify`
 
+### Upstream repo URL
+
+[https://github.com/un33k/python-slugify](https://github.com/un33k/python-slugify)
+
 ### Stub distribution name
 
 `types-python-slugify`
 
 ### Number of lines
 
 45 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *obsolete*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+The runtime package has added inline type hints; these typeshed stubs are now obsolete.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `python-slugify` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `python-slugify` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `python-slugify`
 
@@ -5891,21 +6956,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `python-xlib`
 
+### Upstream repo URL
+
+[https://github.com/python-xlib/python-xlib](https://github.com/python-xlib/python-xlib)
+
 ### Stub distribution name
 
 `types-python-xlib`
 
 ### Number of lines
 
-5,385 (excluding blank lines)
+5,421 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5913,52 +6982,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 11 allowlist entries for `python-xlib` when running stubtest in CI.
+Typeshed currently has 10 unique allowlist entries for `python-xlib` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `python-xlib`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 1,332
+    - Annotated parameters: 1,334
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 15
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 581
+    - Annotated returns: 583
     - Unannotated returns: 0
     - Explicit `Any` returns: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 3,525
+    - Annotated variables: 3,519
     - Explicit `Any` variables: 5
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 425
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `pytz`
 
+### Upstream repo URL
+
+[https://github.com/stub42/pytz](https://github.com/stub42/pytz)
+
 ### Stub distribution name
 
 `types-pytz`
 
 ### Number of lines
 
-128 (excluding blank lines)
+133 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -5966,15 +7039,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 4 allowlist entries for `pytz` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `pytz` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `pytz`
 
@@ -5983,194 +7056,328 @@
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 2
 - Returns:
     - Annotated returns: 51
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 27
+    - Annotated variables: 29
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 16
     - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 3
+    - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `pyvmomi`
+## Info on typeshed's stubs for `pywin32`
+
+### Upstream repo URL
+
+[https://github.com/mhammond/pywin32](https://github.com/mhammond/pywin32)
 
 ### Stub distribution name
 
-`types-pyvmomi`
+`types-pywin32`
 
 ### Number of lines
 
-177 (excluding blank lines)
+34,801 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `win32` only.
+
+Typeshed currently has 46 unique allowlist entries for `pywin32` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `pywin32`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 3,800
+    - Unannotated parameters: 3,558
+    - Explicit `Any` parameters: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 419
+- Returns:
+    - Annotated returns: 3,865
+    - Unannotated returns: 1,987
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 288
+- Variables:
+    - Annotated variables: 25,095
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2,824
+- Class definitions:
+    - Total class definitions: 724
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `pyxdg`
+
+### Upstream repo URL
+
+[https://github.com/takluyver/pyxdg](https://github.com/takluyver/pyxdg)
+
+### Stub distribution name
+
+`types-pyxdg`
+
+### Number of lines
+
+860 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 8 allowlist entries for `pyvmomi` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `pyxdg` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `pyxdg`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 511
+    - Unannotated parameters: 1
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 2
+- Returns:
+    - Annotated returns: 297
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 165
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+- Class definitions:
+    - Total class definitions: 31
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `qrbill`
+
+### Upstream repo URL
+
+[https://github.com/claudep/swiss-qr-bill](https://github.com/claudep/swiss-qr-bill)
+
+### Stub distribution name
+
+`types-qrbill`
+
+### Number of lines
+
+172 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 2 unique allowlist entries for `qrbill` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `pyvmomi`
+### Statistics on the annotations in typeshed's stubs for `qrbill`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 50
+    - Annotated parameters: 96
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 35
+    - Annotated returns: 31
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 16
+    - Explicit `Any` returns: 4
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 57
-    - Explicit `Any` variables: 7
+    - Annotated variables: 33
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 44
+    - Total class definitions: 4
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `pywin32`
+## Info on typeshed's stubs for `qrcode`
+
+### Upstream repo URL
+
+[https://github.com/lincolnloop/python-qrcode](https://github.com/lincolnloop/python-qrcode)
 
 ### Stub distribution name
 
-`types-pywin32`
+`types-qrcode`
 
 ### Number of lines
 
-34,533 (excluding blank lines)
+524 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `win32` only.
+In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 49 allowlist entries for `pywin32` when running stubtest in CI.
+Typeshed currently has 8 unique allowlist entries for `qrcode` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `pywin32`
+### Statistics on the annotations in typeshed's stubs for `qrcode`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 3,635
-    - Unannotated parameters: 3,729
-    - Explicit `Any` parameters: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 426
+    - Annotated parameters: 109
+    - Unannotated parameters: 174
+    - Explicit `Any` parameters: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 14
 - Returns:
-    - Annotated returns: 3,825
-    - Unannotated returns: 2,043
+    - Annotated returns: 109
+    - Unannotated returns: 60
     - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 292
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 2
 - Variables:
-    - Annotated variables: 25,025
+    - Annotated variables: 166
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 2,832
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 91
 - Class definitions:
-    - Total class definitions: 724
+    - Total class definitions: 40
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `redis`
 
+### Extra description
+
+Note: Redis-py 5.0.0 added a py.typed file, but the inline annotations are incomplete. Continuing to use `types-redis` for the time being may lead to superior results.
+
+### Upstream repo URL
+
+[https://github.com/redis/redis-py](https://github.com/redis/redis-py)
+
 ### Stub distribution name
 
 `types-redis`
 
 ### Number of lines
 
-5,610 (excluding blank lines)
+6,165 (excluding blank lines)
 
-### Package status: *up to date*
+### Package status: *out of date*
 
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 68 allowlist entries for `redis` when running stubtest in CI.
+Typeshed currently has 67 unique allowlist entries for `redis` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `redis`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 3,578
-    - Unannotated parameters: 1,293
-    - Explicit `Any` parameters: 68
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 349
-- Returns:
-    - Annotated returns: 1,325
-    - Unannotated returns: 645
-    - Explicit `Any` returns: 322
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 8
+    - Annotated parameters: 3,945
+    - Unannotated parameters: 1,223
+    - Explicit `Any` parameters: 92
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 352
+- Returns:
+    - Annotated returns: 1,379
+    - Unannotated returns: 607
+    - Explicit `Any` returns: 330
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 5
 - Variables:
-    - Annotated variables: 624
-    - Explicit `Any` variables: 214
+    - Annotated variables: 618
+    - Explicit `Any` variables: 158
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 34
 - Class definitions:
-    - Total class definitions: 213
+    - Total class definitions: 215
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 2
 
 ---
 
 ## Info on typeshed's stubs for `regex`
 
+### Upstream repo URL
+
+[https://github.com/mrabarnett/mrab-regex](https://github.com/mrabarnett/mrab-regex)
+
 ### Stub distribution name
 
 `types-regex`
 
 ### Number of lines
 
-748 (excluding blank lines)
+750 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -6178,52 +7385,60 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 13 allowlist entries for `regex` when running stubtest in CI.
+Typeshed currently has 13 unique allowlist entries for `regex` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `regex`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 429
+    - Annotated parameters: 431
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 25
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 114
     - Unannotated returns: 0
     - Explicit `Any` returns: 16
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 72
+    - Annotated variables: 4
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 7
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `requests`
 
+### Extra description
+
+Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
+
+### Upstream repo URL
+
+[https://github.com/psf/requests](https://github.com/psf/requests)
+
 ### Stub distribution name
 
 `types-requests`
 
 ### Number of lines
 
-970 (excluding blank lines)
+1,001 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -6231,45 +7446,106 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 12 allowlist entries for `requests` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `requests` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `requests`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 353
-    - Unannotated parameters: 153
+    - Annotated parameters: 373
+    - Unannotated parameters: 134
     - Explicit `Any` parameters: 9
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 19
 - Returns:
-    - Annotated returns: 111
-    - Unannotated returns: 86
+    - Annotated returns: 129
+    - Unannotated returns: 69
     - Explicit `Any` returns: 5
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 114
+    - Annotated variables: 116
     - Explicit `Any` variables: 39
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 51
-    - Class definitions with `Any`: 1
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `requests-oauthlib`
+
+### Upstream repo URL
+
+[https://github.com/requests/requests-oauthlib](https://github.com/requests/requests-oauthlib)
+
+### Stub distribution name
+
+`types-requests-oauthlib`
+
+### Number of lines
+
+268 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 0 allowlist entries for `requests-oauthlib` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `requests-oauthlib`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 115
+    - Unannotated parameters: 20
+    - Explicit `Any` parameters: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 50
+- Returns:
+    - Annotated returns: 45
+    - Unannotated returns: 4
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 3
+- Variables:
+    - Annotated variables: 25
+    - Explicit `Any` variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 7
+- Class definitions:
+    - Total class definitions: 13
+    - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `retry`
 
+### Upstream repo URL
+
+[https://github.com/invl/retry](https://github.com/invl/retry)
+
 ### Stub distribution name
 
 `types-retry`
 
 ### Number of lines
 
 28 (excluding blank lines)
@@ -6284,15 +7560,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 3 allowlist entries for `retry` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `retry` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `retry`
 
@@ -6313,122 +7589,252 @@
 - Class definitions:
     - Total class definitions: 0
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `setuptools`
+## Info on typeshed's stubs for `s2clientprotocol`
+
+### Extra description
+
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 3.6.1 on [s2client-proto 5.0.12.91115.0](https://github.com/Blizzard/s2client-proto/tree/c04df4adbe274858a4eb8417175ee32ad02fd609)
+
+### Upstream repo URL
+
+[https://github.com/Blizzard/s2client-proto](https://github.com/Blizzard/s2client-proto)
 
 ### Stub distribution name
 
-`types-setuptools`
+`types-s2clientprotocol`
 
 ### Number of lines
 
-2,443 (excluding blank lines)
+5,029 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 1 unique allowlist entry for `s2clientprotocol` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `s2clientprotocol`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 856
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 676
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 1,864
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 239
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `seaborn`
+
+### Upstream repo URL
+
+[https://github.com/mwaskom/seaborn](https://github.com/mwaskom/seaborn)
+
+### Stub distribution name
+
+`types-seaborn`
+
+### Number of lines
+
+2,587 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 30 allowlist entries for `setuptools` when running stubtest in CI.
+Typeshed currently has 5 unique allowlist entries for `seaborn` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `setuptools`
+### Statistics on the annotations in typeshed's stubs for `seaborn`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 821
-    - Unannotated parameters: 390
-    - Explicit `Any` parameters: 29
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 47
+    - Annotated parameters: 1,445
+    - Unannotated parameters: 25
+    - Explicit `Any` parameters: 155
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 34
 - Returns:
-    - Annotated returns: 658
-    - Unannotated returns: 260
-    - Explicit `Any` returns: 6
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 1
+    - Annotated returns: 357
+    - Unannotated returns: 2
+    - Explicit `Any` returns: 17
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 7
 - Variables:
-    - Annotated variables: 624
-    - Explicit `Any` variables: 381
+    - Annotated variables: 282
+    - Explicit `Any` variables: 13
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 24
 - Class definitions:
-    - Total class definitions: 154
+    - Total class definitions: 100
+    - Class definitions with `Any`: 1
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `setuptools`
+
+### Upstream repo URL
+
+[https://github.com/pypa/setuptools](https://github.com/pypa/setuptools)
+
+### Stub distribution name
+
+`types-setuptools`
+
+### Number of lines
+
+3,133 (excluding blank lines)
+
+### Package status: *out of date*
+
+These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` and `win32`.
+
+Typeshed currently has 111 unique allowlist entries for `setuptools` when running stubtest in CI.
+
+### Pyright settings in CI: *strict on some files*
+
+Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
+
+### Statistics on the annotations in typeshed's stubs for `setuptools`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 1,001
+    - Unannotated parameters: 434
+    - Explicit `Any` parameters: 21
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 46
+- Returns:
+    - Annotated returns: 843
+    - Unannotated returns: 263
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 13
+- Variables:
+    - Annotated variables: 658
+    - Explicit `Any` variables: 87
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 285
+- Class definitions:
+    - Total class definitions: 187
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `simplejson`
 
+### Upstream repo URL
+
+[https://github.com/simplejson/simplejson](https://github.com/simplejson/simplejson)
+
 ### Stub distribution name
 
 `types-simplejson`
 
 ### Number of lines
 
-51 (excluding blank lines)
+277 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 14 allowlist entries for `simplejson` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `simplejson` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `simplejson`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 36
+    - Annotated parameters: 180
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 14
+    - Explicit `Any` parameters: 46
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 16
+    - Annotated returns: 24
     - Unannotated returns: 0
-    - Explicit `Any` returns: 4
+    - Explicit `Any` returns: 6
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 17
-    - Explicit `Any` variables: 0
+    - Annotated variables: 49
+    - Explicit `Any` variables: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
     - Total class definitions: 6
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `singledispatch`
 
+### Upstream repo URL
+
+[https://github.com/jaraco/singledispatch](https://github.com/jaraco/singledispatch)
+
 ### Stub distribution name
 
 `types-singledispatch`
 
 ### Number of lines
 
 27 (excluding blank lines)
@@ -6443,15 +7849,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `singledispatch` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `singledispatch` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `singledispatch`
 
@@ -6474,14 +7880,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `six`
 
+### Upstream repo URL
+
+[https://github.com/benjaminp/six](https://github.com/benjaminp/six)
+
 ### Stub distribution name
 
 `types-six`
 
 ### Number of lines
 
 335 (excluding blank lines)
@@ -6496,45 +7906,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 25 allowlist entries for `six` when running stubtest in CI.
+Typeshed currently has 25 unique allowlist entries for `six` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `six`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 71
+    - Annotated parameters: 69
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 9
+    - Explicit `Any` parameters: 8
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 40
+    - Annotated returns: 38
     - Unannotated returns: 0
     - Explicit `Any` returns: 6
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 13
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 4
+    - Total class definitions: 3
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `slumber`
 
+### Upstream repo URL
+
+[https://github.com/samgiles/slumber](https://github.com/samgiles/slumber)
+
 ### Stub distribution name
 
 `types-slumber`
 
 ### Number of lines
 
 74 (excluding blank lines)
@@ -6549,15 +7963,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `slumber` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `slumber` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `slumber`
 
@@ -6580,17 +7994,21 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for the stdlib
 
+### Upstream repo URL
+
+[https://github.com/python/cpython](https://github.com/python/cpython)
+
 ### Number of lines
 
-51,582 (excluding blank lines)
+55,793 (excluding blank lines)
 
 ### Package status: *stdlib*
 
 These are typeshed's stubs for the standard library. Typeshed's stdlib stubs are generally fairly up to date, and are tested against all currently supported Python versions in typeshed's CI.
 
 ### Upload status: *not currently uploaded*
 
@@ -6598,151 +8016,106 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `darwin`, `linux` and `win32`.
 
-Typeshed currently has 1,553 allowlist entries for the stdlib when running stubtest in CI.
+Typeshed currently has 1,620 unique allowlist entries for the stdlib when running stubtest in CI.
 
 ### Pyright settings in CI: *strict on some files*
 
 Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
 
 ### Statistics on the annotations in typeshed's stubs for the stdlib
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 24,716
-    - Unannotated parameters: 720
-    - Explicit `Any` parameters: 2,042
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 88
-- Returns:
-    - Annotated returns: 13,396
-    - Unannotated returns: 417
-    - Explicit `Any` returns: 825
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 18
+    - Annotated parameters: 26,002
+    - Unannotated parameters: 823
+    - Explicit `Any` parameters: 1,939
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 74
+- Returns:
+    - Annotated returns: 14,374
+    - Unannotated returns: 368
+    - Explicit `Any` returns: 831
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 11
 - Variables:
-    - Annotated variables: 8,120
-    - Explicit `Any` variables: 556
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 125
+    - Annotated variables: 8,255
+    - Explicit `Any` variables: 535
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 152
 - Class definitions:
-    - Total class definitions: 2,242
-    - Class definitions with `Any`: 22
+    - Total class definitions: 2,410
+    - Class definitions with `Any`: 26
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `stdlib-list`
-
-### Stub distribution name
-
-`types-stdlib-list`
-
-### Number of lines
-
-16 (excluding blank lines)
-
-### Package status: *up to date*
-
-These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *error on missing stub*
-
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 1 allowlist entry for `stdlib-list` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `stdlib-list`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 4
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 4
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 4
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 0
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
+## Info on typeshed's stubs for `stripe`
 
----
+### Upstream repo URL
 
-## Info on typeshed's stubs for `stripe`
+[https://github.com/stripe/stripe-python](https://github.com/stripe/stripe-python)
 
 ### Stub distribution name
 
 `types-stripe`
 
 ### Number of lines
 
-1,483 (excluding blank lines)
+1,532 (excluding blank lines)
 
-### Package status: *out of date*
+### Package status: *obsolete*
 
-These stubs may be out of date. In typeshed's CI, [stubtest][] tests these stubs against an older version of the runtime package than the latest that's available.
+The runtime package has added inline type hints; these typeshed stubs are now obsolete.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 6 allowlist entries for `stripe` when running stubtest in CI.
+Typeshed currently has 8 unique allowlist entries for `stripe` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `stripe`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 264
-    - Unannotated parameters: 388
+    - Annotated parameters: 270
+    - Unannotated parameters: 396
     - Explicit `Any` parameters: 5
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 156
 - Returns:
     - Annotated returns: 108
-    - Unannotated returns: 168
+    - Unannotated returns: 172
     - Explicit `Any` returns: 4
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 155
+    - Annotated variables: 157
     - Explicit `Any` variables: 42
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 134
+    - Total class definitions: 136
     - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `tabulate`
 
+### Upstream repo URL
+
+[https://github.com/astanin/python-tabulate](https://github.com/astanin/python-tabulate)
+
 ### Stub distribution name
 
 `types-tabulate`
 
 ### Number of lines
 
 60 (excluding blank lines)
@@ -6788,21 +8161,29 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `tensorflow`
 
+### Extra description
+
+Partially generated using [mypy-protobuf==3.6.0](https://github.com/nipunn1313/mypy-protobuf/tree/v3.6.0) and libprotoc 25.1 on tensorflow==2.16.1 .
+
+### Upstream repo URL
+
+[https://github.com/tensorflow/tensorflow](https://github.com/tensorflow/tensorflow)
+
 ### Stub distribution name
 
 `types-tensorflow`
 
 ### Number of lines
 
-592 (excluding blank lines)
+25,535 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -6810,97 +8191,48 @@
 
 ### Stubtest settings in CI: *missing stubs ignored*
 
 The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 14 allowlist entries for `tensorflow` when running stubtest in CI.
+Typeshed currently has 51 unique allowlist entries for `tensorflow` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `tensorflow`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 393
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
+    - Annotated parameters: 5,324
+    - Unannotated parameters: 8
+    - Explicit `Any` parameters: 60
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 23
 - Returns:
-    - Annotated returns: 227
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 2
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 13
+    - Annotated returns: 3,033
+    - Unannotated returns: 4
+    - Explicit `Any` returns: 34
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 58
 - Variables:
-    - Annotated variables: 24
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+    - Annotated variables: 5,294
+    - Explicit `Any` variables: 5
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 7
 - Class definitions:
-    - Total class definitions: 13
-    - Class definitions with `Any`: 0
+    - Total class definitions: 928
+    - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `termcolor`
-
-### Stub distribution name
-
-`types-termcolor`
-
-### Number of lines
-
-12 (excluding blank lines)
-
-### Package status: *obsolete*
-
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
-
-### Upload status: *uploaded*
-
-These stubs are currently uploaded to PyPI.
-
-### Stubtest settings in CI: *error on missing stub*
-
-Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
-
-In CI, stubtest is run on `linux` only.
-
-Typeshed currently has 0 allowlist entries for `termcolor` when running stubtest in CI.
-
-### Pyright settings in CI: *strict*
-
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
-
-### Statistics on the annotations in typeshed's stubs for `termcolor`
-
-- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 9
-    - Unannotated parameters: 0
-    - Explicit `Any` parameters: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
-- Returns:
-    - Annotated returns: 2
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
-- Variables:
-    - Annotated variables: 6
-    - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
-- Class definitions:
-    - Total class definitions: 0
-    - Class definitions with `Any`: 0
-    - Class definitions marked as at least partially `Incomplete`: 0
+## Info on typeshed's stubs for `toml`
 
----
+### Upstream repo URL
 
-## Info on typeshed's stubs for `toml`
+[https://github.com/uiri/toml](https://github.com/uiri/toml)
 
 ### Stub distribution name
 
 `types-toml`
 
 ### Number of lines
 
@@ -6916,15 +8248,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `toml` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `toml` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `toml`
 
@@ -6947,14 +8279,18 @@
     - Class definitions with `Any`: 2
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `toposort`
 
+### Upstream repo URL
+
+[https://gitlab.com/ericvsmith/toposort](https://gitlab.com/ericvsmith/toposort)
+
 ### Stub distribution name
 
 `types-toposort`
 
 ### Number of lines
 
 13 (excluding blank lines)
@@ -7000,21 +8336,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `tqdm`
 
+### Upstream repo URL
+
+[https://github.com/tqdm/tqdm](https://github.com/tqdm/tqdm)
+
 ### Stub distribution name
 
 `types-tqdm`
 
 ### Number of lines
 
-1,377 (excluding blank lines)
+1,379 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7022,52 +8362,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `tqdm` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `tqdm` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `tqdm`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 812
-    - Unannotated parameters: 142
+    - Annotated parameters: 811
+    - Unannotated parameters: 146
     - Explicit `Any` parameters: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 42
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 38
 - Returns:
-    - Annotated returns: 167
-    - Unannotated returns: 24
+    - Annotated returns: 164
+    - Unannotated returns: 27
     - Explicit `Any` returns: 1
-    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 11
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 8
 - Variables:
     - Annotated variables: 100
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 74
 - Class definitions:
     - Total class definitions: 36
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `tree-sitter`
+## Info on typeshed's stubs for `translationstring`
+
+### Upstream repo URL
+
+[https://github.com/Pylons/translationstring](https://github.com/Pylons/translationstring)
 
 ### Stub distribution name
 
-`types-tree-sitter`
+`types-translationstring`
 
 ### Number of lines
 
-124 (excluding blank lines)
+73 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7075,15 +8419,72 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 36 allowlist entries for `tree-sitter` when running stubtest in CI.
+Typeshed currently has 4 unique allowlist entries for `translationstring` when running stubtest in CI.
+
+### Pyright settings in CI: *strict*
+
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+
+### Statistics on the annotations in typeshed's stubs for `translationstring`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 62
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 6
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+- Returns:
+    - Annotated returns: 18
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
+- Variables:
+    - Annotated variables: 4
+    - Explicit `Any` variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
+- Class definitions:
+    - Total class definitions: 7
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `tree-sitter`
+
+### Upstream repo URL
+
+[https://github.com/tree-sitter/py-tree-sitter](https://github.com/tree-sitter/py-tree-sitter)
+
+### Stub distribution name
+
+`types-tree-sitter`
+
+### Number of lines
+
+123 (excluding blank lines)
+
+### Package status: *obsolete*
+
+The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 36 unique allowlist entries for `tree-sitter` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `tree-sitter`
 
@@ -7106,14 +8507,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `tree-sitter-languages`
 
+### Upstream repo URL
+
+[https://github.com/grantjenks/py-tree-sitter-languages](https://github.com/grantjenks/py-tree-sitter-languages)
+
 ### Stub distribution name
 
 `types-tree-sitter-languages`
 
 ### Number of lines
 
 9 (excluding blank lines)
@@ -7128,15 +8533,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 3 allowlist entries for `tree-sitter-languages` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `tree-sitter-languages` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `tree-sitter-languages`
 
@@ -7159,14 +8564,18 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `ttkthemes`
 
+### Upstream repo URL
+
+[https://github.com/RedFantom/ttkthemes](https://github.com/RedFantom/ttkthemes)
+
 ### Stub distribution name
 
 `types-ttkthemes`
 
 ### Number of lines
 
 76 (excluding blank lines)
@@ -7210,76 +8619,88 @@
 - Class definitions:
     - Total class definitions: 3
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `typed-ast`
+## Info on typeshed's stubs for `uWSGI`
+
+### Extra description
+
+Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
+
+### Upstream repo URL
+
+[https://github.com/unbit/uwsgi](https://github.com/unbit/uwsgi)
 
 ### Stub distribution name
 
-`types-typed-ast`
+`types-uWSGI`
 
 ### Number of lines
 
-578 (excluding blank lines)
+381 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
-In CI, stubtest is run on `linux` only.
+In CI, stubtest is run on `darwin` and `linux`.
 
-Typeshed currently has 0 allowlist entries for `typed-ast` when running stubtest in CI.
+Typeshed currently has 9 unique allowlist entries for `uWSGI` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `typed-ast`
+### Statistics on the annotations in typeshed's stubs for `uWSGI`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 46
+    - Annotated parameters: 338
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 4
+    - Explicit `Any` parameters: 15
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 29
+    - Annotated returns: 216
     - Unannotated returns: 0
-    - Explicit `Any` returns: 6
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 309
-    - Explicit `Any` variables: 1
+    - Annotated variables: 61
+    - Explicit `Any` variables: 5
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 223
+    - Total class definitions: 26
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `tzlocal`
+## Info on typeshed's stubs for `ujson`
+
+### Upstream repo URL
+
+[https://github.com/ultrajson/ultrajson](https://github.com/ultrajson/ultrajson)
 
 ### Stub distribution name
 
-`types-tzlocal`
+`types-ujson`
 
 ### Number of lines
 
-19 (excluding blank lines)
+49 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7287,52 +8708,56 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 2 allowlist entries for `tzlocal` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `ujson` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `tzlocal`
+### Statistics on the annotations in typeshed's stubs for `ujson`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 2
+    - Annotated parameters: 40
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
+    - Explicit `Any` parameters: 3
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 3
 - Returns:
     - Annotated returns: 6
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Explicit `Any` returns: 3
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 3
+    - Annotated variables: 1
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 2
+    - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `ujson`
+## Info on typeshed's stubs for `unidiff`
+
+### Upstream repo URL
+
+[https://github.com/matiasb/python-unidiff](https://github.com/matiasb/python-unidiff)
 
 ### Stub distribution name
 
-`types-ujson`
+`types-unidiff`
 
 ### Number of lines
 
-34 (excluding blank lines)
+144 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7340,45 +8765,49 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `ujson` when running stubtest in CI.
+Typeshed currently has 6 unique allowlist entries for `unidiff` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `ujson`
+### Statistics on the annotations in typeshed's stubs for `unidiff`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 28
+    - Annotated parameters: 34
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 3
+    - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 6
+    - Annotated returns: 32
     - Unannotated returns: 0
-    - Explicit `Any` returns: 3
+    - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 1
+    - Annotated variables: 38
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 6
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `untangle`
 
+### Upstream repo URL
+
+[https://github.com/stchris/untangle](https://github.com/stchris/untangle)
+
 ### Stub distribution name
 
 `types-untangle`
 
 ### Number of lines
 
 33 (excluding blank lines)
@@ -7404,15 +8833,15 @@
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `untangle`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 19
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 2
+    - Explicit `Any` parameters: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
     - Annotated returns: 21
     - Unannotated returns: 0
     - Explicit `Any` returns: 2
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
@@ -7422,76 +8851,84 @@
 - Class definitions:
     - Total class definitions: 2
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `urllib3`
+## Info on typeshed's stubs for `usersettings`
+
+### Upstream repo URL
+
+[https://github.com/glvnst/usersettings](https://github.com/glvnst/usersettings)
 
 ### Stub distribution name
 
-`types-urllib3`
+`types-usersettings`
 
 ### Number of lines
 
-696 (excluding blank lines)
+12 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 30 allowlist entries for `urllib3` when running stubtest in CI.
+Typeshed currently has 3 unique allowlist entries for `usersettings` when running stubtest in CI.
 
-### Pyright settings in CI: *not strict*
+### Pyright settings in CI: *strict*
 
-This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `urllib3`
+### Statistics on the annotations in typeshed's stubs for `usersettings`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 158
-    - Unannotated parameters: 160
-    - Explicit `Any` parameters: 3
+    - Annotated parameters: 7
+    - Unannotated parameters: 0
+    - Explicit `Any` parameters: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 95
-    - Unannotated returns: 61
-    - Explicit `Any` returns: 4
+    - Annotated returns: 6
+    - Unannotated returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 155
-    - Explicit `Any` variables: 54
+    - Annotated variables: 3
+    - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 72
+    - Total class definitions: 1
     - Class definitions with `Any`: 1
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `vobject`
 
+### Upstream repo URL
+
+[https://github.com/eventable/vobject](https://github.com/eventable/vobject)
+
 ### Stub distribution name
 
 `types-vobject`
 
 ### Number of lines
 
-525 (excluding blank lines)
+522 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7499,15 +8936,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 11 allowlist entries for `vobject` when running stubtest in CI.
+Typeshed currently has 11 unique allowlist entries for `vobject` when running stubtest in CI.
 
 ### Pyright settings in CI: *not strict*
 
 This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
 ### Statistics on the annotations in typeshed's stubs for `vobject`
 
@@ -7530,67 +8967,75 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `waitress`
 
+### Upstream repo URL
+
+[https://github.com/Pylons/waitress](https://github.com/Pylons/waitress)
+
 ### Stub distribution name
 
 `types-waitress`
 
 ### Number of lines
 
-630 (excluding blank lines)
+651 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
-### Stubtest settings in CI: *missing stubs ignored*
+### Stubtest settings in CI: *error on missing stub*
 
-The `--ignore-missing-stub` stubtest setting is used in typeshed's CI.
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` and `win32`.
 
-Typeshed currently has 38 allowlist entries for `waitress` when running stubtest in CI.
+Typeshed currently has 2 unique allowlist entries for `waitress` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `waitress`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 210
+    - Annotated parameters: 203
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 35
-    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 9
+    - Explicit `Any` parameters: 2
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 209
+    - Annotated returns: 205
     - Unannotated returns: 0
-    - Explicit `Any` returns: 8
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 246
-    - Explicit `Any` variables: 19
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 40
+    - Total class definitions: 39
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `whatthepatch`
 
+### Upstream repo URL
+
+[https://github.com/cscorley/whatthepatch](https://github.com/cscorley/whatthepatch)
+
 ### Stub distribution name
 
 `types-whatthepatch`
 
 ### Number of lines
 
 101 (excluding blank lines)
@@ -7634,23 +9079,27 @@
 - Class definitions:
     - Total class definitions: 9
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `xmltodict`
+## Info on typeshed's stubs for `workalendar`
+
+### Upstream repo URL
+
+[https://github.com/workalendar/workalendar](https://github.com/workalendar/workalendar)
 
 ### Stub distribution name
 
-`types-xmltodict`
+`types-workalendar`
 
 ### Number of lines
 
-35 (excluding blank lines)
+2,918 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7658,105 +9107,170 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `xmltodict` when running stubtest in CI.
+Typeshed currently has 5 unique allowlist entries for `workalendar` when running stubtest in CI.
 
-### Pyright settings in CI: *strict*
+### Pyright settings in CI: *not strict*
 
-All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
 
-### Statistics on the annotations in typeshed's stubs for `xmltodict`
+### Statistics on the annotations in typeshed's stubs for `workalendar`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 20
+    - Annotated parameters: 44
+    - Unannotated parameters: 399
+    - Explicit `Any` parameters: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 23
+- Returns:
+    - Annotated returns: 22
+    - Unannotated returns: 355
+    - Explicit `Any` returns: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) returns: 4
+- Variables:
+    - Annotated variables: 1,367
+    - Explicit `Any` variables: 0
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 249
+- Class definitions:
+    - Total class definitions: 374
+    - Class definitions with `Any`: 0
+    - Class definitions marked as at least partially `Incomplete`: 0
+
+---
+
+## Info on typeshed's stubs for `wurlitzer`
+
+### Upstream repo URL
+
+[https://github.com/minrk/wurlitzer](https://github.com/minrk/wurlitzer)
+
+### Stub distribution name
+
+`types-wurlitzer`
+
+### Number of lines
+
+130 (excluding blank lines)
+
+### Package status: *up to date*
+
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
+
+### Upload status: *uploaded*
+
+These stubs are currently uploaded to PyPI.
+
+### Stubtest settings in CI: *error on missing stub*
+
+Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
+
+In CI, stubtest is run on `linux` only.
+
+Typeshed currently has 0 allowlist entries for `wurlitzer` when running stubtest in CI.
+
+### Pyright settings in CI: *not strict*
+
+This package is tested with pyright in typeshed's CI, but all files in this stubs package are excluded from the stricter pyright settings.
+
+### Statistics on the annotations in typeshed's stubs for `wurlitzer`
+
+- Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
+    - Annotated parameters: 95
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 7
+    - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 3
-    - Unannotated returns: 0
-    - Explicit `Any` returns: 1
+    - Annotated returns: 32
+    - Unannotated returns: 1
+    - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 1
+    - Annotated variables: 7
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 1
+    - Total class definitions: 3
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
-## Info on typeshed's stubs for `xxhash`
+## Info on typeshed's stubs for `xmltodict`
+
+### Upstream repo URL
+
+[https://github.com/martinblech/xmltodict](https://github.com/martinblech/xmltodict)
 
 ### Stub distribution name
 
-`types-xxhash`
+`types-xmltodict`
 
 ### Number of lines
 
-43 (excluding blank lines)
+35 (excluding blank lines)
 
-### Package status: *obsolete*
+### Package status: *up to date*
 
-The runtime package has added inline type hints; these typeshed stubs are now obsolete.
+These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
 These stubs are currently uploaded to PyPI.
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 0 allowlist entries for `xxhash` when running stubtest in CI.
+Typeshed currently has 0 allowlist entries for `xmltodict` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
-### Statistics on the annotations in typeshed's stubs for `xxhash`
+### Statistics on the annotations in typeshed's stubs for `xmltodict`
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
-    - Annotated parameters: 26
+    - Annotated parameters: 20
     - Unannotated parameters: 0
-    - Explicit `Any` parameters: 0
+    - Explicit `Any` parameters: 7
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 17
+    - Annotated returns: 3
     - Unannotated returns: 0
-    - Explicit `Any` returns: 0
+    - Explicit `Any` returns: 1
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
-    - Annotated variables: 6
+    - Annotated variables: 1
     - Explicit `Any` variables: 0
-    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 1
+    - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
 - Class definitions:
-    - Total class definitions: 5
+    - Total class definitions: 1
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `zstd`
 
+### Upstream repo URL
+
+[https://github.com/sergey-dryabzhinsky/python-zstd](https://github.com/sergey-dryabzhinsky/python-zstd)
+
 ### Stub distribution name
 
 `types-zstd`
 
 ### Number of lines
 
-13 (excluding blank lines)
+15 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7778,15 +9292,15 @@
 
 - Parameters (excluding `self`, `cls`, `metacls` and `mcls`):
     - Annotated parameters: 13
     - Unannotated parameters: 0
     - Explicit `Any` parameters: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) parameters: 0
 - Returns:
-    - Annotated returns: 11
+    - Annotated returns: 13
     - Unannotated returns: 0
     - Explicit `Any` returns: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) returns: 0
 - Variables:
     - Annotated variables: 0
     - Explicit `Any` variables: 0
     - Explicitly `Incomplete` (or partially `Incomplete`) variables: 0
@@ -7795,21 +9309,25 @@
     - Class definitions with `Any`: 0
     - Class definitions marked as at least partially `Incomplete`: 0
 
 ---
 
 ## Info on typeshed's stubs for `zxcvbn`
 
+### Upstream repo URL
+
+[https://github.com/dwolfhub/zxcvbn-python](https://github.com/dwolfhub/zxcvbn-python)
+
 ### Stub distribution name
 
 `types-zxcvbn`
 
 ### Number of lines
 
-162 (excluding blank lines)
+164 (excluding blank lines)
 
 ### Package status: *up to date*
 
 These stubs should be fairly up to date. In typeshed's CI, [stubtest][] tests these stubs against the latest version of the runtime package that's available.
 
 ### Upload status: *uploaded*
 
@@ -7817,15 +9335,15 @@
 
 ### Stubtest settings in CI: *error on missing stub*
 
 Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
 
 In CI, stubtest is run on `linux` only.
 
-Typeshed currently has 1 allowlist entry for `zxcvbn` when running stubtest in CI.
+Typeshed currently has 1 unique allowlist entry for `zxcvbn` when running stubtest in CI.
 
 ### Pyright settings in CI: *strict*
 
 All files in this stubs package are tested with the stricter pyright settings in typeshed's CI.
 
 ### Statistics on the annotations in typeshed's stubs for `zxcvbn`
```

### Comparing `typeshed_stats-23.2.1/scripts/regenerate.py` & `typeshed_stats-24.5.21/scripts/regenerate.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,25 +27,25 @@
     for path, formatted_stats in path_to_formatted_stats.items():
         newline = "" if Path(path).suffix == ".csv" else None
         with open(path, "w", encoding="utf-8", newline=newline) as f:
             f.write(formatted_stats)
     print("Examples successfully regenerated!")
 
 
-# I think we need the type: ignore here
-# because mypy is worried that ExitStack() might suppress exceptions.
-# I guess that's reasonable, thought it's somewhat annoying in this case.
-def get_stats(args: argparse.Namespace) -> Sequence[PackageInfo]:  # type: ignore[return]
+def get_stats(args: argparse.Namespace) -> Sequence[PackageInfo]:
     """Get the stats."""
+    stats: Sequence[PackageInfo] | None = None
     with ExitStack() as stack:
         if args.download_typeshed:
             print("Cloning typeshed into a temporary directory...")
             args.typeshed_dir = stack.enter_context(tmpdir_typeshed())
         print("Gathering stats...")
-        return gather_stats_on_multiple_packages(typeshed_dir=args.typeshed_dir)
+        stats = gather_stats_on_multiple_packages(typeshed_dir=args.typeshed_dir)
+    assert stats is not None
+    return stats
 
 
 def get_argument_parser() -> argparse.ArgumentParser:
     """Get the argument parser."""
     parser = argparse.ArgumentParser("Script to regenerate examples")
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument("-t", "--typeshed-dir", type=Path)
```

### Comparing `typeshed_stats-23.2.1/scripts/runtests.py` & `typeshed_stats-24.5.21/scripts/runtests.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,79 +11,60 @@
 
 @overload
 def run_checks(
     *,
     regenerate_examples: Literal[True],
     typeshed_dir: Path,
     download_typeshed: Literal[False] = ...,
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def run_checks(
     *,
     regenerate_examples: Literal[True],
     download_typeshed: Literal[True],
     typeshed_dir: None = ...,
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def run_checks(
     *,
     regenerate_examples: Literal[False],
     download_typeshed: Literal[False] = ...,
     typeshed_dir: None = ...,
-) -> None:
-    ...
+) -> None: ...
 
 
 @overload
 def run_checks(
     *,
     regenerate_examples: bool = ...,
     typeshed_dir: Path | None = ...,
     download_typeshed: bool = ...,
-) -> None:
-    ...
+) -> None: ...
 
 
 def run_checks(
     *,
     regenerate_examples: bool = False,
     typeshed_dir: Path | None = None,
     download_typeshed: bool = False,
 ) -> None:
     """Run the checks."""
-    print("Running requirements-txt-fixer...")
-    subprocess.run(["requirements-txt-fixer", *Path("requirements").glob("*.txt")])
-
-    print("\nRunning pycln...")
-    subprocess.run(["pycln", ".", "--config=pyproject.toml"])
+    print("\nRunning ruff...")
+    subprocess.run(["ruff", "check", "."])
 
-    print("\nRunning pyupgrade...")
-    pyupgrade_files = [
-        path for path in Path(".").rglob("*.py") if Path("env") not in path.parents
-    ]
-    subprocess.run(["pyupgrade", *pyupgrade_files])
-
-    print("\nRunning isort...")
-    subprocess.run(["isort", *FILES_TO_CHECK])
-
-    print("\nRunning black...")
-    black_result = subprocess.run(["black", "."])
-    if black_result.returncode == 123:
-        print("Exiting early since black failed!")
+    print("\nRunning ruff formatter...")
+    ruff_format_result = subprocess.run(["ruff", "format", "."])
+    if ruff_format_result.returncode == 123:
+        print("Exiting early since `ruff format` failed!")
         raise SystemExit(1)
 
-    print("\nRunning flake8...")
-    subprocess.run(["flake8", *FILES_TO_CHECK], check=True)
-
     print("\nRunning mypy...")
     subprocess.run(["mypy"], check=True)
 
     print("\nRunning pytest...")
     for command in "coverage run -m pytest", "coverage report":
         subprocess.run(command.split(), check=True)
```

### Comparing `typeshed_stats-23.2.1/src/typeshed_stats/_cli.py` & `typeshed_stats-24.5.21/src/typeshed_stats/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     PackageInfo,
     PackageName,
     gather_stats_on_multiple_packages,
     tmpdir_typeshed,
 )
 from typeshed_stats.serialize import stats_to_csv, stats_to_json, stats_to_markdown
 
-__all__ = ["OutputOption", "SUPPORTED_EXTENSIONS", "main"]
+__all__ = ["SUPPORTED_EXTENSIONS", "OutputOption", "main"]
 
 
 def _format_stats_for_pprinting(
     stats: Sequence[PackageInfo],
 ) -> dict[PackageName, PackageInfo]:
     # *Don't* stringify this one
     # It makes it harder for pprint or rich to format it nicely
@@ -97,26 +97,24 @@
 _LoggingLevels: TypeAlias = Literal[
     "NOTSET", "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"
 ]
 
 
 def _get_help_formatter() -> type[argparse.HelpFormatter]:
     try:
-        import rich  # noqa: F401
+        import rich  # noqa: F401  # pyright: ignore[reportUnusedImport]
         from rich_argparse import RichHelpFormatter as HelpFormatter
     except ImportError:
         from argparse import HelpFormatter  # type: ignore[assignment]
     else:
-        HelpFormatter.styles.update(
-            {
-                "argparse.groups": "gold3",
-                "argparse.args": "navajo_white1",
-                "argparse.metavar": "dark_orange3",
-            }
-        )
+        HelpFormatter.styles.update({
+            "argparse.groups": "gold3",
+            "argparse.args": "navajo_white1",
+            "argparse.metavar": "dark_orange3",
+        })
         HelpFormatter.group_name_formatter = str.title
     return HelpFormatter
 
 
 def _get_argument_parser() -> argparse.ArgumentParser:
     """Parse arguments and do basic argument validation.
 
@@ -311,18 +309,18 @@
             _validate_packages(packages, typeshed_dir, parser=parser)
 
         output_option = _determine_output_option(args, parser=parser)
 
         logger.info("Gathering stats...")
         stats = gather_stats_on_multiple_packages(packages, typeshed_dir=typeshed_dir)
 
-    logger.info("Formatting stats...")
-    formatted_stats = output_option.convert(stats)
-    logger.info("Writing stats...")
-    _write_stats(formatted_stats, args.writefile, logger)
+        logger.info("Formatting stats...")
+        formatted_stats = output_option.convert(stats)
+        logger.info("Writing stats...")
+        _write_stats(formatted_stats, args.writefile, logger)
 
 
 def main(argv: Sequence[str] | None = None) -> None:
     """CLI entry point."""
     try:
         _run(argv)
     except KeyboardInterrupt:
```

### Comparing `typeshed_stats-23.2.1/src/typeshed_stats/_markdown_template.md.jinja` & `typeshed_stats-24.5.21/src/typeshed_stats/_markdown_template.md.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,20 @@
 
 {% if extra_description %}
 ### Extra description
 
 {{ extra_description }}
 {% endif %}
 
+{% if upstream_url %}
+### Upstream repo URL
+
+[{{ upstream_url }}]({{ upstream_url }})
+{% endif %}
+
 {% if stub_distribution_name != "-" %}
 ### Stub distribution name
 
 `{{ stub_distribution_name }}`
 {% endif %}
 
 ### Number of lines
@@ -50,17 +56,21 @@
 {% elif num_platforms == 2 %}
 In CI, stubtest is run on `{{ stubtest_platforms[0] }}` and `{{ stubtest_platforms[1] }}`.
 {% else %}
 In CI, stubtest is run on `{{ stubtest_platforms[0] }}`, `{{ stubtest_platforms[1] }}` and `{{ stubtest_platforms[2] }}`.
 {% endif %}
 {% endif %}
 
-Typeshed currently has {{ stubtest_allowlist_length }} allowlist
-{{- " entry " if stubtest_allowlist_length == "1" else " entries " -}}
-for {{ package_name }} when running stubtest in CI.
+{% if stubtest_allowlist_length == "0" %}
+Typeshed currently has 0 allowlist entries for {{ package_name }} when running stubtest in CI.
+{% elif stubtest_allowlist_length == "1" %}
+Typeshed currently has 1 unique allowlist entry for {{ package_name }} when running stubtest in CI.
+{% else %}
+Typeshed currently has {{ stubtest_allowlist_length }} unique allowlist entries for {{ package_name }} when running stubtest in CI.
+{% endif %}
 
 ### Pyright settings in CI: *{{ pyright_setting.formatted_name }}*
 
 {{ pyright_setting.value }}
 
 ### Statistics on the annotations in typeshed's stubs for {{ package_name }}
```

### Comparing `typeshed_stats-23.2.1/src/typeshed_stats/gather.py` & `typeshed_stats-24.5.21/src/typeshed_stats/gather.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,57 +11,72 @@
 from collections.abc import Collection, Container, Iterable, Iterator, Mapping, Sequence
 from contextlib import AsyncExitStack, contextmanager
 from enum import Enum
 from functools import lru_cache, partial
 from itertools import chain
 from operator import attrgetter
 from pathlib import Path
-from typing import Annotated, Any, Literal, NewType, TypeAlias, TypeVar, final
+from typing import (
+    Annotated,
+    Any,
+    Literal,
+    NamedTuple,
+    NewType,
+    TypeAlias,
+    TypeGuard,
+    TypeVar,
+    final,
+)
 
 import aiohttp
 import attrs
 from packaging.specifiers import SpecifierSet
 from packaging.version import Version
+from pathspec import PathSpec
+from pathspec.patterns.gitwildmatch import GitWildMatchPattern
 
-if sys.version_info < (3, 10):
+if sys.version_info < (3, 10):  # noqa: UP036
     raise ImportError("Python 3.10+ is required!")
 
 if sys.version_info >= (3, 11):
     import tomllib  # pragma: >=3.11 cover
 else:
     import tomli as tomllib  # pragma: <3.11 cover
 
 
 __all__ = [
     "AnnotationStats",
+    "CompletenessLevel",
     "FileInfo",
     "PackageInfo",
     "PackageName",
     "PackageStatus",
     "PyrightSetting",
     "StubtestSettings",
     "StubtestStrictness",
     "UploadStatus",
     "gather_annotation_stats_on_file",
     "gather_annotation_stats_on_package",
     "gather_stats_on_file",
     "gather_stats_on_multiple_packages",
     "gather_stats_on_package",
+    "get_completeness_level",
     "get_number_of_lines_of_file",
     "get_package_extra_description",
     "get_package_size",
     "get_package_status",
     "get_pyright_setting_for_package",
     "get_pyright_setting_for_path",
     "get_stub_distribution_name",
     "get_stubtest_allowlist_length",
     "get_stubtest_platforms",
     "get_stubtest_settings",
     "get_stubtest_strictness",
     "get_upload_status",
+    "get_upstream_url",
     "tmpdir_typeshed",
 ]
 
 PackageName: TypeAlias = str
 _AbsolutePath = NewType("_AbsolutePath", Path)
 _PathRelativeToTypeshed: TypeAlias = Path
 _NiceReprEnumSelf = TypeVar("_NiceReprEnumSelf", bound="_NiceReprEnum")
@@ -280,18 +295,22 @@
         path: The location of the file to be analysed.
 
     Returns:
         An [`AnnotationStats`](./#AnnotationStats) object
             containing data about the annotations in the file.
 
     Examples:
-        >>> from typeshed_stats.gather import tmpdir_typeshed, gather_annotation_stats_on_file
+        >>> from typeshed_stats.gather import (
+        ...     tmpdir_typeshed,
+        ...     gather_annotation_stats_on_file,
+        ... )
         >>> with tmpdir_typeshed() as typeshed:
-        ...     stats_on_functools = gather_annotation_stats_on_file(typeshed / "stdlib" / "functools.pyi")
-        ...
+        ...     stats_on_functools = gather_annotation_stats_on_file(
+        ...         typeshed / "stdlib" / "functools.pyi"
+        ...     )
         >>> type(stats_on_functools)
         <class 'typeshed_stats.gather.AnnotationStats'>
         >>> stats_on_functools.unannotated_parameters
         0
     """
     visitor = _AnnotationStatsCollector()
     with open(path, encoding="utf-8") as file:
@@ -317,18 +336,22 @@
             in which to find the stubs package source.
 
     Returns:
         An [`AnnotationStats`](./#AnnotationStats) object
             containing data about the annotations in the package.
 
     Examples:
-        >>> from typeshed_stats.gather import tmpdir_typeshed, gather_annotation_stats_on_package
+        >>> from typeshed_stats.gather import (
+        ...     tmpdir_typeshed,
+        ...     gather_annotation_stats_on_package,
+        ... )
         >>> with tmpdir_typeshed() as typeshed:
-        ...     mypy_extensions_stats = gather_annotation_stats_on_package("mypy-extensions", typeshed_dir=typeshed)
-        ...
+        ...     mypy_extensions_stats = gather_annotation_stats_on_package(
+        ...         "mypy-extensions", typeshed_dir=typeshed
+        ...     )
         >>> type(mypy_extensions_stats)
         <class 'typeshed_stats.gather.AnnotationStats'>
         >>> mypy_extensions_stats.unannotated_parameters
         0
     """
     combined: Counter[str] = Counter()
     annot_stats_fields = AnnotationStats.__annotations__
@@ -364,16 +387,20 @@
     Returns:
         The "extra description" of the package given in the `METADATA.toml` file,
             if one is given, else [None][].
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_package_extra_description
         >>> with tmpdir_typeshed() as typeshed:
-        ...     stdlib_description = get_package_extra_description("stdlib", typeshed_dir=typeshed)
-        ...     protobuf_description = get_package_extra_description("protobuf", typeshed_dir=typeshed)
+        ...     stdlib_description = get_package_extra_description(
+        ...         "stdlib", typeshed_dir=typeshed
+        ...     )
+        ...     protobuf_description = get_package_extra_description(
+        ...         "protobuf", typeshed_dir=typeshed
+        ...     )
         >>> stdlib_description is None
         True
         >>> isinstance(protobuf_description, str)
         True
     """
     if package_name == "stdlib":
         return None
@@ -394,15 +421,15 @@
 
 
 @lru_cache
 def _get_stubtest_config(
     package_name: PackageName, typeshed_dir: Path | str
 ) -> Mapping[str, object]:
     metadata = _get_package_metadata(package_name, typeshed_dir)
-    config = metadata.get("tool", {}).get("stubtest", {})
+    config: object = metadata.get("tool", {}).get("stubtest", {})
     assert isinstance(config, dict)
     return config
 
 
 def get_stubtest_strictness(
     package_name: PackageName, *, typeshed_dir: Path | str
 ) -> StubtestStrictness:
@@ -417,15 +444,15 @@
         A member of the [`StubtestStrictness`](./#StubtestStrictness)
             enumeration (see the docs on `StubtestStrictness` for details).
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_stubtest_strictness
         >>> with tmpdir_typeshed() as typeshed:
         ...     stdlib_setting = get_stubtest_strictness("stdlib", typeshed_dir=typeshed)
-        ...     gdb_setting = get_stubtest_strictness("gdb", typeshed_dir=typeshed)
+        ...     gdb_setting = get_stubtest_strictness("RPi.GPIO", typeshed_dir=typeshed)
         >>> stdlib_setting
         StubtestStrictness.ERROR_ON_MISSING_STUB
         >>> help(_)
         Help on StubtestStrictness in module typeshed_stats.gather:
         <BLANKLINE>
         StubtestStrictness.ERROR_ON_MISSING_STUB
             Objects missing from the stub cause stubtest to emit an error in typeshed's CI.
@@ -473,62 +500,68 @@
             return []
         case {"platforms": list() as platforms}:
             return sorted(platforms)
         case _:
             return ["linux"]
 
 
-def _num_allowlist_entries_in_file(path: Path) -> int:
+def _allowlist_entries_in_file(path: Path) -> set[str]:
     with path.open(encoding="utf-8") as file:
-        return sum(
-            1 for line in file if line.strip() and not line.strip().startswith("#")
-        )
+        return {line.split("#")[0].strip() for line in file} - {""}
 
 
 def get_stubtest_allowlist_length(
     package_name: PackageName, *, typeshed_dir: Path | str
 ) -> int:
-    """Get the number of "allowlist entries" typeshed uses in CI when [stubtest][] is run on a certain package.
+    """Get the number of unique "allowlist entries" typeshed uses in CI when [stubtest][] is run on a certain package.
 
     An allowlist entry indicates a place in the stub where stubtest emits an error,
     but typeshed has chosen to silence the error rather than "fix it".
     Not all allowlist entries are bad:
     sometimes there are good reasons to ignore an error emitted by stubtest.
 
     Parameters:
         package_name: The name of the package
             to find the number of allowlist entries for.
         typeshed_dir: A path pointing to a typeshed directory,
             from which to retrieve the number of stubtest allowlist entries.
 
     Returns:
         The number of allowlist entries for that package.
+        Duplicate entries in allowlists are removed.
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_stubtest_allowlist_length
         >>> with tmpdir_typeshed() as typeshed:
-        ...     num_stdlib_allows = get_stubtest_allowlist_length("stdlib", typeshed_dir=typeshed)
-        ...     num_requests_allows = get_stubtest_allowlist_length("requests", typeshed_dir=typeshed)
+        ...     num_stdlib_allows = get_stubtest_allowlist_length(
+        ...         "stdlib", typeshed_dir=typeshed
+        ...     )
+        ...     num_requests_allows = get_stubtest_allowlist_length(
+        ...         "requests", typeshed_dir=typeshed
+        ...     )
         >>> type(num_stdlib_allows)
         <class 'int'>
         >>> num_stdlib_allows > 0 and num_requests_allows > 0
         True
     """
     if package_name == "stdlib":
-        allowlist_dir = Path(typeshed_dir, "tests", "stubtest_allowlists")
-        return sum(
-            _num_allowlist_entries_in_file(file) for file in allowlist_dir.glob("*.txt")
+        allowlist_dir = Path(typeshed_dir, "stdlib", "@tests", "stubtest_allowlists")
+        combined_allowlist = chain.from_iterable(
+            _allowlist_entries_in_file(file) for file in allowlist_dir.glob("*.txt")
         )
-    allowlist_dir = Path(typeshed_dir, "stubs", package_name, "@tests")
-    if not allowlist_dir.exists():
-        return 0
-    return sum(
-        _num_allowlist_entries_in_file(file)
-        for file in allowlist_dir.glob("stubtest_allowlist*.txt")
-    )
+    else:
+        allowlist_dir = Path(typeshed_dir, "stubs", package_name, "@tests")
+        if not allowlist_dir.exists():
+            return 0
+        combined_allowlist = chain.from_iterable(
+            _allowlist_entries_in_file(file)
+            for file in allowlist_dir.glob("stubtest_allowlist*.txt")
+        )
+    deduplicated_allowlist = set(combined_allowlist)
+    return len(deduplicated_allowlist)
 
 
 @final
 @attrs.define
 class StubtestSettings:
     """Information on the settings under which [stubtest][] is run on a certain package."""
 
@@ -598,14 +631,15 @@
 ]
 
 
 async def _get_pypi_data(
     package_name: PackageName, session: aiohttp.ClientSession | None
 ) -> _PypiData:
     pypi_data_url = f"https://pypi.org/pypi/{urllib.parse.quote(package_name)}/json"
+    response_json: dict[str, Any] | None = None
     async with AsyncExitStack() as stack:
         if session is None:
             session = await stack.enter_async_context(aiohttp.ClientSession())
         async with session.get(pypi_data_url) as response:
             response.raise_for_status()
             response_json = await response.json()
     assert isinstance(response_json, dict)
@@ -644,17 +678,18 @@
         A member of the [`PackageStatus`](./#PackageStatus) enumeration
             (see the docs on `PackageStatus` for details).
 
     Examples:
         >>> import asyncio
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_package_status
         >>> with tmpdir_typeshed() as typeshed:
-        ...     stdlib_status = asyncio.run(get_package_status("stdlib", typeshed_dir=typeshed))
+        ...     stdlib_status = asyncio.run(
+        ...         get_package_status("stdlib", typeshed_dir=typeshed)
+        ...     )
         ...     gdb_status = asyncio.run(get_package_status("gdb", typeshed_dir=typeshed))
-        ...
         >>> stdlib_status
         PackageStatus.STDLIB
         >>> help(_)
         Help on PackageStatus in module typeshed_stats.gather:
         <BLANKLINE>
         PackageStatus.STDLIB
             These are typeshed's stubs for the standard library. Typeshed's stdlib stubs are generally fairly up to date, and are tested against all currently supported Python versions in typeshed's CI.
@@ -696,15 +731,15 @@
     package_name: PackageName, *, typeshed_dir: Path | str
 ) -> UploadStatus:
     """Determine whether a certain package is currently uploaded to PyPI.
 
     Parameters:
         package_name: The name of the package to find the upload status for.
         typeshed_dir: A path pointing to a typeshed directory,
-            from which to retrieve the stubtest setting.
+            from which to retrieve the upload status.
 
     Returns:
         A member of the [`UploadStatus`](./#UploadStatus) enumeration
             (see the docs on `UploadStatus` for details).
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_upload_status
@@ -727,14 +762,108 @@
     match _get_package_metadata(package_name, typeshed_dir):
         case {"upload": False}:
             return UploadStatus.NOT_CURRENTLY_UPLOADED
         case _:
             return UploadStatus.UPLOADED
 
 
+class CompletenessLevel(_NiceReprEnum):
+    """Whether or not a stubs package has been explicitly marked as 'partial'.
+
+    See [PEP 561][] for an elaboration of what it means
+    for a stub to be marked as partial.
+    """
+
+    PARTIAL = "The stubs package may not cover the entire API at runtime"
+    COMPLETE = "The stubs package should cover the entire API at runtime"
+    STDLIB = (
+        "These are the stdlib stubs -- the idea of 'partial/complete' "
+        "doesn't really apply in the same way"
+    )
+
+
+def get_completeness_level(
+    package_name: PackageName, *, typeshed_dir: Path | str
+) -> CompletenessLevel:
+    """Determine whether a stubs package is explicitly marked as 'partial'.
+
+    See [PEP 561][] for an elaboration of what it means
+    for a stub to be marked as partial.
+
+    Parameters:
+        package_name: The name of the package to find the partial status for.
+        typeshed_dir: A path pointing to a typeshed directory,
+            from which to retrieve the partial status.
+
+    Returns:
+        A member of the [`CompletenessLevel`](./#CompletenessLevel) enumeration
+            (see the docs on `CompletenessLevel` for details).
+
+    Examples:
+        >>> from typeshed_stats.gather import tmpdir_typeshed, get_completeness_level
+        >>> with tmpdir_typeshed() as typeshed:
+        ...     stdlib_completeness = get_completeness_level(
+        ...         "stdlib", typeshed_dir=typeshed
+        ...     )
+        ...     requests_completeness = get_completeness_level(
+        ...         "requests", typeshed_dir=typeshed
+        ...     )
+        >>> requests_completeness
+        CompletenessLevel.COMPLETE
+        >>> help(_)
+        Help on CompletenessLevel in module typeshed_stats.gather:
+        <BLANKLINE>
+        CompletenessLevel.COMPLETE
+            The stubs package should cover the entire API at runtime
+        <BLANKLINE>
+        >>> stdlib_completeness
+        CompletenessLevel.STDLIB
+    """
+    if package_name == "stdlib":
+        return CompletenessLevel.STDLIB
+    match _get_package_metadata(package_name, typeshed_dir):
+        case {"partial_stub": True}:
+            return CompletenessLevel.PARTIAL
+        case _:
+            return CompletenessLevel.COMPLETE
+
+
+def get_upstream_url(
+    package_name: PackageName, *, typeshed_dir: Path | str
+) -> str | None:
+    """Get the URL for the source code of the runtime package these stubs are for.
+
+    Parameters:
+        package_name: The name of the package to find the upstream URL for.
+        typeshed_dir: A path pointing to a typeshed directory,
+            from which to retrieve the URL.
+
+    Returns:
+        The upstream URL (as a string).
+            If no URL is listed in the stubs package's METADATA.toml file,
+            returns [`None`][].
+
+    Examples:
+        >>> from typeshed_stats.gather import tmpdir_typeshed, get_upstream_url
+        >>> with tmpdir_typeshed() as typeshed:
+        ...     stdlib_url = get_upstream_url("stdlib", typeshed_dir=typeshed)
+        ...     requests_url = get_upstream_url("requests", typeshed_dir=typeshed)
+        ...     hdbcli_url = get_upstream_url("hdbcli", typeshed_dir=typeshed)
+        >>> stdlib_url
+        'https://github.com/python/cpython'
+        >>> requests_url
+        'https://github.com/psf/requests'
+        >>> hdbcli_url is None
+        True
+    """
+    if package_name == "stdlib":
+        return "https://github.com/python/cpython"
+    return _get_package_metadata(package_name, typeshed_dir).get("upstream_repository")
+
+
 def get_stub_distribution_name(
     package_name: PackageName, *, typeshed_dir: Path | str
 ) -> str:
     """Get the name this stubs package is uploaded to PyPI under.
 
     For the vast majority of packages in typeshed, this is `types-{runtime-name}`,
     but there may be a small number of packages
@@ -748,16 +877,20 @@
 
     Returns:
         The name under which the stubs package is uploaded to PyPI.
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_stub_distribution_name
         >>> with tmpdir_typeshed() as typeshed:
-        ...     requests_stub_dist_name = get_stub_distribution_name("requests", typeshed_dir=typeshed)
-        ...     pika_stub_dist_name = get_stub_distribution_name("pika", typeshed_dir=typeshed)
+        ...     requests_stub_dist_name = get_stub_distribution_name(
+        ...         "requests", typeshed_dir=typeshed
+        ...     )
+        ...     pika_stub_dist_name = get_stub_distribution_name(
+        ...         "pika", typeshed_dir=typeshed
+        ...     )
         >>> requests_stub_dist_name
         'types-requests'
         >>> pika_stub_dist_name
         'types-pika-ts'
     """
     if package_name == "stdlib":
         return "-"
@@ -793,43 +926,68 @@
     Returns:
         The number of lines of code the stubs package contains,
             excluding empty lines.
 
     Examples:
         >>> from typeshed_stats.gather import tmpdir_typeshed, get_package_size
         >>> with tmpdir_typeshed() as typeshed:
-        ...     mypy_extensions_size = get_package_size("mypy-extensions", typeshed_dir=typeshed)
-        ...
+        ...     mypy_extensions_size = get_package_size(
+        ...         "mypy-extensions", typeshed_dir=typeshed
+        ...     )
         >>> type(mypy_extensions_size) is int and mypy_extensions_size > 0
         True
     """
     return sum(
         get_number_of_lines_of_file(file)
         for file in _get_package_directory(package_name, typeshed_dir).rglob("*.pyi")
     )
 
 
+def _is_str_list(obj: object) -> TypeGuard[list[str]]:
+    return isinstance(obj, list) and all(isinstance(item, str) for item in obj)
+
+
+class _ExcludeList(NamedTuple):
+    spec: PathSpec
+    pathlist: list[Path]
+
+
+def _normalized_path(path: Path) -> str:
+    normalized_path = path.as_posix()
+    if path.is_dir():
+        normalized_path += "/"
+    return normalized_path
+
+
 @lru_cache
 def _get_pyright_excludelist(
     *,
     typeshed_dir: Path | str,
     config_filename: Literal["pyrightconfig.json", "pyrightconfig.stricter.json"],
-) -> frozenset[Path]:
+) -> _ExcludeList:
     # Read the config file;
     # do some pre-processing so that it can be passed to json.loads()
     config_path = Path(typeshed_dir, config_filename)
     with config_path.open(encoding="utf-8") as file:
         # strip comments from the file
         lines = [line for line in file if not line.strip().startswith("//")]
     # strip trailing commas from the file
     valid_json = re.sub(r",(\s*?[\}\]])", r"\1", "\n".join(lines))
     pyright_config = json.loads(valid_json)
     assert isinstance(pyright_config, dict)
-    excludelist = pyright_config.get("exclude", [])
-    return frozenset(Path(typeshed_dir, item) for item in excludelist)
+    excludelist: object = pyright_config.get("exclude", [])
+    assert _is_str_list(excludelist)
+    excludelist_as_paths = [Path(typeshed_dir, item) for item in excludelist]
+    return _ExcludeList(
+        PathSpec.from_lines(
+            GitWildMatchPattern,
+            [_normalized_path(item) for item in excludelist_as_paths],
+        ),
+        excludelist_as_paths,
+    )
 
 
 class PyrightSetting(_NiceReprEnum):
     """The various possible [pyright][] settings typeshed uses in CI."""
 
     ENTIRELY_EXCLUDED = (
         "All files in this stubs package "
@@ -851,18 +1009,24 @@
     )
     STRICT = (
         "All files in this stubs package are tested with the stricter pyright settings "
         "in typeshed's CI."
     )
 
 
-def _path_or_path_ancestor_is_listed(path: Path, path_list: Collection[Path]) -> bool:
-    return path in path_list or any(
-        listed_path in path.parents for listed_path in path_list
-    )
+def _path_or_path_ancestor_is_listed(path: Path, spec: PathSpec) -> bool:
+    if spec.match_file(_normalized_path(path)):
+        return True
+    if not path.is_dir():
+        return False
+    for subpath in path.rglob("*"):
+        if not spec.match_file(_normalized_path(subpath)):
+            return False
+    else:
+        return True
 
 
 def _child_of_path_is_listed(path: Path, path_list: Collection[Path]) -> bool:
     return any(path in listed_path.parents for listed_path in path_list)
 
 
 def get_pyright_setting_for_path(
@@ -881,23 +1045,25 @@
     """
     entirely_excluded_paths = _get_pyright_excludelist(
         typeshed_dir=typeshed_dir, config_filename="pyrightconfig.json"
     )
     paths_excluded_from_stricter_check = _get_pyright_excludelist(
         typeshed_dir=typeshed_dir, config_filename="pyrightconfig.stricter.json"
     )
-    file_path = file_path if isinstance(file_path, Path) else Path(file_path)
+    file_path = Path(typeshed_dir, file_path)
 
-    if _path_or_path_ancestor_is_listed(file_path, entirely_excluded_paths):
+    if _path_or_path_ancestor_is_listed(file_path, entirely_excluded_paths.spec):
         return PyrightSetting.ENTIRELY_EXCLUDED
-    if _child_of_path_is_listed(file_path, entirely_excluded_paths):
+    if _child_of_path_is_listed(file_path, entirely_excluded_paths.pathlist):
         return PyrightSetting.SOME_FILES_EXCLUDED
-    if _path_or_path_ancestor_is_listed(file_path, paths_excluded_from_stricter_check):
+    if _path_or_path_ancestor_is_listed(
+        file_path, paths_excluded_from_stricter_check.spec
+    ):
         return PyrightSetting.NOT_STRICT
-    if _child_of_path_is_listed(file_path, paths_excluded_from_stricter_check):
+    if _child_of_path_is_listed(file_path, paths_excluded_from_stricter_check.pathlist):
         return PyrightSetting.STRICT_ON_SOME_FILES
     return PyrightSetting.STRICT
 
 
 def get_pyright_setting_for_package(
     package_name: PackageName, *, typeshed_dir: Path | str
 ) -> PyrightSetting:
@@ -909,18 +1075,22 @@
             from which to retrieve the pyright setting.
 
     Returns:
         A member of the [`PyrightSetting`](./#PyrightSetting) enumeration
             (see the docs on `PyrightSetting` for details).
 
     Examples:
-        >>> from typeshed_stats.gather import tmpdir_typeshed, get_pyright_setting_for_package
+        >>> from typeshed_stats.gather import (
+        ...     tmpdir_typeshed,
+        ...     get_pyright_setting_for_package,
+        ... )
         >>> with tmpdir_typeshed() as typeshed:
-        ...     stdlib_setting = get_pyright_setting_for_package("stdlib", typeshed_dir=typeshed)
-        ...
+        ...     stdlib_setting = get_pyright_setting_for_package(
+        ...         "stdlib", typeshed_dir=typeshed
+        ...     )
         >>> stdlib_setting
         PyrightSetting.STRICT_ON_SOME_FILES
         >>> help(_)
         Help on PyrightSetting in module typeshed_stats.gather:
         <BLANKLINE>
         PyrightSetting.STRICT_ON_SOME_FILES
             Some files in this stubs package are tested with the stricter pyright settings in typeshed's CI; some are excluded from the stricter settings.
@@ -935,14 +1105,16 @@
 @final
 @attrs.define
 class PackageInfo:
     """Statistics about a single stubs package in typeshed."""
 
     package_name: PackageName
     stub_distribution_name: str
+    upstream_url: str | None
+    completeness_level: CompletenessLevel
     extra_description: str | None
     number_of_lines: int
     package_status: PackageStatus
     upload_status: UploadStatus
     stubtest_settings: StubtestSettings
     pyright_setting: PyrightSetting
     annotation_stats: AnnotationStats
@@ -974,28 +1146,33 @@
     Returns:
         An instance of the [`PackageInfo`](./#PackageInfo) class.
 
     Examples:
         >>> import asyncio
         >>> from typeshed_stats.gather import tmpdir_typeshed, gather_stats_on_package
         >>> with tmpdir_typeshed() as typeshed:
-        ...     stdlib_info = asyncio.run(gather_stats_on_package("stdlib", typeshed_dir=typeshed))
-        ...
+        ...     stdlib_info = asyncio.run(
+        ...         gather_stats_on_package("stdlib", typeshed_dir=typeshed)
+        ...     )
         >>> stdlib_info.package_name
         'stdlib'
         >>> stdlib_info.stubtest_settings.strictness
         StubtestStrictness.ERROR_ON_MISSING_STUB
         >>> type(stdlib_info.number_of_lines) is int and stdlib_info.number_of_lines > 0
         True
     """
     return PackageInfo(
         package_name=package_name,
         stub_distribution_name=get_stub_distribution_name(
             package_name, typeshed_dir=typeshed_dir
         ),
+        upstream_url=get_upstream_url(package_name, typeshed_dir=typeshed_dir),
+        completeness_level=get_completeness_level(
+            package_name, typeshed_dir=typeshed_dir
+        ),
         extra_description=get_package_extra_description(
             package_name, typeshed_dir=typeshed_dir
         ),
         number_of_lines=get_package_size(package_name, typeshed_dir=typeshed_dir),
         package_status=await get_package_status(
             package_name, typeshed_dir=typeshed_dir, session=session
         ),
@@ -1136,29 +1313,38 @@
         ),
         annotation_stats=gather_annotation_stats_on_file(file_path),
     )
 
 
 async def _gather_stats_on_multiple_packages(
     packages: Iterable[str], *, typeshed_dir: Path | str
-) -> Sequence[PackageInfo]:
+) -> Sequence[PackageInfo | BaseException]:
     conn = aiohttp.TCPConnector(limit_per_host=10)
     async with aiohttp.ClientSession(connector=conn) as session:
         tasks = (
             gather_stats_on_package(
                 package_name, typeshed_dir=typeshed_dir, session=session
             )
             for package_name in packages
         )
         return await asyncio.gather(*tasks, return_exceptions=True)
 
 
 _get_package_name = attrgetter("package_name")
 
 
+def _raise_any_exceptions(
+    results: Iterable[PackageInfo | BaseException],
+) -> TypeGuard[Iterable[PackageInfo]]:
+    for result in results:
+        if isinstance(result, BaseException):
+            raise result
+    return True
+
+
 def gather_stats_on_multiple_packages(
     packages: Iterable[str] | None = None, *, typeshed_dir: Path | str
 ) -> Sequence[PackageInfo]:
     """Concurrently gather statistics on multiple packages.
 
     !!! note
 
@@ -1174,33 +1360,34 @@
 
     Returns:
         A sequence of [`PackageInfo`](./#PackageInfo) objects.
             Each `PackageInfo` object contains information representing an analysis
             of a certain stubs package in typeshed.
 
     Examples:
-        >>> from typeshed_stats.gather import PackageInfo, tmpdir_typeshed, gather_stats_on_multiple_packages
+        >>> from typeshed_stats.gather import (
+        ...     PackageInfo,
+        ...     tmpdir_typeshed,
+        ...     gather_stats_on_multiple_packages,
+        ... )
         >>> with tmpdir_typeshed() as typeshed:
         ...     infos = gather_stats_on_multiple_packages(
         ...         ["stdlib", "aiofiles", "boto"], typeshed_dir=typeshed
         ...     )
-        ...
         >>> [info.package_name for info in infos]
         ['aiofiles', 'boto', 'stdlib']
         >>> all(type(info) is PackageInfo for info in infos)
         True
     """
     if packages is None:
         packages = os.listdir(Path(typeshed_dir, "stubs")) + ["stdlib"]
     results = asyncio.run(
         _gather_stats_on_multiple_packages(packages, typeshed_dir=typeshed_dir)
     )
-    for result in results:
-        if isinstance(result, BaseException):
-            raise result
+    assert _raise_any_exceptions(results)
     return sorted(results, key=_get_package_name)
 
 
 @contextmanager
 def tmpdir_typeshed() -> Iterator[Path]:
     """Clone typeshed into a tempdir, then yield a [`Path`][pathlib.Path] pointing to it.
```

### Comparing `typeshed_stats-23.2.1/src/typeshed_stats/serialize.py` & `typeshed_stats-24.5.21/src/typeshed_stats/serialize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Tools for serializing and deserializing [`PackageInfo`][typeshed_stats.gather.PackageInfo] and [`FileInfo`][typeshed_stats.gather.FileInfo] objects."""
 
 import typing
 from collections.abc import Sequence
 from functools import cache
 from operator import attrgetter
 from pathlib import Path
+from typing import Any
 
 import attrs
 import cattrs
 
 from typeshed_stats.gather import (
     AnnotationStats,
     FileInfo,
     PackageInfo,
     StubtestSettings,
     StubtestStrictness,
-    _NiceReprEnum,
+    _NiceReprEnum,  # pyright: ignore[reportPrivateUsage]
 )
 
 if typing.TYPE_CHECKING:
     import jinja2
 
 __all__ = [
     "file_stats_from_csv",
@@ -33,15 +34,15 @@
 
 _CATTRS_CONVERTER = cattrs.Converter()
 _unstructure = _CATTRS_CONVERTER.unstructure
 _structure = _CATTRS_CONVERTER.structure
 
 _CATTRS_CONVERTER.register_unstructure_hook(_NiceReprEnum, attrgetter("name"))
 _CATTRS_CONVERTER.register_unstructure_hook(Path, Path.as_posix)
-_CATTRS_CONVERTER.register_structure_hook(_NiceReprEnum, lambda d, t: t[d])  # type: ignore[index,no-any-return]
+_CATTRS_CONVERTER.register_structure_hook(_NiceReprEnum, lambda d, t: t[d])
 _CATTRS_CONVERTER.register_structure_hook(
     Path, lambda d, t: Path(d)
 )  # pragma: no branch
 
 
 def stats_to_json(stats: Sequence[PackageInfo | FileInfo]) -> str:
     """Convert stats on multiple stubs packages to JSON format.
@@ -102,56 +103,57 @@
     converted_stats = _unstructure(stats)
     for info in converted_stats:
         info |= info["annotation_stats"]
         del info["annotation_stats"]
 
         # This section is specific to PackageInfo objects
         if "stubtest_settings" in info:
+            for k, v in PackageInfo.__annotations__.items():
+                if v == (str | None) and info[k] is None:
+                    info[k] = "-"
             info |= {
                 f"stubtest_{key}": val for key, val in info["stubtest_settings"].items()
             }
             del info["stubtest_settings"]
             stubtest_platforms = info["stubtest_platforms"]
             if not stubtest_platforms:
                 info["stubtest_platforms"] = "None"
             else:
                 info["stubtest_platforms"] = ";".join(stubtest_platforms)
-            if info["extra_description"] is None:
-                info["extra_description"] = "-"
 
     fieldnames = converted_stats[0].keys()
     csvfile = io.StringIO(newline="")
     writer = csv.DictWriter(csvfile, fieldnames=fieldnames)
     writer.writeheader()
     for info in converted_stats:
         writer.writerow(info)
     return csvfile.getvalue()
 
 
 @typing.overload
-def _stats_from_csv(data: str, cls: type[PackageInfo]) -> list[PackageInfo]:
-    ...
+def _stats_from_csv(data: str, cls: type[PackageInfo]) -> list[PackageInfo]: ...
 
 
 @typing.overload
-def _stats_from_csv(data: str, cls: type[FileInfo]) -> list[FileInfo]:
-    ...
+def _stats_from_csv(data: str, cls: type[FileInfo]) -> list[FileInfo]: ...
 
 
 def _stats_from_csv(
     data: str, cls: type[PackageInfo | FileInfo]
 ) -> list[PackageInfo] | list[FileInfo]:
     import csv
     import io
 
     csvfile = io.StringIO(data, newline="")
     stats = list(csv.DictReader(csvfile))
-    converted_stats = []
+    converted_stats: list[dict[str, Any]] = []
     for stat in stats:
-        converted_stat, annotation_stats, stubtest_settings = {}, {}, {}
+        converted_stat: dict[str, Any] = {}
+        annotation_stats: dict[str, Any] = {}
+        stubtest_settings: dict[str, Any] = {}
         for key, val in stat.items():
             if key in AnnotationStats.__annotations__:
                 annotation_stats[key] = val
             elif key.removeprefix("stubtest_") in StubtestSettings.__annotations__:
                 stubtest_settings[key.removeprefix("stubtest_")] = val
             else:
                 converted_stat[key] = val
@@ -159,18 +161,19 @@
         converted_stat["stubtest_settings"] = stubtest_settings
         if cls is PackageInfo:
             stubtest_platforms = stubtest_settings["platforms"]
             if stubtest_platforms == "None":
                 stubtest_settings["platforms"] = []
             else:
                 stubtest_settings["platforms"] = stubtest_platforms.split(";")
-            if converted_stat["extra_description"] == "-":
-                converted_stat["extra_description"] = None
+            for k, v in PackageInfo.__annotations__.items():
+                if converted_stat[k] == "-" and v == (str | None):
+                    converted_stat[k] = None
         converted_stats.append(converted_stat)
-    return _structure(converted_stats, list[cls])  # type: ignore[valid-type]
+    return _structure(converted_stats, list[cls])  # type: ignore[valid-type]  # pyright: ignore[reportGeneralTypeIssues]
 
 
 def package_stats_from_csv(data: str) -> list[PackageInfo]:
     """Load [`PackageInfo`][typeshed_stats.gather.PackageInfo] objects from csv format.
 
     Parameters:
         data: A CSV string.
```

### Comparing `typeshed_stats-23.2.1/stats_website/gather.md` & `typeshed_stats-24.5.21/stats_website/gather.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/stats_website/logo.png` & `typeshed_stats-24.5.21/stats_website/logo.png`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/stats_website/stats-csv.md` & `typeshed_stats-24.5.21/stats_website/stats-csv.md`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/stats_website/javascripts/filtertable.js` & `typeshed_stats-24.5.21/stats_website/javascripts/filtertable.js`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/tests/conftest.py` & `typeshed_stats-24.5.21/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # Make sure not to import rich or markdown here, since they're optional dependencies
 # Some tests assert behaviour that's predicated on these modules not yet being imported
 import pytest
 
 from typeshed_stats.gather import (
     AnnotationStats,
+    CompletenessLevel,
     FileInfo,
     PackageInfo,
     PackageStatus,
     PyrightSetting,
     StubtestSettings,
     StubtestStrictness,
     UploadStatus,
@@ -220,29 +221,31 @@
 def random_identifier() -> str:
     return "".join(
         random.choice(string.ascii_letters) for _ in range(random.randint(1, 10))
     )
 
 
 def random_AnnotationStats() -> AnnotationStats:
-    return AnnotationStats(
-        *[random.randint(0, 1000) for _ in AnnotationStats.__annotations__]
-    )
+    return AnnotationStats(*[
+        random.randint(0, 1000) for _ in AnnotationStats.__annotations__
+    ])
 
 
 def random_PackageInfo() -> PackageInfo:
     package_name = random_identifier()
     stubtest_strictness = random.choice(list(StubtestStrictness))
     if stubtest_strictness is StubtestStrictness.SKIPPED:
         stubtest_platforms = []
     else:
         stubtest_platforms = [random.choice(["win32", "darwin", "linux"])]
     return PackageInfo(
         package_name=package_name,
         stub_distribution_name=f"types-{package_name}",
+        upstream_url=f"https://github.com/who_knows/{package_name}",
+        completeness_level=CompletenessLevel.COMPLETE,
         extra_description=None,
         number_of_lines=random.randint(10, 500),
         package_status=random.choice(list(PackageStatus)),
         stubtest_settings=StubtestSettings(stubtest_strictness, stubtest_platforms, 55),
         upload_status=random.choice(list(UploadStatus)),
         pyright_setting=random.choice(list(PyrightSetting)),
         annotation_stats=random_AnnotationStats(),
```

### Comparing `typeshed_stats-23.2.1/tests/test___all__.py` & `typeshed_stats-24.5.21/tests/test___all__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import pytest
 
 import typeshed_stats
 
 ALL_SUBMODULES: Final = [
     importlib.import_module(f"typeshed_stats.{m.name}")
     for m in pkgutil.iter_modules(typeshed_stats.__path__)
+    if m.name != "_version"
 ]
 
 
 @pytest.fixture(params=ALL_SUBMODULES)
 def submodule(request: pytest.FixtureRequest) -> types.ModuleType:
     return request.param  # type: ignore[no-any-return]
 
@@ -30,18 +31,14 @@
 
 
 def test_submodule__all___is_valid(submodule: types.ModuleType) -> None:
     assert isinstance(submodule.__all__, list)
     assert all(isinstance(item, str) for item in submodule.__all__)
 
 
-def test___all___alphabetisation(submodule: types.ModuleType) -> None:
-    assert submodule.__all__ == sorted(submodule.__all__)
-
-
 def test_all_public_names_in___all__(submodule: types.ModuleType) -> None:
     """Test that all names not in `__all__` are marked as private."""
     submodule_name = submodule.__name__
 
     def is_from_other_module(obj: object) -> bool:
         return getattr(obj, "__module__", submodule_name) != submodule_name
```

### Comparing `typeshed_stats-23.2.1/tests/test__cli.py` & `typeshed_stats-24.5.21/tests/test__cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 from unittest import mock
 
 # Make sure not to import rich here, as it's optional dependencies
 # Some tests assert behaviour that's predicated on rich not yet being imported
 import markdown
 import pytest
 from pytest_mock import MockerFixture
-from pytest_subtests import SubTests  # type: ignore[import]
+from pytest_subtests import SubTests
 
 import typeshed_stats._cli
 import typeshed_stats.gather
 from typeshed_stats._cli import SUPPORTED_EXTENSIONS, OutputOption, main
 from typeshed_stats.gather import (
+    CompletenessLevel,
     PackageInfo,
     PackageStatus,
     PyrightSetting,
     StubtestStrictness,
     UploadStatus,
 )
 
@@ -219,14 +220,19 @@
         self,
         mocker: MockerFixture,
         EXAMPLE_PACKAGE_NAME: str,
         capsys: pytest.CaptureFixture[str],
     ) -> None:
         patches_to_apply = [
             ("get_package_status", PackageStatus.UP_TO_DATE),
+            ("get_completeness_level", CompletenessLevel.COMPLETE),
+            (
+                "get_upstream_url",
+                f"https://github.com/who_knows/{EXAMPLE_PACKAGE_NAME}",
+            ),
             ("get_stubtest_strictness", StubtestStrictness.MISSING_STUBS_IGNORED),
             ("get_pyright_setting_for_package", PyrightSetting.STRICT_ON_SOME_FILES),
             ("get_package_extra_description", None),
             ("get_upload_status", UploadStatus.UPLOADED),
             ("get_stubtest_platforms", ["linux"]),
             ("get_stub_distribution_name", "types-foo"),
             ("get_stubtest_allowlist_length", 55),
@@ -607,19 +613,22 @@
 # ====================================
 
 
 def test_KeyboardInterrupt_caught(
     args: list[str], typeshed: Path, capsys: pytest.CaptureFixture[str]
 ) -> None:
     args += ["--log", "CRITICAL"]
-    with pytest.raises(SystemExit) as exc_info, mock.patch.object(
-        typeshed_stats.gather,
-        "gather_stats_on_package",
-        autospec=True,
-        side_effect=KeyboardInterrupt(),
+    with (
+        pytest.raises(SystemExit) as exc_info,
+        mock.patch.object(
+            typeshed_stats.gather,
+            "gather_stats_on_package",
+            autospec=True,
+            side_effect=KeyboardInterrupt(),
+        ),
     ):
         main(args)
 
     stderr = capsys.readouterr().err
     num_stderr_lines = len(stderr.strip().splitlines())
     assert num_stderr_lines == 1
     assert "Interrupted!" in stderr
```

### Comparing `typeshed_stats-23.2.1/tests/test_gather.py` & `typeshed_stats-24.5.21/tests/test_gather.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,58 @@
+# pyright: reportPrivateUsage=false,reportUnusedClass=false
 from __future__ import annotations
 
 import json
 import os
 import random
 import sys
 import textwrap
+import types
 from collections.abc import Callable
 from contextlib import AbstractAsyncContextManager, nullcontext
-from dataclasses import InitVar, dataclass
+from dataclasses import dataclass, field
 from itertools import chain
 from pathlib import Path
 from typing import Final, TypeAlias
 from unittest import mock
 
 # Make sure not to import rich here, since it's an optional dependency
 # Some tests assert behaviour that's predicated on rich not yet being imported
 import aiohttp
 import pytest
 from packaging.version import Version
 from pytest_mock import MockerFixture
-from pytest_subtests import SubTests  # type: ignore[import]
+from pytest_subtests import SubTests
 
 import typeshed_stats
 import typeshed_stats.gather
 from typeshed_stats.gather import (
     AnnotationStats,
+    CompletenessLevel,
     PackageInfo,
     PackageStatus,
     PyrightSetting,
     StubtestStrictness,
     UploadStatus,
     _get_pypi_data,
     gather_annotation_stats_on_file,
     gather_annotation_stats_on_package,
     gather_stats_on_file,
     gather_stats_on_multiple_packages,
+    get_completeness_level,
     get_package_extra_description,
     get_package_size,
     get_package_status,
     get_pyright_setting_for_package,
     get_stub_distribution_name,
     get_stubtest_allowlist_length,
     get_stubtest_platforms,
     get_stubtest_strictness,
     get_upload_status,
+    get_upstream_url,
     tmpdir_typeshed,
 )
 
 from .conftest import PYRIGHTCONFIG_TEMPLATE, write_metadata_text
 
 # ===================
 # _NiceReprEnum tests
@@ -337,15 +342,15 @@
 # Tests for get_stubtest_allowlist_length
 # ==============================
 
 
 def test_get_stubtest_allowlist_length_stdlib(
     typeshed: Path, maybe_stringize_path: Callable[[Path], Path | str]
 ) -> None:
-    tests_dir = typeshed / "tests"
+    tests_dir = typeshed / "stdlib" / "@tests"
     tests_dir.mkdir()
     allowlist_dir = tests_dir / "stubtest_allowlists"
     allowlist_dir.mkdir()
     (allowlist_dir / "darwin.txt").write_text(
         textwrap.dedent(
             """\
             foo
@@ -575,14 +580,83 @@
     actual_result = get_upload_status(
         EXAMPLE_PACKAGE_NAME, typeshed_dir=maybe_stringize_path(typeshed)
     )
     expected_result = UploadStatus[expected_result_name]
     assert actual_result is expected_result
 
 
+# =================================
+# Tests for get_upstream_url
+# =================================
+
+
+def test_upstream_url_stdlib() -> None:
+    result = get_upstream_url("stdlib", typeshed_dir=Path("."))
+    assert result == "https://github.com/python/cpython"
+
+
+@pytest.mark.parametrize(
+    ("metadata_text", "expected_upstream_url"),
+    [
+        pytest.param(
+            'upstream_repository = "https://github.com/psf/requests"',
+            "https://github.com/psf/requests",
+            id="upstream_repo_given",
+        ),
+        pytest.param("", None, id="upstream_repo_not_given"),
+    ],
+)
+def test_get_upstream_url_non_stdlib(
+    metadata_text: str,
+    expected_upstream_url: str,
+    typeshed: Path,
+    EXAMPLE_PACKAGE_NAME: str,
+    maybe_stringize_path: Callable[[Path], Path | str],
+) -> None:
+    write_metadata_text(typeshed, EXAMPLE_PACKAGE_NAME, metadata_text)
+    actual_result = get_upstream_url(
+        EXAMPLE_PACKAGE_NAME, typeshed_dir=maybe_stringize_path(typeshed)
+    )
+    assert actual_result == expected_upstream_url
+    assert type(actual_result) is type(expected_upstream_url)
+
+
+# =================================
+# Tests for get_completeness_level
+# =================================
+
+
+def test_get_completeness_level_stdlib() -> None:
+    result = get_completeness_level("stdlib", typeshed_dir=Path("."))
+    assert result is CompletenessLevel.STDLIB
+
+
+@pytest.mark.parametrize(
+    ("metadata_text", "expected_completeness_level"),
+    [
+        pytest.param("partial_stub = true", "PARTIAL", id="partial"),
+        pytest.param("partial_stub = false", "COMPLETE", id="explicitly_complete"),
+        pytest.param("", "COMPLETE", id="implicitly_complete"),
+    ],
+)
+def test_get_completeness_level_non_stdlib(
+    metadata_text: str,
+    expected_completeness_level: str,
+    typeshed: Path,
+    EXAMPLE_PACKAGE_NAME: str,
+    maybe_stringize_path: Callable[[Path], Path | str],
+) -> None:
+    write_metadata_text(typeshed, EXAMPLE_PACKAGE_NAME, metadata_text)
+    actual_result = get_completeness_level(
+        EXAMPLE_PACKAGE_NAME, typeshed_dir=maybe_stringize_path(typeshed)
+    )
+    expected_result = CompletenessLevel[expected_completeness_level]
+    assert actual_result is expected_result
+
+
 # ======================================
 # Tests for get_stub_distribution_name()
 # ======================================
 
 
 def test_get_stub_distribution_name_stdlib() -> None:
     result = get_stub_distribution_name("stdlib", typeshed_dir=Path("."))
@@ -676,89 +750,115 @@
 # ================================
 
 
 @dataclass
 class PyrightTestCase:
     package_to_test: str
     expected_result: str
-    entirely_excluded_path: InitVar[str | None] = None
-    path_excluded_from_strict: InitVar[str | None] = None
+    entirely_excluded_path: str = ""
+    path_excluded_from_strict: str = ""
+    pyrightconfig_basic: str = field(init=False, repr=False)
+    pyrightconfig_strict: str = field(init=False, repr=False)
 
-    def __post_init__(
-        self,
-        entirely_excluded_path: str | None = None,
-        path_excluded_from_strict: str | None = None,
-    ) -> None:
+    def __post_init__(self) -> None:
         default_path = "foo.pyi"
-        entirely_excluded_path = entirely_excluded_path or default_path
+        self.entirely_excluded_path = self.entirely_excluded_path or default_path
         self.pyrightconfig_basic = PYRIGHTCONFIG_TEMPLATE.format(
-            f'"{entirely_excluded_path}"'
+            f'"{self.entirely_excluded_path}"'
         )
-        excluded_from_strict = path_excluded_from_strict or default_path
+        self.excluded_from_strict = self.path_excluded_from_strict or default_path
         self.pyrightconfig_strict = PYRIGHTCONFIG_TEMPLATE.format(
-            f'"{excluded_from_strict}"'
+            f'"{self.excluded_from_strict}"'
         )
 
 
 PYRIGHT_TEST_CASES: Final = (
     # Some files are entirely excluded, none are excluded from strict settings
     PyrightTestCase(
         entirely_excluded_path="stdlib",
         package_to_test="stdlib",
         expected_result="ENTIRELY_EXCLUDED",
     ),
     PyrightTestCase(
+        entirely_excluded_path="stdlib/**/*.pyi",
+        package_to_test="stdlib",
+        expected_result="ENTIRELY_EXCLUDED",
+    ),
+    PyrightTestCase(
         entirely_excluded_path="stdlib/tkinter",
         package_to_test="stdlib",
         expected_result="SOME_FILES_EXCLUDED",
     ),
     PyrightTestCase(
+        entirely_excluded_path="stdlib/lib2to3/fixes/*.pyi",
+        package_to_test="stdlib",
+        expected_result="SOME_FILES_EXCLUDED",
+    ),
+    PyrightTestCase(
         entirely_excluded_path="stdlib",
-        path_excluded_from_strict=None,
         package_to_test="boto",
         expected_result="STRICT",
     ),
     PyrightTestCase(
         entirely_excluded_path="stubs",
         package_to_test="aiofiles",
         expected_result="ENTIRELY_EXCLUDED",
     ),
     PyrightTestCase(
         entirely_excluded_path="stubs/aiofiles",
         package_to_test="aiofiles",
         expected_result="ENTIRELY_EXCLUDED",
     ),
     PyrightTestCase(
+        entirely_excluded_path="stubs/aiofiles/**/*.pyi",
+        package_to_test="aiofiles",
+        expected_result="ENTIRELY_EXCLUDED",
+    ),
+    PyrightTestCase(
         entirely_excluded_path="stubs/aiofiles",
-        path_excluded_from_strict=None,
         package_to_test="boto",
         expected_result="STRICT",
     ),
     # No files are entirely excluded, some are excluded from strict settings
     PyrightTestCase(
         path_excluded_from_strict="stdlib",
         package_to_test="stdlib",
         expected_result="NOT_STRICT",
     ),
     PyrightTestCase(
+        path_excluded_from_strict="stdlib/**/*.pyi",
+        package_to_test="stdlib",
+        expected_result="NOT_STRICT",
+    ),
+    PyrightTestCase(
         path_excluded_from_strict="stdlib/tkinter",
         package_to_test="stdlib",
         expected_result="STRICT_ON_SOME_FILES",
     ),
     PyrightTestCase(
+        path_excluded_from_strict="stdlib/tkinter/*.pyi",
+        package_to_test="stdlib",
+        expected_result="STRICT_ON_SOME_FILES",
+    ),
+    PyrightTestCase(
         path_excluded_from_strict="stubs",
         package_to_test="stdlib",
         expected_result="STRICT",
     ),
     PyrightTestCase(
         path_excluded_from_strict="stubs/aiofiles",
         package_to_test="stdlib",
         expected_result="STRICT",
     ),
     PyrightTestCase(
+        path_excluded_from_strict="stubs/aiofiles/*.pyi",
+        package_to_test="stdlib",
+        expected_result="STRICT",
+    ),
+    PyrightTestCase(
         path_excluded_from_strict="stubs",
         package_to_test="appdirs",
         expected_result="NOT_STRICT",
     ),
     PyrightTestCase(
         path_excluded_from_strict="stubs/boto/auth.pyi",
         package_to_test="boto",
@@ -774,26 +874,38 @@
     PyrightTestCase(
         entirely_excluded_path="stdlib/tkinter",
         path_excluded_from_strict="stdlib/asyncio",
         package_to_test="stdlib",
         expected_result="SOME_FILES_EXCLUDED",
     ),
     PyrightTestCase(
+        entirely_excluded_path="stdlib/tkinter/*.pyi",
+        path_excluded_from_strict="stdlib/asyncio/*.pyi",
+        package_to_test="stdlib",
+        expected_result="SOME_FILES_EXCLUDED",
+    ),
+    PyrightTestCase(
         entirely_excluded_path="stubs",
         path_excluded_from_strict="stdlib/tkinter",
         package_to_test="stdlib",
         expected_result="STRICT_ON_SOME_FILES",
     ),
     PyrightTestCase(
         entirely_excluded_path="stdlib",
         path_excluded_from_strict="stubs/boto/auth.pyi",
         package_to_test="boto",
         expected_result="STRICT_ON_SOME_FILES",
     ),
     PyrightTestCase(
+        entirely_excluded_path="stdlib/*.pyi",
+        path_excluded_from_strict="stubs/boto/auth.pyi",
+        package_to_test="boto",
+        expected_result="STRICT_ON_SOME_FILES",
+    ),
+    PyrightTestCase(
         entirely_excluded_path="stubs/boto/auth.pyi",
         path_excluded_from_strict="stubs/boto/foo.pyi",
         package_to_test="boto",
         expected_result="SOME_FILES_EXCLUDED",
     ),
 )
 
@@ -808,14 +920,21 @@
     maybe_stringize_path: Callable[[Path], Path | str],
 ) -> None:
     config_filenames_to_configs = {
         "pyrightconfig.json": test_case.pyrightconfig_basic,
         "pyrightconfig.stricter.json": test_case.pyrightconfig_strict,
     }
 
+    if test_case.package_to_test == "stdlib":
+        (typeshed / "stdlib" / "functools.pyi").write_text("")
+    else:
+        package_dir = typeshed / "stubs" / test_case.package_to_test
+        package_dir.mkdir()
+        (package_dir / "foo.pyi").write_text("")
+
     for config_filename, config in config_filenames_to_configs.items():
         with pytest.raises(json.JSONDecodeError):
             json.loads(config)
 
         (typeshed / config_filename).write_text(config, encoding="utf-8")
 
     pyright_setting = get_pyright_setting_for_package(
@@ -830,15 +949,15 @@
 # Tests for tmpdir_typeshed
 # =========================
 
 
 @pytest.mark.requires_network
 def test_tmpdir_typeshed() -> None:
     with tmpdir_typeshed() as typeshed:
-        typeshed = typeshed  # noqa: SIM909
+        typeshed = typeshed
         assert isinstance(typeshed, Path)
         assert typeshed.exists()
         assert typeshed.is_dir()
         stubs_dir, stdlib_dir = typeshed / "stubs", typeshed / "stdlib"
         assert stubs_dir.exists()
         assert stubs_dir.is_dir()
         assert stdlib_dir.exists()
@@ -852,15 +971,15 @@
 # Tests for gather_stats_on_file
 # ======================
 
 
 # Tests for bad arguments passed into typeshed_dir
 def test_gather_stats_on_file_bad_typeshed_dir_type() -> None:
     with pytest.raises(TypeError, match="Expected str or Path argument"):
-        gather_stats_on_file("stdlib/functools.pyi", typeshed_dir=5)  # type: ignore[arg-type]
+        gather_stats_on_file("stdlib/functools.pyi", typeshed_dir=5)  # type: ignore[arg-type]  # pyright: ignore[reportGeneralTypeIssues]
 
 
 def test_gather_stats_on_file_nonexistent_typeshed_dir() -> None:
     with pytest.raises(ValueError, match="does not exist"):
         gather_stats_on_file("stdlib/functools.pyi", typeshed_dir="foo/bar")
 
 
@@ -870,15 +989,15 @@
     with pytest.raises(ValueError, match="is not a directory"):
         gather_stats_on_file("stdlib/functools.pyi", typeshed_dir=file)
 
 
 # Tests for bad arguments passed into file_path
 def test_gather_stats_on_file_bad_file_path_type() -> None:
     with pytest.raises(TypeError, match="Expected str or Path argument"):
-        gather_stats_on_file(5, typeshed_dir=".")  # type: ignore[arg-type]
+        gather_stats_on_file(5, typeshed_dir=".")  # type: ignore[arg-type]  # pyright: ignore[reportGeneralTypeIssues]
 
 
 def test_gather_stats_on_file_nonexistent_file() -> None:
     with pytest.raises(ValueError, match="does not exist"):
         gather_stats_on_file("foo/bar.pyi", typeshed_dir=".")
 
 
@@ -1015,22 +1134,50 @@
 
     assert all(isinstance(item, PackageInfo) for item in results)
     package_names_in_results = [item.package_name for item in results]
     assert package_names_in_results == sorted(package_names_in_results)
     assert set(package_names_in_results) == package_names
 
 
+KNOWN_FULLY_ANNOTATED_FILES_WITH_LAX_PYRIGHT_SETTINGS = frozenset({
+    Path("stdlib/lib2to3/fixes/fix_imports2.pyi"),
+    Path("stdlib/lib2to3/fixes/__init__.pyi"),
+    Path("stdlib/xml/sax/__init__.pyi"),
+})
+
+
 @pytest.mark.dependency(depends=["integration_basic"])
 def test_basic_sanity_checks(subtests: SubTests) -> None:
     with tmpdir_typeshed() as typeshed:
         stats_on_packages = gather_stats_on_multiple_packages(typeshed_dir=typeshed)
         stats_on_stdlib_files = [
             gather_stats_on_file(path, typeshed_dir=typeshed)
             for path in (typeshed / "stdlib").rglob("*.pyi")
         ]
+
+    at_least_one_incomplete_package = any(  # pragma: no branch
+        s.completeness_level is CompletenessLevel.PARTIAL for s in stats_on_packages
+    )
+    no_partial_packages_msg = "Likely bug detected: no packages are marked as partial?!"
+    assert at_least_one_incomplete_package, no_partial_packages_msg
+
+    at_least_one_complete_package = any(  # pragma: no branch
+        s.completeness_level is CompletenessLevel.COMPLETE for s in stats_on_packages
+    )
+    no_complete_packages_msg = (
+        "Likely bug detected: no packages are marked as complete?!"
+    )
+    assert at_least_one_complete_package, no_complete_packages_msg
+
+    at_least_one_upstream_url = any(  # pragma: no branch
+        isinstance(s.upstream_url, str) for s in stats_on_packages
+    )
+    no_upstream_urls_msg = "Likely bug detected: no packages list an upstream URL?!"
+    assert at_least_one_upstream_url, no_upstream_urls_msg
+
     for s in stats_on_packages:
         with subtests.test(package_name=s.package_name):
             annot_stats = s.annotation_stats
             is_only_partially_annotated = bool(
                 annot_stats.unannotated_parameters or annot_stats.unannotated_returns
             )
             is_fully_annotated = not is_only_partially_annotated
@@ -1042,14 +1189,18 @@
                 )
             else:
                 assert is_only_partially_annotated, (
                     "Likely bug detected: "
                     f"{s.package_name!r} is fully annotated, "
                     "but does not have the strictest pyright settings in CI"
                 )
+            upstream_url = s.upstream_url
+            assert isinstance(upstream_url, str | types.NoneType)
+            if upstream_url is not None:
+                assert upstream_url.startswith("https://")
     for f in stats_on_stdlib_files:
         if Path("stdlib/distutils/command") in f.file_path.parents:
             continue
         with subtests.test(path=f.file_path):
             annot_stats = f.annotation_stats
             is_only_partially_annotated = bool(
                 annot_stats.unannotated_parameters or annot_stats.unannotated_returns
@@ -1057,23 +1208,28 @@
             is_fully_annotated = not is_only_partially_annotated
             if f.pyright_setting is PyrightSetting.STRICT:
                 assert is_fully_annotated, (
                     "Likely bug detected: "
                     f"{f.file_path!r} has unannotated parameters and/or returns, "
                     "but has the strictest pyright settings in CI"
                 )
-            else:
+            elif (
+                f.file_path not in KNOWN_FULLY_ANNOTATED_FILES_WITH_LAX_PYRIGHT_SETTINGS
+            ):
                 assert is_only_partially_annotated, (
                     "Likely bug detected: "
                     f"{f.file_path!r} is fully annotated, "
                     "but does not have the strictest pyright settings in CI"
                 )
 
 
 def test_exceptions_bubble_up(typeshed: Path) -> None:
-    with pytest.raises(KeyError), mock.patch.object(
-        typeshed_stats.gather,
-        "gather_stats_on_package",
-        autospec=True,
-        side_effect=KeyError,
+    with (
+        pytest.raises(KeyError),
+        mock.patch.object(
+            typeshed_stats.gather,
+            "gather_stats_on_package",
+            autospec=True,
+            side_effect=KeyError,
+        ),
     ):
         gather_stats_on_multiple_packages(typeshed_dir=typeshed)
```

### Comparing `typeshed_stats-23.2.1/tests/test_running_from_command_line.py` & `typeshed_stats-24.5.21/tests/test_running_from_command_line.py`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/tests/test_serialize.py` & `typeshed_stats-24.5.21/tests/test_serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import markdown
 import pytest
 from bs4 import BeautifulSoup
 
 from typeshed_stats.gather import (
     AnnotationStats,
+    CompletenessLevel,
     FileInfo,
     PackageInfo,
     PackageStatus,
     PyrightSetting,
     StubtestSettings,
     StubtestStrictness,
     UploadStatus,
@@ -58,15 +59,17 @@
 
 
 @pytest.fixture
 def unusual_packages() -> list[PackageInfo]:
     pkg1 = PackageInfo(
         "foo",
         stub_distribution_name="types-foo-ts",
+        upstream_url=None,
         extra_description="a very fooey package",
+        completeness_level=CompletenessLevel.PARTIAL,
         number_of_lines=100_000_000_000,
         package_status=PackageStatus.UP_TO_DATE,
         upload_status=UploadStatus.NOT_CURRENTLY_UPLOADED,
         stubtest_settings=StubtestSettings(
             strictness=StubtestStrictness.SKIPPED, platforms=[], allowlist_length=0
         ),
         pyright_setting=PyrightSetting.STRICT,
```

### Comparing `typeshed_stats-23.2.1/.gitignore` & `typeshed_stats-24.5.21/.gitignore`

 * *Files 12% similar despite different names*

```diff
@@ -69,7 +69,10 @@
 env/
 
 # Mypy cache
 .mypy_cache/
 
 # mkdocs documentation
 site/
+
+# autogenerated by hatch-vcs at build time
+src/typeshed_stats/_version.py
```

### Comparing `typeshed_stats-23.2.1/LICENSE` & `typeshed_stats-24.5.21/LICENSE`

 * *Files identical despite different names*

### Comparing `typeshed_stats-23.2.1/README.md` & `typeshed_stats-24.5.21/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 <div align=center>
 
 # typeshed-stats
 
-<img src="https://user-images.githubusercontent.com/66076021/202873196-3af493e6-bca0-4c1a-8853-73635b5c1ca8.png" width="500">
+<img src="https://raw.githubusercontent.com/AlexWaygood/typeshed-stats/main/stats_website/big_logo.png" width="500" alt="A Python in a field of wheat with a shed behind it, golden-red sunset in the background">
 
 <br>
 
 ---
 
 ## A CLI tool and library to gather stats on [typeshed](https://github.com/python/typeshed)
 
 <br>
 
-[![website](https://img.shields.io/website?down_color=red&down_message=Offline&style=for-the-badge&up_color=green&up_message=Running&url=https%3A%2F%2Falexwaygood.github.io%2Ftypeshed-stats%2F)](https://alexwaygood.github.io/typeshed-stats/)[![build status](https://img.shields.io/github/actions/workflow/status/AlexWaygood/typeshed-stats/test.yml?branch=main&label=Tests&style=for-the-badge)](https://github.com/AlexWaygood/typeshed-stats/actions/workflows/test.yml)[![Coveralls](https://img.shields.io/coverallsCoverage/github/AlexWaygood/typeshed-stats?style=for-the-badge)](https://coveralls.io/github/AlexWaygood/typeshed-stats)
+[![website](https://img.shields.io/website?down_color=red&down_message=Offline&style=for-the-badge&up_color=green&up_message=Running&url=https%3A%2F%2Falexwaygood.github.io%2Ftypeshed-stats%2F)](https://alexwaygood.github.io/typeshed-stats/)[![build status](https://img.shields.io/github/actions/workflow/status/AlexWaygood/typeshed-stats/test.yml?branch=main&label=Tests&style=for-the-badge)](https://github.com/AlexWaygood/typeshed-stats/actions/workflows/test.yml)
 <br>
-[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue?style=for-the-badge)](http://mypy-lang.org/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=for-the-badge&labelColor=ef8336)](https://pycqa.github.io/isort/)[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://pre-commit.ci)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue?style=for-the-badge)](http://mypy-lang.org/)[![Code style: Ruff](https://img.shields.io/badge/Code_style-Ruff-D7FF64?style=for-the-badge&logo=ruff)](https://github.com/astral-sh/ruff)[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://pre-commit.ci)
 <br>
-[![PyPI](https://img.shields.io/pypi/v/typeshed-stats?style=for-the-badge)](https://pypi.org/project/typeshed-stats/)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/typeshed-stats?style=for-the-badge)![PyPI - Wheel](https://img.shields.io/pypi/wheel/typeshed-stats?style=for-the-badge)[![license](https://img.shields.io/github/license/AlexWaygood/typeshed-stats?style=for-the-badge)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/typeshed-stats?style=for-the-badge)](https://pypi.org/project/typeshed-stats/)![PyPI - Wheel](https://img.shields.io/pypi/wheel/typeshed-stats?style=for-the-badge)[![license](https://img.shields.io/github/license/AlexWaygood/typeshed-stats?style=for-the-badge)](https://opensource.org/licenses/MIT)
 
 ---
 
 <br>
 </div>
 
 ## What's this project for?
```

### Comparing `typeshed_stats-23.2.1/PKG-INFO` & `typeshed_stats-24.5.21/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: typeshed_stats
-Version: 23.2.1
+Version: 24.5.21
 Summary: Library and command-line tool to gather stats on typeshed packages
 Project-URL: Homepage, https://github.com/AlexWaygood/typeshed-stats
 Project-URL: Bug Tracker, https://github.com/AlexWaygood/typeshed-stats/issues
 Author-email: Alex Waygood <alex.waygood@gmail.com>
 License: MIT
 License-File: LICENSE
 Keywords: stubs,typeshed,typing
@@ -12,109 +12,120 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
-Requires-Dist: aiohttp[speedups]
+Requires-Dist: aiohttp>=3.9.0; python_version >= '3.13'
+Requires-Dist: aiohttp[speedups]>=3.9.0; python_version < '3.13'
 Requires-Dist: attrs>=22.2.0
 Requires-Dist: cattrs
 Requires-Dist: jinja2>=3
 Requires-Dist: packaging
+Requires-Dist: pathspec>=0.10.3
 Requires-Dist: tomli; python_version < '3.11'
 Provides-Extra: dev
-Requires-Dist: aiohttp; extra == 'dev'
-Requires-Dist: attrs>=22.2.0; extra == 'dev'
 Requires-Dist: beautifulsoup4<5,>=4; extra == 'dev'
-Requires-Dist: black==23.1.0; extra == 'dev'
-Requires-Dist: blacken-docs==1.12.1; extra == 'dev'
-Requires-Dist: cattrs; extra == 'dev'
-Requires-Dist: covdefaults==2.2.2; extra == 'dev'
-Requires-Dist: coverage==6.5.0; extra == 'dev'
-Requires-Dist: flake8-bugbear==23.1.20; extra == 'dev'
-Requires-Dist: flake8-docstrings==1.6.0; extra == 'dev'
-Requires-Dist: flake8-noqa==1.3.0; extra == 'dev'
-Requires-Dist: flake8-pytest-style==1.6.0; extra == 'dev'
-Requires-Dist: flake8-simplify==0.19.3; extra == 'dev'
-Requires-Dist: flake8==6.0.0; extra == 'dev'
-Requires-Dist: isort==5.12.0; extra == 'dev'
-Requires-Dist: jinja2>=3; extra == 'dev'
+Requires-Dist: covdefaults==2.3.0; extra == 'dev'
+Requires-Dist: coverage==7.4.4; extra == 'dev'
 Requires-Dist: markdown<4,>=3; extra == 'dev'
-Requires-Dist: markdown==3.3.7; extra == 'dev'
-Requires-Dist: mkdocs-macros-plugin==0.7.0; extra == 'dev'
-Requires-Dist: mkdocs-material==9.0.1; extra == 'dev'
-Requires-Dist: mkdocs==1.4.2; extra == 'dev'
-Requires-Dist: mkdocstrings[python]==0.19.1; extra == 'dev'
-Requires-Dist: mypy==1.0.1; extra == 'dev'
-Requires-Dist: packaging; extra == 'dev'
-Requires-Dist: pre-commit-hooks==4.4.0; extra == 'dev'
-Requires-Dist: pycln==2.1.2; extra == 'dev'
+Requires-Dist: markdown==3.5.2; extra == 'dev'
+Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'dev'
+Requires-Dist: mkdocs-material==9.5.16; extra == 'dev'
+Requires-Dist: mkdocs==1.5.3; extra == 'dev'
+Requires-Dist: mkdocstrings-python==1.9.0; extra == 'dev'
+Requires-Dist: mkdocstrings==0.24.1; extra == 'dev'
+Requires-Dist: mypy==1.9.0; extra == 'dev'
 Requires-Dist: pytest-antilru==1.1.1; extra == 'dev'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'dev'
-Requires-Dist: pytest-dependency==0.5.1; extra == 'dev'
-Requires-Dist: pytest-mock==3.10.0; extra == 'dev'
-Requires-Dist: pytest-subtests==0.9.0; extra == 'dev'
-Requires-Dist: pytest==7.2.0; extra == 'dev'
-Requires-Dist: pyupgrade==3.3.1; extra == 'dev'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'dev'
+Requires-Dist: pytest-dependency==0.6.0; extra == 'dev'
+Requires-Dist: pytest-mock==3.14.0; extra == 'dev'
+Requires-Dist: pytest-subtests==0.12.1; extra == 'dev'
+Requires-Dist: pytest==8.1.1; extra == 'dev'
 Requires-Dist: rich; extra == 'dev'
-Requires-Dist: rich-argparse>=0.6.0; extra == 'dev'
 Requires-Dist: rich-argparse>=1; extra == 'dev'
-Requires-Dist: tomli; python_version < '3.11' and extra == 'dev'
-Requires-Dist: types-beautifulsoup4==4.11.6.1; extra == 'dev'
-Requires-Dist: types-markdown==3.4.2.1; extra == 'dev'
+Requires-Dist: ruff==0.3.5; extra == 'dev'
+Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == 'dev'
+Requires-Dist: types-markdown==3.6.0.20240316; extra == 'dev'
 Provides-Extra: docs
-Requires-Dist: markdown==3.3.7; extra == 'docs'
-Requires-Dist: mkdocs-macros-plugin==0.7.0; extra == 'docs'
-Requires-Dist: mkdocs-material==9.0.1; extra == 'docs'
-Requires-Dist: mkdocs==1.4.2; extra == 'docs'
-Requires-Dist: mkdocstrings[python]==0.19.1; extra == 'docs'
+Requires-Dist: markdown==3.5.2; extra == 'docs'
+Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'docs'
+Requires-Dist: mkdocs-material==9.5.16; extra == 'docs'
+Requires-Dist: mkdocs==1.5.3; extra == 'docs'
+Requires-Dist: mkdocstrings-python==1.9.0; extra == 'docs'
+Requires-Dist: mkdocstrings==0.24.1; extra == 'docs'
 Requires-Dist: rich; extra == 'docs'
 Requires-Dist: rich-argparse>=1; extra == 'docs'
+Provides-Extra: misc-lint
+Requires-Dist: ruff==0.3.5; extra == 'misc-lint'
 Provides-Extra: pytest
 Requires-Dist: beautifulsoup4<5,>=4; extra == 'pytest'
-Requires-Dist: covdefaults==2.2.2; extra == 'pytest'
-Requires-Dist: coverage==6.5.0; extra == 'pytest'
+Requires-Dist: covdefaults==2.3.0; extra == 'pytest'
+Requires-Dist: coverage==7.4.4; extra == 'pytest'
 Requires-Dist: markdown<4,>=3; extra == 'pytest'
 Requires-Dist: pytest-antilru==1.1.1; extra == 'pytest'
-Requires-Dist: pytest-asyncio==0.20.3; extra == 'pytest'
-Requires-Dist: pytest-dependency==0.5.1; extra == 'pytest'
-Requires-Dist: pytest-mock==3.10.0; extra == 'pytest'
-Requires-Dist: pytest-subtests==0.9.0; extra == 'pytest'
-Requires-Dist: pytest==7.2.0; extra == 'pytest'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'pytest'
+Requires-Dist: pytest-dependency==0.6.0; extra == 'pytest'
+Requires-Dist: pytest-mock==3.14.0; extra == 'pytest'
+Requires-Dist: pytest-subtests==0.12.1; extra == 'pytest'
+Requires-Dist: pytest==8.1.1; extra == 'pytest'
 Requires-Dist: rich; extra == 'pytest'
 Requires-Dist: rich-argparse>=1; extra == 'pytest'
-Requires-Dist: tomli; python_version < '3.11' and extra == 'pytest'
 Provides-Extra: rich
 Requires-Dist: rich; extra == 'rich'
 Requires-Dist: rich-argparse>=1; extra == 'rich'
+Provides-Extra: typecheck
+Requires-Dist: beautifulsoup4<5,>=4; extra == 'typecheck'
+Requires-Dist: covdefaults==2.3.0; extra == 'typecheck'
+Requires-Dist: coverage==7.4.4; extra == 'typecheck'
+Requires-Dist: markdown<4,>=3; extra == 'typecheck'
+Requires-Dist: markdown==3.5.2; extra == 'typecheck'
+Requires-Dist: mkdocs-macros-plugin==1.0.5; extra == 'typecheck'
+Requires-Dist: mkdocs-material==9.5.16; extra == 'typecheck'
+Requires-Dist: mkdocs==1.5.3; extra == 'typecheck'
+Requires-Dist: mkdocstrings-python==1.9.0; extra == 'typecheck'
+Requires-Dist: mkdocstrings==0.24.1; extra == 'typecheck'
+Requires-Dist: mypy==1.9.0; extra == 'typecheck'
+Requires-Dist: pytest-antilru==1.1.1; extra == 'typecheck'
+Requires-Dist: pytest-asyncio==0.23.6; extra == 'typecheck'
+Requires-Dist: pytest-dependency==0.6.0; extra == 'typecheck'
+Requires-Dist: pytest-mock==3.14.0; extra == 'typecheck'
+Requires-Dist: pytest-subtests==0.12.1; extra == 'typecheck'
+Requires-Dist: pytest==8.1.1; extra == 'typecheck'
+Requires-Dist: rich; extra == 'typecheck'
+Requires-Dist: rich-argparse>=1; extra == 'typecheck'
+Requires-Dist: types-beautifulsoup4==4.12.0.20240229; extra == 'typecheck'
+Requires-Dist: types-markdown==3.6.0.20240316; extra == 'typecheck'
 Description-Content-Type: text/markdown
 
 <div align=center>
 
 # typeshed-stats
 
-<img src="https://user-images.githubusercontent.com/66076021/202873196-3af493e6-bca0-4c1a-8853-73635b5c1ca8.png" width="500">
+<img src="https://raw.githubusercontent.com/AlexWaygood/typeshed-stats/main/stats_website/big_logo.png" width="500" alt="A Python in a field of wheat with a shed behind it, golden-red sunset in the background">
 
 <br>
 
 ---
 
 ## A CLI tool and library to gather stats on [typeshed](https://github.com/python/typeshed)
 
 <br>
 
-[![website](https://img.shields.io/website?down_color=red&down_message=Offline&style=for-the-badge&up_color=green&up_message=Running&url=https%3A%2F%2Falexwaygood.github.io%2Ftypeshed-stats%2F)](https://alexwaygood.github.io/typeshed-stats/)[![build status](https://img.shields.io/github/actions/workflow/status/AlexWaygood/typeshed-stats/test.yml?branch=main&label=Tests&style=for-the-badge)](https://github.com/AlexWaygood/typeshed-stats/actions/workflows/test.yml)[![Coveralls](https://img.shields.io/coverallsCoverage/github/AlexWaygood/typeshed-stats?style=for-the-badge)](https://coveralls.io/github/AlexWaygood/typeshed-stats)
+[![website](https://img.shields.io/website?down_color=red&down_message=Offline&style=for-the-badge&up_color=green&up_message=Running&url=https%3A%2F%2Falexwaygood.github.io%2Ftypeshed-stats%2F)](https://alexwaygood.github.io/typeshed-stats/)[![build status](https://img.shields.io/github/actions/workflow/status/AlexWaygood/typeshed-stats/test.yml?branch=main&label=Tests&style=for-the-badge)](https://github.com/AlexWaygood/typeshed-stats/actions/workflows/test.yml)
 <br>
-[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue?style=for-the-badge)](http://mypy-lang.org/)[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=for-the-badge)](https://github.com/psf/black)[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=for-the-badge&labelColor=ef8336)](https://pycqa.github.io/isort/)[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://pre-commit.ci)
+[![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue?style=for-the-badge)](http://mypy-lang.org/)[![Code style: Ruff](https://img.shields.io/badge/Code_style-Ruff-D7FF64?style=for-the-badge&logo=ruff)](https://github.com/astral-sh/ruff)[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=for-the-badge)](https://pre-commit.ci)
 <br>
-[![PyPI](https://img.shields.io/pypi/v/typeshed-stats?style=for-the-badge)](https://pypi.org/project/typeshed-stats/)![PyPI - Python Version](https://img.shields.io/pypi/pyversions/typeshed-stats?style=for-the-badge)![PyPI - Wheel](https://img.shields.io/pypi/wheel/typeshed-stats?style=for-the-badge)[![license](https://img.shields.io/github/license/AlexWaygood/typeshed-stats?style=for-the-badge)](https://opensource.org/licenses/MIT)
+[![PyPI](https://img.shields.io/pypi/v/typeshed-stats?style=for-the-badge)](https://pypi.org/project/typeshed-stats/)![PyPI - Wheel](https://img.shields.io/pypi/wheel/typeshed-stats?style=for-the-badge)[![license](https://img.shields.io/github/license/AlexWaygood/typeshed-stats?style=for-the-badge)](https://opensource.org/licenses/MIT)
 
 ---
 
 <br>
 </div>
 
 ## What's this project for?
```

