# Comparing `tmp/vertagus-0.1.0b5.tar.gz` & `tmp/vertagus-0.1.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertagus-0.1.0b5.tar", last modified: Tue May 21 21:45:25 2024, max compression
+gzip compressed data, was "vertagus-0.1.0b6.tar", last modified: Wed May 22 17:42:07 2024, max compression
```

## Comparing `vertagus-0.1.0b5.tar` & `vertagus-0.1.0b6.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.381658 vertagus-0.1.0b5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.385658 vertagus-0.1.0b5/src/vertagus/
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.385658 vertagus-0.1.0b5/src/vertagus/aliases/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/aliases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/aliases/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/aliases/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.385658 vertagus-0.1.0b5/src/vertagus/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      349 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.385658 vertagus-0.1.0b5/src/vertagus/cli/commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/commands/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/commands/create_aliases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/commands/create_tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/configuration/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/configuration/load.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/configuration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/core/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/manifest_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/package_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/rule_bases.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/scm_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/stage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/core/tag_base.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1322 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/providers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/providers/manifest/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/manifest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      552 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/manifest/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/providers/manifest/setuptools_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/manifest/setuptools_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/providers/scm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/providers/scm/git_/
--rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/scm/git_/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4343 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/scm/git_/git_scm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/providers/scm/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/rules/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.389658 vertagus-0.1.0b5/src/vertagus/rules/comparison/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/comparison/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/comparison/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/comparison/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/src/vertagus/rules/single_version/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/single_version/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/single_version/library.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/rules/single_version/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/src/vertagus/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/utils/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/utils/factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/src/vertagus/utils/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/src/vertagus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 21:45:25.000000 vertagus-0.1.0b5/src/vertagus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:45:25.393658 vertagus-0.1.0b5/test/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/test/test_factory.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-21 21:45:21.000000 vertagus-0.1.0b5/test/test_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1054 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3791 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1100 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.802748 vertagus-0.1.0b6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/aliases/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1151 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      747 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/aliases/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       21 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      358 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/cli/commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      108 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/create_aliases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1188 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/create_tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.806748 vertagus-0.1.0b6/src/vertagus/configuration/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/load.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4485 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/configuration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      512 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/manifest_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/package_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5961 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      665 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/rule_bases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      648 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/scm_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1586 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/stage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/core/tag_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2981 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1322 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/manifest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/json_manifest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       59 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      830 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/manifest/yaml_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/scm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       27 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4345 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/git_/git_scm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/providers/scm/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/comparison/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      908 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      732 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/comparison/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.810748 vertagus-0.1.0b6/src/vertagus/rules/single_version/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1564 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/library.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      729 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/rules/single_version/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/src/vertagus/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      588 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      197 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      533 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/src/vertagus/utils/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/src/vertagus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 17:42:07.000000 vertagus-0.1.0b6/src/vertagus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:42:07.814748 vertagus-0.1.0b6/test/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/test/test_factory.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1733 2024-05-22 17:42:01.000000 vertagus-0.1.0b6/test/test_operations.py
```

### Comparing `vertagus-0.1.0b5/LICENSE` & `vertagus-0.1.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/PKG-INFO` & `vertagus-0.1.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b5/README.md` & `vertagus-0.1.0b6/README.md`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/pyproject.toml` & `vertagus-0.1.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vertagus"
-version = "0.1.0b5"
+version = "0.1.0b6"
 description = "A tool to assist the maintenance of package versioning with scm tags"
 readme = "README.md"
 authors = [
     {"name" = "John Raines", "email" = "johndanielraines@gmail.com"}
 ]
 dependencies = [
     "click",
```

### Comparing `vertagus-0.1.0b5/src/vertagus/aliases/library.py` & `vertagus-0.1.0b6/src/vertagus/aliases/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/aliases/loader.py` & `vertagus-0.1.0b6/src/vertagus/aliases/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/cli/commands/create_aliases.py` & `vertagus-0.1.0b6/src/vertagus/cli/commands/create_aliases.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/cli/commands/create_tag.py` & `vertagus-0.1.0b6/src/vertagus/cli/commands/create_tag.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/cli/commands/validate.py` & `vertagus-0.1.0b6/src/vertagus/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/configuration/load.py` & `vertagus-0.1.0b6/src/vertagus/configuration/load.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/configuration/types.py` & `vertagus-0.1.0b6/src/vertagus/configuration/types.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/manifest_base.py` & `vertagus-0.1.0b6/src/vertagus/core/manifest_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/package_base.py` & `vertagus-0.1.0b6/src/vertagus/core/package_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/project.py` & `vertagus-0.1.0b6/src/vertagus/core/project.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/rule_bases.py` & `vertagus-0.1.0b6/src/vertagus/core/rule_bases.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/scm_base.py` & `vertagus-0.1.0b6/src/vertagus/core/scm_base.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/core/stage.py` & `vertagus-0.1.0b6/src/vertagus/core/stage.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/factory.py` & `vertagus-0.1.0b6/src/vertagus/factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/operations.py` & `vertagus-0.1.0b6/src/vertagus/operations.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/providers/manifest/registry.py` & `vertagus-0.1.0b6/src/vertagus/providers/manifest/registry.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import typing as T
 from .setuptools_ import SetuptoolsPyprojectManifest
+from .json_manifest import JsonManifest
+from .yaml_manifest import YamlManifest
 
 _manifest_types = {
     SetuptoolsPyprojectManifest.manifest_type: SetuptoolsPyprojectManifest,
+    JsonManifest.manifest_type: JsonManifest,
+    YamlManifest.manifest_type: YamlManifest,
 }
 
 
 def get_manifest_cls(manifest_type: str) -> T.Type[SetuptoolsPyprojectManifest]:
     if manifest_type not in _manifest_types:
         raise ValueError(f"Unknown manifest type: {manifest_type}")
     return _manifest_types[manifest_type]
```

### Comparing `vertagus-0.1.0b5/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py` & `vertagus-0.1.0b6/src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/providers/scm/git_/git_scm.py` & `vertagus-0.1.0b6/src/vertagus/providers/scm/git_/git_scm.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
             ref=commit,
             message=tag_text,
         )
         self._repo.git.push(tags=True)
     
     def delete_tag(self, tag: Tag):
         _tags = [t.name for t in self._repo.tags]
-        logger.info(
+        logger.debug(
             f"Tags found: {_tags}"
         )
         tag_text = tag.as_string(self.tag_prefix)
         try:
             self._repo.delete_tag(tag_text)
         except GitCommandError as e:
             logger.warning(
@@ -115,15 +115,15 @@
                 logger.warning(f"Invalid version found: {version}")
         if not valid_versions:
             return None
         return max(valid_versions, key=lambda v: parse_version(v))
     
     def _initialize_repo(self):
         repo = git.Repo(self.root)
-        logger.info(
+        logger.debug(
             f"Initializing git repository at {self.root} "
             f"with user data {self.user_data}."
         )
         repo.config_writer().set_value(
             "user", "name", self.user_data['name']
         ).release()
         repo.config_writer().set_value(
```

### Comparing `vertagus-0.1.0b5/src/vertagus/rules/comparison/library.py` & `vertagus-0.1.0b6/src/vertagus/rules/comparison/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/rules/comparison/loader.py` & `vertagus-0.1.0b6/src/vertagus/rules/comparison/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/rules/single_version/library.py` & `vertagus-0.1.0b6/src/vertagus/rules/single_version/library.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/rules/single_version/loader.py` & `vertagus-0.1.0b6/src/vertagus/rules/single_version/loader.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/utils/config.py` & `vertagus-0.1.0b6/src/vertagus/utils/config.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus/utils/regex.py` & `vertagus-0.1.0b6/src/vertagus/utils/regex.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/src/vertagus.egg-info/PKG-INFO` & `vertagus-0.1.0b6/src/vertagus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertagus
-Version: 0.1.0b5
+Version: 0.1.0b6
 Summary: A tool to assist the maintenance of package versioning with scm tags
 Author-email: John Raines <johndanielraines@gmail.com>
 License: Copyright (c) 2024 John Raines
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `vertagus-0.1.0b5/src/vertagus.egg-info/SOURCES.txt` & `vertagus-0.1.0b6/src/vertagus.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 src/vertagus/core/project.py
 src/vertagus/core/rule_bases.py
 src/vertagus/core/scm_base.py
 src/vertagus/core/stage.py
 src/vertagus/core/tag_base.py
 src/vertagus/providers/__init__.py
 src/vertagus/providers/manifest/__init__.py
+src/vertagus/providers/manifest/json_manifest.py
 src/vertagus/providers/manifest/registry.py
+src/vertagus/providers/manifest/yaml_manifest.py
 src/vertagus/providers/manifest/setuptools_/__init__.py
 src/vertagus/providers/manifest/setuptools_/pyproject_manifest.py
 src/vertagus/providers/scm/__init__.py
 src/vertagus/providers/scm/registry.py
 src/vertagus/providers/scm/git_/__init__.py
 src/vertagus/providers/scm/git_/git_scm.py
 src/vertagus/rules/__init__.py
```

### Comparing `vertagus-0.1.0b5/test/test_factory.py` & `vertagus-0.1.0b6/test/test_factory.py`

 * *Files identical despite different names*

### Comparing `vertagus-0.1.0b5/test/test_operations.py` & `vertagus-0.1.0b6/test/test_operations.py`

 * *Files identical despite different names*

