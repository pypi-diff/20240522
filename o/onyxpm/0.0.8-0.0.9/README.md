# Comparing `tmp/onyxpm-0.0.8.tar.gz` & `tmp/onyxpm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onyxpm-0.0.8.tar", max compression
+gzip compressed data, was "onyxpm-0.0.9.tar", max compression
```

## Comparing `onyxpm-0.0.8.tar` & `onyxpm-0.0.9.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      756 2024-05-14 13:42:08.395457 onyxpm-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6541 2024-05-14 11:23:59.653406 onyxpm-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-04-11 09:10:15.831533 onyxpm-0.0.8/src/onyxpm/__init__.py
--rw-r--r--   0        0        0      221 2024-04-11 09:10:15.787854 onyxpm-0.0.8/src/onyxpm/CLASSES/__init__.py
--rw-r--r--   0        0        0      168 2024-04-11 09:10:15.783852 onyxpm-0.0.8/src/onyxpm/CLASSES/EnvConfElement.py
--rw-r--r--   0        0        0      378 2024-04-11 09:10:15.784850 onyxpm-0.0.8/src/onyxpm/CLASSES/NxComponant.py
--rw-r--r--   0        0        0      217 2024-04-11 09:10:15.784850 onyxpm-0.0.8/src/onyxpm/CLASSES/NxComponantAttributes.py
--rw-r--r--   0        0        0    70173 2024-04-11 09:10:15.786849 onyxpm-0.0.8/src/onyxpm/CLASSES/NxOnyxApi.py
--rw-r--r--   0        0        0      226 2024-04-11 09:10:15.786849 onyxpm-0.0.8/src/onyxpm/CLASSES/NxProject.py
--rw-r--r--   0        0        0      266 2024-04-11 09:10:15.787854 onyxpm-0.0.8/src/onyxpm/CLASSES/NxTenant.py
--rw-r--r--   0        0        0      384 2024-04-11 09:10:15.787854 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/__init__.py
--rw-r--r--   0        0        0      235 2024-04-11 09:10:15.789416 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/apply_transco.py
--rw-r--r--   0        0        0     5253 2024-04-11 09:10:15.790374 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/compare_onyx_projects.py
--rw-r--r--   0        0        0      475 2024-04-11 09:10:15.790883 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/find_onyx_project.py
--rw-r--r--   0        0        0       29 2024-04-11 09:10:15.790883 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/load_env.py
--rw-r--r--   0        0        0     9087 2024-04-11 09:10:15.791894 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/read_onyx_project_api.py
--rw-r--r--   0        0        0     1426 2024-04-11 09:10:15.792903 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/read_onyx_project_package.py
--rw-r--r--   0        0        0     1321 2024-04-11 09:10:15.792903 onyxpm-0.0.8/src/onyxpm/LIBS_BUS/write_to_disk_onyx_project.py
--rw-r--r--   0        0        0     2331 2024-04-11 09:10:15.794896 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/__init__.py
--rw-r--r--   0        0        0     2528 2024-05-14 13:47:19.364534 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_1.py
--rw-r--r--   0        0        0     1934 2024-04-11 09:10:15.795895 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_2.py
--rw-r--r--   0        0        0     3811 2024-04-11 09:10:15.796895 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_3.py
--rw-r--r--   0        0        0     1342 2024-04-11 09:10:15.796895 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_4.py
--rw-r--r--   0        0        0      566 2024-04-11 09:10:15.797893 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_5.py
--rw-r--r--   0        0        0      695 2024-04-11 09:10:15.798892 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_package.py
--rw-r--r--   0        0        0     1158 2024-04-11 09:10:15.798892 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_project.py
--rw-r--r--   0        0        0     2341 2024-04-11 09:10:15.800402 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_tenant.py
--rw-r--r--   0        0        0      948 2024-04-11 09:10:15.801411 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/check_project_existence.py
--rw-r--r--   0        0        0      588 2024-04-11 09:10:15.801411 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/clear_screen.py
--rw-r--r--   0        0        0     4510 2024-04-11 09:10:15.802413 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_add_to_workflow.py
--rw-r--r--   0        0        0      231 2024-04-11 09:10:15.802413 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_connect_api.py
--rw-r--r--   0        0        0      451 2024-04-11 09:10:15.803420 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_create_tenant.py
--rw-r--r--   0        0        0     4400 2024-04-11 09:10:15.803420 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_connection.py
--rw-r--r--   0        0        0     1312 2024-04-11 09:10:15.804422 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_id.py
--rw-r--r--   0        0        0     2322 2024-04-11 09:10:15.805420 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_info.py
--rw-r--r--   0        0        0      617 2024-04-11 09:10:15.805420 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_organisation_unit.py
--rw-r--r--   0        0        0      709 2024-04-11 09:10:15.806422 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_tenant_validation.py
--rw-r--r--   0        0        0    13766 2024-04-11 09:10:15.807422 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/creer_arborescence.py
--rw-r--r--   0        0        0     1562 2024-04-11 09:10:15.808421 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oConnections.py
--rw-r--r--   0        0        0     3829 2024-04-11 09:10:15.809421 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oDataPipelines.py
--rw-r--r--   0        0        0     1552 2024-04-11 09:10:15.810420 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oFileProviders.py
--rw-r--r--   0        0        0     3516 2024-04-11 09:10:15.810928 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oForms.py
--rw-r--r--   0        0        0     1354 2024-04-11 09:10:15.811939 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oNotifications.py
--rw-r--r--   0        0        0     1579 2024-04-11 09:10:15.811939 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oPipelineColumns.py
--rw-r--r--   0        0        0     3253 2024-04-11 09:10:15.812937 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oReports.py
--rw-r--r--   0        0        0     1283 2024-04-11 09:10:15.812937 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oShellScripts.py
--rw-r--r--   0        0        0     1761 2024-04-11 09:10:15.813945 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oSqlScripts.py
--rw-r--r--   0        0        0     2369 2024-04-11 09:10:15.815945 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oVariables.py
--rw-r--r--   0        0        0     3090 2024-04-11 09:10:15.816945 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgetButton.py
--rw-r--r--   0        0        0     2253 2024-04-11 09:10:15.817946 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgetFilter.py
--rw-r--r--   0        0        0     4718 2024-04-11 09:10:15.817946 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgets.py
--rw-r--r--   0        0        0     3046 2024-04-11 09:10:15.818947 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWorkFlows.py
--rw-r--r--   0        0        0      129 2024-04-11 09:10:15.818947 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWorkFlowStep.py
--rw-r--r--   0        0        0      276 2024-04-11 09:10:15.820456 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/display_env.py
--rw-r--r--   0        0        0      402 2024-04-12 07:43:46.499044 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/exist_envconf.py
--rw-r--r--   0        0        0      204 2024-04-11 09:10:15.821464 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/exist_tenantName.py
--rw-r--r--   0        0        0       38 2024-04-11 09:10:15.822472 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/get_connection_name.py
--rw-r--r--   0        0        0      113 2024-04-12 07:43:46.483139 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/get_envconf.py
--rw-r--r--   0        0        0      787 2024-04-12 07:43:46.477927 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/get_tenantname.py
--rw-r--r--   0        0        0      331 2024-04-11 09:10:15.825491 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/init_envconf.py
--rw-r--r--   0        0        0      949 2024-04-11 09:10:15.826487 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/list_project.py
--rw-r--r--   0        0        0       93 2024-04-11 09:10:15.826487 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/load_envconf.py
--rw-r--r--   0        0        0      305 2024-04-11 09:10:15.827485 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/on_rm_error.py
--rw-r--r--   0        0        0      206 2024-04-11 09:10:15.827485 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/parameter_selector.py
--rw-r--r--   0        0        0      132 2024-04-11 09:10:15.827485 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/print_console.py
--rw-r--r--   0        0        0      128 2024-04-11 09:10:15.828485 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/print_menu.py
--rw-r--r--   0        0        0      334 2024-04-11 09:10:15.829489 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/refactor_dict.py
--rw-r--r--   0        0        0     1155 2024-04-11 09:10:15.830484 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/transco_id.py
--rw-r--r--   0        0        0      223 2024-04-11 09:10:15.830484 onyxpm-0.0.8/src/onyxpm/LIBS_CLI/update_envconf.py
--rw-r--r--   0        0        0     5669 2024-05-14 08:38:33.959405 onyxpm-0.0.8/src/onyxpm/onyxpm.py
--rw-r--r--   0        0        0     7458 1970-01-01 00:00:00.000000 onyxpm-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      756 2024-05-14 13:50:04.147329 onyxpm-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6541 2024-05-14 13:50:04.142745 onyxpm-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-11 09:10:15.831533 onyxpm-0.0.9/src/onyxpm/__init__.py
+-rw-r--r--   0        0        0      221 2024-04-11 09:10:15.787854 onyxpm-0.0.9/src/onyxpm/CLASSES/__init__.py
+-rw-r--r--   0        0        0      168 2024-04-11 09:10:15.783852 onyxpm-0.0.9/src/onyxpm/CLASSES/EnvConfElement.py
+-rw-r--r--   0        0        0      378 2024-04-11 09:10:15.784850 onyxpm-0.0.9/src/onyxpm/CLASSES/NxComponant.py
+-rw-r--r--   0        0        0      217 2024-04-11 09:10:15.784850 onyxpm-0.0.9/src/onyxpm/CLASSES/NxComponantAttributes.py
+-rw-r--r--   0        0        0    70173 2024-04-11 09:10:15.786849 onyxpm-0.0.9/src/onyxpm/CLASSES/NxOnyxApi.py
+-rw-r--r--   0        0        0      226 2024-04-11 09:10:15.786849 onyxpm-0.0.9/src/onyxpm/CLASSES/NxProject.py
+-rw-r--r--   0        0        0      266 2024-04-11 09:10:15.787854 onyxpm-0.0.9/src/onyxpm/CLASSES/NxTenant.py
+-rw-r--r--   0        0        0      384 2024-04-11 09:10:15.787854 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/__init__.py
+-rw-r--r--   0        0        0      235 2024-04-11 09:10:15.789416 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/apply_transco.py
+-rw-r--r--   0        0        0     5253 2024-04-11 09:10:15.790374 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/compare_onyx_projects.py
+-rw-r--r--   0        0        0      475 2024-04-11 09:10:15.790883 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/find_onyx_project.py
+-rw-r--r--   0        0        0       29 2024-04-11 09:10:15.790883 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/load_env.py
+-rw-r--r--   0        0        0     9087 2024-04-11 09:10:15.791894 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/read_onyx_project_api.py
+-rw-r--r--   0        0        0     1426 2024-04-11 09:10:15.792903 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/read_onyx_project_package.py
+-rw-r--r--   0        0        0     1321 2024-04-11 09:10:15.792903 onyxpm-0.0.9/src/onyxpm/LIBS_BUS/write_to_disk_onyx_project.py
+-rw-r--r--   0        0        0     2331 2024-04-11 09:10:15.794896 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/__init__.py
+-rw-r--r--   0        0        0     2520 2024-05-14 13:49:22.137028 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_1.py
+-rw-r--r--   0        0        0     1934 2024-04-11 09:10:15.795895 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_2.py
+-rw-r--r--   0        0        0     3811 2024-04-11 09:10:15.796895 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_3.py
+-rw-r--r--   0        0        0     1342 2024-04-11 09:10:15.796895 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_4.py
+-rw-r--r--   0        0        0      566 2024-04-11 09:10:15.797893 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_5.py
+-rw-r--r--   0        0        0      695 2024-04-11 09:10:15.798892 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_package.py
+-rw-r--r--   0        0        0     1158 2024-04-11 09:10:15.798892 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_project.py
+-rw-r--r--   0        0        0     2341 2024-04-11 09:10:15.800402 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_tenant.py
+-rw-r--r--   0        0        0      948 2024-04-11 09:10:15.801411 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/check_project_existence.py
+-rw-r--r--   0        0        0      588 2024-04-11 09:10:15.801411 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/clear_screen.py
+-rw-r--r--   0        0        0     4510 2024-04-11 09:10:15.802413 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_add_to_workflow.py
+-rw-r--r--   0        0        0      231 2024-04-11 09:10:15.802413 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_connect_api.py
+-rw-r--r--   0        0        0      451 2024-04-11 09:10:15.803420 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_create_tenant.py
+-rw-r--r--   0        0        0     4400 2024-04-11 09:10:15.803420 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_connection.py
+-rw-r--r--   0        0        0     1312 2024-04-11 09:10:15.804422 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_id.py
+-rw-r--r--   0        0        0     2322 2024-04-11 09:10:15.805420 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_info.py
+-rw-r--r--   0        0        0      617 2024-04-11 09:10:15.805420 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_organisation_unit.py
+-rw-r--r--   0        0        0      709 2024-04-11 09:10:15.806422 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_tenant_validation.py
+-rw-r--r--   0        0        0    13766 2024-04-11 09:10:15.807422 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/creer_arborescence.py
+-rw-r--r--   0        0        0     1562 2024-04-11 09:10:15.808421 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oConnections.py
+-rw-r--r--   0        0        0     3829 2024-04-11 09:10:15.809421 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oDataPipelines.py
+-rw-r--r--   0        0        0     1552 2024-04-11 09:10:15.810420 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oFileProviders.py
+-rw-r--r--   0        0        0     3516 2024-04-11 09:10:15.810928 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oForms.py
+-rw-r--r--   0        0        0     1354 2024-04-11 09:10:15.811939 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oNotifications.py
+-rw-r--r--   0        0        0     1579 2024-04-11 09:10:15.811939 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oPipelineColumns.py
+-rw-r--r--   0        0        0     3253 2024-04-11 09:10:15.812937 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oReports.py
+-rw-r--r--   0        0        0     1283 2024-04-11 09:10:15.812937 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oShellScripts.py
+-rw-r--r--   0        0        0     1761 2024-04-11 09:10:15.813945 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oSqlScripts.py
+-rw-r--r--   0        0        0     2369 2024-04-11 09:10:15.815945 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oVariables.py
+-rw-r--r--   0        0        0     3090 2024-04-11 09:10:15.816945 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgetButton.py
+-rw-r--r--   0        0        0     2253 2024-04-11 09:10:15.817946 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgetFilter.py
+-rw-r--r--   0        0        0     4718 2024-04-11 09:10:15.817946 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgets.py
+-rw-r--r--   0        0        0     3046 2024-04-11 09:10:15.818947 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWorkFlows.py
+-rw-r--r--   0        0        0      129 2024-04-11 09:10:15.818947 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWorkFlowStep.py
+-rw-r--r--   0        0        0      276 2024-04-11 09:10:15.820456 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/display_env.py
+-rw-r--r--   0        0        0      402 2024-04-12 07:43:46.499044 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/exist_envconf.py
+-rw-r--r--   0        0        0      204 2024-04-11 09:10:15.821464 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/exist_tenantName.py
+-rw-r--r--   0        0        0       38 2024-04-11 09:10:15.822472 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/get_connection_name.py
+-rw-r--r--   0        0        0      113 2024-04-12 07:43:46.483139 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/get_envconf.py
+-rw-r--r--   0        0        0      787 2024-04-12 07:43:46.477927 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/get_tenantname.py
+-rw-r--r--   0        0        0      331 2024-04-11 09:10:15.825491 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/init_envconf.py
+-rw-r--r--   0        0        0      949 2024-04-11 09:10:15.826487 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/list_project.py
+-rw-r--r--   0        0        0       93 2024-04-11 09:10:15.826487 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/load_envconf.py
+-rw-r--r--   0        0        0      305 2024-04-11 09:10:15.827485 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/on_rm_error.py
+-rw-r--r--   0        0        0      206 2024-04-11 09:10:15.827485 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/parameter_selector.py
+-rw-r--r--   0        0        0      132 2024-04-11 09:10:15.827485 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/print_console.py
+-rw-r--r--   0        0        0      128 2024-04-11 09:10:15.828485 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/print_menu.py
+-rw-r--r--   0        0        0      334 2024-04-11 09:10:15.829489 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/refactor_dict.py
+-rw-r--r--   0        0        0     1155 2024-04-11 09:10:15.830484 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/transco_id.py
+-rw-r--r--   0        0        0      223 2024-04-11 09:10:15.830484 onyxpm-0.0.9/src/onyxpm/LIBS_CLI/update_envconf.py
+-rw-r--r--   0        0        0     5669 2024-05-14 08:38:33.959405 onyxpm-0.0.9/src/onyxpm/onyxpm.py
+-rw-r--r--   0        0        0     7458 1970-01-01 00:00:00.000000 onyxpm-0.0.9/PKG-INFO
```

### Comparing `onyxpm-0.0.8/pyproject.toml` & `onyxpm-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onyxpm"
-version = "0.0.8"
+version = "0.0.9"
 description = "CICD"
 authors = ["Olivier Siguré <olivier.sigure@alchimiedatasolutions.com>","Kasi Gajavalli <kasi.gajavalli@alchimiedatasolutions.com>", "Antoine Ducoulombier <antoine.ducoulombier@alchimiedatasolutions.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `onyxpm-0.0.8/README.md` & `onyxpm-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - [License](#license)
 
 ## Installation
 
 1. Clone the project from Pipy:
 
    ```sh
-   pip install onyxpm==0.0.6 
+   pip install onyxpm==0.0.9 
    ````
 
 ## First Steps After Installation
 
 1. After installing the project, you'll find the installation directory where Onyxpm has been installed. You can identify this directory during the installation process. Make sure to note down this directory.
 
     ```sh
```

### Comparing `onyxpm-0.0.8/src/onyxpm/CLASSES/NxOnyxApi.py` & `onyxpm-0.0.9/src/onyxpm/CLASSES/NxOnyxApi.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_BUS/compare_onyx_projects.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_BUS/compare_onyx_projects.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_BUS/read_onyx_project_api.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_BUS/read_onyx_project_api.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_BUS/read_onyx_project_package.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_BUS/read_onyx_project_package.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_BUS/write_to_disk_onyx_project.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_BUS/write_to_disk_onyx_project.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/__init__.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/__init__.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_1.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_1.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                             tenant_name=dict["TENANTNAME"], username=dict["TENANTUSERNAME"],
                             password=dict["TENANTPASSWORD"])
 
         tenant_dict = NxOnyxApi(tenant_dict.domain, tenant_dict.username, tenant_dict.password, tenant_dict.tenant_id)
         print("Connection to source", dict["TENANTNAME"], "successful.")
 
         conf_file_path = os.path.abspath(os.path.join(os.path.dirname(__file__), "../env.conf"))
-        conf_file_path_relative = shutil.copy(conf_file_path, os.path.join(os.getcwd(), "env.conf"))
+        #conf_file_path = shutil.copy(conf_file_path, os.path.join(os.getcwd(), "env.conf"))
 
         if not os.path.exists(conf_file_path) or os.getenv(dict["TENANT"] + "_TENANTNAME") is None:
             with open(conf_file_path, 'a+') as file:
                 file.write('\n#' + dict["TENANT"].upper() + '\n')
                 for Element in dict:
                     if Element != "TENANT":
                         file.write(dict["TENANT"] + "_" + str(Element) + '=' + str(dict[Element]) + '\n')
```

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_2.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_2.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_3.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_3.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_4.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_4.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/action_5.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/action_5.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_package.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_package.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_project.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_project.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/ask_tenant.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/ask_tenant.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/check_project_existence.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/check_project_existence.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/clear_screen.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/clear_screen.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_add_to_workflow.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_add_to_workflow.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_connection.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_connection.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_id.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_id.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_info.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_info.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_get_organisation_unit.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_get_organisation_unit.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/cli_tenant_validation.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/cli_tenant_validation.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/creer_arborescence.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/creer_arborescence.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oConnections.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oConnections.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oDataPipelines.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oDataPipelines.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oFileProviders.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oFileProviders.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oForms.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oForms.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oNotifications.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oNotifications.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oPipelineColumns.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oPipelineColumns.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oReports.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oReports.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oShellScripts.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oShellScripts.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oSqlScripts.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oSqlScripts.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oVariables.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oVariables.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgetButton.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgetButton.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgetFilter.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgetFilter.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWidgets.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWidgets.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/deploy_oWorkFlows.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/deploy_oWorkFlows.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/get_tenantname.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/get_tenantname.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/list_project.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/list_project.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/LIBS_CLI/transco_id.py` & `onyxpm-0.0.9/src/onyxpm/LIBS_CLI/transco_id.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/src/onyxpm/onyxpm.py` & `onyxpm-0.0.9/src/onyxpm/onyxpm.py`

 * *Files identical despite different names*

### Comparing `onyxpm-0.0.8/PKG-INFO` & `onyxpm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onyxpm
-Version: 0.0.8
+Version: 0.0.9
 Summary: CICD
 License: MIT
 Author: Olivier Siguré
 Author-email: olivier.sigure@alchimiedatasolutions.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 - [License](#license)
 
 ## Installation
 
 1. Clone the project from Pipy:
 
    ```sh
-   pip install onyxpm==0.0.6 
+   pip install onyxpm==0.0.9 
    ````
 
 ## First Steps After Installation
 
 1. After installing the project, you'll find the installation directory where Onyxpm has been installed. You can identify this directory during the installation process. Make sure to note down this directory.
 
     ```sh
```

