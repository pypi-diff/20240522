# Comparing `tmp/cowboy_client-0.0.8.tar.gz` & `tmp/cowboy_client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowboy_client-0.0.8.tar", last modified: Sun May 12 02:29:03 2024, max compression
+gzip compressed data, was "cowboy_client-0.0.9.tar", last modified: Sun May 12 02:59:27 2024, max compression
```

## Comparing `cowboy_client-0.0.8.tar` & `cowboy_client-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.663680 cowboy_client-0.0.8/
--rw-rw-rw-   0        0        0      303 2024-05-12 02:29:03.657356 cowboy_client-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.568744 cowboy_client-0.0.8/cowboy/
--rw-rw-rw-   0        0        0        0 2024-05-11 22:06:49.000000 cowboy_client-0.0.8/cowboy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.580691 cowboy_client-0.0.8/cowboy/api_cmds/
--rw-rw-rw-   0        0        0      225 2024-05-09 22:21:29.000000 cowboy_client-0.0.8/cowboy/api_cmds/__init__.py
--rw-rw-rw-   0        0        0      512 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/api_cmds/baseline.py
--rw-rw-rw-   0        0        0      187 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/api_cmds/coverage.py
--rw-rw-rw-   0        0        0     1284 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/api_cmds/sorted_coverage.py
--rw-rw-rw-   0        0        0     7474 2024-05-12 02:08:57.000000 cowboy_client-0.0.8/cowboy/cli.py
--rw-rw-rw-   0        0        0      265 2024-05-11 16:09:06.000000 cowboy_client-0.0.8/cowboy/config.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.583574 cowboy_client-0.0.8/cowboy/db/
--rw-rw-rw-   0        0        0        0 2024-05-09 01:20:33.000000 cowboy_client-0.0.8/cowboy/db/__init__.py
--rw-rw-rw-   0        0        0     2614 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/db/core.py
--rw-rw-rw-   0        0        0      147 2024-04-25 17:09:39.000000 cowboy_client-0.0.8/cowboy/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.587279 cowboy_client-0.0.8/cowboy/http/
--rw-rw-rw-   0        0        0       29 2024-05-06 17:20:10.000000 cowboy_client-0.0.8/cowboy/http/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/http/base.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.590573 cowboy_client-0.0.8/cowboy/repo/
--rw-rw-rw-   0        0        0        0 2024-04-29 17:49:42.000000 cowboy_client-0.0.8/cowboy/repo/__init__.py
--rw-rw-rw-   0        0        0     2824 2024-05-11 23:40:37.000000 cowboy_client-0.0.8/cowboy/repo/models.py
--rw-rw-rw-   0        0        0     2544 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/repo/repo.py
--rw-rw-rw-   0        0        0     8705 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/repo/runner.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.598091 cowboy_client-0.0.8/cowboy/task_client/
--rw-rw-rw-   0        0        0        0 2024-05-11 16:23:23.000000 cowboy_client-0.0.8/cowboy/task_client/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-11 19:41:02.000000 cowboy_client-0.0.8/cowboy/task_client/configure_logger.py
--rw-rw-rw-   0        0        0     4938 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy/task_client/runtest_client.py
--rw-rw-rw-   0        0        0      208 2024-04-23 15:26:05.000000 cowboy_client-0.0.8/cowboy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.657356 cowboy_client-0.0.8/cowboy_client.egg-info/
--rw-rw-rw-   0        0        0      303 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1420 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-12 02:29:03.000000 cowboy_client-0.0.8/cowboy_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.617213 cowboy_client-0.0.8/cowboy_lib/
--rw-rw-rw-   0        0        0        0 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.618709 cowboy_client-0.0.8/cowboy_lib/api/
--rw-rw-rw-   0        0        0        0 2024-05-12 02:10:17.000000 cowboy_client-0.0.8/cowboy_lib/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.618709 cowboy_client-0.0.8/cowboy_lib/api/runner/
--rw-rw-rw-   0        0        0        0 2024-05-12 02:10:32.000000 cowboy_client-0.0.8/cowboy_lib/api/runner/__init__.py
--rw-rw-rw-   0        0        0     3474 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/api/runner/shared.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.618709 cowboy_client-0.0.8/cowboy_lib/ast/
--rw-rw-rw-   0        0        0      110 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/ast/__init__.py
--rw-rw-rw-   0        0        0     4696 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/ast/code.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.630085 cowboy_client-0.0.8/cowboy_lib/ast/python/
--rw-rw-rw-   0        0        0        0 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/ast/python/__init__.py
--rw-rw-rw-   0        0        0     5561 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/ast/python/ast.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.633928 cowboy_client-0.0.8/cowboy_lib/baseline/
--rw-rw-rw-   0        0        0       53 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/baseline/__init__.py
--rw-rw-rw-   0        0        0     5392 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/baseline/target_coverage.py
--rw-rw-rw-   0        0        0    17335 2024-05-09 22:10:33.000000 cowboy_client-0.0.8/cowboy_lib/coverage.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.637727 cowboy_client-0.0.8/cowboy_lib/llm/
--rw-rw-rw-   0        0        0       42 2024-05-06 20:53:59.000000 cowboy_client-0.0.8/cowboy_lib/llm/__init__.py
--rw-rw-rw-   0        0        0      937 2024-05-06 20:53:59.000000 cowboy_client-0.0.8/cowboy_lib/llm/invoke_llm.py
--rw-rw-rw-   0        0        0     8729 2024-05-11 22:12:06.000000 cowboy_client-0.0.8/cowboy_lib/llm/models.py
--rw-rw-rw-   0        0        0      993 2024-05-06 20:53:59.000000 cowboy_client-0.0.8/cowboy_lib/llm/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.650847 cowboy_client-0.0.8/cowboy_lib/repo/
--rw-rw-rw-   0        0        0      132 2024-04-30 00:18:47.000000 cowboy_client-0.0.8/cowboy_lib/repo/__init__.py
--rw-rw-rw-   0        0        0     7566 2024-05-08 01:26:05.000000 cowboy_client-0.0.8/cowboy_lib/repo/repository.py
--rw-rw-rw-   0        0        0     7347 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/repo/source_file.py
--rw-rw-rw-   0        0        0     4190 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/repo/source_repo.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.656553 cowboy_client-0.0.8/cowboy_lib/test_modules/
--rw-rw-rw-   0        0        0       74 2024-05-06 20:53:59.000000 cowboy_client-0.0.8/cowboy_lib/test_modules/__init__.py
--rw-rw-rw-   0        0        0     1116 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/test_modules/target_code.py
--rw-rw-rw-   0        0        0     6436 2024-05-12 02:08:04.000000 cowboy_client-0.0.8/cowboy_lib/test_modules/test_module.py
--rw-rw-rw-   0        0        0     1127 2024-04-30 23:46:20.000000 cowboy_client-0.0.8/cowboy_lib/utils.py
--rw-rw-rw-   0        0        0       42 2024-05-12 02:29:03.663680 cowboy_client-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      646 2024-05-12 02:28:21.000000 cowboy_client-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-12 02:29:03.657356 cowboy_client-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2024-05-08 13:39:51.000000 cowboy_client-0.0.8/tests/test_commit.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.871726 cowboy_client-0.0.9/
+-rw-rw-rw-   0        0        0      303 2024-05-12 02:59:27.869726 cowboy_client-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.777227 cowboy_client-0.0.9/cowboy/
+-rw-rw-rw-   0        0        0        0 2024-05-11 22:06:49.000000 cowboy_client-0.0.9/cowboy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.784828 cowboy_client-0.0.9/cowboy/api_cmds/
+-rw-rw-rw-   0        0        0      225 2024-05-09 22:21:29.000000 cowboy_client-0.0.9/cowboy/api_cmds/__init__.py
+-rw-rw-rw-   0        0        0      512 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/api_cmds/baseline.py
+-rw-rw-rw-   0        0        0      187 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/api_cmds/coverage.py
+-rw-rw-rw-   0        0        0     1284 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/api_cmds/sorted_coverage.py
+-rw-rw-rw-   0        0        0     7455 2024-05-12 02:56:05.000000 cowboy_client-0.0.9/cowboy/cli.py
+-rw-rw-rw-   0        0        0      265 2024-05-11 16:09:06.000000 cowboy_client-0.0.9/cowboy/config.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.787861 cowboy_client-0.0.9/cowboy/db/
+-rw-rw-rw-   0        0        0        0 2024-05-09 01:20:33.000000 cowboy_client-0.0.9/cowboy/db/__init__.py
+-rw-rw-rw-   0        0        0     2614 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/db/core.py
+-rw-rw-rw-   0        0        0      147 2024-04-25 17:09:39.000000 cowboy_client-0.0.9/cowboy/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.790986 cowboy_client-0.0.9/cowboy/http/
+-rw-rw-rw-   0        0        0       29 2024-05-06 17:20:10.000000 cowboy_client-0.0.9/cowboy/http/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/http/base.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.799103 cowboy_client-0.0.9/cowboy/repo/
+-rw-rw-rw-   0        0        0        0 2024-04-29 17:49:42.000000 cowboy_client-0.0.9/cowboy/repo/__init__.py
+-rw-rw-rw-   0        0        0     2824 2024-05-11 23:40:37.000000 cowboy_client-0.0.9/cowboy/repo/models.py
+-rw-rw-rw-   0        0        0     2544 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/repo/repo.py
+-rw-rw-rw-   0        0        0     8705 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy/repo/runner.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.804317 cowboy_client-0.0.9/cowboy/task_client/
+-rw-rw-rw-   0        0        0        0 2024-05-11 16:23:23.000000 cowboy_client-0.0.9/cowboy/task_client/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-11 19:41:02.000000 cowboy_client-0.0.9/cowboy/task_client/configure_logger.py
+-rw-rw-rw-   0        0        0     4940 2024-05-12 02:58:43.000000 cowboy_client-0.0.9/cowboy/task_client/runtest_client.py
+-rw-rw-rw-   0        0        0      208 2024-04-23 15:26:05.000000 cowboy_client-0.0.9/cowboy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.867724 cowboy_client-0.0.9/cowboy_client.egg-info/
+-rw-rw-rw-   0        0        0      303 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1420 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-12 02:59:27.000000 cowboy_client-0.0.9/cowboy_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.825564 cowboy_client-0.0.9/cowboy_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.827941 cowboy_client-0.0.9/cowboy_lib/api/
+-rw-rw-rw-   0        0        0        0 2024-05-12 02:10:17.000000 cowboy_client-0.0.9/cowboy_lib/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.831063 cowboy_client-0.0.9/cowboy_lib/api/runner/
+-rw-rw-rw-   0        0        0        0 2024-05-12 02:10:32.000000 cowboy_client-0.0.9/cowboy_lib/api/runner/__init__.py
+-rw-rw-rw-   0        0        0     3543 2024-05-12 02:50:34.000000 cowboy_client-0.0.9/cowboy_lib/api/runner/shared.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.834609 cowboy_client-0.0.9/cowboy_lib/ast/
+-rw-rw-rw-   0        0        0      110 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/ast/__init__.py
+-rw-rw-rw-   0        0        0     4696 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/ast/code.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.837682 cowboy_client-0.0.9/cowboy_lib/ast/python/
+-rw-rw-rw-   0        0        0        0 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/ast/python/__init__.py
+-rw-rw-rw-   0        0        0     5561 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/ast/python/ast.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.842261 cowboy_client-0.0.9/cowboy_lib/baseline/
+-rw-rw-rw-   0        0        0       53 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/baseline/__init__.py
+-rw-rw-rw-   0        0        0     5392 2024-05-12 02:08:04.000000 cowboy_client-0.0.9/cowboy_lib/baseline/target_coverage.py
+-rw-rw-rw-   0        0        0    17335 2024-05-09 22:10:33.000000 cowboy_client-0.0.9/cowboy_lib/coverage.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.851721 cowboy_client-0.0.9/cowboy_lib/llm/
+-rw-rw-rw-   0        0        0       42 2024-05-06 20:53:59.000000 cowboy_client-0.0.9/cowboy_lib/llm/__init__.py
+-rw-rw-rw-   0        0        0      937 2024-05-06 20:53:59.000000 cowboy_client-0.0.9/cowboy_lib/llm/invoke_llm.py
+-rw-rw-rw-   0        0        0     8729 2024-05-11 22:12:06.000000 cowboy_client-0.0.9/cowboy_lib/llm/models.py
+-rw-rw-rw-   0        0        0      993 2024-05-06 20:53:59.000000 cowboy_client-0.0.9/cowboy_lib/llm/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.859252 cowboy_client-0.0.9/cowboy_lib/repo/
+-rw-rw-rw-   0        0        0      132 2024-04-30 00:18:47.000000 cowboy_client-0.0.9/cowboy_lib/repo/__init__.py
+-rw-rw-rw-   0        0        0     7566 2024-05-08 01:26:05.000000 cowboy_client-0.0.9/cowboy_lib/repo/repository.py
+-rw-rw-rw-   0        0        0     7347 2024-05-12 02:08:04.000000 cowboy_client-0.0.9/cowboy_lib/repo/source_file.py
+-rw-rw-rw-   0        0        0     4190 2024-05-12 02:08:04.000000 cowboy_client-0.0.9/cowboy_lib/repo/source_repo.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.864244 cowboy_client-0.0.9/cowboy_lib/test_modules/
+-rw-rw-rw-   0        0        0       74 2024-05-06 20:53:59.000000 cowboy_client-0.0.9/cowboy_lib/test_modules/__init__.py
+-rw-rw-rw-   0        0        0     1116 2024-05-12 02:08:04.000000 cowboy_client-0.0.9/cowboy_lib/test_modules/target_code.py
+-rw-rw-rw-   0        0        0     6436 2024-05-12 02:08:04.000000 cowboy_client-0.0.9/cowboy_lib/test_modules/test_module.py
+-rw-rw-rw-   0        0        0     1127 2024-04-30 23:46:20.000000 cowboy_client-0.0.9/cowboy_lib/utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-12 02:59:27.871726 cowboy_client-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      646 2024-05-12 02:59:23.000000 cowboy_client-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 02:59:27.866724 cowboy_client-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-08 13:39:51.000000 cowboy_client-0.0.9/tests/test_commit.py
```

### Comparing `cowboy_client-0.0.8/cowboy/api_cmds/baseline.py` & `cowboy_client-0.0.9/cowboy/api_cmds/baseline.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/api_cmds/sorted_coverage.py` & `cowboy_client-0.0.9/cowboy/api_cmds/sorted_coverage.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/cli.py` & `cowboy_client-0.0.9/cowboy/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,20 +40,20 @@
             print("Client is alive!")
 
     def start_client(self):
         subprocess.Popen(
             [
                 "python",
                 "-m",
-                "src.task_client.runtest_client",
+                "cowboy.task_client.runtest_client",
                 str(self.heart_beat_fp),
                 str(self.heart_beat_interval),
             ],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            stdout=None,
+            stderr=None,
         )
 
     def is_alive(self):
         if not self.read_beat():
             return False
 
         # adding one to the interval to account lag
```

### Comparing `cowboy_client-0.0.8/cowboy/db/core.py` & `cowboy_client-0.0.9/cowboy/db/core.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/http/base.py` & `cowboy_client-0.0.9/cowboy/http/base.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/repo/models.py` & `cowboy_client-0.0.9/cowboy/repo/models.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/repo/repo.py` & `cowboy_client-0.0.9/cowboy/repo/repo.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/repo/runner.py` & `cowboy_client-0.0.9/cowboy/repo/runner.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy/task_client/runtest_client.py` & `cowboy_client-0.0.9/cowboy/task_client/runtest_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             self.curr_t.remove(task.task_id)
             self.completed += 1
             print("Outstanding tasks: ", len(self.curr_t))
             print("Total completed: ", self.completed)
 
     def start_polling(self):
         while True:
-            print("Polling server at: ", self.fetch_endpoint)
+            # print("Polling server at: ", self.fetch_endpoint)
             fetch_tasks = threading.Thread(target=self.fetch_tasks_thread, daemon=True)
             fetch_tasks.start()
 
             time.sleep(1.0)  # Poll every 'interval' second
 
     # TODO: might be better to write to pipe stdout and redir on the caller side,
     # because multiple processes can potentially be started and mess up the files
```

### Comparing `cowboy_client-0.0.8/cowboy_client.egg-info/SOURCES.txt` & `cowboy_client-0.0.9/cowboy_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/api/runner/shared.py` & `cowboy_client-0.0.9/cowboy_lib/api/runner/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cowboy_lib.utils import generate_id
 from cowboy_lib.repo.repository import PatchFile
 
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, ConfigDict
 from typing import List, Optional, Any, Tuple, Dict
 
 from pathlib import Path
 from enum import Enum
 
 from dataclasses import dataclass, field
 
@@ -18,14 +18,16 @@
 
 
 class Task(BaseModel):
     """
     Task datatype
     """
 
+    config = ConfigDict(arbitrary_types_allowed=True)
+
     repo_name: str
     task_id: str = Field(default_factory=lambda: generate_id())
     result: dict = Field(default_factory=dict)
     status: str = Field(default=TaskStatus.PENDING.value)
     task_args: Optional[Any]
```

### Comparing `cowboy_client-0.0.8/cowboy_lib/ast/code.py` & `cowboy_client-0.0.9/cowboy_lib/ast/code.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/ast/python/ast.py` & `cowboy_client-0.0.9/cowboy_lib/ast/python/ast.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/baseline/target_coverage.py` & `cowboy_client-0.0.9/cowboy_lib/baseline/target_coverage.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/coverage.py` & `cowboy_client-0.0.9/cowboy_lib/coverage.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/llm/invoke_llm.py` & `cowboy_client-0.0.9/cowboy_lib/llm/invoke_llm.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/llm/models.py` & `cowboy_client-0.0.9/cowboy_lib/llm/models.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/llm/utils.py` & `cowboy_client-0.0.9/cowboy_lib/llm/utils.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/repo/repository.py` & `cowboy_client-0.0.9/cowboy_lib/repo/repository.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/repo/source_file.py` & `cowboy_client-0.0.9/cowboy_lib/repo/source_file.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/repo/source_repo.py` & `cowboy_client-0.0.9/cowboy_lib/repo/source_repo.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/test_modules/target_code.py` & `cowboy_client-0.0.9/cowboy_lib/test_modules/target_code.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/test_modules/test_module.py` & `cowboy_client-0.0.9/cowboy_lib/test_modules/test_module.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/cowboy_lib/utils.py` & `cowboy_client-0.0.9/cowboy_lib/utils.py`

 * *Files identical despite different names*

### Comparing `cowboy_client-0.0.8/setup.py` & `cowboy_client-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import Extension, find_packages, setup
 
 setup(
     name="cowboy-client",
-    version="0.0.8",
+    version="0.0.9",
     packages=find_packages(),
     description="Cowboy Client Interface",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     author="John Peng",
     author_email="kongyijipeng@gmail.com",
     install_requires=[
```

