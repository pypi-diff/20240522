# Comparing `tmp/tcrutils-12.0.175.tar.gz` & `tmp/tcrutils-12.0.176.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcrutils-12.0.175.tar", max compression
+gzip compressed data, was "tcrutils-12.0.176.tar", max compression
```

## Comparing `tcrutils-12.0.175.tar` & `tcrutils-12.0.176.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.175/LICENSE
--rw-r--r--   0        0        0      609 2024-05-22 16:38:52.990879 tcrutils-12.0.175/pyproject.toml
--rw-r--r--   0        0        0     2612 2024-05-17 16:58:05.174624 tcrutils-12.0.175/README.md
--rw-r--r--   0        0        0     4868 2024-05-22 16:38:27.389533 tcrutils-12.0.175/tcrutils/__init__.py
--rw-r--r--   0        0        0      209 2024-05-22 16:38:55.485303 tcrutils-12.0.175/tcrutils/_version.py
--rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.175/tcrutils/discord/__init__.py
--rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.175/tcrutils/discord/tcrd_alias.py
--rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.175/tcrutils/discord/tcrd_constants.py
--rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.175/tcrutils/discord/tcrd_embeds.py
--rw-r--r--   0        0        0      445 2024-05-22 16:38:45.538275 tcrutils-12.0.175/tcrutils/discord/tcrd_limits.py
--rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.175/tcrutils/discord/tcrd_permissions.py
--rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.175/tcrutils/discord/tcrd_snowflake.py
--rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.175/tcrutils/discord/tcrd_string.py
--rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.175/tcrutils/discord/tcrd_types.py
--rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.175/tcrutils/dr/__init__.py
--rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.175/tcrutils/dr/core.py
--rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.175/tcrutils/dr/error.py
--rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.175/tcrutils/dr/EXECUTE.md
--rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.175/tcrutils/dr/placeholder_sets.py
--rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.175/tcrutils/dr/placeholders/__init__.py
--rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.175/tcrutils/dr/placeholders/p_discord.py
--rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.175/tcrutils/dr/placeholders/p_math.py
--rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.175/tcrutils/dr/placeholders/p_text.py
--rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.175/tcrutils/dr/PLACEHOLDERS.md
--rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.175/tcrutils/dr/util.py
--rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.175/tcrutils/imgui/__init__.py
--rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.175/tcrutils/imgui/tcri_dependencies.py
--rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.175/tcrutils/imgui/tcri_handler.py
--rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.175/tcrutils/imgui/types/tcri_types_imgui.py
--rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.175/tcrutils/src/tcr_b64.py
--rw-r--r--   0        0        0      980 2024-05-22 09:51:37.173518 tcrutils-12.0.175/tcrutils/src/tcr_class.py
--rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.175/tcrutils/src/tcr_classfuncs.py
--rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.175/tcrutils/src/tcr_cloud_imports.py
--rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.175/tcrutils/src/tcr_compare.py
--rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.175/tcrutils/src/tcr_console.py
--rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.175/tcrutils/src/tcr_constants.py
--rw-r--r--   0        0        0     6457 2024-05-22 16:38:45.539276 tcrutils-12.0.175/tcrutils/src/tcr_decorator.py
--rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.175/tcrutils/src/tcr_dev.py
--rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.175/tcrutils/src/tcr_dict.py
--rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.175/tcrutils/src/tcr_dir.py
--rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.175/tcrutils/src/tcr_error.py
--rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.175/tcrutils/src/tcr_extract_error.py
--rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.175/tcrutils/src/tcr_F.py
--rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.175/tcrutils/src/tcr_getch.py
--rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.175/tcrutils/src/tcr_inject.py
--rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.175/tcrutils/src/tcr_input.py
--rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.175/tcrutils/src/tcr_inspect.py
--rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.175/tcrutils/src/tcr_int.py
--rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.175/tcrutils/src/tcr_iterable.py
--rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.175/tcrutils/src/tcr_joke.py
--rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.175/tcrutils/src/tcr_language.py
--rw-r--r--   0        0        0     2860 2024-05-22 16:38:45.539276 tcrutils-12.0.175/tcrutils/src/tcr_markdown.py
--rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.175/tcrutils/src/tcr_misspellings.py
--rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.175/tcrutils/src/tcr_null.py
--rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.175/tcrutils/src/tcr_other.py
--rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.175/tcrutils/src/tcr_overload.py
--rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.175/tcrutils/src/tcr_path.py
--rw-r--r--   0        0        0    29421 2024-05-21 21:23:31.164988 tcrutils-12.0.175/tcrutils/src/tcr_print.py
--rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.175/tcrutils/src/tcr_regex.py
--rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.175/tcrutils/src/tcr_run.py
--rw-r--r--   0        0        0     5227 2024-05-22 16:38:45.538275 tcrutils-12.0.175/tcrutils/src/tcr_sdb.py
--rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.175/tcrutils/src/tcr_string.py
--rw-r--r--   0        0        0      358 2024-05-22 10:36:37.266846 tcrutils-12.0.175/tcrutils/src/tcr_temp.py
--rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.175/tcrutils/src/tcr_terminal.py
--rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.175/tcrutils/src/tcr_test.py
--rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.175/tcrutils/src/tcr_timestr.py
--rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.175/tcrutils/src/tcr_types.py
--rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.175/tcrutils/src/tcr_uptime.py
--rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.175/tcrutils/src/tcr_void.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 tcrutils-12.0.175/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-11-04 23:11:02.596565 tcrutils-12.0.176/LICENSE
+-rw-r--r--   0        0        0      609 2024-05-22 20:37:11.476867 tcrutils-12.0.176/pyproject.toml
+-rw-r--r--   0        0        0     2612 2024-05-17 16:58:05.174624 tcrutils-12.0.176/README.md
+-rw-r--r--   0        0        0     4868 2024-05-22 16:38:27.389533 tcrutils-12.0.176/tcrutils/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-22 20:37:13.634659 tcrutils-12.0.176/tcrutils/_version.py
+-rw-r--r--   0        0        0      778 2024-04-07 14:45:13.688614 tcrutils-12.0.176/tcrutils/discord/__init__.py
+-rw-r--r--   0        0        0       81 2024-04-07 12:08:11.885327 tcrutils-12.0.176/tcrutils/discord/tcrd_alias.py
+-rw-r--r--   0        0        0       98 2024-01-19 16:02:12.088184 tcrutils-12.0.176/tcrutils/discord/tcrd_constants.py
+-rw-r--r--   0        0        0     2244 2024-03-19 14:26:22.018806 tcrutils-12.0.176/tcrutils/discord/tcrd_embeds.py
+-rw-r--r--   0        0        0      445 2024-05-22 16:38:45.538275 tcrutils-12.0.176/tcrutils/discord/tcrd_limits.py
+-rw-r--r--   0        0        0     4302 2024-02-23 20:13:37.429288 tcrutils-12.0.176/tcrutils/discord/tcrd_permissions.py
+-rw-r--r--   0        0        0      518 2024-02-23 20:13:37.429288 tcrutils-12.0.176/tcrutils/discord/tcrd_snowflake.py
+-rw-r--r--   0        0        0     5788 2024-02-23 20:51:35.076170 tcrutils-12.0.176/tcrutils/discord/tcrd_string.py
+-rw-r--r--   0        0        0     2156 2024-02-23 20:13:37.428288 tcrutils-12.0.176/tcrutils/discord/tcrd_types.py
+-rw-r--r--   0        0        0      414 2024-05-07 17:26:58.759172 tcrutils-12.0.176/tcrutils/dr/__init__.py
+-rw-r--r--   0        0        0     9089 2024-05-13 14:29:20.133657 tcrutils-12.0.176/tcrutils/dr/core.py
+-rw-r--r--   0        0        0     2493 2024-05-07 17:26:58.759172 tcrutils-12.0.176/tcrutils/dr/error.py
+-rw-r--r--   0        0        0     5744 2024-05-15 21:25:46.216676 tcrutils-12.0.176/tcrutils/dr/EXECUTE.md
+-rw-r--r--   0        0        0     3647 2024-05-15 22:09:37.638712 tcrutils-12.0.176/tcrutils/dr/placeholder_sets.py
+-rw-r--r--   0        0        0       72 2024-05-11 19:56:28.575713 tcrutils-12.0.176/tcrutils/dr/placeholders/__init__.py
+-rw-r--r--   0        0        0     9539 2024-05-15 15:53:54.306491 tcrutils-12.0.176/tcrutils/dr/placeholders/p_discord.py
+-rw-r--r--   0        0        0     4387 2024-05-13 12:18:40.217769 tcrutils-12.0.176/tcrutils/dr/placeholders/p_math.py
+-rw-r--r--   0        0        0     1566 2024-05-12 18:44:29.418679 tcrutils-12.0.176/tcrutils/dr/placeholders/p_text.py
+-rw-r--r--   0        0        0    14654 2024-05-18 16:30:33.599876 tcrutils-12.0.176/tcrutils/dr/PLACEHOLDERS.md
+-rw-r--r--   0        0        0     6233 2024-05-15 22:16:27.695353 tcrutils-12.0.176/tcrutils/dr/util.py
+-rw-r--r--   0        0        0      140 2024-05-02 14:13:55.166736 tcrutils-12.0.176/tcrutils/imgui/__init__.py
+-rw-r--r--   0        0        0      768 2024-04-26 20:35:07.575035 tcrutils-12.0.176/tcrutils/imgui/tcri_dependencies.py
+-rw-r--r--   0        0        0     3386 2024-05-12 19:36:59.859676 tcrutils-12.0.176/tcrutils/imgui/tcri_handler.py
+-rw-r--r--   0        0        0   141566 2024-04-27 23:44:35.849274 tcrutils-12.0.176/tcrutils/imgui/types/tcri_types_imgui.py
+-rw-r--r--   0        0        0      456 2024-04-30 10:22:34.407852 tcrutils-12.0.176/tcrutils/src/tcr_b64.py
+-rw-r--r--   0        0        0      980 2024-05-22 09:51:37.173518 tcrutils-12.0.176/tcrutils/src/tcr_class.py
+-rw-r--r--   0        0        0      550 2024-03-19 14:19:35.424053 tcrutils-12.0.176/tcrutils/src/tcr_classfuncs.py
+-rw-r--r--   0        0        0     4370 2024-05-13 18:53:12.432926 tcrutils-12.0.176/tcrutils/src/tcr_cloud_imports.py
+-rw-r--r--   0        0        0     2270 2024-04-26 17:59:16.788049 tcrutils-12.0.176/tcrutils/src/tcr_compare.py
+-rw-r--r--   0        0        0     7105 2024-05-11 21:52:09.173816 tcrutils-12.0.176/tcrutils/src/tcr_console.py
+-rw-r--r--   0        0        0      347 2023-12-23 23:11:59.731531 tcrutils-12.0.176/tcrutils/src/tcr_constants.py
+-rw-r--r--   0        0        0     6457 2024-05-22 16:38:45.539276 tcrutils-12.0.176/tcrutils/src/tcr_decorator.py
+-rw-r--r--   0        0        0     4881 2024-05-03 17:37:29.849453 tcrutils-12.0.176/tcrutils/src/tcr_dev.py
+-rw-r--r--   0        0        0     5802 2024-05-02 10:34:38.791291 tcrutils-12.0.176/tcrutils/src/tcr_dict.py
+-rw-r--r--   0        0        0      245 2024-04-07 14:45:13.688614 tcrutils-12.0.176/tcrutils/src/tcr_dir.py
+-rw-r--r--   0        0        0      987 2024-02-17 18:48:50.338606 tcrutils-12.0.176/tcrutils/src/tcr_error.py
+-rw-r--r--   0        0        0     1006 2024-03-08 15:03:30.998287 tcrutils-12.0.176/tcrutils/src/tcr_extract_error.py
+-rw-r--r--   0        0        0       81 2023-12-23 23:01:58.550444 tcrutils-12.0.176/tcrutils/src/tcr_F.py
+-rw-r--r--   0        0        0     1093 2023-11-06 18:49:03.607042 tcrutils-12.0.176/tcrutils/src/tcr_getch.py
+-rw-r--r--   0        0        0     4301 2024-03-19 17:47:20.530561 tcrutils-12.0.176/tcrutils/src/tcr_inject.py
+-rw-r--r--   0        0        0      950 2024-01-29 17:47:31.333032 tcrutils-12.0.176/tcrutils/src/tcr_input.py
+-rw-r--r--   0        0        0     2241 2024-04-11 22:00:21.527336 tcrutils-12.0.176/tcrutils/src/tcr_inspect.py
+-rw-r--r--   0        0        0     1106 2024-05-14 16:33:00.727996 tcrutils-12.0.176/tcrutils/src/tcr_int.py
+-rw-r--r--   0        0        0     7697 2024-02-23 20:13:37.423287 tcrutils-12.0.176/tcrutils/src/tcr_iterable.py
+-rw-r--r--   0        0        0     3438 2024-05-15 16:14:26.304132 tcrutils-12.0.176/tcrutils/src/tcr_joke.py
+-rw-r--r--   0        0        0     2748 2024-02-15 12:39:41.609862 tcrutils-12.0.176/tcrutils/src/tcr_language.py
+-rw-r--r--   0        0        0     2860 2024-05-22 16:38:45.539276 tcrutils-12.0.176/tcrutils/src/tcr_markdown.py
+-rw-r--r--   0        0        0     1299 2024-02-23 20:13:37.423287 tcrutils-12.0.176/tcrutils/src/tcr_misspellings.py
+-rw-r--r--   0        0        0     1409 2024-03-19 17:47:20.529553 tcrutils-12.0.176/tcrutils/src/tcr_null.py
+-rw-r--r--   0        0        0      298 2024-02-23 23:16:27.228751 tcrutils-12.0.176/tcrutils/src/tcr_other.py
+-rw-r--r--   0        0        0     7591 2024-05-11 21:11:55.531404 tcrutils-12.0.176/tcrutils/src/tcr_overload.py
+-rw-r--r--   0        0        0     3127 2024-02-23 20:13:37.419287 tcrutils-12.0.176/tcrutils/src/tcr_path.py
+-rw-r--r--   0        0        0    29421 2024-05-21 21:23:31.164988 tcrutils-12.0.176/tcrutils/src/tcr_print.py
+-rw-r--r--   0        0        0     1361 2024-02-10 21:19:35.084757 tcrutils-12.0.176/tcrutils/src/tcr_regex.py
+-rw-r--r--   0        0        0      743 2023-11-07 15:44:27.527859 tcrutils-12.0.176/tcrutils/src/tcr_run.py
+-rw-r--r--   0        0        0     5389 2024-05-22 20:33:38.492292 tcrutils-12.0.176/tcrutils/src/tcr_sdb.py
+-rw-r--r--   0        0        0     4083 2024-04-12 20:31:09.874612 tcrutils-12.0.176/tcrutils/src/tcr_string.py
+-rw-r--r--   0        0        0      358 2024-05-22 10:36:37.266846 tcrutils-12.0.176/tcrutils/src/tcr_temp.py
+-rw-r--r--   0        0        0     1152 2024-03-19 17:47:20.531561 tcrutils-12.0.176/tcrutils/src/tcr_terminal.py
+-rw-r--r--   0        0        0     6977 2024-05-13 11:41:52.760202 tcrutils-12.0.176/tcrutils/src/tcr_test.py
+-rw-r--r--   0        0        0    16373 2024-02-23 20:13:37.427288 tcrutils-12.0.176/tcrutils/src/tcr_timestr.py
+-rw-r--r--   0        0        0      404 2024-05-11 19:19:25.965833 tcrutils-12.0.176/tcrutils/src/tcr_types.py
+-rw-r--r--   0        0        0     1819 2024-02-17 18:23:07.659452 tcrutils-12.0.176/tcrutils/src/tcr_uptime.py
+-rw-r--r--   0        0        0     1089 2024-01-13 22:57:18.979846 tcrutils-12.0.176/tcrutils/src/tcr_void.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 tcrutils-12.0.176/PKG-INFO
```

### Comparing `tcrutils-12.0.175/LICENSE` & `tcrutils-12.0.176/LICENSE`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/pyproject.toml` & `tcrutils-12.0.176/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 extend = "C:/CUSTOM_ASSETS/pyproject.toml"
 [tool.ruff.format]
 quote-style = "single"
 indent-style = "space"
 
 [tool.poetry]
 name = "tcrutils"
-version = "12.0.175"
+version = "12.0.176"
 description = "Useful stuff for TCR projects!"
 authors = ["TheCreatorrrr"]
 license = "GPL-3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11.0,<3.13"
```

### Comparing `tcrutils-12.0.175/README.md` & `tcrutils-12.0.176/README.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/__init__.py` & `tcrutils-12.0.176/tcrutils/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/__init__.py` & `tcrutils-12.0.176/tcrutils/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/tcrd_embeds.py` & `tcrutils-12.0.176/tcrutils/discord/tcrd_embeds.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/tcrd_permissions.py` & `tcrutils-12.0.176/tcrutils/discord/tcrd_permissions.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/tcrd_snowflake.py` & `tcrutils-12.0.176/tcrutils/discord/tcrd_snowflake.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/tcrd_string.py` & `tcrutils-12.0.176/tcrutils/discord/tcrd_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/discord/tcrd_types.py` & `tcrutils-12.0.176/tcrutils/discord/tcrd_types.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/core.py` & `tcrutils-12.0.176/tcrutils/dr/core.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/error.py` & `tcrutils-12.0.176/tcrutils/dr/error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/EXECUTE.md` & `tcrutils-12.0.176/tcrutils/dr/EXECUTE.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/placeholder_sets.py` & `tcrutils-12.0.176/tcrutils/dr/placeholder_sets.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/placeholders/p_discord.py` & `tcrutils-12.0.176/tcrutils/dr/placeholders/p_discord.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/placeholders/p_math.py` & `tcrutils-12.0.176/tcrutils/dr/placeholders/p_math.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/placeholders/p_text.py` & `tcrutils-12.0.176/tcrutils/dr/placeholders/p_text.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/PLACEHOLDERS.md` & `tcrutils-12.0.176/tcrutils/dr/PLACEHOLDERS.md`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/dr/util.py` & `tcrutils-12.0.176/tcrutils/dr/util.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/imgui/tcri_dependencies.py` & `tcrutils-12.0.176/tcrutils/imgui/tcri_dependencies.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/imgui/tcri_handler.py` & `tcrutils-12.0.176/tcrutils/imgui/tcri_handler.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/imgui/types/tcri_types_imgui.py` & `tcrutils-12.0.176/tcrutils/imgui/types/tcri_types_imgui.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_class.py` & `tcrutils-12.0.176/tcrutils/src/tcr_class.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_classfuncs.py` & `tcrutils-12.0.176/tcrutils/src/tcr_classfuncs.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_cloud_imports.py` & `tcrutils-12.0.176/tcrutils/src/tcr_cloud_imports.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_compare.py` & `tcrutils-12.0.176/tcrutils/src/tcr_compare.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_console.py` & `tcrutils-12.0.176/tcrutils/src/tcr_console.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_decorator.py` & `tcrutils-12.0.176/tcrutils/src/tcr_decorator.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_dev.py` & `tcrutils-12.0.176/tcrutils/src/tcr_dev.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_dict.py` & `tcrutils-12.0.176/tcrutils/src/tcr_dict.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_error.py` & `tcrutils-12.0.176/tcrutils/src/tcr_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_extract_error.py` & `tcrutils-12.0.176/tcrutils/src/tcr_extract_error.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_getch.py` & `tcrutils-12.0.176/tcrutils/src/tcr_getch.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_inject.py` & `tcrutils-12.0.176/tcrutils/src/tcr_inject.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_input.py` & `tcrutils-12.0.176/tcrutils/src/tcr_input.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_inspect.py` & `tcrutils-12.0.176/tcrutils/src/tcr_inspect.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_int.py` & `tcrutils-12.0.176/tcrutils/src/tcr_int.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_iterable.py` & `tcrutils-12.0.176/tcrutils/src/tcr_iterable.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_joke.py` & `tcrutils-12.0.176/tcrutils/src/tcr_joke.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_language.py` & `tcrutils-12.0.176/tcrutils/src/tcr_language.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_markdown.py` & `tcrutils-12.0.176/tcrutils/src/tcr_markdown.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_misspellings.py` & `tcrutils-12.0.176/tcrutils/src/tcr_misspellings.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_null.py` & `tcrutils-12.0.176/tcrutils/src/tcr_null.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_overload.py` & `tcrutils-12.0.176/tcrutils/src/tcr_overload.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_path.py` & `tcrutils-12.0.176/tcrutils/src/tcr_path.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_print.py` & `tcrutils-12.0.176/tcrutils/src/tcr_print.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_regex.py` & `tcrutils-12.0.176/tcrutils/src/tcr_regex.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_run.py` & `tcrutils-12.0.176/tcrutils/src/tcr_run.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_sdb.py` & `tcrutils-12.0.176/tcrutils/src/tcr_sdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib as p
 import shelve
 import shutil
 import string
-from collections.abc import Callable
-from typing import Any
+from collections.abc import Callable, Iterator
+from typing import Any, Self
 
 ALLOWED_CHARACTERS = string.ascii_letters + string.digits + "!&#'^~$,.%`{}[]();@_-+="  # Allowed characters in DB ID
 
 DISALLOWED_SEQUENCES = (
   'PRN',
   'CON',
   'AUX',
@@ -175,7 +175,13 @@
   def get_path(self) -> p.Path:
     return self.get_directory() / self.alnum_id
 
   def drop_db(self) -> None:
     """Close the shelf and delete the underlying system directory of this database instance."""
     self.s.close()
     shutil.rmtree(self.__directory / self.alnum_id)
+
+  @classmethod
+  def iter_all(cls) -> Iterator[str, Self]:
+    for path in cls.directory.iterdir():
+      yield path.name, cls(path.name)
+
```

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_string.py` & `tcrutils-12.0.176/tcrutils/src/tcr_string.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_terminal.py` & `tcrutils-12.0.176/tcrutils/src/tcr_terminal.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_test.py` & `tcrutils-12.0.176/tcrutils/src/tcr_test.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_timestr.py` & `tcrutils-12.0.176/tcrutils/src/tcr_timestr.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_uptime.py` & `tcrutils-12.0.176/tcrutils/src/tcr_uptime.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/tcrutils/src/tcr_void.py` & `tcrutils-12.0.176/tcrutils/src/tcr_void.py`

 * *Files identical despite different names*

### Comparing `tcrutils-12.0.175/PKG-INFO` & `tcrutils-12.0.176/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tcrutils
-Version: 12.0.175
+Version: 12.0.176
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
-Metadata-Version: 2.1 Name: tcrutils Version: 12.0.175 Summary: Useful stuff
+Metadata-Version: 2.1 Name: tcrutils Version: 12.0.176 Summary: Useful stuff
 for TCR projects! License: GPL-3.0 Author: TheCreatorrrr Requires-Python:
 >=3.11.0,<3.13 Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: attr (>=0.3.2,<0.4.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: colored (>=2.2.4,<3.0.0) Requires-Dist: hikari
 (>=2.0.0.dev122,<3.0.0) Requires-Dist: hikari-arc (>=1.3.0,<2.0.0) Requires-
```

