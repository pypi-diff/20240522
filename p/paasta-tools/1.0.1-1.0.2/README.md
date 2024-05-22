# Comparing `tmp/paasta-tools-1.0.1.tar.gz` & `tmp/paasta-tools-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paasta-tools-1.0.1.tar", last modified: Fri May 17 21:20:53 2024, max compression
+gzip compressed data, was "dist/paasta-tools-1.0.2.tar", last modified: Wed May 22 15:04:06 2024, max compression
```

## Comparing `paasta-tools-1.0.1.tar` & `paasta-tools-1.0.2.tar`

### file list

```diff
@@ -1,326 +1,326 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/k8s_itests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/test_autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/k8s_itests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/adhoc_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/api_docs/
--rw-r--r--   0 runner    (1001) docker     (127)    75493 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/api_docs/swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/tweens/request_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/api/views/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/flink.py
--rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/pause_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/api/views/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/apply_external_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/autoscaling_service_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/forecasting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/max_all_k8s_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/pause_service_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/autoscaling/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/bounce_lib.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2042 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/broadcast_log_to_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cassandracluster_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8435 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_autoscaler_max_instances.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_cassandracluster_services_replication.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7211 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_flink_services_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_kubernetes_api.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_kubernetes_services_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7801 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_oom_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_services_replication_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/check_spark_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_crd.py
--rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cleanup_tron_namespaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8426 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/autoscale.py
--rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/cook_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_docker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_image_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/get_latest_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/itest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/list_deploy_queue.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    49329 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/local_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    52420 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    76217 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/mark_for_deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/mesh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/pause_service_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/push_to_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/rollback.py
--rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/security_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    45133 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/spark_run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/start_stop_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)    81205 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/status.py
--rw-r--r--   0 runner    (1001) docker     (127)    39825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/cmds/wait_for_deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/autosuggest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/fsm_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/paasta_tabcomplete.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/adhoc_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autoscaling_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/deploy_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/eks_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/kubernetes_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/rollback_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/service_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/smartstack_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/schemas/tron_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)    36829 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/clusterman.py
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/config_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/contrib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/bounce_log_latency_parser.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/check_manual_oapi_changes.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/check_orphans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/create_dynamodb_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/create_paasta_playground.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/get_running_task_allocation.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/habitat_fixer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/ide_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3861 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/kill_bad_containers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/mass-deploy-tag.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/mock_patch_checker.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17885 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/paasta_update_soa_memcpu.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3959 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/render_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/rightsizer_soaconfigs_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/service_shard_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/service_shard_update.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2480 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/shared_ip_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/contrib/timeouts_metrics_prom.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/delete_kubernetes_deployments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/deployment_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6935 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/docker_wrapper_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/drain_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/dump_locally_running_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/eks_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/envoy_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/firewall_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/flink_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/flinkeks_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/adhoc_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/native_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/native_service_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/frameworks/task_store.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_all_deployments
--rwxr-xr-x   0 runner    (1001) docker     (127)     9674 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_deployments_for_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_services_file.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/generate_services_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/hacheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/instance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/hpa_metrics_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    46810 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/instance/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/iptables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kafkacluster_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/controller_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/application/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5287 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28779 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)   166865 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/kubernetes_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/list_kubernetes_service_instances.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/list_tron_namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/log_task_lifecycle_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/long_running_service_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mac_address.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/marathon_dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/mesos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/master.py
--rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/mesos_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/slave.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos/zookeeper.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31450 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos_maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/mesos_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37790 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/metastatus_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/metrics/metrics_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/monitoring/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/check_k8s_api_performance.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2070 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monitoring_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/monkrelaycluster_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/nrtsearchservice_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/nrtsearchserviceeks_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/oom_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_deploy_tron_jobs
--rwxr-xr-x   0 runner    (1001) docker     (127)     4099 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_execute_docker_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_native_serviceinit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25707 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_remote_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paasta_service_config_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/autoscaler_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/resources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63296 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api/service_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/adhoc_launch_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/autoscaler_count_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue_service_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_cluster_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/float_and_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/hpa_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response200.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response2001.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_bounce_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_mesh_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_adhoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_cassandracluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_flink.py
--rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kafkacluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_tron.py
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/integer_and_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_replica_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model/task_tail_lines.py
--rw-r--r--   0 runner    (1001) docker     (127)    74015 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/paastaapi/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/prune_completed_pods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/puppet_service_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/remote_git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/run-paasta-api-in-dev-mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/run-paasta-api-playground.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_providers/vault.py
--rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/secret_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_istio_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_cr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_crd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4642 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_internal_crd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_kubernetes_job.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    37673 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_prometheus_adapter_config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/setup_tron_namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/slack.py
--rw-r--r--   0 runner    (1001) docker     (127)    25551 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/smartstack_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/spark_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1421 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/synapse_srv_namespaces_fact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools/tron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/tron_command_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron/tron_timeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/tron_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)   141092 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/paasta_tools/vitesscluster_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/paasta_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/requirements-minimal.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:20:53.000000 paasta-tools-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-17 21:20:50.000000 paasta-tools-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/k8s_itests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/k8s_itests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/k8s_itests/test_autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/k8s_itests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/adhoc_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/api/api_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    75493 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/api_docs/swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/api/tweens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/tweens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/tweens/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/tweens/request_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/api/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13390 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/pause_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/api/views/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/apply_external_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/autoscaling_service_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/forecasting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/max_all_k8s_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/pause_service_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/autoscaling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/bounce_lib.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2042 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/broadcast_log_to_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cassandracluster_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8435 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_autoscaler_max_instances.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1140 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_cassandracluster_services_replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7211 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_flink_services_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_kubernetes_api.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_kubernetes_services_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_oom_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9471 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_services_replication_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/check_spark_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_crd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12446 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cleanup_tron_namespaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8426 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/autoscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12968 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/cook_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/get_docker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/get_image_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/get_latest_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/itest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/list_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/list_deploy_queue.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49329 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/local_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52420 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76217 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/mark_for_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/mesh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/pause_service_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/push_to_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13829 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/rollback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19709 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/security_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45133 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/spark_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14600 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/start_stop_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81205 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39825 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/cmds/wait_for_deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/autosuggest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/fsm_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/paasta_tabcomplete.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     6460 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/adhoc_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5570 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/autoscaling_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/autotuned_defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/deploy_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/eks_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39538 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/kubernetes_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/rollback_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/service_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/smartstack_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    26509 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/schemas/tron_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36829 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/clusterman.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/config_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/contrib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2241 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/bounce_log_latency_parser.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      879 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/check_manual_oapi_changes.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/check_orphans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/create_dynamodb_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/create_paasta_playground.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/emit_allocated_cpu_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10918 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/get_running_task_allocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2638 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/habitat_fixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12334 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/ide_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/is_pod_healthy_in_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3861 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/kill_bad_containers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/mass-deploy-tag.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2575 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/mock_patch_checker.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17885 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/paasta_update_soa_memcpu.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3959 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/render_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/rightsizer_soaconfigs_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/service_shard_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/service_shard_update.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2480 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/shared_ip_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/contrib/timeouts_metrics_prom.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/delete_kubernetes_deployments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/deployment_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6935 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/docker_wrapper_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12725 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/drain_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/dump_locally_running_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/eks_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14276 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/envoy_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16304 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/firewall_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/firewall_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/flink_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/flinkeks_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/adhoc_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24535 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/native_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9181 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/native_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/frameworks/task_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      248 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/generate_all_deployments
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9674 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/generate_deployments_for_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4617 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/generate_services_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/generate_services_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/hacheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/instance/hpa_metrics_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46810 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/instance/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/iptables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kafkacluster_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16009 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/application/controller_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/application/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5287 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28779 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166865 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/kubernetes_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3910 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/list_kubernetes_service_instances.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1679 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/list_tron_namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/log_task_lifecycle_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25773 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/long_running_service_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mac_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/marathon_dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/mesos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/master.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5366 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/mesos_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3993 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/slave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos/zookeeper.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31450 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos_maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35540 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/mesos_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/metrics/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37790 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/metrics/metastatus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/metrics/metrics_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/monitoring/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/monitoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/monitoring/check_k8s_api_performance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2070 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/monitoring/kill_orphaned_docker_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24665 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/monitoring_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/monkrelaycluster_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/nrtsearchservice_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/nrtsearchserviceeks_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/oom_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paasta_deploy_tron_jobs
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4099 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paasta_execute_docker_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paasta_native_serviceinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25707 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paasta_remote_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paasta_service_config_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/autoscaler_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20369 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/resources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63296 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api/service_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35200 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/adhoc_launch_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6937 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/autoscaler_count_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7292 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/deploy_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/deploy_queue_service_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7659 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7459 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7825 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_cluster_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7504 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_job_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/float_and_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/hpa_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6555 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_response200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_response2001.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_bounce_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_mesh_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_adhoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_cassandracluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_flink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7036 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kafkacluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12277 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_tron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/integer_and_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6917 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_container_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_replica_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7450 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7241 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7325 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model/task_tail_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74015 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/paastaapi/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/prune_completed_pods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/puppet_service_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/remote_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/run-paasta-api-in-dev-mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/run-paasta-api-playground.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/secret_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/secret_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/secret_providers/vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9060 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/secret_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_istio_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14675 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_kubernetes_cr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_kubernetes_crd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4642 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_kubernetes_internal_crd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12646 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_kubernetes_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37673 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_prometheus_adapter_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5028 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/setup_tron_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/slack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25551 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/smartstack_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8557 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/spark_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1421 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/synapse_srv_namespaces_fact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools/tron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/tron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/tron/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/tron/tron_command_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/tron/tron_timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48900 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/tron_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)   141092 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3897 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/paasta_tools/vitesscluster_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11750 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/paasta_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/requirements-minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:06.000000 paasta-tools-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 15:04:03.000000 paasta-tools-1.0.2/setup.py
```

### Comparing `paasta-tools-1.0.1/README.md` & `paasta-tools-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/k8s_itests/test_autoscaling.py` & `paasta-tools-1.0.2/k8s_itests/test_autoscaling.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/k8s_itests/utils.py` & `paasta-tools-1.0.2/k8s_itests/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/__init__.py` & `paasta-tools-1.0.2/paasta_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 # It is imperative that this file not contain any imports from our
 # dependencies. Since this file is imported from setup.py in the
 # setup phase, the dependencies may not exist on disk yet.
 #
 # Don't bump version manually. See `make release` docs in ./Makefile
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

### Comparing `paasta-tools-1.0.1/paasta_tools/adhoc_tools.py` & `paasta-tools-1.0.2/paasta_tools/adhoc_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/__init__.py` & `paasta-tools-1.0.2/paasta_tools/api/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/api.py` & `paasta-tools-1.0.2/paasta_tools/api/api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/api_docs/swagger.json` & `paasta-tools-1.0.2/paasta_tools/api/api_docs/swagger.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/client.py` & `paasta-tools-1.0.2/paasta_tools/api/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/settings.py` & `paasta-tools-1.0.2/paasta_tools/api/settings.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/tweens/profiling.py` & `paasta-tools-1.0.2/paasta_tools/api/tweens/profiling.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/tweens/request_logger.py` & `paasta-tools-1.0.2/paasta_tools/api/tweens/request_logger.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/__init__.py` & `paasta-tools-1.0.2/paasta_tools/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/autoscaler.py` & `paasta-tools-1.0.2/paasta_tools/api/views/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/exception.py` & `paasta-tools-1.0.2/paasta_tools/api/views/exception.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/flink.py` & `paasta-tools-1.0.2/paasta_tools/api/views/flink.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/instance.py` & `paasta-tools-1.0.2/paasta_tools/api/views/instance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/pause_autoscaler.py` & `paasta-tools-1.0.2/paasta_tools/api/views/pause_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/resources.py` & `paasta-tools-1.0.2/paasta_tools/api/views/resources.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/service.py` & `paasta-tools-1.0.2/paasta_tools/api/views/service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/api/views/version.py` & `paasta-tools-1.0.2/paasta_tools/api/views/version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/apply_external_resources.py` & `paasta-tools-1.0.2/paasta_tools/apply_external_resources.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/async_utils.py` & `paasta-tools-1.0.2/paasta_tools/async_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/autoscaling/autoscaling_service_lib.py` & `paasta-tools-1.0.2/paasta_tools/autoscaling/autoscaling_service_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/autoscaling/forecasting.py` & `paasta-tools-1.0.2/paasta_tools/autoscaling/forecasting.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/autoscaling/max_all_k8s_services.py` & `paasta-tools-1.0.2/paasta_tools/autoscaling/max_all_k8s_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/autoscaling/pause_service_autoscaler.py` & `paasta-tools-1.0.2/paasta_tools/autoscaling/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/autoscaling/utils.py` & `paasta-tools-1.0.2/paasta_tools/autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/bounce_lib.py` & `paasta-tools-1.0.2/paasta_tools/bounce_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/broadcast_log_to_services.py` & `paasta-tools-1.0.2/paasta_tools/broadcast_log_to_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cassandracluster_tools.py` & `paasta-tools-1.0.2/paasta_tools/cassandracluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_autoscaler_max_instances.py` & `paasta-tools-1.0.2/paasta_tools/check_autoscaler_max_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_cassandracluster_services_replication.py` & `paasta-tools-1.0.2/paasta_tools/check_cassandracluster_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_flink_services_health.py` & `paasta-tools-1.0.2/paasta_tools/check_flink_services_health.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_kubernetes_api.py` & `paasta-tools-1.0.2/paasta_tools/check_kubernetes_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_kubernetes_services_replication.py` & `paasta-tools-1.0.2/paasta_tools/check_kubernetes_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_oom_events.py` & `paasta-tools-1.0.2/paasta_tools/check_oom_events.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from paasta_tools.cli.utils import get_instance_config
 from paasta_tools.utils import DEFAULT_SOA_DIR
 from paasta_tools.utils import get_services_for_cluster
 from paasta_tools.utils import load_system_paasta_config
 
 try:
     from scribereader import scribereader
-    from clog.readers import StreamTailerSetupError
+    from scribereader.clog.readers import StreamTailerSetupError
 except ImportError:
     scribereader = None
 
 
 OOM_EVENTS_STREAM = "tmp_paasta_oom_events"
```

### Comparing `paasta-tools-1.0.1/paasta_tools/check_services_replication_tools.py` & `paasta-tools-1.0.2/paasta_tools/check_services_replication_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/check_spark_jobs.py` & `paasta-tools-1.0.2/paasta_tools/check_spark_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_cr.py` & `paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_crd.py` & `paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cleanup_kubernetes_jobs.py` & `paasta-tools-1.0.2/paasta_tools/cleanup_kubernetes_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cleanup_tron_namespaces.py` & `paasta-tools-1.0.2/paasta_tools/cleanup_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/__init__.py` & `paasta-tools-1.0.2/paasta_tools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cli.py` & `paasta-tools-1.0.2/paasta_tools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/__init__.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/autoscale.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/autoscale.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/check.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/cook_image.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/cook_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_docker_image.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/get_docker_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_image_version.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/get_image_version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/get_latest_deployment.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/get_latest_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/info.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/info.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/itest.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/itest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/list.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/list.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/list_clusters.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/list_clusters.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/list_deploy_queue.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/list_deploy_queue.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/local_run.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/local_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/logs.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/logs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/mark_for_deployment.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/mark_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/mesh_status.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/mesh_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/pause_service_autoscaler.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/push_to_registry.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/push_to_registry.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/remote_run.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/rollback.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/rollback.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/secret.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/secret.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/security_check.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/security_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/spark_run.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/spark_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/start_stop_restart.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/start_stop_restart.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/status.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/validate.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/cmds/wait_for_deployment.py` & `paasta-tools-1.0.2/paasta_tools/cli/cmds/wait_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/fsm/__init__.py` & `paasta-tools-1.0.2/paasta_tools/cli/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/fsm/autosuggest.py` & `paasta-tools-1.0.2/paasta_tools/cli/fsm/autosuggest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml` & `paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/kubernetes-PROD.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml` & `paasta-tools-1.0.2/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/fsm_cmd.py` & `paasta-tools-1.0.2/paasta_tools/cli/fsm_cmd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/paasta_tabcomplete.sh` & `paasta-tools-1.0.2/paasta_tools/cli/paasta_tabcomplete.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/adhoc_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/adhoc_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/autoscaling_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/autoscaling_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/autotuned_defaults/cassandracluster_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/autotuned_defaults/kubernetes_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/deploy_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/deploy_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/eks_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/eks_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/kubernetes_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/kubernetes_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/rollback_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/rollback_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/service_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/service_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/smartstack_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/smartstack_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/schemas/tron_schema.json` & `paasta-tools-1.0.2/paasta_tools/cli/schemas/tron_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/cli/utils.py` & `paasta-tools-1.0.2/paasta_tools/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/clusterman.py` & `paasta-tools-1.0.2/paasta_tools/clusterman.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/config_utils.py` & `paasta-tools-1.0.2/paasta_tools/config_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/bounce_log_latency_parser.py` & `paasta-tools-1.0.2/paasta_tools/contrib/bounce_log_latency_parser.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/check_manual_oapi_changes.sh` & `paasta-tools-1.0.2/paasta_tools/contrib/check_manual_oapi_changes.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/check_orphans.py` & `paasta-tools-1.0.2/paasta_tools/contrib/check_orphans.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/create_dynamodb_table.py` & `paasta-tools-1.0.2/paasta_tools/contrib/create_dynamodb_table.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/create_paasta_playground.py` & `paasta-tools-1.0.2/paasta_tools/contrib/create_paasta_playground.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py` & `paasta-tools-1.0.2/paasta_tools/contrib/emit_allocated_cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/get_running_task_allocation.py` & `paasta-tools-1.0.2/paasta_tools/contrib/get_running_task_allocation.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/habitat_fixer.py` & `paasta-tools-1.0.2/paasta_tools/contrib/habitat_fixer.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/ide_helper.py` & `paasta-tools-1.0.2/paasta_tools/contrib/ide_helper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_proxy.py` & `paasta-tools-1.0.2/paasta_tools/contrib/is_pod_healthy_in_proxy.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py` & `paasta-tools-1.0.2/paasta_tools/contrib/is_pod_healthy_in_smartstack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/kill_bad_containers.py` & `paasta-tools-1.0.2/paasta_tools/contrib/kill_bad_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/mass-deploy-tag.sh` & `paasta-tools-1.0.2/paasta_tools/contrib/mass-deploy-tag.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/mock_patch_checker.py` & `paasta-tools-1.0.2/paasta_tools/contrib/mock_patch_checker.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/paasta_update_soa_memcpu.py` & `paasta-tools-1.0.2/paasta_tools/contrib/paasta_update_soa_memcpu.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/render_template.py` & `paasta-tools-1.0.2/paasta_tools/contrib/render_template.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/rightsizer_soaconfigs_update.py` & `paasta-tools-1.0.2/paasta_tools/contrib/rightsizer_soaconfigs_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/service_shard_remove.py` & `paasta-tools-1.0.2/paasta_tools/contrib/service_shard_remove.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/service_shard_update.py` & `paasta-tools-1.0.2/paasta_tools/contrib/service_shard_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/shared_ip_check.py` & `paasta-tools-1.0.2/paasta_tools/contrib/shared_ip_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/contrib/timeouts_metrics_prom.py` & `paasta-tools-1.0.2/paasta_tools/contrib/timeouts_metrics_prom.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/delete_kubernetes_deployments.py` & `paasta-tools-1.0.2/paasta_tools/delete_kubernetes_deployments.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/deployment_utils.py` & `paasta-tools-1.0.2/paasta_tools/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/docker_wrapper.py` & `paasta-tools-1.0.2/paasta_tools/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/docker_wrapper_imports.py` & `paasta-tools-1.0.2/paasta_tools/docker_wrapper_imports.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/drain_lib.py` & `paasta-tools-1.0.2/paasta_tools/drain_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/dump_locally_running_services.py` & `paasta-tools-1.0.2/paasta_tools/dump_locally_running_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/eks_tools.py` & `paasta-tools-1.0.2/paasta_tools/eks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/envoy_tools.py` & `paasta-tools-1.0.2/paasta_tools/envoy_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/firewall.py` & `paasta-tools-1.0.2/paasta_tools/firewall.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/firewall_logging.py` & `paasta-tools-1.0.2/paasta_tools/firewall_logging.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/firewall_update.py` & `paasta-tools-1.0.2/paasta_tools/firewall_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/flink_tools.py` & `paasta-tools-1.0.2/paasta_tools/flink_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/flinkeks_tools.py` & `paasta-tools-1.0.2/paasta_tools/flinkeks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/frameworks/adhoc_scheduler.py` & `paasta-tools-1.0.2/paasta_tools/frameworks/adhoc_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/frameworks/constraints.py` & `paasta-tools-1.0.2/paasta_tools/frameworks/constraints.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/frameworks/native_scheduler.py` & `paasta-tools-1.0.2/paasta_tools/frameworks/native_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/frameworks/native_service_config.py` & `paasta-tools-1.0.2/paasta_tools/frameworks/native_service_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/frameworks/task_store.py` & `paasta-tools-1.0.2/paasta_tools/frameworks/task_store.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/generate_deployments_for_service.py` & `paasta-tools-1.0.2/paasta_tools/generate_deployments_for_service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/generate_services_file.py` & `paasta-tools-1.0.2/paasta_tools/generate_services_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/generate_services_yaml.py` & `paasta-tools-1.0.2/paasta_tools/generate_services_yaml.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/hacheck.py` & `paasta-tools-1.0.2/paasta_tools/hacheck.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/instance/hpa_metrics_parser.py` & `paasta-tools-1.0.2/paasta_tools/instance/hpa_metrics_parser.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/instance/kubernetes.py` & `paasta-tools-1.0.2/paasta_tools/instance/kubernetes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/iptables.py` & `paasta-tools-1.0.2/paasta_tools/iptables.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kafkacluster_tools.py` & `paasta-tools-1.0.2/paasta_tools/kafkacluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes/application/controller_wrappers.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes/application/controller_wrappers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes/application/tools.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes/application/tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes/bin/paasta_secrets_sync.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/kubernetes_tools.py` & `paasta-tools-1.0.2/paasta_tools/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/list_kubernetes_service_instances.py` & `paasta-tools-1.0.2/paasta_tools/list_kubernetes_service_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/list_tron_namespaces.py` & `paasta-tools-1.0.2/paasta_tools/list_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/log_task_lifecycle_events.py` & `paasta-tools-1.0.2/paasta_tools/log_task_lifecycle_events.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/long_running_service_tools.py` & `paasta-tools-1.0.2/paasta_tools/long_running_service_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mac_address.py` & `paasta-tools-1.0.2/paasta_tools/mac_address.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/cfg.py` & `paasta-tools-1.0.2/paasta_tools/mesos/cfg.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/cluster.py` & `paasta-tools-1.0.2/paasta_tools/mesos/cluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/exceptions.py` & `paasta-tools-1.0.2/paasta_tools/mesos/exceptions.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/framework.py` & `paasta-tools-1.0.2/paasta_tools/mesos/framework.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/log.py` & `paasta-tools-1.0.2/paasta_tools/mesos/log.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/master.py` & `paasta-tools-1.0.2/paasta_tools/mesos/master.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/mesos_file.py` & `paasta-tools-1.0.2/paasta_tools/mesos/mesos_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/parallel.py` & `paasta-tools-1.0.2/paasta_tools/mesos/parallel.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/slave.py` & `paasta-tools-1.0.2/paasta_tools/mesos/slave.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/task.py` & `paasta-tools-1.0.2/paasta_tools/mesos/task.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/util.py` & `paasta-tools-1.0.2/paasta_tools/mesos/util.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos/zookeeper.py` & `paasta-tools-1.0.2/paasta_tools/mesos/zookeeper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos_maintenance.py` & `paasta-tools-1.0.2/paasta_tools/mesos_maintenance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/mesos_tools.py` & `paasta-tools-1.0.2/paasta_tools/mesos_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/metrics/metastatus_lib.py` & `paasta-tools-1.0.2/paasta_tools/metrics/metastatus_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/metrics/metrics_lib.py` & `paasta-tools-1.0.2/paasta_tools/metrics/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/monitoring/__init__.py` & `paasta-tools-1.0.2/paasta_tools/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/monitoring/check_k8s_api_performance.py` & `paasta-tools-1.0.2/paasta_tools/monitoring/check_k8s_api_performance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py` & `paasta-tools-1.0.2/paasta_tools/monitoring/kill_orphaned_docker_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/monitoring_tools.py` & `paasta-tools-1.0.2/paasta_tools/monitoring_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/monkrelaycluster_tools.py` & `paasta-tools-1.0.2/paasta_tools/monkrelaycluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/nrtsearchservice_tools.py` & `paasta-tools-1.0.2/paasta_tools/nrtsearchservice_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/nrtsearchserviceeks_tools.py` & `paasta-tools-1.0.2/paasta_tools/nrtsearchserviceeks_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/oom_logger.py` & `paasta-tools-1.0.2/paasta_tools/oom_logger.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paasta_execute_docker_command.py` & `paasta-tools-1.0.2/paasta_tools/paasta_execute_docker_command.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paasta_native_serviceinit.py` & `paasta-tools-1.0.2/paasta_tools/paasta_native_serviceinit.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paasta_remote_run.py` & `paasta-tools-1.0.2/paasta_tools/paasta_remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paasta_service_config_loader.py` & `paasta-tools-1.0.2/paasta_tools/paasta_service_config_loader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/__init__.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/api/autoscaler_api.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/api/autoscaler_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/api/default_api.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/api/default_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/api/resources_api.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/api/resources_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/api/service_api.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/api/service_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/api_client.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/api_client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/apis/__init__.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/configuration.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/configuration.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/exceptions.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/adhoc_launch_history.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/adhoc_launch_history.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/autoscaler_count_msg.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/autoscaler_count_msg.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/deploy_queue.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/deploy_queue_service_instance.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/deploy_queue_service_instance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_backend.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_backend.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_location.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_location.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/envoy_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/envoy_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_cluster_overview.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_cluster_overview.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_config.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_job_details.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_job_details.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/flink_jobs.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/flink_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/float_and_error.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/float_and_error.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/hpa_metric.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/hpa_metric.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_object.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response200.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_response200.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/inline_response2001.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_bounce_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_bounce_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_mesh_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_mesh_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_adhoc.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_adhoc.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_cassandracluster.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_cassandracluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_flink.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_flink.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kafkacluster.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kafkacluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes_autoscaling_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_kubernetes_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_status_tron.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_status_tron.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/instance_tasks.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/instance_tasks.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/integer_and_error.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/integer_and_error.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_container.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_container_v2.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_container_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_healthcheck.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_healthcheck.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_event.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod_event.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_pod_v2.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_pod_v2.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_replica_set.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_replica_set.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/kubernetes_version.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_item.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource_item.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/resource_value.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/resource_value.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_backend.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_backend.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_location.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_location.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/smartstack_status.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/smartstack_status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model/task_tail_lines.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model/task_tail_lines.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/model_utils.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/model_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/models/__init__.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/paastaapi/rest.py` & `paasta-tools-1.0.2/paasta_tools/paastaapi/rest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/prune_completed_pods.py` & `paasta-tools-1.0.2/paasta_tools/prune_completed_pods.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/puppet_service_tools.py` & `paasta-tools-1.0.2/paasta_tools/puppet_service_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/remote_git.py` & `paasta-tools-1.0.2/paasta_tools/remote_git.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/run-paasta-api-in-dev-mode.py` & `paasta-tools-1.0.2/paasta_tools/run-paasta-api-in-dev-mode.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/run-paasta-api-playground.py` & `paasta-tools-1.0.2/paasta_tools/run-paasta-api-playground.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/secret_providers/__init__.py` & `paasta-tools-1.0.2/paasta_tools/secret_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/secret_providers/vault.py` & `paasta-tools-1.0.2/paasta_tools/secret_providers/vault.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/secret_tools.py` & `paasta-tools-1.0.2/paasta_tools/secret_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_istio_mesh.py` & `paasta-tools-1.0.2/paasta_tools/setup_istio_mesh.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_cr.py` & `paasta-tools-1.0.2/paasta_tools/setup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_crd.py` & `paasta-tools-1.0.2/paasta_tools/setup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_internal_crd.py` & `paasta-tools-1.0.2/paasta_tools/setup_kubernetes_internal_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_kubernetes_job.py` & `paasta-tools-1.0.2/paasta_tools/setup_kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_prometheus_adapter_config.py` & `paasta-tools-1.0.2/paasta_tools/setup_prometheus_adapter_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/setup_tron_namespace.py` & `paasta-tools-1.0.2/paasta_tools/setup_tron_namespace.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/slack.py` & `paasta-tools-1.0.2/paasta_tools/slack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/smartstack_tools.py` & `paasta-tools-1.0.2/paasta_tools/smartstack_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/spark_tools.py` & `paasta-tools-1.0.2/paasta_tools/spark_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/synapse_srv_namespaces_fact.py` & `paasta-tools-1.0.2/paasta_tools/synapse_srv_namespaces_fact.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/tron/client.py` & `paasta-tools-1.0.2/paasta_tools/tron/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/tron/tron_command_context.py` & `paasta-tools-1.0.2/paasta_tools/tron/tron_command_context.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/tron/tron_timeutils.py` & `paasta-tools-1.0.2/paasta_tools/tron/tron_timeutils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/tron_tools.py` & `paasta-tools-1.0.2/paasta_tools/tron_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/utils.py` & `paasta-tools-1.0.2/paasta_tools/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools/vitesscluster_tools.py` & `paasta-tools-1.0.2/paasta_tools/vitesscluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools.egg-info/SOURCES.txt` & `paasta-tools-1.0.2/paasta_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools.egg-info/entry_points.txt` & `paasta-tools-1.0.2/paasta_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-1.0.1/paasta_tools.egg-info/requires.txt` & `paasta-tools-1.0.2/paasta_tools.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 pysensu-yelp>=0.3.4
 PyStaticConfiguration
 python-crontab>=2.1.1
 python-dateutil>=2.4.0
 python-iptables
 pytimeparse>=1.1.0
 pytz>=2014.10
-requests>=2.18.4
+requests<2.32.0,>=2.18.4
 requests-cache>=0.4.10
 retry
 ruamel.yaml
 sensu-plugin
 service-configuration-lib>=2.18.17
 signalfx
 slackclient>=1.2.1
```

### Comparing `paasta-tools-1.0.1/requirements-minimal.txt` & `paasta-tools-1.0.2/requirements-minimal.txt`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,17 @@
 pysensu-yelp >= 0.3.4
 PyStaticConfiguration
 python-crontab>=2.1.1
 python-dateutil >= 2.4.0
 python-iptables
 pytimeparse >= 1.1.0
 pytz >= 2014.10
-requests >= 2.18.4
+# the upper-bound is required for older docker-py (<=7.0.0)
+# to function: https://github.com/psf/requests/issues/6707
+requests >= 2.18.4, <2.32.0
 requests-cache >= 0.4.10
 retry
 ruamel.yaml
 sensu-plugin
 service-configuration-lib >= 2.18.17
 signalfx
 slackclient >= 1.2.1
```

### Comparing `paasta-tools-1.0.1/setup.py` & `paasta-tools-1.0.2/setup.py`

 * *Files identical despite different names*

