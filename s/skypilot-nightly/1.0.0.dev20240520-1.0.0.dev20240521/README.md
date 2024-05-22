# Comparing `tmp/skypilot_nightly-1.0.0.dev20240520.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240520.tar", last modified: Mon May 20 10:38:35 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240521.tar", last modified: Tue May 21 10:38:20 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240520.tar` & `skypilot_nightly-1.0.0.dev20240521.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.780552 skypilot_nightly-1.0.0.dev20240520/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-20 10:38:35.780552 skypilot_nightly-1.0.0.dev20240520/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:38:35.780552 skypilot_nightly-1.0.0.dev20240520/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-20 10:38:32.000000 skypilot_nightly-1.0.0.dev20240520/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.720552 skypilot_nightly-1.0.0.dev20240520/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.724552 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.724552 skypilot_nightly-1.0.0.dev20240520/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   230655 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.724552 skypilot_nightly-1.0.0.dev20240520/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.724552 skypilot_nightly-1.0.0.dev20240520/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   194298 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.728552 skypilot_nightly-1.0.0.dev20240520/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31817 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    48019 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11166 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.732552 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.732552 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.732552 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.732552 skypilot_nightly-1.0.0.dev20240520/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/global_user_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/jobs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    54188 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.736552 skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.740552 skypilot_nightly-1.0.0.dev20240520/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.740552 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.740552 skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.740552 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.740552 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.744552 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.744552 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.744552 skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.744552 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.748552 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.748552 skypilot_nightly-1.0.0.dev20240520/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    28710 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    56630 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.748552 skypilot_nightly-1.0.0.dev20240520/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-20 10:38:32.000000 skypilot_nightly-1.0.0.dev20240520/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.752552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.752552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.752552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.752552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.752552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.756552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.756552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.756552 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/skypilot_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    47807 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.760552 skypilot_nightly-1.0.0.dev20240520/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/jobs-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.760552 skypilot_nightly-1.0.0.dev20240520/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.764552 skypilot_nightly-1.0.0.dev20240520/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.764552 skypilot_nightly-1.0.0.dev20240520/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.764552 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/generate_kind_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/generate_static_kubeconfig.sh
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23115 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.768552 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 10:38:35.000000 skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:38:35.768552 skypilot_nightly-1.0.0.dev20240520/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_jobs_and_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   216733 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-20 10:38:30.000000 skypilot_nightly-1.0.0.dev20240520/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.794042 skypilot_nightly-1.0.0.dev20240521/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-21 10:38:20.794042 skypilot_nightly-1.0.0.dev20240521/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 10:38:20.794042 skypilot_nightly-1.0.0.dev20240521/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-21 10:38:17.000000 skypilot_nightly-1.0.0.dev20240521/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.734042 skypilot_nightly-1.0.0.dev20240521/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.734042 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21408 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.738042 skypilot_nightly-1.0.0.dev20240521/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125420 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   230655 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.738042 skypilot_nightly-1.0.0.dev20240521/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.738042 skypilot_nightly-1.0.0.dev20240521/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26446 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   194298 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.742042 skypilot_nightly-1.0.0.dev20240521/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44519 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30929 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31840 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47944 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20969 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20272 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11991 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25136 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11000 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15383 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.742042 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11802 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34233 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118872 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25107 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/global_user_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.746042 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25556 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33067 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/jobs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56668 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36307 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9339 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16758 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.750042 skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.754042 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24215 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22186 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.754042 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32919 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.754042 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9384 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62091 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.754042 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25103 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.754042 skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.758042 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.758042 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24488 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65346 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.762042 skypilot_nightly-1.0.0.dev20240521/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30136 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28710 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11548 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57216 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37183 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14469 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.762042 skypilot_nightly-1.0.0.dev20240521/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12055 2024-05-21 10:38:17.000000 skypilot_nightly-1.0.0.dev20240521/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.762042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35198 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18824 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.762042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.762042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19215 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16355 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.766042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.766042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13971 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.766042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.766042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.766042 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/skypilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47807 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.770042 skypilot_nightly-1.0.0.dev20240521/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/jobs-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.770042 skypilot_nightly-1.0.0.dev20240521/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.774042 skypilot_nightly-1.0.0.dev20240521/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.774042 skypilot_nightly-1.0.0.dev20240521/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34359 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.778042 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9759 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/generate_kind_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4422 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/generate_static_kubeconfig.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23359 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.782042 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 10:38:20.000000 skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 10:38:20.782042 skypilot_nightly-1.0.0.dev20240521/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17649 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_jobs_and_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   216733 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-05-21 10:38:14.000000 skypilot_nightly-1.0.0.dev20240521/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/LICENSE` & `skypilot_nightly-1.0.0.dev20240521/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240521/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240521/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240520
+Version: 1.0.0.dev20240521
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/README.md` & `skypilot_nightly-1.0.0.dev20240521/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240521/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/setup.py` & `skypilot_nightly-1.0.0.dev20240521/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '19e8ed16a8cdb34f9f1963da19db1ce317798eb1'
+_SKYPILOT_COMMIT_SHA = 'cf840dc7fdbaf59bf6ba31b302fd12f2a1dd62d3'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240520'
+__version__ = '1.0.0.dev20240521'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240521/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240521/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/cloud_vm_ray_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240521/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/check.py` & `skypilot_nightly-1.0.0.dev20240521/sky/check.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from sky.adaptors import cloudflare
 from sky.utils import ux_utils
 
 
 def check(
     quiet: bool = False,
     verbose: bool = False,
-    clouds: Optional[Tuple[str]] = None,
+    clouds: Optional[Iterable[str]] = None,
 ) -> None:
     echo = (lambda *_args, **_kwargs: None) if quiet else click.echo
     echo('Checking credentials to enable clouds for SkyPilot.')
     enabled_clouds = []
     disabled_clouds = []
 
     def check_one_cloud(
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240521/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240521/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/aws.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,17 +336,14 @@
 
         if num_gigabytes > 1:
             cost += (num_gigabytes - 1) * 0.09
 
         cost += 0.0
         return cost
 
-    def is_same_cloud(self, other: clouds.Cloud):
-        return isinstance(other, AWS)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,14 @@
 
         if num_gigabytes > 1:
             cost += (num_gigabytes - 1) * 0.0875
 
         cost += 0.0
         return cost
 
-    def is_same_cloud(self, other):
-        return isinstance(other, Azure)
-
     @classmethod
     def get_image_size(cls, image_id: str, region: Optional[str]) -> float:
         if region is None:
             # The region used here is only for where to send the query,
             # not the image location. Azure's image is globally available.
             region = 'eastus'
         is_skypilot_image_tag = False
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,16 +243,16 @@
     def get_egress_cost(self, num_gigabytes: float):
         """Returns the egress cost.
 
         TODO: takes into account "per month" accumulation per account.
         """
         raise NotImplementedError
 
-    def is_same_cloud(self, other: 'Cloud'):
-        raise NotImplementedError
+    def is_same_cloud(self, other: 'Cloud') -> bool:
+        return isinstance(other, self.__class__)
 
     def make_deploy_resources_variables(
         self,
         resources: 'resources_lib.Resources',
         cluster_name_on_cloud: str,
         region: 'Region',
         zones: Optional[List['Zone']],
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/cudo.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,18 +151,14 @@
         return 0.0
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         # Change if your cloud has egress cost. (You can do this later;
         # `return 0.0` is a good placeholder.)
         return 0.0
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, Cudo)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/fluidstack.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,18 +136,14 @@
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
     def __repr__(self):
         return 'Fluidstack'
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, Fluidstack)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[DiskTier] = None) -> Optional[str]:
         return service_catalog.get_default_instance_type(cpus=cpus,
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/gcp.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,17 +311,14 @@
         if num_gigabytes <= 1024:
             return 0.12 * num_gigabytes
         elif num_gigabytes <= 1024 * 10:
             return 0.11 * num_gigabytes
         else:
             return 0.08 * num_gigabytes
 
-    def is_same_cloud(self, other):
-        return isinstance(other, GCP)
-
     @classmethod
     def _is_machine_image(cls, image_id: str) -> bool:
         find_machine = re.match(r'projects/.*/.*/machineImages/.*', image_id)
         return find_machine is not None
 
     @classmethod
     @functools.lru_cache(maxsize=1)
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/ibm.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,17 +161,14 @@
         for price_threshold in price_thresholds:
             # pylint: disable=line-too-long
             cost += (num_gigabytes - price_threshold['threshold']
                     ) * price_threshold['price_per_gb']
             num_gigabytes -= (num_gigabytes - price_threshold['threshold'])
         return cost
 
-    def is_same_cloud(self, other):
-        return isinstance(other, IBM)
-
     def make_deploy_resources_variables(
         self,
         resources: 'resources_lib.Resources',
         cluster_name_on_cloud: str,
         region: 'clouds.Region',
         zones: Optional[List['clouds.Zone']],
         dryrun: bool = False,
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/kubernetes.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,17 +136,14 @@
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
     def __repr__(self):
         return self._REPR
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        return isinstance(other, Kubernetes)
-
     @classmethod
     def get_port(cls, svc_name) -> int:
         ns = kubernetes_utils.get_current_kube_config_context_namespace()
         return kubernetes_utils.get_port(svc_name, ns)
 
     @classmethod
     def get_default_instance_type(
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/lambda_cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,14 @@
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
     def __repr__(self):
         return 'Lambda'
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, Lambda)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/oci.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,18 +156,14 @@
         # elif region in REGIONS_MidEast_Africa:
         #     return (num_gigabytes - 10 * 1024) * 0.05
         # else:
         #     logger.debug(f"* ! Region {region} is not listed for cost calc!")
         #     return 0.0
         return (num_gigabytes - 10 * 1024) * 0.0085
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, OCI)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/paperspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,18 +143,14 @@
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
     def __repr__(self):
         return self._REPR
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, Paperspace)
-
     @classmethod
     def get_default_instance_type(
         cls,
         cpus: Optional[str] = None,
         memory: Optional[str] = None,
         disk_tier: Optional[resources_utils.DiskTier] = None,
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/runpod.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,18 +136,14 @@
         """Returns the hourly cost of the accelerators, in dollars/hour."""
         del accelerators, use_spot, region, zone  # unused
         return 0.0  # RunPod includes accelerators in the hourly cost.
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, RunPod)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/scp.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,18 +140,14 @@
         del accelerators, use_spot, region, zone  # unused
         # SCP includes accelerators as part of the instance type.
         return 0.0
 
     def get_egress_cost(self, num_gigabytes: float) -> float:
         return 0.0
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, SCP)
-
     @classmethod
     def get_default_instance_type(
             cls,
             cpus: Optional[str] = None,
             memory: Optional[str] = None,
             disk_tier: Optional[resources_utils.DiskTier] = None
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240521/sky/clouds/vsphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,14 @@
     def get_egress_cost(self, num_gigabytes: float) -> float:
         # vSphere doesn't support this part.
         return 0.0
 
     def __repr__(self):
         return 'vSphere'
 
-    def is_same_cloud(self, other: clouds.Cloud) -> bool:
-        # Returns true if the two clouds are the same cloud type.
-        return isinstance(other, Vsphere)
-
     @classmethod
     def get_default_instance_type(
         cls,
         cpus: Optional[str] = None,
         memory: Optional[str] = None,
         disk_tier: Optional[resources_utils.DiskTier] = None,
     ) -> Optional[str]:
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/core.py` & `skypilot_nightly-1.0.0.dev20240521/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240521/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240521/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240521/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240521/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240521/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240521/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/controller.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/core.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/state.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/jobs/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240521/sky/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Optimizer: assigns best resources to user tasks."""
 import collections
 import copy
 import enum
 import json
 import typing
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Set, Tuple
 
 import colorama
 import numpy as np
 import prettytable
 
 from sky import check as sky_check
 from sky import clouds
@@ -116,14 +116,16 @@
             quiet: whether to suppress logging.
 
         Raises:
             exceptions.ResourcesUnavailableError: if no resources are available
                 for a task.
             exceptions.NoCloudAccessError: if no public clouds are enabled.
         """
+        _check_specified_clouds(dag)
+
         # This function is effectful: mutates every node in 'dag' by setting
         # node.best_resources if it is None.
         Optimizer._add_dummy_source_sink_nodes(dag)
         try:
             unused_best_plan = Optimizer._optimize_dag(
                 dag=dag,
                 minimize_cost=minimize == OptimizeTarget.COST,
@@ -265,15 +267,14 @@
             fuzzy_candidates: List[str] = []
             if node_i < len(topo_order) - 1:
                 # Convert partial resource labels to launchable resources.
                 launchable_resources, cloud_candidates, fuzzy_candidates = (
                     _fill_in_launchable_resources(
                         task=node,
                         blocked_resources=blocked_resources,
-                        try_fix_with_sky_check=True,
                         quiet=quiet))
                 node_to_candidate_map[node] = cloud_candidates
             else:
                 # Dummy sink node.
                 launchable_resources = {
                     list(node.resources)[0]: list(node.resources)
                 }
@@ -988,26 +989,26 @@
                             f'{accelerators_str}')
 
         graph = dag.get_graph()
         local_dag = copy.deepcopy(dag) if has_resources_ordered else dag
         for task_id in range(len(dag.tasks)):
             task = dag.tasks[task_id]
             if isinstance(task.resources, list):
+                # For ordered resources, we try the resources in the order
+                # specified by the user.
                 local_task = local_dag.tasks[task_id]
                 for resources in task.resources:
                     # Check if there exists launchable resources
                     local_task.set_resources(resources)
-                    launchable_resources_map, _ , _ = \
+                    launchable_resources_map, _, _ = (
                         _fill_in_launchable_resources(
-                            task = local_task,
-                            blocked_resources = blocked_resources,
-                            try_fix_with_sky_check = True,
-                            quiet = False
-                    )
-                    if len(launchable_resources_map[resources]) != 0:
+                            task=local_task,
+                            blocked_resources=blocked_resources,
+                            quiet=False))
+                    if launchable_resources_map.get(resources, []):
                         break
 
         local_graph = local_dag.get_graph()
         local_topo_order = list(nx.topological_sort(local_graph))
         local_node_to_cost_map, local_node_to_candidate_map = (
             Optimizer._estimate_nodes_cost_or_time(local_topo_order,
                                                    minimize_cost,
@@ -1039,32 +1040,33 @@
                          '      \'sky check\' to check the enabled clouds.')
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesUnavailableError(error_msg)
 
         if has_resources_ordered:
             best_plan = {}
             # We have to manually set the best_resources for the tasks in the
-            # original dag, to pass the optimization results
-            # to the caller, as we deep copied the dag
-            # when the dag has nodes with ordered resources.
+            # original dag, to pass the optimization results to the caller, as
+            # we deep copied the dag when the dag has nodes with ordered
+            # resources.
             for task, resources in local_best_plan.items():
                 task_idx = local_dag.tasks.index(task)
                 dag.tasks[task_idx].best_resources = resources
                 best_plan[dag.tasks[task_idx]] = resources
+
+            topo_order = list(nx.topological_sort(graph))
+            # Get the cost of each specified resources for display purpose.
+            node_to_cost_map, _ = Optimizer._estimate_nodes_cost_or_time(
+                topo_order=topo_order,
+                minimize_cost=minimize_cost,
+                blocked_resources=blocked_resources,
+                quiet=True)
         else:
             best_plan = local_best_plan
-
-        topo_order = list(nx.topological_sort(graph)) if has_resources_ordered \
-            else local_topo_order
-        node_to_cost_map, _ = (Optimizer._estimate_nodes_cost_or_time(
-            topo_order=topo_order,
-            minimize_cost=minimize_cost,
-            blocked_resources=blocked_resources,
-            quiet=True)) if has_resources_ordered else (
-                local_node_to_cost_map, local_node_to_candidate_map)
+            topo_order = local_topo_order
+            node_to_cost_map = local_node_to_cost_map
 
         if not quiet:
             Optimizer.print_optimized_plan(graph, topo_order, best_plan,
                                            total_time, total_cost,
                                            node_to_cost_map, minimize_cost)
             if not env_options.Options.MINIMIZE_LOGGING.get():
                 Optimizer._print_candidates(local_node_to_candidate_map)
@@ -1142,90 +1144,141 @@
             if resources.should_be_blocked_by(blocked):
                 break
         else:  # non-blocked launchable resources. (no break)
             available_resources.append(resources)
     return available_resources
 
 
+def _check_specified_clouds(dag: 'dag_lib.Dag') -> None:
+    """Check if specified clouds are enabled in cache and refresh if needed.
+
+    Our enabled cloud list is cached in a local database, and if a user
+    specified a cloud that is not enabled, we should refresh the cache for that
+    cloud in case the cloud access has been enabled since the last cache update.
+
+    Args:
+        dag: The DAG specified by a user.
+    """
+    enabled_clouds = sky_check.get_cached_enabled_clouds_or_refresh(
+        raise_if_no_cloud_access=True)
+
+    global_disabled_clouds: Set[str] = set()
+    for task in dag.tasks:
+        # Recheck the enabled clouds if the task's requested resources are on a
+        # cloud that is not enabled in the cached enabled_clouds.
+        all_clouds_specified: Set[str] = set()
+        clouds_need_recheck: Set[str] = set()
+        for resources in task.resources:
+            cloud_str = str(resources.cloud)
+            if (resources.cloud is not None and not clouds.cloud_in_iterable(
+                    resources.cloud, enabled_clouds)):
+                # Explicitly check again to update the enabled cloud list.
+                clouds_need_recheck.add(cloud_str)
+            all_clouds_specified.add(cloud_str)
+
+        # Explicitly check again to update the enabled cloud list.
+        sky_check.check(quiet=True,
+                        clouds=list(clouds_need_recheck -
+                                    global_disabled_clouds))
+        enabled_clouds = sky_check.get_cached_enabled_clouds_or_refresh(
+            raise_if_no_cloud_access=True)
+        disabled_clouds = (clouds_need_recheck -
+                           {str(c) for c in enabled_clouds})
+        global_disabled_clouds.update(disabled_clouds)
+        if disabled_clouds:
+            is_or_are = 'is' if len(disabled_clouds) == 1 else 'are'
+            task_name = f' {task.name!r}' if task.name is not None else ''
+            msg = (f'Task{task_name} requires {", ".join(disabled_clouds)} '
+                   f'which {is_or_are} not enabled. To enable access, change '
+                   f'the task cloud requirement or run: {colorama.Style.BRIGHT}'
+                   f'sky check {" ".join(c.lower() for c in disabled_clouds)}'
+                   f'{colorama.Style.RESET_ALL}')
+            if all_clouds_specified == disabled_clouds:
+                # If all resources are specified with a disabled cloud, we
+                # should raise an error as no resource can satisfy the
+                # requirement. Otherwise, we should just skip the resource.
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.ResourcesUnavailableError(msg)
+            logger.warning(
+                f'{colorama.Fore.YELLOW}{msg}{colorama.Style.RESET_ALL}')
+
+
 def _fill_in_launchable_resources(
     task: task_lib.Task,
     blocked_resources: Optional[Iterable[resources_lib.Resources]],
-    try_fix_with_sky_check: bool = True,
     quiet: bool = False
 ) -> Tuple[Dict[resources_lib.Resources, List[resources_lib.Resources]],
            _PerCloudCandidates, List[str]]:
     """Fills in the launchable resources for the task.
 
     Returns:
       A tuple of:
         Dict mapping the task's requested Resources to a list of launchable
           Resources,
         Dict mapping Cloud to a list of feasible Resources (for printing),
         Sorted list of fuzzy candidates (alternative GPU names).
+    Raises:
+      ResourcesUnavailableError: if all resources required by the task are on
+        a cloud that is not enabled.
     """
     enabled_clouds = sky_check.get_cached_enabled_clouds_or_refresh(
         raise_if_no_cloud_access=True)
-    launchable = collections.defaultdict(list)
+
+    launchable: Dict[resources_lib.Resources, List[resources_lib.Resources]] = (
+        collections.defaultdict(list))
     all_fuzzy_candidates = set()
     cloud_candidates: _PerCloudCandidates = collections.defaultdict(
         List[resources_lib.Resources])
     if blocked_resources is None:
         blocked_resources = []
     for resources in task.resources:
         if (resources.cloud is not None and
                 not clouds.cloud_in_iterable(resources.cloud, enabled_clouds)):
-            if try_fix_with_sky_check:
-                # Explicitly check again to update the enabled cloud list.
-                sky_check.check(quiet=True)
-                return _fill_in_launchable_resources(task, blocked_resources,
-                                                     False)
-            with ux_utils.print_exception_no_traceback():
-                raise exceptions.ResourcesUnavailableError(
-                    f'Task requires {resources.cloud} which is '
-                    f'not enabled: {task}.\nTo enable access, run '
-                    f'{colorama.Style.BRIGHT}'
-                    f'sky check {colorama.Style.RESET_ALL}, or change the '
-                    'cloud requirement')
-        else:
-            clouds_list = ([resources.cloud]
-                           if resources.cloud is not None else enabled_clouds)
-            for cloud in clouds_list:
-                (feasible_resources, fuzzy_candidate_list) = (
-                    cloud.get_feasible_launchable_resources(
-                        resources, num_nodes=task.num_nodes))
-                if len(feasible_resources) > 0:
-                    # Assume feasible_resources is sorted by prices.
-                    cheapest = feasible_resources[0]
-                    # Generate region/zone-specified resources.
-                    launchable[resources].extend(
-                        _make_launchables_for_valid_region_zones(cheapest))
-                    cloud_candidates[cloud] = feasible_resources
-                else:
-                    all_fuzzy_candidates.update(fuzzy_candidate_list)
-            if len(launchable[resources]) == 0:
-                clouds_str = str(clouds_list) if len(clouds_list) > 1 else str(
-                    clouds_list[0])
-                num_node_str = ''
-                if task.num_nodes > 1:
-                    num_node_str = f'{task.num_nodes}x '
-                if not quiet:
-                    logger.info(
-                        f'No resource satisfying {num_node_str}'
-                        f'{resources.repr_with_region_zone} on {clouds_str}.')
-                if len(all_fuzzy_candidates) > 0:
+            # Skip the resources that are on a cloud that is not enabled. The
+            # hint has been printed in _check_specified_clouds.
+            launchable[resources] = []
+            continue
+        clouds_list = ([resources.cloud]
+                       if resources.cloud is not None else enabled_clouds)
+        for cloud in clouds_list:
+            (feasible_resources,
+             fuzzy_candidate_list) = cloud.get_feasible_launchable_resources(
+                 resources, num_nodes=task.num_nodes)
+            if len(feasible_resources) > 0:
+                # Assume feasible_resources is sorted by prices. Guaranteed by
+                # the implementation of get_feasible_launchable_resources and
+                # the underlying service_catalog filtering
+                cheapest = feasible_resources[0]
+                # Generate region/zone-specified resources.
+                launchable[resources].extend(
+                    _make_launchables_for_valid_region_zones(cheapest))
+                cloud_candidates[cloud] = feasible_resources
+            else:
+                all_fuzzy_candidates.update(fuzzy_candidate_list)
+        if len(launchable[resources]) == 0:
+            clouds_str = str(clouds_list) if len(clouds_list) > 1 else str(
+                clouds_list[0])
+            num_node_str = ''
+            if task.num_nodes > 1:
+                num_node_str = f'{task.num_nodes}x '
+            if not quiet:
+                logger.info(
+                    f'No resource satisfying {num_node_str}'
+                    f'{resources.repr_with_region_zone} on {clouds_str}.')
+                if all_fuzzy_candidates:
                     logger.info('Did you mean: '
                                 f'{colorama.Fore.CYAN}'
                                 f'{sorted(all_fuzzy_candidates)}'
                                 f'{colorama.Style.RESET_ALL}')
-                else:
-                    if resources.cpus is not None:
-                        logger.info('Try specifying a different CPU count, '
-                                    'or add "+" to the end of the CPU count '
-                                    'to allow for larger instances.')
-                    if resources.memory is not None:
-                        logger.info('Try specifying a different memory size, '
-                                    'or add "+" to the end of the memory size '
-                                    'to allow for larger instances.')
+            else:
+                if resources.cpus is not None:
+                    logger.info('Try specifying a different CPU count, '
+                                'or add "+" to the end of the CPU count '
+                                'to allow for larger instances.')
+                if resources.memory is not None:
+                    logger.info('Try specifying a different memory size, '
+                                'or add "+" to the end of the memory size '
+                                'to allow for larger instances.')
 
         launchable[resources] = _filter_out_blocked_launchable_resources(
             launchable[resources], blocked_resources)
     return launchable, cloud_candidates, list(sorted(all_fuzzy_candidates))
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240521/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/replica_managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -484,14 +484,15 @@
                 f'launched_at={info_dict["launched_at"]}{handle_str})')
         return info
 
     def probe(
         self,
         readiness_path: str,
         post_data: Optional[Dict[str, Any]],
+        headers: Optional[Dict[str, str]],
     ) -> Tuple['ReplicaInfo', bool, float]:
         """Probe the readiness of the replica.
 
         Returns:
             Tuple of (self, is_ready, probe_time).
         """
         replica_identity = f'replica {self.replica_id} with url {self.url}'
@@ -509,20 +510,22 @@
                 return self, False, probe_time
             readiness_path = (f'{url}{readiness_path}')
             logger.info(f'Probing {replica_identity} with {readiness_path}.')
             if post_data is not None:
                 msg += 'POST'
                 response = requests.post(
                     readiness_path,
+                    headers=headers,
                     json=post_data,
                     timeout=serve_constants.READINESS_PROBE_TIMEOUT_SECONDS)
             else:
                 msg += 'GET'
                 response = requests.get(
                     readiness_path,
+                    headers=headers,
                     timeout=serve_constants.READINESS_PROBE_TIMEOUT_SECONDS)
             msg += (f' request to {replica_identity} returned status '
                     f'code {response.status_code}')
             if response.status_code == 200:
                 msg += '.'
                 log_method = logger.info
             else:
@@ -561,17 +564,21 @@
     def __init__(self, service_name: str,
                  spec: 'service_spec.SkyServiceSpec') -> None:
         self.lock = threading.Lock()
         self._next_replica_id: int = 1
         self._service_name: str = service_name
         self._uptime: Optional[float] = None
         self._update_mode = serve_utils.DEFAULT_UPDATE_MODE
+        header_keys = None
+        if spec.readiness_headers is not None:
+            header_keys = list(spec.readiness_headers.keys())
         logger.info(f'Readiness probe path: {spec.readiness_path}\n'
                     f'Initial delay seconds: {spec.initial_delay_seconds}\n'
-                    f'Post data: {spec.post_data}')
+                    f'Post data: {spec.post_data}\n'
+                    f'Readiness header keys: {header_keys}')
 
         # Newest version among the currently provisioned and launched replicas
         self.latest_version: int = serve_constants.INITIAL_VERSION
         # Oldest version among the currently provisioned and launched replicas
         self.least_recent_version: int = serve_constants.INITIAL_VERSION
         serve_state.add_or_update_version(self._service_name,
                                           self.latest_version, spec)
@@ -1029,16 +1036,19 @@
                 if not info.status_property.should_track_service_status():
                     continue
                 replica_to_probe.append(
                     f'replica_{info.replica_id}(url={info.url})')
                 probe_futures.append(
                     pool.apply_async(
                         info.probe,
-                        (self._get_readiness_path(
-                            info.version), self._get_post_data(info.version)),
+                        (
+                            self._get_readiness_path(info.version),
+                            self._get_post_data(info.version),
+                            self._get_readiness_headers(info.version),
+                        ),
                     ),)
             logger.info(f'Replicas to probe: {", ".join(replica_to_probe)}')
 
             # Since futures.as_completed will return futures in the order of
             # completion, we need the info.probe function to return the info
             # object as well, so that we could update the info object in the
             # same order.
@@ -1211,9 +1221,12 @@
 
     def _get_readiness_path(self, version: int) -> str:
         return self._get_version_spec(version).readiness_path
 
     def _get_post_data(self, version: int) -> Optional[Dict[str, Any]]:
         return self._get_version_spec(version).post_data
 
+    def _get_readiness_headers(self, version: int) -> Optional[Dict[str, str]]:
+        return self._get_version_spec(version).readiness_headers
+
     def _get_initial_delay_seconds(self, version: int) -> int:
         return self._get_version_spec(version).initial_delay_seconds
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240521/sky/serve/service_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         self,
         readiness_path: str,
         initial_delay_seconds: int,
         min_replicas: int,
         max_replicas: Optional[int] = None,
         target_qps_per_replica: Optional[float] = None,
         post_data: Optional[Dict[str, Any]] = None,
+        readiness_headers: Optional[Dict[str, str]] = None,
         dynamic_ondemand_fallback: Optional[bool] = None,
         base_ondemand_fallback_replicas: Optional[int] = None,
         upscale_delay_seconds: Optional[int] = None,
         downscale_delay_seconds: Optional[int] = None,
         # The following arguments are deprecated.
         # TODO(ziming): remove this after 2 minor release, i.e. 0.6.0.
         # Deprecated: Always be True
@@ -77,14 +78,15 @@
 
         self._readiness_path: str = readiness_path
         self._initial_delay_seconds: int = initial_delay_seconds
         self._min_replicas: int = min_replicas
         self._max_replicas: Optional[int] = max_replicas
         self._target_qps_per_replica: Optional[float] = target_qps_per_replica
         self._post_data: Optional[Dict[str, Any]] = post_data
+        self._readiness_headers: Optional[Dict[str, str]] = readiness_headers
         self._dynamic_ondemand_fallback: Optional[
             bool] = dynamic_ondemand_fallback
         self._base_ondemand_fallback_replicas: Optional[
             int] = base_ondemand_fallback_replicas
         self._upscale_delay_seconds: Optional[int] = upscale_delay_seconds
         self._downscale_delay_seconds: Optional[int] = downscale_delay_seconds
 
@@ -107,32 +109,35 @@
         service_config: Dict[str, Any] = {}
 
         readiness_section = config['readiness_probe']
         if isinstance(readiness_section, str):
             service_config['readiness_path'] = readiness_section
             initial_delay_seconds = None
             post_data = None
+            readiness_headers = None
         else:
             service_config['readiness_path'] = readiness_section['path']
             initial_delay_seconds = readiness_section.get(
                 'initial_delay_seconds', None)
             post_data = readiness_section.get('post_data', None)
+            readiness_headers = readiness_section.get('headers', None)
         if initial_delay_seconds is None:
             initial_delay_seconds = constants.DEFAULT_INITIAL_DELAY_SECONDS
         service_config['initial_delay_seconds'] = initial_delay_seconds
         if isinstance(post_data, str):
             try:
                 post_data = json.loads(post_data)
             except json.JSONDecodeError as e:
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError(
                         'Invalid JSON string for `post_data` in the '
                         '`readiness_probe` section of your service YAML.'
                     ) from e
         service_config['post_data'] = post_data
+        service_config['readiness_headers'] = readiness_headers
 
         policy_section = config.get('replica_policy', None)
         simplified_policy_section = config.get('replicas', None)
         if policy_section is None or simplified_policy_section is not None:
             if simplified_policy_section is not None:
                 min_replicas = simplified_policy_section
             else:
@@ -200,14 +205,15 @@
                         config[section] = dict()
                     config[section][key] = value
 
         add_if_not_none('readiness_probe', 'path', self.readiness_path)
         add_if_not_none('readiness_probe', 'initial_delay_seconds',
                         self.initial_delay_seconds)
         add_if_not_none('readiness_probe', 'post_data', self.post_data)
+        add_if_not_none('readiness_probe', 'headers', self._readiness_headers)
         add_if_not_none('replica_policy', 'min_replicas', self.min_replicas)
         add_if_not_none('replica_policy', 'max_replicas', self.max_replicas)
         add_if_not_none('replica_policy', 'target_qps_per_replica',
                         self.target_qps_per_replica)
         add_if_not_none('replica_policy', 'dynamic_ondemand_fallback',
                         self.dynamic_ondemand_fallback)
         add_if_not_none('replica_policy', 'base_ondemand_fallback_replicas',
@@ -216,16 +222,20 @@
                         self.upscale_delay_seconds)
         add_if_not_none('replica_policy', 'downscale_delay_seconds',
                         self.downscale_delay_seconds)
         return config
 
     def probe_str(self):
         if self.post_data is None:
-            return f'GET {self.readiness_path}'
-        return f'POST {self.readiness_path} {json.dumps(self.post_data)}'
+            method = f'GET {self.readiness_path}'
+        else:
+            method = f'POST {self.readiness_path} {json.dumps(self.post_data)}'
+        headers = ('' if self.readiness_headers is None else
+                   ' with custom headers')
+        return f'{method}{headers}'
 
     def spot_policy_str(self):
         policy_strs = []
         if (self.dynamic_ondemand_fallback is not None and
                 self.dynamic_ondemand_fallback):
             policy_strs.append('Dynamic on-demand fallback')
             if self.base_ondemand_fallback_replicas is not None:
@@ -284,14 +294,18 @@
         return self._target_qps_per_replica
 
     @property
     def post_data(self) -> Optional[Dict[str, Any]]:
         return self._post_data
 
     @property
+    def readiness_headers(self) -> Optional[Dict[str, str]]:
+        return self._readiness_headers
+
+    @property
     def base_ondemand_fallback_replicas(self) -> Optional[int]:
         return self._base_ondemand_fallback_replicas
 
     @property
     def dynamic_ondemand_fallback(self) -> Optional[bool]:
         return self._dynamic_ondemand_fallback
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240521/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240521/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240521/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240521/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/task.py` & `skypilot_nightly-1.0.0.dev20240521/sky/task.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/jobs-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/jobs-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240521/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240521/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240521/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/generate_static_kubeconfig.sh` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/generate_static_kubeconfig.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,21 @@
                         },
                         'post_data': {
                             'anyOf': [{
                                 'type': 'string',
                             }, {
                                 'type': 'object',
                             }]
-                        }
+                        },
+                        'headers': {
+                            'type': 'object',
+                            'additionalProperties': {
+                                'type': 'string'
+                            }
+                        },
                     }
                 }]
             },
             'replica_policy': {
                 'type': 'object',
                 'required': ['min_replicas'],
                 'additionalProperties': False,
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240521/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240520
+Version: 1.0.0.dev20240521
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240521/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_jobs_and_serve.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_jobs_and_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240520/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240521/tests/test_yaml_parser.py`

 * *Files identical despite different names*

