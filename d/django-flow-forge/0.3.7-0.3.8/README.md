# Comparing `tmp/django_flow_forge-0.3.7.tar.gz` & `tmp/django_flow_forge-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_flow_forge-0.3.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_flow_forge-0.3.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_flow_forge-0.3.7.tar` & `django_flow_forge-0.3.8.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0     6148 2024-05-16 10:26:17.958899 django_flow_forge-0.3.7/.DS_Store
--rw-r--r--   0        0        0       66 2024-05-16 10:26:17.958899 django_flow_forge-0.3.7/.gitattributes
--rw-r--r--   0        0        0      862 2024-05-16 10:26:17.958899 django_flow_forge-0.3.7/.github/workflows/deploy-mkdocs.yml
--rw-r--r--   0        0        0      620 2024-05-16 10:26:17.958899 django_flow_forge-0.3.7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     2879 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/.gitignore
--rw-r--r--   0        0        0     1613 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/.vscode/launch.json
--rw-r--r--   0        0        0     1103 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/Dockerfile
--rw-r--r--   0        0        0     1061 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/LICENSE
--rw-r--r--   0        0        0      151 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/MANIFEST.in
--rw-r--r--   0        0        0      865 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/README.md
--rwxr-xr-x   0        0        0        0 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/__init__.py
--rwxr-xr-x   0        0        0     3638 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/admin.py
--rwxr-xr-x   0        0        0      160 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/apps.py
--rw-r--r--   0        0        0     2306 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/async_utils.py
--rw-r--r--   0        0        0     3203 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/authorization.py
--rw-r--r--   0        0        0     1190 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/batch_utils.py
--rw-r--r--   0        0        0    15970 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/flow_engine.py
--rw-r--r--   0        0        0     5435 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0001_initial.py
--rw-r--r--   0        0        0      816 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
--rw-r--r--   0        0        0      449 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
--rw-r--r--   0        0        0      624 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
--rw-r--r--   0        0        0      428 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0005_alter_flow_options.py
--rw-r--r--   0        0        0      564 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
--rw-r--r--   0        0        0      436 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0007_executedflow_params.py
--rw-r--r--   0        0        0      419 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0008_executedflow_meta.py
--rw-r--r--   0        0        0     1411 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py
--rw-r--r--   0        0        0     1066 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0010_batchhandler.py
--rw-r--r--   0        0        0     2004 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py
--rw-r--r--   0        0        0      416 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0012_rename_total_batches_batchhandler_total_batch_count.py
--rw-r--r--   0        0        0     1346 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py
--rw-r--r--   0        0        0      345 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0014_delete_batchtempdata.py
--rw-r--r--   0        0        0      555 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/0015_batchhandler_date_initialised.py
--rwxr-xr-x   0        0        0        0 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/__init__.py
--rw-r--r--   0        0        0      778 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0001_initial.py
--rw-r--r--   0        0        0      392 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
--rw-r--r--   0        0        0     1236 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
--rw-r--r--   0        0        0      451 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
--rw-r--r--   0        0        0      400 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
--rw-r--r--   0        0        0      627 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
--rw-r--r--   0        0        0      448 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
--rw-r--r--   0        0        0      444 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
--rw-r--r--   0        0        0     1717 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
--rw-r--r--   0        0        0      414 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
--rw-r--r--   0        0        0      573 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
--rw-r--r--   0        0        0      980 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
--rw-r--r--   0        0        0      537 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
--rw-r--r--   0        0        0      732 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
--rw-r--r--   0        0        0      432 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
--rw-r--r--   0        0        0      467 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
--rw-r--r--   0        0        0      613 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
--rw-r--r--   0        0        0      740 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
--rw-r--r--   0        0        0      673 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      451 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
--rw-r--r--   0        0        0      841 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
--rw-r--r--   0        0        0      554 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
--rw-r--r--   0        0        0     1295 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0023_mlresult.py
--rw-r--r--   0        0        0      550 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
--rw-r--r--   0        0        0      542 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
--rw-r--r--   0        0        0      647 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
--rw-r--r--   0        0        0      446 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
--rw-r--r--   0        0        0      639 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
--rw-r--r--   0        0        0      436 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
--rw-r--r--   0        0        0      771 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
--rwxr-xr-x   0        0        0     6712 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/models.py
--rw-r--r--   0        0        0      627 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
--rw-r--r--   0        0        0    47755 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/static/django_flow_forge/htmx.min.js
--rw-r--r--   0        0        0    10754 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/task_utils.py
--rw-r--r--   0        0        0      957 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
--rw-r--r--   0        0        0      570 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
--rw-r--r--   0        0        0     3526 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
--rw-r--r--   0        0        0      806 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
--rw-r--r--   0        0        0     2701 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
--rw-r--r--   0        0        0      825 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
--rw-r--r--   0        0        0     1422 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_result.html
--rw-r--r--   0        0        0     1808 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0     2699 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     3194 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
--rw-r--r--   0        0        0     3723 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
--rw-r--r--   0        0        0     5888 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
--rwxr-xr-x   0        0        0     2962 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/tests.py
--rw-r--r--   0        0        0      680 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/urls.py
--rwxr-xr-x   0        0        0     9525 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/django_flow_forge/views.py
--rw-r--r--   0        0        0      767 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docker-compose-local.yml
--rw-r--r--   0        0        0      846 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/authorization.md
--rw-r--r--   0        0        0     3996 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/considerations.md
--rw-r--r--   0        0        0      866 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/data_science_experiments.md
--rw-r--r--   0        0        0     1031 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/debugging.md
--rw-r--r--   0        0        0     1295 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/flows_dashboard.md
--rw-r--r--   0        0        0     4269 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/index.md
--rw-r--r--   0        0        0     3613 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/installation.md
--rw-r--r--   0        0        0      270 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/roadmap.md
--rw-r--r--   0        0        0     1037 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/docs/strategies.md
--rw-r--r--   0        0        0        0 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/conf/__init__.py
--rw-r--r--   0        0        0      396 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/conf/asgi.py
--rw-r--r--   0        0        0     4130 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/conf/settings.py
--rw-r--r--   0        0        0      898 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/conf/urls.py
--rw-r--r--   0        0        0      396 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/conf/wsgi.py
--rw-r--r--   0        0        0    32768 2024-05-16 10:26:17.962899 django_flow_forge-0.3.7/example_project/db.sqlite3-shm
--rw-r--r--   0        0        0  2904632 2024-05-16 10:26:17.970899 django_flow_forge-0.3.7/example_project/db.sqlite3-wal
--rw-r--r--   0        0        0      177 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/admin.py
--rw-r--r--   0        0        0      605 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/apps.py
--rw-r--r--   0        0        0      831 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/celery_app.py
--rw-r--r--   0        0        0     4720 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__ml_grid_search.py
--rw-r--r--   0        0        0     1394 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__parallel_celery.py
--rw-r--r--   0        0        0     1409 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__simple.py
--rw-r--r--   0        0        0     2980 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__simple_ml.py
--rw-r--r--   0        0        0     1555 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__simple_with_celery.py
--rw-r--r--   0        0        0     2137 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/flow__with_nested_tasks.py
--rw-r--r--   0        0        0        0 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/models.py
--rw-r--r--   0        0        0     2134 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
--rw-r--r--   0        0        0      994 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
--rw-r--r--   0        0        0     1922 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/templates/example_app/index.html
--rw-r--r--   0        0        0       60 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/tests.py
--rw-r--r--   0        0        0      962 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/urls.py
--rw-r--r--   0        0        0     2531 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/example_app/views.py
--rwxr-xr-x   0        0        0      660 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/manage.py
--rw-r--r--   0        0        0      522 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/example_project/run_tasks_no_server.py
--rw-r--r--   0        0        0      399 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/mkdocs.yml
--rw-r--r--   0        0        0      873 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/pyproject.toml
--rw-r--r--   0        0        0       45 2024-05-16 10:26:17.974899 django_flow_forge-0.3.7/requirements.txt
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 django_flow_forge-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.DS_Store
+-rw-r--r--   0        0        0       66 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.gitattributes
+-rw-r--r--   0        0        0      862 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.github/workflows/deploy-mkdocs.yml
+-rw-r--r--   0        0        0      620 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     2879 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.gitignore
+-rw-r--r--   0        0        0     1613 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/.vscode/launch.json
+-rw-r--r--   0        0        0     1103 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/Dockerfile
+-rw-r--r--   0        0        0     1061 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/LICENSE
+-rw-r--r--   0        0        0      151 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/MANIFEST.in
+-rw-r--r--   0        0        0      865 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/__init__.py
+-rwxr-xr-x   0        0        0     3638 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/admin.py
+-rwxr-xr-x   0        0        0      160 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/apps.py
+-rw-r--r--   0        0        0     2306 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/async_utils.py
+-rw-r--r--   0        0        0     3202 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/authorization.py
+-rw-r--r--   0        0        0     1190 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/batch_utils.py
+-rw-r--r--   0        0        0    16058 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/flow_engine.py
+-rw-r--r--   0        0        0     5435 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0001_initial.py
+-rw-r--r--   0        0        0      816 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py
+-rw-r--r--   0        0        0      449 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0003_alter_executedtask_exceptions.py
+-rw-r--r--   0        0        0      624 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py
+-rw-r--r--   0        0        0      428 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0005_alter_flow_options.py
+-rw-r--r--   0        0        0      564 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py
+-rw-r--r--   0        0        0      436 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0007_executedflow_params.py
+-rw-r--r--   0        0        0      419 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0008_executedflow_meta.py
+-rw-r--r--   0        0        0     1411 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py
+-rw-r--r--   0        0        0     1066 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0010_batchhandler.py
+-rw-r--r--   0        0        0     2004 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py
+-rw-r--r--   0        0        0      416 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0012_rename_total_batches_batchhandler_total_batch_count.py
+-rw-r--r--   0        0        0     1346 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py
+-rw-r--r--   0        0        0      345 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0014_delete_batchtempdata.py
+-rw-r--r--   0        0        0      555 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/0015_batchhandler_date_initialised.py
+-rwxr-xr-x   0        0        0        0 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/__init__.py
+-rw-r--r--   0        0        0      778 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0001_initial.py
+-rw-r--r--   0        0        0      392 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0002_processtask_task_output.py
+-rw-r--r--   0        0        0     1236 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py
+-rw-r--r--   0        0        0      451 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0004_processtask_nested_task.py
+-rw-r--r--   0        0        0      400 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0005_rename_nested_task_processtask_bidirectional_task.py
+-rw-r--r--   0        0        0      627 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py
+-rw-r--r--   0        0        0      448 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0007_rename_bidirectional_dependencies_processtask_depends_bidirectionally_with.py
+-rw-r--r--   0        0        0      444 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0008_rename_dependencies_processtask_depends_on.py
+-rw-r--r--   0        0        0     1717 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py
+-rw-r--r--   0        0        0      414 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0010_processtask_nested.py
+-rw-r--r--   0        0        0      573 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py
+-rw-r--r--   0        0        0      980 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py
+-rw-r--r--   0        0        0      537 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      732 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py
+-rw-r--r--   0        0        0      432 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0015_alter_taskrun_output.py
+-rw-r--r--   0        0        0      467 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0016_rename_processrun_executedprocess_and_more.py
+-rw-r--r--   0        0        0      613 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py
+-rw-r--r--   0        0        0      740 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py
+-rw-r--r--   0        0        0      673 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      451 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0020_executedtask_task_name_snapshot.py
+-rw-r--r--   0        0        0      841 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py
+-rw-r--r--   0        0        0      554 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py
+-rw-r--r--   0        0        0     1295 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0023_mlresult.py
+-rw-r--r--   0        0        0      550 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py
+-rw-r--r--   0        0        0      542 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py
+-rw-r--r--   0        0        0      647 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py
+-rw-r--r--   0        0        0      446 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0027_executedtask_task_status.py
+-rw-r--r--   0        0        0      639 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py
+-rw-r--r--   0        0        0      436 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0029_executedtask_exceptions.py
+-rw-r--r--   0        0        0      771 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py
+-rwxr-xr-x   0        0        0     6712 2024-05-22 12:48:40.048153 django_flow_forge-0.3.8/django_flow_forge/models.py
+-rw-r--r--   0        0        0      627 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/static/django_flow_forge/cytoscape_setup.js
+-rw-r--r--   0        0        0    47755 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/static/django_flow_forge/htmx.min.js
+-rw-r--r--   0        0        0    10754 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/task_utils.py
+-rw-r--r--   0        0        0      957 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html
+-rw-r--r--   0        0        0      570 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html
+-rw-r--r--   0        0        0     3526 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html
+-rw-r--r--   0        0        0      806 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html
+-rw-r--r--   0        0        0     2701 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html
+-rw-r--r--   0        0        0      825 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html
+-rw-r--r--   0        0        0     1422 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_result.html
+-rw-r--r--   0        0        0     1808 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0     2699 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     3194 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html
+-rw-r--r--   0        0        0     3723 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html
+-rw-r--r--   0        0        0     6163 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html
+-rwxr-xr-x   0        0        0     2962 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/tests.py
+-rw-r--r--   0        0        0      680 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/urls.py
+-rwxr-xr-x   0        0        0     9525 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/django_flow_forge/views.py
+-rw-r--r--   0        0        0      767 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docker-compose-local.yml
+-rw-r--r--   0        0        0      846 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/authorization.md
+-rw-r--r--   0        0        0     3996 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/considerations.md
+-rw-r--r--   0        0        0      866 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/data_science_experiments.md
+-rw-r--r--   0        0        0     1031 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/debugging.md
+-rw-r--r--   0        0        0     1295 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/flows_dashboard.md
+-rw-r--r--   0        0        0     4402 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/index.md
+-rw-r--r--   0        0        0     3613 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/installation.md
+-rw-r--r--   0        0        0      270 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/roadmap.md
+-rw-r--r--   0        0        0     1037 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/docs/strategies.md
+-rw-r--r--   0        0        0        0 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/conf/__init__.py
+-rw-r--r--   0        0        0      396 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/conf/asgi.py
+-rw-r--r--   0        0        0     4130 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/conf/settings.py
+-rw-r--r--   0        0        0      898 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/conf/urls.py
+-rw-r--r--   0        0        0      396 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/conf/wsgi.py
+-rw-r--r--   0        0        0    32768 2024-05-22 12:48:40.052152 django_flow_forge-0.3.8/example_project/db.sqlite3-shm
+-rw-r--r--   0        0        0  2904632 2024-05-22 12:48:40.060153 django_flow_forge-0.3.8/example_project/db.sqlite3-wal
+-rw-r--r--   0        0        0      177 2024-05-22 12:48:40.060153 django_flow_forge-0.3.8/example_project/example_app/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:48:40.060153 django_flow_forge-0.3.8/example_project/example_app/admin.py
+-rw-r--r--   0        0        0      605 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/apps.py
+-rw-r--r--   0        0        0      831 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/celery_app.py
+-rw-r--r--   0        0        0     4720 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__ml_grid_search.py
+-rw-r--r--   0        0        0     1394 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__parallel_celery.py
+-rw-r--r--   0        0        0     1409 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__simple.py
+-rw-r--r--   0        0        0     2980 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__simple_ml.py
+-rw-r--r--   0        0        0     1555 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__simple_with_celery.py
+-rw-r--r--   0        0        0     2137 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/flow__with_nested_tasks.py
+-rw-r--r--   0        0        0        0 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/models.py
+-rw-r--r--   0        0        0     2134 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html
+-rw-r--r--   0        0        0      994 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html
+-rw-r--r--   0        0        0     1922 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/templates/example_app/index.html
+-rw-r--r--   0        0        0       60 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/tests.py
+-rw-r--r--   0        0        0      962 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/urls.py
+-rw-r--r--   0        0        0     2531 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/example_app/views.py
+-rwxr-xr-x   0        0        0      660 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/manage.py
+-rw-r--r--   0        0        0      522 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/example_project/run_tasks_no_server.py
+-rw-r--r--   0        0        0      399 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/mkdocs.yml
+-rw-r--r--   0        0        0      873 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0       45 2024-05-22 12:48:40.064153 django_flow_forge-0.3.8/requirements.txt
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 django_flow_forge-0.3.8/PKG-INFO
```

### Comparing `django_flow_forge-0.3.7/.DS_Store` & `django_flow_forge-0.3.8/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/.github/workflows/deploy-mkdocs.yml` & `django_flow_forge-0.3.8/.github/workflows/deploy-mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/.github/workflows/publish-to-pypi.yml` & `django_flow_forge-0.3.8/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/.gitignore` & `django_flow_forge-0.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/.vscode/launch.json` & `django_flow_forge-0.3.8/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/Dockerfile` & `django_flow_forge-0.3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/LICENSE` & `django_flow_forge-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/README.md` & `django_flow_forge-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/admin.py` & `django_flow_forge-0.3.8/django_flow_forge/admin.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/async_utils.py` & `django_flow_forge-0.3.8/django_flow_forge/async_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/authorization.py` & `django_flow_forge-0.3.8/django_flow_forge/authorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
         
         setattr(_wrapped_view, permission, True)
         return _wrapped_view
         
 
     return decorator
 
-
 class FlowForgePermissionMixin(LoginRequiredMixin, AccessMixin):
     # Permission to check for
     permission_required = 'django_flow_forge.django_flow_admin_access'
     # Whether to allow superusers access regardless of the permission
     allow_superuser = True
 
     def dispatch(self, request, *args, **kwargs):
```

### Comparing `django_flow_forge-0.3.7/django_flow_forge/batch_utils.py` & `django_flow_forge-0.3.8/django_flow_forge/batch_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/flow_engine.py` & `django_flow_forge-0.3.8/django_flow_forge/flow_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,16 @@
             return
 
     flow_pipeline = flow_pipeline_lookup.get(flow_name)
     flow_snapshot = make_flow_snapshot(flow_pipeline, task_order)
     flow_snapshot['graph'] = get_cytoscape_nodes_and_edges(all_task_objs, show_nested=True)
     flow_snapshot['flow_name'] = flow_name
     flow_run.flow_snapshot = flow_snapshot
+    if kwargs.get('flow_metadata'):
+        flow_run.meta = kwargs.get('flow_metadata')
     flow_run.save()
     kwargs['executed_flow_id'] = flow_run.id
     kwargs['flow_name'] = flow_name
     kwargs['flow_batch_id'] = flow_batch_id
         
     executors = {}
```

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0001_initial.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0002_alter_executedflow_status_alter_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0004_alter_executedflow_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0006_flowtask_code_flowtask_docstring.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0009_flowbatch_flowbatchtempdata.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0010_batchhandler.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0010_batchhandler.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0011_remove_flowbatchtempdata_batch_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0013_remove_batchtempdata_batch_handler_flowbatch_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/0015_batchhandler_date_initialised.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/0015_batchhandler_date_initialised.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0001_initial.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0003_process_alter_processtask_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0006_remove_processtask_bidirectional_task_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0009_processrun_taskrun.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0011_processrun_process_complete_taskrun_task_complete.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0012_process_process_display_name_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0013_remove_taskrun_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0014_taskrun_task_snapshot_id_alter_taskrun_task.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0017_executedtask_task_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0018_process_in_current_code_base_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0019_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0021_alter_executedprocess_process_id_snapshot_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0022_executedprocess_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0023_mlresult.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0023_mlresult.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0024_alter_mlresult_executed_process.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0025_executedprocess_last_checkpoint_datetime.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0026_executedprocess_exceptions_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0028_remove_executedtask_task_status_executedtask_status.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py` & `django_flow_forge-0.3.8/django_flow_forge/migrations/zdnu/0030_alter_executedprocess_status_and_more.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/models.py` & `django_flow_forge-0.3.8/django_flow_forge/models.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/static/django_flow_forge/cytoscape_setup.js` & `django_flow_forge-0.3.8/django_flow_forge/static/django_flow_forge/cytoscape_setup.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/static/django_flow_forge/htmx.min.js` & `django_flow_forge-0.3.8/django_flow_forge/static/django_flow_forge/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/task_utils.py` & `django_flow_forge-0.3.8/django_flow_forge/task_utils.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/clicked_concept_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/clicked_executed_task_node_info.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_clickable_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_cyto_conceptual_script.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/dag_graph_and_ml.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_result.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_result.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/components/task_summary_charts.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/dag_conceptual_index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html` & `django_flow_forge-0.3.8/django_flow_forge/templates/django_flow_forge/dag_tasks_run.html`

 * *Files 2% similar despite different names*

```diff
@@ -95,25 +95,29 @@
                 <div class="col">
                     <table class="table table-dark table-bordered rounded">
                         <thead>
                             <tr>
                                 <th scope="col">Process Name</th>
                                 <th scope="col">Start Time</th>
                                 <th class='text-center narrow-col' scope="col">Status</th>
+                                <th class='text-center narrow-col' scope="col">Metadata</th>
                                 <th scope="col"></th>
                             </tr>
                         </thead>
                         <tbody>
                             {% for flow in page_obj %}
                             <tr class='align-middle' style="font-size: 0.8rem;">
                                 <td >{{ flow.flow_name_snapshot }}</td>
                                 <td>{{ flow.start_time }}</td>
                                 <td class="text-center">
                                     <span class="badge {{ flow.status }} text-dark">{{ flow.get_status_display }}</span>
-                                    
+                                </td>
+                                <td class="text-center">
+                                    <span>{{ flow.meta|slice:":300" }}{% if flow.meta|length > 300 %}...{% endif %}</span>
+
                                 </td>
                                 <td class="text-center">
                                     <button name='executed_flow_option' value='{{ flow.id }}' class="btn btn-primary badge btn-sm" 
                                     hx-get="{% url 'django-flow-forge:tasks_run_viz' %}" hx-target="#cytoscape-and_ml-outer-row" hx-swap="innerHTML">
                                         <i class="fas fa-play"></i> Draw Graph
                                     </button>
                                 </td>
```

#### html2text {}

```diff
@@ -2,17 +2,20 @@
 {% load django_htmx %}
 {% endblock head %} {% block body %}
 ********** FFllooww DDaasshhbbooaarrdd **********
 ===============================================================================
 {% include 'django_flow_forge/components/task_summary_charts.html' %}
 ******** SSttaattuuss TTaabbllee ********
 ===============================================================================
-PPrroocceessss NNaammee            SSttaarrtt TTiimmee         SSttaattuuss
-{                                          {
-{                       {{ flow.start_time {                       Draw Graph
-flow.flow_name_snapshot }}                 flow.get_status_display
-}}                                         }}
+PPrroocceessss NNaammee            SSttaarrtt TTiimmee      SSttaattuuss                  MMeettaaddaattaa
+                                                                {
+{                       {               {                       {
+{                       {               {                       flow.meta|slice: Draw
+flow.flow_name_snapshot flow.start_time flow.get_status_display ":300" }}{% if   Graph
+}}                      }}              }}                      flow.meta|length
+                                                                > 300 %}...{%
+                                                                endif %}
 {% if page_obj.has_previous %} _«_ _f_i_r_s_t _p_r_e_v_i_o_u_s {% endif %} Page {
 { page_obj.number }} of {{ page_obj.paginator.num_pages }}. {% if
 page_obj.has_next %} _n_e_x_t _l_a_s_t_ _» {% endif %}
 {% include 'django_flow_forge/components/dag_graph_and_ml.html' %}
 {% endblock body %}
```

### Comparing `django_flow_forge-0.3.7/django_flow_forge/tests.py` & `django_flow_forge-0.3.8/django_flow_forge/tests.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/urls.py` & `django_flow_forge-0.3.8/django_flow_forge/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/django_flow_forge/views.py` & `django_flow_forge-0.3.8/django_flow_forge/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docker-compose-local.yml` & `django_flow_forge-0.3.8/docker-compose-local.yml`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/authorization.md` & `django_flow_forge-0.3.8/docs/authorization.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/considerations.md` & `django_flow_forge-0.3.8/docs/considerations.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/data_science_experiments.md` & `django_flow_forge-0.3.8/docs/data_science_experiments.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/debugging.md` & `django_flow_forge-0.3.8/docs/debugging.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/flows_dashboard.md` & `django_flow_forge-0.3.8/docs/flows_dashboard.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/index.md` & `django_flow_forge-0.3.8/docs/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Welcome to Django Flow Forge
 
-In a landscape cluttered with complex ML Ops solutions and vendor lock-in pitfalls that all carry significant gaps, Django Flow Forge aims to be a beacon of pragmatism when forging together your data science work flows.
+In a landscape cluttered with complex ML Ops solutions and vendor lock-ins that all carry significant pitfalls, Django Flow Forge aims to be a beacon of pragmatism when forging together your data science work flows.
 
 ## Designed for Data Scientists and Data Engineers
-By relying on Django, a mature web server framework with modules that already solves a lot of problems in ML Ops, this plugin module streamlines tech stacks in Data or ML Ops in the long run, focusing on standardization and flexibility as a project grows, allowing it to be more impactful.
+By relying on Django, a mature web server framework with modules that already solve a lot of problems in ML Ops, this plugin module aims to streamline tech stacks in Data or ML Ops *in the long run*, focusing on standardization and flexibility as a project grows, allowing it to be more impactful.
 
-As most data science projects grow, they typically end up requiring a production ready pipeline process and to serve the model in some way.
-The intelligent design here is that you learn how to use Django, rather than a plethora of other cobbled together tech, minimizing the technical risk of your projects.
+It has a more complex learning curve than other simple tools, but as most data science projects grow, they typically end up requiring a production ready pipeline process and to serve the model in some way, leading you back to a more complex tool like Django. The intelligent design here is that you learn how to use Django, rather than a plethora of other cobbled together tech, minimizing the long term technical risk of your projects.
 
 ![flow-forge-v0](https://github.com/eddyojb88/django-flow-forge/assets/22086433/7e3a81d7-ef98-4a99-96f7-f39d4f44ff9c)
 
 ## Features
 
 - Easily define your data or ML flows (aka pipeline) as a DAG
 - Visualize your flows for stakeholders, both in planning and development phases (inspired by Kedro)
```

### Comparing `django_flow_forge-0.3.7/docs/installation.md` & `django_flow_forge-0.3.8/docs/installation.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/docs/strategies.md` & `django_flow_forge-0.3.8/docs/strategies.md`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/conf/settings.py` & `django_flow_forge-0.3.8/example_project/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/conf/urls.py` & `django_flow_forge-0.3.8/example_project/conf/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/db.sqlite3-shm` & `django_flow_forge-0.3.8/example_project/db.sqlite3-shm`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/db.sqlite3-wal` & `django_flow_forge-0.3.8/example_project/db.sqlite3-wal`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/apps.py` & `django_flow_forge-0.3.8/example_project/example_app/apps.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/celery_app.py` & `django_flow_forge-0.3.8/example_project/example_app/celery_app.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__ml_grid_search.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__ml_grid_search.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__parallel_celery.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__parallel_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__simple.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__simple.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__simple_ml.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__simple_ml.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__simple_with_celery.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__simple_with_celery.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/flow__with_nested_tasks.py` & `django_flow_forge-0.3.8/example_project/example_app/flow__with_nested_tasks.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html` & `django_flow_forge-0.3.8/example_project/example_app/templates/django_flow_forge/components/ml_result_chart.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html` & `django_flow_forge-0.3.8/example_project/example_app/templates/django_flow_forge/components/ml_results_container.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/templates/example_app/index.html` & `django_flow_forge-0.3.8/example_project/example_app/templates/example_app/index.html`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/urls.py` & `django_flow_forge-0.3.8/example_project/example_app/urls.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/example_app/views.py` & `django_flow_forge-0.3.8/example_project/example_app/views.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/manage.py` & `django_flow_forge-0.3.8/example_project/manage.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/example_project/run_tasks_no_server.py` & `django_flow_forge-0.3.8/example_project/run_tasks_no_server.py`

 * *Files identical despite different names*

### Comparing `django_flow_forge-0.3.7/pyproject.toml` & `django_flow_forge-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-flow-forge"
-version = "0.3.7"
+version = "0.3.8"
 description = "Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows."
 authors = [{name = "Ed Burmicz", email = "eddyojb@gmail.com"}]
 readme = "README.md"
 license = {text = "MIT"} 
 keywords = ["django", "mlops", "data", "machine learning", "data science", "pipelines", "flow", "orchestration", "AI",]
 classifiers = [
     "Framework :: Django",
```

### Comparing `django_flow_forge-0.3.7/PKG-INFO` & `django_flow_forge-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flow-forge
-Version: 0.3.7
+Version: 0.3.8
 Summary: Eliminate unnecessary system complexity in Data Ops and in Machine Learning Ops (MLOps) with this Django module for defining, running and monitoring flows.
 Keywords: django,mlops,data,machine learning,data science,pipelines,flow,orchestration,AI
 Author-email: Ed Burmicz <eddyojb@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
```

