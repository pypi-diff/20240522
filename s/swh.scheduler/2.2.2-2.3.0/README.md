# Comparing `tmp/swh.scheduler-2.2.2.tar.gz` & `tmp/swh_scheduler-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.scheduler-2.2.2.tar", last modified: Thu Mar 21 10:01:22 2024, max compression
+gzip compressed data, was "swh_scheduler-2.3.0.tar", last modified: Wed May 22 15:45:49 2024, max compression
```

## Comparing `swh.scheduler-2.2.2.tar` & `swh_scheduler-2.3.0.tar`

### file list

```diff
@@ -1,175 +1,175 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.101777 swh.scheduler-2.2.2/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)      977 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2630 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/LICENSE.Celery
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-03-21 10:01:22.101777 swh.scheduler-2.2.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/README.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.061777 swh.scheduler-2.2.2/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      646 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/data/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/data/elastic-template.json
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/data/update-index-settings.json
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.065777 swh.scheduler-2.2.2/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.065777 swh.scheduler-2.2.2/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.065777 swh.scheduler-2.2.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      887 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7879 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3060 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/docs/simulator.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      939 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1935 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/requirements-journal.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/requirements-simulator.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      187 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-03-21 10:01:22.101777 swh.scheduler-2.2.2/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.065777 swh.scheduler-2.2.2/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/sql/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1384 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/sql/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.053778 swh.scheduler-2.2.2/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.069777 swh.scheduler-2.2.2/swh/scheduler/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2195 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.069777 swh.scheduler-2.2.2/swh/scheduler/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/api/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      649 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      928 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/api/serializers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4203 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/api/server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    39106 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/backend.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.073777 swh.scheduler-2.2.2/swh/scheduler/celery_backend/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/celery_backend/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14058 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/celery_backend/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3320 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/celery_backend/pika_listener.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13254 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/celery_backend/recurrent_visits.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6758 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/celery_backend/runner.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.073777 swh.scheduler-2.2.2/swh/scheduler/cli/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3157 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5590 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/add_forge_now.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7552 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/admin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4791 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/celery_monitor.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1051 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2203 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/journal.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18449 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4985 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/origin_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2552 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/simulator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12725 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/task.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7676 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/task_type.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14932 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli/utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/cli_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2936 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/conftest.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      473 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    18240 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12011 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/journal_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8849 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3640 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.077777 swh.scheduler-2.2.2/swh/scheduler/simulator/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5691 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/simulator/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6293 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/simulator/common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2331 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/simulator/origin_scheduler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7801 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/simulator/origins.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2706 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/simulator/task_scheduler.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.077777 swh.scheduler-2.2.2/swh/scheduler/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10846 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)    14607 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/40-func.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.085777 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2111 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/02.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/03.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/04.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5119 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/05.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/06.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1727 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/07.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1924 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/08.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7034 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/09.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1581 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/10.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2070 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/11.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/12.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      967 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/13.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/14.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1126 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/15.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/16.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      152 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/17.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      328 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/18.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      958 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/19.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/20.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/23.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      471 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/24.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/25.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1478 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/26.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1113 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/27.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2112 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/28.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1241 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/29.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      224 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/30-bis.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2991 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/30.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      680 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/31.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2182 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/32.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3628 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/33.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/34.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/35.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/task.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3680 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/common.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/data/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/data/logging-config.yaml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/lister/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/lister/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/lister/foo/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/lister/foo/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/lister/foo/tasks.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/loader/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/loader/bar/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/loader/bar/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      381 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/fixtures/loader/bar/tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2568 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    11490 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_celery_tasks.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    24118 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5595 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_add_forge_now.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4174 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_celery_monitor.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2042 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3770 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_journal.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8514 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_origin.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1677 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_origin_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4347 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_task_type.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1624 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1952 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_common.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3859 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_config.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2836 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_init.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    30355 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2731 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_model.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8555 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_recurrent_visits.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    63287 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_scheduler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3532 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1967 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_simulator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      776 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_temporary.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5826 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3918 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/swh/scheduler/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-03-21 10:01:22.097777 swh.scheduler-2.2.2/swh.scheduler.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-03-21 10:01:21.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-03-21 10:01:22.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-03-21 10:01:21.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      106 2024-03-21 10:01:21.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      554 2024-03-21 10:01:21.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-03-21 10:01:21.000000 swh.scheduler-2.2.2/swh.scheduler.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1427 2024-03-21 10:01:15.000000 swh.scheduler-2.2.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      352 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      356 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1419 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       14 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2630 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/LICENSE.Celery
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      292 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/README.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      631 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.415625 swh_scheduler-2.3.0/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      646 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/elastic-template.json
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/data/update-index-settings.json
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.415625 swh_scheduler-2.3.0/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      887 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7664 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3060 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/docs/simulator.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      939 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1935 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       12 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-journal.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       21 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-simulator.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       48 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      187 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      465 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      120 2024-05-22 15:45:49.459625 swh_scheduler-2.3.0/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.419625 swh_scheduler-2.3.0/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       36 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1384 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/sql/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.403625 swh_scheduler-2.3.0/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.423625 swh_scheduler-2.3.0/swh/scheduler/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2195 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.427625 swh_scheduler-2.3.0/swh/scheduler/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      649 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      910 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/serializers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4203 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/api/server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    41268 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/backend.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.427625 swh_scheduler-2.3.0/swh/scheduler/celery_backend/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14088 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3283 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/pika_listener.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13221 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6779 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/celery_backend/runner.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.431625 swh_scheduler-2.3.0/swh/scheduler/cli/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3157 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5640 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/add_forge_now.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7546 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/admin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4826 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/celery_monitor.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1051 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2203 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/journal.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18286 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5089 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/origin_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2552 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/simulator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/task.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7914 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/task_type.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15189 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli/utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       62 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/cli_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2933 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/conftest.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      473 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    18935 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12008 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/journal_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14710 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3647 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.431625 swh_scheduler-2.3.0/swh/scheduler/simulator/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5652 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6293 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2349 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/origin_scheduler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7801 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/origins.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2754 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/simulator/task_scheduler.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.435625 swh_scheduler-2.3.0/swh/scheduler/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       44 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10846 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    14607 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/40-func.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      704 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.443625 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2111 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/02.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      661 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/03.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1561 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/04.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5119 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/05.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      625 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/06.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1727 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/07.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1924 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/08.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7034 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/09.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1581 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/10.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2070 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/11.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1769 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/12.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      967 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/13.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1729 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/14.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1126 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/15.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/16.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      152 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/17.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      328 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/18.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      958 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/19.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/20.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2467 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/23.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      471 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/24.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/25.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1478 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/26.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1113 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/27.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2112 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/28.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1241 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/29.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      224 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30-bis.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2991 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      680 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/31.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2182 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/32.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3628 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/33.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1738 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/34.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      617 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/35.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2944 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/task.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.451625 swh_scheduler-2.3.0/swh/scheduler/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3756 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/common.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.451625 swh_scheduler-2.3.0/swh/scheduler/tests/data/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      555 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/data/logging-config.yaml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      386 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/lister/foo/tasks.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      317 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      381 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/fixtures/loader/bar/tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1372 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2568 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    11224 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_celery_tasks.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    24334 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5688 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_add_forge_now.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4174 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_celery_monitor.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2042 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3770 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_journal.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8485 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1677 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4315 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_task_type.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1624 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2055 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3838 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2836 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    30355 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2731 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8371 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    62043 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_scheduler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3532 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1967 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_simulator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      776 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_temporary.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5947 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3915 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/swh/scheduler/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-22 15:45:49.455625 swh_scheduler-2.3.0/swh.scheduler.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2703 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4698 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      106 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      554 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-22 15:45:49.000000 swh_scheduler-2.3.0/swh.scheduler.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1199 2024-05-22 15:45:43.000000 swh_scheduler-2.3.0/tox.ini
```

### Comparing `swh.scheduler-2.2.2/CODE_OF_CONDUCT.md` & `swh_scheduler-2.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/LICENSE` & `swh_scheduler-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/LICENSE.Celery` & `swh_scheduler-2.3.0/LICENSE.Celery`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/PKG-INFO` & `swh_scheduler-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 2.2.2
+Version: 2.3.0
 Summary: Software Heritage scheduler
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-scheduler/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler.git
@@ -31,15 +31,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: sentry-sdk
 Requires-Dist: setuptools
 Requires-Dist: testing.postgresql
 Requires-Dist: typing-extensions
-Requires-Dist: swh.core[db,http]>=3.0.0
+Requires-Dist: swh.core[db,http]>=3.0.1
 Requires-Dist: swh.storage>=2.0.0
 Provides-Extra: journal
 Requires-Dist: swh.journal; extra == "journal"
 Provides-Extra: simulator
 Requires-Dist: plotille; extra == "simulator"
 Requires-Dist: simpy<4,>=3; extra == "simulator"
 Provides-Extra: testing
```

### Comparing `swh.scheduler-2.2.2/conftest.py` & `swh_scheduler-2.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/data/README.md` & `swh_scheduler-2.3.0/data/README.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/data/elastic-template.json` & `swh_scheduler-2.3.0/data/elastic-template.json`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/docs/cli.rst` & `swh_scheduler-2.3.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/docs/index.rst` & `swh_scheduler-2.3.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 .. _swh-scheduler:
 
 .. include:: README.rst
 
-Task manager for asynchronous/delayed tasks, used for both recurrent (e.g.,
-listing a forge, loading new stuff from a Git repository) and one-off
-activities (e.g., loading a specific version of a source package).
-
-
 Description
 -----------
 
 This module provides two independent scheduler services for the Software
 Heritage platform.
 
 The first one is a generic asynchronous task management system allowing to
```

### Comparing `swh.scheduler-2.2.2/docs/simulator.rst` & `swh_scheduler-2.3.0/docs/simulator.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/mypy.ini` & `swh_scheduler-2.3.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/pyproject.toml` & `swh_scheduler-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/sql/Makefile` & `swh_scheduler-2.3.0/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/__init__.py` & `swh_scheduler-2.3.0/swh/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/api/client.py` & `swh_scheduler-2.3.0/swh/scheduler/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/api/serializers.py` & `swh_scheduler-2.3.0/swh/scheduler/api/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Decoder and encoders for swh.scheduler.model objects."""
 
 from typing import Callable, Dict, List, Tuple
 
-import attr
-
 import swh.scheduler.model as model
 
 
 def _encode_model_object(obj):
-    d = attr.asdict(obj, recurse=False)
+    d = obj.to_dict(recurse=False)
     d["__type__"] = type(obj).__name__
     return d
 
 
 def _encode_enum(obj):
     return obj.value
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/api/server.py` & `swh_scheduler-2.3.0/swh/scheduler/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/backend.py` & `swh_scheduler-2.3.0/swh/scheduler/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 import json
 import logging
-from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 from uuid import UUID
 
 import attr
 from psycopg2.errors import CardinalityViolation
 from psycopg2.extensions import AsIs
 import psycopg2.extras
 import psycopg2.pool
 from testing.postgresql import Postgresql
 
 from swh.core.db import BaseDb
 from swh.core.db.common import db_transaction
 from swh.core.db.db_utils import init_admin_extensions, populate_database_for_package
+from swh.scheduler.model import (
+    Task,
+    TaskArguments,
+    TaskPolicy,
+    TaskPriority,
+    TaskRun,
+    TaskRunStatus,
+    TaskStatus,
+    TaskType,
+)
 from swh.scheduler.utils import utcnow
 
 from .exc import SchedulerException, StaleData, UnknownPolicy
 from .interface import ListedOriginPageToken, PaginatedListedOriginList
 from .model import (
     LastVisitStatus,
     ListedOrigin,
@@ -39,23 +49,28 @@
 
 
 psycopg2.extensions.register_adapter(dict, psycopg2.extras.Json)
 psycopg2.extensions.register_adapter(LastVisitStatus, adapt_LastVisitStatus)
 psycopg2.extras.register_uuid()
 
 
-def format_query(query, keys):
+def format_query(query: str, keys: Sequence[str]) -> str:
     """Format a query with the given keys"""
 
     query_keys = ", ".join(keys)
     placeholders = ", ".join(["%s"] * len(keys))
 
     return query.format(keys=query_keys, placeholders=placeholders)
 
 
+def mutate_task_dict(task_dict: Dict[str, Any]) -> Dict[str, Any]:
+    task_dict["arguments"] = TaskArguments(**task_dict["arguments"])
+    return task_dict
+
+
 class SchedulerBackend:
     """Backend for the Software Heritage scheduling database."""
 
     current_version = 35
 
     def __init__(self, db, min_pool_conns=1, max_pool_conns=10):
         """
@@ -80,78 +95,52 @@
             return self._db
         return BaseDb.from_pool(self._pool)
 
     def put_db(self, db):
         if db is not self._db:
             db.put_conn()
 
-    task_type_keys = [
-        "type",
-        "description",
-        "backend_name",
-        "default_interval",
-        "min_interval",
-        "max_interval",
-        "backoff_factor",
-        "max_queue_length",
-        "num_retries",
-        "retry_delay",
-    ]
+    task_type_keys = [field.name for field in attr.fields(TaskType)]
 
     @db_transaction()
-    def create_task_type(self, task_type, db=None, cur=None):
+    def create_task_type(self, task_type: TaskType, db=None, cur=None) -> None:
         """Create a new task type ready for scheduling.
 
         Args:
-            task_type (dict): a dictionary with the following keys:
-
-                - type (str): an identifier for the task type
-                - description (str): a human-readable description of what the
-                  task does
-                - backend_name (str): the name of the task in the
-                  job-scheduling backend
-                - default_interval (datetime.timedelta): the default interval
-                  between two task runs
-                - min_interval (datetime.timedelta): the minimum interval
-                  between two task runs
-                - max_interval (datetime.timedelta): the maximum interval
-                  between two task runs
-                - backoff_factor (float): the factor by which the interval
-                  changes at each run
-                - max_queue_length (int): the maximum length of the task queue
-                  for this task type
-
+            task_type: a TaskType dictionary
         """
-        keys = [key for key in self.task_type_keys if key in task_type]
         query = format_query(
             """insert into task_type ({keys}) values ({placeholders})
             on conflict do nothing""",
-            keys,
+            self.task_type_keys,
         )
-        cur.execute(query, [task_type[key] for key in keys])
+        cur.execute(query, task_type.to_tuple())
 
     @db_transaction()
-    def get_task_type(self, task_type_name, db=None, cur=None):
+    def get_task_type(
+        self, task_type_name: str, db=None, cur=None
+    ) -> Optional[TaskType]:
         """Retrieve the task type with id task_type_name"""
         query = format_query(
             "select {keys} from task_type where type=%s",
             self.task_type_keys,
         )
         cur.execute(query, (task_type_name,))
-        return cur.fetchone()
+        row = cur.fetchone()
+        return TaskType(**row) if row is not None else None
 
     @db_transaction()
-    def get_task_types(self, db=None, cur=None):
+    def get_task_types(self, db=None, cur=None) -> List[TaskType]:
         """Retrieve all registered task types"""
         query = format_query(
             "select {keys} from task_type",
             self.task_type_keys,
         )
         cur.execute(query)
-        return cur.fetchall()
+        return [TaskType(**row) for row in cur.fetchall()]
 
     @db_transaction()
     def get_listers(self, db=None, cur=None) -> List[Lister]:
         """Retrieve information about all listers from the database."""
 
         select_cols = ", ".join(Lister.select_columns())
 
@@ -231,15 +220,15 @@
             )
             select {select_cols} from added
           union all
             select {select_cols} from listers
               where (name, instance_name) = (%(name)s, %(instance_name)s);
         """
 
-        cur.execute(query, attr.asdict(Lister(name=name, instance_name=instance_name)))
+        cur.execute(query, Lister(name=name, instance_name=instance_name).to_dict())
 
         return Lister(**cur.fetchone())
 
     @db_transaction()
     def update_lister(self, lister: Lister, db=None, cur=None) -> Lister:
         """Update the state for the given lister instance in the database.
 
@@ -258,15 +247,15 @@
         )
 
         query = f"""update listers
                       set {set_vars}
                       where id=%(id)s and updated=%(updated)s
                       returning {select_cols}"""
 
-        cur.execute(query, attr.asdict(lister))
+        cur.execute(query, lister.to_dict())
         updated = cur.fetchone()
 
         if not updated:
             raise StaleData("Stale data; Lister state not updated")
 
         return Lister(**updated)
 
@@ -299,15 +288,15 @@
                        SET {upsert_set}
                     RETURNING {", ".join(select_cols)}
         """
 
         ret = psycopg2.extras.execute_values(
             cur=cur,
             sql=query,
-            argslist=(attr.asdict(origin) for origin in deduplicated_origins.values()),
+            argslist=(origin.to_dict() for origin in deduplicated_origins.values()),
             template=f"({', '.join(insert_meta)})",
             page_size=1000,
             fetch=True,
         )
 
         return [ListedOrigin(**d) for d in ret]
 
@@ -589,107 +578,123 @@
             FROM
               selected_origins
         """
 
         cur.execute(query, tuple(query_args))
         return [ListedOrigin(**d) for d in cur]
 
+    task_keys = [field.name for field in attr.fields(Task)]
     task_create_keys = [
-        "type",
-        "arguments",
-        "next_run",
-        "policy",
-        "status",
-        "retries_left",
-        "priority",
+        key for key in task_keys if key not in {"id", "current_interval"}
     ]
-    task_keys = task_create_keys + ["id", "current_interval"]
 
     @db_transaction()
-    def create_tasks(self, tasks, policy="recurring", db=None, cur=None):
+    def create_tasks(
+        self, tasks: List[Task], policy: TaskPolicy = "recurring", db=None, cur=None
+    ) -> List[Task]:
         """Create new tasks.
 
         Args:
-            tasks (list): each task is a dictionary with the following keys:
+            tasks: each task is a Task object created with at least the following parameters:
 
-                - type (str): the task type
-                - arguments (dict): the arguments for the task runner, keys:
+                - type
+                - arguments
+                - next_run
 
-                      - args (list of str): arguments
-                      - kwargs (dict str -> str): keyword arguments
-
-                - next_run (datetime.datetime): the next scheduled run for the
-                  task
+            policy: default task policy (either recurring or oneshot) to use if not
+                set in input task objects
 
         Returns:
-            a list of created tasks.
+            a list of created tasks with database ids filled
 
         """
         cur.execute("select swh_scheduler_mktemp_task()")
         db.copy_to(
-            tasks,
+            (task.to_dict() for task in tasks),
             "tmp_task",
             self.task_create_keys,
-            default_values={"policy": policy, "status": "next_run_not_scheduled"},
+            default_values={"policy": policy},
             cur=cur,
         )
         query = format_query(
             "select {keys} from swh_scheduler_create_tasks_from_temp()",
             self.task_keys,
         )
         cur.execute(query)
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
     def set_status_tasks(
         self,
         task_ids: List[int],
-        status: str = "disabled",
+        status: TaskStatus = "disabled",
         next_run: Optional[datetime.datetime] = None,
         db=None,
         cur=None,
-    ):
+    ) -> None:
         """Set the tasks' status whose ids are listed.
 
-        If given, also set the next_run date.
+        Args:
+            task_ids: list of tasks' identifiers
+            status: the status to set for the tasks
+            next_run: if provided, also set the next_run date
+
         """
         if not task_ids:
             return
         query = ["UPDATE task SET status = %s"]
         args: List[Any] = [status]
         if next_run:
             query.append(", next_run = %s")
             args.append(next_run)
         query.append(" WHERE id IN %s")
         args.append(tuple(task_ids))
 
         cur.execute("".join(query), args)
 
     @db_transaction()
-    def disable_tasks(self, task_ids, db=None, cur=None):
-        """Disable the tasks whose ids are listed."""
-        return self.set_status_tasks(task_ids, db=db, cur=cur)
+    def disable_tasks(self, task_ids: List[int], db=None, cur=None) -> None:
+        """Disable the tasks whose ids are listed.
+
+        Args:
+            task_ids: list of tasks' identifiers
+        """
+        self.set_status_tasks(task_ids, db=db, cur=cur)
 
     @db_transaction()
     def search_tasks(
         self,
-        task_id=None,
-        task_type=None,
-        status=None,
-        priority=None,
-        policy=None,
-        before=None,
-        after=None,
-        limit=None,
+        task_id: Optional[int] = None,
+        task_type: Optional[str] = None,
+        status: Optional[TaskStatus] = None,
+        priority: Optional[TaskPriority] = None,
+        policy: Optional[TaskPolicy] = None,
+        before: Optional[datetime.datetime] = None,
+        after: Optional[datetime.datetime] = None,
+        limit: Optional[int] = None,
         db=None,
         cur=None,
-    ):
-        """Search tasks from selected criterions"""
+    ) -> List[Task]:
+        """Search tasks from selected criterions
+
+        Args:
+            task_id: search a task with given identifier
+            task_type: search tasks with given type
+            status: search tasks with given status
+            priority: search tasks with given priority
+            policy: search tasks with given policy
+            before: search tasks created before given date
+            after: search tasks created after given date
+            limit: maximum number of tasks to return
+
+        Returns:
+            a list of found tasks
+        """
         where = []
-        args = []
+        args: List[Any] = []
 
         if task_id:
             if isinstance(task_id, (str, int)):
                 where.append("id = %s")
             else:
                 where.append("id in %s")
                 task_id = tuple(task_id)
@@ -728,219 +733,285 @@
         query = "select * from task"
         if where:
             query += " where " + " and ".join(where)
         if limit:
             query += " limit %s :: bigint"
             args.append(limit)
         cur.execute(query, args)
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
-    def get_tasks(self, task_ids, db=None, cur=None):
-        """Retrieve the info of tasks whose ids are listed."""
+    def get_tasks(self, task_ids: List[int], db=None, cur=None) -> List[Task]:
+        """Retrieve the info of tasks whose ids are listed.
+
+        Args:
+            task_ids: list of tasks' identifiers
+
+        Returns:
+            a list of Task objects
+        """
         query = format_query("select {keys} from task where id in %s", self.task_keys)
         cur.execute(query, (tuple(task_ids),))
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
     def peek_ready_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
         db=None,
         cur=None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
+        """Fetch the list of tasks (with no priority) to be scheduled.
+
+        Args:
+            task_type: filtering task per their type
+            timestamp: peek tasks that need to be executed
+                before that timestamp
+            num_tasks: only peek at num_tasks tasks (with no priority)
+
+        Returns:
+            the list of tasks which would be scheduled
+
+        """
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             """select * from swh_scheduler_peek_no_priority_tasks(
                 %s, %s, %s :: bigint)""",
             (task_type, timestamp, num_tasks),
         )
         logger.debug("PEEK %s => %s" % (task_type, cur.rowcount))
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
     def grab_ready_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
         db=None,
         cur=None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
+        """Fetch and schedule the list of tasks (with no priority) ready to be scheduled.
+
+        Args:
+            task_type: filtering task per their type
+            timestamp: grab tasks that need to be executed
+                before that timestamp
+            num_tasks: only grab num_tasks tasks (with no priority)
+
+        Returns:
+            the list of scheduled tasks
+
+        """
         if timestamp is None:
             timestamp = utcnow()
         cur.execute(
             """select * from swh_scheduler_grab_ready_tasks(
                  %s, %s, %s :: bigint)""",
             (task_type, timestamp, num_tasks),
         )
         logger.debug("GRAB %s => %s" % (task_type, cur.rowcount))
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
     def peek_ready_priority_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
         db=None,
         cur=None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
+        """Fetch list of tasks (with any priority) ready to be scheduled.
+
+        Args:
+            task_type: filtering task per their type
+            timestamp: peek tasks that need to be executed before that timestamp
+            num_tasks: only peek at num_tasks tasks (with no priority)
+
+        Returns:
+            the list of tasks which would be scheduled
+
+        """
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             """select * from swh_scheduler_peek_any_ready_priority_tasks(
                 %s, %s, %s :: bigint)""",
             (task_type, timestamp, num_tasks),
         )
         logger.debug("PEEK %s => %s", task_type, cur.rowcount)
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     @db_transaction()
     def grab_ready_priority_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
         db=None,
         cur=None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
+        """Fetch and schedule the list of tasks (with any priority) ready to be scheduled.
+
+        Args:
+            task_type: filtering task per their type
+            timestamp: grab tasks that need to be executed
+                before that timestamp
+            num_tasks: only grab num_tasks tasks (with no priority)
+
+        Returns:
+            the list of scheduled tasks
+
+        """
         if timestamp is None:
             timestamp = utcnow()
         cur.execute(
             """select * from swh_scheduler_grab_any_ready_priority_tasks(
                  %s, %s, %s :: bigint)""",
             (task_type, timestamp, num_tasks),
         )
         logger.debug("GRAB %s => %s", task_type, cur.rowcount)
-        return cur.fetchall()
+        return [Task(**mutate_task_dict(row)) for row in cur.fetchall()]
 
     task_run_create_keys = ["task", "backend_id", "scheduled", "metadata"]
 
     @db_transaction()
     def schedule_task_run(
-        self, task_id, backend_id, metadata=None, timestamp=None, db=None, cur=None
-    ):
+        self,
+        task_id: int,
+        backend_id: str,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
+        db=None,
+        cur=None,
+    ) -> TaskRun:
         """Mark a given task as scheduled, adding a task_run entry in the database.
 
         Args:
-            task_id (int): the identifier for the task being scheduled
-            backend_id (str): the identifier of the job in the backend
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            task_id: the identifier for the task being scheduled
+            backend_id: the identifier of the job in the backend
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            a fresh task_run entry
+            a TaskRun object
 
         """
 
         if metadata is None:
             metadata = {}
 
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_schedule_task_run(%s, %s, %s, %s)",
             (task_id, backend_id, metadata, timestamp),
         )
 
-        return cur.fetchone()
+        return TaskRun(**cur.fetchone())
 
     @db_transaction()
-    def mass_schedule_task_runs(self, task_runs, db=None, cur=None):
+    def mass_schedule_task_runs(
+        self, task_runs: List[TaskRun], db=None, cur=None
+    ) -> None:
         """Schedule a bunch of task runs.
 
         Args:
-            task_runs (list): a list of dicts with keys:
-
-                - task (int): the identifier for the task being scheduled
-                - backend_id (str): the identifier of the job in the backend
-                - metadata (dict): metadata to add to the task_run entry
-                - scheduled (datetime.datetime): the instant the event occurred
+            task_runs: a list of TaskRun objects created at least with the following parameters:
 
-        Returns:
-            None
+                - task
+                - backend_id
+                - scheduled
         """
         cur.execute("select swh_scheduler_mktemp_task_run()")
-        db.copy_to(task_runs, "tmp_task_run", self.task_run_create_keys, cur=cur)
+        db.copy_to(
+            (task_run.to_dict() for task_run in task_runs),
+            "tmp_task_run",
+            self.task_run_create_keys,
+            cur=cur,
+        )
         cur.execute("select swh_scheduler_schedule_task_run_from_temp()")
 
     @db_transaction()
     def start_task_run(
-        self, backend_id, metadata=None, timestamp=None, db=None, cur=None
-    ):
+        self,
+        backend_id: str,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
+        db=None,
+        cur=None,
+    ) -> TaskRun:
         """Mark a given task as started, updating the corresponding task_run
            entry in the database.
 
         Args:
-            backend_id (str): the identifier of the job in the backend
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            backend_id: the identifier of the job in the backend
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            the updated task_run entry
+            a TaskRun object with updated fields
 
         """
 
         if metadata is None:
             metadata = {}
 
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_start_task_run(%s, %s, %s)",
             (backend_id, metadata, timestamp),
         )
 
-        return cur.fetchone()
+        return TaskRun(**cur.fetchone())
 
     @db_transaction()
     def end_task_run(
         self,
-        backend_id,
-        status,
-        metadata=None,
-        timestamp=None,
-        result=None,
+        backend_id: str,
+        status: TaskRunStatus,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
         db=None,
         cur=None,
-    ):
+    ) -> TaskRun:
         """Mark a given task as ended, updating the corresponding task_run entry in the
         database.
 
         Args:
-            backend_id (str): the identifier of the job in the backend
-            status (str): how the task ended; one of: 'eventful', 'uneventful',
-                'failed'
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            backend_id: the identifier of the job in the backend
+            status: how the task ended
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            the updated task_run entry
+            a TaskRun object with updated fields
 
         """
 
         if metadata is None:
             metadata = {}
 
         if timestamp is None:
             timestamp = utcnow()
 
         cur.execute(
             "select * from swh_scheduler_end_task_run(%s, %s, %s, %s)",
             (backend_id, status, metadata, timestamp),
         )
-        return cur.fetchone()
+        return TaskRun(**cur.fetchone())
 
     @db_transaction()
     def filter_task_to_archive(
         self,
         after_ts: str,
         before_ts: str,
         limit: int = 10,
@@ -1017,35 +1088,28 @@
         "started",
         "ended",
         "metadata",
         "status",
     ]
 
     @db_transaction()
-    def get_task_runs(self, task_ids, limit=None, db=None, cur=None):
+    def get_task_runs(
+        self, task_ids: List[int], limit: Optional[int] = None, db=None, cur=None
+    ) -> List[TaskRun]:
         """Search task run for a task id"""
-        where = []
-        args = []
-
         if task_ids:
-            if isinstance(task_ids, (str, int)):
-                where.append("task = %s")
-            else:
-                where.append("task in %s")
-                task_ids = tuple(task_ids)
-            args.append(task_ids)
+            args: List[Any] = [tuple(task_ids)]
+            query = "select * from task_run where task in %s"
+            if limit:
+                query += " limit %s :: bigint"
+                args.append(limit)
+            cur.execute(query, args)
+            return [TaskRun(**row) for row in cur.fetchall()]
         else:
-            return ()
-
-        query = "select * from task_run where " + " and ".join(where)
-        if limit:
-            query += " limit %s :: bigint"
-            args.append(limit)
-        cur.execute(query, args)
-        return cur.fetchall()
+            return []
 
     @db_transaction()
     def origin_visit_stats_upsert(
         self, origin_visit_stats: Iterable[OriginVisitStats], db=None, cur=None
     ) -> None:
         pk_cols = OriginVisitStats.primary_key_columns()
         insert_cols, insert_meta = OriginVisitStats.insert_columns_and_metavars()
@@ -1062,17 +1126,15 @@
             SET {upsert_set}
         """
 
         try:
             psycopg2.extras.execute_values(
                 cur=cur,
                 sql=query,
-                argslist=(
-                    attr.asdict(visit_stats) for visit_stats in origin_visit_stats
-                ),
+                argslist=(visit_stats.to_dict() for visit_stats in origin_visit_stats),
                 template=f"({', '.join(insert_meta)})",
                 page_size=1000,
                 fetch=False,
             )
         except CardinalityViolation as e:
             raise SchedulerException(repr(e))
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/celery_backend/config.py` & `swh_scheduler-2.3.0/swh/scheduler/celery_backend/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,33 +160,37 @@
     for these task classes.
 
     """
     logger.info("Setup Queues & Tasks for %s", sender)
     instance.app.conf["worker_name"] = sender
 
 
-def _init_sentry(sentry_dsn: str, main_package: Optional[str] = None):
+def _init_sentry(sentry_dsn: Optional[str] = None, main_package: Optional[str] = None):
     try:
         from sentry_sdk.integrations.celery import CeleryIntegration
     except ImportError:
         integrations = []
     else:
         integrations = [CeleryIntegration()]
-    init_sentry(sentry_dsn, integrations=integrations, main_package=main_package)
+    init_sentry(
+        sentry_dsn,
+        integrations=integrations,
+        main_package=main_package,
+        deferred_init=sentry_dsn is None,
+    )
 
 
 @worker_init.connect
 @_print_errors
 def on_worker_init(*args, **kwargs):
-    # use a fake sentry DSN to ensure celery integration for sentry is
-    # properly configured as it must happen in the worker_init signal
-    # callback, real sentry DSN is then setup in task_prerun signal
-    # callback (see celery_task_prerun function below)
-    sentry_dsn = "https://public@sentry.example.org/1"
-    _init_sentry(sentry_dsn)
+    # init sentry with no DSN first to ensure celery integration for sentry is
+    # properly configured as it must happen in the worker_init signal callback,
+    # real sentry DSN is then setup in task_prerun signal callback
+    # (see celery_task_prerun function below)
+    _init_sentry()
 
     if "pytest" in sys.argv[0] or "PYTEST_XDIST_WORKER" in os.environ:
         # when pytest collects tests, it breaks the proper configuration
         # of the celery integration as a side effect, so we ensure that
         # the celery.worker.consumer.build_tracer function gets overridden
         # as it should have be
         from celery.app import trace
@@ -270,15 +274,15 @@
 
     try:
         queue_length = get_queue_length(app, queue_name)
         # Clamp the return value to MAX_NUM_TASKS
         max_val = max(0, min(max_length - queue_length, MAX_NUM_TASKS))
     except (ValueError, TypeError):
         # Unknown queue length, just schedule all the tasks
-        max_val = MAX_NUM_TASKS
+        max_val = max_length
 
     return max_val
 
 
 def register_task_class(app, name, cls):
     """Register a class-based task under the given name"""
     if name in app.tasks:
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/celery_backend/pika_listener.py` & `swh_scheduler-2.3.0/swh/scheduler/celery_backend/pika_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,15 @@
             status = result["status"]
             if status == "success":
                 status = "eventful" if result.get("eventful") else "uneventful"
 
         if status is None:
             status = "eventful" if result else "uneventful"
 
-        scheduler_backend.end_task_run(
-            uuid, timestamp=utcnow(), status=status, result=result
-        )
+        scheduler_backend.end_task_run(uuid, timestamp=utcnow(), status=status)
     elif event_type == "task-failed":
         scheduler_backend.end_task_run(uuid, timestamp=utcnow(), status="failed")
 
 
 if __name__ == "__main__":
     url = sys.argv[1]
     logging.basicConfig(level=logging.DEBUG)
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/celery_backend/recurrent_visits.py` & `swh_scheduler-2.3.0/swh/scheduler/celery_backend/recurrent_visits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 The Software Heritage developers
+# Copyright (C) 2021-2024 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """This schedules the recurrent visits, for listed origins, in Celery.
 
 For "oneshot" (save code now, lister) tasks, check the
@@ -20,19 +20,19 @@
 from threading import Thread
 import time
 from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 from kombu.utils.uuid import uuid
 
 from swh.scheduler.celery_backend.config import get_available_slots
-from swh.scheduler.utils import create_origin_task_dicts
+from swh.scheduler.utils import create_origin_tasks
 
 if TYPE_CHECKING:
     from ..interface import SchedulerInterface
-    from ..model import ListedOrigin
+    from ..model import ListedOrigin, TaskType
 
 logger = logging.getLogger(__name__)
 
 
 DEFAULT_POLICY = [
     {"policy": "already_visited_order_by_lag", "weight": 40},
     {"policy": "never_visited_oldest_update_first", "weight": 40},
@@ -170,15 +170,15 @@
     return random.uniform(0, BACKOFF_SPLAY)
 
 
 def send_visits_for_visit_type(
     scheduler: SchedulerInterface,
     app,
     visit_type: str,
-    task_type: Dict,
+    task_type: TaskType,
     policy_cfg: List[Dict[str, Any]],
     no_origins_scheduled_backoff: int = DEFAULT_NO_ORIGINS_SCHEDULED_BACKOFF,
 ) -> float:
     """Schedule the next batch of visits for the given ``visit_type``.
 
     First, we determine the number of available slots by introspecting the RabbitMQ
     queue.
@@ -202,16 +202,16 @@
     :py:func:`grab_next_visits_policy_weights()` function.
 
     Returns:
        the earliest :py:func:`time.monotonic` value at which to run the next iteration
        of the loop.
 
     """
-    queue_name = task_type["backend_name"]
-    max_queue_length = task_type.get("max_queue_length") or 0
+    queue_name = task_type.backend_name
+    max_queue_length = task_type.max_queue_length or 0
     min_available_slots = max_queue_length * MIN_SLOTS_RATIO
 
     current_iteration_start = time.monotonic()
 
     # Check queue level
     available_slots = get_available_slots(app, queue_name, max_queue_length)
     logger.debug(
@@ -231,20 +231,20 @@
         logger.debug("No origins to visit for type %s", visit_type)
         return current_iteration_start + no_origins_scheduled_backoff
 
     # Try to smooth the ingestion load, origins pulled by different
     # scheduling policies have different resource usage patterns
     random.shuffle(origins)
 
-    for task_dict in create_origin_task_dicts(origins, scheduler):
+    for task in create_origin_tasks(origins, scheduler):
         app.send_task(
             queue_name,
             task_id=uuid(),
-            args=task_dict["arguments"]["args"],
-            kwargs=task_dict["arguments"]["kwargs"],
+            args=task.arguments.args,
+            kwargs=task.arguments.kwargs,
             queue=queue_name,
         )
 
     logger.info(
         "%s: %s visits scheduled in queue %s",
         visit_type,
         len(origins),
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/celery_backend/runner.py` & `swh_scheduler-2.3.0/swh/scheduler/celery_backend/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015-2021 The Software Heritage developers
+# Copyright (C) 2015-2024 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """This is the first scheduler runner. It is in charge of scheduling "oneshot" tasks
 (e.g save code now, indexer, vault, deposit, ...). To do this, it reads tasks ouf of the
 scheduler backend and pushes those to their associated rabbitmq queues.
@@ -18,28 +18,29 @@
 from deprecated import deprecated
 from kombu.utils.uuid import uuid
 
 from swh.core.statsd import statsd
 from swh.scheduler import get_scheduler
 from swh.scheduler.celery_backend.config import get_available_slots
 from swh.scheduler.interface import SchedulerInterface
+from swh.scheduler.model import TaskRun, TaskType
 from swh.scheduler.utils import utcnow
 
 logger = logging.getLogger(__name__)
 
 # Max batch size for tasks
 MAX_NUM_TASKS = 10000
 
 
 def run_ready_tasks(
     backend: SchedulerInterface,
     app,
-    task_types: List[Dict] = [],
+    task_types: List[TaskType] = [],
     with_priority: bool = False,
-) -> List[Dict]:
+) -> List[TaskRun]:
     """Schedule tasks ready to be scheduled.
 
     This lookups any tasks per task type and mass schedules those accordingly (send
     messages to rabbitmq and mark as scheduled equivalent tasks in the scheduler
     backend).
 
     If tasks (per task type) with priority exist, they will get redirected to dedicated
@@ -66,27 +67,27 @@
         The result can be used to block-wait for the tasks' results::
 
           backend_tasks = run_ready_tasks(self.scheduler, app)
           for task in backend_tasks:
               AsyncResult(id=task['backend_id']).get()
 
     """
-    all_backend_tasks: List[Dict] = []
+    all_backend_tasks: List[TaskRun] = []
     while True:
         if not task_types:
             task_types = backend.get_task_types()
         task_types_d = {}
         pending_tasks = []
         for task_type in task_types:
-            task_type_name = task_type["type"]
+            task_type_name = task_type.type
             task_types_d[task_type_name] = task_type
-            max_queue_length = task_type["max_queue_length"]
+            max_queue_length = task_type.max_queue_length
             if max_queue_length is None:
                 max_queue_length = 0
-            backend_name = task_type["backend_name"]
+            backend_name = task_type.backend_name
 
             if with_priority:
                 # grab max_queue_length (or 10) potential tasks with any priority for
                 # the same type (limit the result to avoid too long running queries)
                 grabbed_priority_tasks = backend.grab_ready_priority_tasks(
                     task_type_name, num_tasks=max_queue_length or 10
                 )
@@ -124,33 +125,33 @@
 
         if not pending_tasks:
             return all_backend_tasks
 
         backend_tasks = []
         celery_tasks: List[Tuple[bool, str, str, List, Dict]] = []
         for task in pending_tasks:
-            args = task["arguments"]["args"]
-            kwargs = task["arguments"]["kwargs"]
+            args = task.arguments.args
+            kwargs = task.arguments.kwargs
 
-            backend_name = task_types_d[task["type"]]["backend_name"]
+            backend_name = task_types_d[task.type].backend_name
             backend_id = uuid()
             celery_tasks.append(
                 (
-                    task.get("priority") is not None,
+                    task.priority is not None,
                     backend_name,
                     backend_id,
                     args,
                     kwargs,
                 )
             )
-            data = {
-                "task": task["id"],
-                "backend_id": backend_id,
-                "scheduled": utcnow(),
-            }
+            data = TaskRun(
+                task=task.id,
+                backend_id=backend_id,
+                scheduled=utcnow(),
+            )
 
             backend_tasks.append(data)
         logger.debug("Sent %s celery tasks", len(backend_tasks))
 
         backend.mass_schedule_task_runs(backend_tasks)
         for with_priority, backend_name, backend_id, args, kwargs in celery_tasks:
             kw = dict(
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/__init__.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/add_forge_now.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/add_forge_now.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import click
 
 from . import cli
 
 if TYPE_CHECKING:
     from typing import Dict, List, Optional
 
+    from swh.scheduler.model import TaskPolicy
+
 
 @cli.group("add-forge-now")
 @click.option(
     "-p",
     "--preset",
     "preset",
     default="production",
@@ -85,19 +87,19 @@
         ctx.fail(f"Unknown lister type {lister_name}.")
 
     (args, kw) = parse_options(options)
 
     max_pages = kw.get("max_pages", 2)
     max_origins_per_page = kw.get("max_origins_per_page", 5)
 
+    policy: TaskPolicy = "oneshot"
     # Recurring policy on production
     if preset == "production":
         policy = "recurring"
     else:  # staging, "full" but limited listing as a oneshot
-        policy = "oneshot"
         kw.update(
             {
                 "max_pages": max_pages,
                 "max_origins_per_page": max_origins_per_page,
                 "enable_origins": False,
             }
         )
@@ -110,15 +112,15 @@
     from swh.scheduler.utils import utcnow
 
     for listing_type, task_type in task_types.items():
         now = utcnow()
         next_run = now + timedelta(days=1) if listing_type == "incremental" else now
         task_add(
             scheduler,
-            task_type_name=task_type["type"],
+            task_type_name=task_type.type,
             args=args,
             kw=kw,
             policy=policy,
             next_run=next_run,
         )
 
 
@@ -166,15 +168,15 @@
     visit_type_to_queue: Dict[str, str] = {}
     unknown_task_types = []
     for visit_type_name in visit_type_names:
         task_type = get_task_type(scheduler, visit_type_name)
         if not task_type:
             unknown_task_types.append(visit_type_name)
             continue
-        queue_name = task_type["backend_name"]
+        queue_name = task_type.backend_name
         visit_type_to_queue[visit_type_name] = f"{queue_name_prefix}:{queue_name}"
 
     if unknown_task_types:
         ctx.fail(f"Unknown task types {','.join(unknown_task_types)}.")
 
     send_to_celery(
         scheduler,
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/admin.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,19 +163,19 @@
     scheduler = ctx.obj["scheduler"]
 
     if not visit_types:
         visit_types = []
         # Figure out which visit types exist in the scheduler
         all_task_types = scheduler.get_task_types()
         for task_type in all_task_types:
-            if not task_type["type"].startswith("load-"):
+            if not task_type.type.startswith("load-"):
                 # only consider loading tasks as recurring ones, the rest is dismissed
                 continue
             # get visit type name from task type
-            visit_types.append(task_type["type"][5:])
+            visit_types.append(task_type.type[5:])
     else:
         # Check that the passed visit types exist in the scheduler
         for visit_type in visit_types:
             task_type_name = f"load-{visit_type}"
             task_type = scheduler.get_task_type(task_type_name)
             if not task_type:
                 ctx.fail(f"Unknown task type: {task_type_name}")
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/celery_monitor.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/celery_monitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,15 @@
     type=click.Choice(["pretty", "csv"]),
 )
 @click.pass_context
 def list_running(ctx: click.Context, format: str):
     """List running tasks on the lister workers"""
     from ast import literal_eval
     import csv
+    from operator import itemgetter
 
     response_times = {}
 
     def active_callback(response):
         rtt = time.monotonic() - active_time
         for destination in response:
             response_times[destination] = rtt
@@ -150,11 +151,11 @@
         ctx.exit(127)
 
     for worker, active in sorted(ret.items()):
         if not active:
             logger.info("%s: no active tasks", worker)
             continue
 
-        for task in sorted(active, key=lambda t: t["time_start"]):
+        for task in sorted(active, key=itemgetter("time_start")):
             output(get_task_data(worker, task))
 
     ctx.exit(0)
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/config.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/journal.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/origin.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/origin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import click
 
 from . import cli
-from ..utils import create_origin_task_dicts
+from ..utils import create_origin_tasks
 
 if TYPE_CHECKING:
     from typing import Dict, Iterable, List, Optional
     from uuid import UUID
 
-    from ..interface import SchedulerInterface
+    from ..interface import SchedulerInterface, TaskPolicy
     from ..model import ListedOrigin
 
 
 @cli.group("origin")
 @click.pass_context
 def origin(ctx):
     """Manipulate listed origins."""
@@ -89,15 +89,20 @@
     default=True,
     help="Print the CSV header?",
 )
 @click.argument("type", type=str)
 @click.argument("count", type=int)
 @click.pass_context
 def grab_next(
-    ctx, policy: str, fields: Optional[str], with_header: bool, type: str, count: int
+    ctx,
+    policy: TaskPolicy,
+    fields: Optional[str],
+    with_header: bool,
+    type: str,
+    count: int,
 ):
     """Grab the next COUNT origins to visit using the TYPE loader from the
     listed origins table."""
 
     if fields:
         parsed_fields: Optional[List[str]] = fields.split(",")
     else:
@@ -115,33 +120,32 @@
 @origin.command("schedule-next")
 @click.option(
     "--policy", "-p", default="oldest_scheduled_first", help="Scheduling policy"
 )
 @click.argument("type", type=str)
 @click.argument("count", type=int)
 @click.pass_context
-def schedule_next(ctx, policy: str, type: str, count: int):
+def schedule_next(ctx, policy: TaskPolicy, type: str, count: int):
     """Send the next COUNT origin visits of the TYPE loader to the scheduler as
     one-shot tasks."""
     from ..utils import utcnow
     from .utils import pretty_print_task
 
     scheduler = ctx.obj["scheduler"]
 
     origins = scheduler.grab_next_visits(type, count, policy=policy)
 
     created = scheduler.create_tasks(
         [
-            {
-                **task_dict,
-                "policy": "oneshot",
-                "next_run": utcnow(),
-                "retries_left": 1,
-            }
-            for task_dict in create_origin_task_dicts(origins, scheduler)
+            task.evolve(
+                policy="oneshot",
+                next_run=utcnow(),
+                retries_left=1,
+            )
+            for task in create_origin_tasks(origins, scheduler)
         ]
     )
 
     output = ["Created %d tasks\n" % len(created)]
     for task in created:
         output.append(pretty_print_task(task))
 
@@ -242,15 +246,15 @@
     scheduler = ctx.obj["scheduler"]
 
     task_type = get_task_type(scheduler, visit_type_name)
     if not task_type:
         ctx.fail(f"Unknown task type {task_type}.")
         assert False  # for mypy
 
-    queue_name = queue or task_type["backend_name"]
+    queue_name = queue or task_type.backend_name
 
     send_to_celery(
         scheduler,
         visit_type_to_queue={visit_type_name: queue_name},
         policy=policy,
         tablesample=tablesample,
         enabled=enabled,
@@ -275,30 +279,28 @@
     Examples:
        swh scheduler origin update-metrics
        swh scheduler origin update-metrics --lister github
        swh scheduler origin update-metrics --lister phabricator --instance llvm
     """
     import json
 
-    import attr
-
     scheduler: SchedulerInterface = ctx.obj["scheduler"]
 
     lister_id: Optional[UUID] = None
     if lister is not None:
         lister_instance = scheduler.get_lister(name=lister, instance_name=instance)
         if not lister_instance:
             click.echo(f"Lister not found: {lister} instance={instance}")
             ctx.exit(2)
             assert False  # for mypy
 
         lister_id = lister_instance.id
 
     def dictify_metrics(d):
-        return {k: str(v) for (k, v) in attr.asdict(d).items()}
+        return {k: str(v) for (k, v) in d.to_dict().items()}
 
     ret = scheduler.update_metrics(lister_id=lister_id)
     click.echo(json.dumps(list(map(dictify_metrics, ret)), indent=4, sort_keys=True))
 
 
 @origin.command("check-listed-origins")
 @click.option(
@@ -516,39 +518,39 @@
     from time import sleep
 
     from swh.scheduler.celery_backend.config import app, get_available_slots
     from swh.scheduler.cli.utils import parse_options
 
     from .origin_utils import (
         TASK_ARGS_GENERATOR_CALLABLES,
-        get_scheduler_task_info,
+        get_scheduler_task_type,
         lines_to_task_args,
     )
 
     scheduler = ctx.obj["scheduler"]
 
     try:
-        task_info = get_scheduler_task_info(scheduler, task_type)
+        task_type_info = get_scheduler_task_type(scheduler, task_type)
     except ValueError as e:
         ctx.fail(e)
 
     if debug:
-        click.echo(f"Scheduler task information: {task_info}")
+        click.echo(f"Scheduler task information: {task_type_info}")
 
-    celery_task_name = task_info["backend_name"]
+    celery_task_name = task_type_info.backend_name
     if queue_name_prefix:
         queue_name = f"{queue_name_prefix}:{celery_task_name}"
     else:
         queue_name = celery_task_name
 
     if debug:
         click.echo(f"Destination queue: {queue_name}")
 
     if not threshold:
-        threshold = task_info.get("max_queue_length") or 1000
+        threshold = task_type_info.max_queue_length
 
     # Compute the callable function to generate the tasks to schedule. Tasks are read
     # out of the file_input.
     task_fn = partial(
         TASK_ARGS_GENERATOR_CALLABLES.get(
             task_type, partial(lines_to_task_args, columns=["url"])
         ),
@@ -567,19 +569,17 @@
         remains_data = False
         pending_tasks = []
 
         if limit_reached:
             break
 
         # we can send new tasks, compute how many we can send
-        queue_length = get_available_slots(app, queue_name, 1000)
-        nb_tasks_to_send = abs(threshold - queue_length) if queue_length else threshold
+        nb_tasks_to_send = get_available_slots(app, queue_name, threshold)
 
         if debug:
-            click.echo(f"Destination queue length: {queue_length}")
             click.echo(f"Nb tasks to send : {nb_tasks_to_send}")
 
         if nb_tasks_to_send > 0:
             count = 0
             for _task in task_fn(**extra_kwargs):
                 pending_tasks.append(_task)
                 count += 1
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/origin_utils.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/origin_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,46 @@
 from functools import partial
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional
 
     from swh.scheduler.interface import SchedulerInterface
+    from swh.scheduler.model import TaskType
 
 
-def get_scheduler_task_info(scheduler: SchedulerInterface, task_type: str) -> Dict:
-    """Retrieve information on task_type from the scheduler.
+def get_scheduler_task_type(
+    scheduler: SchedulerInterface, task_type_name: str
+) -> TaskType:
+    """Retrieve a TaskType instance for a task type name from the scheduler.
 
     Args:
         scheduler: Scheduler instance to lookup data from
-        task_type: The task type to lookup
+        task_type_name: The task type name to lookup
 
     Raises:
-        ValueError when task_type and its fallback is not found.
+        ValueError when task_type_name or its fallback are not found.
 
     Returns:
-        Dict of information for the task type
+        Information about the task type
 
     """
-    origin_task_type = task_type
+    origin_task_type_name = task_type_name
     # Lookup standard scheduler task (e.g. load-git, load-hg, ...)
-    scheduler_info = scheduler.get_task_type(task_type)
+    scheduler_info = scheduler.get_task_type(task_type_name)
     while True:
         if scheduler_info:
-            return dict(scheduler_info)
+            return scheduler_info
         # Lookup task type derivative (e.g. load-git-large, load-hg-bitbucket, ...)
-        new_scheduler_task_type = task_type.rsplit("-", 1)[0]
-        if new_scheduler_task_type == task_type:
-            error_msg = f"Could not find scheduler <{origin_task_type}> task type"
+        new_task_type_name = task_type_name.rsplit("-", 1)[0]
+        if new_task_type_name == task_type_name:
+            error_msg = f"Could not find scheduler <{origin_task_type_name}> task type"
             raise ValueError(error_msg)
-        task_type = new_scheduler_task_type
-        scheduler_info = scheduler.get_task_type(task_type)
+        task_type_name = new_task_type_name
+        scheduler_info = scheduler.get_task_type(task_type_name)
 
 
 def lines_to_task_args(
     lines: Iterable[str],
     columns: List[str] = ["url"],
     postprocess: Optional[Callable[[Dict[str, Any]], Dict[str, Any]]] = None,
     **kwargs,
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/simulator.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/task.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2016-2021  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from __future__ import annotations
 
 # WARNING: do not import unnecessary things here to keep cli startup time under
@@ -79,33 +79,40 @@
                 task schedule \\
                     --columns type --columns kwargs --columns policy \\
                     --delimiter ';' -
     """
     import csv
     import json
 
+    import iso8601
+
+    from swh.scheduler.model import Task, TaskArguments
     from swh.scheduler.utils import utcnow
 
     from .utils import pretty_print_task
 
     tasks = []
     now = utcnow()
     scheduler = ctx.obj["scheduler"]
 
     reader = csv.reader(file, delimiter=delimiter)
     for line in reader:
-        task = dict(zip(columns, line))
-        args = json.loads(task.pop("args", "[]"))
-        kwargs = json.loads(task.pop("kwargs", "{}"))
-        task["arguments"] = {
-            "args": args,
-            "kwargs": kwargs,
-        }
-        task["next_run"] = task.get("next_run", now)
-        tasks.append(task)
+        task_params = dict(zip(columns, line))
+        args = json.loads(task_params.pop("args", "[]"))
+        kwargs = json.loads(task_params.pop("kwargs", "{}"))
+        task_params["arguments"] = TaskArguments(
+            args=args,
+            kwargs=kwargs,
+        )
+        task_params["next_run"] = (
+            iso8601.parse_date(task_params["next_run"])
+            if "next_run" in task_params
+            else now
+        )
+        tasks.append(Task(**task_params))
 
     created = scheduler.create_tasks(tasks)
 
     output = [
         "Created %d tasks\n" % len(created),
     ]
     for task in created:
@@ -376,22 +383,22 @@
     help="Also list past executions of each task.",
 )
 @click.pass_context
 def list_tasks(
     ctx, task_id, task_type, limit, status, policy, priority, before, after, list_runs
 ):
     """List tasks."""
-    from operator import itemgetter
+    from operator import attrgetter
 
     from .utils import pretty_print_run, pretty_print_task
 
     scheduler = ctx.obj["scheduler"]
 
     if not task_type:
-        task_type = [x["type"] for x in scheduler.get_task_types()]
+        task_type = [x.type for x in scheduler.get_task_types()]
 
     # if task_id is not given, default value for status is
     #  'next_run_not_scheduled'
     # if task_id is given, default status is 'all'
     if task_id is None and status is None:
         status = ["next_run_not_scheduled"]
     if status and "all" in status:
@@ -408,26 +415,26 @@
         priority=priority,
         policy=policy,
         before=before,
         after=after,
         limit=limit,
     )
     if list_runs:
-        runs = {t["id"]: [] for t in tasks}
-        for r in scheduler.get_task_runs([task["id"] for task in tasks]):
-            runs[r["task"]].append(r)
+        runs = {t.id: [] for t in tasks}
+        for r in scheduler.get_task_runs([task.id for task in tasks]):
+            runs[r.task].append(r)
     else:
         runs = {}
 
     output.append("Found %d tasks\n" % (len(tasks)))
-    for task in sorted(tasks, key=itemgetter("id")):
+    for task in sorted(tasks, key=attrgetter("id")):
         output.append(pretty_print_task(task, full=True))
-        if runs.get(task["id"]):
+        if runs.get(task.id):
             output.append(click.style("  Executions:", bold=True))
-            for run in sorted(runs[task["id"]], key=itemgetter("id")):
+            for run in sorted(runs[task.id], key=attrgetter("id")):
                 output.append(pretty_print_run(run, indent=4))
 
     click.echo("\n".join(output))
 
 
 @task.command("respawn")
 @click.argument("task-ids", required=True, nargs=-1)
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/task_type.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/task_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,47 @@
-# Copyright (C) 2016-2019  The Software Heritage developers
+# Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
+from __future__ import annotations
+
+from datetime import timedelta
 from importlib import import_module
 import logging
-from typing import Mapping
+from typing import TYPE_CHECKING, Any, Dict
 
 # WARNING: do not import unnecessary things here to keep cli startup time under
 # control
 import click
 from pkg_resources import iter_entry_points
 
+from swh.scheduler.model import TaskType
+
+if TYPE_CHECKING:
+    from swh.scheduler.task import SWHTask
+
 from . import cli
 
 logger = logging.getLogger(__name__)
 
 
-DEFAULT_TASK_TYPE = {
-    "full": {  # for tasks like 'list_xxx_full()'
-        "default_interval": "90 days",
-        "min_interval": "90 days",
-        "max_interval": "90 days",
-        "backoff_factor": 1,
-    },
-    "*": {  # value if not suffix matches
-        "default_interval": "1 day",
-        "min_interval": "1 day",
-        "max_interval": "1 day",
-        "backoff_factor": 1,
-    },
+DEFAULT_TASK_TYPE_PARAMETERS = {
+    "full": dict(  # for tasks like 'list_xxx_full()'
+        default_interval=timedelta(days=90),
+        min_interval=timedelta(days=90),
+        max_interval=timedelta(days=90),
+        backoff_factor=1.0,
+    ),
+    "*": dict(  # value if not suffix matches
+        default_interval=timedelta(days=1),
+        min_interval=timedelta(days=1),
+        max_interval=timedelta(days=1),
+        backoff_factor=1.0,
+    ),
 }
 
 
 def _plugin_worker_descriptions():
     return {
         entry_point.name: entry_point
         for entry_point in iter_entry_points("swh.workers")
@@ -69,14 +77,16 @@
     "-n",
     multiple=True,
     default=None,
     help="List task types of given backend task name",
 )
 @click.pass_context
 def list_task_types(ctx, verbose, task_type, task_name):
+    from operator import attrgetter
+
     click.echo("Known task types:")
     if verbose:
         tmpl = (
             click.style("{type}: ", bold=True)
             + """{backend_name}
   {description}
   interval: {default_interval} [{min_interval}, {max_interval}]
@@ -85,21 +95,21 @@
   num_retries: {num_retries}
   retry_delay: {retry_delay}
 """
         )
     else:
         tmpl = "{type}:\n  {description}"
     for tasktype in sorted(
-        ctx.obj["scheduler"].get_task_types(), key=lambda x: x["type"]
+        ctx.obj["scheduler"].get_task_types(), key=attrgetter("type")
     ):
-        if task_type and tasktype["type"] not in task_type:
+        if task_type and tasktype.type not in task_type:
             continue
-        if task_name and tasktype["backend_name"] not in task_name:
+        if task_name and tasktype.backend_name not in task_name:
             continue
-        click.echo(tmpl.format(**tasktype))
+        click.echo(tmpl.format(**tasktype.to_dict()))
 
 
 @task_type.command("register")
 @click.option(
     "--plugins",
     "-p",
     "plugins",
@@ -147,60 +157,66 @@
                 if isinstance(taskobj, celery.app.task.Task):
                     tt_name = task_name.replace("_", "-")
                     task_cfg = registry_entry.get("task_types", {}).get(tt_name, {})
                     ensure_task_type(task_module, tt_name, taskobj, task_cfg, scheduler)
 
 
 def ensure_task_type(
-    task_module: str, task_type: str, swhtask, task_config: Mapping, scheduler
+    task_module: str,
+    task_type_name: str,
+    swhtask: SWHTask,
+    task_config: Dict[str, Any],
+    scheduler,
 ):
     """Ensure a given task-type (for the task_module) exists in the scheduler.
 
     Args:
         task_module: task module we are currently checking for task type
             consistency
         task_type: the type of the task to check/insert (correspond to
             the 'type' field in the db)
-        swhtask (SWHTask): the SWHTask instance the task-type correspond to
+        swhtask: the SWHTask instance the task-type correspond to
         task_config: a dict with specific/overloaded values for the
             task-type to be created
         scheduler: the scheduler object used to access the scheduler db
 
     """
-    for suffix, defaults in DEFAULT_TASK_TYPE.items():
-        if task_type.endswith("-" + suffix):
-            task_type_dict = defaults.copy()
+    task_type_params = dict(
+        type=task_type_name,
+        backend_name=swhtask.name,
+        description=swhtask.__doc__,
+    )
+    for suffix, defaults in DEFAULT_TASK_TYPE_PARAMETERS.items():
+        if task_type_name.endswith("-" + suffix):
+            task_type_params.update(defaults)
             break
     else:
-        task_type_dict = DEFAULT_TASK_TYPE["*"].copy()
+        task_type_params.update(DEFAULT_TASK_TYPE_PARAMETERS["*"])
 
-    task_type_dict["type"] = task_type
-    task_type_dict["backend_name"] = swhtask.name
-    if swhtask.__doc__:
-        task_type_dict["description"] = swhtask.__doc__.splitlines()[0]
+    task_type_params.update(task_config)
 
-    task_type_dict.update(task_config)
+    task_type = TaskType(**task_type_params)
 
-    current_task_type = scheduler.get_task_type(task_type)
+    current_task_type = scheduler.get_task_type(task_type_name)
     if current_task_type:
         # Ensure the existing task_type is consistent in the scheduler
-        if current_task_type["backend_name"] != task_type_dict["backend_name"]:
+        if current_task_type.backend_name != task_type.backend_name:
             logger.warning(
                 "Existing task type %s for module %s has a "
                 "different backend name than current "
                 "code version provides (%s vs. %s)",
                 task_type,
                 task_module,
-                current_task_type["backend_name"],
-                task_type_dict["backend_name"],
+                current_task_type.backend_name,
+                task_type.backend_name,
             )
     else:
-        logger.info("Create task type %s in scheduler", task_type)
-        logger.debug("  %s", task_type_dict)
-        scheduler.create_task_type(task_type_dict)
+        logger.info("Create task type %s in scheduler", task_type_name)
+        logger.debug("  %s", task_type)
+        scheduler.create_task_type(task_type)
 
 
 @task_type.command("add")
 @click.argument("type", required=True)
 @click.argument("task-name", required=True)
 @click.argument("description", required=True)
 @click.option(
@@ -229,21 +245,18 @@
     description,
     default_interval,
     min_interval,
     max_interval,
     backoff_factor,
 ):
     """Create a new task type"""
-    task_type = dict(
+    task_type = TaskType(
         type=type,
         backend_name=task_name,
         description=description,
         default_interval=default_interval,
         min_interval=min_interval,
         max_interval=max_interval,
         backoff_factor=backoff_factor,
-        max_queue_length=None,
-        num_retries=None,
-        retry_delay=None,
     )
     ctx.obj["scheduler"].create_task_type(task_type)
     click.echo("OK")
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/cli/utils.py` & `swh_scheduler-2.3.0/swh/scheduler/cli/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 # See top-level LICENSE file for more information
 
 # WARNING: do not import unnecessary things here to keep cli startup time under
 # control
 
 from __future__ import annotations
 
-from datetime import timedelta
+from datetime import datetime, timedelta
 import re
 from typing import TYPE_CHECKING, Iterable
 
 import click
 
+from swh.scheduler.model import Task
+
 if TYPE_CHECKING:
-    from typing import Dict, List, Optional, Tuple
+    from typing import Any, Dict, List, Optional, Tuple
 
     from swh.scheduler.interface import SchedulerInterface
+    from swh.scheduler.model import TaskPolicy, TaskPriority, TaskRun, TaskType
 
 
 TASK_BATCH_SIZE = 1000  # Number of tasks per query to the scheduler
 
 
 TIME_INTERVAL_REGEXP = re.compile(
     r"""
@@ -81,15 +84,15 @@
         raise ValueError(f"{time_str!r} could not be parsed as a time interval")
     return timedelta(**time_params)
 
 
 def schedule_origin_batches(scheduler, task_type, origins, origin_batch_size, kwargs):
     from itertools import islice
 
-    from swh.scheduler.utils import create_task_dict
+    from swh.scheduler.utils import create_task
 
     nb_origins = 0
     nb_tasks = 0
 
     while True:
         task_batch = []
         for _ in range(TASK_BATCH_SIZE):
@@ -99,15 +102,15 @@
                 origin_batch.append(origin)
             nb_origins += len(origin_batch)
             if not origin_batch:
                 break
 
             # Create a task for these origins
             args = [origin_batch]
-            task_dict = create_task_dict(task_type, "oneshot", *args, **kwargs)
+            task_dict = create_task(task_type, "oneshot", *args, **kwargs)
             task_batch.append(task_dict)
 
         # Schedule a batch of tasks
         if not task_batch:
             break
         nb_tasks += len(task_batch)
         if scheduler:
@@ -169,15 +172,15 @@
     """
     kw_pairs = [x.split("=", 1) for x in options if "=" in x]
     args = [parse_argument(x) for x in options if "=" not in x]
     kw = {k: parse_argument(v) for (k, v) in kw_pairs}
     return (args, kw)
 
 
-def get_task_type(scheduler: SchedulerInterface, visit_type: str) -> Optional[Dict]:
+def get_task_type(scheduler: SchedulerInterface, visit_type: str) -> Optional[TaskType]:
     "Given a visit type, return its associated task type."
     return scheduler.get_task_type(f"load-{visit_type}")
 
 
 def send_to_celery(
     scheduler: SchedulerInterface,
     visit_type_to_queue: Dict[str, str],
@@ -216,21 +219,21 @@
 
     """
 
     from kombu.utils.uuid import uuid
 
     from swh.scheduler.celery_backend.config import app, get_available_slots
 
-    from ..utils import create_origin_task_dicts
+    from ..utils import create_origin_tasks
 
     for visit_type_name, queue_name in visit_type_to_queue.items():
         task_type = get_task_type(scheduler, visit_type_name)
         assert task_type is not None
-        task_name = task_type["backend_name"]
-        num_tasks = get_available_slots(app, queue_name, task_type["max_queue_length"])
+        task_name = task_type.backend_name
+        num_tasks = get_available_slots(app, queue_name, task_type.max_queue_length)
 
         click.echo(f"{num_tasks} slots available in celery queue")
 
         origins = scheduler.grab_next_visits(
             visit_type_name,
             num_tasks,
             policy=policy,
@@ -241,30 +244,30 @@
             absolute_cooldown=absolute_cooldown,
             scheduled_cooldown=scheduled_cooldown,
             failed_cooldown=failed_cooldown,
             not_found_cooldown=not_found_cooldown,
         )
 
         click.echo(f"{len(origins)} visits to send to celery")
-        for task_dict in create_origin_task_dicts(origins, scheduler):
+        for task in create_origin_tasks(origins, scheduler):
             app.send_task(
                 task_name,
                 task_id=uuid(),
-                args=task_dict["arguments"]["args"],
-                kwargs=task_dict["arguments"]["kwargs"],
+                args=task.arguments.args,
+                kwargs=task.arguments.kwargs,
                 queue=queue_name,
             )
 
 
-def pretty_print_list(list, indent=0):
+def pretty_print_list(list: List[Any], indent: int = 0):
     """Pretty-print a list"""
     return "".join("%s%r\n" % (" " * indent, item) for item in list)
 
 
-def pretty_print_dict(dict, indent=0):
+def pretty_print_dict(dict: Dict[str, Any], indent: int = 0):
     """Pretty-print a list"""
     return "".join(
         "%s%s: %r\n" % (" " * indent, click.style(key, bold=True), value)
         for key, value in sorted(dict.items())
     )
 
 
@@ -278,41 +281,42 @@
             v = v.isoformat()
         elif isinstance(v, dict):
             v = format_dict(v)
         ret[k] = v
     return ret
 
 
-def pretty_print_run(run, indent=4):
+def pretty_print_run(run: TaskRun, indent: int = 4):
     fmt = (
         "{indent}{backend_id} [{status}]\n"
         "{indent}  scheduled: {scheduled} [{started}:{ended}]"
     )
-    return fmt.format(indent=" " * indent, **format_dict(run))
+    return fmt.format(indent=" " * indent, **format_dict(run.to_dict()))
 
 
-def pretty_print_task(task, full=False):
+def pretty_print_task(task: Task, full: bool = False):
     """Pretty-print a task
 
-    If 'full' is True, also print the status and priority fields.
+    If ``full`` is :const:`True`, also print the status and priority fields.
 
     >>> import datetime
-    >>> task = {
-    ...     'id': 1234,
-    ...     'arguments': {
-    ...         'args': ['foo', 'bar', True],
-    ...         'kwargs': {'key': 'value', 'key2': 42},
-    ...     },
-    ...     'current_interval': datetime.timedelta(hours=1),
-    ...     'next_run': datetime.datetime(2019, 2, 21, 13, 52, 35, 407818),
-    ...     'policy': 'oneshot',
-    ...     'priority': None,
-    ...     'status': 'next_run_not_scheduled',
-    ...     'type': 'test_task',
-    ... }
+    >>> from swh.scheduler.model import Task, TaskArguments
+    >>> task = Task(
+    ...     id=1234,
+    ...     arguments=TaskArguments(
+    ...         args=["foo", "bar", True],
+    ...         kwargs={"key": "value", "key2": 42},
+    ...     ),
+    ...     current_interval=datetime.timedelta(hours=1),
+    ...     next_run=datetime.datetime(2019, 2, 21, 13, 52, 35, 407818),
+    ...     policy="oneshot",
+    ...     priority=None,
+    ...     status="next_run_not_scheduled",
+    ...     type="test_task",
+    ... )
     >>> print(click.unstyle(pretty_print_task(task)))
     Task 1234
       Next run: ... (2019-02-21T13:52:35.407818)
       Interval: 1:00:00
       Type: test_task
       Policy: oneshot
       Args:
@@ -338,71 +342,72 @@
       Keyword args:
         key: 'value'
         key2: 42
     <BLANKLINE>
     """
     import humanize
 
-    next_run = task["next_run"]
+    next_run = task.next_run
     lines = [
-        "%s %s\n" % (click.style("Task", bold=True), task["id"]),
+        "%s %s\n" % (click.style("Task", bold=True), task.id),
         click.style("  Next run: ", bold=True),
         "%s (%s)" % (humanize.naturaldate(next_run), next_run.isoformat()),
         "\n",
         click.style("  Interval: ", bold=True),
-        str(task["current_interval"]),
+        str(task.current_interval),
         "\n",
         click.style("  Type: ", bold=True),
-        task["type"] or "",
+        task.type or "",
         "\n",
         click.style("  Policy: ", bold=True),
-        task["policy"] or "",
+        task.policy or "",
         "\n",
     ]
     if full:
         lines += [
             click.style("  Status: ", bold=True),
-            task["status"] or "",
+            task.status or "",
             "\n",
             click.style("  Priority: ", bold=True),
-            task["priority"] or "",
+            task.priority or "",
             "\n",
         ]
     lines += [
         click.style("  Args:\n", bold=True),
-        pretty_print_list(task["arguments"]["args"], indent=4),
+        pretty_print_list(task.arguments.args, indent=4),
         click.style("  Keyword args:\n", bold=True),
-        pretty_print_dict(task["arguments"]["kwargs"], indent=4),
+        pretty_print_dict(task.arguments.kwargs, indent=4),
     ]
 
     return "".join(lines)
 
 
 def task_add(
     scheduler: SchedulerInterface,
     task_type_name: str,
     args: List[str],
     kw: Dict,
-    policy: str,
-    priority: Optional[str] = None,
-    next_run: Optional[str] = None,
+    policy: TaskPolicy,
+    priority: Optional[TaskPriority] = None,
+    next_run: Optional[datetime] = None,
 ):
     """Add a task task_type_name in the scheduler."""
+    from swh.scheduler.model import TaskArguments
     from swh.scheduler.utils import utcnow
 
-    task = {
-        "type": task_type_name,
-        "policy": policy,
-        "priority": priority,
-        "arguments": {
-            "args": args,
-            "kwargs": kw,
-        },
-        "next_run": next_run or utcnow(),
-    }
+    task = Task(
+        type=task_type_name,
+        policy=policy,
+        priority=priority,
+        arguments=TaskArguments(
+            args=args,
+            kwargs=kw,
+        ),
+        next_run=next_run or utcnow(),
+    )
     created = scheduler.create_tasks([task])
 
     output = [f"Created {len(created)} tasks\n"]
     for task in created:
         output.append(pretty_print_task(task))
 
     click.echo("\n".join(output))
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/conftest.py` & `swh_scheduler-2.3.0/swh/scheduler/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,9 +92,9 @@
 @pytest.fixture
 def task_types(swh_scheduler):
     from swh.scheduler.tests.common import TASK_TYPES
 
     all_task_types = {}
     for task_type in TASK_TYPES.values():
         swh_scheduler.create_task_type(task_type)
-        all_task_types[task_type["type"]] = task_type
+        all_task_types[task_type.type] = task_type
     return all_task_types
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/interface.py` & `swh_scheduler-2.3.0/swh/scheduler/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,34 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 import datetime
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 from uuid import UUID
 
 from typing_extensions import Protocol, runtime_checkable
 
 from swh.core.api import remote_api_endpoint
 from swh.core.api.classes import PagedResult
-from swh.scheduler.model import ListedOrigin, Lister, OriginVisitStats, SchedulerMetrics
+from swh.scheduler.model import (
+    ListedOrigin,
+    Lister,
+    OriginVisitStats,
+    SchedulerMetrics,
+    Task,
+    TaskPolicy,
+    TaskPriority,
+    TaskRun,
+    TaskRunStatus,
+    TaskStatus,
+    TaskType,
+)
 
 ListedOriginPageToken = Tuple[str, str]
 
 
 class PaginatedListedOriginList(PagedResult[ListedOrigin, ListedOriginPageToken]):
     """A list of listed origins, with a continuation token"""
 
@@ -32,116 +44,140 @@
             parsed_next_page_token = tuple(next_page_token)  # type: ignore
         super().__init__(results, parsed_next_page_token)
 
 
 @runtime_checkable
 class SchedulerInterface(Protocol):
     @remote_api_endpoint("task_type/create")
-    def create_task_type(self, task_type):
-        """Create a new task type ready for scheduling.
+    def create_task_type(self, task_type: TaskType) -> None:
+        """Create a new task type in database ready for scheduling.
 
         Args:
-            task_type (dict): a dictionary with the following keys:
-
-                - type (str): an identifier for the task type
-                - description (str): a human-readable description of what the
-                  task does
-                - backend_name (str): the name of the task in the
-                  job-scheduling backend
-                - default_interval (datetime.timedelta): the default interval
-                  between two task runs
-                - min_interval (datetime.timedelta): the minimum interval
-                  between two task runs
-                - max_interval (datetime.timedelta): the maximum interval
-                  between two task runs
-                - backoff_factor (float): the factor by which the interval
-                  changes at each run
-                - max_queue_length (int): the maximum length of the task queue
-                  for this task type
-
+            task_type: a TaskType object
         """
         ...
 
     @remote_api_endpoint("task_type/get")
-    def get_task_type(self, task_type_name):
-        """Retrieve the task type with id task_type_name"""
+    def get_task_type(self, task_type_name: str) -> Optional[TaskType]:
+        """Retrieve the registered task type with a given name
+
+        Args:
+            task_type_name: name of the task type to retrieve
+
+        Returns:
+            a TaskType object or :const:`None` if no such task type exists
+        """
         ...
 
     @remote_api_endpoint("task_type/get_all")
-    def get_task_types(self):
-        """Retrieve all registered task types"""
+    def get_task_types(self) -> List[TaskType]:
+        """Retrieve all registered task types
+
+        Returns:
+            a list of TaskType objects
+        """
         ...
 
     @remote_api_endpoint("task/create")
-    def create_tasks(self, tasks, policy="recurring"):
-        """Create new tasks.
+    def create_tasks(
+        self, tasks: List[Task], policy: TaskPolicy = "recurring"
+    ) -> List[Task]:
+        """Register new tasks in database.
 
         Args:
-            tasks (list): each task is a dictionary with the following keys:
+            tasks: each task is a Task object created with at least the following parameters:
 
-                - type (str): the task type
-                - arguments (dict): the arguments for the task runner, keys:
+                - type
+                - arguments
+                - next_run
 
-                      - args (list of str): arguments
-                      - kwargs (dict str -> str): keyword arguments
+            policy: default task policy (either recurring or oneshot) to use if not
+                set in input task objects
 
-                - next_run (datetime.datetime): the next scheduled run for the
-                  task
 
         Returns:
-            a list of created tasks.
+            a list of created tasks with database ids filled.
 
         """
         ...
 
     @remote_api_endpoint("task/set_status")
     def set_status_tasks(
         self,
         task_ids: List[int],
-        status: str = "disabled",
+        status: TaskStatus = "disabled",
         next_run: Optional[datetime.datetime] = None,
-    ):
+    ) -> None:
         """Set the tasks' status whose ids are listed.
 
-        If given, also set the next_run date.
+        Args:
+            task_ids: list of tasks' identifiers
+            status: the status to set for the tasks
+            next_run: if provided, also set the next_run date
+
         """
         ...
 
     @remote_api_endpoint("task/disable")
-    def disable_tasks(self, task_ids):
-        """Disable the tasks whose ids are listed."""
+    def disable_tasks(self, task_ids: List[int]) -> None:
+        """Disable the tasks whose ids are listed.
+
+        Args:
+            task_ids: list of tasks' identifiers
+        """
         ...
 
     @remote_api_endpoint("task/search")
     def search_tasks(
         self,
-        task_id=None,
-        task_type=None,
-        status=None,
-        priority=None,
-        policy=None,
-        before=None,
-        after=None,
-        limit=None,
-    ):
-        """Search tasks from selected criterions"""
+        task_id: Optional[int] = None,
+        task_type: Optional[str] = None,
+        status: Optional[TaskStatus] = None,
+        priority: Optional[TaskPriority] = None,
+        policy: Optional[TaskPolicy] = None,
+        before: Optional[datetime.datetime] = None,
+        after: Optional[datetime.datetime] = None,
+        limit: Optional[int] = None,
+    ) -> List[Task]:
+        """Search tasks from selected criterions
+
+        Args:
+            task_id: search a task with given identifier
+            task_type: search tasks with given type
+            status: search tasks with given status
+            priority: search tasks with given priority
+            policy: search tasks with given policy
+            before: search tasks created before given date
+            after: search tasks created after given date
+            limit: maximum number of tasks to return
+
+        Returns:
+            a list of found tasksa
+        """
         ...
 
     @remote_api_endpoint("task/get")
-    def get_tasks(self, task_ids):
-        """Retrieve the info of tasks whose ids are listed."""
+    def get_tasks(self, task_ids: List[int]) -> List[Task]:
+        """Retrieve the info of tasks whose ids are listed.
+
+        Args:
+            task_ids: list of tasks' identifiers
+
+        Returns:
+            a list of tasks
+        """
         ...
 
     @remote_api_endpoint("task/peek_ready")
     def peek_ready_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
         """Fetch the list of tasks (with no priority) to be scheduled.
 
         Args:
             task_type: filtering task per their type
             timestamp: peek tasks that need to be executed
                 before that timestamp
             num_tasks: only peek at num_tasks tasks (with no priority)
@@ -154,15 +190,15 @@
 
     @remote_api_endpoint("task/grab_ready")
     def grab_ready_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
         """Fetch and schedule the list of tasks (with no priority) ready to be scheduled.
 
         Args:
             task_type: filtering task per their type
             timestamp: grab tasks that need to be executed
                 before that timestamp
             num_tasks: only grab num_tasks tasks (with no priority)
@@ -175,119 +211,125 @@
 
     @remote_api_endpoint("task/peek_ready_with_priority")
     def peek_ready_priority_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
         """Fetch list of tasks (with any priority) ready to be scheduled.
 
         Args:
             task_type: filtering task per their type
             timestamp: peek tasks that need to be executed before that timestamp
             num_tasks: only peek at num_tasks tasks (with no priority)
 
         Returns:
-            a list of tasks
+            the list of tasks which would be scheduled
 
         """
         ...
 
     @remote_api_endpoint("task/grab_ready_with_priority")
     def grab_ready_priority_tasks(
         self,
         task_type: str,
         timestamp: Optional[datetime.datetime] = None,
         num_tasks: Optional[int] = None,
-    ) -> List[Dict]:
+    ) -> List[Task]:
         """Fetch and schedule the list of tasks (with any priority) ready to be scheduled.
 
         Args:
             task_type: filtering task per their type
             timestamp: grab tasks that need to be executed
                 before that timestamp
             num_tasks: only grab num_tasks tasks (with no priority)
 
         Returns:
-            a list of tasks
+            the list of scheduled tasks
 
         """
         ...
 
     @remote_api_endpoint("task_run/schedule_one")
-    def schedule_task_run(self, task_id, backend_id, metadata=None, timestamp=None):
+    def schedule_task_run(
+        self,
+        task_id: int,
+        backend_id: str,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
+    ) -> TaskRun:
         """Mark a given task as scheduled, adding a task_run entry in the database.
 
         Args:
-            task_id (int): the identifier for the task being scheduled
-            backend_id (str): the identifier of the job in the backend
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            task_id: the identifier for the task being scheduled
+            backend_id: the identifier of the job in the backend
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            a fresh task_run entry
+            a TaskRun object
 
         """
         ...
 
     @remote_api_endpoint("task_run/schedule")
-    def mass_schedule_task_runs(self, task_runs):
+    def mass_schedule_task_runs(self, task_runs: List[TaskRun]) -> None:
         """Schedule a bunch of task runs.
 
         Args:
-            task_runs (list): a list of dicts with keys:
+            task_runs: a list of TaskRun objects created at least with the following parameters:
 
-                - task (int): the identifier for the task being scheduled
-                - backend_id (str): the identifier of the job in the backend
-                - metadata (dict): metadata to add to the task_run entry
-                - scheduled (datetime.datetime): the instant the event occurred
+                - task
+                - backend_id
+                - scheduled
 
-        Returns:
-            None
         """
         ...
 
     @remote_api_endpoint("task_run/start")
-    def start_task_run(self, backend_id, metadata=None, timestamp=None):
+    def start_task_run(
+        self,
+        backend_id: str,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
+    ) -> TaskRun:
         """Mark a given task as started, updating the corresponding task_run
            entry in the database.
 
         Args:
-            backend_id (str): the identifier of the job in the backend
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            backend_id: the identifier of the job in the backend
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            the updated task_run entry
+            a TaskRun object with updated fields
 
         """
         ...
 
     @remote_api_endpoint("task_run/end")
     def end_task_run(
         self,
-        backend_id,
-        status,
-        metadata=None,
-        timestamp=None,
-        result=None,
-    ):
+        backend_id: str,
+        status: TaskRunStatus,
+        metadata: Optional[Dict[str, Any]] = None,
+        timestamp: Optional[datetime.datetime] = None,
+    ) -> TaskRun:
         """Mark a given task as ended, updating the corresponding task_run entry in the
         database.
 
         Args:
-            backend_id (str): the identifier of the job in the backend
-            status (str): how the task ended; one of: 'eventful', 'uneventful',
-                'failed'
-            metadata (dict): metadata to add to the task_run entry
-            timestamp (datetime.datetime): the instant the event occurred
+            backend_id: the identifier of the job in the backend
+            status: how the task ended
+            metadata: metadata to add to the task_run entry
+            timestamp: the instant the event occurred
 
         Returns:
-            the updated task_run entry
+            a TaskRun object with updated fields
 
         """
         ...
 
     @remote_api_endpoint("task/filter_for_archive")
     def filter_task_to_archive(
         self,
@@ -320,15 +362,17 @@
         """Delete archived tasks as much as possible. Only the task_ids whose
         complete associated task_run have been cleaned up will be.
 
         """
         ...
 
     @remote_api_endpoint("task_run/get")
-    def get_task_runs(self, task_ids, limit=None):
+    def get_task_runs(
+        self, task_ids: List[int], limit: Optional[int] = None
+    ) -> List[TaskRun]:
         """Search task run for a task id"""
         ...
 
     @remote_api_endpoint("listers/get")
     def get_listers(self) -> List[Lister]:
         """Retrieve information about all listers from the database."""
         ...
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/journal_client.py` & `swh_scheduler-2.3.0/swh/scheduler/journal_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         if "type" in msg and msg["status"] not in ("created", "ongoing")
     ]
 
     if not interesting_messages:
         return
 
     origin_visit_stats: Dict[Tuple[str, str], Dict] = {
-        (visit_stats.url, visit_stats.visit_type): attr.asdict(visit_stats)
+        (visit_stats.url, visit_stats.visit_type): visit_stats.to_dict()
         for visit_stats in scheduler.origin_visit_stats_get(
             list(set((vs["origin"], vs["type"]) for vs in interesting_messages))
         )
     }
     existing_origin_visit_stats = copy.deepcopy(origin_visit_stats)
 
     # Use the default values from the model object
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/pytest_plugin.py` & `swh_scheduler-2.3.0/swh/scheduler/pytest_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022  The Software Heritage developers
+# Copyright (C) 2020-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from datetime import timedelta
 from functools import partial
 
@@ -11,14 +11,15 @@
 import pkg_resources
 import pytest
 from pytest_postgresql import factories
 
 from swh.core.db.db_utils import initialize_database_for_module
 from swh.scheduler import get_scheduler
 from swh.scheduler.backend import SchedulerBackend
+from swh.scheduler.model import TaskType
 
 # celery tasks for testing purpose; tasks themselves should be
 # in swh/scheduler/tests/tasks.py
 TASK_NAMES = ["ping", "multiping", "add", "error", "echo"]
 
 
 scheduler_postgresql_proc = factories.postgresql_proc(
@@ -48,22 +49,22 @@
 
 
 @pytest.fixture
 def swh_scheduler(swh_scheduler_class, swh_scheduler_config):
     scheduler = get_scheduler(swh_scheduler_class, **swh_scheduler_config)
     for taskname in TASK_NAMES:
         scheduler.create_task_type(
-            {
-                "type": "swh-test-{}".format(taskname),
-                "description": "The {} testing task".format(taskname),
-                "backend_name": "swh.scheduler.tests.tasks.{}".format(taskname),
-                "default_interval": timedelta(days=1),
-                "min_interval": timedelta(hours=6),
-                "max_interval": timedelta(days=12),
-            }
+            TaskType(
+                type=f"swh-test-{taskname}",
+                description=f"The {taskname} testing task",
+                backend_name=f"swh.scheduler.tests.tasks.{taskname}",
+                default_interval=timedelta(days=1),
+                min_interval=timedelta(hours=6),
+                max_interval=timedelta(days=12),
+            )
         )
 
     return scheduler
 
 
 # this alias is used to be able to easily instantiate a db-backed Scheduler
 # eg. for the RPC client/server test suite.
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/simulator/__init__.py` & `swh_scheduler-2.3.0/swh/scheduler/simulator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """This package runs the scheduler in a simulated environment, to evaluate
 various metrics. See :ref:`swh-scheduler-simulator`.
 
@@ -13,15 +13,15 @@
 from datetime import datetime, timedelta, timezone
 import logging
 from typing import Dict, Generator, Optional
 
 from simpy import Event
 
 from swh.scheduler.interface import SchedulerInterface
-from swh.scheduler.utils import create_origin_task_dicts
+from swh.scheduler.utils import create_origin_tasks, utcnow
 
 from . import origin_scheduler, task_scheduler
 from .common import Environment, Queue, SimulationReport, Task
 from .origins import generate_listed_origin, lister_process, load_task_process
 
 logger = logging.getLogger(__name__)
 
@@ -117,23 +117,20 @@
 
     # Generate 'num_origins' new origins
     origins = [generate_listed_origin(stored_lister.id) for _ in range(num_origins)]
     scheduler.record_listed_origins(origins)
 
     scheduler.create_tasks(
         [
-            {
-                **task_dict,
-                "policy": "recurring",
-                "next_run": origin.last_update,
-                "interval": timedelta(days=64),
-            }
-            for (origin, task_dict) in zip(
-                origins, create_origin_task_dicts(origins, scheduler)
+            task.evolve(
+                policy="recurring",
+                next_run=origin.last_update or utcnow(),
+                current_interval=timedelta(days=64),
             )
+            for (origin, task) in zip(origins, create_origin_tasks(origins, scheduler))
         ]
     )
 
 
 def run(
     scheduler: SchedulerInterface,
     scheduler_type: str,
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/simulator/common.py` & `swh_scheduler-2.3.0/swh/scheduler/simulator/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/simulator/origin_scheduler.py` & `swh_scheduler-2.3.0/swh/scheduler/simulator/origin_scheduler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Agents using the new origin-aware scheduler."""
 
 import logging
@@ -14,15 +14,18 @@
 
 from .common import Environment, Queue, Task, TaskEvent
 
 logger = logging.getLogger(__name__)
 
 
 def scheduler_runner_process(
-    env: Environment, task_queues: Dict[str, Queue], policy: str, min_batch_size: int
+    env: Environment,
+    task_queues: Dict[str, Queue],
+    policy: str,
+    min_batch_size: int,
 ) -> Iterator[Event]:
     """Scheduler runner. Grabs next visits from the database according to the
     scheduling policy, and fills the task_queues accordingly."""
 
     while True:
         for visit_type, queue in task_queues.items():
             remaining = queue.slots_remaining()
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/simulator/origins.py` & `swh_scheduler-2.3.0/swh/scheduler/simulator/origins.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/simulator/task_scheduler.py` & `swh_scheduler-2.3.0/swh/scheduler/simulator/task_scheduler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Agents using the "old" task-based scheduler."""
 
 import logging
 from typing import Dict, Generator, Iterator
 
 from simpy import Event
 
+from swh.scheduler.model import TaskRun, TaskRunStatus
+
 from .common import Environment, Queue, Task, TaskEvent
 
 logger = logging.getLogger(__name__)
 
 
 def scheduler_runner_process(
     env: Environment,
@@ -35,25 +37,25 @@
                 "%s runner: running %s %s tasks",
                 env.time,
                 visit_type,
                 len(next_tasks),
             )
 
             sim_tasks = [
-                Task(visit_type=visit_type, origin=task["arguments"]["kwargs"]["url"])
+                Task(visit_type=visit_type, origin=task.arguments.kwargs["url"])
                 for task in next_tasks
             ]
 
             env.scheduler.mass_schedule_task_runs(
                 [
-                    {
-                        "task": task["id"],
-                        "scheduled": env.time,
-                        "backend_id": str(sim_task.backend_id),
-                    }
+                    TaskRun(
+                        task=task.id,
+                        scheduled=env.time,
+                        backend_id=str(sim_task.backend_id),
+                    )
                     for task, sim_task in zip(next_tasks, sim_tasks)
                 ]
             )
 
             for sim_task in sim_tasks:
                 yield queue.put(sim_task)
 
@@ -65,17 +67,16 @@
 ) -> Generator[Event, TaskEvent, None]:
     """Scheduler listener. In the real world this would listen to celery
     events, but we listen to the status_queue and simulate celery events from
     that."""
     while True:
         event = yield status_queue.get()
         if event.status.status == "ongoing":
-            env.scheduler.start_task_run(event.task.backend_id, timestamp=env.time)
+            env.scheduler.start_task_run(str(event.task.backend_id), timestamp=env.time)
         else:
+            status: TaskRunStatus = "failed"
             if event.status.status == "full":
                 status = "eventful" if event.eventful else "uneventful"
-            else:
-                status = "failed"
 
             env.scheduler.end_task_run(
                 str(event.task.backend_id), status=status, timestamp=env.time
             )
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/30-schema.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/40-func.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/40-func.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/60-indexes.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/02.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/02.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/03.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/03.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/04.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/04.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/05.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/05.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/06.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/06.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/07.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/07.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/08.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/08.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/09.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/09.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/10.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/10.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/11.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/11.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/12.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/12.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/13.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/13.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/14.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/14.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/15.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/15.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/16.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/16.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/19.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/19.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/23.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/23.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/25.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/25.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/26.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/26.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/27.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/27.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/28.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/28.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/29.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/29.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/30.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/30.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/31.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/31.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/32.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/32.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/33.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/33.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/34.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/34.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/sql/upgrades/35.sql` & `swh_scheduler-2.3.0/swh/scheduler/sql/upgrades/35.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/task.py` & `swh_scheduler-2.3.0/swh/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/data/logging-config.yaml` & `swh_scheduler-2.3.0/swh/scheduler/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/tasks.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_api_client.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_celery_tasks.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_celery_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# Copyright (C) 2019-2021 The Software Heritage developers
+# Copyright (C) 2019-2024 The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Module in charge of testing the scheduler runner module"""
 
 import copy
 from itertools import count
 from time import sleep
+from typing import List, Tuple
 
 from celery.result import AsyncResult, GroupResult
 from kombu import Exchange, Queue
 import pytest
 
 from swh.scheduler.celery_backend import config
 from swh.scheduler.celery_backend.runner import run_ready_tasks
+from swh.scheduler.model import TaskPolicy, TaskPriority
 from swh.scheduler.tests.tasks import (
     TASK_ADD,
     TASK_ECHO,
     TASK_ERROR,
     TASK_MULTIPING,
     TASK_PING,
 )
-from swh.scheduler.utils import create_task_dict
+from swh.scheduler.utils import create_task
 
 # Queues to subscribe. Due to the rerouting of high priority tasks, this module requires
 # to declare all queues/task names
 TEST_QUEUES = [
     "celery",
     TASK_ECHO,
     TASK_ERROR,
@@ -94,147 +96,138 @@
 def test_scheduler_fixture(
     swh_scheduler_celery_app, swh_scheduler_celery_worker, swh_scheduler
 ):
     "Test that the scheduler fixture works properly"
     task_type = swh_scheduler.get_task_type("swh-test-ping")
 
     assert task_type
-    assert task_type["backend_name"] == TASK_PING
+    assert task_type.backend_name == TASK_PING
 
-    swh_scheduler.create_tasks([create_task_dict("swh-test-ping", "oneshot")])
+    swh_scheduler.create_tasks([create_task("swh-test-ping", "oneshot")])
 
     backend_tasks = run_ready_tasks(swh_scheduler, swh_scheduler_celery_app)
     assert backend_tasks
     for task in backend_tasks:
         # Make sure the task completed
-        AsyncResult(id=task["backend_id"]).get()
+        AsyncResult(id=task.backend_id).get()
 
 
 def test_run_ready_task_standard(
     swh_scheduler_celery_app, swh_scheduler_celery_worker, swh_scheduler
 ):
     """Ensure scheduler runner schedules tasks ready for scheduling"""
     task_type_name, backend_name = "swh-test-add", TASK_ADD
     task_type = swh_scheduler.get_task_type(task_type_name)
     assert task_type
-    assert task_type["backend_name"] == backend_name
+    assert task_type.backend_name == backend_name
 
-    task_inputs = [
+    task_inputs: List[Tuple[TaskPolicy, Tuple[int, int]]] = [
         ("oneshot", (12, 30)),
         ("oneshot", (20, 10)),
         ("recurring", (30, 10)),
     ]
 
     tasks = swh_scheduler.create_tasks(
-        create_task_dict(task_type_name, policy, *args)
-        for (policy, args) in task_inputs
+        create_task(task_type_name, policy, *args) for (policy, args) in task_inputs
     )
 
     assert len(tasks) == len(task_inputs)
 
     task_ids = set()
     for task in tasks:
-        assert task["status"] == "next_run_not_scheduled"
-        assert task["priority"] is None
-        task_ids.add(task["id"])
+        assert task.status == "next_run_not_scheduled"
+        assert task.priority is None
+        task_ids.add(task.id)
 
     backend_tasks = run_ready_tasks(swh_scheduler, swh_scheduler_celery_app)
     assert len(backend_tasks) == len(tasks)
 
     scheduled_tasks = swh_scheduler.search_tasks(task_type=task_type_name)
     assert len(scheduled_tasks) == len(tasks)
     for task in scheduled_tasks:
-        assert task["status"] == "next_run_scheduled"
-        assert task["id"] in task_ids
+        assert task.status == "next_run_scheduled"
+        assert task.id in task_ids
 
     # Ensure each task is indeed scheduled to the queue backend
     for i, (_, args) in enumerate(task_inputs):
         task = backend_tasks[i]
-        value = AsyncResult(id=task["backend_id"]).get()
+        value = AsyncResult(id=task.backend_id).get()
         assert value == sum(args)
 
 
 def test_run_ready_task_with_priority(
     swh_scheduler_celery_app, swh_scheduler_celery_worker, swh_scheduler
 ):
     """Ensure scheduler runner schedules priority tasks ready for scheduling"""
     task_type_name, backend_name = "swh-test-add", TASK_ADD
     task_type = swh_scheduler.get_task_type(task_type_name)
     assert task_type
-    assert task_type["backend_name"] == backend_name
+    assert task_type.backend_name == backend_name
 
-    task_inputs = [
+    task_inputs: List[Tuple[TaskPolicy, Tuple[int, int], TaskPriority]] = [
         ("oneshot", (10, 22), "low"),
         ("oneshot", (20, 10), "normal"),
         ("recurring", (30, 10), "high"),
     ]
 
     tasks = swh_scheduler.create_tasks(
-        create_task_dict(task_type_name, policy, *args, priority=priority)
+        create_task(task_type_name, policy, *args, priority=priority)
         for (policy, args, priority) in task_inputs
     )
 
     assert len(tasks) == len(task_inputs)
 
     task_ids = set()
     for task in tasks:
-        assert task["status"] == "next_run_not_scheduled"
-        assert task["priority"] is not None
-        task_ids.add(task["id"])
+        assert task.status == "next_run_not_scheduled"
+        assert task.priority is not None
+        task_ids.add(task.id)
 
     backend_tasks = run_ready_tasks(
         swh_scheduler, swh_scheduler_celery_app, task_types=[], with_priority=True
     )
     assert len(backend_tasks) == len(tasks)
 
     scheduled_tasks = swh_scheduler.search_tasks(task_type=task_type_name)
     assert len(scheduled_tasks) == len(tasks)
     for task in scheduled_tasks:
-        assert task["status"] == "next_run_scheduled"
-        assert task["id"] in task_ids
+        assert task.status == "next_run_scheduled"
+        assert task.id in task_ids
 
     # Ensure each priority task is indeed scheduled to the queue backend
     for i, (_, args, _) in enumerate(task_inputs):
         task = backend_tasks[i]
-        value = AsyncResult(id=task["backend_id"]).get()
+        value = AsyncResult(id=task.backend_id).get()
         assert value == sum(args)
 
 
 def test_task_exception(
     swh_scheduler_celery_app,
     swh_scheduler_celery_worker,
     swh_scheduler,
-    mocker,
+    sentry_events,
 ):
-    from sentry_sdk.integrations import celery
-
-    # using the sentry_events fixture does not work for celery tasks so
-    # we spy the capture_event method from the client of the sentry Hub
-    # used in celery integration instead
-    capture_event = mocker.spy(celery.Hub.current.client, "capture_event")
-
     task_type = swh_scheduler.get_task_type("swh-test-error")
     assert task_type
-    assert task_type["backend_name"] == TASK_ERROR
+    assert task_type.backend_name == TASK_ERROR
 
     swh_scheduler.create_tasks(
-        [create_task_dict("swh-test-error", "oneshot", "arg", kwarg="kwarg")]
+        [create_task("swh-test-error", "oneshot", "arg", kwarg="kwarg")]
     )
 
     backend_tasks = run_ready_tasks(swh_scheduler, swh_scheduler_celery_app)
     assert len(backend_tasks) == 1
 
     task = backend_tasks[0]
-    result = AsyncResult(id=task["backend_id"])
+    result = AsyncResult(id=task.backend_id)
     with pytest.raises(NotImplementedError):
         result.get()
 
     # check celery integration for sentry is enabled
-    assert capture_event.mock_calls
-    sentry_event_extra = capture_event.mock_calls[0].kwargs["event"]["extra"]
+    sentry_event_extra = sentry_events[0]["extra"]
     assert "celery-job" in sentry_event_extra
     assert sentry_event_extra["celery-job"] == {
         "task_name": TASK_ERROR,
         "args": ["arg"],
         "kwargs": {"kwarg": "kwarg"},
     }
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 from click.testing import CliRunner
 import pytest
 
 from swh.core.api.classes import stream_results
 from swh.model.model import Origin
 from swh.scheduler.cli import cli
-from swh.scheduler.utils import create_task_dict, utcnow
+from swh.scheduler.utils import create_task, utcnow
 
 CLI_CONFIG = """
 scheduler:
     cls: foo
     args: {}
 """
 
@@ -195,17 +195,26 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_pending_tasks(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task2["next_run"] += datetime.timedelta(days=1)
+    task1 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow(),
+        key="value1",
+    )
+    task2 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=1),
+        key="value2",
+    )
     swh_scheduler.create_tasks([task1, task2])
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -247,15 +256,15 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_pending_tasks_filter(swh_scheduler):
-    task = create_task_dict("swh-test-multiping", "oneshot", key="value")
+    task = create_task("swh-test-multiping", "oneshot", key="value")
     swh_scheduler.create_tasks([task])
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -271,16 +280,16 @@
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_pending_tasks_filter_2(swh_scheduler):
     swh_scheduler.create_tasks(
         [
-            create_task_dict("swh-test-multiping", "oneshot", key="value"),
-            create_task_dict("swh-test-ping", "oneshot", key="value2"),
+            create_task("swh-test-multiping", "oneshot", key="value"),
+            create_task("swh-test-ping", "oneshot", key="value2"),
         ]
     )
 
     result = invoke(
         swh_scheduler,
         False,
         [
@@ -308,18 +317,15 @@
 
 
 # Fails because "task list-pending --limit 3" only returns 2 tasks, because
 # of how compute_nb_tasks_from works.
 @pytest.mark.xfail
 def test_list_pending_tasks_limit(swh_scheduler):
     swh_scheduler.create_tasks(
-        [
-            create_task_dict("swh-test-ping", "oneshot", key="value%d" % i)
-            for i in range(10)
-        ]
+        [create_task("swh-test-ping", "oneshot", key="value%d" % i) for i in range(10)]
     )
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -362,18 +368,27 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_pending_tasks_before(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task1["next_run"] += datetime.timedelta(days=3)
-    task2["next_run"] += datetime.timedelta(days=1)
+    task1 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=3),
+        key="value",
+    )
+    task2 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=1),
+        key="value2",
+    )
+
     swh_scheduler.create_tasks([task1, task2])
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -398,17 +413,26 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task1["next_run"] += datetime.timedelta(days=3, hours=2)
+    task1 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=3, hours=2),
+        key="value1",
+    )
+    task2 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow(),
+        key="value2",
+    )
     swh_scheduler.create_tasks([task1, task2])
 
     swh_scheduler.grab_ready_tasks("swh-test-ping")
 
     result = invoke(
         swh_scheduler,
         False,
@@ -445,17 +469,17 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_id(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task3 = create_task_dict("swh-test-ping", "oneshot", key="value3")
+    task1 = create_task("swh-test-ping", "oneshot", key="value1")
+    task2 = create_task("swh-test-ping", "oneshot", key="value2")
+    task3 = create_task("swh-test-ping", "oneshot", key="value3")
     swh_scheduler.create_tasks([task1, task2, task3])
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -481,17 +505,17 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_id_2(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task3 = create_task_dict("swh-test-ping", "oneshot", key="value3")
+    task1 = create_task("swh-test-ping", "oneshot", key="value1")
+    task2 = create_task("swh-test-ping", "oneshot", key="value2")
+    task3 = create_task("swh-test-ping", "oneshot", key="value3")
     swh_scheduler.create_tasks([task1, task2, task3])
 
     result = invoke(
         swh_scheduler, False, ["task", "list", "--task-id", "2", "--task-id", "3"]
     )
 
     expected = r"""
@@ -521,17 +545,17 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_type(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-multiping", "oneshot", key="value2")
-    task3 = create_task_dict("swh-test-ping", "oneshot", key="value3")
+    task1 = create_task("swh-test-ping", "oneshot", key="value1")
+    task2 = create_task("swh-test-multiping", "oneshot", key="value2")
+    task3 = create_task("swh-test-ping", "oneshot", key="value3")
     swh_scheduler.create_tasks([task1, task2, task3])
 
     result = invoke(
         swh_scheduler, False, ["task", "list", "--task-type", "swh-test-ping"]
     )
 
     expected = r"""
@@ -561,17 +585,17 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_limit(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task3 = create_task_dict("swh-test-ping", "oneshot", key="value3")
+    task1 = create_task("swh-test-ping", "oneshot", key="value1")
+    task2 = create_task("swh-test-ping", "oneshot", key="value2")
+    task3 = create_task("swh-test-ping", "oneshot", key="value3")
     swh_scheduler.create_tasks([task1, task2, task3])
 
     result = invoke(
         swh_scheduler,
         False,
         [
             "task",
@@ -608,17 +632,26 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_before(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task1["next_run"] += datetime.timedelta(days=3, hours=2)
+    task1 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=3, hours=2),
+        key="value1",
+    )
+    task2 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow(),
+        key="value2",
+    )
     swh_scheduler.create_tasks([task1, task2])
 
     swh_scheduler.grab_ready_tasks("swh-test-ping")
 
     result = invoke(
         swh_scheduler,
         False,
@@ -646,17 +679,26 @@
 
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_list_tasks_after(swh_scheduler):
-    task1 = create_task_dict("swh-test-ping", "oneshot", key="value1")
-    task2 = create_task_dict("swh-test-ping", "oneshot", key="value2")
-    task1["next_run"] += datetime.timedelta(days=3, hours=2)
+    task1 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow() + datetime.timedelta(days=3, hours=2),
+        key="value1",
+    )
+    task2 = create_task(
+        "swh-test-ping",
+        "oneshot",
+        next_run=utcnow(),
+        key="value2",
+    )
     swh_scheduler.create_tasks([task1, task2])
 
     swh_scheduler.grab_ready_tasks("swh-test-ping")
 
     result = invoke(
         swh_scheduler,
         False,
@@ -726,21 +768,19 @@
 
 
 def _assert_origin_tasks_contraints(tasks, max_tasks, max_task_size, expected_origins):
     # check there are not too many tasks
     assert len(tasks) <= max_tasks
 
     # check tasks are not too large
-    assert all(len(task["arguments"]["args"][0]) <= max_task_size for task in tasks)
+    assert all(len(task.arguments.args[0]) <= max_task_size for task in tasks)
 
     # check the tasks are exhaustive
-    assert sum([len(task["arguments"]["args"][0]) for task in tasks]) == len(
-        expected_origins
-    )
-    assert set.union(*(set(task["arguments"]["args"][0]) for task in tasks)) == {
+    assert sum([len(task.arguments.args[0]) for task in tasks]) == len(expected_origins)
+    assert set.union(*(set(task.arguments.args[0]) for task in tasks)) == {
         origin.url for origin in expected_origins
     }
 
 
 @patch("swh.scheduler.cli.utils.TASK_BATCH_SIZE", 3)
 def test_task_schedule_origins(swh_scheduler, storage):
     """Tests the scheduling when neither origin_batch_size or
@@ -767,15 +807,15 @@
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), repr(result.output)
 
     # Check tasks
     tasks = swh_scheduler.search_tasks()
     _assert_origin_tasks_contraints(tasks, 4, 20, origins)
-    assert all(task["arguments"]["kwargs"] == {} for task in tasks)
+    assert all(task.arguments.kwargs == {} for task in tasks)
 
 
 def test_task_schedule_origins_kwargs(swh_scheduler, storage):
     """Tests support of extra keyword-arguments."""
     origins = _fill_storage_with_origins(storage, 30)
 
     result = invoke(
@@ -800,16 +840,15 @@
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), repr(result.output)
 
     # Check tasks
     tasks = swh_scheduler.search_tasks()
     _assert_origin_tasks_contraints(tasks, 2, 20, origins)
     assert all(
-        task["arguments"]["kwargs"] == {"key1": "value1", "key2": "value2"}
-        for task in tasks
+        task.arguments.kwargs == {"key1": "value1", "key2": "value2"} for task in tasks
     )
 
 
 def test_task_schedule_origins_with_limit(swh_scheduler, storage):
     """Tests support of extra keyword-arguments."""
     _fill_storage_with_origins(storage, 50)
     limit = 20
@@ -894,15 +933,15 @@
     _assert_origin_tasks_contraints(tasks, max_task_size, nb_origins, expected_origins)
 
 
 def test_cli_task_runner_unknown_task_types(swh_scheduler, storage):
     """When passing at least one unknown task type, the runner should fail."""
 
     task_types = swh_scheduler.get_task_types()
-    task_type_names = [t["type"] for t in task_types]
+    task_type_names = [t.type for t in task_types]
     known_task_type = random.choice(task_type_names)
     unknown_task_type = "unknown-task-type"
     assert unknown_task_type not in task_type_names
 
     result = invoke(
         swh_scheduler,
         True,
@@ -921,15 +960,15 @@
 @pytest.mark.parametrize("flag_priority", ["--with-priority", "--without-priority"])
 def test_cli_task_runner_with_known_tasks(
     swh_scheduler, storage, caplog, flag_priority
 ):
     """Trigger runner with known tasks runs smoothly."""
 
     task_types = swh_scheduler.get_task_types()
-    task_type_names = [t["type"] for t in task_types]
+    task_type_names = [t.type for t in task_types]
     task_type_name = random.choice(task_type_names)
     task_type_name2 = random.choice(task_type_names)
 
     # The runner will just iterate over the following known tasks and do noop. We are
     # just checking the runner does not explode here.
     result = invoke(
         swh_scheduler,
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_add_forge_now.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_add_forge_now.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-# Copyright (C) 2022  The Software Heritage developers
+# Copyright (C) 2022-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from typing import Dict, Tuple
+from datetime import timedelta
+from typing import Tuple
 
 import attr
 import pytest
 
 from swh.scheduler.cli.utils import lister_task_type
 from swh.scheduler.interface import SchedulerInterface
+from swh.scheduler.model import TaskType
 from swh.scheduler.tests.common import TASK_TYPES
 from swh.scheduler.tests.test_cli import invoke as basic_invoke
 
 
 def invoke(scheduler, args: Tuple[str, ...] = (), catch_exceptions: bool = False):
     return basic_invoke(
         scheduler, args=["add-forge-now", *args], catch_exceptions=catch_exceptions
@@ -85,15 +87,15 @@
     assert result.exit_code == 0
 
     scheduled_tasks = {
         (call[0][0], call[1]["kwargs"]["url"]) for call in send_task.call_args_list
     }
 
     expected_tasks = {
-        (TASK_TYPES[origin.visit_type]["backend_name"], origin.url)
+        (TASK_TYPES[origin.visit_type].backend_name, origin.url)
         for origin in listed_origins_by_type[visit_type]
     }
 
     assert scheduled_tasks == expected_tasks
 
     # Ensure the scheduling happens on the right queue
     queue_name = send_task.call_args[1]["queue"]
@@ -107,30 +109,30 @@
 
     assert queue_name_prefix == expected_queue_name_prefix
     assert queue_name_suffix == "swh.loader.git.tasks.UpdateGitRepository"
 
 
 def _create_task_type(
     swh_scheduler: SchedulerInterface, lister_name: str, listing_type: str = "full"
-) -> Dict:
-    task_type = {
-        "type": lister_task_type(lister_name, listing_type),  # only relevant bit
-        "description": f"{listing_type} listing",
-        "backend_name": "swh.example.backend",
-        "default_interval": "1 day",
-        "min_interval": "1 day",
-        "max_interval": "1 day",
-        "backoff_factor": "1",
-        "max_queue_length": "100",
-        "num_retries": 3,
-    }
-    swh_scheduler.create_task_type(task_type)
-    task_type = swh_scheduler.get_task_type(task_type["type"])
-    assert task_type is not None
-    return task_type
+) -> TaskType:
+    task_type_in = TaskType(
+        type=lister_task_type(lister_name, listing_type),  # only relevant bit
+        description=f"{listing_type} listing",
+        backend_name="swh.example.backend",
+        default_interval=timedelta(days=1),
+        min_interval=timedelta(days=1),
+        max_interval=timedelta(days=1),
+        backoff_factor=1.0,
+        max_queue_length=100,
+        num_retries=3,
+    )
+    swh_scheduler.create_task_type(task_type_in)
+    task_type_out = swh_scheduler.get_task_type(task_type_in.type)
+    assert task_type_out is not None
+    return task_type_out
 
 
 @pytest.mark.parametrize("preset", ["staging", "production"])
 def test_schedule_register_lister(swh_scheduler, stored_lister, preset):
     # given
     assert stored_lister is not None
     lister_name = stored_lister.name
@@ -151,21 +153,21 @@
     )
 
     output = result.output.lstrip()
 
     expected_msgs = []
     if preset == "production":
         # 2 tasks: 1 full + 1 incremental (tomorrow) with recurring policy
-        expected_msgs = ["Policy: recurring", incremental["type"], "Next run: tomorrow"]
+        expected_msgs = ["Policy: recurring", incremental.type, "Next run: tomorrow"]
     else:
         # 1 task full with policy oneshot
         expected_msgs = ["Policy: oneshot"]
 
     # In any case, there is the full listing type too
-    expected_msgs.append(full["type"])
+    expected_msgs.append(full.type)
 
     assert len(expected_msgs) > 0
     for msg in expected_msgs:
         assert msg in output
 
 
 def test_register_lister_unknown_task_type(swh_scheduler):
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_celery_monitor.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_config.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_journal.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_journal.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_origin.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,17 +110,15 @@
     result = invoke(swh_scheduler, args=("schedule-next", visit_type, str(NUM_RESULTS)))
     assert result.exit_code == 0
 
     # pull all tasks out of the scheduler
     tasks = swh_scheduler.search_tasks()
     assert len(tasks) == NUM_RESULTS
 
-    scheduled_tasks = {
-        (task["type"], task["arguments"]["kwargs"]["url"]) for task in tasks
-    }
+    scheduled_tasks = {(task.type, task.arguments.kwargs["url"]) for task in tasks}
     all_possible_tasks = {
         (f"load-{origin.visit_type}", origin.url)
         for origin in listed_origins_by_type[visit_type]
     }
 
     assert scheduled_tasks <= all_possible_tasks
 
@@ -182,15 +180,15 @@
     assert result.exit_code == 0
 
     scheduled_tasks = {
         (call[0][0], call[1]["kwargs"]["url"]) for call in send_task.call_args_list
     }
 
     expected_tasks = {
-        (TASK_TYPES[origin.visit_type]["backend_name"], origin.url)
+        (TASK_TYPES[origin.visit_type].backend_name, origin.url)
         for origin in listed_origins_by_type[visit_type]
     }
 
     assert expected_tasks == scheduled_tasks
 
 
 def test_update_metrics(swh_scheduler, listed_origins):
@@ -262,15 +260,15 @@
         assert "Destination queue" in result.output
 
     actual_scheduled_tasks = {
         (call[1]["name"], call[1]["kwargs"]["url"], call[1]["queue"])
         for call in send_task.call_args_list
     }
 
-    backend_name = task_types[task_type_param]["backend_name"]
+    backend_name = task_types[task_type_param].backend_name
     queue = f"{queue_name_prefix}:{backend_name}" if queue_name_prefix else backend_name
     expected_tasks = (
         {}
         if dry_run
         else {
             (backend_name, origin.url, queue)
             for origin in origins_to_schedule[
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_origin_utils.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_origin_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Copyright (C) 2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
 
-from swh.scheduler.cli.origin_utils import get_scheduler_task_info
+from swh.scheduler.cli.origin_utils import get_scheduler_task_type
 
 
-def test_get_scheduler_task_info_found(swh_scheduler, task_types):
+def test_get_scheduler_task_type_found(swh_scheduler, task_types):
     """It should find standard task types"""
     # Check we found the standard task type
     for task_type, task_type_info in task_types.items():
-        actual_task_info = get_scheduler_task_info(swh_scheduler, task_type)
+        actual_task_info = get_scheduler_task_type(swh_scheduler, task_type)
         assert actual_task_info == task_type_info
 
 
 @pytest.mark.parametrize(
     "task_type_suffix", ["bitbucket", "extra-mercurial", "overly-long-task-suffix"]
 )
-def test_get_scheduler_task_info_found_derivative(
+def test_get_scheduler_task_type_found_derivative(
     swh_scheduler, task_types, task_type_suffix
 ):
     """It should find derivative task types"""
     # Create another task type derivative out of a standard task type
     first_task_type = next(iter(task_types))
     another_task_type = f"{first_task_type}-{task_type_suffix}"
 
-    actual_task_info_2 = get_scheduler_task_info(swh_scheduler, another_task_type)
+    actual_task_info_2 = get_scheduler_task_type(swh_scheduler, another_task_type)
     # we found it and it matches the origin task type it derives from
     assert actual_task_info_2 == task_types[first_task_type]
 
 
-def test_get_scheduler_task_info_found_raise(swh_scheduler, task_types):
+def test_get_scheduler_task_type_found_raise(swh_scheduler, task_types):
     """It should raise when no task_type is found"""
     unknown_task_type = "foobar-task-type"
     assert unknown_task_type not in task_types
 
     with pytest.raises(ValueError, match="not find scheduler"):
-        get_scheduler_task_info(swh_scheduler, unknown_task_type)
+        get_scheduler_task_type(swh_scheduler, unknown_task_type)
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_task_type.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_task_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -98,20 +98,20 @@
     ]:
         result = cli_runner.invoke(cli, command)
 
         assert result.exit_code == 0, traceback.print_exception(*result.exc_info)
 
         scheduler = get_scheduler(**local_sched_config["scheduler"])
 
-        all_tasks = ["list-foo-full", "load-bar"]
-        for task in all_tasks:
-            task_type_desc = scheduler.get_task_type(task)
-            assert task_type_desc
-            assert task_type_desc["type"] == task
-            assert task_type_desc["backoff_factor"] == 1
+        all_task_type_names = ["list-foo-full", "load-bar"]
+        for task_type_name in all_task_type_names:
+            task_type = scheduler.get_task_type(task_type_name)
+            assert task_type
+            assert task_type.type == task_type_name
+            assert task_type.backoff_factor == 1.0
 
 
 def test_register_task_types_filter(
     cli_runner,
     local_sched_config,
     local_sched_configfile,
 ):
@@ -127,22 +127,20 @@
             "lister.foo",
         ],
     )
 
     assert result.exit_code == 0, traceback.print_exception(*result.exc_info)
 
     scheduler = get_scheduler(**local_sched_config["scheduler"])
-    all_tasks = [
-        "list-foo-full",
-    ]
-    for task in all_tasks:
-        task_type_desc = scheduler.get_task_type(task)
-        assert task_type_desc
-        assert task_type_desc["type"] == task
-        assert task_type_desc["backoff_factor"] == 1
+
+    task_type_name = "list-foo-full"
+    task_type = scheduler.get_task_type(task_type_name)
+    assert task_type
+    assert task_type.type == task_type_name
+    assert task_type.backoff_factor == 1.0
 
 
 @pytest.mark.parametrize("cli_command", ["list", "register", "add"])
 def test_cli_task_type_raise(cli_runner, cli_command):
     """Without a proper configuration, the cli raises"""
     result = cli_runner.invoke(cli, ["task-type", cli_command])
     assert "Scheduler class" in result.output
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_cli_utils.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_common.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_common.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,43 @@
-# Copyright (C) 2017-2019  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
+from typing import Dict, Optional
+
+from swh.scheduler.model import TaskPriority
+from swh.scheduler.utils import utcnow
 
 from .common import TEMPLATES, tasks_from_template
 
 
 def test_tasks_from_template_no_priority():
     nb_tasks = 3
     template = TEMPLATES["test-git"]
-    next_run = datetime.datetime.utcnow()
+    next_run = utcnow()
     tasks = tasks_from_template(template, next_run, nb_tasks)
 
     assert len(tasks) == nb_tasks
 
     for i, t in enumerate(tasks):
-        assert t["type"] == template["type"]
-        assert t["arguments"] is not None
-        assert t.get("policy") is None  # not defined in template
-        assert len(t["arguments"]["args"]) == 1
-        assert len(t["arguments"]["kwargs"].keys()) == 1
-        assert t["next_run"] == next_run - datetime.timedelta(microseconds=i)
-        assert t.get("priority") is None
+        assert t.type == template.type
+        assert t.arguments is not None
+        # not defined in template but is recurring by default
+        assert t.policy == "recurring"
+        assert len(t.arguments.args) == 1
+        assert len(t.arguments.kwargs.keys()) == 1
+        assert t.next_run == next_run - datetime.timedelta(microseconds=i)
+        assert t.priority is None
 
 
 def test_tasks_from_template_priority():
     template = TEMPLATES["test-hg"]
-    num_priorities = {
+    num_priorities: Dict[Optional[TaskPriority], int] = {
         None: 3,
         "high": 5,
         "normal": 3,
         "low": 2,
     }
 
     next_run = datetime.datetime.utcnow()
@@ -42,18 +47,18 @@
         num_priorities=num_priorities,
     )
 
     assert len(tasks) == sum(num_priorities.values())
 
     repartition_priority = {k: 0 for k in num_priorities}
     for i, t in enumerate(tasks):
-        assert t["type"] == template["type"]
-        assert t["arguments"] is not None
-        assert t["policy"] == template["policy"]
-        assert len(t["arguments"]["args"]) == 1
-        assert len(t["arguments"]["kwargs"].keys()) == 1
-        assert t["next_run"] == next_run - datetime.timedelta(microseconds=i)
-        priority = t.get("priority")
+        assert t.type == template.type
+        assert t.arguments is not None
+        assert t.policy == template.policy
+        assert len(t.arguments.args) == 1
+        assert len(t.arguments.kwargs.keys()) == 1
+        assert t.next_run == next_run - datetime.timedelta(microseconds=i)
+        priority = t.priority
         assert priority in num_priorities
         repartition_priority[priority] += 1
 
     assert repartition_priority == num_priorities
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_config.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 
 
 def test_get_available_slots_issue_when_reading_queue(mocker):
     mock = mocker.patch("swh.scheduler.celery_backend.config.get_queue_length")
     mock.side_effect = ValueError
 
     actual_num = get_available_slots(app, "anything", max_length=10)
-    assert actual_num == MAX_NUM_TASKS
+    assert actual_num == 10
     assert mock.called
 
 
 def test_get_available_slots_no_queue_length(mocker):
     mock = mocker.patch("swh.scheduler.celery_backend.config.get_queue_length")
     mock.return_value = None
     actual_num = get_available_slots(app, "anything", max_length=100)
-    assert actual_num == MAX_NUM_TASKS
+    assert actual_num == 100
     assert mock.called
 
 
 def test_get_available_slots_no_more_slots(mocker):
     mock = mocker.patch("swh.scheduler.celery_backend.config.get_queue_length")
     max_length = 100
     queue_length = 9000
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_init.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_journal_client.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_model.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_recurrent_visits.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_recurrent_visits.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021  The Software Heritage developers
+# Copyright (C) 2021-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from datetime import timedelta
 import logging
 from queue import Queue
@@ -16,14 +16,15 @@
     VisitSchedulerThreads,
     grab_next_visits_policy_weights,
     send_visits_for_visit_type,
     spawn_visit_scheduler_thread,
     terminate_visit_scheduler_threads,
     visit_scheduler_thread,
 )
+from swh.scheduler.model import TaskType
 
 from .test_cli import invoke
 
 TEST_MAX_QUEUE = 10000
 MODULE_NAME = "swh.scheduler.celery_backend.recurrent_visits"
 
 
@@ -34,33 +35,30 @@
 
 @pytest.fixture
 def swh_scheduler(swh_scheduler):
     """Override default fixture of the scheduler to install some more task types."""
     for visit_type in ["test-git", "test-hg", "test-svn"]:
         task_type = f"load-{visit_type}"
         swh_scheduler.create_task_type(
-            {
-                "type": task_type,
-                "max_queue_length": TEST_MAX_QUEUE,
-                "description": "The {} testing task".format(task_type),
-                "backend_name": _compute_backend_name(visit_type),
-                "default_interval": timedelta(days=1),
-                "min_interval": timedelta(hours=6),
-                "max_interval": timedelta(days=12),
-            }
+            TaskType(
+                type=task_type,
+                max_queue_length=TEST_MAX_QUEUE,
+                description=f"The {task_type} testing task",
+                backend_name=_compute_backend_name(visit_type),
+                default_interval=timedelta(days=1),
+                min_interval=timedelta(hours=6),
+                max_interval=timedelta(days=12),
+            )
         )
     return swh_scheduler
 
 
 @pytest.fixture
 def all_task_types(swh_scheduler):
-    return {
-        task_type_d["type"]: task_type_d
-        for task_type_d in swh_scheduler.get_task_types()
-    }
+    return {task_type.type: task_type for task_type in swh_scheduler.get_task_types()}
 
 
 def test_cli_schedule_recurrent_unknown_visit_type(swh_scheduler):
     """When passed an unknown visit type, the recurrent visit scheduler should refuse
     to start."""
 
     result = invoke(
@@ -164,20 +162,17 @@
 
     task_types = []
     origins = []
     for visit_type, _origins in listed_origins_by_type.items():
         origins.extend(swh_scheduler.record_listed_origins(_origins))
         task_type_name = f"load-{visit_type}"
         assert task_type_name in all_task_types.keys()
-        task_type = all_task_types[task_type_name]
-        task_type["visit_type"] = visit_type
-        # we'll limit the orchestrator to the origins' type we know
-        task_types.append(task_type)
+        task_types.append((visit_type, all_task_types[task_type_name]))
 
-    for visit_type in ["test-git", "test-svn"]:
+    for visit_type in visit_types:
         task_type = f"load-{visit_type}"
         send_visits_for_visit_type(
             swh_scheduler,
             mock_celery_app,
             visit_type,
             all_task_types[task_type],
             DEFAULT_DVCS_POLICY,
@@ -186,17 +181,16 @@
     assert mock_available_slots.called, "The available slots functions should be called"
 
     records = [record.message for record in caplog.records]
 
     # Mapping over the dict ratio/policies entries can change overall order so let's
     # check the set of records
     expected_records = set()
-    for task_type in task_types:
-        visit_type = task_type["visit_type"]
-        queue_name = task_type["backend_name"]
+    for visit_type, task_type in task_types:
+        queue_name = task_type.backend_name
         msg = (
             f"{nb_origins} available slots for visit type {visit_type} "
             f"in queue {queue_name}"
         )
         expected_records.add(msg)
 
     for expected_record in expected_records:
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_scheduler.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,59 +1,63 @@
-# Copyright (C) 2017-2023  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
 import copy
 from datetime import datetime, timedelta, timezone
 import inspect
+from operator import attrgetter
 import random
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 import uuid
 
 import attr
 from psycopg2.extras import execute_values
 import pytest
 
 from swh.model.hashutil import hash_to_bytes
 from swh.scheduler.exc import SchedulerException, StaleData, UnknownPolicy
 from swh.scheduler.interface import ListedOriginPageToken, SchedulerInterface
 from swh.scheduler.model import (
     LastVisitStatus,
     ListedOrigin,
     OriginVisitStats,
-    SchedulerMetrics,
+    TaskPriority,
+    TaskRun,
 )
-from swh.scheduler.utils import create_oneshot_task_dict, utcnow
+from swh.scheduler.utils import create_oneshot_task, utcnow
 
 from .common import (
     LISTERS,
     TASK_TYPES,
     TEMPLATES,
     tasks_from_template,
     tasks_with_priority_from_template,
 )
 
 ONEDAY = timedelta(days=1)
 
-NUM_PRIORITY_TASKS = {None: 100, "high": 60, "normal": 30, "low": 20}
+NUM_PRIORITY_TASKS: Dict[Optional[TaskPriority], int] = {
+    None: 100,
+    "high": 60,
+    "normal": 30,
+    "low": 20,
+}
 
 
 def subdict(d, keys=None, excl=()):
     if keys is None:
         keys = [k for k in d.keys()]
     return {k: d[k] for k in keys if k not in excl}
 
 
-def metrics_sort_key(m: SchedulerMetrics) -> Tuple[uuid.UUID, str]:
-    return (m.lister_id, m.visit_type)
-
-
 def assert_metrics_equal(left, right):
+    metrics_sort_key = attrgetter("lister_id", "visit_type")
     assert sorted(left, key=metrics_sort_key) == sorted(right, key=metrics_sort_key)
 
 
 class TestScheduler:
     def test_interface(self, swh_scheduler):
         """Checks all methods of SchedulerInterface are implemented by this
         backend, and that they have the same signature."""
@@ -83,25 +87,25 @@
             assert expected_signature == actual_signature, meth_name
 
         assert missing_methods == []
 
     def test_add_task_type(self, swh_scheduler):
         tt = TASK_TYPES["test-git"]
         swh_scheduler.create_task_type(tt)
-        assert tt == swh_scheduler.get_task_type(tt["type"])
+        assert tt == swh_scheduler.get_task_type(tt.type)
         tt2 = TASK_TYPES["test-hg"]
         swh_scheduler.create_task_type(tt2)
-        assert tt == swh_scheduler.get_task_type(tt["type"])
-        assert tt2 == swh_scheduler.get_task_type(tt2["type"])
+        assert tt == swh_scheduler.get_task_type(tt.type)
+        assert tt2 == swh_scheduler.get_task_type(tt2.type)
 
     def test_create_task_type_idempotence(self, swh_scheduler):
         tt = TASK_TYPES["test-git"]
         swh_scheduler.create_task_type(tt)
         swh_scheduler.create_task_type(tt)
-        assert tt == swh_scheduler.get_task_type(tt["type"])
+        assert tt == swh_scheduler.get_task_type(tt.type)
 
     def test_get_task_types(self, swh_scheduler):
         tt, tt2 = TASK_TYPES["test-git"], TASK_TYPES["test-hg"]
         swh_scheduler.create_task_type(tt)
         swh_scheduler.create_task_type(tt2)
         actual_task_types = swh_scheduler.get_task_types()
         assert tt in actual_task_types
@@ -114,218 +118,203 @@
         tasks_2 = tasks_from_template(
             TEMPLATES["test-hg"], utcnow(), num_priorities=NUM_PRIORITY_TASKS
         )
         tasks = tasks_1 + tasks_2
 
         # tasks are returned only once with their ids
         ret1 = swh_scheduler.create_tasks(tasks + tasks)
-        set_ret1 = set([t["id"] for t in ret1])
+        set_ret1 = set([t.id for t in ret1])
 
         # creating the same set result in the same ids
         ret = swh_scheduler.create_tasks(tasks)
-        set_ret = set([t["id"] for t in ret])
+        set_ret = set([t.id for t in ret])
 
         # Idempotence results
         assert set_ret == set_ret1
         assert len(ret) == len(ret1)
 
         ids = set()
-        actual_priorities = defaultdict(int)
+        actual_priorities: Dict[Optional[TaskPriority], int] = defaultdict(int)
 
         for task, orig_task in zip(ret, tasks):
             task = copy.deepcopy(task)
-            task_type = TASK_TYPES[orig_task["type"].split("-", 1)[-1]]
-            assert task["id"] not in ids
-            assert task["status"] == "next_run_not_scheduled"
-            assert task["current_interval"] == task_type["default_interval"]
-            assert task["policy"] == orig_task.get("policy", "recurring")
-            priority = task.get("priority")
-            actual_priorities[priority] += 1
-
-            assert task["retries_left"] == (task_type["num_retries"] or 0)
-            ids.add(task["id"])
-            del task["id"]
-            del task["status"]
-            del task["current_interval"]
-            del task["retries_left"]
-            if "policy" not in orig_task:
-                del task["policy"]
-            if "priority" not in orig_task:
-                del task["priority"]
-                assert task == orig_task
+            task_type = TASK_TYPES[orig_task.type.split("-", 1)[-1]]
+            assert task.id not in ids
+            assert task.status == "next_run_not_scheduled"
+            assert task.current_interval == task_type.default_interval
+            assert task.policy == orig_task.policy
+            actual_priorities[task.priority] += 1
+            assert task.retries_left == (task_type.num_retries or 0)
+            ids.add(task.id)
 
         expected_priorities = NUM_PRIORITY_TASKS.copy()
         expected_priorities[None] += num_git
         assert dict(actual_priorities) == expected_priorities
 
     def test_create_tasks_with_custom_next_run(self, swh_scheduler):
         self._create_task_types(swh_scheduler)
         first_next_run = utcnow()
         second_next_run = utcnow() + timedelta(hours=6)
-        task_type = TEMPLATES["test-git"]["type"]
+        task_type = TEMPLATES["test-git"].type
 
         tasks = swh_scheduler.create_tasks(
-            [create_oneshot_task_dict(task_type, next_run=first_next_run)]
+            [create_oneshot_task(task_type, next_run=first_next_run)]
         )
         assert tasks
-        assert tasks[0]["next_run"] == first_next_run
+        assert tasks[0].next_run == first_next_run
 
         tasks += swh_scheduler.create_tasks(
-            [create_oneshot_task_dict(task_type, next_run=second_next_run)]
+            [create_oneshot_task(task_type, next_run=second_next_run)]
         )
         assert len(tasks) > 1
-        assert tasks[1]["next_run"] == second_next_run
+        assert tasks[1].next_run == second_next_run
 
         ready_tasks = swh_scheduler.peek_ready_tasks(task_type, timestamp=utcnow())
         assert ready_tasks
-        assert ready_tasks[0]["id"] == tasks[0]["id"]
+        assert ready_tasks[0].id == tasks[0].id
 
         ready_tasks = swh_scheduler.peek_ready_tasks(
             task_type, timestamp=utcnow() + timedelta(hours=6)
         )
         assert len(ready_tasks) > 1
-        assert ready_tasks[1]["id"] == tasks[1]["id"]
+        assert ready_tasks[1].id == tasks[1].id
 
         grabbed_tasks = swh_scheduler.grab_ready_tasks(
             task_type, timestamp=utcnow() + timedelta(hours=6)
         )
         assert len(grabbed_tasks) == len(ready_tasks)
 
         backend_tasks = [
-            {
-                "task": task["id"],
-                "backend_id": str(uuid.uuid4()),
-                "scheduled": utcnow() + timedelta(hours=i * 6),
-            }
+            TaskRun(
+                task=task.id,
+                backend_id=str(uuid.uuid4()),
+                scheduled=utcnow() + timedelta(hours=i * 6),
+            )
             for i, task in enumerate(grabbed_tasks)
         ]
 
         swh_scheduler.mass_schedule_task_runs(backend_tasks)
 
-        task_runs = swh_scheduler.get_task_runs(task_ids=[task["id"] for task in tasks])
+        task_runs = swh_scheduler.get_task_runs(task_ids=[task.id for task in tasks])
         assert len(task_runs) == len(tasks)
         for i, task in enumerate(backend_tasks):
             status = "eventful"
             start = utcnow() + timedelta(hours=i * 6)
             end = start + timedelta(minutes=5)
             task_run = swh_scheduler.start_task_run(
-                task["backend_id"],
+                task.backend_id,
                 timestamp=start,
             )
             task_run = swh_scheduler.end_task_run(
-                task["backend_id"],
+                task.backend_id,
                 status=status,
                 timestamp=end,
             )
-            assert task_run["status"] == status
-            assert task_run["started"] == start
-            assert task_run["ended"] == end
+            assert task_run.status == status
+            assert task_run.started == start
+            assert task_run.ended == end
 
     def test_peek_ready_tasks_no_priority(self, swh_scheduler):
         self._create_task_types(swh_scheduler)
         t = utcnow()
-        task_type = TEMPLATES["test-git"]["type"]
+        task_type = TEMPLATES["test-git"].type
         tasks = tasks_from_template(TEMPLATES["test-git"], t, 100)
         random.shuffle(tasks)
         swh_scheduler.create_tasks(tasks)
 
         ready_tasks = swh_scheduler.peek_ready_tasks(task_type)
         assert len(ready_tasks) == len(tasks)
         for i in range(len(ready_tasks) - 1):
-            assert ready_tasks[i]["next_run"] <= ready_tasks[i + 1]["next_run"]
+            assert ready_tasks[i].next_run <= ready_tasks[i + 1].next_run
 
         # Only get the first few ready tasks
         limit = random.randrange(5, 5 + len(tasks) // 2)
         ready_tasks_limited = swh_scheduler.peek_ready_tasks(task_type, num_tasks=limit)
 
         assert len(ready_tasks_limited) == limit
         assert ready_tasks_limited == ready_tasks[:limit]
 
         # Limit by timestamp
-        max_ts = tasks[limit - 1]["next_run"]
+        max_ts = tasks[limit - 1].next_run
         ready_tasks_timestamped = swh_scheduler.peek_ready_tasks(
             task_type, timestamp=max_ts
         )
 
         for ready_task in ready_tasks_timestamped:
-            assert ready_task["next_run"] <= max_ts
+            assert ready_task.next_run <= max_ts
 
         # Make sure we get proper behavior for the first ready tasks
         assert ready_tasks[: len(ready_tasks_timestamped)] == ready_tasks_timestamped
 
         # Limit by both
         ready_tasks_both = swh_scheduler.peek_ready_tasks(
             task_type, timestamp=max_ts, num_tasks=limit // 3
         )
         assert len(ready_tasks_both) <= limit // 3
         for ready_task in ready_tasks_both:
-            assert ready_task["next_run"] <= max_ts
+            assert ready_task.next_run <= max_ts
             assert ready_task in ready_tasks[: limit // 3]
 
     def test_peek_ready_tasks_returns_only_no_priority_tasks(self, swh_scheduler):
         """Peek ready tasks only return standard tasks (no priority)"""
         self._create_task_types(swh_scheduler)
         t = utcnow()
-        task_type = TEMPLATES["test-git"]["type"]
+        task_type = TEMPLATES["test-git"].type
         # Create tasks with and without priorities
         tasks = tasks_from_template(
             TEMPLATES["test-git"],
             t,
             num_priorities=NUM_PRIORITY_TASKS,
         )
 
         count_priority = 0
         for task in tasks:
-            count_priority += 0 if task.get("priority") is None else 1
+            count_priority += 0 if task.priority is None else 1
 
         assert count_priority > 0, "Some created tasks should have some priority"
 
         random.shuffle(tasks)
         swh_scheduler.create_tasks(tasks)
 
         # take all available no priority tasks
         ready_tasks = swh_scheduler.peek_ready_tasks(task_type)
 
         assert len(ready_tasks) == len(tasks) - count_priority
 
         # No read task should have any priority
         for task in ready_tasks:
-            assert task.get("priority") is None
+            assert task.priority is None
 
     def test_grab_ready_tasks(self, swh_scheduler):
         self._create_task_types(swh_scheduler)
         t = utcnow()
-        task_type = TEMPLATES["test-git"]["type"]
+        task_type = TEMPLATES["test-git"].type
         # Create tasks with and without priorities
         tasks = tasks_from_template(
             TEMPLATES["test-git"], t, num_priorities=NUM_PRIORITY_TASKS
         )
         random.shuffle(tasks)
         swh_scheduler.create_tasks(tasks)
 
         first_ready_tasks = swh_scheduler.peek_ready_tasks(task_type, num_tasks=50)
         grabbed_tasks = swh_scheduler.grab_ready_tasks(task_type, num_tasks=50)
-        first_ready_tasks.sort(key=lambda task: task["arguments"]["args"][0])
-        grabbed_tasks.sort(key=lambda task: task["arguments"]["args"][0])
+        first_ready_tasks.sort(key=lambda task: task.arguments.args[0])
+        grabbed_tasks.sort(key=lambda task: task.arguments.args[0])
 
         for peeked, grabbed in zip(first_ready_tasks, grabbed_tasks):
-            assert peeked["status"] == "next_run_not_scheduled"
-            del peeked["status"]
-            assert grabbed["status"] == "next_run_scheduled"
-            del grabbed["status"]
-            assert peeked == grabbed
-            priority = grabbed["priority"]
-            assert priority == peeked["priority"]
-            assert priority is None
+            assert peeked.status == "next_run_not_scheduled"
+            assert grabbed.status == "next_run_scheduled"
+            assert peeked.priority is None
+            assert peeked == grabbed.evolve(status=peeked.status)
 
     def test_grab_ready_priority_tasks(self, swh_scheduler):
         """check the grab and peek priority tasks endpoint behave as expected"""
         self._create_task_types(swh_scheduler)
         t = utcnow()
-        task_type = TEMPLATES["test-git"]["type"]
+        task_type = TEMPLATES["test-git"].type
         num_tasks = 100
         # Create tasks with and without priorities
         tasks0 = tasks_with_priority_from_template(
             TEMPLATES["test-git"],
             t,
             num_tasks,
             "high",
@@ -345,52 +334,43 @@
         tasks = tasks0 + tasks1 + tasks2
 
         random.shuffle(tasks)
         swh_scheduler.create_tasks(tasks)
 
         ready_tasks = swh_scheduler.peek_ready_priority_tasks(task_type, num_tasks=50)
         grabbed_tasks = swh_scheduler.grab_ready_priority_tasks(task_type, num_tasks=50)
-        ready_tasks.sort(key=lambda task: task["arguments"]["args"][0])
-        grabbed_tasks.sort(key=lambda task: task["arguments"]["args"][0])
+        ready_tasks.sort(key=lambda task: task.arguments.args[0])
+        grabbed_tasks.sort(key=lambda task: task.arguments.args[0])
 
         for peeked, grabbed in zip(ready_tasks, grabbed_tasks):
-            assert peeked["status"] == "next_run_not_scheduled"
-            del peeked["status"]
-            assert grabbed["status"] == "next_run_scheduled"
-            del grabbed["status"]
-            assert peeked == grabbed
-            assert peeked["priority"] == grabbed["priority"]
-            assert peeked["priority"] is not None
+            assert peeked.status == "next_run_not_scheduled"
+            assert grabbed.status == "next_run_scheduled"
+            assert peeked.priority is not None
+            assert peeked == grabbed.evolve(status=peeked.status)
 
     def test_get_tasks(self, swh_scheduler):
         self._create_task_types(swh_scheduler)
-        t = utcnow()
-        tasks = tasks_from_template(TEMPLATES["test-git"], t, 100)
+        tasks = tasks_from_template(TEMPLATES["test-git"], utcnow(), 100)
         tasks = swh_scheduler.create_tasks(tasks)
         random.shuffle(tasks)
         while len(tasks) > 1:
             length = random.randrange(1, len(tasks))
-            cur_tasks = sorted(tasks[:length], key=lambda x: x["id"])
+            cur_tasks = sorted(tasks[:length], key=attrgetter("id"))
             tasks[:length] = []
 
-            ret = swh_scheduler.get_tasks(task["id"] for task in cur_tasks)
+            ret = swh_scheduler.get_tasks(task.id for task in cur_tasks)
             # result is not guaranteed to be sorted
-            ret.sort(key=lambda x: x["id"])
+            ret.sort(key=attrgetter("id"))
             assert ret == cur_tasks
 
     def test_search_tasks(self, swh_scheduler):
-        def make_real_dicts(lst):
-            """RealDictRow is not a real dict."""
-            return [dict(d.items()) for d in lst]
-
         self._create_task_types(swh_scheduler)
-        t = utcnow()
-        tasks = tasks_from_template(TEMPLATES["test-git"], t, 100)
+        tasks = tasks_from_template(TEMPLATES["test-git"], utcnow(), 100)
         tasks = swh_scheduler.create_tasks(tasks)
-        assert make_real_dicts(swh_scheduler.search_tasks()) == make_real_dicts(tasks)
+        assert swh_scheduler.search_tasks() == tasks
 
     def assert_filtered_task_ok(
         self, task: Dict[str, Any], after: datetime, before: datetime
     ) -> None:
         """Ensure filtered tasks have the right expected properties
         (within the range, recurring disabled, etc..)
 
@@ -410,27 +390,27 @@
         recurring = tasks_from_template(TEMPLATES["test-git"], _time, 12)
         oneshots = tasks_from_template(TEMPLATES["test-hg"], _time, 12)
         total_tasks = len(recurring) + len(oneshots)
 
         # simulate scheduling tasks
         pending_tasks = swh_scheduler.create_tasks(recurring + oneshots)
         backend_tasks = [
-            {
-                "task": task["id"],
-                "backend_id": str(uuid.uuid4()),
-                "scheduled": utcnow(),
-            }
+            TaskRun(
+                task=task.id,
+                backend_id=str(uuid.uuid4()),
+                scheduled=utcnow(),
+            )
             for task in pending_tasks
         ]
         swh_scheduler.mass_schedule_task_runs(backend_tasks)
 
         # we simulate the task are being done
         _tasks = []
-        for task in backend_tasks:
-            t = swh_scheduler.end_task_run(task["backend_id"], status="eventful")
+        for task_run in backend_tasks:
+            t = swh_scheduler.end_task_run(task_run.backend_id, status="eventful")
             _tasks.append(t)
 
         # Randomly update task's status per policy
         status_per_policy = {"recurring": 0, "oneshot": 0}
         status_choice = {
             # policy: [tuple (1-for-filtering, 'associated-status')]
             "recurring": [
@@ -445,22 +425,22 @@
             ],
         }
 
         tasks_to_update = defaultdict(list)
         _task_ids = defaultdict(list)
         # randomize 'disabling' recurring task or 'complete' oneshot task
         for task in pending_tasks:
-            policy = task["policy"]
-            _task_ids[policy].append(task["id"])
+            policy = task.policy
+            _task_ids[policy].append(task.id)
             status = random.choice(status_choice[policy])
             if status[0] != 1:
                 continue
             # elected for filtering
             status_per_policy[policy] += status[0]
-            tasks_to_update[policy].append(task["id"])
+            tasks_to_update[policy].append(task.id)
 
         swh_scheduler.disable_tasks(tasks_to_update["recurring"])
         # hack: change the status to something else than completed/disabled
         swh_scheduler.set_status_tasks(
             _task_ids["oneshot"], status="next_run_not_scheduled"
         )
         # complete the tasks to update
@@ -530,173 +510,165 @@
         self._create_task_types(swh_scheduler)
         _time = utcnow()
         recurring = tasks_from_template(TEMPLATES["test-git"], _time, 12)
         oneshots = tasks_from_template(TEMPLATES["test-hg"], _time, 12)
         total_tasks = len(recurring) + len(oneshots)
         pending_tasks = swh_scheduler.create_tasks(recurring + oneshots)
         backend_tasks = [
-            {
-                "task": task["id"],
-                "backend_id": str(uuid.uuid4()),
-                "scheduled": utcnow(),
-            }
+            TaskRun(
+                task=task.id,
+                backend_id=str(uuid.uuid4()),
+                scheduled=utcnow(),
+            )
             for task in pending_tasks
         ]
         swh_scheduler.mass_schedule_task_runs(backend_tasks)
 
         _tasks = []
         percent = random.randint(0, 100)  # random election removal boundary
         for task in backend_tasks:
-            t = swh_scheduler.end_task_run(task["backend_id"], status="eventful")
+            t = swh_scheduler.end_task_run(task.backend_id, status="eventful")
             c = random.randint(0, 100)
             if c <= percent:
-                _tasks.append({"task_id": t["task"], "task_run_id": t["id"]})
+                _tasks.append({"task_id": t.task, "task_run_id": t.id})
 
         swh_scheduler.delete_archived_tasks(_tasks)
 
-        all_tasks = [task["id"] for task in swh_scheduler.search_tasks()]
+        all_tasks = [task.id for task in swh_scheduler.search_tasks()]
         tasks_count = len(all_tasks)
         tasks_run_count = len(swh_scheduler.get_task_runs(all_tasks))
 
         assert tasks_count == total_tasks - len(_tasks)
         assert tasks_run_count == total_tasks - len(_tasks)
 
     def test_get_task_runs_no_task(self, swh_scheduler):
         """No task exist in the scheduler's db, get_task_runs() should always return an
         empty list.
 
         """
-        assert not swh_scheduler.get_task_runs(task_ids=())
-        assert not swh_scheduler.get_task_runs(task_ids=(1, 2, 3))
-        assert not swh_scheduler.get_task_runs(task_ids=(1, 2, 3), limit=10)
+        assert not swh_scheduler.get_task_runs(task_ids=[])
+        assert not swh_scheduler.get_task_runs(task_ids=[1, 2, 3])
+        assert not swh_scheduler.get_task_runs(task_ids=[1, 2, 3], limit=10)
 
     def test_get_task_runs_no_task_executed(self, swh_scheduler):
         """No task has been executed yet, get_task_runs() should always return an empty
         list.
 
         """
         self._create_task_types(swh_scheduler)
         _time = utcnow()
         recurring = tasks_from_template(TEMPLATES["test-git"], _time, 12)
         oneshots = tasks_from_template(TEMPLATES["test-hg"], _time, 12)
         swh_scheduler.create_tasks(recurring + oneshots)
 
-        assert not swh_scheduler.get_task_runs(task_ids=())
-        assert not swh_scheduler.get_task_runs(task_ids=(1, 2, 3))
-        assert not swh_scheduler.get_task_runs(task_ids=(1, 2, 3), limit=10)
+        assert not swh_scheduler.get_task_runs(task_ids=[])
+        assert not swh_scheduler.get_task_runs(task_ids=[1, 2, 3])
+        assert not swh_scheduler.get_task_runs(task_ids=[1, 2, 3], limit=10)
 
     def test_get_task_runs_with_scheduled(self, swh_scheduler):
         """Some tasks have been scheduled but not executed yet, get_task_runs() should
         not return an empty list. limit should behave as expected.
 
         """
         self._create_task_types(swh_scheduler)
         _time = utcnow()
         recurring = tasks_from_template(TEMPLATES["test-git"], _time, 12)
         oneshots = tasks_from_template(TEMPLATES["test-hg"], _time, 12)
         total_tasks = len(recurring) + len(oneshots)
         pending_tasks = swh_scheduler.create_tasks(recurring + oneshots)
         backend_tasks = [
-            {
-                "task": task["id"],
-                "backend_id": str(uuid.uuid4()),
-                "scheduled": utcnow(),
-            }
+            TaskRun(
+                task=task.id,
+                backend_id=str(uuid.uuid4()),
+                scheduled=utcnow(),
+            )
             for task in pending_tasks
         ]
         swh_scheduler.mass_schedule_task_runs(backend_tasks)
 
         assert not swh_scheduler.get_task_runs(task_ids=[total_tasks + 1])
 
         btask = backend_tasks[0]
-        runs = swh_scheduler.get_task_runs(task_ids=[btask["task"]])
+        runs = swh_scheduler.get_task_runs(task_ids=[btask.task])
         assert len(runs) == 1
         run = runs[0]
 
-        assert subdict(run, excl=("id",)) == {
-            "task": btask["task"],
-            "backend_id": btask["backend_id"],
-            "scheduled": btask["scheduled"],
-            "started": None,
-            "ended": None,
-            "metadata": None,
-            "status": "scheduled",
-        }
+        assert run.evolve(id=None) == TaskRun(
+            task=btask.task,
+            backend_id=btask.backend_id,
+            scheduled=btask.scheduled,
+        )
 
         runs = swh_scheduler.get_task_runs(
-            task_ids=[bt["task"] for bt in backend_tasks], limit=2
+            task_ids=[bt.task for bt in backend_tasks], limit=2
         )
         assert len(runs) == 2
 
-        runs = swh_scheduler.get_task_runs(
-            task_ids=[bt["task"] for bt in backend_tasks]
-        )
+        runs = swh_scheduler.get_task_runs(task_ids=[bt.task for bt in backend_tasks])
         assert len(runs) == total_tasks
 
-        keys = ("task", "backend_id", "scheduled")
         assert (
-            sorted([subdict(x, keys) for x in runs], key=lambda x: x["task"])
+            sorted([x.evolve(id=None) for x in runs], key=attrgetter("task"))
             == backend_tasks
         )
 
     def test_get_task_runs_with_executed(self, swh_scheduler):
         """Some tasks have been executed, get_task_runs() should
         not return an empty list. limit should behave as expected.
 
         """
         self._create_task_types(swh_scheduler)
         _time = utcnow()
         recurring = tasks_from_template(TEMPLATES["test-git"], _time, 12)
         oneshots = tasks_from_template(TEMPLATES["test-hg"], _time, 12)
         pending_tasks = swh_scheduler.create_tasks(recurring + oneshots)
         backend_tasks = [
-            {
-                "task": task["id"],
-                "backend_id": str(uuid.uuid4()),
-                "scheduled": utcnow(),
-            }
+            TaskRun(
+                task=task.id,
+                backend_id=str(uuid.uuid4()),
+                scheduled=utcnow(),
+            )
             for task in pending_tasks
         ]
         swh_scheduler.mass_schedule_task_runs(backend_tasks)
 
         btask = backend_tasks[0]
         ts = utcnow()
         swh_scheduler.start_task_run(
-            btask["backend_id"], metadata={"something": "stupid"}, timestamp=ts
+            btask.backend_id, metadata={"something": "stupid"}, timestamp=ts
         )
-        runs = swh_scheduler.get_task_runs(task_ids=[btask["task"]])
+        runs = swh_scheduler.get_task_runs(task_ids=[btask.task])
         assert len(runs) == 1
-        assert subdict(runs[0], excl=("id")) == {
-            "task": btask["task"],
-            "backend_id": btask["backend_id"],
-            "scheduled": btask["scheduled"],
-            "started": ts,
-            "ended": None,
-            "metadata": {"something": "stupid"},
-            "status": "started",
-        }
+        assert runs[0].evolve(id=None) == TaskRun(
+            task=btask.task,
+            backend_id=btask.backend_id,
+            scheduled=btask.scheduled,
+            started=ts,
+            metadata={"something": "stupid"},
+            status="started",
+        )
 
         ts2 = utcnow()
         swh_scheduler.end_task_run(
-            btask["backend_id"],
+            btask.backend_id,
             metadata={"other": "stuff"},
             timestamp=ts2,
             status="eventful",
         )
-        runs = swh_scheduler.get_task_runs(task_ids=[btask["task"]])
+        runs = swh_scheduler.get_task_runs(task_ids=[btask.task])
         assert len(runs) == 1
-        assert subdict(runs[0], excl=("id")) == {
-            "task": btask["task"],
-            "backend_id": btask["backend_id"],
-            "scheduled": btask["scheduled"],
-            "started": ts,
-            "ended": ts2,
-            "metadata": {"something": "stupid", "other": "stuff"},
-            "status": "eventful",
-        }
+        assert runs[0].evolve(id=None) == TaskRun(
+            task=btask.task,
+            backend_id=btask.backend_id,
+            scheduled=btask.scheduled,
+            started=ts,
+            ended=ts2,
+            metadata={"something": "stupid", "other": "stuff"},
+            status="eventful",
+        )
 
     def test_get_or_create_lister(self, swh_scheduler):
         db_listers = []
         for lister_args in LISTERS:
             db_listers.append(swh_scheduler.get_or_create_lister(**lister_args))
 
         for lister, lister_args in zip(db_listers, LISTERS):
@@ -820,15 +792,15 @@
             assert ret.results[0].url == origin.url
 
     @pytest.mark.parametrize("num_origins,limit", [(20, 6), (5, 42), (20, 20)])
     def test_get_listed_origins_limit(
         self, swh_scheduler, listed_origins, num_origins, limit
     ) -> None:
         added_origins = sorted(
-            listed_origins[:num_origins], key=lambda o: (o.lister_id, o.url)
+            listed_origins[:num_origins], key=attrgetter("lister_id", "url")
         )
         swh_scheduler.record_listed_origins(added_origins)
 
         returned_origins: List[ListedOrigin] = []
         call_count = 0
         next_page_token: Optional[ListedOriginPageToken] = None
         while True:
@@ -1057,15 +1029,15 @@
                 **ovs_args,
             )
             for i, origin in enumerate(origins)
         ]
         swh_scheduler.origin_visit_stats_upsert(visit_stats)
 
         cooldown_td = timedelta(days=cooldown)
-        cooldown_args = {
+        cooldown_args: Dict[str, Optional[timedelta]] = {
             "scheduled_cooldown": None,
             "failed_cooldown": None,
             "not_found_cooldown": None,
             "absolute_cooldown": None,
         }
         cooldown_args[f"{which_cooldown}_cooldown"] = cooldown_td
 
@@ -1124,15 +1096,15 @@
             attr.evolve(origin, last_update=base_date - timedelta(seconds=i))
             for i, origin in enumerate(origins)
         ]
         updated_origins = swh_scheduler.record_listed_origins(updated_origins)
 
         # We expect to retrieve origins with the oldest update date, that is
         # origins at the end of our updated_origins list.
-        expected_origins = sorted(updated_origins, key=lambda o: o.last_update)
+        expected_origins = sorted(updated_origins, key=attrgetter("last_update"))
 
         self._check_grab_next_visit(
             swh_scheduler,
             visit_type=visit_type,
             policy="never_visited_oldest_update_first",
             expected=expected_origins,
         )
@@ -1352,15 +1324,15 @@
             lister_id=lister2.id,
             last_update=origin1.last_update + timedelta(seconds=10),
         )
 
         origins = [origin1, origin2]
         recorded_origins = swh_scheduler.record_listed_origins(origins)
 
-        expected_origins = sorted(recorded_origins, key=lambda o: o.last_update)
+        expected_origins = sorted(recorded_origins, key=attrgetter("last_update"))
 
         self._check_grab_next_visit(
             swh_scheduler,
             visit_type=origin1.visit_type,
             policy="never_visited_oldest_update_first",
             expected=expected_origins,
         )
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_server.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_simulator.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_temporary.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_temporary.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh/scheduler/tests/test_utils.py` & `swh_scheduler-2.3.0/swh/scheduler/tests/test_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,208 +1,210 @@
-# Copyright (C) 2017-2022  The Software Heritage developers
+# Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from datetime import datetime, timedelta, timezone
 import uuid
 
 import pytest
 
-from swh.scheduler import model, utils
+from swh.scheduler.model import ListedOrigin, Lister, Task, TaskArguments
+from swh.scheduler.utils import (
+    create_oneshot_task,
+    create_origin_task,
+    create_origin_tasks,
+    create_task,
+    utcnow,
+)
 
 from .common import LISTERS
 
 
 @pytest.fixture
 def mock_datetime(mocker):
     now = datetime.now(tz=timezone.utc)
     mock_datetime = mocker.patch("swh.scheduler.utils.datetime")
     mock_datetime.now.return_value = now
     return mock_datetime
 
 
-def test_create_oneshot_task_dict_simple(mock_datetime):
-    actual_task = utils.create_oneshot_task_dict("some-task-type")
+def test_create_oneshot_task_simple(mock_datetime):
+    actual_task = create_oneshot_task("some-task-type")
 
-    expected_task = {
-        "policy": "oneshot",
-        "type": "some-task-type",
-        "next_run": mock_datetime.now.return_value,
-        "arguments": {
-            "args": [],
-            "kwargs": {},
-        },
-    }
-
-    assert actual_task == expected_task
+    assert actual_task == Task(
+        policy="oneshot",
+        type="some-task-type",
+        next_run=mock_datetime.now.return_value,
+        arguments=TaskArguments(
+            args=[],
+            kwargs={},
+        ),
+    )
     mock_datetime.now.assert_called_once_with(tz=timezone.utc)
 
 
-def test_create_oneshot_task_dict_with_next_run():
-    next_run = datetime.now(tz=timezone.utc) + timedelta(hours=1)
-    actual_task = utils.create_oneshot_task_dict("some-task-type", next_run=next_run)
-
-    expected_task = {
-        "policy": "oneshot",
-        "type": "some-task-type",
-        "next_run": next_run,
-        "arguments": {
-            "args": [],
-            "kwargs": {},
-        },
-    }
-
-    assert actual_task == expected_task
+def test_create_oneshot_task_with_next_run():
+    next_run = utcnow() + timedelta(hours=1)
+    actual_task = create_oneshot_task("some-task-type", next_run=next_run)
+
+    assert actual_task == Task(
+        policy="oneshot",
+        type="some-task-type",
+        next_run=next_run,
+        arguments=TaskArguments(
+            args=[],
+            kwargs={},
+        ),
+    )
 
 
-def test_create_oneshot_task_dict_other_call(mock_datetime):
-    actual_task = utils.create_oneshot_task_dict(
+def test_create_oneshot_task_other_call(mock_datetime):
+    actual_task = create_oneshot_task(
         "some-task-type", "arg0", "arg1", priority="high", other_stuff="normal"
     )
 
-    expected_task = {
-        "policy": "oneshot",
-        "type": "some-task-type",
-        "next_run": mock_datetime.now.return_value,
-        "arguments": {
-            "args": ("arg0", "arg1"),
-            "kwargs": {"other_stuff": "normal"},
-        },
-        "priority": "high",
-    }
-
-    assert actual_task == expected_task
+    assert actual_task == Task(
+        policy="oneshot",
+        type="some-task-type",
+        next_run=mock_datetime.now.return_value,
+        arguments=TaskArguments(
+            args=["arg0", "arg1"],
+            kwargs={"other_stuff": "normal"},
+        ),
+        priority="high",
+    )
     mock_datetime.now.assert_called_once_with(tz=timezone.utc)
 
 
-def test_create_task_dict(mock_datetime):
-    actual_task = utils.create_task_dict(
+def test_create_task(mock_datetime):
+    actual_task = create_task(
         "task-type",
         "recurring",
         "arg0",
         "arg1",
         priority="low",
         other_stuff="normal",
         retries_left=3,
     )
 
-    expected_task = {
-        "policy": "recurring",
-        "type": "task-type",
-        "next_run": mock_datetime.now.return_value,
-        "arguments": {
-            "args": ("arg0", "arg1"),
-            "kwargs": {"other_stuff": "normal"},
-        },
-        "priority": "low",
-        "retries_left": 3,
-    }
-
-    assert actual_task == expected_task
+    assert actual_task == Task(
+        policy="recurring",
+        type="task-type",
+        next_run=mock_datetime.now.return_value,
+        arguments=TaskArguments(
+            args=["arg0", "arg1"],
+            kwargs={"other_stuff": "normal"},
+        ),
+        priority="low",
+        retries_left=3,
+    )
     mock_datetime.now.assert_called_once_with(tz=timezone.utc)
 
 
-def test_create_origin_task_dict():
-    lister = model.Lister(**LISTERS[1], id=uuid.uuid4())
-    origin = model.ListedOrigin(
+def test_create_origin_task(mock_datetime):
+    lister = Lister(**LISTERS[1], id=uuid.uuid4())
+    origin = ListedOrigin(
         lister_id=lister.id,
         url="http://example.com/",
         visit_type="git",
     )
 
-    task = utils.create_origin_task_dict(origin, lister)
-    assert task == {
-        "type": "load-git",
-        "arguments": {
-            "args": [],
-            "kwargs": {
+    assert create_origin_task(origin, lister) == Task(
+        type="load-git",
+        next_run=mock_datetime.now.return_value,
+        arguments=TaskArguments(
+            args=[],
+            kwargs={
                 "url": "http://example.com/",
                 "lister_name": LISTERS[1]["name"],
                 "lister_instance_name": LISTERS[1]["instance_name"],
             },
-        },
-    }
+        ),
+    )
 
     loader_args = {"foo": "bar", "baz": {"foo": "bar"}}
 
-    origin_w_args = model.ListedOrigin(
+    origin_w_args = ListedOrigin(
         lister_id=lister.id,
         url="http://example.com/svn/",
         visit_type="svn",
         extra_loader_arguments=loader_args,
     )
 
-    task_w_args = utils.create_origin_task_dict(origin_w_args, lister)
-    assert task_w_args == {
-        "type": "load-svn",
-        "arguments": {
-            "args": [],
-            "kwargs": {
+    assert create_origin_task(origin_w_args, lister) == Task(
+        type="load-svn",
+        next_run=mock_datetime.now.return_value,
+        arguments=TaskArguments(
+            args=[],
+            kwargs={
                 "url": "http://example.com/svn/",
                 "lister_name": LISTERS[1]["name"],
                 "lister_instance_name": LISTERS[1]["instance_name"],
                 **loader_args,
             },
-        },
-    }
+        ),
+    )
 
 
-def test_create_origin_task_dicts(swh_scheduler):
+def test_create_origin_tasks(swh_scheduler, mock_datetime):
     listers = []
     for lister_args in LISTERS:
         listers.append(swh_scheduler.get_or_create_lister(**lister_args))
 
-    origin1 = model.ListedOrigin(
+    origin1 = ListedOrigin(
         lister_id=listers[0].id,
         url="http://example.com/1",
         visit_type="git",
     )
-    origin2 = model.ListedOrigin(
+    origin2 = ListedOrigin(
         lister_id=listers[0].id,
         url="http://example.com/2",
         visit_type="git",
     )
-    origin3 = model.ListedOrigin(
+    origin3 = ListedOrigin(
         lister_id=listers[1].id,
         url="http://example.com/3",
         visit_type="git",
     )
 
     origins = [origin1, origin2, origin3]
 
-    tasks = utils.create_origin_task_dicts(origins, swh_scheduler)
+    tasks = create_origin_tasks(origins, swh_scheduler)
     assert tasks == [
-        {
-            "type": "load-git",
-            "arguments": {
-                "args": [],
-                "kwargs": {
+        Task(
+            type="load-git",
+            next_run=mock_datetime.now.return_value,
+            arguments=TaskArguments(
+                args=[],
+                kwargs={
                     "url": "http://example.com/1",
                     "lister_name": LISTERS[0]["name"],
                     "lister_instance_name": LISTERS[0]["instance_name"],
                 },
-            },
-        },
-        {
-            "type": "load-git",
-            "arguments": {
-                "args": [],
-                "kwargs": {
+            ),
+        ),
+        Task(
+            type="load-git",
+            next_run=mock_datetime.now.return_value,
+            arguments=TaskArguments(
+                args=[],
+                kwargs={
                     "url": "http://example.com/2",
                     "lister_name": LISTERS[0]["name"],
                     "lister_instance_name": LISTERS[0]["instance_name"],
                 },
-            },
-        },
-        {
-            "type": "load-git",
-            "arguments": {
-                "args": [],
-                "kwargs": {
+            ),
+        ),
+        Task(
+            type="load-git",
+            next_run=mock_datetime.now.return_value,
+            arguments=TaskArguments(
+                args=[],
+                kwargs={
                     "url": "http://example.com/3",
                     "lister_name": LISTERS[1]["name"],
                     "lister_instance_name": LISTERS[1]["instance_name"],
                 },
-            },
-        },
+            ),
+        ),
     ]
```

### Comparing `swh.scheduler-2.2.2/swh/scheduler/utils.py` & `swh_scheduler-2.3.0/swh/scheduler/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 # Copyright (C) 2017-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 from datetime import datetime, timezone
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
 from swh.scheduler.interface import SchedulerInterface
-from swh.scheduler.model import ListedOrigin, Lister
+from swh.scheduler.model import (
+    ListedOrigin,
+    Lister,
+    Task,
+    TaskArguments,
+    TaskPolicy,
+    TaskPriority,
+)
 
 
 def utcnow():
     return datetime.now(tz=timezone.utc)
 
 
 def get_task(task_name):
@@ -30,17 +37,23 @@
     from swh.scheduler.celery_backend.config import app
 
     for module in app.conf.CELERY_IMPORTS:
         __import__(module)
     return app.tasks[task_name]
 
 
-def create_task_dict(
-    type: str, policy: str, *args, next_run: Optional[datetime] = None, **kwargs
-) -> Dict[str, Any]:
+def create_task(
+    type: str,
+    policy: TaskPolicy,
+    *args,
+    next_run: Optional[datetime] = None,
+    priority: Optional[TaskPriority] = None,
+    retries_left: Optional[int] = None,
+    **kwargs,
+) -> Task:
     """Create a task with type and policy, scheduled for as soon as
        possible.
 
     Args:
         type: Type of oneshot task as per swh-scheduler's db
                     table task_type's column (Ex: load-git,
                     check-deposit)
@@ -49,79 +62,75 @@
             use current time otherwise
 
     Returns:
         Expected dictionary for the one-shot task scheduling api
         (swh.scheduler.backend.create_tasks)
 
     """
-    task_extra = {}
-    for extra_key in ["priority", "retries_left"]:
-        if extra_key in kwargs:
-            extra_val = kwargs.pop(extra_key)
-            task_extra[extra_key] = extra_val
-
-    task = {
-        "policy": policy,
-        "type": type,
-        "next_run": next_run or utcnow(),
-        "arguments": {
-            "args": args if args else [],
-            "kwargs": kwargs if kwargs else {},
-        },
-    }
-    task.update(task_extra)
+    task = Task(
+        policy=policy,
+        type=type,
+        next_run=next_run or utcnow(),
+        arguments=TaskArguments(
+            args=list(args) if args else [],
+            kwargs=kwargs if kwargs else {},
+        ),
+        priority=priority,
+        retries_left=retries_left,
+    )
     return task
 
 
-def create_origin_task_dict(origin: ListedOrigin, lister: Lister) -> Dict[str, Any]:
+def create_origin_task(origin: ListedOrigin, lister: Lister) -> Task:
     if origin.lister_id != lister.id:
         raise ValueError(
             "origin.lister_id and lister.id differ", origin.lister_id, lister.id
         )
-    return {
-        "type": f"load-{origin.visit_type}",
-        "arguments": {
-            "args": [],
-            "kwargs": {
+    return Task(
+        type=f"load-{origin.visit_type}",
+        arguments=TaskArguments(
+            args=[],
+            kwargs={
                 "url": origin.url,
                 "lister_name": lister.name,
                 "lister_instance_name": lister.instance_name or None,
                 **origin.extra_loader_arguments,
             },
-        },
-    }
+        ),
+        next_run=utcnow(),
+    )
 
 
-def create_origin_task_dicts(
+def create_origin_tasks(
     origins: List[ListedOrigin], scheduler: SchedulerInterface
-) -> List[Dict[str, Any]]:
+) -> List[Task]:
     """Returns a task dict for each origin, in the same order."""
 
     lister_ids = {o.lister_id for o in origins}
     listers = {
         lister.id: lister
         for lister in scheduler.get_listers_by_id(list(map(str, lister_ids)))
     }
 
     missing_lister_ids = lister_ids - set(listers)
     assert not missing_lister_ids, f"Missing listers: {missing_lister_ids}"
 
-    return [create_origin_task_dict(o, listers[o.lister_id]) for o in origins]
+    return [create_origin_task(o, listers[o.lister_id]) for o in origins]
 
 
-def create_oneshot_task_dict(
+def create_oneshot_task(
     type: str, *args, next_run: Optional[datetime] = None, **kwargs
-):
+) -> Task:
     """Create a oneshot task scheduled for as soon as possible.
 
     Args:
         type: Type of oneshot task as per swh-scheduler's db
             table task_type's column (Ex: load-git, check-deposit)
         next_run: optional date and time from which the task can be executed,
             use current time otherwise
 
     Returns:
         Expected dictionary for the one-shot task scheduling api
         (:func:`swh.scheduler.backend.create_tasks`)
 
     """
-    return create_task_dict(type, "oneshot", *args, next_run=next_run, **kwargs)
+    return create_task(type, "oneshot", *args, next_run=next_run, **kwargs)
```

### Comparing `swh.scheduler-2.2.2/swh.scheduler.egg-info/PKG-INFO` & `swh_scheduler-2.3.0/swh.scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 2.2.2
+Version: 2.3.0
 Summary: Software Heritage scheduler
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-scheduler/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-scheduler.git
@@ -31,15 +31,15 @@
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: sentry-sdk
 Requires-Dist: setuptools
 Requires-Dist: testing.postgresql
 Requires-Dist: typing-extensions
-Requires-Dist: swh.core[db,http]>=3.0.0
+Requires-Dist: swh.core[db,http]>=3.0.1
 Requires-Dist: swh.storage>=2.0.0
 Provides-Extra: journal
 Requires-Dist: swh.journal; extra == "journal"
 Provides-Extra: simulator
 Requires-Dist: plotille; extra == "simulator"
 Requires-Dist: simpy<4,>=3; extra == "simulator"
 Provides-Extra: testing
```

### Comparing `swh.scheduler-2.2.2/swh.scheduler.egg-info/SOURCES.txt` & `swh_scheduler-2.3.0/swh.scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.scheduler-2.2.2/swh.scheduler.egg-info/requires.txt` & `swh_scheduler-2.3.0/swh.scheduler.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pyyaml
 requests
 tabulate
 sentry-sdk
 setuptools
 testing.postgresql
 typing-extensions
-swh.core[db,http]>=3.0.0
+swh.core[db,http]>=3.0.1
 swh.storage>=2.0.0
 
 [:python_version <= "3.7"]
 importlib_metadata<5
 
 [journal]
 swh.journal
```

