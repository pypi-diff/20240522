# Comparing `tmp/tcrutils-12.0.166.tar.gz` & `tmp/tcrutils-12.0.167.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.166.tar", max compression
+gzip compressed data, was "tcrutils-12.0.167.tar", max compression
```

## Comparing `tcrutils-12.0.166.tar` & `tcrutils-12.0.167.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.166/LICENSE
--rw-r--r--   0        0        0      609 2024-05-20 23:14:02.390095 tcrutils-12.0.166/pyproject.toml
--rw-r--r--   0        0        0     2612 2024-05-17 16:58:05.174624 tcrutils-12.0.166/README.md
--rw-r--r--   0        0        0     4783 2024-05-20 23:13:37.975811 tcrutils-12.0.166/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-05-20 23:14:05.016352 tcrutils-12.0.166/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.166/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.166/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.166/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.166/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      444 2024-05-20 23:01:55.967516 tcrutils-12.0.166/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.166/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.166/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.166/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.166/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.166/tcrutils/dr/__init__.py
--rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.166/tcrutils/dr/core.py
--rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.166/tcrutils/dr/error.py
--rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.166/tcrutils/dr/EXECUTE.md
--rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.166/tcrutils/dr/placeholder_sets.py
--rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.166/tcrutils/dr/placeholders/__init__.py
--rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.166/tcrutils/dr/placeholders/p_discord.py
--rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.166/tcrutils/dr/placeholders/p_math.py
--rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.166/tcrutils/dr/placeholders/p_text.py
--rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.166/tcrutils/dr/PLACEHOLDERS.md
--rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.166/tcrutils/dr/util.py
--rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.166/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.166/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.166/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.166/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.166/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.166/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.166/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.166/tcrutils/src/tcr_cloud_imports.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.166/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.166/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.166/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.166/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.166/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.166/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.166/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.166/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.166/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.166/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.166/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.166/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.166/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.166/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.166/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.166/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.166/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.166/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     2858 2024-05-20 23:13:27.081335 tcrutils-12.0.166/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.166/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.166/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.166/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.166/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.166/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29286 2024-04-19 22:20:25.582375 tcrutils-12.0.166/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.166/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.166/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     4092 2024-05-19 19:04:07.466948 tcrutils-12.0.166/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.166/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.166/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.166/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.166/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.166/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.166/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.166/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 tcrutils-12.0.166/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.167/LICENSE
+-rw-r--r--   0        0        0      609 2024-05-21 21:24:38.647024 tcrutils-12.0.167/pyproject.toml
+-rw-r--r--   0        0        0     2612 2024-05-17 16:58:05.174624 tcrutils-12.0.167/README.md
+-rw-r--r--   0        0        0     4783 2024-05-20 23:13:37.975811 tcrutils-12.0.167/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-21 21:24:41.297778 tcrutils-12.0.167/tcrutils/_version.py
+-rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.167/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.167/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.167/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.167/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      444 2024-05-20 23:01:55.967516 tcrutils-12.0.167/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.167/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.167/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.167/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.167/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.167/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.167/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.167/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.167/tcrutils/dr/EXECUTE.md
+-rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.167/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.167/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.167/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.167/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.167/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.167/tcrutils/dr/PLACEHOLDERS.md
+-rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.167/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.167/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.167/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.167/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.167/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.167/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0     1655 2024-05-02 14:13:55.166736 tcrutils-12.0.167/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.167/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.167/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.167/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.167/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.167/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0     5892 2024-05-02 12:11:41.388680 tcrutils-12.0.167/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.167/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.167/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.167/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.167/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.167/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.167/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.167/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.167/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.167/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.167/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.167/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.167/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.167/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.167/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     2858 2024-05-20 23:13:27.081335 tcrutils-12.0.167/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.167/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.167/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.167/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.167/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.167/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29421 2024-05-21 21:23:31.164988 tcrutils-12.0.167/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.167/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.167/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     4092 2024-05-19 19:04:07.466948 tcrutils-12.0.167/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.167/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.167/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.167/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.167/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.167/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.167/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.167/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 tcrutils-12.0.167/PKG-INFO
```

### Comparing `tcrutils-12.0.166/LICENSE` & `tcrutils-12.0.167/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/pyproject.toml` & `tcrutils-12.0.167/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.166"
+version = "12.0.167"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
```

### Comparing `tcrutils-12.0.166/README.md` & `tcrutils-12.0.167/README.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/__init__.py` & `tcrutils-12.0.167/tcrutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/__init__.py` & `tcrutils-12.0.167/tcrutils/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.167/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.167/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.167/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.167/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.167/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/core.py` & `tcrutils-12.0.167/tcrutils/dr/core.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/error.py` & `tcrutils-12.0.167/tcrutils/dr/error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/EXECUTE.md` & `tcrutils-12.0.167/tcrutils/dr/EXECUTE.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/placeholder_sets.py` & `tcrutils-12.0.167/tcrutils/dr/placeholder_sets.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/placeholders/p_discord.py` & `tcrutils-12.0.167/tcrutils/dr/placeholders/p_discord.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/placeholders/p_math.py` & `tcrutils-12.0.167/tcrutils/dr/placeholders/p_math.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/placeholders/p_text.py` & `tcrutils-12.0.167/tcrutils/dr/placeholders/p_text.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/PLACEHOLDERS.md` & `tcrutils-12.0.167/tcrutils/dr/PLACEHOLDERS.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/dr/util.py` & `tcrutils-12.0.167/tcrutils/dr/util.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.167/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.167/tcrutils/imgui/tcri_handler.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.167/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_class.py` & `tcrutils-12.0.167/tcrutils/src/tcr_class.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.167/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_cloud_imports.py` & `tcrutils-12.0.167/tcrutils/src/tcr_cloud_imports.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.167/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_console.py` & `tcrutils-12.0.167/tcrutils/src/tcr_console.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.167/tcrutils/src/tcr_decorator.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.167/tcrutils/src/tcr_dev.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.167/tcrutils/src/tcr_dict.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_error.py` & `tcrutils-12.0.167/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.167/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.167/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.167/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_input.py` & `tcrutils-12.0.167/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.167/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_int.py` & `tcrutils-12.0.167/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.167/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_joke.py` & `tcrutils-12.0.167/tcrutils/src/tcr_joke.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_language.py` & `tcrutils-12.0.167/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.167/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.167/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_null.py` & `tcrutils-12.0.167/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.167/tcrutils/src/tcr_overload.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_path.py` & `tcrutils-12.0.167/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_print.py` & `tcrutils-12.0.167/tcrutils/src/tcr_print.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
       and not isinstance(it, str | bytes)
       # If their length can be checked (e.g. not generators)
       and able(len, it)
       # And they have any length:
       and len(it) > 0
     ):
       if isinstance(it, Mapping):
-        if len(it) == 1:
+        if len(it) == 1 and ((type(next(iter(it.values()))) in (int, float, complex, bool)) or next(iter(it.values())) in (None, Null, '', [], (), {}, set())):
           force_no_indent = -1
       else:
         # Case 1: If the iterable in question contains iterables
         # If there is at most 1 iterable in the outer iterable of iterables
         if len(it) <= Or(kwargs.get('let_no_inder_max_iterables'), 1) and any(isinstance(x, Iterable) for x in it):
           force_no_indent = -1
         # Case 2: If the outer iterable consists of non-iterables: If there are at most 4 non-iterables
```

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.167/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_run.py` & `tcrutils-12.0.167/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.167/tcrutils/src/tcr_sdb.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_string.py` & `tcrutils-12.0.167/tcrutils/src/tcr_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.167/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_test.py` & `tcrutils-12.0.167/tcrutils/src/tcr_test.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.167/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.167/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/tcrutils/src/tcr_void.py` & `tcrutils-12.0.167/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.166/PKG-INFO` & `tcrutils-12.0.167/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcrutils
-Version: 12.0.166
+Version: 12.0.167
 Summary: Useful stuff for TCR projects!
 License: GPL-3.0
 Author: TheCreatorrrr
 Requires-Python: >=3.11.0,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tcrutils Version: 12.0.166 Summary: Useful stuff
+Metadata-Version: 2.1 Name: tcrutils Version: 12.0.167 Summary: Useful stuff
 for TCR projects! License: GPL-3.0 Author: TheCreatorrrr Requires-Python:
 >=3.11.0,<3.13 Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: attr (>=0.3.2,<0.4.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: colored (>=2.2.4,<3.0.0) Requires-Dist: hikari
 (>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-arc (>=1.3.0,<2.0.0) Requires-
```

