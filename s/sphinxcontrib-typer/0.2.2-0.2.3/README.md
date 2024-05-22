# Comparing `tmp/sphinxcontrib_typer-0.2.2.tar.gz` & `tmp/sphinxcontrib_typer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib_typer-0.2.2.tar", max compression
+gzip compressed data, was "sphinxcontrib_typer-0.2.3.tar", max compression
```

## Comparing `sphinxcontrib_typer-0.2.2.tar` & `sphinxcontrib_typer-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.2.2/LICENSE
--rw-r--r--   0        0        0     5272 2024-05-15 04:52:56.770601 sphinxcontrib_typer-0.2.2/README.md
--rw-r--r--   0        0        0     2914 2024-05-15 05:55:36.320976 sphinxcontrib_typer-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    34219 2024-05-15 05:54:45.783863 sphinxcontrib_typer-0.2.2/sphinxcontrib/typer/__init__.py
--rw-r--r--   0        0        0     6899 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-12-14 00:10:27.893967 sphinxcontrib_typer-0.2.3/LICENSE
+-rw-r--r--   0        0        0     5323 2024-05-18 14:56:08.366192 sphinxcontrib_typer-0.2.3/README.md
+-rw-r--r--   0        0        0     2914 2024-05-22 16:54:07.852818 sphinxcontrib_typer-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    34497 2024-05-22 17:06:43.503141 sphinxcontrib_typer-0.2.3/sphinxcontrib/typer/__init__.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 sphinxcontrib_typer-0.2.3/PKG-INFO
```

### Comparing `sphinxcontrib_typer-0.2.2/LICENSE` & `sphinxcontrib_typer-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib_typer-0.2.2/README.md` & `sphinxcontrib_typer-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer)
 [![Documentation Status](https://readthedocs.org/projects/sphinxcontrib-typer/badge/?version=latest)](http://sphinxcontrib-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/sphinx-contrib/typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://app.codecov.io/gh/sphinx-contrib/typer)
 [![Test Status](https://github.com/sphinx-contrib/typer/workflows/test/badge.svg)](https://github.com/sphinx-contrib/typer/actions/workflows/test.yml)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 # sphinxcontrib-typer
 
 A Sphinx directive for auto generating docs for [Typer](https://typer.tiangolo.com/) 
 (and [Click](https://click.palletsprojects.com/) commands!) using the rich console
 formatting available in [Typer](https://typer.tiangolo.com/). This package generates
 concise command documentation in text, html or svg formats out of the box, but if your
```

### Comparing `sphinxcontrib_typer-0.2.2/pyproject.toml` & `sphinxcontrib_typer-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxcontrib-typer"
-version = "0.2.2"
+version = "0.2.3"
 description = "Auto generate docs for typer commands."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sphinx-contrib/typer"
 homepage = "https://sphinxcontrib-typer.readthedocs.io"
 classifiers = [
```

### Comparing `sphinxcontrib_typer-0.2.2/sphinxcontrib/typer/__init__.py` & `sphinxcontrib_typer-0.2.3/sphinxcontrib/typer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from sphinx.util import logging
 
 from typer import rich_utils as typer_rich_utils
 from typer.main import Typer, TyperGroup
 from typer.main import get_command as get_typer_command
 from typer.models import Context as TyperContext
 
-VERSION = (0, 2, 2)
+VERSION = (0, 2, 3)
 
 __title__ = "SphinxContrib Typer"
 __version__ = ".".join(str(i) for i in VERSION)
 __author__ = "Brian Kohan"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Brian Kohan"
 
@@ -581,17 +581,21 @@
             )
         else:
             supported = builder_targets[self.builder]
             self.target = (
                 self.preferred if self.preferred in supported else supported[0]
             )
 
-        return self.generate_nodes(
-            self.prog_name, command, getattr(self, "parent", None)
-        )
+        parent = getattr(self, "parent", None)
+        if parent and self.options.get("prog", None):
+            # we unset this because we're not at the root command and this gets
+            # messed up for whatever reason
+            # https://github.com/sphinx-contrib/typer/issues/24
+            parent.info_name = ""
+        return self.generate_nodes(self.prog_name, command, parent)
 
 
 def typer_get_iframe_height(
     directive: TyperDirective, normal_cmd: str, html_page: str
 ) -> int:
     """
     The default iframe height calculation function. The iframe height resolution proceeds as
```

### Comparing `sphinxcontrib_typer-0.2.2/PKG-INFO` & `sphinxcontrib_typer-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-typer
-Version: 0.2.2
+Version: 0.2.3
 Summary: Auto generate docs for typer commands.
 Home-page: https://sphinxcontrib-typer.readthedocs.io
 License: MIT
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -41,15 +41,15 @@
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer/)
 [![PyPI status](https://img.shields.io/pypi/status/sphinxcontrib-typer.svg)](https://pypi.python.org/pypi/sphinxcontrib-typer)
 [![Documentation Status](https://readthedocs.org/projects/sphinxcontrib-typer/badge/?version=latest)](http://sphinxcontrib-typer.readthedocs.io/?badge=latest/)
 [![Code Cov](https://codecov.io/gh/sphinx-contrib/typer/branch/main/graph/badge.svg?token=0IZOKN2DYL)](https://app.codecov.io/gh/sphinx-contrib/typer)
 [![Test Status](https://github.com/sphinx-contrib/typer/workflows/test/badge.svg)](https://github.com/sphinx-contrib/typer/actions/workflows/test.yml)
-[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 # sphinxcontrib-typer
 
 A Sphinx directive for auto generating docs for [Typer](https://typer.tiangolo.com/) 
 (and [Click](https://click.palletsprojects.com/) commands!) using the rich console
 formatting available in [Typer](https://typer.tiangolo.com/). This package generates
 concise command documentation in text, html or svg formats out of the box, but if your
```

