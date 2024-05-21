# Comparing `tmp/hklpy2-0.0.8.tar.gz` & `tmp/hklpy2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hklpy2-0.0.8.tar", last modified: Fri May 10 06:07:16 2024, max compression
+gzip compressed data, was "hklpy2-0.0.9.tar", last modified: Thu May 16 20:14:41 2024, max compression
```

## Comparing `hklpy2-0.0.8.tar` & `hklpy2-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.778638 hklpy2-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.770638 hklpy2-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-10 06:07:04.000000 hklpy2-0.0.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.770638 hklpy2-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-10 06:07:04.000000 hklpy2-0.0.8/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-10 06:07:04.000000 hklpy2-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-10 06:07:04.000000 hklpy2-0.0.8/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-10 06:07:04.000000 hklpy2-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-10 06:07:04.000000 hklpy2-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-10 06:07:04.000000 hklpy2-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-10 06:07:16.778638 hklpy2-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-10 06:07:04.000000 hklpy2-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.770638 hklpy2-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.774638 hklpy2-0.0.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.774638 hklpy2-0.0.8/docs/source/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.774638 hklpy2-0.0.8/docs/source/api/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/backends/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/backends/hkl_soleil.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/backends/no_op.rst
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/backends/th_tth_q.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/backends.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/lattice.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/reflection.rst
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/sample.rst
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api/z_misc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/license.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.774638 hklpy2-0.0.8/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/notebooks/demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-10 06:07:04.000000 hklpy2-0.0.8/docs/source/substitutions.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-10 06:07:04.000000 hklpy2-0.0.8/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.774638 hklpy2-0.0.8/hklpy2/
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.778638 hklpy2-0.0.8/hklpy2/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/hkl_soleil.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/no_op.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.778638 hklpy2-0.0.8/hklpy2/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/tests/test_hkl_soleil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/tests/test_th_tth_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/backends/th_tth_q.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/notes.md
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.778638 hklpy2-0.0.8/hklpy2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_demo_notebook.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-10 06:07:04.000000 hklpy2-0.0.8/hklpy2/tests/test_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 06:07:16.778638 hklpy2-0.0.8/hklpy2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 06:07:16.000000 hklpy2-0.0.8/hklpy2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-10 06:07:04.000000 hklpy2-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 06:07:16.778638 hklpy2-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.494690 hklpy2-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.486690 hklpy2-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 20:14:33.000000 hklpy2-0.0.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.486690 hklpy2-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-16 20:14:33.000000 hklpy2-0.0.9/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-16 20:14:33.000000 hklpy2-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-16 20:14:33.000000 hklpy2-0.0.9/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 20:14:33.000000 hklpy2-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-16 20:14:33.000000 hklpy2-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 20:14:33.000000 hklpy2-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 20:14:41.494690 hklpy2-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-16 20:14:33.000000 hklpy2-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.486690 hklpy2-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.486690 hklpy2-0.0.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.490690 hklpy2-0.0.9/docs/source/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.490690 hklpy2-0.0.9/docs/source/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/backends/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/backends/hkl_soleil.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/backends/no_op.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/backends/th_tth_q.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/lattice.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/reflection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/sample.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api/z_misc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2495 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/license.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.490690 hklpy2-0.0.9/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/notebooks/demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 20:14:33.000000 hklpy2-0.0.9/docs/source/substitutions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 20:14:33.000000 hklpy2-0.0.9/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.490690 hklpy2-0.0.9/hklpy2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.494690 hklpy2-0.0.9/hklpy2/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/no_op.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.494690 hklpy2-0.0.9/hklpy2/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/tests/test_hkl_soleil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/tests/test_th_tth_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/backends/th_tth_q.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/notes.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.494690 hklpy2-0.0.9/hklpy2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_demo_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4658 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-16 20:14:33.000000 hklpy2-0.0.9/hklpy2/tests/test_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:14:41.494690 hklpy2-0.0.9/hklpy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 20:14:41.000000 hklpy2-0.0.9/hklpy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-16 20:14:33.000000 hklpy2-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:14:41.494690 hklpy2-0.0.9/setup.cfg
```

### Comparing `hklpy2-0.0.8/.github/workflows/code.yml` & `hklpy2-0.0.9/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/.github/workflows/docs.yml` & `hklpy2-0.0.9/.github/workflows/docs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -32,38 +32,62 @@
     steps:
 
       - name: Deploy Information
         if: ${{ github.event.inputs.deploy }}
         run: |
           echo "The docs will be published from this workflow run."
 
-      - name: Set time zone
-        run: echo "TZ=America/Chicago" >> "$GITHUB_ENV"
+      - name: Set timezone
+        uses: szenius/set-timezone@v2.0
+        with:
+          timezoneLinux: "America/Chicago"
+
+      - name: Make Temporary Directory for Sphinx content
+        run: |
+          echo "SRC_DIR=$(pwd)" >> ${GITHUB_ENV}
+          echo "TMP_DIR=$(mktemp -d)" >> ${GITHUB_ENV}
 
       - name: install pandoc in the OS
         run: sudo apt-get install pandoc
 
-      - name: Sphinx build
-        id: deployment
-        uses: sphinx-notes/pages@v3
+      - name: Checkout
+        uses: actions/checkout@v4
         with:
-          documentation_path: ./docs/source
-          publish: false
-          python_version: 3.12
-          requirements_path: ./docs/requirements.txt
-
-      - name: Diagnostic
-        run: ls -lAFgh ${{ steps.deployment.outputs.artifact }}
-    
+          fetch-depth: 0 # otherwise, you will fail to push refs to dest repo
+
+      - uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+
+      - name: Install Sphinx build requirements
+        run: pip install -r ./docs/requirements.txt
+
+      - name: Install our package
+        run: pip install --no-deps -e . -vv
+
+      - name: Show Environment variables
+        run: |
+          echo "SRC_DIR=${SRC_DIR}"
+          echo "TMP_DIR=${TMP_DIR}"
+
+      - name: Sphinx
+        run: sphinx-build -M html ./docs/source "${TMP_DIR}/build"
+
+      - name: Define ... HTML_DIR
+        run: echo "HTML_DIR=${TMP_DIR}/build/html" >> ${GITHUB_ENV}
+
+      - name: Diagnostics
+        run: ls -lAFghR "${HTML_DIR}"
+
       - name: Upload Docs ZIP file as artifact
         uses: actions/upload-artifact@v4
         with:
           name: hklpy2-docs
-          path: ${{ steps.deployment.outputs.artifact }}
+          path: ${{ env.HTML_DIR }}
 
       - name: Deploy (to gh-pages branch) only on demand
         uses: peaceiris/actions-gh-pages@v4
         if: ${{ github.event.inputs.deploy }}
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_branch: gh-pages
-          publish_dir: ${{ steps.deployment.outputs.artifact }}
+          publish_dir: ${{ env.HTML_DIR }}
```

### Comparing `hklpy2-0.0.8/.github/workflows/pypi.yml` & `hklpy2-0.0.9/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/.gitignore` & `hklpy2-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/LICENSE` & `hklpy2-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/PKG-INFO` & `hklpy2-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.8
+Version: 0.0.9
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
```

### Comparing `hklpy2-0.0.8/README.md` & `hklpy2-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/Makefile` & `hklpy2-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/make.bat` & `hklpy2-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/api/backends.rst` & `hklpy2-0.0.9/docs/source/api/backends.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/api/lattice.rst` & `hklpy2-0.0.9/docs/source/api/lattice.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/api/reflection.rst` & `hklpy2-0.0.9/docs/source/api/reflection.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/conf.py` & `hklpy2-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/index.rst` & `hklpy2-0.0.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/docs/source/notebooks/demo.ipynb` & `hklpy2-0.0.9/docs/source/notebooks/demo.ipynb`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/__init__.py` & `hklpy2-0.0.9/hklpy2/__init__.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/__init__.py` & `hklpy2-0.0.9/hklpy2/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/base.py` & `hklpy2-0.0.9/hklpy2/backends/base.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/hkl_soleil.py` & `hklpy2-0.0.9/hklpy2/backends/hkl_soleil.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/no_op.py` & `hklpy2-0.0.9/hklpy2/backends/no_op.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/tests/test_hkl_soleil.py` & `hklpy2-0.0.9/hklpy2/backends/tests/test_hkl_soleil.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/tests/test_th_tth_q.py` & `hklpy2-0.0.9/hklpy2/backends/tests/test_th_tth_q.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/backends/th_tth_q.py` & `hklpy2-0.0.9/hklpy2/backends/th_tth_q.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/lattice.py` & `hklpy2-0.0.9/hklpy2/lattice.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/misc.py` & `hklpy2-0.0.9/hklpy2/misc.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/reflection.py` & `hklpy2-0.0.9/hklpy2/reflection.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/sample.py` & `hklpy2-0.0.9/hklpy2/sample.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_backends.py` & `hklpy2-0.0.9/hklpy2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_demo_notebook.py` & `hklpy2-0.0.9/hklpy2/tests/test_demo_notebook.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_lattice.py` & `hklpy2-0.0.9/hklpy2/tests/test_lattice.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_reflection.py` & `hklpy2-0.0.9/hklpy2/tests/test_reflection.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_sample.py` & `hklpy2-0.0.9/hklpy2/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2/tests/test_solver.py` & `hklpy2-0.0.9/hklpy2/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/hklpy2.egg-info/PKG-INFO` & `hklpy2-0.0.9/hklpy2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hklpy2
-Version: 0.0.8
+Version: 0.0.9
 Summary: 2nd generation diffractometer controls for the Bluesky Framework.
 Author-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 Maintainer-email: Pete Jemian <prjemian+hklpy2@gmail.com>
 License: Copyright (c) 2023-2024, UChicago Argonne, LLC
         
         All Rights Reserved
```

### Comparing `hklpy2-0.0.8/hklpy2.egg-info/SOURCES.txt` & `hklpy2-0.0.9/hklpy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hklpy2-0.0.8/pyproject.toml` & `hklpy2-0.0.9/pyproject.toml`

 * *Files identical despite different names*

