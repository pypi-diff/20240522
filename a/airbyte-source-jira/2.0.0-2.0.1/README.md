# Comparing `tmp/airbyte_source_jira-2.0.0.tar.gz` & `tmp/airbyte_source_jira-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_jira-2.0.0.tar", max compression
+gzip compressed data, was "airbyte_source_jira-2.0.1.tar", max compression
```

## Comparing `airbyte_source_jira-2.0.0.tar` & `airbyte_source_jira-2.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     4470 2024-05-13 12:54:10.648111 airbyte_source_jira-2.0.0/README.md
--rw-r--r--   0        0        0      756 2024-05-13 12:58:19.468801 airbyte_source_jira-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       57 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/components/__init__.py
--rw-r--r--   0        0        0      773 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/components/extractors.py
--rw-r--r--   0        0        0     5524 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/components/partition_routers.py
--rw-r--r--   0        0        0      894 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/components/transformations.py
--rw-r--r--   0        0        0    47437 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/manifest.yaml
--rw-r--r--   0        0        0      224 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/run.py
--rw-r--r--   0        0        0     2897 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/application_roles.json
--rw-r--r--   0        0        0     4192 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/audit_records.json
--rw-r--r--   0        0        0     1339 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/avatars.json
--rw-r--r--   0        0        0     2910 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/board_issues.json
--rw-r--r--   0        0        0     2278 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/boards.json
--rw-r--r--   0        0        0   104863 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/dashboards.json
--rw-r--r--   0        0        0     1388 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/dynamic_modules.json
--rw-r--r--   0        0        0    95171 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/filter_sharing.json
--rw-r--r--   0        0        0   129222 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/filters.json
--rw-r--r--   0        0        0      612 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/groups.json
--rw-r--r--   0        0        0      618 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_comment_properties.json
--rw-r--r--   0        0        0     2336 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_comments.json
--rw-r--r--   0        0        0      956 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_contexts.json
--rw-r--r--   0        0        0      972 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_options.json
--rw-r--r--   0        0        0     3340 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_options_apps.json
--rw-r--r--   0        0        0      635 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_field_configurations.json
--rw-r--r--   0        0        0     6060 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_fields.json
--rw-r--r--   0        0        0     1269 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_link_types.json
--rw-r--r--   0        0        0      486 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_navigator_settings.json
--rw-r--r--   0        0        0    28698 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_notification_schemes.json
--rw-r--r--   0        0        0      951 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_priorities.json
--rw-r--r--   0        0        0      755 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_properties.json
--rw-r--r--   0        0        0     4830 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_remote_links.json
--rw-r--r--   0        0        0      737 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_resolutions.json
--rw-r--r--   0        0        0     1759 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_security_schemes.json
--rw-r--r--   0        0        0     3210 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_transitions.json
--rw-r--r--   0        0        0      522 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_properties.json
--rw-r--r--   0        0        0      822 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_schemes.json
--rw-r--r--   0        0        0      533 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_screen_schemes.json
--rw-r--r--   0        0        0     5082 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_types.json
--rw-r--r--   0        0        0     9838 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_votes.json
--rw-r--r--   0        0        0     3803 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_watchers.json
--rw-r--r--   0        0        0     9310 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issue_worklogs.json
--rw-r--r--   0        0        0    39688 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/issues.json
--rw-r--r--   0        0        0     1400 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/jira_settings.json
--rw-r--r--   0        0        0     2768 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/jql.json
--rw-r--r--   0        0        0      179 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/labels.json
--rw-r--r--   0        0        0     6468 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/permission_schemes.json
--rw-r--r--   0        0        0      611 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/permissions.json
--rw-r--r--   0        0        0     1448 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_avatars.json
--rw-r--r--   0        0        0      718 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_categories.json
--rw-r--r--   0        0        0    21156 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_components.json
--rw-r--r--   0        0        0      409 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_email.json
--rw-r--r--   0        0        0      789 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_permission_schemes.json
--rw-r--r--   0        0        0     6610 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_roles.json
--rw-r--r--   0        0        0      837 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_types.json
--rw-r--r--   0        0        0     4857 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/project_versions.json
--rw-r--r--   0        0        0     5224 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/projects.json
--rw-r--r--   0        0        0     1885 2024-05-13 12:54:10.652111 airbyte_source_jira-2.0.0/source_jira/schemas/pull_requests.json
--rw-r--r--   0        0        0     1290 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/screen_schemes.json
--rw-r--r--   0        0        0      678 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/screen_tab_fields.json
--rw-r--r--   0        0        0      551 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/screen_tabs.json
--rw-r--r--   0        0        0     3829 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/screens.json
--rw-r--r--   0        0        0     2022 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/server_info.json
--rw-r--r--   0        0        0     4810 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/sprint_issues.json
--rw-r--r--   0        0        0     1559 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/sprints.json
--rw-r--r--   0        0        0      735 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/time_tracking.json
--rw-r--r--   0        0        0     8052 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/users.json
--rw-r--r--   0        0        0     7841 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/users_groups_detailed.json
--rw-r--r--   0        0        0     1012 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/webhooks.json
--rw-r--r--   0        0        0    11945 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_scheme_drafts.json
--rw-r--r--   0        0        0    13097 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_scheme_project_associations.json
--rw-r--r--   0        0        0    11774 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_schemes.json
--rw-r--r--   0        0        0      824 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_status_categories.json
--rw-r--r--   0        0        0     1933 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_statuses.json
--rw-r--r--   0        0        0      633 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_transition_properties.json
--rw-r--r--   0        0        0     4158 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflow_transition_rules.json
--rw-r--r--   0        0        0     5138 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/schemas/workflows.json
--rw-r--r--   0        0        0     4405 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/source.py
--rw-r--r--   0        0        0     4334 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/spec.json
--rw-r--r--   0        0        0    19295 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/streams.py
--rw-r--r--   0        0        0     1068 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/type_transfromer.py
--rw-r--r--   0        0        0     1035 2024-05-13 12:54:10.656111 airbyte_source_jira-2.0.0/source_jira/utils.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 airbyte_source_jira-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4470 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/README.md
+-rw-r--r--   0        0        0      756 2024-05-22 15:25:22.174807 airbyte_source_jira-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       57 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/components/__init__.py
+-rw-r--r--   0        0        0      773 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/components/extractors.py
+-rw-r--r--   0        0        0     5524 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/components/partition_routers.py
+-rw-r--r--   0        0        0      894 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/components/transformations.py
+-rw-r--r--   0        0        0    47437 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/manifest.yaml
+-rw-r--r--   0        0        0      224 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/run.py
+-rw-r--r--   0        0        0     2897 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/application_roles.json
+-rw-r--r--   0        0        0     4192 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/audit_records.json
+-rw-r--r--   0        0        0     1339 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/avatars.json
+-rw-r--r--   0        0        0     2910 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/board_issues.json
+-rw-r--r--   0        0        0     2278 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/boards.json
+-rw-r--r--   0        0        0   104863 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/dashboards.json
+-rw-r--r--   0        0        0     1388 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/dynamic_modules.json
+-rw-r--r--   0        0        0    95171 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/filter_sharing.json
+-rw-r--r--   0        0        0   129222 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/filters.json
+-rw-r--r--   0        0        0      612 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/groups.json
+-rw-r--r--   0        0        0      618 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_comment_properties.json
+-rw-r--r--   0        0        0     2336 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_comments.json
+-rw-r--r--   0        0        0      956 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_contexts.json
+-rw-r--r--   0        0        0      972 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_options.json
+-rw-r--r--   0        0        0     3340 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_options_apps.json
+-rw-r--r--   0        0        0      635 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_field_configurations.json
+-rw-r--r--   0        0        0     6060 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_fields.json
+-rw-r--r--   0        0        0     1269 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_link_types.json
+-rw-r--r--   0        0        0      486 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_navigator_settings.json
+-rw-r--r--   0        0        0    28698 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_notification_schemes.json
+-rw-r--r--   0        0        0      951 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_priorities.json
+-rw-r--r--   0        0        0      755 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_properties.json
+-rw-r--r--   0        0        0     4830 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_remote_links.json
+-rw-r--r--   0        0        0      737 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_resolutions.json
+-rw-r--r--   0        0        0     1759 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_security_schemes.json
+-rw-r--r--   0        0        0     3210 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_transitions.json
+-rw-r--r--   0        0        0      522 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_properties.json
+-rw-r--r--   0        0        0      822 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_schemes.json
+-rw-r--r--   0        0        0      533 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_screen_schemes.json
+-rw-r--r--   0        0        0     5082 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_types.json
+-rw-r--r--   0        0        0     9838 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_votes.json
+-rw-r--r--   0        0        0     3803 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_watchers.json
+-rw-r--r--   0        0        0     9310 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issue_worklogs.json
+-rw-r--r--   0        0        0    39688 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/issues.json
+-rw-r--r--   0        0        0     1400 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/jira_settings.json
+-rw-r--r--   0        0        0     2768 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/jql.json
+-rw-r--r--   0        0        0      179 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/labels.json
+-rw-r--r--   0        0        0     6468 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/permission_schemes.json
+-rw-r--r--   0        0        0      611 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/permissions.json
+-rw-r--r--   0        0        0     1448 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_avatars.json
+-rw-r--r--   0        0        0      718 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_categories.json
+-rw-r--r--   0        0        0    21156 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_components.json
+-rw-r--r--   0        0        0      409 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_email.json
+-rw-r--r--   0        0        0      789 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_permission_schemes.json
+-rw-r--r--   0        0        0     6610 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_roles.json
+-rw-r--r--   0        0        0      837 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_types.json
+-rw-r--r--   0        0        0     4857 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/project_versions.json
+-rw-r--r--   0        0        0     5224 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/projects.json
+-rw-r--r--   0        0        0     1885 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/pull_requests.json
+-rw-r--r--   0        0        0     1290 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/screen_schemes.json
+-rw-r--r--   0        0        0      678 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/screen_tab_fields.json
+-rw-r--r--   0        0        0      551 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/screen_tabs.json
+-rw-r--r--   0        0        0     3829 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/screens.json
+-rw-r--r--   0        0        0     2022 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/server_info.json
+-rw-r--r--   0        0        0     4810 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/sprint_issues.json
+-rw-r--r--   0        0        0     1559 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/sprints.json
+-rw-r--r--   0        0        0      735 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/time_tracking.json
+-rw-r--r--   0        0        0     8052 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/users.json
+-rw-r--r--   0        0        0     7841 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/users_groups_detailed.json
+-rw-r--r--   0        0        0     1012 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/webhooks.json
+-rw-r--r--   0        0        0    11945 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_scheme_drafts.json
+-rw-r--r--   0        0        0    13097 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_scheme_project_associations.json
+-rw-r--r--   0        0        0    11774 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_schemes.json
+-rw-r--r--   0        0        0      824 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_status_categories.json
+-rw-r--r--   0        0        0     1933 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_statuses.json
+-rw-r--r--   0        0        0      633 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_transition_properties.json
+-rw-r--r--   0        0        0     4158 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflow_transition_rules.json
+-rw-r--r--   0        0        0     5138 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/schemas/workflows.json
+-rw-r--r--   0        0        0     4421 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/source.py
+-rw-r--r--   0        0        0     4334 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/spec.json
+-rw-r--r--   0        0        0    19295 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/streams.py
+-rw-r--r--   0        0        0     1068 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/type_transfromer.py
+-rw-r--r--   0        0        0     1035 2024-05-22 14:54:39.000000 airbyte_source_jira-2.0.1/source_jira/utils.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 airbyte_source_jira-2.0.1/PKG-INFO
```

### Comparing `airbyte_source_jira-2.0.0/README.md` & `airbyte_source_jira-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/pyproject.toml` & `airbyte_source_jira-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.0"
+version = "2.0.1"
 name = "airbyte-source-jira"
 description = "Source implementation for Jira."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_jira-2.0.0/source_jira/components/extractors.py` & `airbyte_source_jira-2.0.1/source_jira/components/extractors.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/components/partition_routers.py` & `airbyte_source_jira-2.0.1/source_jira/components/partition_routers.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/components/transformations.py` & `airbyte_source_jira-2.0.1/source_jira/components/transformations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/manifest.yaml` & `airbyte_source_jira-2.0.1/source_jira/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/application_roles.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/application_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/audit_records.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/audit_records.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/avatars.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/avatars.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/board_issues.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/board_issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/boards.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/boards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/dashboards.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/dashboards.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/dynamic_modules.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/dynamic_modules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/filter_sharing.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/filter_sharing.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/filters.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/filters.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/groups.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/groups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_comment_properties.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_comment_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_comments.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_comments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_contexts.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_contexts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_options.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_options.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_custom_field_options_apps.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_custom_field_options_apps.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_field_configurations.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_field_configurations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_fields.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_link_types.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_link_types.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_notification_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_notification_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_priorities.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_priorities.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_properties.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_remote_links.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_remote_links.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_resolutions.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_resolutions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_security_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_security_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_transitions.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_transitions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_properties.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_type_screen_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_type_screen_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_types.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_types.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_votes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_votes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_watchers.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_watchers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issue_worklogs.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issue_worklogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/issues.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/jira_settings.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/jira_settings.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/jql.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/jql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/permission_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/permission_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/permissions.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/permissions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_avatars.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_avatars.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_categories.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_components.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_components.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_permission_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_permission_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_roles.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_roles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_types.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_types.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/project_versions.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/project_versions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/projects.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/projects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/pull_requests.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/pull_requests.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/screen_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/screen_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/screen_tab_fields.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/screen_tab_fields.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/screen_tabs.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/screen_tabs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/screens.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/screens.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/server_info.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/server_info.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/sprint_issues.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/sprint_issues.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/sprints.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/sprints.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/time_tracking.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/time_tracking.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/users.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/users_groups_detailed.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/users_groups_detailed.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/webhooks.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/webhooks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_scheme_drafts.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_scheme_drafts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_scheme_project_associations.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_scheme_project_associations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_schemes.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_schemes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_status_categories.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_status_categories.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_statuses.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_statuses.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_transition_properties.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_transition_properties.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflow_transition_rules.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflow_transition_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/schemas/workflows.json` & `airbyte_source_jira-2.0.1/source_jira/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/source.py` & `airbyte_source_jira-2.0.1/source_jira/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, List, Mapping, Tuple
 
 import pendulum
 from airbyte_cdk.models import FailureType
 from airbyte_cdk.sources.declarative.exceptions import ReadException
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams.core import Stream
-from airbyte_cdk.sources.streams.http.auth import BasicHttpAuthenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth import BasicHttpAuthenticator
 from airbyte_cdk.utils.traced_exception import AirbyteTracedException
 from pydantic.error_wrappers import ValidationError
 from requests.exceptions import InvalidURL
 
 from .streams import IssueComments, IssueFields, Issues, IssueWorklogs, PullRequests
 from .utils import read_full_refresh
```

### Comparing `airbyte_source_jira-2.0.0/source_jira/spec.json` & `airbyte_source_jira-2.0.1/source_jira/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/streams.py` & `airbyte_source_jira-2.0.1/source_jira/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/type_transfromer.py` & `airbyte_source_jira-2.0.1/source_jira/type_transfromer.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/source_jira/utils.py` & `airbyte_source_jira-2.0.1/source_jira/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_jira-2.0.0/PKG-INFO` & `airbyte_source_jira-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-jira
-Version: 2.0.0
+Version: 2.0.1
 Summary: Source implementation for Jira.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

