# Comparing `tmp/feincms3_data-0.6.0.tar.gz` & `tmp/feincms3_data-0.6.1.tar.gz`

## Comparing `feincms3_data-0.6.0.tar` & `feincms3_data-0.6.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.editorconfig
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.readthedocs.yml
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/CHANGELOG.rst
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tox.ini
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/Makefile
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/conf.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/index.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/docs/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/__init__.py
--rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/data.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/serializers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/f3dumpdata.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/feincms3_data/management/commands/f3loaddata.py
--rwxr-xr-x   0        0        0      331 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/manage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/__init__.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/models.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/settings.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/specs.py
--rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/tests/testapp/test_data.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/.gitignore
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/LICENSE
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/README.rst
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 feincms3_data-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/.editorconfig
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/.readthedocs.yml
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/CHANGELOG.rst
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tox.ini
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/docs/Makefile
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/docs/index.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/docs/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/__init__.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/data.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/serializers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/management/commands/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/management/commands/f3dumpdata.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/feincms3_data/management/commands/f3loaddata.py
+-rwxr-xr-x   0        0        0      331 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/manage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/testapp/__init__.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/testapp/models.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/testapp/settings.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/testapp/specs.py
+-rw-r--r--   0        0        0    18692 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/tests/testapp/test_data.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/README.rst
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 feincms3_data-0.6.1/PKG-INFO
```

### Comparing `feincms3_data-0.6.0/.pre-commit-config.yaml` & `feincms3_data-0.6.1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 exclude: ".yarn/|yarn.lock|\\.min\\.(css|js)$"
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-builtin-literals
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
   - repo: https://github.com/adamchainz/django-upgrade
-    rev: 1.13.0
+    rev: 1.17.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "3.2"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
-  - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.272"
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: "v0.4.4"
     hooks:
       - id: ruff
-  - repo: https://github.com/psf/black
-    rev: 23.3.0
-    hooks:
-      - id: black
+      - id: ruff-format
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.9-for-vscode
+    rev: v3.1.0
     hooks:
       - id: prettier
         args: [--list-different, --no-semi]
         exclude: "^conf/|.*\\.html$"
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.11.2
+    rev: 2.1.3
     hooks:
       - id: pyproject-fmt
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.13
+    rev: v0.18
     hooks:
       - id: validate-pyproject
```

### Comparing `feincms3_data-0.6.0/CHANGELOG.rst` & `feincms3_data-0.6.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ==========
 Change log
 ==========
 
 `Next version`_
 ~~~~~~~~~~~~~~~
 
+- Added ``./manage.py f3dumpdata -`` which allows reading JSON data from stdin.
+- Added Python 3.12 and Django 5.0.
+
 
 0.6 (2023-06-12)
 ~~~~~~~~~~~~~~~~
 
 - Fixed the broken argument validation of ``./manage.py f3dumpdata``.
 - Switched to hatchling and ruff.
 - Made ``specs_for_*_models`` helpers return a list instead of a generator.
```

### Comparing `feincms3_data-0.6.0/tox.ini` & `feincms3_data-0.6.1/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tox]
 envlist =
     py{38,39,310}-dj{32,40,41,42}
-    py{310,311}-dj{32,40,41,42,main}
+    py{310,311,312}-dj{32,40,41,42,50,main}
 
 [testenv]
 usedevelop = true
 extras = all,tests
 commands =
     python -Wd {envbindir}/coverage run tests/manage.py test -v2 --keepdb {posargs:testapp}
     coverage report -m
 deps =
     dj32: Django>=3.2,<4.0
     dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
     dj42: Django>=4.2,<5.0
+    dj50: Django>=5.0,<5.1
     djmain: https://github.com/django/django/archive/main.tar.gz
 
 [testenv:docs]
 deps =
     Sphinx
     sphinx-rtd-theme
     Django
```

### Comparing `feincms3_data-0.6.0/.github/workflows/tests.yml` & `feincms3_data-0.6.1/.github/workflows/tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -14,14 +14,15 @@
       fail-fast: false
       matrix:
         python-version:
           - "3.8"
           - "3.9"
           - "3.10"
           - "3.11"
+          - "3.12"
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `feincms3_data-0.6.0/docs/Makefile` & `feincms3_data-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/docs/conf.py` & `feincms3_data-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/docs/make.bat` & `feincms3_data-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/feincms3_data/data.py` & `feincms3_data-0.6.1/feincms3_data/data.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/feincms3_data/management/commands/f3dumpdata.py` & `feincms3_data-0.6.1/feincms3_data/management/commands/f3dumpdata.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/feincms3_data/management/commands/f3loaddata.py` & `feincms3_data-0.6.1/feincms3_data/management/commands/f3loaddata.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import sys
 
 from django.core.management.base import BaseCommand
 
 from feincms3_data.data import load_dump, silence
 
 
 class Command(BaseCommand):
@@ -18,14 +19,17 @@
                 " currently exist on the model."
             ),
         )
         parser.add_argument("args", metavar="dump", nargs="+", help="Dumps.")
 
     def handle(self, *dumps, **options):
         for dump in dumps:
-            with open(dump, encoding="utf-8") as f:
-                data = json.load(f)
+            if dump == "-":
+                data = json.loads(sys.stdin.read())
+            else:
+                with open(dump, encoding="utf-8") as f:
+                    data = json.load(f)
             load_dump(
                 data,
                 progress=self.stderr.write if options["verbosity"] >= 2 else silence,
                 ignorenonexistent=options["ignorenonexistent"],
             )
```

### Comparing `feincms3_data-0.6.0/tests/testapp/models.py` & `feincms3_data-0.6.1/tests/testapp/models.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/tests/testapp/settings.py` & `feincms3_data-0.6.1/tests/testapp/settings.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/tests/testapp/test_data.py` & `feincms3_data-0.6.1/tests/testapp/test_data.py`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/LICENSE` & `feincms3_data-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/README.rst` & `feincms3_data-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `feincms3_data-0.6.0/pyproject.toml` & `feincms3_data-0.6.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,107 +3,101 @@
 requires = [
   "hatchling",
 ]
 
 [project]
 name = "feincms3-data"
 readme = "README.rst"
-license = {text = "BSD-3-Clause"}
+license = { text = "BSD-3-Clause" }
 authors = [
-    { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
+  { name = "Matthias Kestenholz", email = "mk@feinheit.ch" },
 ]
 requires-python = ">=3.8"
 classifiers = [
   "Environment :: Web Environment",
   "Framework :: Django",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
   "Topic :: Software Development",
   "Topic :: Software Development :: Libraries :: Application Frameworks",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  "Django>=3.2",
+  "django>=3.2",
 ]
-[project.optional-dependencies]
-tests = [
+optional-dependencies.tests = [
   "coverage",
 ]
-[project.urls]
-Homepage = "https://github.com/matthiask/feincms3-data/"
+urls.Homepage = "https://github.com/matthiask/feincms3-data/"
 
 [tool.hatch.version]
 path = "feincms3_data/__init__.py"
 
 [tool.ruff]
-extend-select = [
-  # pyflakes, pycodestyle
-  "F", "E", "W",
-  # mmcabe
-  "C90",
-  # isort
-  "I",
-  # pep8-naming
-  "N",
-  # pyupgrade
-  "UP",
-  # flake8-2020
-  "YTT",
-  # flake8-boolean-trap
-  "FBT",
+target-version = "py38"
+
+fix = true
+show-fixes = true
+lint.extend-select = [
   # flake8-bugbear
   "B",
-  # flake8-builtins
-  "A",
   # flake8-comprehensions
   "C4",
+  # mmcabe
+  "C90",
   # flake8-django
   "DJ",
+  "E",
+  # pyflakes, pycodestyle
+  "F",
+  # flake8-boolean-trap
+  "FBT",
   # flake8-logging-format
   "G",
-  # flake8-pie
-  "PIE",
-  # flake8-simplify
-  "SIM",
+  # isort
+  "I",
   # flake8-gettext
   "INT",
+  # pep8-naming
+  "N",
   # pygrep-hooks
   "PGH",
+  # flake8-pie
+  "PIE",
   # pylint
   "PL",
   # unused noqa
   "RUF100",
+  # flake8-simplify
+  "SIM",
+  # pyupgrade
+  "UP",
+  "W",
+  # flake8-2020
+  "YTT",
 ]
-extend-ignore = [
+lint.extend-ignore = [
   # Allow zip() without strict=
   "B905",
   # No line length errors
   "E501",
 ]
-fix = true
-show-fixes = true
-target-version = "py38"
-
-[tool.ruff.isort]
-combine-as-imports = true
-lines-after-imports = 2
-
-[tool.ruff.mccabe]
-max-complexity = 15
-
-[tool.ruff.per-file-ignores]
-"*/migrat*/*" = [
+lint.per-file-ignores."*/migrat*/*" = [
   # Allow using PascalCase model names in migrations
   "N806",
   # Ignore the fact that migration files are invalid module names
   "N999",
 ]
+lint.isort.combine-as-imports = true
+lint.isort.lines-after-imports = 2
+lint.mccabe.max-complexity = 15
```

### Comparing `feincms3_data-0.6.0/PKG-INFO` & `feincms3_data-0.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: feincms3-data
-Version: 0.6.0
+Version: 0.6.1
 Project-URL: Homepage, https://github.com/matthiask/feincms3-data/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Requires-Dist: django>=3.2
 Provides-Extra: tests
 Requires-Dist: coverage; extra == 'tests'
```

