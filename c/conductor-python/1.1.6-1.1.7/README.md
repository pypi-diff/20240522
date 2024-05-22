# Comparing `tmp/conductor_python-1.1.6.tar.gz` & `tmp/conductor_python-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conductor_python-1.1.6.tar", last modified: Sun May 19 23:41:48 2024, max compression
+gzip compressed data, was "conductor_python-1.1.7.tar", last modified: Wed May 22 18:05:30 2024, max compression
```

## Comparing `conductor_python-1.1.6.tar` & `conductor_python-1.1.7.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.407451 conductor_python-1.1.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-05-19 23:41:30.000000 conductor_python-1.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)    10086 2024-05-19 23:41:48.407451 conductor_python-1.1.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9065 2024-05-19 23:41:30.000000 conductor_python-1.1.6/README.md
--rw-r--r--   0 root         (0) root         (0)     1018 2024-05-19 23:41:48.407451 conductor_python-1.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-19 23:41:30.000000 conductor_python-1.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.347450 conductor_python-1.1.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.351450 conductor_python-1.1.6/src/conductor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.351450 conductor_python-1.1.6/src/conductor/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.355450 conductor_python-1.1.6/src/conductor/client/ai/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/ai/configuration.py
--rw-r--r--   0 root         (0) root         (0)     2146 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/ai/integrations.py
--rw-r--r--   0 root         (0) root         (0)     5220 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/ai/orchestrator.py
--rw-r--r--   0 root         (0) root         (0)     4557 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/authorization_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.355450 conductor_python-1.1.6/src/conductor/client/automator/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/automator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8168 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/automator/task_handler.py
--rw-r--r--   0 root         (0) root         (0)    11409 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/automator/task_runner.py
--rw-r--r--   0 root         (0) root         (0)     4089 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/automator/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.355450 conductor_python-1.1.6/src/conductor/client/configuration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4489 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/configuration/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.355450 conductor_python-1.1.6/src/conductor/client/configuration/settings/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/configuration/settings/__init__.py
--rw-r--r--   0 root         (0) root         (0)      150 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/configuration/settings/authentication_settings.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/configuration/settings/metrics_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.355450 conductor_python-1.1.6/src/conductor/client/event/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1250 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/event_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.359450 conductor_python-1.1.6/src/conductor/client/event/queue/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/queue/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1339 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/queue/kafka_queue_configuration.py
--rw-r--r--   0 root         (0) root         (0)      851 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/queue/queue_configuration.py
--rw-r--r--   0 root         (0) root         (0)      192 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/event/queue/queue_worker_configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.359450 conductor_python-1.1.6/src/conductor/client/exceptions/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/exceptions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      446 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/exceptions/api_error.py
--rw-r--r--   0 root         (0) root         (0)     1616 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/exceptions/api_exception_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.359450 conductor_python-1.1.6/src/conductor/client/helpers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/helpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6554 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/helpers/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.359450 conductor_python-1.1.6/src/conductor/client/http/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.367450 conductor_python-1.1.6/src/conductor/client/http/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53352 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/application_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    11819 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/authorization_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    33405 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/event_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    29299 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/group_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    90712 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/integration_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    47915 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/metadata_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    30772 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/prompt_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    53765 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/scheduler_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    35501 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/secret_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    66289 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/task_resource_api.py
--rw-r--r--   0 root         (0) root         (0)     7141 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/token_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    17899 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/user_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    19200 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/workflow_bulk_resource_api.py
--rw-r--r--   0 root         (0) root         (0)   123243 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api/workflow_resource_api.py
--rw-r--r--   0 root         (0) root         (0)    28954 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.383450 conductor_python-1.1.6/src/conductor/client/http/models/
--rw-r--r--   0 root         (0) root         (0)     4057 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/action.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/authorization_request.py
--rw-r--r--   0 root         (0) root         (0)     4031 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/bulk_response.py
--rw-r--r--   0 root         (0) root         (0)     4108 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/conductor_application.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/conductor_user.py
--rw-r--r--   0 root         (0) root         (0)     3869 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/correlation_ids_search_request.py
--rw-r--r--   0 root         (0) root         (0)     2971 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/create_or_update_application_request.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/event_handler.py
--rw-r--r--   0 root         (0) root         (0)     3436 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/external_storage_location.py
--rw-r--r--   0 root         (0) root         (0)     3502 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/generate_token_request.py
--rw-r--r--   0 root         (0) root         (0)     3930 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/group.py
--rw-r--r--   0 root         (0) root         (0)     4149 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/health.py
--rw-r--r--   0 root         (0) root         (0)     4715 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/health_check_status.py
--rw-r--r--   0 root         (0) root         (0)    10565 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/integration.py
--rw-r--r--   0 root         (0) root         (0)     9075 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/integration_api.py
--rw-r--r--   0 root         (0) root         (0)     4454 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/integration_api_update.py
--rw-r--r--   0 root         (0) root         (0)     8468 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/integration_def.py
--rw-r--r--   0 root         (0) root         (0)     5993 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/integration_update.py
--rw-r--r--   0 root         (0) root         (0)     2731 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/permission.py
--rw-r--r--   0 root         (0) root         (0)     4854 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/poll_data.py
--rw-r--r--   0 root         (0) root         (0)     9073 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/prompt_template.py
--rw-r--r--   0 root         (0) root         (0)     7450 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/prompt_test_request.py
--rw-r--r--   0 root         (0) root         (0)     3706 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/rate_limit.py
--rw-r--r--   0 root         (0) root         (0)     6537 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/rerun_workflow_request.py
--rw-r--r--   0 root         (0) root         (0)     2156 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/response.py
--rw-r--r--   0 root         (0) root         (0)     3407 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/role.py
--rw-r--r--   0 root         (0) root         (0)     9583 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/save_schedule_request.py
--rw-r--r--   0 root         (0) root         (0)     3817 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     3572 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/search_result_task.py
--rw-r--r--   0 root         (0) root         (0)     3677 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/search_result_task_summary.py
--rw-r--r--   0 root         (0) root         (0)     3632 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow.py
--rw-r--r--   0 root         (0) root         (0)     3962 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py
--rw-r--r--   0 root         (0) root         (0)     3737 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     3702 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/skip_task_request.py
--rw-r--r--   0 root         (0) root         (0)     5631 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/start_workflow.py
--rw-r--r--   0 root         (0) root         (0)    10467 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/start_workflow_request.py
--rw-r--r--   0 root         (0) root         (0)     1953 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/state_change_event.py
--rw-r--r--   0 root         (0) root         (0)     5158 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/sub_workflow_params.py
--rw-r--r--   0 root         (0) root         (0)     3718 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/subject_ref.py
--rw-r--r--   0 root         (0) root         (0)     4157 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/tag_object.py
--rw-r--r--   0 root         (0) root         (0)     4148 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/tag_string.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/target_ref.py
--rw-r--r--   0 root         (0) root         (0)    34938 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task.py
--rw-r--r--   0 root         (0) root         (0)    21491 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_def.py
--rw-r--r--   0 root         (0) root         (0)     4916 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_details.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_exec_log.py
--rw-r--r--   0 root         (0) root         (0)    10711 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_result.py
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_result_status.py
--rw-r--r--   0 root         (0) root         (0)    17342 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/task_summary.py
--rw-r--r--   0 root         (0) root         (0)      407 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/token.py
--rw-r--r--   0 root         (0) root         (0)     4101 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/upsert_group_request.py
--rw-r--r--   0 root         (0) root         (0)     4697 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/upsert_user_request.py
--rw-r--r--   0 root         (0) root         (0)    25837 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow.py
--rw-r--r--   0 root         (0) root         (0)    17948 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_def.py
--rw-r--r--   0 root         (0) root         (0)    12696 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_run.py
--rw-r--r--   0 root         (0) root         (0)    11026 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_schedule.py
--rw-r--r--   0 root         (0) root         (0)    10715 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_schedule_execution_model.py
--rw-r--r--   0 root         (0) root         (0)     4769 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_state_update.py
--rw-r--r--   0 root         (0) root         (0)     6730 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_status.py
--rw-r--r--   0 root         (0) root         (0)    18136 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_summary.py
--rw-r--r--   0 root         (0) root         (0)     2876 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_tag.py
--rw-r--r--   0 root         (0) root         (0)    27934 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_task.py
--rw-r--r--   0 root         (0) root         (0)    11477 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/models/workflow_test_request.py
--rw-r--r--   0 root         (0) root         (0)    10231 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/rest.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/http/thread.py
--rw-r--r--   0 root         (0) root         (0)     3695 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/integration_client.py
--rw-r--r--   0 root         (0) root         (0)     1724 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/metadata_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.387450 conductor_python-1.1.6/src/conductor/client/orkes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.387450 conductor_python-1.1.6/src/conductor/client/orkes/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35385 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/api/tags_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.391450 conductor_python-1.1.6/src/conductor/client/orkes/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/access_key.py
--rw-r--r--   0 root         (0) root         (0)      107 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/access_key_status.py
--rw-r--r--   0 root         (0) root         (0)      165 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/access_type.py
--rw-r--r--   0 root         (0) root         (0)     1409 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/created_access_key.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/granted_permission.py
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/metadata_tag.py
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/models/ratelimit_tag.py
--rw-r--r--   0 root         (0) root         (0)     8561 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_authorization_client.py
--rw-r--r--   0 root         (0) root         (0)     2142 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_base_client.py
--rw-r--r--   0 root         (0) root         (0)     3740 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_integration_client.py
--rw-r--r--   0 root         (0) root         (0)     4173 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_metadata_client.py
--rw-r--r--   0 root         (0) root         (0)     2525 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_prompt_client.py
--rw-r--r--   0 root         (0) root         (0)     4009 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)     1529 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_secret_client.py
--rw-r--r--   0 root         (0) root         (0)     3512 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_task_client.py
--rw-r--r--   0 root         (0) root         (0)     7986 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes/orkes_workflow_client.py
--rw-r--r--   0 root         (0) root         (0)     2441 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/orkes_clients.py
--rw-r--r--   0 root         (0) root         (0)     1371 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/prompt_client.py
--rw-r--r--   0 root         (0) root         (0)     2535 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/scheduler_client.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/secret_client.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/task_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.391450 conductor_python-1.1.6/src/conductor/client/telemetry/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9334 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/metrics_collector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.391450 conductor_python-1.1.6/src/conductor/client/telemetry/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/model/metric_documentation.py
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/model/metric_label.py
--rw-r--r--   0 root         (0) root         (0)      716 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/telemetry/model/metric_name.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.391450 conductor_python-1.1.6/src/conductor/client/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/worker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      120 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/worker/exception.py
--rw-r--r--   0 root         (0) root         (0)     5965 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/worker/worker.py
--rw-r--r--   0 root         (0) root         (0)     3492 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/worker/worker_interface.py
--rw-r--r--   0 root         (0) root         (0)     1894 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/worker/worker_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.391450 conductor_python-1.1.6/src/conductor/client/workflow/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15584 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/conductor_workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.395450 conductor_python-1.1.6/src/conductor/client/workflow/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10637 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/executor/workflow_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.399450 conductor_python-1.1.6/src/conductor/client/workflow/task/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2128 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/do_while_task.py
--rw-r--r--   0 root         (0) root         (0)     1402 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/dynamic_fork_task.py
--rw-r--r--   0 root         (0) root         (0)      840 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/dynamic_task.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/event_task.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/fork_task.py
--rw-r--r--   0 root         (0) root         (0)      565 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/get_document.py
--rw-r--r--   0 root         (0) root         (0)     2725 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/http_poll_task.py
--rw-r--r--   0 root         (0) root         (0)     2828 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/http_task.py
--rw-r--r--   0 root         (0) root         (0)     1476 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/human_task.py
--rw-r--r--   0 root         (0) root         (0)      626 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/inline.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/javascript_task.py
--rw-r--r--   0 root         (0) root         (0)      863 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/join_task.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/json_jq_task.py
--rw-r--r--   0 root         (0) root         (0)      608 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/kafka_publish.py
--rw-r--r--   0 root         (0) root         (0)      876 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/kafka_publish_input.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.403450 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1832 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py
--rw-r--r--   0 root         (0) root         (0)      727 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     2670 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py
--rw-r--r--   0 root         (0) root         (0)     2037 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py
--rw-r--r--   0 root         (0) root         (0)      834 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py
--rw-r--r--   0 root         (0) root         (0)     1668 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.403450 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py
--rw-r--r--   0 root         (0) root         (0)      647 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py
--rw-r--r--   0 root         (0) root         (0)      379 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/set_variable_task.py
--rw-r--r--   0 root         (0) root         (0)      695 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/simple_task.py
--rw-r--r--   0 root         (0) root         (0)      890 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/start_workflow_task.py
--rw-r--r--   0 root         (0) root         (0)     1994 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/sub_workflow_task.py
--rw-r--r--   0 root         (0) root         (0)     2325 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/switch_task.py
--rw-r--r--   0 root         (0) root         (0)     6107 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/task.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/task_type.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/terminate_task.py
--rw-r--r--   0 root         (0) root         (0)      126 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/timeout_policy.py
--rw-r--r--   0 root         (0) root         (0)     1468 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/wait_for_webhook_task.py
--rw-r--r--   0 root         (0) root         (0)     1536 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow/task/wait_task.py
--rw-r--r--   0 root         (0) root         (0)     3731 2024-05-19 23:41:30.000000 conductor_python-1.1.6/src/conductor/client/workflow_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 23:41:48.403450 conductor_python-1.1.6/src/conductor_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10086 2024-05-19 23:41:48.000000 conductor_python-1.1.6/src/conductor_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10042 2024-05-19 23:41:48.000000 conductor_python-1.1.6/src/conductor_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 23:41:48.000000 conductor_python-1.1.6/src/conductor_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2024-05-19 23:41:48.000000 conductor_python-1.1.6/src/conductor_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-19 23:41:48.000000 conductor_python-1.1.6/src/conductor_python.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.728948 conductor_python-1.1.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-22 18:05:10.000000 conductor_python-1.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    10086 2024-05-22 18:05:30.728948 conductor_python-1.1.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9065 2024-05-22 18:05:10.000000 conductor_python-1.1.7/README.md
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-05-22 18:05:30.728948 conductor_python-1.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-22 18:05:10.000000 conductor_python-1.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.672949 conductor_python-1.1.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.672949 conductor_python-1.1.7/src/conductor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.676949 conductor_python-1.1.7/src/conductor/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.676949 conductor_python-1.1.7/src/conductor/client/ai/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/ai/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/ai/integrations.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/ai/orchestrator.py
+-rw-r--r--   0 root         (0) root         (0)     4557 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/authorization_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.676949 conductor_python-1.1.7/src/conductor/client/automator/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/automator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/automator/task_handler.py
+-rw-r--r--   0 root         (0) root         (0)    11409 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/automator/task_runner.py
+-rw-r--r--   0 root         (0) root         (0)     4089 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/automator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.680949 conductor_python-1.1.7/src/conductor/client/configuration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4489 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/configuration/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.680949 conductor_python-1.1.7/src/conductor/client/configuration/settings/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/configuration/settings/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      150 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/configuration/settings/authentication_settings.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/configuration/settings/metrics_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.680949 conductor_python-1.1.7/src/conductor/client/event/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/event_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.680949 conductor_python-1.1.7/src/conductor/client/event/queue/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/queue/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/queue/kafka_queue_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      851 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/queue/queue_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      192 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/event/queue/queue_worker_configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.680949 conductor_python-1.1.7/src/conductor/client/exceptions/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/exceptions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      446 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/exceptions/api_error.py
+-rw-r--r--   0 root         (0) root         (0)     1616 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/exceptions/api_exception_handler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.684949 conductor_python-1.1.7/src/conductor/client/helpers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/helpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6554 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/helpers/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.684949 conductor_python-1.1.7/src/conductor/client/http/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.688949 conductor_python-1.1.7/src/conductor/client/http/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53352 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/application_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    11819 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/authorization_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    33405 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/event_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    29299 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/group_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    90712 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/integration_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    47915 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/metadata_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    30772 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/prompt_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    53765 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/scheduler_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    35501 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/secret_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    66289 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/task_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)     7141 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/token_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    17899 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/user_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    19200 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/workflow_bulk_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)   123243 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api/workflow_resource_api.py
+-rw-r--r--   0 root         (0) root         (0)    28954 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.708948 conductor_python-1.1.7/src/conductor/client/http/models/
+-rw-r--r--   0 root         (0) root         (0)     4057 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/action.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/authorization_request.py
+-rw-r--r--   0 root         (0) root         (0)     4031 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/bulk_response.py
+-rw-r--r--   0 root         (0) root         (0)     4108 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/conductor_application.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/conductor_user.py
+-rw-r--r--   0 root         (0) root         (0)     3869 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/correlation_ids_search_request.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/create_or_update_application_request.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/event_handler.py
+-rw-r--r--   0 root         (0) root         (0)     3436 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/external_storage_location.py
+-rw-r--r--   0 root         (0) root         (0)     3502 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/generate_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/group.py
+-rw-r--r--   0 root         (0) root         (0)     4149 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/health.py
+-rw-r--r--   0 root         (0) root         (0)     4715 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/health_check_status.py
+-rw-r--r--   0 root         (0) root         (0)    10565 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/integration.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/integration_api.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/integration_api_update.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/integration_def.py
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/integration_update.py
+-rw-r--r--   0 root         (0) root         (0)     2731 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)     4854 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/poll_data.py
+-rw-r--r--   0 root         (0) root         (0)     9073 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/prompt_template.py
+-rw-r--r--   0 root         (0) root         (0)     7450 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/prompt_test_request.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/rate_limit.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/rerun_workflow_request.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/response.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/role.py
+-rw-r--r--   0 root         (0) root         (0)     9583 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/save_schedule_request.py
+-rw-r--r--   0 root         (0) root         (0)     3817 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/search_result_task.py
+-rw-r--r--   0 root         (0) root         (0)     3677 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/search_result_task_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow.py
+-rw-r--r--   0 root         (0) root         (0)     3962 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3702 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/skip_task_request.py
+-rw-r--r--   0 root         (0) root         (0)     5631 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/start_workflow.py
+-rw-r--r--   0 root         (0) root         (0)    10467 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/start_workflow_request.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/state_change_event.py
+-rw-r--r--   0 root         (0) root         (0)     5158 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/sub_workflow_params.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/subject_ref.py
+-rw-r--r--   0 root         (0) root         (0)     4157 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/tag_object.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/tag_string.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/target_ref.py
+-rw-r--r--   0 root         (0) root         (0)    34938 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task.py
+-rw-r--r--   0 root         (0) root         (0)    21491 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_def.py
+-rw-r--r--   0 root         (0) root         (0)     4916 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_details.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_exec_log.py
+-rw-r--r--   0 root         (0) root         (0)    10711 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_result.py
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_result_status.py
+-rw-r--r--   0 root         (0) root         (0)    17342 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/task_summary.py
+-rw-r--r--   0 root         (0) root         (0)      407 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/token.py
+-rw-r--r--   0 root         (0) root         (0)     4101 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/upsert_group_request.py
+-rw-r--r--   0 root         (0) root         (0)     4697 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/upsert_user_request.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow.py
+-rw-r--r--   0 root         (0) root         (0)    18612 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_def.py
+-rw-r--r--   0 root         (0) root         (0)    12696 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_run.py
+-rw-r--r--   0 root         (0) root         (0)    11026 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_schedule.py
+-rw-r--r--   0 root         (0) root         (0)    10715 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_schedule_execution_model.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_state_update.py
+-rw-r--r--   0 root         (0) root         (0)     6730 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_status.py
+-rw-r--r--   0 root         (0) root         (0)    18136 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_tag.py
+-rw-r--r--   0 root         (0) root         (0)    27934 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)    11477 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/models/workflow_test_request.py
+-rw-r--r--   0 root         (0) root         (0)    10348 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/rest.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/http/thread.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/integration_client.py
+-rw-r--r--   0 root         (0) root         (0)     1724 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/metadata_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.708948 conductor_python-1.1.7/src/conductor/client/orkes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.708948 conductor_python-1.1.7/src/conductor/client/orkes/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35385 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/api/tags_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.712949 conductor_python-1.1.7/src/conductor/client/orkes/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/access_key.py
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/access_key_status.py
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/access_type.py
+-rw-r--r--   0 root         (0) root         (0)     1409 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/created_access_key.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/granted_permission.py
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/metadata_tag.py
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/models/ratelimit_tag.py
+-rw-r--r--   0 root         (0) root         (0)     8561 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_authorization_client.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_base_client.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_integration_client.py
+-rw-r--r--   0 root         (0) root         (0)     4173 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_metadata_client.py
+-rw-r--r--   0 root         (0) root         (0)     2525 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_prompt_client.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)     1529 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_secret_client.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_task_client.py
+-rw-r--r--   0 root         (0) root         (0)     7986 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes/orkes_workflow_client.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/orkes_clients.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/prompt_client.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/scheduler_client.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/secret_client.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/task_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.712949 conductor_python-1.1.7/src/conductor/client/telemetry/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9334 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/metrics_collector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.712949 conductor_python-1.1.7/src/conductor/client/telemetry/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/model/metric_documentation.py
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/model/metric_label.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/telemetry/model/metric_name.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.716949 conductor_python-1.1.7/src/conductor/client/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/worker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      120 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/worker/exception.py
+-rw-r--r--   0 root         (0) root         (0)     5965 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/worker/worker.py
+-rw-r--r--   0 root         (0) root         (0)     3492 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/worker/worker_interface.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/worker/worker_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.716949 conductor_python-1.1.7/src/conductor/client/workflow/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16181 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/conductor_workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.716949 conductor_python-1.1.7/src/conductor/client/workflow/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10637 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/executor/workflow_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.724949 conductor_python-1.1.7/src/conductor/client/workflow/task/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2128 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/do_while_task.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/dynamic_fork_task.py
+-rw-r--r--   0 root         (0) root         (0)      840 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/dynamic_task.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/event_task.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/fork_task.py
+-rw-r--r--   0 root         (0) root         (0)      565 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/get_document.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/http_poll_task.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/http_task.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/human_task.py
+-rw-r--r--   0 root         (0) root         (0)      626 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/inline.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/javascript_task.py
+-rw-r--r--   0 root         (0) root         (0)      863 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/join_task.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/json_jq_task.py
+-rw-r--r--   0 root         (0) root         (0)      608 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/kafka_publish.py
+-rw-r--r--   0 root         (0) root         (0)      876 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/kafka_publish_input.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.724949 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1832 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py
+-rw-r--r--   0 root         (0) root         (0)      727 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     2670 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py
+-rw-r--r--   0 root         (0) root         (0)      834 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.724949 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py
+-rw-r--r--   0 root         (0) root         (0)      647 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py
+-rw-r--r--   0 root         (0) root         (0)      379 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/set_variable_task.py
+-rw-r--r--   0 root         (0) root         (0)      695 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/simple_task.py
+-rw-r--r--   0 root         (0) root         (0)      890 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/start_workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)     1994 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/sub_workflow_task.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/switch_task.py
+-rw-r--r--   0 root         (0) root         (0)     6107 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/task.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/task_type.py
+-rw-r--r--   0 root         (0) root         (0)      792 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/terminate_task.py
+-rw-r--r--   0 root         (0) root         (0)      126 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/timeout_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1468 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/wait_for_webhook_task.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow/task/wait_task.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2024-05-22 18:05:10.000000 conductor_python-1.1.7/src/conductor/client/workflow_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 18:05:30.728948 conductor_python-1.1.7/src/conductor_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10086 2024-05-22 18:05:30.000000 conductor_python-1.1.7/src/conductor_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10042 2024-05-22 18:05:30.000000 conductor_python-1.1.7/src/conductor_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 18:05:30.000000 conductor_python-1.1.7/src/conductor_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2024-05-22 18:05:30.000000 conductor_python-1.1.7/src/conductor_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 18:05:30.000000 conductor_python-1.1.7/src/conductor_python.egg-info/top_level.txt
```

### Comparing `conductor_python-1.1.6/LICENSE` & `conductor_python-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/PKG-INFO` & `conductor_python-1.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Netflix Conductor Python SDK
 Home-page: https://github.com/conductor-sdk/conductor-python
 Author: Orkes
 Author-email: developers@orkes.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `conductor_python-1.1.6/README.md` & `conductor_python-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/setup.cfg` & `conductor_python-1.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/ai/integrations.py` & `conductor_python-1.1.7/src/conductor/client/ai/integrations.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/ai/orchestrator.py` & `conductor_python-1.1.7/src/conductor/client/ai/orchestrator.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/authorization_client.py` & `conductor_python-1.1.7/src/conductor/client/authorization_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/automator/task_handler.py` & `conductor_python-1.1.7/src/conductor/client/automator/task_handler.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/automator/task_runner.py` & `conductor_python-1.1.7/src/conductor/client/automator/task_runner.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/automator/utils.py` & `conductor_python-1.1.7/src/conductor/client/automator/utils.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/configuration/configuration.py` & `conductor_python-1.1.7/src/conductor/client/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/configuration/settings/metrics_settings.py` & `conductor_python-1.1.7/src/conductor/client/configuration/settings/metrics_settings.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/event/event_client.py` & `conductor_python-1.1.7/src/conductor/client/event/event_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/event/queue/kafka_queue_configuration.py` & `conductor_python-1.1.7/src/conductor/client/event/queue/kafka_queue_configuration.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/event/queue/queue_configuration.py` & `conductor_python-1.1.7/src/conductor/client/event/queue/queue_configuration.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/exceptions/api_exception_handler.py` & `conductor_python-1.1.7/src/conductor/client/exceptions/api_exception_handler.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/helpers/helper.py` & `conductor_python-1.1.7/src/conductor/client/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/application_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/application_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/authorization_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/authorization_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/event_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/event_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/group_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/group_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/integration_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/integration_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/metadata_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/metadata_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/prompt_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/prompt_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/scheduler_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/scheduler_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/secret_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/secret_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/task_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/task_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/token_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/token_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/user_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/user_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/workflow_bulk_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/workflow_bulk_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api/workflow_resource_api.py` & `conductor_python-1.1.7/src/conductor/client/http/api/workflow_resource_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/api_client.py` & `conductor_python-1.1.7/src/conductor/client/http/api_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/__init__.py` & `conductor_python-1.1.7/src/conductor/client/http/models/__init__.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/action.py` & `conductor_python-1.1.7/src/conductor/client/http/models/action.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/authorization_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/authorization_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/bulk_response.py` & `conductor_python-1.1.7/src/conductor/client/http/models/bulk_response.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/conductor_application.py` & `conductor_python-1.1.7/src/conductor/client/http/models/conductor_application.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/conductor_user.py` & `conductor_python-1.1.7/src/conductor/client/http/models/conductor_user.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/correlation_ids_search_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/correlation_ids_search_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/create_or_update_application_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/create_or_update_application_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/event_handler.py` & `conductor_python-1.1.7/src/conductor/client/http/models/event_handler.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/external_storage_location.py` & `conductor_python-1.1.7/src/conductor/client/http/models/external_storage_location.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/generate_token_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/generate_token_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/group.py` & `conductor_python-1.1.7/src/conductor/client/http/models/group.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/health.py` & `conductor_python-1.1.7/src/conductor/client/http/models/health.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/health_check_status.py` & `conductor_python-1.1.7/src/conductor/client/http/models/health_check_status.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/integration.py` & `conductor_python-1.1.7/src/conductor/client/http/models/integration.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/integration_api.py` & `conductor_python-1.1.7/src/conductor/client/http/models/integration_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/integration_api_update.py` & `conductor_python-1.1.7/src/conductor/client/http/models/integration_api_update.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/integration_def.py` & `conductor_python-1.1.7/src/conductor/client/http/models/integration_def.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/integration_update.py` & `conductor_python-1.1.7/src/conductor/client/http/models/integration_update.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/permission.py` & `conductor_python-1.1.7/src/conductor/client/http/models/permission.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/poll_data.py` & `conductor_python-1.1.7/src/conductor/client/http/models/poll_data.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/prompt_template.py` & `conductor_python-1.1.7/src/conductor/client/http/models/prompt_template.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/prompt_test_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/prompt_test_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/rate_limit.py` & `conductor_python-1.1.7/src/conductor/client/http/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/rerun_workflow_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/rerun_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/response.py` & `conductor_python-1.1.7/src/conductor/client/http/models/response.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/role.py` & `conductor_python-1.1.7/src/conductor/client/http/models/role.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/save_schedule_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/save_schedule_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py` & `conductor_python-1.1.7/src/conductor/client/http/models/scrollable_search_result_workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/search_result_task.py` & `conductor_python-1.1.7/src/conductor/client/http/models/search_result_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/search_result_task_summary.py` & `conductor_python-1.1.7/src/conductor/client/http/models/search_result_task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow.py` & `conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py` & `conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow_schedule_execution_model.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/search_result_workflow_summary.py` & `conductor_python-1.1.7/src/conductor/client/http/models/search_result_workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/skip_task_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/skip_task_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/start_workflow.py` & `conductor_python-1.1.7/src/conductor/client/http/models/start_workflow.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/start_workflow_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/start_workflow_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/state_change_event.py` & `conductor_python-1.1.7/src/conductor/client/http/models/state_change_event.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/sub_workflow_params.py` & `conductor_python-1.1.7/src/conductor/client/http/models/sub_workflow_params.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/subject_ref.py` & `conductor_python-1.1.7/src/conductor/client/http/models/subject_ref.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/tag_object.py` & `conductor_python-1.1.7/src/conductor/client/http/models/tag_object.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/tag_string.py` & `conductor_python-1.1.7/src/conductor/client/http/models/tag_string.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/target_ref.py` & `conductor_python-1.1.7/src/conductor/client/http/models/target_ref.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task_def.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task_def.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task_details.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task_details.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task_exec_log.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task_exec_log.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task_result.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task_result.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/task_summary.py` & `conductor_python-1.1.7/src/conductor/client/http/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/upsert_group_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/upsert_group_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/upsert_user_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/upsert_user_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_def.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_def.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         'tasks': 'list[WorkflowTask]',
         'input_parameters': 'list[str]',
         'output_parameters': 'dict(str, object)',
         'failure_workflow': 'str',
         'schema_version': 'int',
         'restartable': 'bool',
         'workflow_status_listener_enabled': 'bool',
+        'workflow_status_listener_sink': 'str',
         'owner_email': 'str',
         'timeout_policy': 'str',
         'timeout_seconds': 'int',
         'variables': 'dict(str, object)',
         'input_template': 'dict(str, object)'
     }
 
@@ -54,24 +55,26 @@
         'tasks': 'tasks',
         'input_parameters': 'inputParameters',
         'output_parameters': 'outputParameters',
         'failure_workflow': 'failureWorkflow',
         'schema_version': 'schemaVersion',
         'restartable': 'restartable',
         'workflow_status_listener_enabled': 'workflowStatusListenerEnabled',
+        'workflow_status_listener_sink': 'workflowStatusListenerSink',
         'owner_email': 'ownerEmail',
         'timeout_policy': 'timeoutPolicy',
         'timeout_seconds': 'timeoutSeconds',
         'variables': 'variables',
         'input_template': 'inputTemplate'
     }
 
     def __init__(self, owner_app=None, create_time=None, update_time=None, created_by=None, updated_by=None, name=None,
                  description=None, version=None, tasks=None, input_parameters=None, output_parameters: dict = {},
                  failure_workflow=None, schema_version=None, restartable=None, workflow_status_listener_enabled=None,
+                 workflow_status_listener_sink=None,
                  owner_email=None, timeout_policy=None, timeout_seconds=None, variables=None,
                  input_template=None):  # noqa: E501
         """WorkflowDef - a model defined in Swagger"""  # noqa: E501
         self._owner_app = None
         self._create_time = None
         self._update_time = None
         self._created_by = None
@@ -82,14 +85,15 @@
         self._tasks = []
         self._input_parameters = None
         self._output_parameters = None
         self._failure_workflow = None
         self._schema_version = None
         self._restartable = None
         self._workflow_status_listener_enabled = None
+        self._workflow_status_listener_sink = None
         self._owner_email = None
         self._timeout_policy = None
         self._timeout_seconds = None
         self._variables = None
         self._input_template = None
         self.discriminator = None
         if owner_app is not None:
@@ -115,15 +119,17 @@
         if failure_workflow is not None:
             self.failure_workflow = failure_workflow
         if schema_version is not None:
             self.schema_version = schema_version
         if restartable is not None:
             self.restartable = restartable
         if workflow_status_listener_enabled is not None:
-            self.workflow_status_listener_enabled = workflow_status_listener_enabled
+            self._workflow_status_listener_enabled = workflow_status_listener_enabled
+        if workflow_status_listener_sink is not None:
+            self._workflow_status_listener_sink = workflow_status_listener_sink
         if owner_email is not None:
             self.owner_email = owner_email
         if timeout_policy is not None:
             self.timeout_policy = timeout_policy
         self.timeout_seconds = timeout_seconds
         if variables is not None:
             self.variables = variables
@@ -442,14 +448,22 @@
         :param workflow_status_listener_enabled: The workflow_status_listener_enabled of this WorkflowDef.  # noqa: E501
         :type: bool
         """
 
         self._workflow_status_listener_enabled = workflow_status_listener_enabled
 
     @property
+    def workflow_status_listener_sink(self):
+        return self._workflow_status_listener_sink
+
+    @workflow_status_listener_sink.setter
+    def workflow_status_listener_sink(self, workflow_status_listener_sink):
+        self._workflow_status_listener_sink = workflow_status_listener_sink
+
+    @property
     def owner_email(self):
         """Gets the owner_email of this WorkflowDef.  # noqa: E501
 
 
         :return: The owner_email of this WorkflowDef.  # noqa: E501
         :rtype: str
         """
```

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_run.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_run.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_schedule.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_schedule.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_schedule_execution_model.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_schedule_execution_model.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_state_update.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_state_update.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_status.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_status.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_summary.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_summary.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_tag.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_tag.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_task.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/models/workflow_test_request.py` & `conductor_python-1.1.7/src/conductor/client/http/models/workflow_test_request.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/http/rest.py` & `conductor_python-1.1.7/src/conductor/client/http/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,16 @@
             if method in ['POST', 'PUT', 'PATCH', 'OPTIONS', 'DELETE']:
                 if query_params:
                     url += '?' + urlencode(query_params)
                 if re.search('json', headers['Content-Type'], re.IGNORECASE) or isinstance(body, str):
                     request_body = '{}'
                     if body is not None:
                         request_body = json.dumps(body)
+                        if isinstance(body, str):
+                            request_body = request_body.strip('"')
                     r = self.connection.request(
                         method, url,
                         data=request_body,
                         timeout=timeout,
                         headers=headers
                     )
                 else:
```

### Comparing `conductor_python-1.1.6/src/conductor/client/integration_client.py` & `conductor_python-1.1.7/src/conductor/client/integration_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/metadata_client.py` & `conductor_python-1.1.7/src/conductor/client/metadata_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/api/tags_api.py` & `conductor_python-1.1.7/src/conductor/client/orkes/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/models/access_key.py` & `conductor_python-1.1.7/src/conductor/client/orkes/models/access_key.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/models/created_access_key.py` & `conductor_python-1.1.7/src/conductor/client/orkes/models/created_access_key.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/models/granted_permission.py` & `conductor_python-1.1.7/src/conductor/client/orkes/models/granted_permission.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_authorization_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_authorization_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_base_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_base_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_integration_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_integration_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_metadata_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_metadata_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_prompt_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_prompt_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_scheduler_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_scheduler_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_secret_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_secret_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_task_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_task_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes/orkes_workflow_client.py` & `conductor_python-1.1.7/src/conductor/client/orkes/orkes_workflow_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/orkes_clients.py` & `conductor_python-1.1.7/src/conductor/client/orkes_clients.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/prompt_client.py` & `conductor_python-1.1.7/src/conductor/client/prompt_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/scheduler_client.py` & `conductor_python-1.1.7/src/conductor/client/scheduler_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/secret_client.py` & `conductor_python-1.1.7/src/conductor/client/secret_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/task_client.py` & `conductor_python-1.1.7/src/conductor/client/task_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/telemetry/metrics_collector.py` & `conductor_python-1.1.7/src/conductor/client/telemetry/metrics_collector.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/telemetry/model/metric_documentation.py` & `conductor_python-1.1.7/src/conductor/client/telemetry/model/metric_documentation.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/telemetry/model/metric_name.py` & `conductor_python-1.1.7/src/conductor/client/telemetry/model/metric_name.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/worker/worker.py` & `conductor_python-1.1.7/src/conductor/client/worker/worker.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/worker/worker_interface.py` & `conductor_python-1.1.7/src/conductor/client/worker/worker_interface.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/worker/worker_task.py` & `conductor_python-1.1.7/src/conductor/client/worker/worker_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/conductor_workflow.py` & `conductor_python-1.1.7/src/conductor/client/workflow/conductor_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         self._timeout_seconds = 60
         self._failure_workflow = ''
         self._input_parameters = []
         self._output_parameters = {}
         self._input_template = {}
         self._variables = {}
         self._restartable = True
+        self._workflow_status_listener_enabled = False
+        self._workflow_status_listener_sink = None
 
     @property
     def name(self) -> str:
         return self._name
 
     @name.setter
     def name(self, name: str) -> None:
@@ -97,14 +99,22 @@
     # Set this to false if restarting workflow can have side effects
     def restartable(self, restartable: bool) -> Self:
         if not isinstance(restartable, bool):
             raise Exception('invalid type')
         self._restartable = deepcopy(restartable)
         return self
 
+    def enable_status_listener(self, sink_name: bool) -> Self:
+        self._workflow_status_listener_sink = sink_name
+        self._workflow_status_listener_enabled = True
+
+    def disable_status_listener(self) -> Self:
+        self._workflow_status_listener_sink = None
+        self._workflow_status_listener_enabled = False
+
     # Workflow output follows similar structure as task input
     # See https://conductor.netflix.com/how-tos/Tasks/task-inputs.html for more details
     def output_parameters(self, output_parameters: Dict[str, Any]) -> Self:
         if output_parameters == None:
             self._output_parameters = {}
             return
         if not isinstance(output_parameters, dict):
@@ -253,14 +263,16 @@
             failure_workflow=self._failure_workflow,
             schema_version=ConductorWorkflow.SCHEMA_VERSION,
             owner_email=self._owner_email,
             timeout_policy=self._timeout_policy,
             timeout_seconds=self._timeout_seconds,
             variables=self._variables,
             input_template=self._input_template,
+            workflow_status_listener_enabled=self._workflow_status_listener_enabled,
+            workflow_status_listener_sink=self._workflow_status_listener_sink
         )
 
     def to_workflow_task(self):
         sub_workflow_task = InlineSubWorkflowTask(task_ref_name=self.name + '_' + str(uuid()), workflow=self)
         sub_workflow_task.input_parameters.update(self._input_template)
         return sub_workflow_task.to_workflow_task()
```

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/executor/workflow_executor.py` & `conductor_python-1.1.7/src/conductor/client/workflow/executor/workflow_executor.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/do_while_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/do_while_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/dynamic_fork_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/dynamic_fork_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/dynamic_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/dynamic_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/event_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/event_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/fork_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/fork_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/get_document.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/get_document.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/http_poll_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/http_poll_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/http_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/http_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/human_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/human_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/inline.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/inline.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/javascript_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/javascript_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/join_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/join_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/kafka_publish.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/kafka_publish.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/kafka_publish_input.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/kafka_publish_input.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_chat_complete.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_generate_embeddings.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_index_documents.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_index_text.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_query_embeddings.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_search_index.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/llm_text_complete.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/embedding_model.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/llm_tasks/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/simple_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/simple_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/start_workflow_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/start_workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/sub_workflow_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/sub_workflow_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/switch_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/switch_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/task_type.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/task_type.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/terminate_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/terminate_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/wait_for_webhook_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/wait_for_webhook_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow/task/wait_task.py` & `conductor_python-1.1.7/src/conductor/client/workflow/task/wait_task.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor/client/workflow_client.py` & `conductor_python-1.1.7/src/conductor/client/workflow_client.py`

 * *Files identical despite different names*

### Comparing `conductor_python-1.1.6/src/conductor_python.egg-info/PKG-INFO` & `conductor_python-1.1.7/src/conductor_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conductor-python
-Version: 1.1.6
+Version: 1.1.7
 Summary: Netflix Conductor Python SDK
 Home-page: https://github.com/conductor-sdk/conductor-python
 Author: Orkes
 Author-email: developers@orkes.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

### Comparing `conductor_python-1.1.6/src/conductor_python.egg-info/SOURCES.txt` & `conductor_python-1.1.7/src/conductor_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

