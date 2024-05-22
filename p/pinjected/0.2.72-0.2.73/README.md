# Comparing `tmp/pinjected-0.2.72.tar.gz` & `tmp/pinjected-0.2.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinjected-0.2.72.tar", max compression
+gzip compressed data, was "pinjected-0.2.73.tar", max compression
```

## Comparing `pinjected-0.2.72.tar` & `pinjected-0.2.73.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.72/LICENSE
--rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.72/pinjected/__init__.py
--rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.72/pinjected/__main__.py
--rw-r--r--   0        0        0        0 2024-05-21 04:05:50.568481 pinjected-0.2.72/pinjected/common/__init__.py
--rw-r--r--   0        0        0        3 2024-05-21 04:18:58.523298 pinjected-0.2.72/pinjected/common/callbacks.py
--rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.72/pinjected/compatibility/__init__.py
--rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.72/pinjected/compatibility/task_group.py
--rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.72/pinjected/decoration.py
--rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.72/pinjected/demo.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.72/pinjected/di/__init__.py
--rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.72/pinjected/di/app_designed.py
--rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.72/pinjected/di/app_injected.py
--rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.72/pinjected/di/applicative.py
--rw-r--r--   0        0        0     7958 2024-05-16 04:59:01.249430 pinjected-0.2.72/pinjected/di/ast.py
--rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.72/pinjected/di/async_injected.py
--rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.72/pinjected/di/bindings.py
--rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.72/pinjected/di/decorators.py
--rw-r--r--   0        0        0    14720 2024-05-22 03:45:59.797079 pinjected-0.2.72/pinjected/di/design.py
--rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.72/pinjected/di/design_bind_contextx.py
--rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.72/pinjected/di/designed.py
--rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.72/pinjected/di/dynamic_proxy.py
--rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.72/pinjected/di/graph.py
--rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.72/pinjected/di/implicit_globals.py
--rw-r--r--   0        0        0    56168 2024-05-15 06:42:25.667673 pinjected-0.2.72/pinjected/di/injected.py
--rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.72/pinjected/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.72/pinjected/di/metadata/__init__.py
--rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.72/pinjected/di/metadata/bind_metadata.py
--rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.72/pinjected/di/metadata/location_data.py
--rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.72/pinjected/di/modular_injected.py
--rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.72/pinjected/di/monadic.py
--rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.72/pinjected/di/overload_experimental.py
--rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.72/pinjected/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.72/pinjected/di/provider.py
--rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.72/pinjected/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.72/pinjected/di/session.py
--rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.72/pinjected/di/sessioned.py
--rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.72/pinjected/di/static_proxy.py
--rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.72/pinjected/di/test_ast.py
--rw-r--r--   0        0        0     1051 2024-05-21 04:20:44.424963 pinjected-0.2.72/pinjected/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1632 2024-05-21 04:31:46.228251 pinjected-0.2.72/pinjected/di/test_graph.py
--rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.72/pinjected/di/test_injected.py
--rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.72/pinjected/di/test_proxiable.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.72/pinjected/di/tools/__init__.py
--rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.72/pinjected/di/tools/add_overload.py
--rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.72/pinjected/di/util.py
--rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.72/pinjected/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.72/pinjected/exporter/__init__.py
--rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.72/pinjected/exporter/llm_export_v2.py
--rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.72/pinjected/exporter/llm_exporter.py
--rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.72/pinjected/exporter/optimize_import_stmts.py
--rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.72/pinjected/global_configs.py
--rw-r--r--   0        0        0     3126 2024-05-20 09:02:27.376887 pinjected-0.2.72/pinjected/graph_inspection.py
--rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.72/pinjected/helper_structure.py
--rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.72/pinjected/helpers.py
--rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.72/pinjected/ide_supports/__init__.py
--rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.72/pinjected/ide_supports/console_run_helper.py
--rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.72/pinjected/ide_supports/create_configs.py
--rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.72/pinjected/ide_supports/default_design.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.72/pinjected/llm_support/__init__.py
--rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.72/pinjected/llm_support/inspect_module.py
--rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.72/pinjected/llm_support/inspect_module_prompts.py
--rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.72/pinjected/logging_helper.py
--rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.72/pinjected/main_impl.py
--rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.72/pinjected/maybe_patch.py
--rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.72/pinjected/meta_main.py
--rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.72/pinjected/module_helper.py
--rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.72/pinjected/module_inspector.py
--rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.72/pinjected/module_var_path.py
--rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.72/pinjected/notification.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.72/pinjected/nx_graph_util.py
--rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.72/pinjected/providable.py
--rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.72/pinjected/run_config_utils.py
--rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.72/pinjected/run_config_utils_v2.py
--rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.72/pinjected/run_helpers/__init__.py
--rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.72/pinjected/run_helpers/config.py
--rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.72/pinjected/run_helpers/pinjected_environments.py
--rw-r--r--   0        0        0     9492 2024-05-22 03:45:59.774901 pinjected-0.2.72/pinjected/run_helpers/run_injected.py
--rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.72/pinjected/runnables.py
--rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.72/pinjected/test_package/__init__.py
--rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.72/pinjected/test_package/child/__init__.py
--rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.72/pinjected/test_package/child/module1.py
--rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.72/pinjected/test_package/child/module_with.py
--rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.72/pinjected/v2/__init__.py
--rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.72/pinjected/v2/ainjected.py
--rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.72/pinjected/v2/binds.py
--rw-r--r--   0        0        0      132 2024-05-21 04:19:54.467096 pinjected-0.2.72/pinjected/v2/callback.py
--rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.72/pinjected/v2/di.py
--rw-r--r--   0        0        0      796 2024-05-21 04:19:54.473975 pinjected-0.2.72/pinjected/v2/events.py
--rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.72/pinjected/v2/keys.py
--rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.72/pinjected/v2/provide_context.py
--rw-r--r--   0        0        0    25050 2024-05-21 04:33:02.098641 pinjected-0.2.72/pinjected/v2/resolver.py
--rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.72/pinjected/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.72/pinjected/viz/__init__.py
--rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.72/pinjected/viz/graph.py
--rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.72/pinjected/with_context.py
--rw-r--r--   0        0        0      627 2024-05-22 03:46:01.588153 pinjected-0.2.72/pyproject.toml
--rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.72/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinjected-0.2.73/LICENSE
+-rw-r--r--   0        0        0      489 2024-05-01 08:00:14.716375 pinjected-0.2.73/pinjected/__init__.py
+-rw-r--r--   0        0        0       76 2024-03-26 02:52:38.833691 pinjected-0.2.73/pinjected/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:05:50.568481 pinjected-0.2.73/pinjected/common/__init__.py
+-rw-r--r--   0        0        0        3 2024-05-21 04:18:58.523298 pinjected-0.2.73/pinjected/common/callbacks.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:51:53.980366 pinjected-0.2.73/pinjected/compatibility/__init__.py
+-rw-r--r--   0        0        0      753 2024-05-14 16:55:01.337952 pinjected-0.2.73/pinjected/compatibility/task_group.py
+-rw-r--r--   0        0        0      994 2024-04-16 04:30:55.994066 pinjected-0.2.73/pinjected/decoration.py
+-rw-r--r--   0        0        0      977 2023-08-29 05:38:30.733896 pinjected-0.2.73/pinjected/demo.py
+-rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinjected-0.2.73/pinjected/di/__init__.py
+-rw-r--r--   0        0        0     1767 2023-08-01 10:55:32.726526 pinjected-0.2.73/pinjected/di/app_designed.py
+-rw-r--r--   0        0        0     5898 2024-05-13 08:52:30.783178 pinjected-0.2.73/pinjected/di/app_injected.py
+-rw-r--r--   0        0        0      967 2024-03-26 02:52:38.835800 pinjected-0.2.73/pinjected/di/applicative.py
+-rw-r--r--   0        0        0     7958 2024-05-16 04:59:01.249430 pinjected-0.2.73/pinjected/di/ast.py
+-rw-r--r--   0        0        0        2 2024-03-26 02:52:38.837156 pinjected-0.2.73/pinjected/di/async_injected.py
+-rw-r--r--   0        0        0       63 2024-03-26 02:52:38.837781 pinjected-0.2.73/pinjected/di/bindings.py
+-rw-r--r--   0        0        0     9753 2024-05-14 11:27:40.261061 pinjected-0.2.73/pinjected/di/decorators.py
+-rw-r--r--   0        0        0    14714 2024-05-22 03:48:51.014828 pinjected-0.2.73/pinjected/di/design.py
+-rw-r--r--   0        0        0        3 2023-10-16 08:41:10.564875 pinjected-0.2.73/pinjected/di/design_bind_contextx.py
+-rw-r--r--   0        0        0     2095 2024-01-10 03:58:40.482782 pinjected-0.2.73/pinjected/di/designed.py
+-rw-r--r--   0        0        0     1336 2023-08-01 10:55:32.716283 pinjected-0.2.73/pinjected/di/dynamic_proxy.py
+-rw-r--r--   0        0        0    32390 2024-03-26 02:52:38.840785 pinjected-0.2.73/pinjected/di/graph.py
+-rw-r--r--   0        0        0      127 2024-03-26 02:52:38.841437 pinjected-0.2.73/pinjected/di/implicit_globals.py
+-rw-r--r--   0        0        0    56168 2024-05-15 06:42:25.667673 pinjected-0.2.73/pinjected/di/injected.py
+-rw-r--r--   0        0        0     2988 2024-05-14 06:50:46.840175 pinjected-0.2.73/pinjected/di/injected_analysis.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.566458 pinjected-0.2.73/pinjected/di/metadata/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-26 02:52:38.842716 pinjected-0.2.73/pinjected/di/metadata/bind_metadata.py
+-rw-r--r--   0        0        0      490 2023-10-16 08:41:10.566962 pinjected-0.2.73/pinjected/di/metadata/location_data.py
+-rw-r--r--   0        0        0     2948 2023-10-16 08:41:10.568227 pinjected-0.2.73/pinjected/di/modular_injected.py
+-rw-r--r--   0        0        0       91 2023-10-16 08:41:10.568506 pinjected-0.2.73/pinjected/di/monadic.py
+-rw-r--r--   0        0        0     1082 2023-11-02 05:16:21.799077 pinjected-0.2.73/pinjected/di/overload_experimental.py
+-rw-r--r--   0        0        0      142 2023-08-01 10:55:32.740625 pinjected-0.2.73/pinjected/di/playground.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinjected-0.2.73/pinjected/di/provider.py
+-rw-r--r--   0        0        0     2572 2024-03-26 02:52:38.843165 pinjected-0.2.73/pinjected/di/proxiable.py
+-rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinjected-0.2.73/pinjected/di/session.py
+-rw-r--r--   0        0        0     2039 2023-08-01 10:55:32.746751 pinjected-0.2.73/pinjected/di/sessioned.py
+-rw-r--r--   0        0        0     6484 2024-03-26 02:52:38.843741 pinjected-0.2.73/pinjected/di/static_proxy.py
+-rw-r--r--   0        0        0      146 2023-08-01 10:55:32.717766 pinjected-0.2.73/pinjected/di/test_ast.py
+-rw-r--r--   0        0        0     1051 2024-05-21 04:20:44.424963 pinjected-0.2.73/pinjected/di/test_dynamic_proxy.py
+-rw-r--r--   0        0        0     1632 2024-05-21 04:31:46.228251 pinjected-0.2.73/pinjected/di/test_graph.py
+-rw-r--r--   0        0        0     2277 2024-03-26 02:52:38.844637 pinjected-0.2.73/pinjected/di/test_injected.py
+-rw-r--r--   0        0        0      452 2024-05-14 10:11:59.767149 pinjected-0.2.73/pinjected/di/test_proxiable.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.845134 pinjected-0.2.73/pinjected/di/tools/__init__.py
+-rw-r--r--   0        0        0     6109 2024-03-26 02:52:38.845558 pinjected-0.2.73/pinjected/di/tools/add_overload.py
+-rw-r--r--   0        0        0    15534 2024-05-05 06:03:05.073926 pinjected-0.2.73/pinjected/di/util.py
+-rw-r--r--   0        0        0     1290 2024-05-10 07:03:44.040855 pinjected-0.2.73/pinjected/exceptions.py
+-rw-r--r--   0        0        0        0 2024-03-26 02:52:38.846334 pinjected-0.2.73/pinjected/exporter/__init__.py
+-rw-r--r--   0        0        0      409 2024-04-16 06:03:24.715733 pinjected-0.2.73/pinjected/exporter/llm_export_v2.py
+-rw-r--r--   0        0        0    31460 2024-05-05 06:25:12.638593 pinjected-0.2.73/pinjected/exporter/llm_exporter.py
+-rw-r--r--   0        0        0     2216 2024-04-16 09:23:13.383068 pinjected-0.2.73/pinjected/exporter/optimize_import_stmts.py
+-rw-r--r--   0        0        0       30 2023-08-01 10:58:43.083092 pinjected-0.2.73/pinjected/global_configs.py
+-rw-r--r--   0        0        0     3126 2024-05-20 09:02:27.376887 pinjected-0.2.73/pinjected/graph_inspection.py
+-rw-r--r--   0        0        0     3763 2024-04-16 12:18:24.324205 pinjected-0.2.73/pinjected/helper_structure.py
+-rw-r--r--   0        0        0     3585 2023-10-16 08:41:10.571442 pinjected-0.2.73/pinjected/helpers.py
+-rw-r--r--   0        0        0        0 2023-09-01 04:31:07.870037 pinjected-0.2.73/pinjected/ide_supports/__init__.py
+-rw-r--r--   0        0        0     8598 2024-04-23 08:38:19.296844 pinjected-0.2.73/pinjected/ide_supports/console_run_helper.py
+-rw-r--r--   0        0        0     7360 2024-04-23 12:26:40.452081 pinjected-0.2.73/pinjected/ide_supports/create_configs.py
+-rw-r--r--   0        0        0     1304 2024-04-16 09:21:04.827442 pinjected-0.2.73/pinjected/ide_supports/default_design.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.572016 pinjected-0.2.73/pinjected/llm_support/__init__.py
+-rw-r--r--   0        0        0     1818 2023-10-16 08:41:10.572364 pinjected-0.2.73/pinjected/llm_support/inspect_module.py
+-rw-r--r--   0        0        0      702 2023-10-16 08:41:10.572716 pinjected-0.2.73/pinjected/llm_support/inspect_module_prompts.py
+-rw-r--r--   0        0        0      449 2023-08-31 03:46:00.516287 pinjected-0.2.73/pinjected/logging_helper.py
+-rw-r--r--   0        0        0     4279 2024-04-23 08:38:19.298255 pinjected-0.2.73/pinjected/main_impl.py
+-rw-r--r--   0        0        0      554 2023-09-01 04:31:07.870989 pinjected-0.2.73/pinjected/maybe_patch.py
+-rw-r--r--   0        0        0      324 2023-09-01 04:31:07.871211 pinjected-0.2.73/pinjected/meta_main.py
+-rw-r--r--   0        0        0     2501 2024-01-10 03:58:40.485483 pinjected-0.2.73/pinjected/module_helper.py
+-rw-r--r--   0        0        0     2453 2024-04-15 03:39:25.763167 pinjected-0.2.73/pinjected/module_inspector.py
+-rw-r--r--   0        0        0     4875 2024-04-23 08:38:19.299043 pinjected-0.2.73/pinjected/module_var_path.py
+-rw-r--r--   0        0        0      573 2024-01-29 15:55:46.346639 pinjected-0.2.73/pinjected/notification.py
+-rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinjected-0.2.73/pinjected/nx_graph_util.py
+-rw-r--r--   0        0        0      322 2024-02-19 03:58:15.714818 pinjected-0.2.73/pinjected/providable.py
+-rw-r--r--   0        0        0    21356 2024-04-23 08:38:19.299441 pinjected-0.2.73/pinjected/run_config_utils.py
+-rw-r--r--   0        0        0     1617 2023-10-16 08:41:10.573926 pinjected-0.2.73/pinjected/run_config_utils_v2.py
+-rw-r--r--   0        0        0        0 2023-08-31 03:41:38.403233 pinjected-0.2.73/pinjected/run_helpers/__init__.py
+-rw-r--r--   0        0        0     1724 2023-09-01 04:31:07.872367 pinjected-0.2.73/pinjected/run_helpers/config.py
+-rw-r--r--   0        0        0        3 2024-01-10 03:58:40.486377 pinjected-0.2.73/pinjected/run_helpers/pinjected_environments.py
+-rw-r--r--   0        0        0     9492 2024-05-22 03:45:59.774901 pinjected-0.2.73/pinjected/run_helpers/run_injected.py
+-rw-r--r--   0        0        0     1713 2023-10-16 08:41:10.574625 pinjected-0.2.73/pinjected/runnables.py
+-rw-r--r--   0        0        0      934 2023-09-01 04:31:07.873382 pinjected-0.2.73/pinjected/test_package/__init__.py
+-rw-r--r--   0        0        0      214 2023-08-01 10:55:32.738699 pinjected-0.2.73/pinjected/test_package/child/__init__.py
+-rw-r--r--   0        0        0      678 2024-03-29 04:52:43.844255 pinjected-0.2.73/pinjected/test_package/child/module1.py
+-rw-r--r--   0        0        0      356 2024-04-23 08:38:19.300152 pinjected-0.2.73/pinjected/test_package/child/module_with.py
+-rw-r--r--   0        0        0        0 2023-10-16 08:41:10.575198 pinjected-0.2.73/pinjected/v2/__init__.py
+-rw-r--r--   0        0        0     2774 2024-03-26 02:52:38.850100 pinjected-0.2.73/pinjected/v2/ainjected.py
+-rw-r--r--   0        0        0     7032 2024-05-05 05:55:33.403415 pinjected-0.2.73/pinjected/v2/binds.py
+-rw-r--r--   0        0        0      132 2024-05-21 04:19:54.467096 pinjected-0.2.73/pinjected/v2/callback.py
+-rw-r--r--   0        0        0     3140 2024-03-26 02:52:38.851127 pinjected-0.2.73/pinjected/v2/di.py
+-rw-r--r--   0        0        0      796 2024-05-21 04:19:54.473975 pinjected-0.2.73/pinjected/v2/events.py
+-rw-r--r--   0        0        0      616 2024-05-15 04:08:13.929515 pinjected-0.2.73/pinjected/v2/keys.py
+-rw-r--r--   0        0        0      627 2024-05-10 02:30:28.919876 pinjected-0.2.73/pinjected/v2/provide_context.py
+-rw-r--r--   0        0        0    25050 2024-05-21 04:33:02.098641 pinjected-0.2.73/pinjected/v2/resolver.py
+-rw-r--r--   0        0        0    20026 2024-05-14 08:55:44.478760 pinjected-0.2.73/pinjected/visualize_di.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinjected-0.2.73/pinjected/viz/__init__.py
+-rw-r--r--   0        0        0       65 2023-10-16 08:41:10.576904 pinjected-0.2.73/pinjected/viz/graph.py
+-rw-r--r--   0        0        0       74 2024-03-26 02:52:38.853414 pinjected-0.2.73/pinjected/with_context.py
+-rw-r--r--   0        0        0      627 2024-05-22 03:48:52.414366 pinjected-0.2.73/pyproject.toml
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 pinjected-0.2.73/PKG-INFO
```

### Comparing `pinjected-0.2.72/LICENSE` & `pinjected-0.2.73/LICENSE`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/compatibility/task_group.py` & `pinjected-0.2.73/pinjected/compatibility/task_group.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/decoration.py` & `pinjected-0.2.73/pinjected/decoration.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/demo.py` & `pinjected-0.2.73/pinjected/demo.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/app_designed.py` & `pinjected-0.2.73/pinjected/di/app_designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/app_injected.py` & `pinjected-0.2.73/pinjected/di/app_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/applicative.py` & `pinjected-0.2.73/pinjected/di/applicative.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/ast.py` & `pinjected-0.2.73/pinjected/di/ast.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/decorators.py` & `pinjected-0.2.73/pinjected/di/decorators.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/design.py` & `pinjected-0.2.73/pinjected/di/design.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,17 +218,15 @@
         from pinjected.v2.resolver import AsyncResolver,BaseResolverCallback
         bindings = {**IMPLICIT_BINDINGS, **self.bindings}
         if callback is None:
             callback = BaseResolverCallback()
         assert isinstance(callback, IResolverCallback)
         return AsyncResolver(
             Design(bindings=bindings, modules=self.modules),
-            callbacks=[
-
-            ]
+            callbacks=[callback]
         )
 
     def to_graph(self):
         return self.to_resolver().to_blocking()
 
     def run(self, f, modules=None):
         return self.to_graph(modules).run(f)
```

### Comparing `pinjected-0.2.72/pinjected/di/designed.py` & `pinjected-0.2.73/pinjected/di/designed.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/dynamic_proxy.py` & `pinjected-0.2.73/pinjected/di/dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/graph.py` & `pinjected-0.2.73/pinjected/di/graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/injected.py` & `pinjected-0.2.73/pinjected/di/injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/injected_analysis.py` & `pinjected-0.2.73/pinjected/di/injected_analysis.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/modular_injected.py` & `pinjected-0.2.73/pinjected/di/modular_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/overload_experimental.py` & `pinjected-0.2.73/pinjected/di/overload_experimental.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/proxiable.py` & `pinjected-0.2.73/pinjected/di/proxiable.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/session.py` & `pinjected-0.2.73/pinjected/di/session.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/sessioned.py` & `pinjected-0.2.73/pinjected/di/sessioned.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/static_proxy.py` & `pinjected-0.2.73/pinjected/di/static_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/test_dynamic_proxy.py` & `pinjected-0.2.73/pinjected/di/test_dynamic_proxy.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/test_graph.py` & `pinjected-0.2.73/pinjected/di/test_graph.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/test_injected.py` & `pinjected-0.2.73/pinjected/di/test_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/tools/add_overload.py` & `pinjected-0.2.73/pinjected/di/tools/add_overload.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/di/util.py` & `pinjected-0.2.73/pinjected/di/util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/exceptions.py` & `pinjected-0.2.73/pinjected/exceptions.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/exporter/llm_exporter.py` & `pinjected-0.2.73/pinjected/exporter/llm_exporter.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/exporter/optimize_import_stmts.py` & `pinjected-0.2.73/pinjected/exporter/optimize_import_stmts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/graph_inspection.py` & `pinjected-0.2.73/pinjected/graph_inspection.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/helper_structure.py` & `pinjected-0.2.73/pinjected/helper_structure.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/helpers.py` & `pinjected-0.2.73/pinjected/helpers.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/ide_supports/console_run_helper.py` & `pinjected-0.2.73/pinjected/ide_supports/console_run_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/ide_supports/create_configs.py` & `pinjected-0.2.73/pinjected/ide_supports/create_configs.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/ide_supports/default_design.py` & `pinjected-0.2.73/pinjected/ide_supports/default_design.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/llm_support/inspect_module.py` & `pinjected-0.2.73/pinjected/llm_support/inspect_module.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/llm_support/inspect_module_prompts.py` & `pinjected-0.2.73/pinjected/llm_support/inspect_module_prompts.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/main_impl.py` & `pinjected-0.2.73/pinjected/main_impl.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/maybe_patch.py` & `pinjected-0.2.73/pinjected/maybe_patch.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/module_helper.py` & `pinjected-0.2.73/pinjected/module_helper.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/module_inspector.py` & `pinjected-0.2.73/pinjected/module_inspector.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/module_var_path.py` & `pinjected-0.2.73/pinjected/module_var_path.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/notification.py` & `pinjected-0.2.73/pinjected/notification.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/nx_graph_util.py` & `pinjected-0.2.73/pinjected/nx_graph_util.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/run_config_utils.py` & `pinjected-0.2.73/pinjected/run_config_utils.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/run_config_utils_v2.py` & `pinjected-0.2.73/pinjected/run_config_utils_v2.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/run_helpers/config.py` & `pinjected-0.2.73/pinjected/run_helpers/config.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/run_helpers/run_injected.py` & `pinjected-0.2.73/pinjected/run_helpers/run_injected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/runnables.py` & `pinjected-0.2.73/pinjected/runnables.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/test_package/__init__.py` & `pinjected-0.2.73/pinjected/test_package/__init__.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/test_package/child/module1.py` & `pinjected-0.2.73/pinjected/test_package/child/module1.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/ainjected.py` & `pinjected-0.2.73/pinjected/v2/ainjected.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/binds.py` & `pinjected-0.2.73/pinjected/v2/binds.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/di.py` & `pinjected-0.2.73/pinjected/v2/di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/events.py` & `pinjected-0.2.73/pinjected/v2/events.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/keys.py` & `pinjected-0.2.73/pinjected/v2/keys.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/provide_context.py` & `pinjected-0.2.73/pinjected/v2/provide_context.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/v2/resolver.py` & `pinjected-0.2.73/pinjected/v2/resolver.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pinjected/visualize_di.py` & `pinjected-0.2.73/pinjected/visualize_di.py`

 * *Files identical despite different names*

### Comparing `pinjected-0.2.72/pyproject.toml` & `pinjected-0.2.73/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pinjected"
-version = "0.2.72"
+version = "0.2.73"
 description = "Immutable Dependency Injection for Python."
 authors = [ "proboscis <nameissoap@gmail.com>",]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 returns = "*"
```

### Comparing `pinjected-0.2.72/PKG-INFO` & `pinjected-0.2.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pinjected
-Version: 0.2.72
+Version: 0.2.73
 Summary: Immutable Dependency Injection for Python.
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

