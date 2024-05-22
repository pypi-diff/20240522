# Comparing `tmp/youwol-0.1.9rc0.tar.gz` & `tmp/youwol-0.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youwol-0.1.9rc0.tar", last modified: Mon Apr  8 09:00:17 2024, max compression
+gzip compressed data, was "youwol-0.1.9rc1.tar", last modified: Mon Apr 15 10:15:21 2024, max compression
```

## Comparing `youwol-0.1.9rc0.tar` & `youwol-0.1.9rc1.tar`

### file list

```diff
@@ -1,480 +1,480 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.516010 youwol-0.1.9rc0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.528010 youwol-0.1.9rc0/src/youwol/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-08 09:00:11.000000 youwol-0.1.9rc0/src/youwol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.532009 youwol-0.1.9rc0/src/youwol/app/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.532009 youwol-0.1.9rc0/src/youwol/app/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/browser_cache_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/config_from_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/errors_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/local_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/flow_switches.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/model_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    22216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/models_token_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/predefined_configs/default_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/encrypted_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/path_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/native_backends_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/online_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/proxied_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/python_dynamic_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/fastapi_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/main_args.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.536009 youwol-0.1.9rc0/src/youwol/app/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/browser_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/hybridizer_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/backends/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/commons.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.540009 youwol-0.1.9rc0/src/youwol/app/routers/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/auto_download_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/custom_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/flux_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/story.py
--rw-r--r--   0 runner    (1001) docker     (127)   359173 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/fortunes.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    19420 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/custom_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/flux_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/story.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.544009 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/native_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/native_backends_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/projects/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25855 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/models_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/projects/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/python/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/python/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/router_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/app/routers/system/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/documentation_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8666 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/routers/system/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/shut_down.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/web_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/app/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.548009 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/impersonation_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/admin/registration_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/accounts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/routers/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.552009 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/all_icons_emojipedia.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.556009 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/assets_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/cdn_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/files_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/flux_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/stories_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/treedb_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/assets_gateway/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.556009 youwol-0.1.9rc0/src/youwol/backends/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/loading_graph_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    24721 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn/utils_indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/router.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/files/
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/files/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.560009 youwol-0.1.9rc0/src/youwol/backends/flux/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/backward_compatibility.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    22697 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js
--rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/style.29a727c7731e84e314ac.css
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/flux/workflow_new_project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/stories/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    29141 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/root_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/stories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/tree_db/
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/drives.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/items.py
--rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/backends/tree_db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.564009 youwol-0.1.9rc0/src/youwol/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/install.sh
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/__init__.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/dependencies.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/start.sh
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/run.view.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.568009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/auto-generated.ts
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/mock-requests.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.572009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py
--rw-r--r--   0 runner    (1001) docker     (127)    13814 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.npmignore
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.prettierignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/jest.config.ts
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.app.json
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/rx-vdom-config.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.ts
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/main.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/style.css
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/fake.test.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.576009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/index.ts
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/fake.test.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/typedoc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/pipelines/publish_cdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/accounts/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/assets/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.580009 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/assets_gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cache/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cache/redis_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn/cdn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/local_docdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/docdb/patches.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/local_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/file_system/minio_file_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/files/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/files/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.584009 youwol-0.1.9rc0/src/youwol/utils/clients/flux/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/flux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/flux/flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/oidc_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/service_account_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/tokens_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/oidc/users_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/request_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/patches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8499 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/stories/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/stories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/stories/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/clients/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/context/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/context/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.588009 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/computation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/traces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/digest/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/constantes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/file_encryption.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/null.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/siv_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.592009 youwol-0.1.9rc0/src/youwol/utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/middlewares/root_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.528010 youwol-0.1.9rc0/src/youwol/utils/python_next/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/python_next/v3_12/tomllib.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/request_info_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol/utils/servers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/servers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-08 08:59:51.000000 youwol-0.1.9rc0/src/youwol/utils/utils_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:00:17.596009 youwol-0.1.9rc0/src/youwol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20543 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 09:00:17.000000 youwol-0.1.9rc0/src/youwol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.528255 youwol-0.1.9rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-15 10:15:21.528255 youwol-0.1.9rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 10:15:21.528255 youwol-0.1.9rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.448255 youwol-0.1.9rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.460255 youwol-0.1.9rc1/src/youwol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 10:15:16.000000 youwol-0.1.9rc1/src/youwol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.460255 youwol-0.1.9rc1/src/youwol/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.464255 youwol-0.1.9rc1/src/youwol/app/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/browser_cache_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/config_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/errors_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7883 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/local_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.464255 youwol-0.1.9rc1/src/youwol/app/environment/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/flow_switches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/model_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22216 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/models_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7730 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/models_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/models_token_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.464255 youwol-0.1.9rc1/src/youwol/app/environment/models/predefined_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/predefined_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/predefined_configs/default_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.464255 youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/encrypted_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/path_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9595 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/native_backends_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/online_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/proxied_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/python_dynamic_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/youwol_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/environment/youwol_environment_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14633 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/fastapi_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/main_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.468255 youwol-0.1.9rc1/src/youwol/app/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/browser_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/hybridizer_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.468255 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.468255 youwol-0.1.9rc1/src/youwol/app/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.468255 youwol-0.1.9rc1/src/youwol/app/routers/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/backends/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/backends/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/commons.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/custom_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.468255 youwol-0.1.9rc1/src/youwol/app/routers/custom_commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/custom_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/custom_commands/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.472255 youwol-0.1.9rc1/src/youwol/app/routers/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.472255 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/auto_download_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/custom_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/flux_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)   359173 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/fortunes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19420 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.472255 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/custom_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/flux_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/story.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/native_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/native_backends_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/app/routers/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25855 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/models_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/projects_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25723 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/projects/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/app/routers/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16586 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/python/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/router_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/app/routers/system/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/system/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/system/documentation_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8668 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/system/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18752 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/routers/system/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/shut_down.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/web_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/app/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.476255 youwol-0.1.9rc1/src/youwol/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.480255 youwol-0.1.9rc1/src/youwol/backends/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.480255 youwol-0.1.9rc1/src/youwol/backends/accounts/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/admin/impersonation_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/admin/registration_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.480255 youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/openid_flows_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/openid_flows_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10132 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/accounts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.480255 youwol-0.1.9rc1/src/youwol/backends/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.484255 youwol-0.1.9rc1/src/youwol/backends/assets/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7899 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8422 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8725 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/routers/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.484255 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63536 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/all_icons_emojipedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.484255 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/assets_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11505 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/cdn_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6199 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/files_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/flux_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/stories_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27841 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/treedb_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/assets_gateway/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.488255 youwol-0.1.9rc1/src/youwol/backends/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20110 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/loading_graph_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24721 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn/utils_indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.488255 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.488255 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.488255 youwol-0.1.9rc1/src/youwol/backends/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/files/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/files/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/files/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/files/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.492255 youwol-0.1.9rc1/src/youwol/backends/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3315 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/backward_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.492255 youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22697 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14014 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/style.29a727c7731e84e314ac.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21715 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14644 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/flux/workflow_new_project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.492255 youwol-0.1.9rc1/src/youwol/backends/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29141 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/root_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/stories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.492255 youwol-0.1.9rc1/src/youwol/backends/tree_db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/drives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17313 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/backends/tree_db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16208 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/install.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/__init__.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/dependencies.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/start.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/views/run.view.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_raw_app/
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_raw_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_raw_app/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.496255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9533 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10429 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/auto-generated.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.500255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/mock-requests.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.504255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13814 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.504255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.npmignore
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.prettierignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.504255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/jest.config.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.app.json
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/rx-vdom-config.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.504255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.ts
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/main.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/tests/fake.test.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/index.ts
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/tests/fake.test.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/typedoc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22920 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/pipelines/publish_cdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.508255 youwol-0.1.9rc1/src/youwol/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/accounts/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/assets/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/assets_gateway/assets_gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cache/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cache/redis_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cdn/cdn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/cdn_sessions_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cdn_sessions_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.512255 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/local_docdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/docdb/patches.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/file_system/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/file_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/file_system/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/file_system/local_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/file_system/minio_file_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/files/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/flux/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/flux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/flux/flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/oidc_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/service_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16117 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/tokens_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/oidc/users_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/request_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/storage/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/storage/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/storage/patches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8499 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/stories/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/stories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/stories/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.516255 youwol-0.1.9rc1/src/youwol/utils/clients/treedb/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/treedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/treedb/treedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/treedb/treedb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/clients/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/context/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27658 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/context/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9004 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/context/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/computation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/digest/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/constantes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/file_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/null.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/siv_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/http_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_gateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_gateway/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.520255 youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7513 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/http_clients/files_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/files_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/files_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/http_clients/flux_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/flux_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/flux_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/http_clients/stories_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/stories_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/stories_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/http_clients/tree_db_backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/tree_db_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/http_clients/tree_db_backend/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8147 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/middlewares/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/middlewares/root_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.456255 youwol-0.1.9rc1/src/youwol/utils/python_next/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/python_next/v3_12/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/python_next/v3_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/python_next/v3_12/tomllib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/request_info_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol/utils/servers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/servers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/servers/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/servers/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/servers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14903 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/utils_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/utils_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/utils_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 10:14:59.000000 youwol-0.1.9rc1/src/youwol/utils/utils_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:15:21.524255 youwol-0.1.9rc1/src/youwol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20543 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 10:15:21.000000 youwol-0.1.9rc1/src/youwol.egg-info/top_level.txt
```

### Comparing `youwol-0.1.9rc0/LICENSE` & `youwol-0.1.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/PKG-INFO` & `youwol-0.1.9rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youwol
-Version: 0.1.9rc0
+Version: 0.1.9rc1
 Summary: YouWol as a desktop application
 Author-email: "G. Reinisch" <greinisch@youwol.com>, "J. Decharne" <jdecharne@youwol.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `youwol-0.1.9rc0/README.md` & `youwol-0.1.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/pyproject.toml` & `youwol-0.1.9rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/__init__.py` & `youwol-0.1.9rc1/src/youwol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 It offers solutions for logging, HTTP clients, and various other helper functions.
 
 * [pipelines](@yw-nav-mod:youwol.pipelines): Pipelines introduce abstractions to work with projects (python backends,
 javascript applications, typescript projects, etc.) using a specific stack.
 They formalize steps such as initialization, building, testing, and deployment.
 """
 
-__version__ = "0.1.9rc"
+__version__ = "0.1.9rc1"
```

### Comparing `youwol-0.1.9rc0/src/youwol/app/__init__.py` & `youwol-0.1.9rc1/src/youwol/app/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/__init__.py` & `youwol-0.1.9rc1/src/youwol/app/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/browser_cache_store.py` & `youwol-0.1.9rc1/src/youwol/app/environment/browser_cache_store.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/clients.py` & `youwol-0.1.9rc1/src/youwol/app/environment/clients.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/config_from_module.py` & `youwol-0.1.9rc1/src/youwol/app/environment/config_from_module.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/errors_handling.py` & `youwol-0.1.9rc1/src/youwol/app/environment/errors_handling.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/local_auth.py` & `youwol-0.1.9rc1/src/youwol/app/environment/local_auth.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/defaults.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/defaults.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/flow_switches.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/flow_switches.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/model_remote.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/model_remote.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/models.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/models_config.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/models_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/models_project.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/models_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/models_token_storage.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/models_token_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/encrypted_file.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/encrypted_file.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/file.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/file.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/models/tokens_storage/path_base.py` & `youwol-0.1.9rc1/src/youwol/app/environment/models/tokens_storage/path_base.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/native_backends_config.py` & `youwol-0.1.9rc1/src/youwol/app/environment/native_backends_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/online_environments.py` & `youwol-0.1.9rc1/src/youwol/app/environment/online_environments.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/paths.py` & `youwol-0.1.9rc1/src/youwol/app/environment/paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/proxied_backends.py` & `youwol-0.1.9rc1/src/youwol/app/environment/proxied_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/python_dynamic_loader.py` & `youwol-0.1.9rc1/src/youwol/app/environment/python_dynamic_loader.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment.py` & `youwol-0.1.9rc1/src/youwol/app/environment/youwol_environment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/environment/youwol_environment_models.py` & `youwol-0.1.9rc1/src/youwol/app/environment/youwol_environment_models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/fastapi_app.py` & `youwol-0.1.9rc1/src/youwol/app/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/main.py` & `youwol-0.1.9rc1/src/youwol/app/main.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/main_args.py` & `youwol-0.1.9rc1/src/youwol/app/main_args.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/browser_middleware.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/browser_middleware.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/hybridizer_middleware.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/hybridizer_middleware.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/abstract_local_cloud_dispatch.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/common.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/custom_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/deprecated_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/download_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/forward_only_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/loading_graph_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py` & `youwol-0.1.9rc1/src/youwol/app/middlewares/local_cloud_hybridizers/workspace_explorer_rules.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/admin.py` & `youwol-0.1.9rc1/src/youwol/app/routers/admin.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/backends/implementation.py` & `youwol-0.1.9rc1/src/youwol/app/routers/backends/implementation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/backends/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/backends/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/commons.py` & `youwol-0.1.9rc1/src/youwol/app/routers/commons.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/custom_backends.py` & `youwol-0.1.9rc1/src/youwol/app/routers/custom_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/custom_commands/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/custom_commands/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/auto_download_thread.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/auto_download_thread.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/common.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/custom_asset.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/custom_asset.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/data.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/data.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/flux_project.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/flux_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/package.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/package.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/download_assets/story.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/download_assets/story.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/fortunes.txt` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/fortunes.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/custom_asset.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/custom_asset.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/data.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/data.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/flux_project.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/flux_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/package.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/package.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/story.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/story.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/environment/upload_assets/upload.py` & `youwol-0.1.9rc1/src/youwol/app/routers/environment/upload_assets/upload.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/implementation.py` & `youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/implementation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/local_cdn/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/local_cdn/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/native_backends.py` & `youwol-0.1.9rc1/src/youwol/app/routers/native_backends.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/native_backends_config.py` & `youwol-0.1.9rc1/src/youwol/app/routers/native_backends_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/dependencies.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/dependencies.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/implementation.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/implementation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/models_project.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/models_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/__init__.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/projects_finder_handlers.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/projects_resolver/projects_loader.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/projects_resolver/projects_loader.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/projects/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/projects/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/python/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/python/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/router_remote.py` & `youwol-0.1.9rc1/src/youwol/app/routers/router_remote.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/system/documentation.py` & `youwol-0.1.9rc1/src/youwol/app/routers/system/documentation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/system/documentation_models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/system/documentation_models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/system/models.py` & `youwol-0.1.9rc1/src/youwol/app/routers/system/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
             channelId = options?.channelId || `${{uuid.v4()}}`
             const resp$ = new ReplaySubject()
             wsData$.pipe(
                 filter(({{labels, attributes}}) => {{
                     return labels.includes('AsyncTaskResult') &&
                     (
                         labels.includes(channelId) || // deprecated, use attributes instead (youwol>=0.1.9)
-                        attributes[{FuturesResponse.channelIdKey}] === channelId
+                        attributes['{FuturesResponse.channelIdKey}'] === channelId
                     )
                 }}),
                 takeWhile((m) => !m.labels.includes("{FuturesResponseEnd.__name__}"))
             ).subscribe(
                 (d) => {{resp$.next(d)}},
                 (e) => console.error(e),
                 () => resp$.complete()
```

### Comparing `youwol-0.1.9rc0/src/youwol/app/routers/system/router.py` & `youwol-0.1.9rc1/src/youwol/app/routers/system/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/shut_down.py` & `youwol-0.1.9rc1/src/youwol/app/shut_down.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/start.py` & `youwol-0.1.9rc1/src/youwol/app/start.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/web_socket.py` & `youwol-0.1.9rc1/src/youwol/app/web_socket.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/app/wrapper.py` & `youwol-0.1.9rc1/src/youwol/app/wrapper.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/admin/impersonation_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/admin/impersonation_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/admin/registration_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/admin/registration_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/configuration.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/configuration.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_service.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/openid_flows_service.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/openid_flows_states.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/openid_flows_states.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/openid_rp/paths.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/openid_rp/paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/accounts/router.py` & `youwol-0.1.9rc1/src/youwol/backends/accounts/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/router.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/access.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/access.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/assets.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/assets.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/files.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/files.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/images.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/images.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/permissions.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/permissions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/routers/raw.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/routers/raw.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/assets/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/all_icons_emojipedia.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/all_icons_emojipedia.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/assets_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/assets_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/cdn_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/cdn_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/common.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/deprecated.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/deprecated.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/files_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/files_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/flux_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/flux_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/misc.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/misc.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/stories_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/stories_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/routers/treedb_backend.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/routers/treedb_backend.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/assets_gateway/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/assets_gateway/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/loading_graph_implementation.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/loading_graph_implementation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn/utils_indexing.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn/utils_indexing.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_apps_server/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_apps_server/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/cdn_sessions_storage/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/cdn_sessions_storage/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/files/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/files/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/files/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/files/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/files/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/files/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/files/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/files/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/backward_compatibility.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/index.html` & `youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/index.html`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js` & `youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/main.4dd266971cc92c3a3cc3.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js` & `youwol-0.1.9rc1/src/youwol/backends/flux/bundle_app_template/on-load_ts.fdb7e88f67ac0ae6bc0d.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/flux/workflow_new_project.py` & `youwol-0.1.9rc1/src/youwol/backends/flux/workflow_new_project.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/stories/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/stories/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/stories/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/stories/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/stories/root_paths.py` & `youwol-0.1.9rc1/src/youwol/backends/stories/root_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/stories/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/stories/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/__init__.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/configurations.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/configurations.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/deployment.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/deployment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/router.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/router.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/drives.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/drives.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/entities.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/entities.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/folders.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/folders.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/groups.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/groups.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/routers/items.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/routers/items.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/backends/tree_db/utils.py` & `youwol-0.1.9rc1/src/youwol/backends/tree_db/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/__init__.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/.yw_pipeline/yw_pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/install.sh` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/install.sh`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/pyproject.toml.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/fastapi_app.py.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/src/main.py.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template/start.sh` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template/start.sh`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/template.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/template.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_python_backend/views/run.view.js` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_python_backend/views/run.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/__init__.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_raw_app/__init__.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_raw_app/pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_raw_app/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_dependencies_version.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/npm_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/steps.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/common/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/environment.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/skeleton.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/.yw_pipeline/yw_pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/README.lib.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/common.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/external/templates/src/tests/install.test.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/build_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/common.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/dependencies_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/doc_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/pipeline.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/setup_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/skeleton.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.app.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/.yw_pipeline/yw_pipeline.lib.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/LICENSE`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.app.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/README.lib.md`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/auto-generated.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/package.json`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/index.html`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.app/app/on-load.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/src.lib/lib/hello.view.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.app.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/template.lib.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.app.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/templates/webpack.config.lib.ts`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/test_step.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/consistency.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/views/dependencies.view.js`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py` & `youwol-0.1.9rc1/src/youwol/pipelines/pipeline_typescript_weback_npm/regular/webpack_dev_server_switch.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/pipelines/publish_cdn.py` & `youwol-0.1.9rc1/src/youwol/pipelines/publish_cdn.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/assets/assets.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/assets/assets.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/assets_gateway/assets_gateway.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/assets_gateway/assets_gateway.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/cache/cache.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/cache/cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/cache/local_cache.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/cache/local_cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/cache/redis_cache.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/cdn/cdn.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/cdn/cdn.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/cdn_sessions_storage/cdn_sessions_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/docdb.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/docdb/docdb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/local_docdb.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/docdb/local_docdb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/models.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/docdb/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/docdb/patches.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/docdb/patches.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/interfaces.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/file_system/interfaces.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/local_file_system.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/file_system/local_file_system.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/file_system/minio_file_system.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/file_system/minio_file_system.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/files/files.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/files/files.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/flux/flux.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/flux/flux.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/oidc_config.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/oidc/oidc_config.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/service_account_client.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/oidc/service_account_client.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/tokens_manager.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/oidc/tokens_manager.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/oidc/users_management.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/oidc/users_management.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/request_executor.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/request_executor.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/storage/local_storage.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/storage/local_storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/storage/storage.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/storage/storage.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/stories/stories.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/stories/stories.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/treedb/treedb.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/treedb/treedb_utils.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/treedb/treedb_utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/types.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/clients/utils.py` & `youwol-0.1.9rc1/src/youwol/utils/clients/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/context/context.py` & `youwol-0.1.9rc1/src/youwol/utils/context/context.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/context/models.py` & `youwol-0.1.9rc1/src/youwol/utils/context/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/context/reporter.py` & `youwol-0.1.9rc1/src/youwol/utils/context/reporter.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/computation.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/digest/computation.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/defaults.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/digest/defaults.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/helpers.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/digest/helpers.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/traces.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/digest/traces.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/digest/types.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/digest/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/constantes.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/constantes.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/exceptions.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/exceptions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/file_encryption.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/file_encryption.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/null.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/null.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/siv_256.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/siv_256.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/crypto/file_encryption/utils.py` & `youwol-0.1.9rc1/src/youwol/utils/crypto/file_encryption/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/exceptions.py` & `youwol-0.1.9rc1/src/youwol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/assets_gateway/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/assets_gateway/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/cdn_backend/utils.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/cdn_backend/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/files_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/files_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/flux_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/flux_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/stories_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/stories_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/http_clients/tree_db_backend/models.py` & `youwol-0.1.9rc1/src/youwol/utils/http_clients/tree_db_backend/models.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/middlewares/authentication.py` & `youwol-0.1.9rc1/src/youwol/utils/middlewares/authentication.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/middlewares/root_middleware.py` & `youwol-0.1.9rc1/src/youwol/utils/middlewares/root_middleware.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/request_info_factory.py` & `youwol-0.1.9rc1/src/youwol/utils/request_info_factory.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/servers/env.py` & `youwol-0.1.9rc1/src/youwol/utils/servers/env.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/servers/fast_api.py` & `youwol-0.1.9rc1/src/youwol/utils/servers/fast_api.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/types.py` & `youwol-0.1.9rc1/src/youwol/utils/types.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/utils.py` & `youwol-0.1.9rc1/src/youwol/utils/utils.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/utils_helm.py` & `youwol-0.1.9rc1/src/youwol/utils/utils_helm.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/utils_paths.py` & `youwol-0.1.9rc1/src/youwol/utils/utils_paths.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/utils_requests.py` & `youwol-0.1.9rc1/src/youwol/utils/utils_requests.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol/utils/utils_shell.py` & `youwol-0.1.9rc1/src/youwol/utils/utils_shell.py`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol.egg-info/PKG-INFO` & `youwol-0.1.9rc1/src/youwol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youwol
-Version: 0.1.9rc0
+Version: 0.1.9rc1
 Summary: YouWol as a desktop application
 Author-email: "G. Reinisch" <greinisch@youwol.com>, "J. Decharne" <jdecharne@youwol.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `youwol-0.1.9rc0/src/youwol.egg-info/SOURCES.txt` & `youwol-0.1.9rc1/src/youwol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `youwol-0.1.9rc0/src/youwol.egg-info/requires.txt` & `youwol-0.1.9rc1/src/youwol.egg-info/requires.txt`

 * *Files identical despite different names*

