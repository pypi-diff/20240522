# Comparing `tmp/exasol_script_languages_container_tool-0.18.3.tar.gz` & `tmp/exasol_script_languages_container_tool-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exasol_script_languages_container_tool-0.18.3.tar", max compression
+gzip compressed data, was "exasol_script_languages_container_tool-0.19.0.tar", max compression
```

## Comparing `exasol_script_languages_container_tool-0.18.3.tar` & `exasol_script_languages_container_tool-0.19.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0     1063 2024-05-13 11:59:26.329851 exasol_script_languages_container_tool-0.18.3/LICENSE
--rw-r--r--   0        0        0     7271 2024-05-13 11:59:26.329851 exasol_script_languages_container_tool-0.18.3/README.md
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/__init__.py
--rw-r--r--   0        0        0      501 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/__init__.py
--rw-r--r--   0        0        0     4511 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/build.py
--rw-r--r--   0        0        0     3231 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/build_test_container.py
--rw-r--r--   0        0        0     3145 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/clean.py
--rw-r--r--   0        0        0     4539 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/export.py
--rw-r--r--   0        0        0     1066 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
--rw-r--r--   0        0        0     1070 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
--rw-r--r--   0        0        0     3759 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/push.py
--rw-r--r--   0        0        0     3571 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/push_test_container.py
--rw-r--r--   0        0        0    13335 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
--rw-r--r--   0        0        0     4251 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/save.py
--rw-r--r--   0        0        0     4413 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/security_scan.py
--rw-r--r--   0        0        0     5364 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/upload.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/__init__.py
--rw-r--r--   0        0        0      820 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/flavor_options.py
--rw-r--r--   0        0        0      617 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/goal_options.py
--rw-r--r--   0        0        0      346 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/test_container_options.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/__init__.py
--rw-r--r--   0        0        0      501 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/__init__.py
--rw-r--r--   0        0        0       50 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/api_errors.py
--rw-r--r--   0        0        0     3363 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/build.py
--rw-r--r--   0        0        0     2910 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/build_test_container.py
--rw-r--r--   0        0        0     3120 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/clean.py
--rw-r--r--   0        0        0     3519 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/export.py
--rw-r--r--   0        0        0     1681 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
--rw-r--r--   0        0        0      733 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
--rw-r--r--   0        0        0     3497 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/push.py
--rw-r--r--   0        0        0     3046 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/push_test_container.py
--rw-r--r--   0        0        0     9455 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/run_db_tests.py
--rw-r--r--   0        0        0     3552 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/save.py
--rw-r--r--   0        0        0     3603 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/security_scan.py
--rw-r--r--   0        0        0     4398 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/upload.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
--rw-r--r--   0        0        0     1487 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
--rw-r--r--   0        0        0     1311 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
--rw-r--r--   0        0        0     4219 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
--rw-r--r--   0        0        0     4470 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
--rw-r--r--   0        0        0      525 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
--rw-r--r--   0        0        0     9855 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
--rw-r--r--   0        0        0     1366 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
--rw-r--r--   0        0        0     1736 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
--rw-r--r--   0        0        0     3701 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
--rw-r--r--   0        0        0      756 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
--rw-r--r--   0        0        0     2958 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
--rw-r--r--   0        0        0     1702 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
--rw-r--r--   0        0        0     1600 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
--rw-r--r--   0        0        0      231 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
--rw-r--r--   0        0        0     5728 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
--rw-r--r--   0        0        0      223 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
--rw-r--r--   0        0        0      553 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
--rw-r--r--   0        0        0     1973 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
--rw-r--r--   0        0        0     6871 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
--rw-r--r--   0        0        0     2246 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
--rw-r--r--   0        0        0     1961 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
--rw-r--r--   0        0        0     2840 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
--rw-r--r--   0        0        0     2235 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
--rw-r--r--   0        0        0     3179 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
--rw-r--r--   0        0        0     1450 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
--rw-r--r--   0        0        0     8499 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
--rw-r--r--   0        0        0     1420 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
--rw-r--r--   0        0        0     9225 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
--rw-r--r--   0        0        0     1010 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
--rw-r--r--   0        0        0     2663 2024-05-13 11:59:26.333852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
--rw-r--r--   0        0        0     4863 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
--rw-r--r--   0        0        0      630 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
--rw-r--r--   0        0        0     1312 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
--rw-r--r--   0        0        0     1545 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
--rw-r--r--   0        0        0     2995 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
--rw-r--r--   0        0        0      248 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
--rw-r--r--   0        0        0        0 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/utils/__init__.py
--rw-r--r--   0        0        0      922 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/utils/docker_utils.py
--rw-r--r--   0        0        0      915 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
--rwxr-xr-x   0        0        0      278 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/main.py
--rwxr-xr-x   0        0        0      459 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
--rwxr-xr-x   0        0        0     1061 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
--rwxr-xr-x   0        0        0     5629 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
--rwxr-xr-x   0        0        0     2903 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
--rwxr-xr-x   0        0        0     1502 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
--rwxr-xr-x   0        0        0     4495 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
--rw-r--r--   0        0        0     1769 2024-05-13 11:59:26.337852 exasol_script_languages_container_tool-0.18.3/pyproject.toml
--rw-r--r--   0        0        0     8328 1970-01-01 00:00:00.000000 exasol_script_languages_container_tool-0.18.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/LICENSE
+-rw-r--r--   0        0        0     7272 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/__init__.py
+-rw-r--r--   0        0        0      501 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4511 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/build.py
+-rw-r--r--   0        0        0     3231 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py
+-rw-r--r--   0        0        0     3145 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/clean.py
+-rw-r--r--   0        0        0     4539 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/export.py
+-rw-r--r--   0        0        0     1066 2024-05-22 17:45:16.473384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py
+-rw-r--r--   0        0        0     1070 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py
+-rw-r--r--   0        0        0     3759 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/push.py
+-rw-r--r--   0        0        0     3571 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py
+-rw-r--r--   0        0        0    13480 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py
+-rw-r--r--   0        0        0     4251 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/save.py
+-rw-r--r--   0        0        0     4413 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/security_scan.py
+-rw-r--r--   0        0        0     5364 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/upload.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/__init__.py
+-rw-r--r--   0        0        0      820 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/flavor_options.py
+-rw-r--r--   0        0        0      617 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/goal_options.py
+-rw-r--r--   0        0        0      346 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/test_container_options.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/__init__.py
+-rw-r--r--   0        0        0      501 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/api_errors.py
+-rw-r--r--   0        0        0     3363 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/build.py
+-rw-r--r--   0        0        0     2910 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/build_test_container.py
+-rw-r--r--   0        0        0     3120 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/clean.py
+-rw-r--r--   0        0        0     3519 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/export.py
+-rw-r--r--   0        0        0     1681 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py
+-rw-r--r--   0        0        0      733 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py
+-rw-r--r--   0        0        0     3497 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/push.py
+-rw-r--r--   0        0        0     3046 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/push_test_container.py
+-rw-r--r--   0        0        0     9817 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py
+-rw-r--r--   0        0        0     3552 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/save.py
+-rw-r--r--   0        0        0     3603 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/security_scan.py
+-rw-r--r--   0        0        0     4398 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/upload.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/__init__.py
+-rw-r--r--   0        0        0     1487 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py
+-rw-r--r--   0        0        0     1311 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py
+-rw-r--r--   0        0        0     4219 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/clean/__init__.py
+-rw-r--r--   0        0        0     4470 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/__init__.py
+-rw-r--r--   0        0        0      525 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py
+-rw-r--r--   0        0        0     9855 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py
+-rw-r--r--   0        0        0     1366 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py
+-rw-r--r--   0        0        0     1736 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py
+-rw-r--r--   0        0        0     3701 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py
+-rw-r--r--   0        0        0      756 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py
+-rw-r--r--   0        0        0     2958 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/push/__init__.py
+-rw-r--r--   0        0        0     1702 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/save/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py
+-rw-r--r--   0        0        0      231 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save_parameter.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/security_scan/__init__.py
+-rw-r--r--   0        0        0     5728 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py
+-rw-r--r--   0        0        0      223 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan_parameter.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py
+-rw-r--r--   0        0        0     1973 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py
+-rw-r--r--   0        0        0     6878 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py
+-rw-r--r--   0        0        0     2246 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py
+-rw-r--r--   0        0        0     1961 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py
+-rw-r--r--   0        0        0     2840 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py
+-rw-r--r--   0        0        0     2235 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py
+-rw-r--r--   0        0        0     3179 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py
+-rw-r--r--   0        0        0     1450 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py
+-rw-r--r--   0        0        0     8499 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py
+-rw-r--r--   0        0        0     1420 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py
+-rw-r--r--   0        0        0    10721 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py
+-rw-r--r--   0        0        0     1010 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/__init__.py
+-rw-r--r--   0        0        0     2663 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py
+-rw-r--r--   0        0        0     4863 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py
+-rw-r--r--   0        0        0      630 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py
+-rw-r--r--   0        0        0     1312 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py
+-rw-r--r--   0        0        0     1545 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py
+-rw-r--r--   0        0        0     2995 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py
+-rw-r--r--   0        0        0      248 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers_parameter.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/utils/__init__.py
+-rw-r--r--   0        0        0      922 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py
+-rw-r--r--   0        0        0      915 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py
+-rwxr-xr-x   0        0        0      278 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/main.py
+-rwxr-xr-x   0        0        0      459 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/construct_docker_runner_image_name.sh
+-rwxr-xr-x   0        0        0     1061 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh
+-rwxr-xr-x   0        0        0     5629 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh
+-rwxr-xr-x   0        0        0     2903 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh
+-rwxr-xr-x   0        0        0     1502 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh
+-rwxr-xr-x   0        0        0     4495 2024-05-22 17:45:16.477384 exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh
+-rw-r--r--   0        0        0     1264 2024-05-22 17:45:16.481384 exasol_script_languages_container_tool-0.19.0/pyproject.toml
+-rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 exasol_script_languages_container_tool-0.19.0/PKG-INFO
```

### Comparing `exasol_script_languages_container_tool-0.18.3/LICENSE` & `exasol_script_languages_container_tool-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/README.md` & `exasol_script_languages_container_tool-0.19.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
       * [bash](https://www.gnu.org/software/bash/) >= 4.2
     * MacOsX
       * [bash](https://www.gnu.org/software/bash/) > 3.2
     * [coreutils](https://www.gnu.org/software/coreutils/)
       * sha512sum
       * sed
     * [curl](https://curl.se/)
-    * Python 3 (>=3.8)
+    * Python 3 (>=3.10)
       * Pip
 
 
 #### For running
 
 In order to use this tool, your system needs to fulfill the following prerequisites:
```

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/build.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/build_test_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/build_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/clean.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/export.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/push.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/push_test_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/push_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/run_db_tests.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/run_db_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
                 docker_db_image_name: str,
                 db_os_access: str,
                 create_certificates: bool,
                 additional_db_parameter: Tuple[str, ...],
                 external_exasol_db_host: Optional[str],
                 external_exasol_db_port: int,
                 external_exasol_bucketfs_port: int,
+                external_exasol_ssh_port: Optional[int],
                 external_exasol_db_user: Optional[str],
                 external_exasol_db_password: Optional[str],
                 external_exasol_bucketfs_write_password: Optional[str],
                 external_exasol_xmlrpc_host: Optional[str],
                 external_exasol_xmlrpc_port: int,
                 external_exasol_xmlrpc_user: str,
                 external_exasol_xmlrpc_password: Optional[str],
@@ -157,14 +158,15 @@
                                      create_certificates=create_certificates,
                                      additional_db_parameter=additional_db_parameter,
                                      external_exasol_db_host=external_exasol_db_host,
                                      external_exasol_db_port=external_exasol_db_port,
                                      external_exasol_bucketfs_port=external_exasol_bucketfs_port,
                                      external_exasol_db_user=external_exasol_db_user,
                                      external_exasol_db_password=external_exasol_db_password,
+                                     external_exasol_ssh_port=external_exasol_ssh_port,
                                      external_exasol_bucketfs_write_password=external_exasol_bucketfs_write_password,
                                      external_exasol_xmlrpc_host=external_exasol_xmlrpc_host,
                                      external_exasol_xmlrpc_port=external_exasol_xmlrpc_port,
                                      external_exasol_xmlrpc_user=external_exasol_xmlrpc_user,
                                      external_exasol_xmlrpc_password=external_exasol_xmlrpc_password,
                                      external_exasol_xmlrpc_cluster_name=external_exasol_xmlrpc_cluster_name,
                                      db_mem_size=db_mem_size,
```

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/save.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/save.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/security_scan.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/commands/upload.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/flavor_options.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/flavor_options.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/cli/options/goal_options.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/cli/options/goal_options.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/build.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/build_test_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/build_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/clean.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/clean.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/export.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/export.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/generate_language_activation.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/generate_language_activation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/install_starter_scripts.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/push.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/push_test_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/push_test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/run_db_tests.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/run_db_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 from typing import Tuple, Optional
 
 from exasol_integration_test_docker_environment.cli.options.test_environment_options import LATEST_DB_VERSION
 from exasol_integration_test_docker_environment.lib.api.common import run_task, generate_root_task, \
     set_docker_repository_config, set_build_config, import_build_steps, cli_function
 from exasol_integration_test_docker_environment.lib.base.dependency_logger_base_task import DependencyLoggerBaseTask
+from exasol_integration_test_docker_environment.lib.test_environment.parameter.docker_db_test_environment_parameter import \
+    DbOsAccess
 
 from exasol_script_languages_container_tool.lib.api import api_errors
 from exasol_script_languages_container_tool.lib.tasks.test.test_container import TestContainer, AllTestsResult
 from exasol_integration_test_docker_environment.lib.data.environment_type import EnvironmentType
 
 from exasol_script_languages_container_tool.lib.tasks.test.test_container_content import build_test_container_content
 
@@ -26,15 +28,16 @@
                 docker_db_image_version: str = LATEST_DB_VERSION,
                 docker_db_image_name: str = "exasol/docker-db",
                 db_os_access: str = "DOCKER_EXEC",
                 create_certificates: bool = False,
                 additional_db_parameter: Tuple[str, ...] = tuple(),
                 external_exasol_db_host: Optional[str] = None,
                 external_exasol_db_port: int = 8563,
-                external_exasol_bucketfs_port: int = 6583,
+                external_exasol_bucketfs_port: int = 2580,
+                external_exasol_ssh_port: Optional[int] = None,
                 external_exasol_db_user: Optional[str] = None,
                 external_exasol_db_password: Optional[str] = None,
                 external_exasol_bucketfs_write_password: Optional[str] = None,
                 external_exasol_xmlrpc_host: Optional[str] = None,
                 external_exasol_xmlrpc_port: int = 443,
                 external_exasol_xmlrpc_user: str = "admin",
                 external_exasol_xmlrpc_password: Optional[str] = None,
@@ -121,26 +124,28 @@
                                   test_environment_vars=json.loads(test_environment_vars),
                                   test_log_level=test_log_level,
                                   reuse_uploaded_container=reuse_uploaded_container,
                                   environment_type=EnvironmentType[environment_type],
                                   reuse_database_setup=reuse_database_setup,
                                   reuse_test_container=reuse_test_container,
                                   reuse_database=reuse_database,
+                                  db_os_access=DbOsAccess[db_os_access],
                                   no_test_container_cleanup_after_success=reuse_test_container,
                                   no_test_container_cleanup_after_failure=reuse_test_container,
                                   no_database_cleanup_after_success=reuse_database,
                                   no_database_cleanup_after_failure=reuse_database,
                                   docker_db_image_name=docker_db_image_name,
                                   docker_db_image_version=docker_db_image_version,
                                   max_start_attempts=max_start_attempts,
                                   external_exasol_db_host=external_exasol_db_host,
                                   external_exasol_db_port=external_exasol_db_port,
                                   external_exasol_bucketfs_port=external_exasol_bucketfs_port,
                                   external_exasol_db_user=external_exasol_db_user,
                                   external_exasol_db_password=external_exasol_db_password,
+                                  external_exasol_ssh_port=external_exasol_ssh_port,
                                   external_exasol_bucketfs_write_password=external_exasol_bucketfs_write_password,
                                   external_exasol_xmlrpc_host=external_exasol_xmlrpc_host,
                                   external_exasol_xmlrpc_port=external_exasol_xmlrpc_port,
                                   external_exasol_xmlrpc_user=external_exasol_xmlrpc_user,
                                   external_exasol_xmlrpc_password=external_exasol_xmlrpc_password,
                                   external_exasol_xmlrpc_cluster_name=external_exasol_xmlrpc_cluster_name,
                                   create_certificates=create_certificates,
```

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/save.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/save.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/security_scan.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/api/upload.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/api/upload.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_build.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_build_base.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/build/docker_flavor_image_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/clean/clean_images.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/create_export_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_containers.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/export/export_info.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/export/export_info.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/install_starter_scripts/run_starter_script_installation.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/push/docker_push.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/save/docker_save.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/security_scan/security_scan.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/populate_test_engine.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_generic_language_tests.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             file.write(test_output)
             exit_code = exec_run_and_write_to_stream(docker_client, test_container, bash_cmd, file, environment)
         return exit_code
 
     def generate_test_command(self) -> str:
         credentials = f"--user '{self.db_user}' --password '{self.db_password}'"
         log_level = f"--loglevel={self.test_log_level}"
-        server = f"--server '{self._database_info.host}:{self._database_info.db_port}'"
+        server = f"--server '{self._database_info.host}:{self._database_info.ports.database}'"
         environment = "--driver=/downloads/ODBC/lib/linux/x86_64/libexaodbc-uo2214lv2.so  " \
                       "--jdbc-path /downloads/JDBC/exajdbc.jar"
         language_definition = f"--script-languages '{self.language_definition}'"
         language_path = f"--lang-path /tests/lang"
         language = ""
         if self.language is not None:
             language = "--lang %s" % self.language
```

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_files.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_folder.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_in_directory.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_test_result.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_in_test_config.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/run_db_tests_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_container_content.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/test_runner_db_test_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 import pathlib
 from typing import Generator, Any, Dict
 
 import luigi
+from docker.models.containers import ExecResult
+from exasol_integration_test_docker_environment.lib.base.db_os_executor import DbOsExecFactory, SshExecFactory, \
+    DockerClientFactory, DockerExecFactory, DbOsExecutor
+from exasol_integration_test_docker_environment.lib.base.json_pickle_parameter import JsonPickleParameter
+from exasol_integration_test_docker_environment.lib.data.database_info import DatabaseInfo
+from exasol_integration_test_docker_environment.lib.test_environment.parameter.docker_db_test_environment_parameter import \
+    DbOsAccess
+
 from exasol_script_languages_container_tool.lib.tasks.export.export_containers import ExportFlavorContainer
 from exasol_script_languages_container_tool.lib.tasks.export.export_info import ExportInfo
 from exasol_script_languages_container_tool.lib.tasks.test.populate_test_engine import PopulateTestEngine
 from exasol_script_languages_container_tool.lib.tasks.test.run_db_test_result import RunDBTestsInTestConfigResult
 from exasol_script_languages_container_tool.lib.tasks.test.run_db_tests_in_test_config import RunDBTestsInTestConfig
 from exasol_script_languages_container_tool.lib.tasks.test.run_db_tests_parameter import RunDBTestsInTestConfigParameter
 from exasol_script_languages_container_tool.lib.tasks.test.upload_exported_container import UploadExportedContainer
@@ -15,14 +23,34 @@
 from exasol_integration_test_docker_environment.lib.data.environment_info import EnvironmentInfo
 from exasol_integration_test_docker_environment.lib.data.environment_type import EnvironmentType
 from exasol_integration_test_docker_environment.lib.test_environment.parameter.spawn_test_environment_parameter import \
     SpawnTestEnvironmentParameter
 from exasol_integration_test_docker_environment.lib.test_environment.spawn_test_environment import SpawnTestEnvironment
 
 
+class DummyExecutor(DbOsExecutor):
+
+    def exec(self, cmd: str) -> ExecResult:
+        raise RuntimeError("Not supposed to be called.")
+
+    def prepare(self):
+        pass
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, type_, value, traceback):
+        pass
+
+
+class DummyExecFactory(DbOsExecFactory):
+    def executor(self) -> DbOsExecutor:
+        return DummyExecutor()
+
+
 class TestRunnerDBTestTask(FlavorBaseTask,
                            SpawnTestEnvironmentParameter,
                            RunDBTestsInTestConfigParameter):
     reuse_uploaded_container = luigi.BoolParameter(False, significant=False)
     release_goal = luigi.Parameter()
 
     def __init__(self, *args, **kwargs):
@@ -59,27 +87,37 @@
         database_credentials = self.get_database_credentials()
         yield from self.upload_container(database_credentials,
                                          export_info)
         yield from self.populate_test_engine_data(self.test_environment_info, database_credentials)
         test_results = yield from self.run_test(self.test_environment_info, export_info)
         self.return_object(test_results)
 
+    def _executor_factory(self, database_info: DatabaseInfo) -> DbOsExecFactory:
+
+        if self.db_os_access == DbOsAccess.SSH:
+            return SshExecFactory.from_database_info(database_info)
+        client_factory = DockerClientFactory(timeout=100000)
+        if database_info.container_info is not None:
+            return DockerExecFactory(database_info.container_info.container_name, client_factory)
+        return DummyExecFactory()
+
     def upload_container(self, database_credentials: DatabaseCredentials, export_info: ExportInfo):
         reuse = \
             self.reuse_database and \
             self.reuse_uploaded_container and \
             not export_info.is_new
         upload_task = self.create_child_task_with_common_params(
             UploadExportedContainer,
             export_info=export_info,
             environment_name=self.test_environment_info.name,
             test_environment_info=self.test_environment_info,
             release_name=export_info.name,
             reuse_uploaded=reuse,
-            bucketfs_write_password=database_credentials.bucketfs_write_password
+            bucketfs_write_password=database_credentials.bucketfs_write_password,
+            executor_factory=self._executor_factory(self.test_environment_info.database_info)
         )
         yield from self.run_dependencies(upload_task)
 
     def populate_test_engine_data(self, test_environment_info: EnvironmentInfo,
                                   database_credentials: DatabaseCredentials) -> None:
         reuse = self.reuse_database_setup and self.test_environment_info.database_info.reused
         if not reuse:
```

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/test/upload_exported_container.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/language_definition.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_base_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_parameter.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_task.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_container_tasks_creator.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/tasks/upload/upload_containers.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/utils/docker_utils.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/lib/utils/tar_safe_extract.py`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_install_template.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_slim.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/exaslct_within_docker_container_without_container_build.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh` & `exasol_script_languages_container_tool-0.19.0/exasol_script_languages_container_tool/starter_scripts/mount_point_parsing.sh`

 * *Files identical despite different names*

### Comparing `exasol_script_languages_container_tool-0.18.3/PKG-INFO` & `exasol_script_languages_container_tool-0.19.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: exasol-script-languages-container-tool
-Version: 0.18.3
+Version: 0.19.0
 Summary: Script Languages Container Tool
 Home-page: https://github.com/exasol/script-languages-container-tool
 License: MIT
 Keywords: exasol,udf,script-languages
 Author: Torsten Kilias
 Author-email: torsten.kilias@exasol.com
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docker (>=4.0.0,<7.0.0) ; sys_platform != "win32"
-Requires-Dist: docutils (<=0.20.1)
-Requires-Dist: exasol-integration-test-docker-environment (>=1.7.1,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: exasol-integration-test-docker-environment (>=3.0.0,<4.0.0)
 Requires-Dist: importlib-resources (>=5.4.0)
 Requires-Dist: importlib_metadata (>=4.6.0)
 Requires-Dist: networkx (==2.8.2)
+Requires-Dist: requests (==2.31.0)
 Project-URL: Repository, https://github.com/exasol/script-languages-container-tool
 Description-Content-Type: text/markdown
 
 # Script-Languages-Container-Tool
 
 ## Overview
 
@@ -47,15 +45,15 @@
       * [bash](https://www.gnu.org/software/bash/) >= 4.2
     * MacOsX
       * [bash](https://www.gnu.org/software/bash/) > 3.2
     * [coreutils](https://www.gnu.org/software/coreutils/)
       * sha512sum
       * sed
     * [curl](https://curl.se/)
-    * Python 3 (>=3.8)
+    * Python 3 (>=3.10)
       * Pip
 
 
 #### For running
 
 In order to use this tool, your system needs to fulfill the following prerequisites:
```

