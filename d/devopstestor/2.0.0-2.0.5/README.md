# Comparing `tmp/devopstestor-2.0.0.tar.gz` & `tmp/devopstestor-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devopstestor-2.0.0.tar", last modified: Thu Jan 18 16:03:14 2024, max compression
+gzip compressed data, was "devopstestor-2.0.5.tar", last modified: Wed May 22 16:20:53 2024, max compression
```

## Comparing `devopstestor-2.0.0.tar` & `devopstestor-2.0.5.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.487342 devopstestor-2.0.0/
--rw-rw-rw-   0 root         (0) root         (0)    22958 2024-01-18 16:03:00.000000 devopstestor-2.0.0/LICENCE
--rw-rw-rw-   0 root         (0) root         (0)      228 2024-01-18 16:03:00.000000 devopstestor-2.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      908 2024-01-18 16:03:14.486342 devopstestor-2.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      316 2024-01-18 16:03:00.000000 devopstestor-2.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.463342 devopstestor-2.0.0/bin/
--rwxrwxrwx   0 root         (0) root         (0)      405 2024-01-18 16:03:00.000000 devopstestor-2.0.0/bin/devopstestor-presets
--rwxrwxrwx   0 root         (0) root         (0)       89 2024-01-18 16:03:00.000000 devopstestor-2.0.0/bin/devopstestor-saltstack
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.464342 devopstestor-2.0.0/devopstestor/
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.466342 devopstestor-2.0.0/devopstestor/config/
--rw-rw-rw-   0 root         (0) root         (0)     2965 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      323 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/core.yml
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)     1584 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.466342 devopstestor-2.0.0/devopstestor/presets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.467342 devopstestor-2.0.0/devopstestor/presets/saltstack/
--rw-rw-rw-   0 root         (0) root         (0)      251 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)      689 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/build4docker.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.468342 devopstestor-2.0.0/devopstestor/presets/saltstack/config/
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/arguments.yml
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/machine.yml
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/provisionner.yml
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/report.yml
--rw-rw-rw-   0 root         (0) root         (0)      329 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/source_manager.yml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/config/testcase.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.468342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/docker-saltstack
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.458342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.457342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/etc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.457342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/etc/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.468342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/override.conf
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.469342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/tmp/
--rw-rw-rw-   0 root         (0) root         (0)     1053 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.458342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.458342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.458342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.459342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.459342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.469342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.469342 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/
--rw-rw-rw-   0 root         (0) root         (0)      345 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.469342 devopstestor-2.0.0/devopstestor/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.470342 devopstestor-2.0.0/devopstestor/src/abstract/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/abstract/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5424 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/abstract/abstract_machine_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/abstract/abstract_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     3498 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/abstract/abstract_report.py
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/abstract/abstract_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.472342 devopstestor-2.0.0/devopstestor/src/core/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5789 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/devopstestor_client.py
--rw-rw-rw-   0 root         (0) root         (0)     2230 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/devopstestor_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8427 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/global_config_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     8219 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/machines_factory.py
--rw-rw-rw-   0 root         (0) root         (0)     4851 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/ordonnanceur.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/report_render_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     2083 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/source_manager.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/core/testcase_executor_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.473342 devopstestor-2.0.0/devopstestor/src/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/core_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1713 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/json_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/log_manager.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/lib/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.475342 devopstestor-2.0.0/devopstestor/src/machine/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/debug_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     8647 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/docker_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3420 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/docker_no_volume_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/local_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     7265 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/machine/vagrant_controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.476342 devopstestor-2.0.0/devopstestor/src/provisionner/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/provisionner/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/provisionner/empty_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4850 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/provisionner/logstash_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     9335 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/provisionner/minion_provisionner.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/provisionner/systemd_provisionner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.477342 devopstestor-2.0.0/devopstestor/src/reporting/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/campaign_report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/deployment_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/report_elk_renderer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.478342 devopstestor-2.0.0/devopstestor/src/reporting/report_html_renderer/
--rw-rw-rw-   0 root         (0) root         (0)     1487 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/report_html_renderer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9223 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
--rw-rw-rw-   0 root         (0) root         (0)     7258 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/report_text_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/scenario_report.py
--rw-rw-rw-   0 root         (0) root         (0)      552 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/testcase_report.py
--rw-rw-rw-   0 root         (0) root         (0)     1110 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/reporting/verifier_report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.479342 devopstestor-2.0.0/devopstestor/src/scenarios/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/devopstestor.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/logstash.py
--rw-rw-rw-   0 root         (0) root         (0)     6473 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/mock_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/saltastck.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/scenarios/systemd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.480342 devopstestor-2.0.0/devopstestor/src/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/sources/copytemplate_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/sources/dirlink_source_accessor.py
--rw-rw-rw-   0 root         (0) root         (0)     2587 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/sources/git_source_accessor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.481342 devopstestor-2.0.0/devopstestor/src/testcase/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/testcase/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8757 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/testcase/scenario_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     6314 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/testcase/test_case.py
--rw-rw-rw-   0 root         (0) root         (0)     2539 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/testcase/testcase_executor.py
--rw-rw-rw-   0 root         (0) root         (0)     3114 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/src/testcase/tests_cases_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.461342 devopstestor-2.0.0/devopstestor/testconf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.462342 devopstestor-2.0.0/devopstestor/testconf/verifiers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.482342 devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1677 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)      332 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.482342 devopstestor-2.0.0/devopstestor/testconf/verifiers/service/
--rw-rw-rw-   0 root         (0) root         (0)     4529 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/service/http_logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.482342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.482342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/http_logger/
--rw-rw-rw-   0 root         (0) root         (0)     1317 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.483342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/logstash/
--rw-rw-rw-   0 root         (0) root         (0)     5411 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.483342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.483342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.484341 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/packages/
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.484341 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
--rw-rw-rw-   0 root         (0) root         (0)     2256 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.485342 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/users/
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.485342 devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.485342 devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/logstash/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/logstash/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6214 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
--rw-rw-rw-   0 root         (0) root         (0)     4964 2024-01-18 16:03:00.000000 devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/verififier_luncher.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 16:03:14.485342 devopstestor-2.0.0/devopstestor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      908 2024-01-18 16:03:14.000000 devopstestor-2.0.0/devopstestor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5412 2024-01-18 16:03:14.000000 devopstestor-2.0.0/devopstestor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 16:03:14.000000 devopstestor-2.0.0/devopstestor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-01-18 16:03:14.000000 devopstestor-2.0.0/devopstestor.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-01-18 16:03:14.000000 devopstestor-2.0.0/devopstestor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-18 16:03:14.487342 devopstestor-2.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-01-18 16:03:00.000000 devopstestor-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.069990 devopstestor-2.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)    22958 2024-05-22 16:20:40.000000 devopstestor-2.0.5/LICENCE
+-rw-rw-rw-   0 root         (0) root         (0)      228 2024-05-22 16:20:40.000000 devopstestor-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      908 2024-05-22 16:20:53.069990 devopstestor-2.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      316 2024-05-22 16:20:40.000000 devopstestor-2.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.044990 devopstestor-2.0.5/bin/
+-rwxrwxrwx   0 root         (0) root         (0)      405 2024-05-22 16:20:40.000000 devopstestor-2.0.5/bin/devopstestor-presets
+-rwxrwxrwx   0 root         (0) root         (0)       89 2024-05-22 16:20:40.000000 devopstestor-2.0.5/bin/devopstestor-saltstack
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.045990 devopstestor-2.0.5/devopstestor/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.047990 devopstestor-2.0.5/devopstestor/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2965 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/core.yml
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.048990 devopstestor-2.0.5/devopstestor/presets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.048990 devopstestor-2.0.5/devopstestor/presets/saltstack/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)      689 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/build4docker.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.050990 devopstestor-2.0.5/devopstestor/presets/saltstack/config/
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/arguments.yml
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/machine.yml
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/provisionner.yml
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/report.yml
+-rw-rw-rw-   0 root         (0) root         (0)      329 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/source_manager.yml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/config/testcase.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.050990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.038990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.038990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/etc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.038990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/etc/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.050990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/override.conf
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.050990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/tmp/
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.039990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.039990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.039990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.039990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.039990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.050990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.051990 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/presets/saltstack/machine/salt-machine-debian
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.051990 devopstestor-2.0.5/devopstestor/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.052990 devopstestor-2.0.5/devopstestor/src/abstract/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/abstract/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5424 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/abstract/abstract_machine_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/abstract/abstract_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     3498 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/abstract/abstract_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/abstract/abstract_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.054990 devopstestor-2.0.5/devopstestor/src/core/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5789 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/devopstestor_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/devopstestor_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8427 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/global_config_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     8219 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/machines_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4851 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/ordonnanceur.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/report_render_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     2083 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/source_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/core/testcase_executor_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.055990 devopstestor-2.0.5/devopstestor/src/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/core_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1713 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/json_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/log_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.057990 devopstestor-2.0.5/devopstestor/src/machine/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/debug_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)    10096 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/docker_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3420 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/docker_no_volume_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/local_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     7265 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/machine/vagrant_controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.058990 devopstestor-2.0.5/devopstestor/src/provisionner/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/provisionner/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/provisionner/empty_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4850 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/provisionner/logstash_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     9335 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/provisionner/minion_provisionner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/provisionner/systemd_provisionner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.060990 devopstestor-2.0.5/devopstestor/src/reporting/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/campaign_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/deployment_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/report_elk_renderer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.060990 devopstestor-2.0.5/devopstestor/src/reporting/report_html_renderer/
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/report_html_renderer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9223 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja
+-rw-rw-rw-   0 root         (0) root         (0)     7258 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/report_text_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/scenario_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/testcase_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/reporting/verifier_report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.061990 devopstestor-2.0.5/devopstestor/src/scenarios/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/devopstestor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/logstash.py
+-rw-rw-rw-   0 root         (0) root         (0)     6473 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/mock_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/saltastck.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/scenarios/systemd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.062990 devopstestor-2.0.5/devopstestor/src/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/sources/copytemplate_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/sources/dirlink_source_accessor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2587 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/sources/git_source_accessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.063990 devopstestor-2.0.5/devopstestor/src/testcase/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/testcase/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8757 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/testcase/scenario_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     6314 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/testcase/test_case.py
+-rw-rw-rw-   0 root         (0) root         (0)     2539 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/testcase/testcase_executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3114 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/src/testcase/tests_cases_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.041990 devopstestor-2.0.5/devopstestor/testconf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.043990 devopstestor-2.0.5/devopstestor/testconf/verifiers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.064990 devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1677 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/context_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)      332 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/logstash_fixtures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.064990 devopstestor-2.0.5/devopstestor/testconf/verifiers/service/
+-rw-rw-rw-   0 root         (0) root         (0)     4529 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/service/http_logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.065990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.065990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/http_logger/
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.065990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.066990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.066990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.066990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/packages/
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.067990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py
+-rw-rw-rw-   0 root         (0) root         (0)     2256 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.067990 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/users/
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.067990 devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.068990 devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/logstash/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/logstash/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6214 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py
+-rw-rw-rw-   0 root         (0) root         (0)     4964 2024-05-22 16:20:40.000000 devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/verififier_luncher.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:20:53.068990 devopstestor-2.0.5/devopstestor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      908 2024-05-22 16:20:52.000000 devopstestor-2.0.5/devopstestor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5415 2024-05-22 16:20:53.000000 devopstestor-2.0.5/devopstestor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 16:20:52.000000 devopstestor-2.0.5/devopstestor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-22 16:20:52.000000 devopstestor-2.0.5/devopstestor.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-22 16:20:52.000000 devopstestor-2.0.5/devopstestor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 16:20:53.069990 devopstestor-2.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-22 16:20:40.000000 devopstestor-2.0.5/setup.py
```

### Comparing `devopstestor-2.0.0/LICENCE` & `devopstestor-2.0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/PKG-INFO` & `devopstestor-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 2.0.0
+Version: 2.0.5
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-2.0.0/devopstestor/config/arguments.yml` & `devopstestor-2.0.5/devopstestor/config/arguments.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/config/machine.yml` & `devopstestor-2.0.5/devopstestor/config/machine.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/config/report.yml` & `devopstestor-2.0.5/devopstestor/config/report.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/config/testcase.yml` & `devopstestor-2.0.5/devopstestor/config/testcase.yml`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/presets/saltstack/build4docker.bash` & `devopstestor-2.0.5/devopstestor/presets/saltstack/build4docker.bash`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/presets/saltstack/machine/docker-saltstack` & `devopstestor-2.0.5/devopstestor/presets/saltstack/machine/salt-machine-debian`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # syntax=docker/dockerfile:1.3-labs
-# FROM artifactory-registry.forge.diplomatie.gouv.fr/docker-images-core/debian:bullseye-13a82fb127443db94f66a90b3dd1a9f423ac12db
-FROM debian:bullseye-slim
+FROM debian:bookworm-slim
 
 ENV container docker
 ENV LC_ALL C
 ENV DEBIAN_FRONTEND noninteractive
 
 COPY ressources/tmp /tmp/ressources
 
 # run install and cleanup
 RUN bash /tmp/ressources/install_base.bash
-# RUN rm -rf {/tmp/deb,/tmp/ressources} && apt -y autoremove && apt clean
+RUN rm -rf {/tmp/deb,/tmp/ressources} && apt -y autoremove && apt clean
 
 # Mock salt sdb
 COPY ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py /usr/lib/python3/dist-packages/salt/modules/sdb.py
 COPY ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py /usr/lib/python3/dist-packages/salt/runners/sdb.py
 
 # Config saltstack
 COPY ressources/etc/salt/master.d/override.conf /etc/salt/master.d/override.conf
 
 # Start systemd
-CMD ["/lib/systemd/systemd"]
+ENTRYPOINT ["/lib/systemd/systemd"]
```

### Comparing `devopstestor-2.0.0/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash` & `devopstestor-2.0.5/devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/bin/bash
 set -e
 set -o pipefail
 
 ## Preparation du systeme
 apt-get update \
     && apt-get install -y \
-        systemd procps apt iputils-ping netcat
+        systemd procps apt iputils-ping
 
 mkdir /etc/bash_completion.d
 
+
 # pre-requis testauto
-apt -y install python3-pytest python3-testinfra python3-coloredlogs curl python3-dateutil
+apt -y install python3-pytest python3-testinfra python3-coloredlogs curl python3-dateutil python3-pip
 
+python3 -m pip install --break-system-packages devopstestor
 # Mise a jour du system
 apt -y dist-upgrade
 
 # Installation de Saltstack
-mkdir /etc/apt/keyrings
-curl -fsSL -o /etc/apt/keyrings/salt-archive-keyring-2023.gpg https://repo.saltproject.io/salt/py3/debian/11/amd64/SALT-PROJECT-GPG-PUBKEY-2023.gpg
-echo "deb [signed-by=/etc/apt/keyrings/salt-archive-keyring-2023.gpg arch=amd64] https://repo.saltproject.io/salt/py3/debian/11/amd64/latest bullseye main" | tee /etc/apt/sources.list.d/salt.list
+curl -fsSL -o /etc/apt/keyrings/salt-archive-keyring-2023.gpg https://repo.saltproject.io/salt/py3/debian/12/amd64/SALT-PROJECT-GPG-PUBKEY-2023.gpg
+echo "deb [signed-by=/etc/apt/keyrings/salt-archive-keyring-2023.gpg arch=amd64] https://repo.saltproject.io/salt/py3/debian/12/amd64/latest bookworm main" | tee /etc/apt/sources.list.d/salt.list
 apt update
 apt -y install salt-master
 apt -y install salt-minion
 systemctl enable salt-master
 systemctl enable salt-minion
 
 echo 'master: 127.0.0.1' >> /etc/salt/minion
```

### Comparing `devopstestor-2.0.0/devopstestor/src/abstract/abstract_machine_controller.py` & `devopstestor-2.0.5/devopstestor/src/abstract/abstract_machine_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/abstract/abstract_provisionner.py` & `devopstestor-2.0.5/devopstestor/src/abstract/abstract_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/abstract/abstract_report.py` & `devopstestor-2.0.5/devopstestor/src/abstract/abstract_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/abstract/abstract_source_accessor.py` & `devopstestor-2.0.5/devopstestor/src/abstract/abstract_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/devopstestor.py` & `devopstestor-2.0.5/devopstestor/src/core/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/devopstestor_client.py` & `devopstestor-2.0.5/devopstestor/src/core/devopstestor_client.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/devopstestor_server.py` & `devopstestor-2.0.5/devopstestor/src/core/devopstestor_server.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/global_config_factory.py` & `devopstestor-2.0.5/devopstestor/src/core/global_config_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/machines_factory.py` & `devopstestor-2.0.5/devopstestor/src/core/machines_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/ordonnanceur.py` & `devopstestor-2.0.5/devopstestor/src/core/ordonnanceur.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/report_render_manager.py` & `devopstestor-2.0.5/devopstestor/src/core/report_render_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/source_manager.py` & `devopstestor-2.0.5/devopstestor/src/core/source_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/core/testcase_executor_factory.py` & `devopstestor-2.0.5/devopstestor/src/core/testcase_executor_factory.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/lib/config.py` & `devopstestor-2.0.5/devopstestor/src/lib/config.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/lib/core_utils.py` & `devopstestor-2.0.5/devopstestor/src/lib/core_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     Recherche un fichier ou dossier
     :param global_config: instance de configuration global
     :param in_path: chemin a convertir
     :return: chemin absolu si existant
     """
     if os.path.isabs(in_path) and os.path.exists(in_path):
         return in_path  # Le chemin existe deja, il est absolu
-    rel_base_paths = [global_config.get('client_path'), global_config.get('lib_path')]
+    rel_base_paths = [global_config.get('client_path'), global_config.get('lib_path')] + global_config.get('core::other_conf_dirs')
     for base_path in rel_base_paths:
         test_path = os.path.join(base_path, in_path)
         if os.path.exists(test_path):
             return test_path
     raise Exception('file {} not found'.format(in_path))
 
 def import_py_file(global_config, relative_path):
```

### Comparing `devopstestor-2.0.0/devopstestor/src/lib/json_utils.py` & `devopstestor-2.0.5/devopstestor/src/lib/json_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/lib/log_manager.py` & `devopstestor-2.0.5/devopstestor/src/lib/log_manager.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/lib/utils.py` & `devopstestor-2.0.5/devopstestor/src/lib/utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/machine/debug_controller.py` & `devopstestor-2.0.5/devopstestor/src/machine/debug_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/machine/docker_controller.py` & `devopstestor-2.0.5/devopstestor/src/machine/docker_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -33,38 +33,59 @@
         client = docker.from_env()
         dockerfile_path = get_global_path(
             global_config=global_config,
             in_path=machine_configuration.get('dockerfile_path')
         )
         context_path = os.path.dirname(dockerfile_path)
         filename = os.path.basename(dockerfile_path)
-        tag = machine_configuration.get('docker_run_args::image')
-        logger.info('Build config', context_path=context_path, filename=filename, tag=tag)
+        image_name = machine_configuration.get('docker_run_args::image')
+        tag = machine_configuration.get('docker_run_args::tag')
+        logger.info('Build config', context_path=context_path, filename=filename, image_name=image_name, tag=tag)
         build_kwargs = {}
         if global_config.get('machine::proxy') is not False:
             # Activate proxy config in docker build
             proxy_url = global_config.get('machine::proxy')
             build_kwargs['use_config_proxy'] = True 
             if not 'buildargs' in build_kwargs:
                 build_kwargs['buildargs'] = {}            
             build_kwargs['buildargs']['http_proxy'] = proxy_url
             build_kwargs['buildargs']['https_proxy'] = proxy_url
             build_kwargs['buildargs']['HTTP_PROXY'] = proxy_url
             build_kwargs['buildargs']['HTTPS_PROXY'] = proxy_url
 
-        (image, logs) = client.images.build(
-            tag=tag,
-            path=context_path,
-            dockerfile=filename,
-            rm=True,
-            **build_kwargs
-        )
-        for entry in logs:
-            logger.debug(entry.get('stream',str(entry)).rstrip())
-        logger.fin('build', 'Build image fini')
+        # if pull failure, build
+        do_build=True
+        try:
+            logger.info('Trying to pull image ', repository=image_name, tag=tag)
+            pullres = client.images.pull(
+                repository=image_name,
+                tag=tag
+            )
+            do_build=False
+        except docker.errors.APIError as e:
+            logger.error('pull failed', e=str(e))
+        except docker.errors.NotFound as e:
+            logger.error('pull failed NotFound', e=str(e))
+        except Exception as e:
+            logger.error('pull failed', e=str(e))
+        except TypeError as e:
+            logger.error('pull failed', e=str(e))
+
+        if do_build:
+            logger.info('Pull failed, trying to build docker image')
+            (image, logs) = client.images.build(
+                tag=image_name + ':' + tag,
+                path=context_path,
+                dockerfile=filename,
+                rm=True,
+                **build_kwargs
+            )
+            for entry in logs:
+                logger.debug(entry.get('stream',str(entry)).rstrip())
+            logger.fin('build', 'Build image finish')
         logger.debut('network')
         try:
             client.api.inspect_network("testauto")
         except docker.errors.NotFound as e:
             logger.info("Network not exist, create")
             client.api.create_network("testauto", driver="bridge")
         logger.fin('network')
@@ -86,14 +107,27 @@
             config_docker['volumes'] = []
         binds_host_config = {}
         for name, accessor in list(source_manager.get_accessors().items()):          
             self.share_source_accessor(accessor=accessor, config_docker=config_docker, binds_host_config=binds_host_config)
 
         logger.debut("container_"+machine_name, "Creation d'un conteneur", container_name=machine_name, config_docker=config_docker, binds_host_config=binds_host_config)
         config_docker['host_config'] = client.api.create_host_config(binds=binds_host_config, **machine_configuration.config.get('host_config',{}))
+        if global_config.get('machine::proxy') is not False:
+            # Activate proxy config in docker build
+            proxy_url = global_config.get('machine::proxy')     
+            config_docker['environment'] = [
+                'http_proxy='+proxy_url,
+                'https_proxy='+proxy_url,
+                'HTTP_PROXY='+proxy_url,
+                'HTTPS_PROXY='+proxy_url
+            ]
+        # Low level api, tag is in image name
+        config_docker['image'] += ':'+config_docker['tag']
+        del config_docker['tag']
+        
         container_id = client.api.create_container(**config_docker)
         client.api.connect_container_to_network(container=container_id, net_id="testauto")
         self.container = client.containers.get(machine_name)
         self.container.start()
 
     def share_source_accessor(self, accessor:AbstractSourceAccessor, config_docker, binds_host_config, **kwargs):
         """
```

### Comparing `devopstestor-2.0.0/devopstestor/src/machine/docker_no_volume_controller.py` & `devopstestor-2.0.5/devopstestor/src/machine/docker_no_volume_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/machine/local_controller.py` & `devopstestor-2.0.5/devopstestor/src/machine/local_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/machine/vagrant_controller.py` & `devopstestor-2.0.5/devopstestor/src/machine/vagrant_controller.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/provisionner/empty_provisionner.py` & `devopstestor-2.0.5/devopstestor/src/provisionner/empty_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/provisionner/logstash_provisionner.py` & `devopstestor-2.0.5/devopstestor/src/provisionner/logstash_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/provisionner/minion_provisionner.py` & `devopstestor-2.0.5/devopstestor/src/provisionner/minion_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/provisionner/systemd_provisionner.py` & `devopstestor-2.0.5/devopstestor/src/provisionner/systemd_provisionner.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/report_elk_renderer.py` & `devopstestor-2.0.5/devopstestor/src/reporting/report_elk_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/report_html_renderer/__init__.py` & `devopstestor-2.0.5/devopstestor/src/reporting/report_html_renderer/__init__.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja` & `devopstestor-2.0.5/devopstestor/src/reporting/report_html_renderer/html_template.html.jinja`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/report_text_renderer.py` & `devopstestor-2.0.5/devopstestor/src/reporting/report_text_renderer.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/scenario_report.py` & `devopstestor-2.0.5/devopstestor/src/reporting/scenario_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/testcase_report.py` & `devopstestor-2.0.5/devopstestor/src/reporting/testcase_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/reporting/verifier_report.py` & `devopstestor-2.0.5/devopstestor/src/reporting/verifier_report.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/scenarios/devopstestor.py` & `devopstestor-2.0.5/devopstestor/src/scenarios/devopstestor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/scenarios/logstash.py` & `devopstestor-2.0.5/devopstestor/src/scenarios/logstash.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/scenarios/mock_utils.py` & `devopstestor-2.0.5/devopstestor/src/scenarios/mock_utils.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/scenarios/saltastck.py` & `devopstestor-2.0.5/devopstestor/src/scenarios/saltastck.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/scenarios/systemd.py` & `devopstestor-2.0.5/devopstestor/src/scenarios/systemd.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/sources/copytemplate_source_accessor.py` & `devopstestor-2.0.5/devopstestor/src/sources/copytemplate_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/sources/dirlink_source_accessor.py` & `devopstestor-2.0.5/devopstestor/src/sources/dirlink_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/sources/git_source_accessor.py` & `devopstestor-2.0.5/devopstestor/src/sources/git_source_accessor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/testcase/scenario_executor.py` & `devopstestor-2.0.5/devopstestor/src/testcase/scenario_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/testcase/test_case.py` & `devopstestor-2.0.5/devopstestor/src/testcase/test_case.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/testcase/testcase_executor.py` & `devopstestor-2.0.5/devopstestor/src/testcase/testcase_executor.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/src/testcase/tests_cases_loader.py` & `devopstestor-2.0.5/devopstestor/src/testcase/tests_cases_loader.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/context_fixtures.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/context_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/fixtures/saltstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/service/http_logger.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/service/http_logger.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/http_logger/check_requests.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/logstash/test_logstash_IO.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/logstash/test_status_is_green.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/directories_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/files_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/filesystem/symlinks_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/packages/packages_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_down.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/service_is_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/systemd/services_are_up.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/tests/system/users/users_are_present.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/logstash/logstash_manipulator.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor/testconf/verifiers/utils/verififier_luncher.py` & `devopstestor-2.0.5/devopstestor/testconf/verifiers/utils/verififier_luncher.py`

 * *Files identical despite different names*

### Comparing `devopstestor-2.0.0/devopstestor.egg-info/PKG-INFO` & `devopstestor-2.0.5/devopstestor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devopstestor
-Version: 2.0.0
+Version: 2.0.5
 Summary: Framwork to auto test machine provisioning
 Home-page: https://gitlab.com/alexis.porzier.pro/devopstestor
 Author: Alexis PORZIER
 Author-email: alexis.porzier.pro@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
```

### Comparing `devopstestor-2.0.0/devopstestor.egg-info/SOURCES.txt` & `devopstestor-2.0.5/devopstestor.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 devopstestor/presets/saltstack/build4docker.bash
 devopstestor/presets/saltstack/config/arguments.yml
 devopstestor/presets/saltstack/config/machine.yml
 devopstestor/presets/saltstack/config/provisionner.yml
 devopstestor/presets/saltstack/config/report.yml
 devopstestor/presets/saltstack/config/source_manager.yml
 devopstestor/presets/saltstack/config/testcase.yml
-devopstestor/presets/saltstack/machine/docker-saltstack
+devopstestor/presets/saltstack/machine/salt-machine-debian
 devopstestor/presets/saltstack/machine/ressources/etc/salt/master.d/override.conf
 devopstestor/presets/saltstack/machine/ressources/tmp/install_base.bash
 devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/modules/sdb.py
 devopstestor/presets/saltstack/machine/ressources/usr/lib/python3/dist-packages/salt/runners/sdb.py
 devopstestor/src/__init__.py
 devopstestor/src/abstract/__init__.py
 devopstestor/src/abstract/abstract_machine_controller.py
```

### Comparing `devopstestor-2.0.0/setup.py` & `devopstestor-2.0.5/setup.py`

 * *Files identical despite different names*

