# Comparing `tmp/tach-0.2.0.tar.gz` & `tmp/tach-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tach-0.2.0.tar", last modified: Mon May 20 02:23:13 2024, max compression
+gzip compressed data, was "tach-0.2.1.tar", last modified: Wed May 22 18:24:19 2024, max compression
```

## Comparing `tach-0.2.0.tar` & `tach-0.2.1.tar`

### file list

```diff
@@ -1,137 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.676150 tach-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.680150 tach-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 02:23:04.000000 tach-0.2.0/.github/workflows/publish_docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-20 02:23:04.000000 tach-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 02:23:04.000000 tach-0.2.0/.pre-commit-hooks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 02:23:04.000000 tach-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 02:23:13.696150 tach-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-20 02:23:04.000000 tach-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 02:23:04.000000 tach-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-20 02:23:04.000000 tach-0.2.0/docs/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 02:23:04.000000 tach-0.2.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-20 02:23:04.000000 tach-0.2.0/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-20 02:23:04.000000 tach-0.2.0/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 02:23:04.000000 tach-0.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 02:23:04.000000 tach-0.2.0/docs/strict-mode.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-20 02:23:04.000000 tach-0.2.0/docs/tach-ignore.md
--rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-20 02:23:04.000000 tach-0.2.0/docs/tach_demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-20 02:23:04.000000 tach-0.2.0/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-20 02:23:04.000000 tach-0.2.0/docs/why-tach.md
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-20 02:23:04.000000 tach-0.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-20 02:23:04.000000 tach-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 02:23:13.696150 tach-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tach/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-20 02:23:04.000000 tach-0.2.0/tach/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     6352 2024-05-20 02:23:04.000000 tach-0.2.0/tach/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-20 02:23:04.000000 tach-0.2.0/tach/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)    11518 2024-05-20 02:23:04.000000 tach-0.2.0/tach/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/colors/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-20 02:23:04.000000 tach-0.2.0/tach/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/colors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.684150 tach-0.2.0/tach/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 02:23:04.000000 tach-0.2.0/tach/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/constants/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/core/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 02:23:04.000000 tach-0.2.0/tach/core/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-20 02:23:04.000000 tach-0.2.0/tach/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 02:23:04.000000 tach-0.2.0/tach/errors/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/filesystem/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/package.py
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-20 02:23:04.000000 tach-0.2.0/tach/filesystem/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      405 2024-05-20 02:23:04.000000 tach-0.2.0/tach/hooks/pre-commit
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.688150 tach-0.2.0/tach/interactive/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-20 02:23:04.000000 tach-0.2.0/tach/interactive/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-20 02:23:04.000000 tach-0.2.0/tach/loading.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-20 02:23:04.000000 tach-0.2.0/tach/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tach/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/ast_visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 02:23:04.000000 tach-0.2.0/tach/parsing/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-20 02:23:04.000000 tach-0.2.0/tach/pkg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-20 02:23:04.000000 tach-0.2.0/tach/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 02:23:13.000000 tach-0.2.0/tach.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-20 02:23:04.000000 tach-0.2.0/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_one/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_one/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.692150 tach-0.2.0/tests/example/domain_two/subdomain/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/domain_two/subdomain/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/empty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/empty/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/.hidden/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/invalid/hidden/unhidden/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/invalid/tach.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_one/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_one/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_three/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_three/package.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 02:23:13.696150 tach-0.2.0/tests/example/valid/domain_two/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/domain_two/package.yml
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-20 02:23:04.000000 tach-0.2.0/tests/example/valid/tach.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_package_trie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 02:23:04.000000 tach-0.2.0/tests/test_show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.831595 tach-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.835595 tach-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 18:24:14.000000 tach-0.2.1/.github/workflows/publish_docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-22 18:24:14.000000 tach-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-22 18:24:14.000000 tach-0.2.1/.pre-commit-hooks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 18:24:14.000000 tach-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-22 18:24:19.851595 tach-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5837 2024-05-22 18:24:14.000000 tach-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 18:24:14.000000 tach-0.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.835595 tach-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-22 18:24:14.000000 tach-0.2.1/docs/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-22 18:24:14.000000 tach-0.2.1/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-22 18:24:14.000000 tach-0.2.1/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 18:24:14.000000 tach-0.2.1/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-22 18:24:14.000000 tach-0.2.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-22 18:24:14.000000 tach-0.2.1/docs/strict-mode.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-22 18:24:14.000000 tach-0.2.1/docs/tach-ignore.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92208 2024-05-22 18:24:14.000000 tach-0.2.1/docs/tach_demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-22 18:24:14.000000 tach-0.2.1/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-22 18:24:14.000000 tach-0.2.1/docs/why-tach.md
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 18:24:14.000000 tach-0.2.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-22 18:24:14.000000 tach-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:24:19.851595 tach-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tach/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-22 18:24:14.000000 tach-0.2.1/tach/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-22 18:24:14.000000 tach-0.2.1/tach/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 18:24:14.000000 tach-0.2.1/tach/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12102 2024-05-22 18:24:14.000000 tach-0.2.1/tach/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-22 18:24:14.000000 tach-0.2.1/tach/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/colors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 18:24:14.000000 tach-0.2.1/tach/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/constants/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.839595 tach-0.2.1/tach/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 18:24:14.000000 tach-0.2.1/tach/core/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-22 18:24:14.000000 tach-0.2.1/tach/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 18:24:14.000000 tach-0.2.1/tach/errors/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/filesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-05-22 18:24:14.000000 tach-0.2.1/tach/filesystem/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-05-22 18:24:14.000000 tach-0.2.1/tach/hooks/pre_commit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19334 2024-05-22 18:24:14.000000 tach-0.2.1/tach/interactive/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-22 18:24:14.000000 tach-0.2.1/tach/loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 18:24:14.000000 tach-0.2.1/tach/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.843595 tach-0.2.1/tach/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/ast_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-22 18:24:14.000000 tach-0.2.1/tach/parsing/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-22 18:24:14.000000 tach-0.2.1/tach/pkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-22 18:24:14.000000 tach-0.2.1/tach/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 18:24:19.000000 tach-0.2.1/tach.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 18:24:14.000000 tach-0.2.1/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_one/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_one/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/domain_two/subdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/domain_two/subdomain/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/empty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/empty/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/.hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.847596 tach-0.2.1/tests/example/invalid/hidden/unhidden/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/invalid/tach.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_one/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_one/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_three/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_three/package.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:24:19.851595 tach-0.2.1/tests/example/valid/domain_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 18:24:14.000000 tach-0.2.1/tests/example/valid/tach.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_package_trie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:24:14.000000 tach-0.2.1/tests/test_show.py
```

### Comparing `tach-0.2.0/.github/workflows/ci.yml` & `tach-0.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/.github/workflows/publish.yml` & `tach-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/.github/workflows/publish_docs.yml` & `tach-0.2.1/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/.gitignore` & `tach-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/LICENSE` & `tach-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/PKG-INFO` & `tach-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.2.0/README.md` & `tach-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/configuration.md` & `tach-0.2.1/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/faq.md` & `tach-0.2.1/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/favicon.ico` & `tach-0.2.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/getting-started.md` & `tach-0.2.1/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/index.md` & `tach-0.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/strict-mode.md` & `tach-0.2.1/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/tach-ignore.md` & `tach-0.2.1/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/tach_demo.mp4` & `tach-0.2.1/docs/tach_demo.mp4`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/docs/usage.md` & `tach-0.2.1/docs/usage.md`

 * *Files 3% similar despite different names*

```diff
@@ -103,21 +103,24 @@
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
 -   repo: https://github.com/Never-Over/tach
-    rev: v0.2.0  # change this to the latest tag!
+    rev: v0.2.1  # change this to the latest tag!
     hooks:
     -   id: tach
+        # args: ["--root=backend_root"]
 ```
 
 Note that you should specify the version you are using in the `rev` key.
 
+Using `args`, you can specify the root of your Python project, where `tach check` should run.
+This path should be relative to your git root.
 
 ### Standard install
 If you don't already have pre-commit hooks set up, you can run:
 
 ```bash
 tach install pre-commit
 ```
```

### Comparing `tach-0.2.0/docs/why-tach.md` & `tach-0.2.1/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/mkdocs.yml` & `tach-0.2.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/pyproject.toml` & `tach-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `tach-0.2.0/tach/add.py` & `tach-0.2.1/tach/add.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/check.py` & `tach-0.2.1/tach/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,56 +120,61 @@
     project_config: ProjectConfig,
     exclude_paths: Optional[list[str]] = None,
     exclude_hidden_paths: Optional[bool] = True,
 ) -> list[BoundaryError]:
     if not os.path.isdir(root):
         raise errors.TachSetupError(f"The path {root} is not a valid directory.")
 
-    # This 'canonicalizes' the path arguments, resolving directory traversal
-    root = fs.canonical(root)
+    cwd = fs.get_cwd()
+    try:
+        fs.chdir(root)
+        # This 'canonicalizes' the path arguments, resolving directory traversal
+        root = fs.canonical(root)
+
+        if exclude_paths is not None and project_config.exclude is not None:
+            exclude_paths.extend(project_config.exclude)
+        else:
+            exclude_paths = project_config.exclude
 
-    if exclude_paths is not None and project_config.exclude is not None:
-        exclude_paths.extend(project_config.exclude)
-    else:
-        exclude_paths = project_config.exclude
-
-    package_trie = build_package_trie(
-        root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
-    )
-
-    boundary_errors: list[BoundaryError] = []
-    for file_path in fs.walk_pyfiles(
-        root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
-    ):
-        mod_path = fs.file_to_module_path(file_path)
-        nearest_package = package_trie.find_nearest(mod_path)
-        if nearest_package is None:
-            continue
-
-        # This should only give us imports from within our project
-        # (excluding stdlib, builtins, and 3rd party packages)
-        project_imports = get_project_imports(
-            root,
-            file_path,
-            ignore_type_checking_imports=project_config.ignore_type_checking_imports,
+        package_trie = build_package_trie(
+            root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
         )
-        for project_import in project_imports:
-            check_error = check_import(
-                project_config=project_config,
-                package_trie=package_trie,
-                import_mod_path=project_import.mod_path,
-                file_nearest_package=nearest_package,
-                file_mod_path=mod_path,
-            )
-            if check_error is None:
+
+        boundary_errors: list[BoundaryError] = []
+        for file_path in fs.walk_pyfiles(
+            root, exclude_paths=exclude_paths, exclude_hidden_paths=exclude_hidden_paths
+        ):
+            mod_path = fs.file_to_module_path(file_path)
+            nearest_package = package_trie.find_nearest(mod_path)
+            if nearest_package is None:
                 continue
 
-            boundary_errors.append(
-                BoundaryError(
-                    file_path=file_path,
+            # This should only give us imports from within our project
+            # (excluding stdlib, builtins, and 3rd party packages)
+            project_imports = get_project_imports(
+                root,
+                file_path,
+                ignore_type_checking_imports=project_config.ignore_type_checking_imports,
+            )
+            for project_import in project_imports:
+                check_error = check_import(
+                    project_config=project_config,
+                    package_trie=package_trie,
                     import_mod_path=project_import.mod_path,
-                    line_number=project_import.line_number,
-                    error_info=check_error,
+                    file_nearest_package=nearest_package,
+                    file_mod_path=mod_path,
+                )
+                if check_error is None:
+                    continue
+
+                boundary_errors.append(
+                    BoundaryError(
+                        file_path=file_path,
+                        import_mod_path=project_import.mod_path,
+                        line_number=project_import.line_number,
+                        error_info=check_error,
+                    )
                 )
-            )
 
-    return boundary_errors
+        return boundary_errors
+    finally:
+        fs.chdir(cwd)
```

### Comparing `tach-0.2.0/tach/cli.py` & `tach-0.2.1/tach/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -134,14 +134,21 @@
     check_parser = subparsers.add_parser(
         "check",
         prog="tach check",
         help="Check existing boundaries against your dependencies and package interfaces",
         description="Check existing boundaries against your dependencies and package interfaces",
     )
     check_parser.add_argument(
+        "--root",
+        required=False,
+        type=str,
+        default=".",
+        help="The root directory from which the check should run",
+    )
+    check_parser.add_argument(
         "--strict",
         action="store_true",
         help="Raise errors if any dependency constraints are unused.",
     )
     add_base_arguments(check_parser)
     install_parser = subparsers.add_parser(
         "install",
@@ -156,15 +163,22 @@
     )
     install_parser.add_argument(
         "-p",
         "--path",
         required=False,
         type=str,
         default=".",
-        help="The path where this installation should occur (default '.')",
+        help="The path where this installation should occur (e.g. git root for hooks)",
+    )
+    install_parser.add_argument(
+        "--project-root",
+        required=False,
+        type=str,
+        default="",
+        help="The relative path where 'tach check' should run (defaults to git root)",
     )
     sync_parser = subparsers.add_parser(
         "sync",
         prog="tach sync",
         help="Sync constraints with actual dependencies in your project.",
         description="Sync constraints with actual dependencies in your project.",
     )
@@ -196,27 +210,28 @@
         # TODO: unify project config handling
         fs.validate_project_config_path()
 
     return parsed_args, parser
 
 
 def tach_check(
+    root: str = ".",
     strict: bool = False,
     exclude_paths: Optional[list[str]] = None,
 ):
     try:
         project_config = parse_project_config()
 
         if exclude_paths is not None and project_config.exclude is not None:
             exclude_paths.extend(project_config.exclude)
         else:
             exclude_paths = project_config.exclude
 
         boundary_errors: list[BoundaryError] = check(
-            ".",
+            root,
             project_config,
             exclude_paths=exclude_paths,
             exclude_hidden_paths=project_config.exclude_hidden_paths,
         )
 
         # If we are checking in strict mode, we want to also verify that pruning constraints has no effect
         if not boundary_errors and strict:
@@ -298,18 +313,20 @@
     PRE_COMMIT = "pre-commit"
 
     @classmethod
     def choices(cls) -> list[str]:
         return [item.value for item in cls]
 
 
-def tach_install(path: str, target: InstallTarget) -> None:
+def tach_install(path: str, target: InstallTarget, project_root: str = "") -> None:
     try:
         if target == InstallTarget.PRE_COMMIT:
-            installed, warning = install_pre_commit(path=path)
+            installed, warning = install_pre_commit(
+                path=path, project_root=project_root
+            )
         else:
             raise NotImplementedError(f"Target {target} is not supported by 'install'.")
     except Exception as e:
         print(str(e))
         sys.exit(1)
 
     if installed:
@@ -329,24 +346,26 @@
     exclude_paths = args.exclude.split(",") if getattr(args, "exclude", None) else None
     if args.command == "pkg":
         tach_pkg(depth=args.depth, exclude_paths=exclude_paths)
     elif args.command == "sync":
         tach_sync(prune=args.prune, exclude_paths=exclude_paths)
     elif args.command == "check":
         start_spinner("Scanning...")
-        tach_check(strict=args.strict, exclude_paths=exclude_paths)
+        tach_check(root=args.root, strict=args.strict, exclude_paths=exclude_paths)
     elif args.command == "clean":
         tach_clean(force=args.force)
     elif args.command == "install":
         try:
             install_target = InstallTarget(args.target)
         except ValueError:
             print(f"{args.target} is not a valid installation target.")
             sys.exit(1)
-        tach_install(path=args.path, target=install_target)
+        tach_install(
+            path=args.path, target=install_target, project_root=args.project_root
+        )
     else:
         print("Unrecognized command")
         parser.print_help()
         exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `tach-0.2.0/tach/core/config.py` & `tach-0.2.1/tach/core/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/core/package.py` & `tach-0.2.1/tach/core/package.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/filesystem/__init__.py` & `tach-0.2.1/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/filesystem/project.py` & `tach-0.2.1/tach/filesystem/project.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/filesystem/service.py` & `tach-0.2.1/tach/filesystem/service.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/interactive/packages.py` & `tach-0.2.1/tach/interactive/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/loading.py` & `tach-0.2.1/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/parsing/config.py` & `tach-0.2.1/tach/parsing/config.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/parsing/imports.py` & `tach-0.2.1/tach/parsing/imports.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/parsing/interface.py` & `tach-0.2.1/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/parsing/packages.py` & `tach-0.2.1/tach/parsing/packages.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/pkg.py` & `tach-0.2.1/tach/pkg.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach/sync.py` & `tach-0.2.1/tach/sync.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tach.egg-info/PKG-INFO` & `tach-0.2.1/tach.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tach
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python tool to maintain a modular package architecture.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/tach
 Project-URL: Issues, https://github.com/never-over/tach/issues
 Keywords: python,module,package,guard,enforcement,boundary,enforcer,domain,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tach-0.2.0/tach.egg-info/SOURCES.txt` & `tach-0.2.1/tach.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 tach/errors/package.yml
 tach/filesystem/__init__.py
 tach/filesystem/install.py
 tach/filesystem/package.py
 tach/filesystem/package.yml
 tach/filesystem/project.py
 tach/filesystem/service.py
-tach/hooks/pre-commit
+tach/hooks/__init__.py
+tach/hooks/package.yml
+tach/hooks/pre_commit.py
 tach/interactive/__init__.py
 tach/interactive/package.yml
 tach/interactive/packages.py
 tach/parsing/__init__.py
 tach/parsing/ast_visitor.py
 tach/parsing/config.py
 tach/parsing/imports.py
```

### Comparing `tach-0.2.0/tests/test_add.py` & `tach-0.2.1/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tests/test_check.py` & `tach-0.2.1/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tests/test_cli.py` & `tach-0.2.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tests/test_init.py` & `tach-0.2.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tests/test_package_trie.py` & `tach-0.2.1/tests/test_package_trie.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.0/tests/test_parsing.py` & `tach-0.2.1/tests/test_parsing.py`

 * *Files identical despite different names*

