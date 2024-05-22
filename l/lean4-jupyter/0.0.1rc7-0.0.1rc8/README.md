# Comparing `tmp/lean4_jupyter-0.0.1rc7.tar.gz` & `tmp/lean4_jupyter-0.0.1rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lean4_jupyter-0.0.1rc7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lean4_jupyter-0.0.1rc8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lean4_jupyter-0.0.1rc7.tar` & `lean4_jupyter-0.0.1rc8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0       30 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.flake8
--rw-r--r--   0        0        0     2031 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3096 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/.gitignore
--rw-r--r--   0        0        0     1069 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/LICENSE
--rw-r--r--   0        0        0     5034 2024-05-16 10:37:33.849804 lean4_jupyter-0.0.1rc7/README.md
--rw-r--r--   0        0        0    67337 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/00_tutorial.ipynb
--rw-r--r--   0        0        0    11782 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/01_cd.ipynb
--rw-r--r--   0        0        0    19404 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/02_load.ipynb
--rw-r--r--   0        0        0    35042 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/03_import.ipynb
--rw-r--r--   0        0        0        7 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/.gitignore
--rw-r--r--   0        0        0      154 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj.lean
--rw-r--r--   0        0        0       37 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj/Basic.lean
--rw-r--r--   0        0        0       70 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/DemoProj/Standalone.lean
--rw-r--r--   0        0        0     2171 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lake-manifest.json
--rw-r--r--   0        0        0      505 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lakefile.lean
--rw-r--r--   0        0        0       28 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/demo_proj/lean-toolchain
--rw-r--r--   0        0        0    11222 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-msg.ipynb
--rw-r--r--   0        0        0    10532 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-sorries.ipynb
--rw-r--r--   0        0        0       91 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/__init__.py
--rw-r--r--   0        0        0      129 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/__main__.py
--rw-r--r--   0        0        0     9058 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/display.py
--rw-r--r--   0        0        0     2134 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/install.py
--rw-r--r--   0        0        0     3251 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/kernel.py
--rw-r--r--   0        0        0     7359 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/repl.py
--rw-r--r--   0        0        0       86 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/__init__.py
--rw-r--r--   0        0        0    11263 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/lean_logo.svg
--rw-r--r--   0        0        0      728 2024-05-16 10:37:33.853804 lean4_jupyter-0.0.1rc7/pyproject.toml
--rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc7/setup.py
--rw-r--r--   0        0        0     5650 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc7/PKG-INFO
+-rw-r--r--   0        0        0       52 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/.flake8
+-rw-r--r--   0        0        0     3263 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3096 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/.gitignore
+-rw-r--r--   0        0        0     1069 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/LICENSE
+-rw-r--r--   0        0        0     5215 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/README.md
+-rw-r--r--   0        0        0    67337 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/00_tutorial.ipynb
+-rw-r--r--   0        0        0    11782 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/01_cd.ipynb
+-rw-r--r--   0        0        0    19404 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/02_load.ipynb
+-rw-r--r--   0        0        0    35042 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/03_import.ipynb
+-rw-r--r--   0        0        0        7 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/.gitignore
+-rw-r--r--   0        0        0      154 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/DemoProj.lean
+-rw-r--r--   0        0        0       37 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/DemoProj/Basic.lean
+-rw-r--r--   0        0        0       70 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/DemoProj/Standalone.lean
+-rw-r--r--   0        0        0     2171 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/lake-manifest.json
+-rw-r--r--   0        0        0      505 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/lakefile.lean
+-rw-r--r--   0        0        0       28 2024-05-16 13:06:14.883910 lean4_jupyter-0.0.1rc8/examples/demo_proj/lean-toolchain
+-rw-r--r--   0        0        0    11222 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/examples/repl-issue-40-dup-msg.ipynb
+-rw-r--r--   0        0        0    10532 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/examples/repl-issue-40-dup-sorries.ipynb
+-rw-r--r--   0        0        0       91 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/__main__.py
+-rw-r--r--   0        0        0     9058 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/display.py
+-rw-r--r--   0        0        0     2134 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/install.py
+-rw-r--r--   0        0        0     3251 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/kernel.py
+-rw-r--r--   0        0        0     7359 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/repl.py
+-rw-r--r--   0        0        0       87 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/resources/__init__.py
+-rw-r--r--   0        0        0    11263 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/lean4_jupyter/resources/lean_logo.svg
+-rw-r--r--   0        0        0      916 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/pyproject.toml
+-rwxr-xr-x   0        0        0      430 2024-05-16 13:06:14.887910 lean4_jupyter-0.0.1rc8/scripts/install_repl.sh
+-rw-r--r--   0        0        0      712 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc8/setup.py
+-rw-r--r--   0        0        0     6014 1970-01-01 00:00:00.000000 lean4_jupyter-0.0.1rc8/PKG-INFO
```

### Comparing `lean4_jupyter-0.0.1rc7/.github/workflows/ci.yml` & `lean4_jupyter-0.0.1rc8/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -23,28 +23,55 @@
         && !contains(github.event.head_commit.message, '[skip tests]')
     strategy:
       matrix:
         python-version: ["3.11"]
       fail-fast: false
     runs-on: ubuntu-latest
     steps:
-    - name: Checkout
-      uses: actions/checkout@v3
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v4
-      with:
-        python-version: ${{ matrix.python-version }}
-    # - name: Install dependencies
-    #   run: |
-    #     python -m pip install -r test_requirements.txt
-    #     python -m pip install -e .
-    #     python -m pip check
-    # - name: Lint
-    #   run: |
-    #     flake8 -v
+      - name: Checkout
+        uses: actions/checkout@v4
+        with:
+          submodules: recursive
+      - name: Install Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Install dependencies
+        run: |
+          python -m pip install -e ".[test]"
+      - name: Lint
+        run: |
+          flake8 -v
+      - name: Install elan
+        run: |
+          set -o pipefail
+          curl https://raw.githubusercontent.com/leanprover/elan/master/elan-init.sh -sSf | bash -s -- -y --default-toolchain none
+          echo "$HOME/.elan/bin" >> $GITHUB_PATH
+      - name: Install repl
+        run: |
+          set -o pipefail
+          ./scripts/install_repl.sh
+      - name: Install Lean 4 Jupyter Kernel
+        run: |
+          python -m lean4_jupyter.install
+      - name: Try run kernel
+        run: |
+          python -m lean4_jupyter.kernel --help
+      # - name: Try run kernel with papermill
+      #   run: |
+      #     python -m papermill --kernel lean4 examples/repl-issue-40-dup-msg.ipynb examples/repl-issue-40-dup-msg.expected.ipynb
+      - name: Prepare Lean 4 toolchain and demo projects
+        run: |
+          set -o pipefail
+          elan default leanprover/lean4:v4.8.0-rc1
+          cd examples/demo_proj
+          lake exe cache get && lake build
+      - name: Test
+        run: |
+          pytest -vv --durations=50 --nbval --nbval-kernel-name lean4 examples/
 
   release:
     name: Create release and send to PyPI
     needs: build
     if: >-
         github.ref_type == 'tag'
         && startsWith(github.ref, 'refs/tags/v')
@@ -53,21 +80,27 @@
     runs-on: ubuntu-latest
     # https://github.com/pypa/gh-action-pypi-publish/tree/release/v1/?tab=readme-ov-file#trusted-publishing
     permissions:
       id-token: write
     environment:
       name: pypi
       url: https://pypi.org/p/lean4_jupyter
+    strategy:
+      matrix:
+        python-version: ["3.11"]
+      fail-fast: false
     steps:
-      - name: Check out code
-        uses: actions/checkout@v3
-      - name: Set up Python
-        uses: actions/setup-python@v4
+      - name: Checkout
+        uses: actions/checkout@v4
+        with:
+          submodules: recursive
+      - name: Install Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: ${{ matrix.python-version }}
       - name: Install flit
         run: |
           python -m pip install flit
       - name: Build package distributions
         run: |
           python -m flit build --setup-py
       - name: Publish package distributions to PyPI
```

### Comparing `lean4_jupyter-0.0.1rc7/.gitignore` & `lean4_jupyter-0.0.1rc8/.gitignore`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/LICENSE` & `lean4_jupyter-0.0.1rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/README.md` & `lean4_jupyter-0.0.1rc8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 A Lean 4 Jupyter kernel via [repl](https://github.com/leanprover-community/repl).
 
 [![PyPI](https://img.shields.io/pypi/v/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
 ![PyPI - License](https://img.shields.io/pypi/l/lean4_jupyter)
 ![PyPI - Status](https://img.shields.io/pypi/status/lean4_jupyter)
 [![Python CI](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml/badge.svg)](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml)
-[![Maintainability](https://api.codeclimate.com/v1/badges/666a7d45d436a598df2b/maintainability)](https://codeclimate.com/github/utensil/lean4_jupyter/maintainability) 
-
-## Status
-
-Alpha.
+[![lint - flake8](https://img.shields.io/badge/lint-flake8-blue)](https://github.com/PyCQA/flake8)
+[![Static Badge](https://img.shields.io/badge/test-nbval-purple)](https://github.com/computationalmodelling/nbval)
+[![Maintainability](https://api.codeclimate.com/v1/badges/666a7d45d436a598df2b/maintainability)](https://codeclimate.com/github/utensil/lean4_jupyter/maintainability)
 
 ## What's already working
 
 🔥 See it in action: [Tutorial notebook](https://nbviewer.org/github/utensil/lean4_jupyter/blob/main/examples/00_tutorial.ipynb?flush_cache=true).
 
 The kernel can:
 
@@ -32,15 +30,15 @@
 
 ## What's next
 
 - Fix [repl#40](https://github.com/leanprover-community/repl/issues/40) (PRed as [repl#41](https://github.com/leanprover-community/repl/issues/41))
 - Improve the alectryon annotation to support annotations in the middle of a line
 - Make magics like `%cd` and `%load` work more robustly
 - Support show `tactics` after `%load`
-- Add a CI based on [papermill](https://github.com/nteract/papermill/)
+- Add all `repl` test cases to the CI and set up coverage
 - Improve UI in Jupyter Dark themes
 - Minor code refactor to smooth things out
 
 ## Installation
 
 First, you need a working Lean 4 installation. You can install it via [elan](https://github.com/leanprover/elan).
```

### Comparing `lean4_jupyter-0.0.1rc7/examples/00_tutorial.ipynb` & `lean4_jupyter-0.0.1rc8/examples/00_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/01_cd.ipynb` & `lean4_jupyter-0.0.1rc8/examples/01_cd.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/02_load.ipynb` & `lean4_jupyter-0.0.1rc8/examples/02_load.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/03_import.ipynb` & `lean4_jupyter-0.0.1rc8/examples/03_import.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/demo_proj/lake-manifest.json` & `lean4_jupyter-0.0.1rc8/examples/demo_proj/lake-manifest.json`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-msg.ipynb` & `lean4_jupyter-0.0.1rc8/examples/repl-issue-40-dup-msg.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/examples/repl-issue-40-dup-sorries.ipynb` & `lean4_jupyter-0.0.1rc8/examples/repl-issue-40-dup-sorries.ipynb`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/lean4_jupyter/display.py` & `lean4_jupyter-0.0.1rc8/lean4_jupyter/display.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/lean4_jupyter/install.py` & `lean4_jupyter-0.0.1rc8/lean4_jupyter/install.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/lean4_jupyter/kernel.py` & `lean4_jupyter-0.0.1rc8/lean4_jupyter/kernel.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/lean4_jupyter/repl.py` & `lean4_jupyter-0.0.1rc8/lean4_jupyter/repl.py`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/lean4_jupyter/resources/lean_logo.svg` & `lean4_jupyter-0.0.1rc8/lean4_jupyter/resources/lean_logo.svg`

 * *Files identical despite different names*

### Comparing `lean4_jupyter-0.0.1rc7/pyproject.toml` & `lean4_jupyter-0.0.1rc8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -23,7 +23,16 @@
     "Operating System :: POSIX :: Linux",
     "Development Status :: 3 - Alpha"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Source = "https://github.com/utensil/lean4_jupyter"
+
+# https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#a-full-example
+[project.optional-dependencies]
+test = [
+    "flake8",
+    "pytest",
+    "nbval",
+    "papermill"
+]
```

### Comparing `lean4_jupyter-0.0.1rc7/setup.py` & `lean4_jupyter-0.0.1rc8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,21 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['pexpect>=4.0', 'ipykernel', 'alectryon']
 
+extras_require = \
+{'test': ['flake8', 'pytest', 'nbval', 'papermill']}
+
 setup(name='lean4_jupyter',
-      version='0.0.1rc7',
+      version='0.0.1rc8',
       description='lean4_jupyter: A Lean 4 Jupyter kernel via REPL',
       author=None,
       author_email='Utensil Song <utensilcandel@gmail.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
+      extras_require=extras_require,
      )
```

### Comparing `lean4_jupyter-0.0.1rc7/PKG-INFO` & `lean4_jupyter-0.0.1rc8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: lean4_jupyter
-Version: 0.0.1rc7
+Version: 0.0.1rc8
 Summary: lean4_jupyter: A Lean 4 Jupyter kernel via REPL
 Author-email: Utensil Song <utensilcandel@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: Framework :: Jupyter
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: pexpect (>=4.0)
 Requires-Dist: ipykernel
 Requires-Dist: alectryon
+Requires-Dist: flake8 ; extra == "test"
+Requires-Dist: pytest ; extra == "test"
+Requires-Dist: nbval ; extra == "test"
+Requires-Dist: papermill ; extra == "test"
 Project-URL: Source, https://github.com/utensil/lean4_jupyter
+Provides-Extra: test
 
 # lean4_jupyter
 
 A Lean 4 Jupyter kernel via [repl](https://github.com/leanprover-community/repl).
 
 [![PyPI](https://img.shields.io/pypi/v/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/lean4_jupyter.svg)](https://pypi.org/project/lean4_jupyter/)
 ![PyPI - License](https://img.shields.io/pypi/l/lean4_jupyter)
 ![PyPI - Status](https://img.shields.io/pypi/status/lean4_jupyter)
 [![Python CI](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml/badge.svg)](https://github.com/utensil/lean4_jupyter/actions/workflows/ci.yml)
-[![Maintainability](https://api.codeclimate.com/v1/badges/666a7d45d436a598df2b/maintainability)](https://codeclimate.com/github/utensil/lean4_jupyter/maintainability) 
-
-## Status
-
-Alpha.
+[![lint - flake8](https://img.shields.io/badge/lint-flake8-blue)](https://github.com/PyCQA/flake8)
+[![Static Badge](https://img.shields.io/badge/test-nbval-purple)](https://github.com/computationalmodelling/nbval)
+[![Maintainability](https://api.codeclimate.com/v1/badges/666a7d45d436a598df2b/maintainability)](https://codeclimate.com/github/utensil/lean4_jupyter/maintainability)
 
 ## What's already working
 
 🔥 See it in action: [Tutorial notebook](https://nbviewer.org/github/utensil/lean4_jupyter/blob/main/examples/00_tutorial.ipynb?flush_cache=true).
 
 The kernel can:
 
@@ -49,15 +52,15 @@
 
 ## What's next
 
 - Fix [repl#40](https://github.com/leanprover-community/repl/issues/40) (PRed as [repl#41](https://github.com/leanprover-community/repl/issues/41))
 - Improve the alectryon annotation to support annotations in the middle of a line
 - Make magics like `%cd` and `%load` work more robustly
 - Support show `tactics` after `%load`
-- Add a CI based on [papermill](https://github.com/nteract/papermill/)
+- Add all `repl` test cases to the CI and set up coverage
 - Improve UI in Jupyter Dark themes
 - Minor code refactor to smooth things out
 
 ## Installation
 
 First, you need a working Lean 4 installation. You can install it via [elan](https://github.com/leanprover/elan).
```

