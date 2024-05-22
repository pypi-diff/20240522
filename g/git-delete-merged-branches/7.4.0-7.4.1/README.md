# Comparing `tmp/git-delete-merged-branches-7.4.0.tar.gz` & `tmp/git_delete_merged_branches-7.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-delete-merged-branches-7.4.0.tar", last modified: Fri Dec 23 20:40:09 2022, max compression
+gzip compressed data, was "git_delete_merged_branches-7.4.1.tar", last modified: Wed May 22 16:43:42 2024, max compression
```

## Comparing `git-delete-merged-branches-7.4.0.tar` & `git_delete_merged_branches-7.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.244080 git-delete-merged-branches-7.4.0/
--rw-r--r--   0 sping     (1000) sping     (1000)       31 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.flake8
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.239080 git-delete-merged-branches-7.4.0/.github/
--rw-r--r--   0 sping     (1000) sping     (1000)      317 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.github/dependabot.yml
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.239080 git-delete-merged-branches-7.4.0/.github/workflows/
--rw-r--r--   0 sping     (1000) sping     (1000)     1164 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.github/workflows/enforce-copies-of-help-output-in-sync.yml
--rw-r--r--   0 sping     (1000) sping     (1000)     2042 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.github/workflows/pre-commit-detect-outdated.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      383 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 sping     (1000) sping     (1000)      655 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.github/workflows/run-tests.yml
--rw-r--r--   0 sping     (1000) sping     (1000)       66 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)       27 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.isort.cfg
--rw-r--r--   0 sping     (1000) sping     (1000)      696 2022-12-23 20:36:29.000000 git-delete-merged-branches-7.4.0/.pre-commit-config.yaml
--rw-r--r--   0 sping     (1000) sping     (1000)      179 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/.style.yapf
--rw-r--r--   0 sping     (1000) sping     (1000)    35149 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/LICENSE
--rw-r--r--   0 sping     (1000) sping     (1000)     6346 2022-12-23 20:40:09.244080 git-delete-merged-branches-7.4.0/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     5265 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/README.md
--rw-r--r--   0 sping     (1000) sping     (1000)     2411 2022-12-23 20:39:36.000000 git-delete-merged-branches-7.4.0/git-delete-merged-branches.1
--rw-r--r--   0 sping     (1000) sping     (1000)     2333 2022-12-23 20:39:36.000000 git-delete-merged-branches-7.4.0/git-dmb.1
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.241080 git-delete-merged-branches-7.4.0/git_delete_merged_branches/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      159 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1384 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_argparse_color.py
--rw-r--r--   0 sping     (1000) sping     (1000)     7392 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_cli.py
--rw-r--r--   0 sping     (1000) sping     (1000)      748 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_confirm.py
--rw-r--r--   0 sping     (1000) sping     (1000)    24300 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_engine.py
--rw-r--r--   0 sping     (1000) sping     (1000)    11921 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_git.py
--rw-r--r--   0 sping     (1000) sping     (1000)     2077 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_messenger.py
--rw-r--r--   0 sping     (1000) sping     (1000)      219 2022-12-23 20:39:36.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_metadata.py
--rw-r--r--   0 sping     (1000) sping     (1000)    15078 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_multiselect.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1610 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/_shell.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.243080 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/__init__.py
--rw-r--r--   0 sping     (1000) sping     (1000)     1504 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/helpers.py
--rw-r--r--   0 sping     (1000) sping     (1000)      513 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_cli.py
--rw-r--r--   0 sping     (1000) sping     (1000)    11420 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_engine.py
--rw-r--r--   0 sping     (1000) sping     (1000)     5583 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_git.py
--rw-r--r--   0 sping     (1000) sping     (1000)      541 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_shell.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2022-12-23 20:40:09.242080 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)     6346 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     1369 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)      139 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       62 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/requires.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       27 2022-12-23 20:40:09.000000 git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/top_level.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2022-12-23 20:40:09.244080 git-delete-merged-branches-7.4.0/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     1981 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/setup.py
--rwxr-xr-x   0 sping     (1000) sping     (1000)     1495 2022-12-23 00:15:34.000000 git-delete-merged-branches-7.4.0/sync-manpage-with-help-output.sh
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.322939 git_delete_merged_branches-7.4.1/
+-rw-r--r--   0 sping     (1000) sping     (1000)       31 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/.flake8
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.316939 git_delete_merged_branches-7.4.1/.github/
+-rw-r--r--   0 sping     (1000) sping     (1000)      317 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/.github/dependabot.yml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.316939 git_delete_merged_branches-7.4.1/.github/workflows/
+-rw-r--r--   0 sping     (1000) sping     (1000)     1253 2024-05-22 16:42:58.000000 git_delete_merged_branches-7.4.1/.github/workflows/enforce-copies-of-help-output-in-sync.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     2178 2024-05-22 16:06:10.000000 git_delete_merged_branches-7.4.1/.github/workflows/pre-commit-detect-outdated.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)      515 2024-05-22 16:06:10.000000 git_delete_merged_branches-7.4.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)      801 2024-05-22 16:06:10.000000 git_delete_merged_branches-7.4.1/.github/workflows/run-tests.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)       66 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)       27 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/.isort.cfg
+-rw-r--r--   0 sping     (1000) sping     (1000)      697 2024-04-19 17:56:24.000000 git_delete_merged_branches-7.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 sping     (1000) sping     (1000)      179 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/.style.yapf
+-rw-r--r--   0 sping     (1000) sping     (1000)    35149 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/LICENSE
+-rw-r--r--   0 sping     (1000) sping     (1000)     7058 2024-05-22 16:43:42.321939 git_delete_merged_branches-7.4.1/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     5860 2023-06-26 19:22:27.000000 git_delete_merged_branches-7.4.1/README.md
+-rw-r--r--   0 sping     (1000) sping     (1000)     2406 2024-05-22 16:42:58.000000 git_delete_merged_branches-7.4.1/git-delete-merged-branches.1
+-rw-r--r--   0 sping     (1000) sping     (1000)     2328 2024-05-22 16:42:58.000000 git_delete_merged_branches-7.4.1/git-dmb.1
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.318939 git_delete_merged_branches-7.4.1/git_delete_merged_branches/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      159 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1384 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_argparse_color.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     7392 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_cli.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      748 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_confirm.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    24300 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_engine.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    11921 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_git.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     2077 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_messenger.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      219 2024-05-22 16:42:58.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_metadata.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    15018 2024-05-22 16:06:10.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_multiselect.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1610 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/_shell.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.321939 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/__init__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     1504 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/helpers.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      513 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_cli.py
+-rw-r--r--   0 sping     (1000) sping     (1000)    11462 2023-04-21 17:51:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_engine.py
+-rw-r--r--   0 sping     (1000) sping     (1000)     5583 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_git.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      541 2022-12-23 00:15:34.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_shell.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2024-05-22 16:43:42.321939 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)     7058 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     1370 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)      139 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       62 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/requires.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       27 2024-05-22 16:43:42.000000 git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/top_level.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2024-05-22 16:43:42.322939 git_delete_merged_branches-7.4.1/setup.cfg
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     1982 2024-04-19 17:56:24.000000 git_delete_merged_branches-7.4.1/setup.py
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     1495 2024-05-22 16:42:58.000000 git_delete_merged_branches-7.4.1/sync-manpages-with-help-output.sh
```

### Comparing `git-delete-merged-branches-7.4.0/.github/workflows/enforce-copies-of-help-output-in-sync.yml` & `git_delete_merged_branches-7.4.1/.github/workflows/enforce-copies-of-help-output-in-sync.yml`

 * *Files 17% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 - push
 
 jobs:
   run_pre_commit:
     name: Check if copies of --help output are in sync
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v3.2.0
+      - uses: actions/checkout@a5ac7e51b41094c92402da3b24376905380afc29  # v4.1.6
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@v4.3.1
+      - name: Set up Python 3.12
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d  # v5.1.0
         with:
-          python-version: 3.11
+          python-version: 3.12
 
       - name: Install build dependencies
         run: |
           sudo apt-get install --no-install-recommends -y help2man
 
       - name: Install delete-merged-branches entry point script
         run: |-
@@ -31,9 +31,9 @@
             --no-warn-script-location \
             .
           echo "PATH=${HOME}/.local/bin:${PATH}" >> "${GITHUB_ENV}"
 
       - name: Check if the man page is in sync with --help output
         run: |-
           rm git-{delete-merged-branches,dmb}.1  # to enforce a diff for the generator to remove
-          ./sync-manpage-with-help-output.sh
+          ./sync-manpages-with-help-output.sh
           git diff --exit-code -- git-{delete-merged-branches,dmb}.1
```

### Comparing `git-delete-merged-branches-7.4.0/.pre-commit-config.yaml` & `git_delete_merged_branches-7.4.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Copyright (C) 2020 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GPL v3 or later
 
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
-        args: ['--py37-plus']
+        args: ['--py38-plus']
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
       - id: check-merge-conflict
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.0.0
+    rev: 7.0.0
     hooks:
       - id: flake8
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.11.4
+    rev: 5.13.2
     hooks:
       - id: isort
 
   - repo: https://github.com/google/yapf
-    rev: v0.32.0
+    rev: v0.40.2
     hooks:
       - id: yapf
```

### Comparing `git-delete-merged-branches-7.4.0/LICENSE` & `git_delete_merged_branches-7.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/PKG-INFO` & `git_delete_merged_branches-7.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: git-delete-merged-branches
-Version: 7.4.0
+Version: 7.4.1
 Summary: Command-line tool to delete merged Git branches
 Home-page: https://github.com/hartwork/git-delete-merged-branches
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: colorama>=0.4.3
+Requires-Dist: prompt-toolkit>=3.0.18
+Provides-Extra: tests
+Requires-Dist: parameterized; extra == "tests"
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run the test suite](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml)
 [![Packaging status](https://repology.org/badge/tiny-repos/git-delete-merged-branches.svg)](https://repology.org/project/git-delete-merged-branches/versions)
 
 
 # git-delete-merged-branches
 
 A convenient command-line tool helping you keep repositories clean.
@@ -38,20 +42,24 @@
 ```console
 # pip install git-delete-merged-branches
 ```
 
 If you are using one of the distributions below, you can install
 `git-delete-merged-branches` through the respective package manager, e.g.:
 
- - [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) —
-   `# yay -S git-delete-merged-branches`
- - [Debian GNU/Linux (sid)](https://packages.debian.org/sid/git-delete-merged-branches) — `# apt install git-delete-merged-branches`
- - [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) — `# emerge -av dev-vcs/git-delete-merged-branches`
- - [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) — `# brew install git-delete-merged-branches`
- - [NixOS](https://github.com/NixOS/nixpkgs/blob/master/pkgs/applications/version-management/git-and-tools/git-delete-merged-branches/default.nix)
+| Distribution | Command |
+| ------------ | ------- |
+| [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) | `yay -S git-delete-merged-branches` |
+| [Debian GNU/Linux (>=bookworm)](https://packages.debian.org/bookworm/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) | `emerge -av dev-vcs/git-delete-merged-branches` |
+| [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) | `brew install git-delete-merged-branches` |
+| [MacPorts](https://ports.macports.org/port/py-git-delete-merged-branches/details/) | `port install py-git-delete-merged-branches` |
+| [NixOS](https://search.nixos.org/packages?query=git-delete-merged-branches) | `nix-shell -p git-delete-merged-branches` |
+| [Ubuntu (>=lunar/23.04)](https://packages.ubuntu.com/source/lunar/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Void Linux](https://github.com/void-linux/void-packages/tree/master/srcpkgs/git-delete-merged-branches) | `xbps-install -S git-delete-merged-branches` |
 
 
 # Example
 
 ```console
 # git-delete-merged-branches
 Do you want to run "git remote update --prune" for 1 remote(s):
```

### Comparing `git-delete-merged-branches-7.4.0/README.md` & `git_delete_merged_branches-7.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run the test suite](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml)
 [![Packaging status](https://repology.org/badge/tiny-repos/git-delete-merged-branches.svg)](https://repology.org/project/git-delete-merged-branches/versions)
 
 
 # git-delete-merged-branches
 
 A convenient command-line tool helping you keep repositories clean.
@@ -12,20 +13,24 @@
 ```console
 # pip install git-delete-merged-branches
 ```
 
 If you are using one of the distributions below, you can install
 `git-delete-merged-branches` through the respective package manager, e.g.:
 
- - [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) —
-   `# yay -S git-delete-merged-branches`
- - [Debian GNU/Linux (sid)](https://packages.debian.org/sid/git-delete-merged-branches) — `# apt install git-delete-merged-branches`
- - [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) — `# emerge -av dev-vcs/git-delete-merged-branches`
- - [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) — `# brew install git-delete-merged-branches`
- - [NixOS](https://github.com/NixOS/nixpkgs/blob/master/pkgs/applications/version-management/git-and-tools/git-delete-merged-branches/default.nix)
+| Distribution | Command |
+| ------------ | ------- |
+| [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) | `yay -S git-delete-merged-branches` |
+| [Debian GNU/Linux (>=bookworm)](https://packages.debian.org/bookworm/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) | `emerge -av dev-vcs/git-delete-merged-branches` |
+| [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) | `brew install git-delete-merged-branches` |
+| [MacPorts](https://ports.macports.org/port/py-git-delete-merged-branches/details/) | `port install py-git-delete-merged-branches` |
+| [NixOS](https://search.nixos.org/packages?query=git-delete-merged-branches) | `nix-shell -p git-delete-merged-branches` |
+| [Ubuntu (>=lunar/23.04)](https://packages.ubuntu.com/source/lunar/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Void Linux](https://github.com/void-linux/void-packages/tree/master/srcpkgs/git-delete-merged-branches) | `xbps-install -S git-delete-merged-branches` |
 
 
 # Example
 
 ```console
 # git-delete-merged-branches
 Do you want to run "git remote update --prune" for 1 remote(s):
```

### Comparing `git-delete-merged-branches-7.4.0/git-delete-merged-branches.1` & `git_delete_merged_branches-7.4.1/git-delete-merged-branches.1`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man.
-.TH GIT-DELETE-MERGED-BRANCHES "1" "December 2022" "git-delete-merged-branches 7.4.0" "User Commands"
+.TH GIT-DELETE-MERGED-BRANCHES "1" "May 2024" "git-delete-merged-branches 7.4.1" "User Commands"
 .SH NAME
 git-delete-merged-branches \- Command-line tool to delete merged Git branches
 .SH SYNOPSIS
 
 .B git\-delete\-merged\-branches
 [\fB\-\-configure\fR | \fB\-\-help\fR | \fB\-\-version\fR\] [\fB\-\-branch\fR BRANCH] [\fB\-\-effort\fR LEVEL] [\fB\-\-remote\fR REMOTE] [\fB\-\-exclude\fR BRANCH] [\fB\-\-include\-regex\fR PATTERN] [\fB\-\-debug\fR] [\fB\-\-dry\-run\fR] [\fB\-\-verbose\fR] [\fB\-\-yes\fR]
 .SH DESCRIPTION
```

### Comparing `git-delete-merged-branches-7.4.0/git-dmb.1` & `git_delete_merged_branches-7.4.1/git-dmb.1`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 .\" DO NOT MODIFY THIS FILE!  It was generated by help2man.
-.TH GIT-DMB "1" "December 2022" "git-dmb 7.4.0" "User Commands"
+.TH GIT-DMB "1" "May 2024" "git-dmb 7.4.1" "User Commands"
 .SH NAME
 git-dmb \- Command-line tool to delete merged Git branches
 .SH SYNOPSIS
 
 .B git\-dmb
 [\fB\-\-configure\fR | \fB\-\-help\fR | \fB\-\-version\fR\] [\fB\-\-branch\fR BRANCH] [\fB\-\-effort\fR LEVEL] [\fB\-\-remote\fR REMOTE] [\fB\-\-exclude\fR BRANCH] [\fB\-\-include\-regex\fR PATTERN] [\fB\-\-debug\fR] [\fB\-\-dry\-run\fR] [\fB\-\-verbose\fR] [\fB\-\-yes\fR]
 .SH DESCRIPTION
```

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_argparse_color.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_argparse_color.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_cli.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_cli.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_confirm.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_confirm.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_engine.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_engine.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_git.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_git.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_messenger.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_messenger.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_multiselect.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_multiselect.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,17 +302,15 @@
         return key_bindings
 
     def _create_text_display_window_for(self, lines: List[_LineBase]) -> Window:
         document = Document(text='\n'.join(line.text for line in lines))
         buffer = Buffer(read_only=True, document=document)
         buffer_control = BufferControl(
             buffer=buffer, input_processors=[_NonItemRenderProcessor(prompt=self, lines=lines)])
-        return Window(buffer_control,
-                      wrap_lines=True,
-                      height=Dimension(min=len(lines), max=len(lines)))
+        return Window(buffer_control, wrap_lines=True, height=Dimension(min=len(lines)))
 
     def _create_layout(self) -> Tuple[Layout, _HeightTrackingScrollablePane]:
         header = self._create_text_display_window_for(self._header_lines)
         footer = self._create_text_display_window_for(self._footer_lines)
 
         search = SearchToolbar(ignore_case=True)
         buffer_control = BufferControl(buffer=self._buffer,
```

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/_shell.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/_shell.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/helpers.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_cli.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_engine.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,17 +252,17 @@
              excluded_branches_extra, included_branches_patterns, expected_exclusion_set):
         git_mock = Mock(find_all_branch_names=Mock(return_value=existing_branches))
         dmb = DeleteMergedBranches(git=git_mock,
                                    messenger=Mock(),
                                    confirmation=Mock(),
                                    selector=Mock(),
                                    effort_level=999)
+        git_config_key_format = DeleteMergedBranches._FORMAT_BRANCH_EXCLUDED
         git_config = {
-            DeleteMergedBranches._FORMAT_BRANCH_EXCLUDED.format(name=branch_name):
-            DeleteMergedBranches._CONFIG_VALUE_TRUE
+            git_config_key_format.format(name=branch_name): DeleteMergedBranches._CONFIG_VALUE_TRUE
             for branch_name in excluded_branches_from_config
         }
 
         actual_exclusion_set = dmb.determine_excluded_branches(git_config, excluded_branches_extra,
                                                                included_branches_patterns)
 
         self.assertEqual(actual_exclusion_set, expected_exclusion_set)
```

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_git.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches/tests/test_shell.py` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/PKG-INFO` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 Metadata-Version: 2.1
 Name: git-delete-merged-branches
-Version: 7.4.0
+Version: 7.4.1
 Summary: Command-line tool to delete merged Git branches
 Home-page: https://github.com/hartwork/git-delete-merged-branches
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPLv3+
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Software Development :: Version Control :: Git
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: colorama>=0.4.3
+Requires-Dist: prompt-toolkit>=3.0.18
+Provides-Extra: tests
+Requires-Dist: parameterized; extra == "tests"
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Run the test suite](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml/badge.svg)](https://github.com/hartwork/git-delete-merged-branches/actions/workflows/run-tests.yml)
 [![Packaging status](https://repology.org/badge/tiny-repos/git-delete-merged-branches.svg)](https://repology.org/project/git-delete-merged-branches/versions)
 
 
 # git-delete-merged-branches
 
 A convenient command-line tool helping you keep repositories clean.
@@ -38,20 +42,24 @@
 ```console
 # pip install git-delete-merged-branches
 ```
 
 If you are using one of the distributions below, you can install
 `git-delete-merged-branches` through the respective package manager, e.g.:
 
- - [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) —
-   `# yay -S git-delete-merged-branches`
- - [Debian GNU/Linux (sid)](https://packages.debian.org/sid/git-delete-merged-branches) — `# apt install git-delete-merged-branches`
- - [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) — `# emerge -av dev-vcs/git-delete-merged-branches`
- - [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) — `# brew install git-delete-merged-branches`
- - [NixOS](https://github.com/NixOS/nixpkgs/blob/master/pkgs/applications/version-management/git-and-tools/git-delete-merged-branches/default.nix)
+| Distribution | Command |
+| ------------ | ------- |
+| [Arch Linux (AUR)](https://aur.archlinux.org/packages/git-delete-merged-branches/) | `yay -S git-delete-merged-branches` |
+| [Debian GNU/Linux (>=bookworm)](https://packages.debian.org/bookworm/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Gentoo Linux](https://packages.gentoo.org/packages/dev-vcs/git-delete-merged-branches) | `emerge -av dev-vcs/git-delete-merged-branches` |
+| [Homebrew](https://formulae.brew.sh/formula/git-delete-merged-branches) | `brew install git-delete-merged-branches` |
+| [MacPorts](https://ports.macports.org/port/py-git-delete-merged-branches/details/) | `port install py-git-delete-merged-branches` |
+| [NixOS](https://search.nixos.org/packages?query=git-delete-merged-branches) | `nix-shell -p git-delete-merged-branches` |
+| [Ubuntu (>=lunar/23.04)](https://packages.ubuntu.com/source/lunar/git-delete-merged-branches) | `apt install git-delete-merged-branches` |
+| [Void Linux](https://github.com/void-linux/void-packages/tree/master/srcpkgs/git-delete-merged-branches) | `xbps-install -S git-delete-merged-branches` |
 
 
 # Example
 
 ```console
 # git-delete-merged-branches
 Do you want to run "git remote update --prune" for 1 remote(s):
```

### Comparing `git-delete-merged-branches-7.4.0/git_delete_merged_branches.egg-info/SOURCES.txt` & `git_delete_merged_branches-7.4.1/git_delete_merged_branches.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 .pre-commit-config.yaml
 .style.yapf
 LICENSE
 README.md
 git-delete-merged-branches.1
 git-dmb.1
 setup.py
-sync-manpage-with-help-output.sh
+sync-manpages-with-help-output.sh
 .github/dependabot.yml
 .github/workflows/enforce-copies-of-help-output-in-sync.yml
 .github/workflows/pre-commit-detect-outdated.yml
 .github/workflows/pre-commit.yml
 .github/workflows/run-tests.yml
 git_delete_merged_branches/__init__.py
 git_delete_merged_branches/__main__.py
```

### Comparing `git-delete-merged-branches-7.4.0/setup.py` & `git_delete_merged_branches-7.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     license='GPLv3+',
     description=DESCRIPTION,
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Sebastian Pipping',
     author_email='sebastian@pipping.org',
     url=f'https://github.com/hartwork/{APP}',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     setup_requires=[
         'setuptools>=38.6.0',  # for long_description_content_type
     ],
     install_requires=[
         'colorama>=0.4.3',
         'prompt-toolkit>=3.0.18',
     ],
@@ -44,19 +44,19 @@
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Version Control',
         'Topic :: Software Development :: Version Control :: Git',
     ],
     data_files=[('share/man/man1', [
         f'{APP}.1',
         'git-dmb.1',
     ])],
```

### Comparing `git-delete-merged-branches-7.4.0/sync-manpage-with-help-output.sh` & `git_delete_merged_branches-7.4.1/sync-manpages-with-help-output.sh`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env bash
 # Copyright (C) 2022 Sebastian Pipping <sebastian@pipping.org>
 # Licensed under GPL v3 or later
 
 set -e
 set -o pipefail
 
-_BUILD_MONTH=2022-12  # for reproducible builds; bump when doing releases
+_BUILD_MONTH=2024-05  # for reproducible builds; bump when doing releases
 
 sed_args=(
     # Produce familiar section "synopsis"
     -e 's,^\.SH DESCRIPTION,.SH SYNOPSIS,'
     -e 's,^usage: ,,'
     -e 's,.*\[\\-\\-yes\]$,\0\n.SH DESCRIPTION,'
```

