# Comparing `tmp/grepsr_cli-0.7.9.tar.gz` & `tmp/grepsr_cli-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grepsr_cli-0.7.9.tar", last modified: Wed May 15 11:03:08 2024, max compression
+gzip compressed data, was "grepsr_cli-0.8.0.tar", last modified: Wed May 22 03:04:12 2024, max compression
```

## Comparing `grepsr_cli-0.7.9.tar` & `grepsr_cli-0.8.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-15 11:03:00.000000 grepsr_cli-0.7.9/.version
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/CHANGELOG.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/LICENSE.md
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/MANIFEST.in
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2943 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/README.md
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/grepsr_cli.egg-info/
--rw-r--r--   0 zznix     (1000) zznix     (1000)     3475 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/PKG-INFO
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/entry_points.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/requires.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-15 11:03:08.000000 grepsr_cli-0.7.9/grepsr_cli.egg-info/top_level.txt
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/controllers/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.7.9/grepsrcli/controllers/base.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    18775 2024-05-15 10:59:50.000000 grepsr_cli-0.7.9/grepsrcli/controllers/crawler.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/generate.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/controllers/report.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/core/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.7.9/grepsrcli/core/aws_s3.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.7.9/grepsrcli/core/config.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/exc.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/input_prompts.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.7.9/grepsrcli/core/message_log.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/core/report_api.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.7.9/grepsrcli/core/sdk_setup.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/core/test_local.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)    16013 2024-05-15 10:59:50.000000 grepsr_cli-0.7.9/grepsrcli/core/utils.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/ext/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/ext/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.7.9/grepsrcli/main.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/plugins/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/plugins/__init__.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/grepsrcli/templates/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/__init__.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/autocomplete.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/autocomplete_zsh.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/composer.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/node_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2084 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     3458 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_brp_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     2087 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/grepsrcli/templates/php_vc_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/grepsrcli/templates/py_boilerplate.jinja2
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/requirements-dev.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/requirements.txt
--rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-15 11:03:08.395675 grepsr_cli-0.7.9/setup.cfg
--rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.7.9/setup.py
-drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-15 11:03:08.391675 grepsr_cli-0.7.9/tests/
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.7.9/tests/test_grepsrcli.py
--rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.7.9/tests/test_unit.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        6 2024-05-22 03:01:49.000000 grepsr_cli-0.8.0/.version
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1240 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/CHANGELOG.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/LICENSE.md
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      193 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/MANIFEST.in
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3061 2024-05-21 03:15:08.000000 grepsr_cli-0.8.0/README.md
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/grepsr_cli.egg-info/
+-rw-r--r--   0 zznix     (1000) zznix     (1000)     3593 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1264 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        1 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       45 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      133 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/requires.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       10 2024-05-22 03:04:11.000000 grepsr_cli-0.8.0/grepsr_cli.egg-info/top_level.txt
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.004200 grepsr_cli-0.8.0/grepsrcli/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/controllers/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1549 2023-06-06 11:43:01.000000 grepsr_cli-0.8.0/grepsrcli/controllers/base.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    19297 2024-05-21 05:07:27.000000 grepsr_cli-0.8.0/grepsrcli/controllers/crawler.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1018 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/generate.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2106 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/controllers/report.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/core/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1185 2023-03-02 07:11:29.000000 grepsr_cli-0.8.0/grepsrcli/core/aws_s3.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     7454 2023-06-05 10:31:03.000000 grepsr_cli-0.8.0/grepsrcli/core/config.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       69 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/exc.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/input_prompts.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      825 2023-01-07 17:23:26.000000 grepsr_cli-0.8.0/grepsrcli/core/message_log.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      885 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/core/report_api.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3221 2023-09-06 03:15:01.000000 grepsr_cli-0.8.0/grepsrcli/core/sdk_setup.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     5713 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/core/test_local.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)    16893 2024-05-21 04:05:06.000000 grepsr_cli-0.8.0/grepsrcli/core/utils.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/ext/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/ext/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2169 2024-04-25 17:32:12.000000 grepsr_cli-0.8.0/grepsrcli/main.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.008200 grepsr_cli-0.8.0/grepsrcli/plugins/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/plugins/__init__.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/grepsrcli/templates/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)        0 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/__init__.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      296 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/autocomplete.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      577 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/autocomplete_zsh.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      488 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/composer.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3049 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/node_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2084 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     3458 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_brp_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     2087 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/grepsrcli/templates/php_vc_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1753 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/grepsrcli/templates/py_boilerplate.jinja2
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      107 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/requirements-dev.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      132 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/requirements.txt
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)       38 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/setup.cfg
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)     1115 2022-09-21 03:08:28.000000 grepsr_cli-0.8.0/setup.py
+drwxrwxr-x   0 zznix     (1000) zznix     (1000)        0 2024-05-22 03:04:12.012200 grepsr_cli-0.8.0/tests/
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      615 2024-05-07 09:17:11.000000 grepsr_cli-0.8.0/tests/test_grepsrcli.py
+-rw-rw-r--   0 zznix     (1000) zznix     (1000)      932 2024-04-25 17:32:12.000000 grepsr_cli-0.8.0/tests/test_unit.py
```

### Comparing `grepsr_cli-0.7.9/CHANGELOG.md` & `grepsr_cli-0.8.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/PKG-INFO` & `grepsr_cli-0.8.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.9
+Version: 0.8.0
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -95,7 +95,8 @@
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
 - auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
 
 
 # TODO:
 - Experiment with git rebase on deploy fail. `git rebase origin/master --autostash && git push`
+- Handle Prioritization of same plugin name across multiple repo more deterministically. (maybe prioritize cwd path?)
```

### Comparing `grepsr_cli-0.7.9/README.md` & `grepsr_cli-0.8.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -75,8 +75,9 @@
 ## Features Added
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
 - auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
 
 
 # TODO:
-- Experiment with git rebase on deploy fail. `git rebase origin/master --autostash && git push`
+- Experiment with git rebase on deploy fail. `git rebase origin/master --autostash && git push`
+- Handle Prioritization of same plugin name across multiple repo more deterministically. (maybe prioritize cwd path?)
```

### Comparing `grepsr_cli-0.7.9/grepsr_cli.egg-info/PKG-INFO` & `grepsr_cli-0.8.0/grepsr_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grepsr-cli
-Version: 0.7.9
+Version: 0.8.0
 Summary: A Cli tool for Grepsr Developers
 Home-page: https://bitbucket.org/grepsr/grepsr-cli/
 Author: grepsr
 Author-email: dev@grepsr.com
 License: unlicensed
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -95,7 +95,8 @@
 - drop stash after pushed successully. Before this, all stashes were always kept.
 - run a custom shell file before running your crawler. This allows possiblity like always injecting a php function in all your crawlers.
 - auto add `Dependencies: ...` that your crawler class extends (dependecies that are not extended by crawler classes but used elsewhere is upcoming)
 
 
 # TODO:
 - Experiment with git rebase on deploy fail. `git rebase origin/master --autostash && git push`
+- Handle Prioritization of same plugin name across multiple repo more deterministically. (maybe prioritize cwd path?)
```

### Comparing `grepsr_cli-0.7.9/grepsr_cli.egg-info/SOURCES.txt` & `grepsr_cli-0.8.0/grepsr_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/controllers/base.py` & `grepsr_cli-0.8.0/grepsrcli/controllers/base.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/controllers/crawler.py` & `grepsr_cli-0.8.0/grepsrcli/controllers/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     ask_user_input_YN,
     ask_user_input,
     return_parsed_url,
     insert_all_chained_dependencies,
     generate_plugin_name,
     string_to_list,
     first_found_numbers,
+    get_current_branch_name,
+    cmd_shell_exec,
 )
 from ..core.test_local import TestLocal
 from ..core.message_log import Log
 from ..core.aws_s3 import S3
 
 class CrawlerBase(Controller):
     class Meta:
@@ -110,16 +112,16 @@
     def sync(self):
         if(self.app.pargs.type):
             type = self.app.pargs.type
             crawler_paths = self.config[type]['paths']
 
             for crawler_path in crawler_paths:
                 Log.info(f"Syncing: {crawler_path}")
-                system(
-                    f"""cd {crawler_path}  && git pull origin master""")
+                curr_branch_name = get_current_branch_name(crawler_path)
+                system(f"""cd {crawler_path} && git pull origin {curr_branch_name}""")
         else:
             Log.warn("Please enter a valid type")
 
     @ex(
         help="create basic boilerplate for plugins ",
         arguments=[
             (
@@ -319,22 +321,30 @@
                 sys.stdout.write(
                     "Deploying: [%s]" % (" " * toolbar_width))
                 sys.stdout.write("\b" * (toolbar_width + 1))
                 sys.stdout.flush()
             try:
                 quiet_mode = "" if verbose_mode else "--quiet"
                 root_repo_dir = path.dirname(plugin_dir_path)
+                curr_branch_name = get_current_branch_name(root_repo_dir)
+                
                 # dont pop stash. cuz if there is a merge conflict, good luck with that.
                 # instead apply stash and if and only if everything has passed, then drop the stash.
-                # TODO: only apply stash if `git stash` stashed >0 files.
+
+                stashed = True
+                stash_cmd_proc = cmd_shell_exec('git stash', root_repo_dir)      # no quiet mode cuz we want the full output
+                if stash_cmd_proc.stdout.strip().lower() == 'no local changes to save':
+                    stashed = False
+                
                 git_sync_cmds = [
-                    f'git stash {quiet_mode}',
-                    f'git pull origin master {quiet_mode}',
-                    f'git stash apply {quiet_mode}',
+                    f'git pull origin {curr_branch_name} {quiet_mode}',
                 ]
+                if stashed:
+                    git_sync_cmds.append(f'git stash apply {quiet_mode}')
+                    
                 if verbose_mode:
                     cmd = verbosify(git_sync_cmds)
                 else:
                     cmd = return_cmd_with_progress(git_sync_cmds, toolbar_width)
                 try:
                     proc = subprocess.run(cmd, shell=True, check=True, timeout=100, cwd=root_repo_dir)
                 except subprocess.TimeoutExpired:
@@ -354,30 +364,31 @@
                         self.app.log.warning("PID was not forced. This may cause issues.")
 
                 commit_msg = f'[{deploy_type}] [{version_info}] {deploy_message}'
                 # self.app.log.info(commit_msg)
                 main_git_cmds = [
                     f'git add {plugin_name}/',
                     f'git commit -m "{commit_msg}" {quiet_mode}',
-                    f'git push origin master {quiet_mode}',
+                    f'git push origin {curr_branch_name} {quiet_mode}',
                 ]
                 post_deploy_cmds = [
                     f'git stash drop {quiet_mode}'
                 ]
                 
                 if verbose_mode:
                     cmd = verbosify(main_git_cmds)
                 else:
                     cmd = return_cmd_with_progress(main_git_cmds, toolbar_width)
                 try:
                     proc = subprocess.run(cmd, shell=True, check=True, timeout=300, cwd=root_repo_dir)
                     if proc.returncode == 0:
-                        proc = subprocess.run(' && '.join(post_deploy_cmds), shell=True, cwd=root_repo_dir)
-                        if proc.returncode != 0:
-                            self.app.log.warning('Failed to drop the latest stash.')
+                        if stashed:
+                            proc = subprocess.run(' && '.join(post_deploy_cmds), shell=True, cwd=root_repo_dir)
+                            if proc.returncode != 0:
+                                self.app.log.warning('Failed to drop the latest stash.')
 
                 except subprocess.TimeoutExpired:
                     self.app.log.error(f'Timeout occured when deploying {plugin_name}')
 
             except subprocess.CalledProcessError as e:
                 if verbose_mode:
                     self.app.log.error(e)
```

### Comparing `grepsr_cli-0.7.9/grepsrcli/controllers/generate.py` & `grepsr_cli-0.8.0/grepsrcli/controllers/generate.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/controllers/report.py` & `grepsr_cli-0.8.0/grepsrcli/controllers/report.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/aws_s3.py` & `grepsr_cli-0.8.0/grepsrcli/core/aws_s3.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/config.py` & `grepsr_cli-0.8.0/grepsrcli/core/config.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/message_log.py` & `grepsr_cli-0.8.0/grepsrcli/core/message_log.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/report_api.py` & `grepsr_cli-0.8.0/grepsrcli/core/report_api.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/sdk_setup.py` & `grepsr_cli-0.8.0/grepsrcli/core/sdk_setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/test_local.py` & `grepsr_cli-0.8.0/grepsrcli/core/test_local.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/core/utils.py` & `grepsr_cli-0.8.0/grepsrcli/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,20 +429,47 @@
         multiplier = 0
     # just echo some dashes after each command for progress. lol.
     echoer = 'echo -n ' + '-' * multiplier
     # .join() only does n-1 additions. Hence add a echoer at last. And then echo remaining to fill the bar (caused by floor division)
     cmd = f' && {echoer} &&'.join(cmds) + f' && {echoer}' + f' && echo -n {"-" * (toolbar_width - (len(cmds) * multiplier))}'
     return cmd
 
+def is_path_tracked_by_git(relative_path, root_repo_dir):
+    proc = cmd_shell_exec(f'git ls-files --error-unmatch {relative_path}', root_repo_dir)
+    if proc.returncode == 0:
+        return True
+    return False
+
 def does_plugin_have_modifications(plugin_name, root_repo_dir):
     """check if plugin has any modification in the code
     """
-    # TODO: handle untracked file. untracked file have newline added incorrectly.
-    proc = subprocess.run(f'git diff -s --exit-code {plugin_name}/{plugin_name}.php', shell=True, timeout=100, cwd=root_repo_dir)
+    if not is_path_tracked_by_git(f'{plugin_name}/', root_repo_dir):
+        # is untracked file. meaning plugin was just created. it does have modifications.
+        return True
+    proc = cmd_shell_exec(f'git diff -s --exit-code {plugin_name}/{plugin_name}.php', root_repo_dir)
     if proc.returncode == 0:
         return False
     elif proc.returncode == 1:
         return True
     return None
 
 def verbosify(cmds: List[str]) -> str:
-    return ' && '.join([f'echo {cmd} && {cmd}' for cmd in cmds])
+    return ' && '.join([f'echo {cmd} && {cmd}' for cmd in cmds])
+
+def cmd_shell_exec(cmd, working_dir, timeout=100):
+    return subprocess.run(cmd, shell=True, timeout=timeout, cwd=working_dir, capture_output=True, text=True)
+
+def get_current_branch_name(root_repo_dir: str) -> str:
+    git_cmds = [
+        'git branch --show-current',
+        'git rev-parse --abbrev-ref HEAD',
+        'git symbolic-ref --short HEAD',
+    ]
+    
+    branch_name = ''
+    for git_cmd in git_cmds:
+        proc = cmd_shell_exec(git_cmd, root_repo_dir)
+        if proc.returncode == 0:
+            branch_name = proc.stdout.strip()
+            break
+    
+    return branch_name
```

### Comparing `grepsr_cli-0.7.9/grepsrcli/main.py` & `grepsr_cli-0.8.0/grepsrcli/main.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/autocomplete_zsh.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/autocomplete_zsh.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/node_boilerplate.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/node_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/php_boilerplate.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/php_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/php_brp_boilerplate.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/php_brp_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/php_vc_boilerplate.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/php_vc_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/grepsrcli/templates/py_boilerplate.jinja2` & `grepsr_cli-0.8.0/grepsrcli/templates/py_boilerplate.jinja2`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/setup.py` & `grepsr_cli-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/tests/test_grepsrcli.py` & `grepsr_cli-0.8.0/tests/test_grepsrcli.py`

 * *Files identical despite different names*

### Comparing `grepsr_cli-0.7.9/tests/test_unit.py` & `grepsr_cli-0.8.0/tests/test_unit.py`

 * *Files identical despite different names*

