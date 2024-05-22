# Comparing `tmp/exasol_saas_api-0.5.0.tar.gz` & `tmp/exasol_saas_api-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_saas_api-0.5.0.tar", max compression
+gzip compressed data, was "exasol_saas_api-0.6.0.tar", max compression
```

## Comparing `exasol_saas_api-0.5.0.tar` & `exasol_saas_api-0.6.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     1063 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/LICENSE
--rw-r--r--   0        0        0      559 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/README.md
--rw-r--r--   0        0        0      939 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/__init__.py
--rw-r--r--   0        0        0     7831 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/api_access.py
--rw-r--r--   0        0        0      178 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/__init__.py
--rw-r--r--   0        0        0       47 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/__init__.py
--rw-r--r--   0        0        0     4453 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/create_cluster.py
--rw-r--r--   0        0        0     2861 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py
--rw-r--r--   0        0        0     4273 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/get_cluster.py
--rw-r--r--   0        0        0     4412 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py
--rw-r--r--   0        0        0     4206 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/list_clusters.py
--rw-r--r--   0        0        0     3240 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py
--rw-r--r--   0        0        0     2864 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/start_cluster.py
--rw-r--r--   0        0        0     2863 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py
--rw-r--r--   0        0        0     3241 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/update_cluster.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/__init__.py
--rw-r--r--   0        0        0     4112 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/create_database.py
--rw-r--r--   0        0        0     2656 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/delete_database.py
--rw-r--r--   0        0        0     3941 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/get_database.py
--rw-r--r--   0        0        0     3854 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/list_databases.py
--rw-r--r--   0        0        0     2659 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/start_database.py
--rw-r--r--   0        0        0     2658 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/stop_database.py
--rw-r--r--   0        0        0     3043 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/update_database.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/__init__.py
--rw-r--r--   0        0        0     5559 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/create_extension_instance.py
--rw-r--r--   0        0        0     3385 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/delete_extension_instance.py
--rw-r--r--   0        0        0     4896 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/get_extension.py
--rw-r--r--   0        0        0     3172 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/install_extension.py
--rw-r--r--   0        0        0     5201 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/list_extension_instances.py
--rw-r--r--   0        0        0     4234 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/list_extensions.py
--rw-r--r--   0        0        0     3174 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/uninstall_extension.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/__init__.py
--rw-r--r--   0        0        0     2773 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/create_folder.py
--rw-r--r--   0        0        0     2774 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/delete_file.py
--rw-r--r--   0        0        0     2775 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/delete_folder.py
--rw-r--r--   0        0        0     4205 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/download_file.py
--rw-r--r--   0        0        0     4164 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/list_files.py
--rw-r--r--   0        0        0     4171 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/upload_file.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/__init__.py
--rw-r--r--   0        0        0     3851 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py
--rw-r--r--   0        0        0     3460 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_platforms.py
--rw-r--r--   0        0        0     3787 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_regions.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/profile/__init__.py
--rw-r--r--   0        0        0     2607 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/profile/update_profile.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/__init__.py
--rw-r--r--   0        0        0     4150 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py
--rw-r--r--   0        0        0     2716 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py
--rw-r--r--   0        0        0     4047 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py
--rw-r--r--   0        0        0     3880 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py
--rw-r--r--   0        0        0     3111 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/usage/__init__.py
--rw-r--r--   0        0        0     4841 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/usage/get_usage.py
--rw-r--r--   0        0        0        0 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/__init__.py
--rw-r--r--   0        0        0     2604 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/delete_user.py
--rw-r--r--   0        0        0     3814 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/get_user.py
--rw-r--r--   0        0        0     5224 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/list_users.py
--rw-r--r--   0        0        0     2958 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/patch_user.py
--rw-r--r--   0        0        0    12455 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/client.py
--rw-r--r--   0        0        0      546 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/errors.py
--rw-r--r--   0        0        0     2747 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/__init__.py
--rw-r--r--   0        0        0     2584 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/allowed_ip.py
--rw-r--r--   0        0        0     2332 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/api_error.py
--rw-r--r--   0        0        0     1063 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/auto_stop.py
--rw-r--r--   0        0        0     3752 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster.py
--rw-r--r--   0        0        0     1760 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster_connection.py
--rw-r--r--   0        0        0     1639 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster_size.py
--rw-r--r--   0        0        0     1143 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/connection_i_ps.py
--rw-r--r--   0        0        0     1041 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_allowed_ip.py
--rw-r--r--   0        0        0     1786 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_cluster.py
--rw-r--r--   0        0        0     2607 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_database.py
--rw-r--r--   0        0        0     1850 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_database_initial_cluster.py
--rw-r--r--   0        0        0     1787 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_extension_instance.py
--rw-r--r--   0        0        0     5263 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database.py
--rw-r--r--   0        0        0     1055 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database_clusters.py
--rw-r--r--   0        0        0     1962 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database_integrations_item.py
--rw-r--r--   0        0        0      846 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/download_file.py
--rw-r--r--   0        0        0     2439 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension.py
--rw-r--r--   0        0        0     2263 2024-05-16 15:43:28.993543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_detail.py
--rw-r--r--   0        0        0      999 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_instance.py
--rw-r--r--   0        0        0     1396 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_parameter_definitions.py
--rw-r--r--   0        0        0     1035 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_parameter_value.py
--rw-r--r--   0        0        0     1467 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_version.py
--rw-r--r--   0        0        0     2448 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/file.py
--rw-r--r--   0        0        0      151 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/get_usage_type.py
--rw-r--r--   0        0        0     2151 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/patch_user.py
--rw-r--r--   0        0        0     1123 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/patch_user_databases.py
--rw-r--r--   0        0        0      961 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/platform.py
--rw-r--r--   0        0        0     1453 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/region.py
--rw-r--r--   0        0        0      856 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/scale_cluster.py
--rw-r--r--   0        0        0      485 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/status.py
--rw-r--r--   0        0        0     1041 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_allowed_ip.py
--rw-r--r--   0        0        0     1643 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_cluster.py
--rw-r--r--   0        0        0     1558 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_database.py
--rw-r--r--   0        0        0     1109 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_profile.py
--rw-r--r--   0        0        0      838 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/upload_file.py
--rw-r--r--   0        0        0     2479 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage.py
--rw-r--r--   0        0        0     2124 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage_additional_property_item.py
--rw-r--r--   0        0        0     2469 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage_cluster.py
--rw-r--r--   0        0        0     4420 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user.py
--rw-r--r--   0        0        0      979 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user_database.py
--rw-r--r--   0        0        0      963 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user_role.py
--rw-r--r--   0        0        0      193 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user_status.py
--rw-r--r--   0        0        0       25 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/py.typed
--rw-r--r--   0        0        0     1034 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/exasol/saas/client/openapi/types.py
--rw-r--r--   0        0        0     2191 2024-05-16 15:43:28.997543 exasol_saas_api-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2119 1970-01-01 00:00:00.000000 exasol_saas_api-0.5.0/setup.py
--rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 exasol_saas_api-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/LICENSE
+-rw-r--r--   0        0        0      559 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/README.md
+-rw-r--r--   0        0        0      939 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/__init__.py
+-rw-r--r--   0        0        0    10641 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/api_access.py
+-rw-r--r--   0        0        0      178 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/__init__.py
+-rw-r--r--   0        0        0       47 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/__init__.py
+-rw-r--r--   0        0        0     4453 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/create_cluster.py
+-rw-r--r--   0        0        0     2861 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py
+-rw-r--r--   0        0        0     4273 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/get_cluster.py
+-rw-r--r--   0        0        0     4412 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py
+-rw-r--r--   0        0        0     4206 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/list_clusters.py
+-rw-r--r--   0        0        0     3240 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py
+-rw-r--r--   0        0        0     2864 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/start_cluster.py
+-rw-r--r--   0        0        0     2863 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py
+-rw-r--r--   0        0        0     3241 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/update_cluster.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/__init__.py
+-rw-r--r--   0        0        0     4112 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/create_database.py
+-rw-r--r--   0        0        0     2656 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/delete_database.py
+-rw-r--r--   0        0        0     3941 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/get_database.py
+-rw-r--r--   0        0        0     3854 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/list_databases.py
+-rw-r--r--   0        0        0     2659 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/start_database.py
+-rw-r--r--   0        0        0     2658 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/stop_database.py
+-rw-r--r--   0        0        0     3043 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/update_database.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/__init__.py
+-rw-r--r--   0        0        0     5559 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/create_extension_instance.py
+-rw-r--r--   0        0        0     3385 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/delete_extension_instance.py
+-rw-r--r--   0        0        0     4896 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/get_extension.py
+-rw-r--r--   0        0        0     3172 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/install_extension.py
+-rw-r--r--   0        0        0     5201 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/list_extension_instances.py
+-rw-r--r--   0        0        0     4234 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/list_extensions.py
+-rw-r--r--   0        0        0     3174 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/uninstall_extension.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/__init__.py
+-rw-r--r--   0        0        0     2773 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/create_folder.py
+-rw-r--r--   0        0        0     2774 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/delete_file.py
+-rw-r--r--   0        0        0     2775 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/delete_folder.py
+-rw-r--r--   0        0        0     4205 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/download_file.py
+-rw-r--r--   0        0        0     4164 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/list_files.py
+-rw-r--r--   0        0        0     4171 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/upload_file.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/__init__.py
+-rw-r--r--   0        0        0     3851 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py
+-rw-r--r--   0        0        0     3460 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_platforms.py
+-rw-r--r--   0        0        0     3787 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_regions.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/profile/__init__.py
+-rw-r--r--   0        0        0     2607 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/profile/update_profile.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/__init__.py
+-rw-r--r--   0        0        0     4150 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py
+-rw-r--r--   0        0        0     2716 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py
+-rw-r--r--   0        0        0     4047 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py
+-rw-r--r--   0        0        0     3880 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py
+-rw-r--r--   0        0        0     3111 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/usage/__init__.py
+-rw-r--r--   0        0        0     4841 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/usage/get_usage.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/__init__.py
+-rw-r--r--   0        0        0     2604 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/delete_user.py
+-rw-r--r--   0        0        0     3814 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/get_user.py
+-rw-r--r--   0        0        0     5224 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/list_users.py
+-rw-r--r--   0        0        0     2958 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/patch_user.py
+-rw-r--r--   0        0        0    12455 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/client.py
+-rw-r--r--   0        0        0      546 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/errors.py
+-rw-r--r--   0        0        0     2747 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/__init__.py
+-rw-r--r--   0        0        0     2584 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/allowed_ip.py
+-rw-r--r--   0        0        0     2332 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/api_error.py
+-rw-r--r--   0        0        0     1063 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/auto_stop.py
+-rw-r--r--   0        0        0     3752 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster.py
+-rw-r--r--   0        0        0     1760 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster_connection.py
+-rw-r--r--   0        0        0     1639 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster_size.py
+-rw-r--r--   0        0        0     1143 2024-05-22 10:38:45.124636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/connection_i_ps.py
+-rw-r--r--   0        0        0     1041 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_allowed_ip.py
+-rw-r--r--   0        0        0     1786 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_cluster.py
+-rw-r--r--   0        0        0     2607 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_database.py
+-rw-r--r--   0        0        0     1850 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_database_initial_cluster.py
+-rw-r--r--   0        0        0     1787 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_extension_instance.py
+-rw-r--r--   0        0        0     5263 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database.py
+-rw-r--r--   0        0        0     1055 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database_clusters.py
+-rw-r--r--   0        0        0     1962 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database_integrations_item.py
+-rw-r--r--   0        0        0      846 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/download_file.py
+-rw-r--r--   0        0        0     2439 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension.py
+-rw-r--r--   0        0        0     2263 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_detail.py
+-rw-r--r--   0        0        0      999 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_instance.py
+-rw-r--r--   0        0        0     1396 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_parameter_definitions.py
+-rw-r--r--   0        0        0     1035 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_parameter_value.py
+-rw-r--r--   0        0        0     1467 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_version.py
+-rw-r--r--   0        0        0     2448 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/file.py
+-rw-r--r--   0        0        0      151 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/get_usage_type.py
+-rw-r--r--   0        0        0     2151 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/patch_user.py
+-rw-r--r--   0        0        0     1123 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/patch_user_databases.py
+-rw-r--r--   0        0        0      961 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/platform.py
+-rw-r--r--   0        0        0     1453 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/region.py
+-rw-r--r--   0        0        0      856 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/scale_cluster.py
+-rw-r--r--   0        0        0      485 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/status.py
+-rw-r--r--   0        0        0     1041 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_allowed_ip.py
+-rw-r--r--   0        0        0     1643 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_cluster.py
+-rw-r--r--   0        0        0     1558 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_database.py
+-rw-r--r--   0        0        0     1109 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_profile.py
+-rw-r--r--   0        0        0      838 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/upload_file.py
+-rw-r--r--   0        0        0     2479 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage.py
+-rw-r--r--   0        0        0     2124 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage_additional_property_item.py
+-rw-r--r--   0        0        0     2469 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage_cluster.py
+-rw-r--r--   0        0        0     4420 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user.py
+-rw-r--r--   0        0        0      979 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user_database.py
+-rw-r--r--   0        0        0      963 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user_role.py
+-rw-r--r--   0        0        0      193 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user_status.py
+-rw-r--r--   0        0        0       25 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/py.typed
+-rw-r--r--   0        0        0     1034 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/exasol/saas/client/openapi/types.py
+-rw-r--r--   0        0        0     2213 2024-05-22 10:38:45.128636 exasol_saas_api-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2119 1970-01-01 00:00:00.000000 exasol_saas_api-0.6.0/setup.py
+-rw-r--r--   0        0        0     1917 1970-01-01 00:00:00.000000 exasol_saas_api-0.6.0/PKG-INFO
```

### Comparing `exasol_saas_api-0.5.0/LICENSE` & `exasol_saas_api-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/README.md` & `exasol_saas_api-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/__init__.py` & `exasol_saas_api-0.6.0/exasol/saas/client/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/api_access.py` & `exasol_saas_api-0.6.0/exasol/saas/client/api_access.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import getpass
 import logging
 import time
 
-from typing import Iterable, List, Optional
+from typing import Iterable, List, Optional, Any
 from contextlib import contextmanager
 import datetime as dt
 from datetime import datetime, timedelta
 
 from tenacity import retry, TryAgain
 from tenacity.wait import wait_fixed
 from tenacity.stop import stop_after_delay
@@ -28,14 +28,15 @@
     list_clusters,
 )
 from exasol.saas.client.openapi.api.security import (
     list_allowed_i_ps,
     add_allowed_ip,
     delete_allowed_ip,
 )
+from exasol.saas.client.openapi.types import UNSET
 
 
 LOG = logging.getLogger(__name__)
 LOG.setLevel(logging.INFO)
 
 
 def timestamp_name(project_short_tag: str | None = None) -> str:
@@ -72,14 +73,83 @@
     return openapi.AuthenticatedClient(
         base_url=host,
         token=pat,
         raise_on_unexpected_status = raise_on_unexpected_status,
     )
 
 
+def _get_database_id(
+        account_id: str,
+        client: openapi.AuthenticatedClient,
+        database_name: str,
+) -> str:
+    """
+    Finds the database id, given an optional database name. If the name is not
+    provided returns an id of any non-deleted database. The latter option may be
+    useful for testing.
+    """
+    dbs = list_databases.sync(account_id, client=client)
+    dbs = list(filter(lambda db: (db.name == database_name) and         # type: ignore
+                                 (db.deleted_at is UNSET) and           # type: ignore
+                                 (db.deleted_by is UNSET), dbs))        # type: ignore
+    if not dbs:
+        raise RuntimeError(f'SaaS database {database_name} was not found.')
+    return dbs[0].id
+
+
+def get_connection_params(
+        host: str,
+        account_id: str,
+        pat: str,
+        database_id: str | None = None,
+        database_name: str | None = None,
+) -> dict[str, Any]:
+    """
+    Gets the database connection parameters, such as those required by pyexasol:
+    - dns
+    - user
+    - password.
+    Returns the parameters in a dictionary that can be used as kwargs when
+    creating a connection, like in the code below:
+
+    connection_params = get_connection_params(...)
+    connection = pyexasol.connect(**connection_params)
+
+    Args:
+        host:           SaaS service URL.
+        account_id:     User account ID
+        pat:            Personal Access Token.
+        database_id:    Database ID, id known.
+        database_name:  Database name, in case the id is unknown.
+    """
+
+    with create_saas_client(host, pat) as client:
+        if not database_id:
+            if not database_name:
+                raise ValueError(('To get SaaS connection parameters, '
+                                  'either database name or database id must be provided.'))
+            database_id = _get_database_id(account_id, client, database_name=database_name)
+        clusters = list_clusters.sync(account_id,
+                                      database_id,
+                                      client=client)
+        cluster_id = next(filter(lambda cl: cl.main_cluster, clusters)).id  # type: ignore
+        connections = get_cluster_connection.sync(account_id,
+                                                  database_id,
+                                                  cluster_id,
+                                                  client=client)
+        if connections is None:
+            raise RuntimeError('Failed to get the SaaS connection data.')
+        connection_params = {
+            'dsn': f'{connections.dns}:{connections.port}',
+            'user': connections.db_username,
+            'password': pat
+        }
+        return connection_params
+
+
 class OpenApiAccess:
     """
     This class is meant to be used only in the context of the API
     generator repository while integration tests in other repositories are
     planned to only use fixture ``saas_database_id()``.
     """
 
@@ -186,15 +256,14 @@
                 print(f'status = {db.status}')
                 raise TryAgain
             return db.status
 
         if poll_status() not in success:
             raise DatabaseStartupFailure()
 
-
     def clusters(
             self,
             database_id: str,
     ) -> Optional[List[openapi.models.Cluster]]:
         return list_clusters.sync(
             self._account_id,
             database_id,
```

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/create_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/create_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/get_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/get_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/list_clusters.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/list_clusters.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/start_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/start_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/clusters/update_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/clusters/update_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/create_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/create_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/delete_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/delete_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/get_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/get_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/list_databases.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/list_databases.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/start_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/start_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/stop_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/stop_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/databases/update_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/databases/update_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/create_extension_instance.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/create_extension_instance.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/delete_extension_instance.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/delete_extension_instance.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/get_extension.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/get_extension.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/install_extension.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/install_extension.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/list_extension_instances.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/list_extension_instances.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/list_extensions.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/list_extensions.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/extensions/uninstall_extension.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/extensions/uninstall_extension.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/create_folder.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/create_folder.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/delete_file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/delete_file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/delete_folder.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/delete_folder.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/download_file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/download_file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/list_files.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/list_files.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/files/upload_file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/files/upload_file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_platforms.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_platforms.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/platform/list_regions.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/platform/list_regions.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/profile/update_profile.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/profile/update_profile.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/usage/get_usage.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/usage/get_usage.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/delete_user.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/delete_user.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/get_user.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/get_user.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/list_users.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/list_users.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/api/users/patch_user.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/api/users/patch_user.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/client.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/client.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/errors.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/errors.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/__init__.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/api_error.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/api_error.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/auto_stop.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/auto_stop.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster_connection.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster_connection.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/cluster_size.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/cluster_size.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/connection_i_ps.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/connection_i_ps.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_database_initial_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_database_initial_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/create_extension_instance.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/create_extension_instance.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database_clusters.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database_clusters.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/database_integrations_item.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/database_integrations_item.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/download_file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/download_file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_detail.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_detail.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_instance.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_instance.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_parameter_definitions.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_parameter_definitions.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_parameter_value.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_parameter_value.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/extension_version.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/extension_version.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/patch_user.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/patch_user.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/patch_user_databases.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/patch_user_databases.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/platform.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/platform.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/region.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/region.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/scale_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/scale_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_allowed_ip.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/update_profile.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/update_profile.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/upload_file.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage_additional_property_item.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage_additional_property_item.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/usage_cluster.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/usage_cluster.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user_database.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user_database.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/models/user_role.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/models/user_role.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/exasol/saas/client/openapi/types.py` & `exasol_saas_api-0.6.0/exasol/saas/client/openapi/types.py`

 * *Files identical despite different names*

### Comparing `exasol_saas_api-0.5.0/pyproject.toml` & `exasol_saas_api-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "exasol-saas-api"
-version = "0.5.0"
+version = "0.6.0"
 description = "API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services"
 packages = [ {include = "exasol"}, ]
 authors = [ "Christoph Kuhnke <christoph.kuhnke@exasol.com>" ]
 maintainers = [ "Christoph Kuhnke <christoph.kuhnke@exasol.com>" ]
 classifiers = [
    "Programming Language :: Python :: 3",
    "Development Status :: 3 - Alpha",
@@ -38,14 +38,15 @@
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.1"
 pytest-mock = "^3.7.0"
 exasol-toolbox = "^0.9.0"
 openapi-python-client = "^0.19.1"
+pyexasol = ">=0.25.0"
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 
 testpaths = [
     "test"
```

### Comparing `exasol_saas_api-0.5.0/setup.py` & `exasol_saas_api-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
  'types-requests>=2.31.0.6,<3.0.0.0']
 
 entry_points = \
 {'console_scripts': ['tbx = exasol.toolbox.tools.tbx:CLI']}
 
 setup_kwargs = {
     'name': 'exasol-saas-api',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services',
     'long_description': '# SaaS API for Python\n\nAPI enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services.\n\nThe model layer of this API is generated from the OpenAPI specification in JSON format of the SaaS API https://cloud.exasol.com/openapi.json using [openapi-python-client](https://github.com/openapi-generators/openapi-python-client).\n\nA GitHub action will check each morning if the generated model layer is outdated.\n\nSee\n* [User Guide](doc/user_guide/user-guide.md)\n* [Developer Guide](doc/developer_guide/developer_guide.md)\n',
     'author': 'Christoph Kuhnke',
     'author_email': 'christoph.kuhnke@exasol.com',
     'maintainer': 'Christoph Kuhnke',
     'maintainer_email': 'christoph.kuhnke@exasol.com',
     'url': 'None',
```

### Comparing `exasol_saas_api-0.5.0/PKG-INFO` & `exasol_saas_api-0.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exasol-saas-api
-Version: 0.5.0
+Version: 0.6.0
 Summary: API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services
 License: MIT
 Author: Christoph Kuhnke
 Author-email: christoph.kuhnke@exasol.com
 Maintainer: Christoph Kuhnke
 Maintainer-email: christoph.kuhnke@exasol.com
 Requires-Python: >=3.8.0,<4.0
```

