# Comparing `tmp/deadline-0.48.1.tar.gz` & `tmp/deadline-0.48.2.tar.gz`

## Comparing `deadline-0.48.1.tar` & `deadline-0.48.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.48.1/THIRD_PARTY_LICENSES
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/_version.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/__main__.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/_version.py
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/exceptions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/py.typed
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_get_storage_profile_for_queue.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_list_apis.py
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_loginout.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_queue_parameters.py
--rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_session.py
--rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_submit_job_bundle.py
--rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/api/_telemetry.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/__init__.py
--rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_common.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_deadline_cli.py
--rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_deadline_web_url.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/deadline_cli_main.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/deadline_dev_gui_main.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/_sigint_handler.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/auth_group.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/bundle_group.py
--rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/config_group.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/farm_group.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/fleet_group.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/handle_web_url_command.py
--rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/job_group.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/queue_group.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/cli/_groups/worker_group.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/config/__init__.py
--rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/config/config_file.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/__init__.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/_yaml.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/adaptors.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/job_template.py
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/loader.py
--rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/parameters.py
--rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/job_bundle/submission.py
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/__init__.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/cli_job_submitter.py
--rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/deadline_authentication_status.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dev_application.py
--rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/job_bundle_submitter.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dataclasses/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/_types.py
--rw-r--r--   0        0        0    34230 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py
--rw-r--r--   0        0        0    29733 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
--rw-r--r--   0        0        0    20978 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/deadline_logo.svg
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/info.svg
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
--rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/__init__.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
--rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/host_requirements_tab.py
--rw-r--r--   0        0        0    15622 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/job_attachments_tab.py
--rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
--rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/path_widgets.py
--rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py
--rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/client/ui/widgets/spinbox_widgets.py
--rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/README.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/__init__.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_utils.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_version.py
--rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_sync.py
--rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/download.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/exceptions.py
--rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/models.py
--rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/os_file_permission.py
--rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/progress_tracker.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/py.typed
--rw-r--r--   0        0        0    52996 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/upload.py
--rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/vfs.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/__init__.py
--rw-r--r--   0        0        0     4423 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/aws_clients.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/aws_config.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_aws/deadline.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_windows/__init__.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/_windows/file.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/base_manifest.py
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/decode.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/manifest_model.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/versions.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
--rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/__init__.py
--rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/cache_db.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/hash_cache.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.48.1/src/deadline/job_attachments/caches/s3_check_cache.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.48.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.48.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.48.1/NOTICE
--rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.48.1/README.md
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.48.1/hatch.toml
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 deadline-0.48.1/pyproject.toml
--rw-r--r--   0        0        0     7935 2020-02-02 00:00:00.000000 deadline-0.48.1/PKG-INFO
+-rw-r--r--   0        0        0    50578 2020-02-02 00:00:00.000000 deadline-0.48.2/THIRD_PARTY_LICENSES
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.2/_version.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/__main__.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/_version.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/exceptions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/py.typed
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_get_storage_profile_for_queue.py
+-rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_list_apis.py
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_loginout.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_queue_parameters.py
+-rw-r--r--   0        0        0    13355 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_session.py
+-rw-r--r--   0        0        0    18628 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_submit_job_bundle.py
+-rw-r--r--   0        0        0    14070 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/api/_telemetry.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/__init__.py
+-rw-r--r--   0        0        0     6214 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_common.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_deadline_cli.py
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_deadline_web_url.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/deadline_cli_main.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/deadline_dev_gui_main.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/_sigint_handler.py
+-rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/auth_group.py
+-rw-r--r--   0        0        0    12509 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/bundle_group.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/config_group.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/farm_group.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/fleet_group.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/handle_web_url_command.py
+-rw-r--r--   0        0        0    39347 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/job_group.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/queue_group.py
+-rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/cli/_groups/worker_group.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/config/__init__.py
+-rw-r--r--   0        0        0    17510 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/config/config_file.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/__init__.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/_yaml.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/adaptors.py
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/job_template.py
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/loader.py
+-rw-r--r--   0        0        0    32688 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/parameters.py
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/job_bundle/submission.py
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/__init__.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/cli_job_submitter.py
+-rw-r--r--   0        0        0     8022 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/deadline_authentication_status.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dev_application.py
+-rw-r--r--   0        0        0     7159 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/job_bundle_submitter.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dataclasses/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/_types.py
+-rw-r--r--   0        0        0    34230 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py
+-rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py
+-rw-r--r--   0        0        0    29733 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py
+-rw-r--r--   0        0        0    21055 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/resources/deadline_logo.svg
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/resources/info.svg
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml
+-rw-r--r--   0        0        0     6139 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/__init__.py
+-rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py
+-rw-r--r--   0        0        0    36343 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/host_requirements_tab.py
+-rw-r--r--   0        0        0    15622 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/job_attachments_tab.py
+-rw-r--r--   0        0        0     5340 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py
+-rw-r--r--   0        0        0    31193 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/path_widgets.py
+-rw-r--r--   0        0        0    23274 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py
+-rw-r--r--   0        0        0     8687 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/client/ui/widgets/spinbox_widgets.py
+-rw-r--r--   0        0        0     6367 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/README.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/__init__.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_utils.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_version.py
+-rw-r--r--   0        0        0    28207 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_sync.py
+-rw-r--r--   0        0        0    46754 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/download.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/exceptions.py
+-rw-r--r--   0        0        0    10785 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/models.py
+-rw-r--r--   0        0        0     7308 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/os_file_permission.py
+-rw-r--r--   0        0        0    15063 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/progress_tracker.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/py.typed
+-rw-r--r--   0        0        0    52996 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/upload.py
+-rw-r--r--   0        0        0    21984 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/vfs.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_aws/__init__.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_aws/aws_clients.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_aws/aws_config.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_aws/deadline.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_windows/__init__.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/_windows/file.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/__init__.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/base_manifest.py
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/decode.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/manifest_model.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/versions.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/__init__.py
+-rw-r--r--   0        0        0     3321 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/caches/__init__.py
+-rw-r--r--   0        0        0     3394 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/caches/cache_db.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/caches/hash_cache.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 deadline-0.48.2/src/deadline/job_attachments/caches/s3_check_cache.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 deadline-0.48.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline-0.48.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline-0.48.2/NOTICE
+-rw-r--r--   0        0        0     6250 2020-02-02 00:00:00.000000 deadline-0.48.2/README.md
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 deadline-0.48.2/hatch.toml
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 deadline-0.48.2/pyproject.toml
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 deadline-0.48.2/PKG-INFO
```

### Comparing `deadline-0.48.1/THIRD_PARTY_LICENSES` & `deadline-0.48.2/THIRD_PARTY_LICENSES`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/exceptions.py` & `deadline-0.48.2/src/deadline/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/__init__.py` & `deadline-0.48.2/src/deadline/client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_get_storage_profile_for_queue.py` & `deadline-0.48.2/src/deadline/client/api/_get_storage_profile_for_queue.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_list_apis.py` & `deadline-0.48.2/src/deadline/client/api/_list_apis.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_loginout.py` & `deadline-0.48.2/src/deadline/client/api/_loginout.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_queue_parameters.py` & `deadline-0.48.2/src/deadline/client/api/_queue_parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_session.py` & `deadline-0.48.2/src/deadline/client/api/_session.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_submit_job_bundle.py` & `deadline-0.48.2/src/deadline/client/api/_submit_job_bundle.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/api/_telemetry.py` & `deadline-0.48.2/src/deadline/client/api/_telemetry.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_common.py` & `deadline-0.48.2/src/deadline/client/cli/_common.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_deadline_cli.py` & `deadline-0.48.2/src/deadline/client/cli/_deadline_cli.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_deadline_web_url.py` & `deadline-0.48.2/src/deadline/client/cli/_deadline_web_url.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/deadline_dev_gui_main.py` & `deadline-0.48.2/src/deadline/client/cli/deadline_dev_gui_main.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/_sigint_handler.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/_sigint_handler.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/auth_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/auth_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/bundle_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/bundle_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,26 +37,35 @@
 @_handle_error
 def cli_bundle():
     """
     Commands to work with Open Job Description job bundles.
     """
 
 
+# Latin alphanumeric, starting with a letter
+_openjd_identifier_regex = r"(?-m:^[A-Za-z_][A-Za-z0-9_]*\Z)"
+
+
 def validate_parameters(ctx, param, value):
     """
-    Validate provided --parameter values, ensuring that they are in the format "Key=Value", and convert them to a dict with the
+    Validate provided --parameter values, ensuring that they are in the format "ParamName=Value", and convert them to a dict with the
     following format:
         [{"name": "<name>", "value": "<value>"}, ...]
     """
     parameters_split = []
     for parameter in value:
-        regex_match = re.match("(.+)=(.*)", parameter)
+        regex_match = re.match("([^=]+)=(.*)", parameter)
         if not regex_match:
             raise click.BadParameter(
-                f'Parameters must be provided in the format "Key=Value". Invalid Parameter: {parameter}'
+                f'Parameters must be provided in the format "ParamName=Value". Invalid parameter: {parameter}'
+            )
+
+        if not re.match(_openjd_identifier_regex, regex_match[1]):
+            raise click.BadParameter(
+                f"Parameter names must be alphanumeric Open Job Description identifiers. Invalid parameter name: {regex_match[1]}"
             )
 
         parameters_split.append({"name": regex_match[1], "value": regex_match[2]})
 
     return parameters_split
```

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/config_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/config_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/farm_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/farm_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/fleet_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/fleet_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/handle_web_url_command.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/handle_web_url_command.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/job_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/job_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/queue_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/queue_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/cli/_groups/worker_group.py` & `deadline-0.48.2/src/deadline/client/cli/_groups/worker_group.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/config/__init__.py` & `deadline-0.48.2/src/deadline/client/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/config/config_file.py` & `deadline-0.48.2/src/deadline/client/config/config_file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/__init__.py` & `deadline-0.48.2/src/deadline/client/job_bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/_yaml.py` & `deadline-0.48.2/src/deadline/client/job_bundle/_yaml.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/adaptors.py` & `deadline-0.48.2/src/deadline/client/job_bundle/adaptors.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/job_template.py` & `deadline-0.48.2/src/deadline/client/job_bundle/job_template.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/loader.py` & `deadline-0.48.2/src/deadline/client/job_bundle/loader.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/parameters.py` & `deadline-0.48.2/src/deadline/client/job_bundle/parameters.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/job_bundle/submission.py` & `deadline-0.48.2/src/deadline/client/job_bundle/submission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/__init__.py` & `deadline-0.48.2/src/deadline/client/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/cli_job_submitter.py` & `deadline-0.48.2/src/deadline/client/ui/cli_job_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/deadline_authentication_status.py` & `deadline-0.48.2/src/deadline/client/ui/deadline_authentication_status.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dev_application.py` & `deadline-0.48.2/src/deadline/client/ui/dev_application.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/job_bundle_submitter.py` & `deadline-0.48.2/src/deadline/client/ui/job_bundle_submitter.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dataclasses/__init__.py` & `deadline-0.48.2/src/deadline/client/ui/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_config_dialog.py` & `deadline-0.48.2/src/deadline/client/ui/dialogs/deadline_config_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dialogs/deadline_login_dialog.py` & `deadline-0.48.2/src/deadline/client/ui/dialogs/deadline_login_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py` & `deadline-0.48.2/src/deadline/client/ui/dialogs/submit_job_progress_dialog.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py` & `deadline-0.48.2/src/deadline/client/ui/dialogs/submit_job_to_deadline_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,14 +381,17 @@
             message = str(exc)
             QMessageBox.warning(self, f"{settings.submitter_name} job submission", message)
 
     def on_submit(self):
         """
         Perform a submission when the submit button is pressed
         """
+        # Unset any cached response
+        self.create_job_response = None
+
         # Retrieve all the settings into the dataclass
         settings = self.job_settings_type()
         self.shared_job_settings.update_settings(settings)
         self.job_settings.update_settings(settings)
 
         queue_parameters = self.shared_job_settings.get_parameters()
```

### Comparing `deadline-0.48.1/src/deadline/client/ui/resources/deadline_logo.svg` & `deadline-0.48.2/src/deadline/client/ui/resources/deadline_logo.svg`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/resources/blender_example_bundle/template.yaml` & `deadline-0.48.2/src/deadline/client/ui/resources/blender_example_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/resources/cli_job_bundle/template.yaml` & `deadline-0.48.2/src/deadline/client/ui/resources/cli_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml` & `deadline-0.48.2/src/deadline/client/ui/resources/controls_demo_job_bundle/template.yaml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/cli_job_settings_tab.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/cli_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/deadline_authentication_status_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/host_requirements_tab.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/host_requirements_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/job_attachments_tab.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/job_attachments_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/job_bundle_settings_tab.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/job_bundle_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/openjd_parameters_widget.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/openjd_parameters_widget.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/path_widgets.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/path_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/shared_job_settings_tab.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/shared_job_settings_tab.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/client/ui/widgets/spinbox_widgets.py` & `deadline-0.48.2/src/deadline/client/ui/widgets/spinbox_widgets.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/README.md` & `deadline-0.48.2/src/deadline/job_attachments/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/_utils.py` & `deadline-0.48.2/src/deadline/job_attachments/_utils.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_sync.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_sync.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/download.py` & `deadline-0.48.2/src/deadline/job_attachments/download.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/exceptions.py` & `deadline-0.48.2/src/deadline/job_attachments/exceptions.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/models.py` & `deadline-0.48.2/src/deadline/job_attachments/models.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/os_file_permission.py` & `deadline-0.48.2/src/deadline/job_attachments/os_file_permission.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/progress_tracker.py` & `deadline-0.48.2/src/deadline/job_attachments/progress_tracker.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/upload.py` & `deadline-0.48.2/src/deadline/job_attachments/upload.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/vfs.py` & `deadline-0.48.2/src/deadline/job_attachments/vfs.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/_aws/aws_clients.py` & `deadline-0.48.2/src/deadline/job_attachments/_aws/aws_clients.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 """Functions for handling and retrieving AWS clients."""
 from __future__ import annotations
 
 from functools import lru_cache
 from typing import Optional
 
 import boto3
+from boto3.s3.transfer import create_crt_transfer_manager, create_transfer_manager
+
 import botocore
-from boto3.s3.transfer import create_transfer_manager
 from botocore.client import BaseClient, Config
 
 from deadline.client.config import config_file
 
 from .. import version
 from ..exceptions import AssetSyncError
 from .aws_config import (
@@ -100,14 +101,21 @@
         )
     return s3_max_pool_connections
 
 
 @lru_cache(maxsize=MAX_SIZE_CACHE)
 def get_s3_transfer_manager(s3_client: BaseClient):
     transfer_config = boto3.s3.transfer.TransferConfig()
+
+    crt_transfer_manager = create_crt_transfer_manager(client=s3_client, config=transfer_config)
+    if crt_transfer_manager:
+        return crt_transfer_manager
+
+    # Fallback to regular transfer manager if CRT transfer manager does not support the configuration, which can happen if the client
+    # and bucket are in different regions.
     return create_transfer_manager(client=s3_client, config=transfer_config)
 
 
 @lru_cache(maxsize=MAX_SIZE_CACHE)
 def get_sts_client(session: Optional[boto3.session.Session] = None) -> BaseClient:
     """
     Get a boto3 sts client to make API calls to STS.
```

### Comparing `deadline-0.48.1/src/deadline/job_attachments/_aws/deadline.py` & `deadline-0.48.2/src/deadline/job_attachments/_aws/deadline.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/_windows/file.py` & `deadline-0.48.2/src/deadline/job_attachments/_windows/file.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/__init__.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/__init__.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/_canonical_json.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/_canonical_json.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/base_manifest.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/base_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/decode.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/decode.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/hash_algorithms.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/hash_algorithms.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/manifest_model.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/manifest_model.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/schemas/2023-03-03.json`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py` & `deadline-0.48.2/src/deadline/job_attachments/asset_manifests/v2023_03_03/asset_manifest.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/caches/cache_db.py` & `deadline-0.48.2/src/deadline/job_attachments/caches/cache_db.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/caches/hash_cache.py` & `deadline-0.48.2/src/deadline/job_attachments/caches/hash_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/src/deadline/job_attachments/caches/s3_check_cache.py` & `deadline-0.48.2/src/deadline/job_attachments/caches/s3_check_cache.py`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/LICENSE` & `deadline-0.48.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/README.md` & `deadline-0.48.2/README.md`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/hatch.toml` & `deadline-0.48.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline-0.48.1/pyproject.toml` & `deadline-0.48.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   "Topic :: Software Development :: Libraries"
 ]
 
 # Note: All deps should be using >= since this is a *library* as well as an application.
 # Applications that consume this library should be the ones that are more strictly
 # limiting dependencies if they want/need to.
 dependencies = [
-    "boto3 >= 1.34.75",
+    "boto3[crt] >= 1.34.75",
     "click >= 8.1.7",
     "pyyaml >= 6.0",
     # Job Attachments
     "typing_extensions >= 4.7,< 4.12; python_version == '3.7'",
     "typing_extensions >= 4.8; python_version > '3.7'",
     # Pinning due to 3.4 not being available upstream
     "xxhash == 3.4.*",
```

### Comparing `deadline-0.48.1/PKG-INFO` & `deadline-0.48.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline
-Version: 0.48.1
+Version: 0.48.2
 Summary: Multi-purpose library and command line tool that implements functionality to support applications using AWS Deadline Cloud.
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
-Requires-Dist: boto3>=1.34.75
+Requires-Dist: boto3[crt]>=1.34.75
 Requires-Dist: click>=8.1.7
 Requires-Dist: jsonschema==4.17.*
 Requires-Dist: pywin32==306; sys_platform == 'win32'
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: qtpy==2.4.*
 Requires-Dist: typing-extensions<4.12,>=4.7; python_version == '3.7'
 Requires-Dist: typing-extensions>=4.8; python_version > '3.7'
```

