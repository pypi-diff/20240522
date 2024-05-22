# Comparing `tmp/spaceone-cost-analysis-2.0.dev98.tar.gz` & `tmp/spaceone-cost-analysis-2.0.dev99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-cost-analysis-2.0.dev98.tar", last modified: Thu Feb  1 05:11:10 2024, max compression
+gzip compressed data, was "spaceone-cost-analysis-2.0.dev99.tar", last modified: Thu Feb  1 05:12:16 2024, max compression
```

## Comparing `spaceone-cost-analysis-2.0.dev98.tar` & `spaceone-cost-analysis-2.0.dev99.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.092421 spaceone-cost-analysis-2.0.dev98/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.092421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.092421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.096421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/currency_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/datasource_plugin_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/smtp_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.096421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/cost_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/data_source_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/job_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.096421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/budget_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/budget_usage_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/common_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/cost_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/cost_query_set_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/data_source_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/data_source_rule_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/job_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/job_task_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.096421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.100421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/budget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/budget_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_query_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/data_source_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/job_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.100421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.100421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/v1/data_source_sync_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.100421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/budget_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/budget_usage_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_query_set_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/currency_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_rule_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/email_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/job_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/job_task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/notification_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/repository_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/secret_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/budget_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/budget_usage_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_query_set_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/data_source_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/data_source_rule_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/job_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/job_task_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.104421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/job.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/lib/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/cost_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/cost_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/data_source_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/data_source_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/job_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/cost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/data_source_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/job_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.108421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/skeleton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/skeleton/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/budget_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/budget_usage_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_query_set_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_config_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_data_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_serivce.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/data_source_rule_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    21474 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/data_source_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    33660 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/job_task_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/
--rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_en.html
--rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_jp.html
--rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-02-01 05:11:02.000000 spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_ko.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:11:10.112421 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-01 05:11:09.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-02-01 05:11:10.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 05:11:09.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 05:11:09.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-01 05:11:09.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 05:11:09.000000 spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.606747 spaceone-cost-analysis-2.0.dev99/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-01 05:12:16.606747 spaceone-cost-analysis-2.0.dev99/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 05:12:16.606747 spaceone-cost-analysis-2.0.dev99/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.586747 spaceone-cost-analysis-2.0.dev99/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.586747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.586747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.586747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/currency_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/datasource_plugin_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/smtp_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.586747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/cost_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/data_source_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/job_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/budget_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/budget_usage_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/common_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/cost_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/cost_query_set_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/data_source_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/data_source_rule_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/job_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/job_task_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/budget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/budget_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/data_source_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/job_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/v1/data_source_sync_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.590747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.594747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/budget_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14568 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/budget_usage_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_query_set_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/currency_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11329 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_rule_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/email_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/job_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/job_task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/notification_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/repository_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/secret_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/budget_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/budget_usage_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_query_set_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/data_source_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/data_source_rule_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/job_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/job_task_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.598747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/lib/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.602747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/cost_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/cost_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/data_source_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/data_source_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/job_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.602747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/cost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/data_source_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/job_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.602747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/skeleton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/skeleton/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.602747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/budget_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4829 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/budget_usage_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6209 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_query_set_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10405 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_config_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12074 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_data_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20847 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_serivce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/data_source_rule_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21474 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/data_source_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33660 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/job_task_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.606747 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/
+-rw-r--r--   0 runner    (1001) docker     (127)    15212 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_en.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15353 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_jp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15257 2024-02-01 05:12:05.000000 spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_ko.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 05:12:16.606747 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-01 05:12:16.000000 spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/top_level.txt
```

### Comparing `spaceone-cost-analysis-2.0.dev98/setup.py` & `spaceone-cost-analysis-2.0.dev99/setup.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/conf/global_conf.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/currency_connector.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/currency_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/datasource_plugin_connector.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/datasource_plugin_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/connector/smtp_connector.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/connector/smtp_connector.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/budget.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/budget.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/error/data_source.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/error/data_source.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/budget_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/budget_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/budget_usage_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/budget_usage_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/cost_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/cost_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/cost_query_set_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/cost_query_set_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/data_source_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/data_source_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/data_source_rule_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/data_source_rule_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/job_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/job_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/info/job_task_info.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/info/job_task_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/budget.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/budget.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/budget_usage.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/budget_usage.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_query_set.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_query_set.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report_config.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report_config.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/cost_report_data.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/cost_report_data.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/data_source.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/data_source.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/data_source_rule.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/data_source_rule.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/job.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/job.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/grpc/job_task.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/grpc/job_task.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/interface/task/v1/data_source_sync_scheduler.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/interface/task/v1/data_source_sync_scheduler.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/budget_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/budget_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/budget_usage_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/budget_usage_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_query_set_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_query_set_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_config_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_config_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_data_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_data_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/cost_report_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/cost_report_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/currency_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/currency_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_plugin_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/data_source_rule_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/data_source_rule_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/email_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/email_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/identity_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/job_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/job_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/job_task_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/job_task_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/notification_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/notification_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/plugin_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/repository_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/repository_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/manager/secret_manager.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/manager/secret_manager.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/budget_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/budget_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/budget_usage_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/budget_usage_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_query_set_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_query_set_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/database.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/request.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report/response.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/database.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/request.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_config/response.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_config/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/database.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/database.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/request.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/request.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/cost_report_data/response.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/cost_report_data/response.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/data_source_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/data_source_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/data_source_rule_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/data_source_rule_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/job_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/job_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/model/job_task_model.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/model/job_task_model.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/cost.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/cost.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/data_source.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/data_source.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/interface/grpc/job.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/interface/grpc/job.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/lib/server.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/lib/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/cost_response.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/cost_response.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/model/data_source_response.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/model/data_source_response.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/cost_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/cost_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/data_source_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/data_source_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/service/job_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/service/job_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/plugin/data_source/skeleton/main.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/plugin/data_source/skeleton/main.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/__init__.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/budget_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/budget_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/budget_usage_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/budget_usage_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_query_set_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_query_set_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_config_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_config_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_data_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_data_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_report_serivce.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_report_serivce.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/cost_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/cost_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/data_source_rule_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/data_source_rule_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/data_source_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/data_source_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/job_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/job_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/service/job_task_service.py` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/service/job_task_service.py`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_en.html` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_en.html`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_jp.html` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_jp.html`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone/cost_analysis/template/cost_report_ko.html` & `spaceone-cost-analysis-2.0.dev99/spaceone/cost_analysis/template/cost_report_ko.html`

 * *Files identical despite different names*

### Comparing `spaceone-cost-analysis-2.0.dev98/spaceone_cost_analysis.egg-info/SOURCES.txt` & `spaceone-cost-analysis-2.0.dev99/spaceone_cost_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

