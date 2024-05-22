# Comparing `tmp/jf_ingest-0.0.84.tar.gz` & `tmp/jf-ingest-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jf_ingest-0.0.84.tar", last modified: Wed May 22 15:13:47 2024, max compression
+gzip compressed data, was "jf-ingest-0.0.9.tar", last modified: Mon Oct 16 19:49:45 2023, max compression
```

## Comparing `jf_ingest-0.0.84.tar` & `jf-ingest-0.0.9.tar`

### file list

```diff
@@ -1,92 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/
--rw-r--r--   0 root         (0) root         (0)     2844 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/.gitignore
--rw-r--r--   0 root         (0) root         (0)      293 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)     1066 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1329 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      732 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/README.md
--rw-r--r--   0 root         (0) root         (0)     2427 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/example.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/jf_ingest/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15159 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/config.py
--rw-r--r--   0 root         (0) root         (0)      634 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/constants.py
--rw-r--r--   0 root         (0) root         (0)     9724 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/diagnostics.py
--rw-r--r--   0 root         (0) root         (0)    11573 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/file_operations.py
--rw-r--r--   0 root         (0) root         (0)     8340 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/graphql_utils.py
--rw-r--r--   0 root         (0) root         (0)     5686 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/harness.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/jf_ingest/jf_git/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/jf_ingest/jf_git/adapters/
--rw-r--r--   0 root         (0) root         (0)    20069 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/adapters/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19785 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/adapters/github.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/jf_ingest/jf_git/clients/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/clients/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37160 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/clients/github.py
--rw-r--r--   0 root         (0) root         (0)      350 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_git/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/jf_ingest/jf_jira/
--rw-r--r--   0 root         (0) root         (0)    27185 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_jira/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8077 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_jira/auth.py
--rw-r--r--   0 root         (0) root         (0)    89092 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_jira/downloaders.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/jf_jira/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6217 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/logging_helper.py
--rw-r--r--   0 root         (0) root         (0)     1333 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/name_redactor.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/regression_detector.py
--rw-r--r--   0 root         (0) root         (0)    18088 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/utils.py
--rw-r--r--   0 root         (0) root         (0)    30948 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/jf_ingest/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/jf_ingest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1329 2024-05-22 15:13:47.000000 jf_ingest-0.0.84/jf_ingest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2893 2024-05-22 15:13:47.000000 jf_ingest-0.0.84/jf_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 15:13:47.000000 jf_ingest-0.0.84/jf_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2024-05-22 15:13:47.000000 jf_ingest-0.0.84/jf_ingest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 15:13:47.000000 jf_ingest-0.0.84/jf_ingest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)    90551 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/pdm.lock
--rw-r--r--   0 root         (0) root         (0)     2300 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.760246 jf_ingest-0.0.84/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.764246 jf_ingest-0.0.84/tests/jf_jira/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.764246 jf_ingest-0.0.84/tests/jf_jira/fixtures/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/
--rw-r--r--   0 root         (0) root         (0)     1395 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/boards.json
--rw-r--r--   0 root         (0) root         (0)       87 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/boards_empty_agile_payload.json
--rw-r--r--   0 root         (0) root         (0)      857 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/boards_sprints_for_board_1.json
--rw-r--r--   0 root         (0) root         (0)      130 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/boards_sprints_for_board_1_links.json
--rw-r--r--   0 root         (0) root         (0)       74 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/boards_sprints_not_supported.json
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/fields.json
--rw-r--r--   0 root         (0) root         (0)     1436 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/issueLinkType.json
--rw-r--r--   0 root         (0) root         (0)    37181 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/issues.json
--rw-r--r--   0 root         (0) root         (0)     2478 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/issuetype.json
--rw-r--r--   0 root         (0) root         (0)     1520 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/priority.json
--rw-r--r--   0 root         (0) root         (0)     2122 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/project.json
--rw-r--r--   0 root         (0) root         (0)      356 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/project_components_OJ.json
--rw-r--r--   0 root         (0) root         (0)     6364 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/project_versions_JFR.json
--rw-r--r--   0 root         (0) root         (0)     5361 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/project_versions_OJ.json
--rw-r--r--   0 root         (0) root         (0)     1653 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/resolution.json
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/status.json
--rw-r--r--   0 root         (0) root         (0)      311 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/worklog_deleted.json
--rw-r--r--   0 root         (0) root         (0)    10225 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/worklog_list.json
--rw-r--r--   0 root         (0) root         (0)      995 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/worklog_updated.json
--rw-r--r--   0 root         (0) root         (0)     6602 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/jellyfish_issue_metadata.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/tests/jf_jira/fixtures/results/
--rw-r--r--   0 root         (0) root         (0)    16054 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/fixtures/results/project_version_component.json
--rw-r--r--   0 root         (0) root         (0)     8551 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_gql_utils.py
--rw-r--r--   0 root         (0) root         (0)     2753 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_auth.py
--rw-r--r--   0 root         (0) root         (0)     6585 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_boards_and_sprints.py
--rw-r--r--   0 root         (0) root         (0)     1780 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_fields.py
--rw-r--r--   0 root         (0) root         (0)      754 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_issuelinktype.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_issuetype.py
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_priority.py
--rw-r--r--   0 root         (0) root         (0)     6621 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_projects_and_versions.py
--rw-r--r--   0 root         (0) root         (0)      703 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_resolutions.py
--rw-r--r--   0 root         (0) root         (0)      814 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_status.py
--rw-r--r--   0 root         (0) root         (0)    16088 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_download_users.py
--rw-r--r--   0 root         (0) root         (0)    25490 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_issues.py
--rw-r--r--   0 root         (0) root         (0)     3261 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/test_jira_worklogs.py
--rw-r--r--   0 root         (0) root         (0)     4496 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/jf_jira/utils.py
--rw-r--r--   0 root         (0) root         (0)     9578 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/test_file_operations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 15:13:47.768246 jf_ingest-0.0.84/tests/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1999 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/utils/test_diagnostics.py
--rw-r--r--   0 root         (0) root         (0)     4781 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/utils/test_logging_helper.py
--rw-r--r--   0 root         (0) root         (0)    13819 2024-05-22 15:13:11.000000 jf_ingest-0.0.84/tests/utils/test_util_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      427 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       19 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.716625 jf-ingest-0.0.9/jf_ingest/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest/jf_git/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      217 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_git/standardized_models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest/jf_jira/
+-rw-r--r--   0 root         (0) root         (0)    10290 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5883 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/auth.py
+-rw-r--r--   0 root         (0) root         (0)     3217 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/jf_jira/downloaders.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3144 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/jf_ingest/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/jf_ingest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      427 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      611 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-10-16 19:49:45.000000 jf-ingest-0.0.9/jf_ingest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    34489 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/pdm.lock
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/jf_jira/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 19:49:45.720625 jf-ingest-0.0.9/tests/jf_jira/fixtures/
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/fixtures/jira_fields_response.json
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/test_jira_auth.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-10-16 19:49:14.000000 jf-ingest-0.0.9/tests/jf_jira/test_jira_downloaders.py
```

### Comparing `jf_ingest-0.0.84/.gitignore` & `jf-ingest-0.0.9/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -153,16 +153,10 @@
 .pytype/
 
 # Cython debug symbols
 cython_debug/
 
 # IDE templates
 .idea/
-.vscode/
 
 # Docker stuff
-.DS_Store
-
-# Test Harness Stuff
-creds.env
-config.yml
-output
+.DS_Store
```

### Comparing `jf_ingest-0.0.84/LICENSE` & `jf-ingest-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.84/tests/jf_jira/fixtures/api_responses/fields.json` & `jf-ingest-0.0.9/tests/jf_jira/fixtures/jira_fields_response.json`

 * *Files identical despite different names*

### Comparing `jf_ingest-0.0.84/tests/jf_jira/test_jira_auth.py` & `jf-ingest-0.0.9/tests/jf_jira/test_jira_auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,51 @@
-from unittest.mock import patch
-
-import pytest
 from jira import JIRAError
+from jf_ingest.utils import JiraRetryLimitExceeded
+import pytest
+from unittest.mock import Mock, patch
 
-from jf_ingest.config import JiraAuthConfig
-from jf_ingest.jf_jira.auth import JiraAuthenticationException, JiraAuthMethod, get_jira_connection
-from jf_ingest.jf_jira.exceptions import JiraRetryLimitExceeded
+from jf_ingest.jf_jira.auth import (
+    JiraAuthConfig,
+    JiraAuthMethod,
+    JiraAuthenticationException,
+    get_jira_connection,
+)
 
 
 def _get_jira_auth_config(args):
     company_slug = "test_company"
     url = "https://test-co.atlassian.net/"
     return JiraAuthConfig(company_slug=company_slug, url=url, **args)
 
 
+@pytest.fixture
+def mock_JIRA(mocker):
+    mock = Mock()
+    mocker.patch("jira.client.JIRA", return_value=mock)
+    return mock
+
+
 def test_jira_conn_basic_auth_no_auth():
-    config = _get_jira_auth_config({"available_auth_methods": [JiraAuthMethod.BasicAuth]})
+    config = _get_jira_auth_config({"auth_method": JiraAuthMethod.BasicAuth})
 
     with pytest.raises(RuntimeError) as excinfo:
         get_jira_connection(config)
 
     assert (
         str(excinfo.value)
         == f"No valid basic authentication mechanism for {config.url} - need a username/password combo or a personal access token"
     )
 
 
 def test_jira_conn_basic_auth_user_password():
     config = _get_jira_auth_config(
         {
-            "available_auth_methods": [JiraAuthMethod.BasicAuth],
+            "auth_method": JiraAuthMethod.BasicAuth,
             "user": "jira_user@test.co",
-            "password": "test_password",  # pragma: allowlist secret
+            "password": "test_password",
         }
     )
 
     # TEST BASIC AUTH ERROR LOGIC
     with patch("jf_ingest.jf_jira.auth.JIRA", side_effect=JIRAError(status_code=401)):
         with pytest.raises(JiraAuthenticationException):
             get_jira_connection(config, max_retries=0)
@@ -49,18 +59,15 @@
     with patch("jf_ingest.jf_jira.auth.JIRA", side_effect=JIRAError(status_code=429)):
         with pytest.raises(JiraRetryLimitExceeded):
             get_jira_connection(config, max_retries=0)
 
 
 def test_jira_conn_basic_auth_personal_access_token():
     config = _get_jira_auth_config(
-        {
-            "available_auth_methods": [JiraAuthMethod.BasicAuth],
-            "personal_access_token": "a_PAT",
-        }
+        {"auth_method": JiraAuthMethod.BasicAuth, "personal_access_token": "a_PAT"}
     )
 
     # TEST BASIC AUTH ERROR LOGIC
     with patch("jf_ingest.jf_jira.auth.JIRA", side_effect=JIRAError(status_code=401)):
         with pytest.raises(JiraAuthenticationException):
             get_jira_connection(config, max_retries=0)
```

